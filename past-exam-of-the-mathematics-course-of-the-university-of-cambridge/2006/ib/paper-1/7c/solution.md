<h1 id="7c/solution">Solution</h1>

↑ **Parent:** [7C](../7c.md)

For the independent [normal distribution](../../../../../normal-distribution.md) observations, the log [likelihood](../../../../../likelihood-function.md) is

$$
\ell(\theta)=-\frac n2\log(2\pi)-\frac12\sum_{i=1}^n(X_i-\theta)^2.
$$

Its [derivative](../../../../../derivative.md) is $\sum_i(X_i-\theta)$ and its second [derivative](../../../../../derivative.md) is $-n<0$, so the unique [maximum-likelihood estimate](../../../../../maximum-likelihood-estimator.md) is

$$
\boxed{\widehat\theta_M=\overline X=\frac1n\sum_iX_i.}
$$

For the prior $\theta\sim N(\mu,\tau^{-1})$ with $\tau>0$, multiplying prior [density](../../../../../density.md) by [likelihood](../../../../../likelihood-function.md) and completing the square gives

$$
\sum_i(X_i-\theta)^2+\tau(\theta-\mu)^2
=(n+\tau)\left(\theta-\frac{n\overline X+\tau\mu}{n+\tau}\right)^2+\text{a term independent of }\theta.
$$

Thus [normal-normal conjugacy](../../../../../normal-normal-conjugacy-with-known-observation-variance.md) gives the [posterior distribution](../../../../../bayesian-posterior.md)

$$
\theta\mid X\sim N\!\left(\frac{n\overline X+\tau\mu}{n+\tau},\frac1{n+\tau}\right).
$$

For [quadratic loss](../../../../../squared-error-loss.md), the conditional expected loss of action $a$ is the [posterior variance](../../../../../posterior-variance.md) plus $(a-\mathbb E[\theta\mid X])^2$. Its unique minimizer is the [posterior mean](../../../../../posterior-mean.md), so the [Bayes estimator](../../../../../bayes-estimator.md) is

$$
\boxed{\widehat\theta_B=\frac{n\overline X+\tau\mu}{n+\tau}.}
$$

This weights the sample and prior [means](../../../../../expected-value.md) by their respective precisions.

## ↑ Ancestors (10)

1. [7C](../7c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
