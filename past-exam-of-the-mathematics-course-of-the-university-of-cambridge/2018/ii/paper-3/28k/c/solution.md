<h1 id="28k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [multivariate Wald statistic](../../../../../../multivariate-wald-statistic.md) for a proposed value $\theta$ is

$$
W_n(\theta)
=n(\overline X-\theta)^T\widehat i_n(\overline X-\theta).
$$

Because $\widehat i_n\to I_p$ and

$$
\sqrt n(\overline X-\theta_0)\sim N_p(0,I_p),
$$

[Slutsky theorem](../../../../../../slutsky-theorem.md) gives

$$
\boxed{W_n(\theta_0)\xrightarrow{\mathrm d}\chi_p^2.}
$$

If $q_{p,1-\alpha}$ is the $(1-\alpha)$-quantile of the [chi-squared distribution](../../../../../../chi-squared-distribution.md) with $p$ degrees of freedom, an asymptotic $(1-\alpha)$ confidence region is

$$
\boxed{\left\{\theta:
n(\overline X-\theta)^T\widehat i_n(\overline X-\theta)
\leq q_{p,1-\alpha}\right\}.}
$$

In this known-identity-covariance model one may replace $\widehat i_n$ by $I_p$; then the confidence ball is exact. For an individual coordinate, the corresponding exact [confidence interval](../../../../../../confidence-interval.md) is

$$
\overline X_j\mathbin\pm z_{1-\alpha/2}/\sqrt n.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [28K](../../28k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
