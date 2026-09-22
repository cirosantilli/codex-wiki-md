<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $w_k=C_k^{-1}$, $u_i=H_i^{-1}$, $A=\sum_kw_k$, $B=\sum_i u_i$, and form the [weighted means](../../../../../../weighted-arithmetic-mean.md)

$$
\bar q_w=\frac{\sum_kw_kq_k}{A},
\qquad
\bar r_u=\frac{\sum_i u_ir_i}{B}.
$$

The two equations obtained from the [score function](../../../../../../informant-function.md) are

$$
A(\bar q_w-M_0)+B(\bar r_u-M_0+\theta)=0,
\qquad
-B(\bar r_u-M_0+\theta)=0.
$$

Consequently the [maximum-likelihood estimators](../../../../../../maximum-likelihood-estimator.md) are

$$
\boxed{\widehat M_0=\bar q_w,
\qquad \widehat\theta=\bar q_w-\bar r_u.}
$$

The [Hessian matrix](../../../../../../hessian-matrix.md) of the log likelihood is

$$
\begin{pmatrix}-(A+B)&B\\B&-B\end{pmatrix}.
$$

Its first leading principal minor is negative and its [determinant](../../../../../../determinant.md) is $AB>0$, so it is a [negative-definite matrix](../../../../../../negative-definite-matrix.md). Thus the stationary point is the unique global maximum.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
