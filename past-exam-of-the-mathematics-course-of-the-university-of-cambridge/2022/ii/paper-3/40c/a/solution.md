<h1 id="40c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [power method](../../../../../../power-method.md) starts with a unit vector $\mathbf x_0$ and iterates

$$
\mathbf x_{k+1}
=\frac{A\mathbf x_k}{\|A\mathbf x_k\|}.
$$

Its eigenvalue estimate is the [Rayleigh quotient](../../../../../../rayleigh-quotient.md)

$$
r(\mathbf x_k)
=\frac{\mathbf x_k^TA\mathbf x_k}
{\mathbf x_k^T\mathbf x_k}.
$$

By the [real spectral theorem](../../../../../../real-spectral-theorem.md), choose an orthonormal eigenbasis $\mathbf v_1,\ldots,\mathbf v_n$ and write

$$
\mathbf x_0=\sum_{j=1}^nc_j\mathbf v_j.
$$

Assume $|\lambda_1|>|\lambda_2|$, $\lambda_1\ne0$, and $c_1\ne0$. Before normalization,

$$
A^k\mathbf x_0
=c_1\lambda_1^k
\left[
\mathbf v_1
+\sum_{j=2}^n
\frac{c_j}{c_1}
\left(\frac{\lambda_j}{\lambda_1}\right)^k
\mathbf v_j
\right].
$$

Thus the direction error is $O(|\lambda_2/\lambda_1|^k)$. Orthogonality makes the linear terms vanish from the Rayleigh quotient:

$$
r(\mathbf x_k)-\lambda_1
=
\frac{
\sum_{j=2}^nc_j^2\lambda_j^{2k}(\lambda_j-\lambda_1)
}{
\sum_{j=1}^nc_j^2\lambda_j^{2k}
}.
$$

Consequently

$$
\boxed{
r(\mathbf x_k)-\lambda_1
=O\!\left(\left|\frac{\lambda_2}{\lambda_1}\right|^{2k}\right)
}.
$$

This is the [quadratic Rayleigh-quotient improvement for the power method](../../../../../../quadratic-rayleigh-quotient-improvement-for-the-power-method.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [40C](../../40c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
