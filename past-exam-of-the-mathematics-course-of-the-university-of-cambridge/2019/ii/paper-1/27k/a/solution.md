<h1 id="27k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $d=1$ and $X\sim N(0,\sigma^2)$, the [characteristic function](../../../../../../characteristic-function.md) is

$$
\boxed{\varphi_X(u)=e^{-\sigma^2u^2/2}}.
$$

For a [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md) with covariance matrix $\sigma^2I_d$, the coordinates are uncorrelated and hence independent by [independence of uncorrelated jointly normal variables](../../../../../../independence-of-uncorrelated-jointly-normal-variables.md). Therefore

$$
\varphi_X(u)
=\prod_{j=1}^d\mathbb E[e^{iu_jX_j}]
=\prod_{j=1}^de^{-\sigma^2u_j^2/2}
=\boxed{\exp\left(-\frac{\sigma^2}{2}\sum_{j=1}^du_j^2\right)}.
$$

This is the [characteristic function of an isotropic Gaussian vector](../../../../../../characteristic-function-of-an-isotropic-gaussian-vector.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [27K](../../27k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
