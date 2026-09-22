<h1 id="29k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [multivariate Wald statistic](../../../../../../multivariate-wald-statistic.md) for a candidate parameter $\theta\in\mathbb R^p$ is

$$
W_n(\theta)
=n(\widehat\theta_n-\theta)^T
I(\widehat\theta_n)
(\widehat\theta_n-\theta).
$$

Replacing $I(\widehat\theta_n)$ by any consistent estimator of $I(\theta_0)$ gives the same limit.

Under $P_{\theta_0}$, part (a) and consistency of the information matrix imply, by [Slutsky theorem](../../../../../../slutsky-theorem.md), that

$$
I(\widehat\theta_n)^{1/2}
\sqrt n(\widehat\theta_n-\theta_0)
\xrightarrow d N_p(0,I_p).
$$

Consequently

$$
\boxed{W_n(\theta_0)\xrightarrow d\chi_p^2,}
$$

using the characterization of the [chi-squared distribution](../../../../../../chi-squared-distribution.md) as the squared norm of a standard normal vector.

If $q_{p,1-\alpha}$ is the $(1-\alpha)$ quantile of $\chi_p^2$, an asymptotic $(1-\alpha)$ confidence region is

$$
\boxed{
C_n=\{\theta\in\mathbb R^p:W_n(\theta)\leq q_{p,1-\alpha}\}.
}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [29K](../../29k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
