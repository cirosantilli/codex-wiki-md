<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

A [Mehrstellen method](../../../../../mehrstellen-method.md) gains accuracy by exploiting the [differential equation](../../../../../differential-equation-split.md) in the [local truncation error](../../../../../local-truncation-error.md) of a compact [finite difference method](../../../../../finite-difference-method.md) stencil. The extra nearby values alone do not guarantee higher order: one must also modify the source term. Consider $\Delta u=f$ on a square with prescribed [Dirichlet boundary data](../../../../../dirichlet-boundary-data.md), using the same spacing $h$ in both directions.

For comparison, the [five-point Laplacian](../../../../../five-point-laplacian.md) has expansion

$$
D_5u=\Delta u+\frac{h^2}{12}(u_{xxxx}+u_{yyyy})+O(h^4).
$$

Its leading error is not a multiple of $\Delta^2u$, because the mixed fourth [derivative](../../../../../derivative.md) is missing. To obtain an isotropic leading error, consider a symmetric [nine-point finite-difference stencil](../../../../../nine-point-finite-difference-stencil.md) with weight $a$ on each axial neighbor, $b$ on each diagonal neighbor, and $c$ on the center, all divided by $h^2$. Vanishing on constants and [consistency of a numerical method](../../../../../consistency-of-a-numerical-method.md) require $4a+4b+c=0$ and $a+2b=1$. [Taylor expansion](../../../../../taylor-expansion.md) then gives the fourth-derivative contribution

$$
h^2\left[\frac1{12}(u_{xxxx}+u_{yyyy})+b\,u_{xxyy}\right].
$$

For this to equal $h^2\Delta^2u/12$ we must choose $b=1/6$, hence $a=2/3$, $c=-10/3$. The resulting [nine-point finite-difference stencil](../../../../../nine-point-finite-difference-stencil.md) operator is

$$
D_9U_{ij}=\frac{4(U_{i+1,j}+U_{i-1,j}+U_{i,j+1}+U_{i,j-1})
+U_{i+1,j+1}+U_{i+1,j-1}+U_{i-1,j+1}+U_{i-1,j-1}-20U_{ij}}{6h^2}.
$$

Its expansion, retaining the next term for later use, is

$$
D_9u=\Delta u+\frac{h^2}{12}\Delta^2u
+\frac{h^4}{360}\bigl(u_{xxxxxx}+u_{yyyyyy}+5u_{xxxxyy}+5u_{xxyyyy}\bigr)+O(h^6).
$$

Thus $D_9$ by itself is second order on a general function. On a [Poisson equation](../../../../../poisson-equation.md) solution, however, $\Delta^2u=\Delta f$. Approximating this known source [derivative](../../../../../derivative.md) by $D_5f$ gives the fourth-order [Mehrstellen method](../../../../../mehrstellen-method.md) equation

$$
\boxed{D_9U_{ij}=f_{ij}+\frac{h^2}{12}D_5f_{ij}
=\frac23f_{ij}+\frac1{12}(f_{i+1,j}+f_{i-1,j}+f_{i,j+1}+f_{i,j-1}).}
$$

Equivalently, its two stencils are

$$
\frac1{6h^2}\begin{pmatrix}1&4&1\\4&-20&4\\1&4&1\end{pmatrix}U
=\frac1{12}\begin{pmatrix}0&1&0\\1&8&1\\0&1&0\end{pmatrix}f.
$$

The normalized [local truncation error](../../../../../local-truncation-error.md) is $O(h^4)$, since $D_5f-\Delta f=O(h^2)$. If the equation is multiplied by $6h^2$, the row residual is $O(h^6)$; this change of normalization does not make the solution sixth order. The [fourth-order correction of the nine-point Poisson stencil](../../../../../fourth-order-correction-of-the-nine-point-poisson-stencil.md) retains only the closest axial and diagonal unknowns. A fourth-order one-dimensional second [derivative](../../../../../derivative.md) instead uses $( -U_{i+2}+16U_{i+1}-30U_i+16U_{i-1}-U_{i-2})/(12h^2)$, widening the unknown stencil and introducing negative outer weights. [Mehrstellen method](../../../../../mehrstellen-method.md) accuracy is obtained by correcting known source values rather than widening that unknown stencil.

The compact scheme has useful [stability](../../../../../stability-of-a-numerical-method.md) and solvability properties. With homogeneous [Dirichlet boundary data](../../../../../dirichlet-boundary-data.md), $-D_9$ is symmetric, has positive diagonal and nonpositive off-diagonal entries, and is a [positive definite symmetric operator](../../../../../positive-definite-symmetric-operator.md). Indeed its [quadratic form](../../../../../quadratic-form.md) is a sum of positive edge weights times squared differences, with boundary values set to zero. Vanishing of this sum would force a constant on the connected grid and then zero by connection to the boundary. Consequently the [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md) [linear system](../../../../../system-of-linear-equations.md) has a unique solution. The same weights give a [discrete maximum principle](../../../../../discrete-maximum-principle.md): if $D_9v\ge0$ at every interior node and $v\le0$ on the boundary, a positive maximum inside would make every weighted difference to its neighbors nonpositive. Equality forces the maximum to propagate to the boundary, which is impossible. Thus $v\le0$ everywhere.

