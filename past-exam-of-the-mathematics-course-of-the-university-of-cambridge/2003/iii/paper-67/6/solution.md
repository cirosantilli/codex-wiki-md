<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Consider $-\Delta u=f$ on a rectangle, with prescribed [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md), and assume initially that the solution is smooth up to the boundary. A [finite difference method](../../../../../finite-difference-method.md) chooses grid values as unknowns, approximates the differential operator by a local stencil, incorporates the boundary data, and solves the resulting sparse [linear system](../../../../../system-of-linear-equations.md). Accuracy of a stencil by itself is insufficient: one also needs a well-posed discrete problem, a stability estimate uniform under refinement, and a sufficiently accurate algebraic solve.

For a square grid of spacing $h$, centered second differences give the [five-point Laplacian](../../../../../five-point-laplacian.md)

$$
D_5U_{ij}=\frac{U_{i+1,j}+U_{i-1,j}+U_{i,j+1}+U_{i,j-1}-4U_{ij}}{h^2}.
$$

Expanding each opposite pair in a [Taylor series](../../../../../taylor-series.md) gives

$$
D_5u=\Delta u+\frac{h^2}{12}(u_{xxxx}+u_{yyyy})+O(h^4).
$$

Thus the standard equation $-D_5U=f$ has second-order normalized [local truncation error](../../../../../local-truncation-error.md). Known boundary values move to the right-hand side; they are not iterated as independent unknowns. Nonrectangular geometry requires a consistent boundary approximation rather than silently retaining a full interior stencil outside the domain.

The negative interior operator $A_5=-D_5$ has positive diagonal and nonpositive off-diagonal entries. For a grid vector extended by zero on the boundary,

$$
v^TA_5v=h^{-2}\sum_{\text{grid edges}}(v_i-v_j)^2>0\quad(v\ne0).
$$

The edge sum includes links to the fixed boundary. Connectivity makes the [matrix](../../../../../matrix.md) positive definite, proving uniqueness and providing an energy structure. The same sign pattern gives a [discrete maximum principle](../../../../../discrete-maximum-principle.md): at a negative interior minimum, $A_5v$ is nonpositive. If $A_5v\geq0$ and the boundary is nonnegative, equality can only persist by propagating that minimum through all neighbors to the boundary, a contradiction. Therefore $v\geq0$.

On the unit square, the barrier $b(x,y)=[x(1-x)+y(1-y)]/4$ satisfies $A_5b=1$ exactly. If $e$ has zero boundary values and $A_5e=r$, apply the maximum principle to $\|r\|_\infty b\pm e$ to obtain

$$
\|e\|_\infty\leq\tfrac18\|r\|_\infty.
$$

The bound is independent of $h$, so the $O(h^2)$ consistency error gives an $O(h^2)$ nodal error. It also separates the algebraic residual from the discretization error: solving the [linear system](../../../../../system-of-linear-equations.md) much less accurately than $h^2$ would spoil the spatial accuracy.

A direct higher-order design is possible. In one coordinate,

$$
u_{xx}(x)\approx\frac{-u(x+2h)+16u(x+h)-30u(x)+16u(x-h)-u(x-2h)}{12h^2}
$$

has fourth-order accuracy. Adding the corresponding formula in the other coordinate gives a wider stencil. Its advantages must be balanced against boundary closures, more distant couplings, and the possible loss of monotonicity. Higher order does not automatically imply a stable or geometrically convenient scheme.

The [Mehrstellen method](../../../../../mehrstellen-method.md) takes a different route: it uses the [Poisson equation](../../../../../poisson-equation.md) to eliminate leading truncation derivatives while keeping a compact unknown stencil. Define the [nine-point finite-difference stencil](../../../../../nine-point-finite-difference-stencil.md)

$$
D_9U=\frac{4\sum_{\mathrm{axial}}U+\sum_{\mathrm{diagonal}}U-20U_{ij}}{6h^2}.
$$

Here each sum has four terms. Equivalently $D_9=D_5+(h^2/6)\delta_{xx}\delta_{yy}$. Expanding gives

$$
D_9u=\Delta u+\frac{h^2}{12}(u_{xxxx}+2u_{xxyy}+u_{yyyy})+O(h^4)
=\Delta u+\frac{h^2}{12}\Delta^2u+O(h^4).
$$

The uncorrected nine-point operator is only second order for a general function. But $-\Delta u=f$ implies $\Delta^2u=-\Delta f$. Moving this known leading defect to the source and approximating its Laplacian with $D_5$ gives

$$
\boxed{-D_9U=f+\frac{h^2}{12}D_5f,\qquad\text{fourth-order normalized residual}.}
$$

Indeed $D_5f=\Delta f+O(h^2)$, and multiplication by $h^2$ makes that replacement's error fourth order. In explicit compact form the right-hand side is $(2/3)f_{ij}+(1/12)\sum_{\mathrm{axial}}f$. Only known source samples, not additional distant solution unknowns, enter this correction. The corresponding unscaled stencil residual is $O(h^6)$. If $f=0$, the leading term already vanishes, which explains [harmonic superconvergence of the nine-point stencil](../../../../../harmonic-superconvergence-of-the-nine-point-stencil.md).

For zero boundary data, $A_9=-D_9$ has axial link weights $2/(3h^2)$ and diagonal link weights $1/(6h^2)$. Their energy sum proves positive definiteness, and their sign pattern again proves the [discrete maximum principle](../../../../../discrete-maximum-principle.md). The same quadratic barrier is exact for $A_9$, so

$$
\|e\|_\infty\leq\tfrac18\|A_9e\|_\infty.
$$

For smooth solutions and accurately imposed boundary values this proves fourth-order nodal convergence of the corrected scheme. Singular corners, rough sources or low-order boundary treatment can reduce the observed rate; a formal interior expansion is not a global regularity theorem.

More generally, compact high-order schemes choose a solution stencil and a source stencil together, match their [Taylor expansions](../../../../../taylor-expansion.md), and use differentiated forms of the PDE to remove derivatives that would otherwise need a wide solution stencil. Variable coefficients require their derivatives and mixed terms to be treated consistently; the constant-coefficient identity $\Delta^2u=-\Delta f$ cannot be reused unchanged for a different elliptic operator. On irregular meshes, conservation and consistent fluxes may be more useful starting points than a symmetric Cartesian formula.

Finally, discretization and solution cost are coupled. The five-point Dirichlet [matrix](../../../../../matrix.md) has [eigenvalues](../../../../../eigenvalue.md) proportional to sums of squared sine frequencies, so its smallest [eigenvalue](../../../../../eigenvalue.md) stays of order one while its largest is $O(h^{-2})$. Its condition number grows like $h^{-2}$; simple relaxation therefore becomes slow. Sparse direct elimination, [Conjugate gradient method](../../../../../conjugate-gradient-method.md) with appropriate [matrix preconditioning](../../../../../matrix-preconditioning.md), and the [multigrid method](../../../../../multigrid-method.md) are alternatives. A sound design combines local accuracy, boundary fidelity, mesh-independent stability, and an algebraic solver whose residual is small enough for the intended error tolerance.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 67](../../paper-67-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
