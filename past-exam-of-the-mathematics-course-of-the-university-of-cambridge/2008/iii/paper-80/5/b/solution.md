<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\Omega=(0,1)^2$ and $V=H_0^1(\Omega)$, the closure of smooth compactly supported functions in the [Sobolev space](../../../../../../sobolev-space-split.md) $H^1$. Its elements have zero boundary trace. Set

$$
a(v,w)=\int_\Omega\nabla v\cdot\nabla w\,dx,\qquad
\ell(w)=\int_\Omega fw\,dx,\qquad f\in L^2(\Omega).
$$

The form is symmetric and continuous by [Cauchy-Schwarz](../../../../../../cauchy-schwarz-inequality.md). For a smooth function with zero boundary values, $v(x,y)=\int_0^xv_x(s,y)\,ds$ gives $\|v\|_{L^2}\leq\|v_x\|_{L^2}\leq\|\nabla v\|_{L^2}$ after integration. Density extends this [Poincaré inequality](../../../../../../poincare-inequality.md) to $H_0^1$. Therefore the gradient [norm](../../../../../../norm.md) makes $V$ complete and equivalent to its usual $H^1$ [norm](../../../../../../norm.md), with

$$
a(v,v)=\|\nabla v\|_2^2\geq\tfrac12\|v\|_{H^1}^2,\qquad
|\ell(w)|\leq\|f\|_2\|w\|_2\leq\|f\|_2\|\nabla w\|_2.
$$

All the hypotheses of part (a) hold. Green's identity identifies the [weak solution](../../../../../../weak-solution.md) of the [Dirichlet problem](../../../../../../dirichlet-problem.md) as

$$
\boxed{\int_\Omega\nabla u\cdot\nabla w\,dx=\int_\Omega fw\,dx
\quad\text{for every }w\in H_0^1(\Omega).}
$$

For smooth $u$ this is $-\nabla^2u=f$ with zero boundary values; in general it defines the unique [weak solution](../../../../../../weak-solution.md) without requiring pointwise second derivatives.

For the [Ritz method](../../../../../../rayleigh-ritz-method.md), choose a finite-dimensional conforming space $V_h\subset H_0^1(\Omega)$ with basis $\phi_1,\ldots,\phi_N$ and put $u_h=\sum_jU_j\phi_j$. Minimize $I(u_h)$ in the coefficients. Its derivative in each basis direction gives the [finite element method](../../../../../../finite-element-method.md) equations

$$
\boxed{\sum_jK_{ij}U_j=F_i,\qquad
K_{ij}=\int_\Omega\nabla\phi_j\cdot\nabla\phi_i\,dx,\qquad
F_i=\int_\Omega f\phi_i\,dx.}
$$

The [stiffness matrix](../../../../../../stiffness-matrix.md) is symmetric positive definite: for a nonzero coefficient vector $U$, the corresponding basis combination is nonzero and $U^TKU=\|\nabla u_h\|_2^2>0$. Hence the Ritz system has a unique solution.

For example, triangulate the square and use continuous piecewise-affine nodal basis functions at the interior vertices, with boundary vertex values fixed to zero. On a triangle $T$ of area $A_T$, let $\lambda_i$ be its barycentric basis functions. If its counterclockwise vertices are $(x_i,y_i)$, define $\beta_i=y_j-y_k$ and $\chi_i=x_k-x_j$ cyclically. Then $\nabla\lambda_i=(\beta_i,\chi_i)/(2A_T)$, giving the directly assemblable element matrices and loads

$$
\boxed{K_{ij}^{T}=\frac{\beta_i\beta_j+\chi_i\chi_j}{4A_T},\qquad
F_i^{T}=\int_Tf\lambda_i\,dx.}
$$

If $f$ is constant on $T$, $F_i^T=f_TA_T/3$; otherwise integrate or quadrature the load. Assemble by adding element contributions with the same global vertex labels and eliminate prescribed boundary coefficients. Only overlapping basis supports interact, making $K$ sparse. This gives the [Ritz-Galerkin equivalence for a symmetric coercive form](../../../../../../ritz-galerkin-equivalence-for-a-symmetric-coercive-form.md) in a practical finite element form.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
