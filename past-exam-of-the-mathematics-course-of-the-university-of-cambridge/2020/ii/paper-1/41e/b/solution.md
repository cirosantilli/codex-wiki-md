<h1 id="41e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put

$$
M=\sum_{i\geq2}a_i^2,
\qquad
c^2=1+\epsilon^2M.
$$

The [Rayleigh quotient](../../../../../../rayleigh-quotient.md) shift is exactly

$$
s_k
=\frac{\lambda_1+\epsilon^2\sum_{i\geq2}a_i^2\lambda_i}
{1+\epsilon^2M}.
$$

Expanding the denominator gives

$$
s_k
=\lambda_1+\epsilon^2
\sum_{i\geq2}a_i^2(\lambda_i-\lambda_1)
+O(\epsilon^4).
$$

The question prints this as $s_k=\lambda_1-K\epsilon^2+O(\epsilon^4)$, so its sign convention requires

$$
\boxed{
K=\sum_{i\geq2}a_i^2(\lambda_1-\lambda_i)<0
}
$$

unless every $a_i$ vanishes. Equivalently, $-K$ is the positive quadratic Rayleigh-quotient error.

The shifted inverse solve has the [spectral decomposition](../../../../../../spectral-decomposition.md)

$$
y=c^{-1}\left[
\frac1{\lambda_1-s_k}w_1
+\epsilon\sum_{i\geq2}
\frac{a_i}{\lambda_i-s_k}w_i
\right].
$$

Only relative coefficients matter after normalization, so factor out $(\lambda_1-s_k)^{-1}$:

$$
y\mathrel\parallel
w_1+\epsilon\sum_{i\geq2}
a_i\frac{\lambda_1-s_k}{\lambda_i-s_k}w_i.
$$

From the shift expansion,

$$
\lambda_1-s_k=K\epsilon^2+O(\epsilon^4),
$$

whereas, for $i\geq2$,

$$
\lambda_i-s_k
=(\lambda_i-\lambda_1)+K\epsilon^2+O(\epsilon^4).
$$

Consequently

$$
\epsilon a_i\frac{\lambda_1-s_k}{\lambda_i-s_k}
=\epsilon^3\frac{Ka_i}{\lambda_i-\lambda_1}
+O(\epsilon^5).
$$

After the final normalization,

$$
\boxed{
x^{(k+1)}=c_1^{-1}\left(
w_1+\epsilon^3\sum_{i\geq2}b_iw_i+O(\epsilon^5)
\right),
\qquad
b_i=\frac{Ka_i}{\lambda_i-\lambda_1}.
}
$$

**Thus an $O(\epsilon)$ eigenvector-direction error becomes $O(\epsilon^3)$ in one step, proving the [Local cubic convergence of Rayleigh quotient iteration](../../../../../../local-cubic-convergence-of-rayleigh-quotient-iteration.md) for this symmetric matrix.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [41E](../../41e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
