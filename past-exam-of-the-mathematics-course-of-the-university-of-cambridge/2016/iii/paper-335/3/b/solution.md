<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [singular system of a compact operator](../../../../../../singular-system-of-a-compact-operator.md) consists of positive [singular values](../../../../../../singular-value.md) $\sigma_i$ and [orthonormal](../../../../../../orthonormal-set.md) vectors $v_i\in X$, $u_i\in Y$, with

$$
\boxed{Av_i=\sigma_i u_i,\qquad A^*u_i=\sigma_i v_i.}
$$

The $v_i$ form an [orthonormal basis](../../../../../../orthonormal-basis.md) of $(\ker A)^\perp$, and the $u_i$ form one of $\overline{\operatorname{ran}A}$. There are finitely many positive [singular values](../../../../../../singular-value.md) for finite-rank $A$; otherwise $\sigma_i\to0$. Obtain the system by applying the [spectral theorem for compact self-adjoint operators](../../../../../../spectral-theorem-for-compact-hermitian-operators.md) to $A^*A$, choosing $A^*Av_i=\sigma_i^2v_i$, and setting $u_i=Av_i/\sigma_i$. The [inner product](../../../../../../inner-product.md) identities verify orthonormality and the displayed relations.

With [inner products](../../../../../../inner-product.md) linear in the first argument,

$$
Ax=\sum_i\sigma_i(x,v_i)u_i,\qquad
A^*y=\sum_i\sigma_i(y,u_i)v_i.
$$

The [normal equation for a linear inverse problem](../../../../../../normal-equation-for-a-linear-inverse-problem.md) with the [Tikhonov regularization](../../../../../../tikhonov-regularization.md) penalty acts separately on each $v_i$. Hence the [singular-system Tikhonov filter](../../../../../../singular-system-tikhonov-filter.md) gives **the regularized solution**

$$
\boxed{x_\alpha=\sum_i\frac{\sigma_i}{\sigma_i^2+\alpha}(y,u_i)v_i.}
$$

This norm-convergent series follows from [Bessel's inequality](../../../../../../bessel-s-inequality.md) and the bound $\sigma_i/(\sigma_i^2+\alpha)\leq1/(2\sqrt\alpha)$. Data orthogonal to $\overline{\operatorname{ran}A}$ are annihilated by $A^*$, and the minimizing solution has no component in $\ker A$. The same formula with $y^\delta$ reconstructs noisy data. In contrast, the unregularized inverse would divide $(y,u_i)$ by $\sigma_i$, with convergence governed by the [Picard criterion](../../../../../../picard-criterion.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
