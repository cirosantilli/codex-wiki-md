<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Because both vectors are linear transformations of the same [multivariate normal](../../../../../../multivariate-normal-distribution.md) response, $(\widehat Y,e)$ is jointly [multivariate normal](../../../../../../multivariate-normal-distribution.md). Its cross-[covariance matrix](../../../../../../covariance-matrix.md) is

$$
\operatorname{Cov}(\widehat Y,e)=P(\sigma^2I_n)(I_n-P)^T
=\sigma^2(P-P^2)=0.
$$

Zero cross-[covariance](../../../../../../covariance.md) implies independence for jointly [multivariate normal](../../../../../../multivariate-normal-distribution.md) vectors, including singular ones. Therefore **the [fitted values](../../../../../../fitted-values.md) and the entire vector of [regression residuals](../../../../../../regression-residual.md) are independent**. The [fitted-residual orthogonality](../../../../../../fitted-residual-orthogonality.md) identity gives the zero [covariance](../../../../../../covariance.md); the [normal distribution](../../../../../../normal-distribution.md) assumption is what upgrades it to independence.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
