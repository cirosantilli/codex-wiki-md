<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For fixed finite matrices, the [matrix exponential](../../../../../matrix-exponential.md) and a [Taylor expansion](../../../../../taylor-expansion.md) show

$$
S(h)=e^{hA/2}e^{hB}e^{hA/2}
=I+h(A+B)+\frac{h^2}{2}(A^2+AB+BA+B^2)+O(h^3).
$$

This agrees through degree two with $e^{h(A+B)}$, even when $A$ and $B$ do not commute. On a fixed time interval, $\|S(h)\|\leq e^{h(\|A\|+\|B\|)}$ and the telescoping identity

$$
S(h)^N-E(h)^N=\sum_{j=0}^{N-1}S(h)^{N-1-j}\bigl(S(h)-E(h)\bigr)E(h)^j,
\qquad E(h)=e^{h(A+B)},
$$

turns the $O(h^3)$ one-step defect into $O(Nh^3)=O(h^2)$ [global error](../../../../../global-discretization-error.md) for $Nh\leq T$. Hence **Strang splitting is second order** in general; for commuting matrices it is exact.

For the spatial discretization, use $d=2/(M+1)$, $x_m=-1+md$ and the interior vector $U=(u_1,\ldots,u_M)^T$, with $u_0=u_{M+1}=0$. The [central finite differences](../../../../../central-finite-difference.md) give

$$
\boxed{A=\frac1{d^2}\operatorname{tridiag}(1,-2,1),\qquad
B=\frac{\alpha}{2d}\operatorname{tridiag}(-1,0,1).}
$$

Here $\operatorname{tridiag}$ lists lower diagonal, main diagonal and upper diagonal, in that order. Thus $A^T=A$ and $B^T=-B$. Discrete [summation by parts](../../../../../abel-s-summation-formula.md) gives

$$
U^TAU=-\frac1{d^2}\sum_{m=0}^{M}(u_{m+1}-u_m)^2\leq0.
$$

The [matrix exponential](../../../../../matrix-exponential.md) $e^{hA/2}$ is consequently a contraction in the [Euclidean norm](../../../../../euclidean-norm.md), while $e^{hB}$ is an [orthogonal matrix](../../../../../orthogonal-matrix.md) for real $\alpha$. Therefore

$$
\boxed{\|e^{hA/2}e^{hB}e^{hA/2}\|_2\leq1\quad(h\geq0).}
$$

Repeated split steps are contractive in the mesh-weighted norm $d\sum|u_m|^2$, uniformly in the spatial mesh and without a [Courant–Friedrichs–Lewy condition](../../../../../courant-friedrichs-lewy-condition.md). **The split semidiscretization is unconditionally stable.** No commutativity or shared [eigenvectors](../../../../../eigenvector.md) are needed for this [Strang splitting contraction for symmetric diffusion and skew advection](../../../../../strang-splitting-contraction-for-symmetric-diffusion-and-skew-advection.md). Its time-order proof is for fixed spatial matrices; as $d\to0$, commutators can grow, so this [stability](../../../../../stability-of-a-numerical-method.md) result alone is not a uniform-in-mesh second-order error estimate.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
