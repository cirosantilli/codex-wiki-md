<h1 id="29j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because every column of $X$ has [sample mean](../../../../../../sample-mean.md) zero, every column $u_i$ of $U=XV$ also has sample mean zero. The [spectral theorem for real symmetric matrices](../../../../../../spectral-theorem-for-real-symmetric-matrices.md) gives

$$
U^TU=V^TX^TXV=V^T\Sigma V=\Lambda.
$$

Hence for $i\ne j$ the [sample covariance](../../../../../../sample-covariance.md) is $n^{-1}u_i^Tu_j=0$, while the [sample variance](../../../../../../sample-variance.md) of $u_i$ is

$$
\frac1n u_i^Tu_i=\frac{\Lambda_{ii}}n.
$$

**Thus the $u_i$ are pairwise uncorrelated [sample principal components](../../../../../../sample-principal-component.md), ordered by decreasing sample variance.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [29J](../../29j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
