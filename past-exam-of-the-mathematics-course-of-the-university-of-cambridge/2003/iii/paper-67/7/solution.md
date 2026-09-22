<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

The [multigrid method](../../../../../multigrid-method.md) addresses a characteristic failure of single-grid relaxation: its cheapest updates rapidly remove oscillatory error but barely change smooth error. For example, the one-dimensional [Poisson equation](../../../../../poisson-equation.md) [matrix](../../../../../matrix.md) has diagonal $2/h^2$. The [weighted Jacobi method](../../../../../weighted-jacobi-method.md) with weight $\omega$ has Fourier error factor

$$
s_\omega(\theta)=1-\omega(1-\cos\theta)=1-2\omega\sin^2(\theta/2).
$$

At low physical frequency, $\theta=O(h)$ and this factor is $1-O(h^2)$, requiring $O(h^{-2})$ sweeps for a fixed error reduction. With $\omega=2/3$, high grid frequencies $\pi/2\leq|\theta|\leq\pi$ are multiplied by at most $1/3$ in modulus. Smooth error on a fine mesh is well represented on a coarser mesh, where it is relatively more oscillatory and hence cheaper to remove. These two complementary mechanisms motivate smoothing and [coarse-grid correction](../../../../../coarse-grid-correction.md).

Write the discrete problem as $A_hu_h=f_h$. For an approximation $v_h$, the residual is $r_h=f_h-A_hv_h$ and the error $e_h=u_h-v_h$ satisfies $A_he_h=r_h$. It is this error equation that is transferred to a coarse grid; restricting the approximate solution alone would not solve the missing error. With prolongation $P$ and restriction $R$, solve

$$
A_He_H=Rr_h,\qquad v_h\leftarrow v_h+Pe_H.
$$

For nested Cartesian grids with $H=2h$, linear interpolation copies a coarse value at a coincident fine node and averages the two nearest coarse values at an intermediate node. Its two-dimensional counterpart is bilinear interpolation. [Full-weighting restriction](../../../../../full-weighting-restriction.md) uses weights $(1,2,1)/4$ in one dimension and

$$
\frac1{16}\begin{pmatrix}1&2&1\\2&4&2\\1&2&1\end{pmatrix}
$$

in two dimensions. With these choices $R=2^{-d}P^T$ in ordinary coordinate inner products. A [Galerkin coarse-grid operator](../../../../../galerkin-coarse-grid-operator.md) is $A_H=RA_hP$; alternatively one can rediscretize the PDE on the coarse mesh when that choice remains compatible with the transfers.

For a symmetric positive-definite fine operator and $R=cP^T$, the exact correction [matrix](../../../../../matrix.md) is

$$
C_h=I-P(RA_hP)^{-1}RA_h.
$$

It satisfies $C_hP=0$ and $P^TA_hC_h=0$. Thus it removes the coarse-space component of the error and is an orthogonal projection in the energy inner product. With pre- and post-smoothing [matrices](../../../../../matrix.md) $S_{\mathrm{pre}},S_{\mathrm{post}}$, the exact two-grid error [matrix](../../../../../matrix.md) is $S_{\mathrm{post}}C_hS_{\mathrm{pre}}$. Effective smoothing on the complementary space and accurate coarse representation of smooth error are both needed for contraction.

A concrete harmonic calculation makes the mechanism quantitative. On the one-dimensional constant-coefficient problem, couple the two harmonics $\theta$ and $\theta+\pi$, put $s=\sin^2(\theta/2)$ and $c=1-s$, and use the above transfers. Linear interpolation has harmonic weights $(c,s)^T$, while the fine operator has diagonal symbol $4\operatorname{diag}(s,c)/h^2$. Therefore its Galerkin correction on this pair is

$$
C=\begin{pmatrix}s&-c\\-s&c\end{pmatrix}.
$$

One pre- and one post-sweep of [weighted Jacobi](../../../../../weighted-jacobi-method.md) with $\omega=2/3$ gives $E=SCS$, $S=\operatorname{diag}(1-4s/3,1-4c/3)$. This rank-one [matrix](../../../../../matrix.md) has [eigenvalues](../../../../../eigenvalue.md) zero and

$$
s(1-4s/3)^2+c(1-4c/3)^2=\frac19.
$$

The [two-grid Poisson factor with weighted Jacobi](../../../../../two-grid-poisson-factor-with-weighted-jacobi.md) is therefore mesh-independent in this model. A periodic constant nullspace must first be removed; a Dirichlet problem has no such nullspace. This is evidence for the design, not a claim that the same factor applies to every PDE or every smoother.

The [geometric multigrid V-cycle](../../../../../geometric-multigrid-v-cycle.md) replaces the exact coarse solve by one recursively defined coarse cycle. A complete implementation on level $\ell$ proceeds as follows:

- On the coarsest level, solve $A_\ell v_\ell=f_\ell$ directly and return.
- Otherwise perform a fixed number $\nu_1$ of pre-smoothing sweeps, for example $v_\ell\leftarrow v_\ell+\omega D_\ell^{-1}(f_\ell-A_\ell v_\ell)$.
- Compute the current residual $r_\ell=f_\ell-A_\ell v_\ell$ and restrict it: $f_{\ell-1}=R_\ell r_\ell$.
- Initialize the coarse error approximation at zero and apply one V-cycle to $A_{\ell-1}e_{\ell-1}=f_{\ell-1}$.
- Prolong and add the correction: $v_\ell\leftarrow v_\ell+P_\ell e_{\ell-1}$.
- Perform $\nu_2$ post-smoothing sweeps and return the improved approximation.

Boundary values of the solution are imposed on the fine level; the error equation has homogeneous boundary conditions when those values were already imposed exactly. Residuals must be computed after pre-smoothing, not before. The zero initialization on each recursive error solve makes the cycle an error correction rather than an accidental addition of an old coarse solution. For an energy-symmetric cycle usable in [Conjugate gradient method](../../../../../conjugate-gradient-method.md), choose compatible adjoint transfers and symmetric smoothing, such as forward Gauss-Seidel before correction and its backward sweep afterward.

With bounded stencil size and fixed sweep counts, a sweep, residual calculation or transfer costs $O(N_\ell)$. Uniform coarsening gives $N_{\ell-1}\approx2^{-d}N_\ell$, so

$$
\boxed{W(N)=O(N)+W(N/2^d)=O(N),\qquad\text{storage }O(N).}
$$

If the full V-cycle has an error reduction factor $q<1$ independent of mesh size, reducing an arbitrary initial algebraic error by a factor $\varepsilon$ takes $O(\log(1/\varepsilon))$ cycles and $O(N\log(1/\varepsilon))$ work. Linear work per cycle alone does not prove the mesh-independent factor; it rests on the smoothing and approximation properties just illustrated. [Full multigrid](../../../../../full-multigrid.md) starts on a coarse mesh, interpolates its solution to each successive finer mesh, and uses a few cycles per level. When the interpolation accuracy and cycle contraction match the discretization error, this reaches discretization-level accuracy in $O(N)$ work.

Performance depends on the operator. Strong anisotropy can leave error oscillatory in one direction but weakly penalized by the differential operator, defeating point smoothing; line or plane relaxation and selective coarsening address this. Large coefficient jumps demand compatible coarse spaces. Nonrectangular meshes motivate algebraic rather than purely geometric coarsening. Nonlinear problems use a full-approximation formulation instead of the linear residual correction verbatim. Singular Neumann or periodic operators need right-hand-side compatibility and consistent nullspace treatment on every level. Multigrid is fast because its components address different error scales, not because coarsening alone guarantees a good solver.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 67](../../paper-67-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
