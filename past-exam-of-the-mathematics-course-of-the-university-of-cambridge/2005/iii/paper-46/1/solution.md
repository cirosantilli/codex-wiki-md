<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write the partitioned mean as $(\mu_1^T,\mu_2^T)^T$ and assume $V_{22}$ is nonsingular, as required by the displayed inverse. For the [conditional multivariate normal distribution](../../../../../conditional-multivariate-normal-distribution.md), form the residual

$$
U=X_1-\mu_1-V_{12}V_{22}^{-1}(X_2-\mu_2).
$$

A [linear transformation](../../../../../linear-map.md) of a [multivariate normal distribution](../../../../../multivariate-normal-distribution.md) is again normal. Direct calculation gives

$$
\operatorname{Cov}(U,X_2)=V_{12}-V_{12}V_{22}^{-1}V_{22}=0,\qquad \operatorname{Cov}(U)=V_{11}-V_{12}V_{22}^{-1}V_{21}.
$$

The jointly normal blocks $U$ and $X_2$ are therefore [independent](../../../../../independent-random-variables.md): their joint [characteristic function](../../../../../characteristic-function.md) has no cross term in its quadratic exponent and factors into the two marginal [characteristic functions](../../../../../characteristic-function.md). Conditioning leaves the distribution of $U$ unchanged. Reconstructing $X_1$ proves the full conditional law, including the requested [Schur complement](../../../../../schur-complement.md) [covariance](../../../../../covariance.md):

$$
\boxed{X_1\mid X_2=x_2\sim N\!\left(\mu_1+V_{12}V_{22}^{-1}(x_2-\mu_2),\ V_{11}-V_{12}V_{22}^{-1}V_{21}\right).}
$$

This describes a regular conditional law; it does not require the equality event to have positive probability.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