This also turns [consistency of a numerical method](../../../../../consistency-of-a-numerical-method.md) into a quantitative convergence result, rather than merely suggesting an order. Let $B_hf=f+h^2D_5f/12$, let $\tau=D_9u-B_hf$ be the normalized residual of the exact solution, and set $e=U-u$. Exact [Dirichlet boundary data](../../../../../dirichlet-boundary-data.md) imply $e=0$ on the boundary and $D_9e=-\tau$. On the unit square the quadratic barrier

$$
q(x,y)=\frac{x(1-x)+y(1-y)}4
$$

has $D_9q=-1$ exactly, is nonnegative on the boundary, and has maximum $1/8$. If $\|\tau\|_\infty\le\varepsilon$, then $D_9(e-\varepsilon q)\ge0$ and $D_9(-e-\varepsilon q)\ge0$, while both comparison functions are nonpositive on the boundary. The [discrete maximum principle](../../../../../discrete-maximum-principle.md) proves

$$
\boxed{|e_{ij}|\le\varepsilon q(x_i,y_j),\qquad
\|U-u\|_\infty\le\tfrac18\|\tau\|_\infty=O(h^4).}
$$

This is [maximum-norm convergence of the corrected nine-point Poisson scheme](../../../../../maximum-norm-convergence-of-the-corrected-nine-point-poisson-scheme.md). It requires sufficient smoothness of the solution up to the boundary for the uniform truncation bound. On other domains the source and boundary closures must retain the required accuracy; boundary singularities can invalidate a smooth-solution order estimate.

The same expansion reveals how to add still more accuracy. Differentiating $\Delta u=f$ gives

$$
u_{xxxxyy}+u_{xxyyyy}=f_{xxyy},\qquad
u_{xxxxxx}+u_{yyyyyy}=\Delta^2f-3f_{xxyy}.
$$

Thus the sixth [derivatives](../../../../../derivative.md) appearing in the $h^4$ term can also be expressed solely through the source. With exact source [derivatives](../../../../../derivative.md),

$$
D_9U=f+\frac{h^2}{12}\Delta f
+\frac{h^4}{360}(f_{xxxx}+4f_{xxyy}+f_{yyyy})
$$

is the [sixth-order source correction of the nine-point Poisson stencil](../../../../../sixth-order-source-correction-of-the-nine-point-poisson-stencil.md), with normalized residual $O(h^6)$. If source [derivatives](../../../../../derivative.md) are replaced by differences, $\Delta f$ must be approximated through fourth order and the fourth [derivatives](../../../../../derivative.md) through second order to retain that accuracy. The unknowns still occupy the same [nine-point finite-difference stencil](../../../../../nine-point-finite-difference-stencil.md); only evaluation of known source data becomes more elaborate. The same inverse bound yields sixth-order convergence when these approximations and the boundary data have matching accuracy.

A particularly instructive case is the [Laplace equation](../../../../../laplace-equation.md), $f=0$. Both displayed error corrections automatically vanish: $\Delta^2u=0$ and $u_{xxxxyy}+u_{xxyyyy}=\Delta u_{xxyy}=0$, which also makes the pure sixth [derivatives](../../../../../derivative.md) sum to zero. Expanding the stencil two orders further gives, for a sufficiently smooth [harmonic function](../../../../../harmonic-function.md),

$$
\boxed{D_9u=\frac{h^6}{3024}u_{xxxxxxxx}+O(h^8).}
$$

For verification, the three eighth-derivative contributions are $(u_{xxxxxxxx}+u_{yyyyyyyy})/20160$, $(u_{xxxxxxyy}+u_{xxyyyyyy})/2160$ and $u_{xxxxyyyy}/864$. Because $u$ is a [harmonic function](../../../../../harmonic-function.md), their sum is $u_{xxxxxxxx}(1/10080-1/1080+1/864)=u_{xxxxxxxx}/3024$. The example $u=\operatorname{Re}(x+iy)^8$ has $D_9u(0,0)=40h^6/3$, so this term is genuinely present. The unmodified harmonic nine-point scheme therefore has sixth-order nodal convergence under the same smoothness and boundary assumptions. This [harmonic superconvergence of the nine-point stencil](../../../../../harmonic-superconvergence-of-the-nine-point-stencil.md) is special to [harmonic functions](../../../../../harmonic-function.md); it should not be confused with the fourth-order source-corrected scheme for general [Poisson equation](../../../../../poisson-equation.md) data.

The appeal of [Mehrstellenverfahren](../../../../../mehrstellen-method.md) is this combination of a compact [sparse matrix](../../../../../sparse-matrix.md), favorable [discrete maximum principle](../../../../../discrete-maximum-principle.md) properties, and high accuracy obtained by using the governing equation. The derivation also shows precisely which accuracy belongs to the operator on arbitrary functions, which belongs to its action on solutions, and which survives in the computed boundary-value solution.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
