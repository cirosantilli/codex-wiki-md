<h1 id="5i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the [hat matrix](../../../../../../hat-matrix.md) $H=X(X^TX)^{-1}X^T$. It is symmetric and idempotent, the [orthogonal projection](../../../../../../orthogonal-projection.md) onto the column space of $X$. Since $HX=X$,

$$
\widehat Y=HY=X\beta+H\epsilon,\qquad
\boxed{\widehat Y\sim N_n(X\beta,\sigma^2H).}
$$

The [covariance](../../../../../../covariance.md) is $\sigma^2HH^T=\sigma^2H$. This [normal distribution](../../../../../../normal-distribution.md) can be singular when $p<n$, since all fitted vectors lie in the $p$-dimensional model subspace.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5I](../../5i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
