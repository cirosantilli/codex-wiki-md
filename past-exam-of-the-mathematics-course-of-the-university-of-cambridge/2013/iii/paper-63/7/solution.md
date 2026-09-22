<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

A [stability](../../../../../stability-of-a-numerical-method.md) analysis asks whether perturbations in an evolution remain bounded on a fixed physical time interval by a constant independent of the mesh. For a linear update $U^{n+1}=G_{d,k}U^n$, the basic requirement is

$$
\|G_{d,k}^n\|\leq C_T\quad(nk\leq T).
$$

This permits physical growth bounded by $e^{\omega T}$; it need not require every step to be a contraction. [Consistency of a numerical method](../../../../../consistency-of-a-numerical-method.md) measures how well its stencil reproduces the differential equation, whereas [stability of a numerical method](../../../../../stability-of-a-numerical-method.md) controls the accumulated defects. For a well-posed linear problem, the [Lax equivalence theorem](../../../../../lax-equivalence-theorem.md) connects [stability](../../../../../stability-of-a-numerical-method.md) and convergence for a consistent approximation in the specified norm.

On the whole line or a periodic grid, constant-coefficient stencils commute with translations. The [Fourier modes](../../../../../fourier-mode.md) $e^{ij\theta}$ diagonalize such spatial operators, turning a scalar one-step scheme into

$$
\widehat U^{n+1}(\theta)=g(\theta;d,k)\widehat U^n(\theta).
$$

The [Fourier symbol](../../../../../fourier-symbol-of-a-difference-operator.md) is found simply by replacing a shift by $e^{i\theta}$. The [Parseval identity](../../../../../parseval-identity.md) makes this modal calculation a norm estimate: if $|g(\theta)|\leq1$ at every resolvable frequency, then the discrete $L^2$ norm cannot increase. More generally, a uniform $|g|\leq1+Ck$ gives $|g|^n\leq e^{CT}$ and a fixed-time [stability](../../../../../stability-of-a-numerical-method.md) bound. All frequencies matter, including those near the grid scale; a small-wavenumber expansion establishes consistency but cannot test the entire [stability](../../../../../stability-of-a-numerical-method.md) range.

For the [heat equation](../../../../../heat-equation.md), put $r=k/d^2$ and $s=\sin^2(\theta/2)$. The [Forward Euler diffusion scheme](../../../../../forward-euler-diffusion-scheme.md) has

$$
g_{\rm FE}=1-4rs.
$$

The condition $|g_{\rm FE}|\leq1$ for every $s\in[0,1]$ is exactly $0\leq r\leq1/2$. This illustrates a parabolic time-step restriction $k\leq d^2/2$. The [Backward Euler diffusion scheme](../../../../../backward-euler-diffusion-scheme.md) instead has

$$
g_{\rm BE}=\frac1{1+4rs},
$$

which is contractive for every $r\geq0$. The [Crank-Nicolson diffusion scheme](../../../../../crank-nicolson-diffusion-scheme.md) has

$$
g_{\rm CN}=\frac{1-2rs}{1+2rs},
$$

and is likewise unconditionally $L^2$ stable. However, its high-frequency amplification approaches $-1$ for large $r$, so it need not damp rapidly decaying modes effectively and may produce alternating transients from nonsmooth data. An [A-stable](../../../../../a-stability.md) time integrator can stabilize a diffusion semidiscretization with left-half-plane spectrum, but damping and accuracy remain separate questions.

For transport $u_t+a u_x=0$, define the hyperbolic [Courant number](../../../../../courant-number.md) $\nu=ak/d$. Forward Euler with a centered spatial difference gives $g=1-i\nu\sin\theta$ and $|g|^2=1+\nu^2\sin^2\theta$. It is unstable under a fixed nonzero CFL ratio. For $a>0$, the [upwind finite difference scheme](../../../../../upwind-finite-difference-scheme.md) has

$$
g=1-\nu(1-e^{-i\theta}),\qquad
|g|^2=1-4\nu(1-\nu)\sin^2(\theta/2).
$$

Thus $0\leq\nu\leq1$ is the stable range. Upwinding for negative $a$ reverses the spatial difference and gives $|\nu|\leq1$. The [Lax-Wendroff advection scheme](../../../../../lax-wendroff-advection-scheme.md) gives a second-order example:

$$
g=1-i\nu\sin\theta+\nu^2(\cos\theta-1),\qquad
|g|^2=1-4\nu^2(1-\nu^2)\sin^4(\theta/2).
$$

It is stable for $|\nu|\leq1$, but that $L^2$ result does not imply monotonicity or exclude oscillations at shocks. The [Courant–Friedrichs–Lewy condition](../../../../../courant-friedrichs-lewy-condition.md) has a domain-of-dependence interpretation for explicit hyperbolic schemes; the Fourier calculation supplies the sharper algebraic [stability](../../../../../stability-of-a-numerical-method.md) criterion for the particular stencil.

For multilevel methods, each frequency gives an amplification polynomial and a companion [matrix](../../../../../matrix.md). Every amplification root must lie in the closed unit disk, with unit-modulus roots simple. Uniformity across frequencies and meshes is essential: one also needs control of the associated matrix powers, for example through a uniformly bounded diagonalization or the [uniform power bound from separated amplification roots](../../../../../uniform-power-bound-from-separated-amplification-roots.md). A repeated unit root generates a [Jordan block](../../../../../jordan-block.md) and polynomial growth in the number of steps. The same issue occurs for systems: checking only [eigenvalue](../../../../../eigenvalue.md) moduli of a [nonnormal Fourier amplification matrix](../../../../../nonnormal-fourier-amplification-matrix.md) is insufficient. For instance

