<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [spectral theorem for real symmetric matrices](../../../../../../spectral-theorem-for-real-symmetric-matrices.md) to write $\Sigma=Q\Lambda Q^T$, with $Q$ orthogonal and $\Lambda=\operatorname{diag}(\lambda_1,\ldots,\lambda_d)$, $\lambda_i\geq0$. Set $L=Q\Lambda^{1/2}$ and generate

$$
\boxed{X=\mu+LZ,\qquad Z=(X_1,\ldots,X_d)^T\sim N_d(0,I).}
$$

Then $LL^T=\Sigma$. The [characteristic function](../../../../../../characteristic-function.md) is

$$
E e^{it^TX}=e^{it^T\mu}E e^{i(L^Tt)^TZ}
=\exp\left(it^T\mu-\tfrac12t^T\Sigma t\right),
$$

which identifies the [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md) $N_d(\mu,\Sigma)$. Equivalently, every linear combination is normal, with the required mean and [variance](../../../../../../variance-split.md). A [Cholesky decomposition](../../../../../../cholesky-decomposition.md) can be used for a [positive-definite matrix](../../../../../../positive-definite-matrix.md). The spectral construction also works for singular $\Sigma$, producing a degenerate [Gaussian distribution](../../../../../../normal-distribution.md) on an [affine subspace](../../../../../../affine-subspace.md); in that case there need not be a density on all of $\mathbb R^d$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
