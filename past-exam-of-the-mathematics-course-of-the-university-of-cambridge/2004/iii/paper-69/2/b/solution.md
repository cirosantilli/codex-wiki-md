<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $r=k/h^2$. The update is

$$
U_m^{n+1}=r a_{m-1/2}U_{m-1}^n+[1-r(a_{m-1/2}+a_{m+1/2})]U_m^n+r a_{m+1/2}U_{m+1}^n.
$$

Under $k\le h^2/(2\beta)$, all three weights are nonnegative and sum to one. With the imposed zero [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md), this is a [convex combination](../../../../../../convex-combination.md) including any boundary values. Thus the [monotone half-grid diffusion update](../../../../../../monotone-half-grid-diffusion-update.md) gives

$$
\boxed{\|U^{n+1}\|_\infty\le\|U^n\|_\infty\le\|U^0\|_\infty}.
$$

Differences of two computed solutions obey the same estimate, proving [numerical stability](../../../../../../stability-of-a-numerical-method.md) in the discrete [maximum norm](../../../../../../supremum-norm.md), uniformly in $h,k,n$.

There is also an [L2 norm](../../../../../../l2-norm.md) proof. The diffusion [matrix](../../../../../../matrix.md) $L_h$ is [symmetric](../../../../../../symmetric-relation.md) and satisfies

$$
v^TL_hv=-h^{-2}\sum_{m=0}^{M-1}a_{m+1/2}(v_{m+1}-v_m)^2,\qquad v_0=v_M=0.
$$

Since $(v_{m+1}-v_m)^2\le2(v_{m+1}^2+v_m^2)$, every [eigenvalue](../../../../../../eigenvalue.md) lies in $[-4\beta/h^2,0]$. Hence the [eigenvalues](../../../../../../eigenvalue.md) of $I+kL_h$ lie in $[-1,1]$ under the same step restriction, and the [spectral theorem for real symmetric matrices](../../../../../../spectral-theorem-for-real-symmetric-matrices.md) gives an [L2 norm](../../../../../../l2-norm.md) contraction. These stability estimates are valid for the printed recurrence, although they cannot repair its inconsistency with the printed [advection equation](../../../../../../transport-equation.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