$$
G=\begin{pmatrix}1&1\\0&1\end{pmatrix},\qquad
G^n=\begin{pmatrix}1&n\\0&1\end{pmatrix}
$$

has unit [eigenvalues](../../../../../eigenvalue.md) but no fixed-time mesh-uniform bound as $n=T/k\to\infty$. For a [hyperbolic system](../../../../../hyperbolic-system.md) with a constant coefficient matrix admitting a uniformly bounded characteristic diagonalization, scalar modal estimates for each characteristic speed do give a system estimate. A positive energy symmetrizer provides another route. Frozen-coefficient Fourier tests for variable coefficients are useful local diagnostics, but a global estimate must also account for coefficient variation and boundary terms.

Boundary conditions change the allowable modes and can change the conclusion. A periodic calculation is exact only for a periodic closure. On a finite interval with zero [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md), the centered diffusion matrix is diagonalized instead by the [discrete sine transform](../../../../../discrete-sine-transform.md). On $M$ interior points its [eigenvalues](../../../../../eigenvalue.md) are $-4\sin^2(j\pi/[2(M+1)])$ before scaling by $d^{-2}$. Thus the exact fixed-grid Forward Euler restriction is

$$
0\leq r\leq\frac1{2\cos^2(\pi/[2(M+1)])},
$$

which tends to the whole-line threshold $1/2$ as the grid is refined. Backward Euler and Crank-Nicolson remain stable for all nonnegative $r$. An appropriate [Neumann boundary condition](../../../../../neumann-boundary-condition.md) uses cosine-type modes and includes a constant mode with [eigenvalue](../../../../../eigenvalue.md) zero. The constant mode must be preserved, rather than forced to decay; depending on the boundary stencil, the natural discrete inner product may have endpoint weights.

For hyperbolic transport, the continuous and discrete boundary closures must respect the direction of propagation. If $a>0$ on $[0,L]$, prescribe the left inflow value; prescribing an independent outflow value can overdetermine the problem. The [energy method](../../../../../energy-method.md) exposes this directly:

$$
\frac12\frac d{dt}\int_0^L u^2\,dx
=-\frac a2\bigl(u(L)^2-u(0)^2\bigr).
$$

Homogeneous inflow is dissipative, while forced inflow contributes data to the estimate. A compatible upwind boundary update has the same one-sided information flow. For diffusion,

$$
\frac12\frac d{dt}\int_0^L u^2\,dx
=-\int_0^L u_x^2\,dx+[uu_x]_0^L.
$$

The last term vanishes for homogeneous Dirichlet or Neumann conditions. With [Robin boundary conditions](../../../../../robin-boundary-condition.md) of dissipative sign it contributes a further nonpositive term. A non-dissipative boundary can produce genuine PDE growth, which a valid [stability](../../../../../stability-of-a-numerical-method.md) estimate should represent rather than incorrectly suppress.

Even a perfectly stable interior symbol cannot detect every defective [boundary closure of a difference scheme](../../../../../boundary-closure-of-a-difference-scheme.md). As a concrete counterexample, leave a stable explicit heat stencil on all grid points away from the left endpoint, but replace its first interior row by $U_1^{n+1}=2U_1^n$, still keeping $U_0=0$. The interior Fourier symbol is unchanged, yet $U_1^n=2^nU_1^0$ makes the finite-interval update unstable. The faulty boundary-adjacent row creates a mode absent from the periodic interior calculation. Thus the entire finite update matrix, or an energy estimate including its boundary rows, must be examined.

A more systematic [boundary stability of a finite-difference method](../../../../../boundary-stability-of-a-finite-difference-method.md) analysis transforms time and any tangential spatial variables, then looks for modes $U_j^n=z^n\kappa^j$ with $|z|>1$ and $|\kappa|<1$ on a half-line. The interior dispersion relation selects decaying spatial modes; the boundary equations must determine their coefficients without admitting a nonzero growing homogeneous mode. A uniform inverse estimate for the boundary system, expressed by the [Uniform Kreiss--Lopatinskii condition](../../../../../uniform-kreiss-lopatinskii-condition.md), also rules out arbitrarily weak boundary control near limiting frequencies. Merely excluding one obvious unstable mode is weaker than proving a mesh-uniform estimate. Discrete [summation by parts](../../../../../abel-s-summation-formula.md) and suitable boundary penalties offer an energy-based alternative.

Finally, nonlinear [scalar conservation laws](../../../../../scalar-conservation-law.md) can develop discontinuities, so linearized Fourier [stability](../../../../../stability-of-a-numerical-method.md) is only one part of the analysis. A [monotone conservative scheme](../../../../../monotone-conservative-scheme.md), such as the [Engquist-Osher method](../../../../../engquist-osher-method.md) under its CFL restriction, has an invariant state range and [L1 contraction of a monotone conservative scheme](../../../../../l1-contraction-of-a-monotone-conservative-scheme.md), with a [discrete entropy inequality](../../../../../discrete-entropy-inequality.md) selecting admissible shocks. These complement the Fourier and boundary estimates. For an evolution problem, the meaningful outcome is a [stability](../../../../../stability-of-a-numerical-method.md) bound in a specified norm, uniform over the chosen mesh family and compatible with the actual boundary and initial data.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
