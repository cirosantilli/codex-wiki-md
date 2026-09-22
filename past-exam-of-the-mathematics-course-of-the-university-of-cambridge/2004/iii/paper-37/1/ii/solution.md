<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The working [score function](../../../../../../informant-function.md) and its derivative are

$$
U(\beta)=\sum_i x_i\{Y_i-e^{\beta x_i}\},\qquad
U'(\beta)=-\sum_i x_i^2e^{\beta x_i}=-I(\beta).
$$

At an interior working maximizer, $U(\widehat\beta)=0$. A [Taylor expansion](../../../../../../taylor-expansion.md) at $\beta_0$ yields

$$
0=U(\beta_0)-I(\beta_0)(\widehat\beta-\beta_0)
-\frac12\left(\sum_i x_i^3e^{\beta^*x_i}\right)(\widehat\beta-\beta_0)^2
$$

for an intermediate value $\beta^*$. When the last term is negligible relative to the linear one, this gives

$$
\boxed{\widehat\beta-\beta_0\approx I(\beta_0)^{-1}U(\beta_0).}
$$

This is the [Poisson score linearization under proportional variance](../../../../../../poisson-score-linearization-under-proportional-variance.md). Correct specification of the mean alone implies $EU(\beta_0)=0$. The stipulated independence and [variance](../../../../../../variance-split.md) relation give

$$
\operatorname{Var}U(\beta_0)=\sum_i x_i^2\operatorname{Var}(Y_i)=\phi\sum_i x_i^2e^{\beta_0x_i}=\phi I(\beta_0).
$$

Taking the mean and [variance](../../../../../../variance-split.md) of the linear approximation therefore proves

$$
\boxed{E\widehat\beta\approx\beta_0,\qquad
\operatorname{Var}(\widehat\beta)\approx\frac{\phi}{I(\beta_0)}.}
$$

These are first-order conclusions, not exact finite-sample identities. The mean and [variance](../../../../../../variance-split.md) assumptions alone do not guarantee that the approximation is accurate: an interior consistent solution, increasing information, control of leverage, and a suitable central limit condition are needed for normal inference.

The [quasi-likelihood](../../../../../../quasi-likelihood.md) score for [variance](../../../../../../variance-split.md) $\phi\mu_i$ is $U/\phi$, so its zero is unchanged by the unknown common [dispersion parameter](../../../../../../dispersion-parameter.md). Thus the working Poisson estimating equation remains appropriate for the mean parameter, but its unadjusted Poisson [variance](../../../../../../variance-split.md) estimate is wrong when $\phi\ne1$. A usual [Pearson dispersion estimator](../../../../../../pearson-dispersion-estimator.md) for this one-parameter model is

$$
\widehat\phi=\frac1{n-1}\sum_i\frac{(Y_i-\widehat\mu_i)^2}{\widehat\mu_i},\qquad
\widehat{\operatorname{Var}}(\widehat\beta)=\frac{\widehat\phi}{I(\widehat\beta)}.
$$

In particular [overdispersion](../../../../../../overdispersion.md) multiplies coefficient [standard errors](../../../../../../standard-error.md) by approximately $\sqrt\phi$, even though it leaves the coefficient estimating equation unchanged.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
