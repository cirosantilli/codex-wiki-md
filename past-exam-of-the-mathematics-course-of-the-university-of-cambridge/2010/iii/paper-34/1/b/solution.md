<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Zero observed events do not mean that the underlying event [probability](../../../../../../probability.md) cannot be estimated. For independent observations having a common [Bernoulli distribution](../../../../../../bernoulli-distribution.md), the [binomial likelihood](../../../../../../binomial-likelihood.md) with no events is $(1-p)^{1515}$, maximized at $\widehat p=0$. A [zero-event binomial upper confidence bound](../../../../../../zero-event-binomial-upper-confidence-bound.md) shows the remaining uncertainty: the one-sided 95% upper bound solves $(1-p_U)^{1515}=0.05$, giving

$$
\boxed{p_U=1-0.05^{1/1515}\simeq0.00198.}
$$

Thus the point estimate is zero, but a nonzero mortality risk is compatible with the observations. This bound is an illustration under independent equal-risk sampling; [clustered data](../../../../../../clustered-data.md) or unequal risks require their own uncertainty calculation.

The empirical unadjusted [odds ratio](../../../../../../odds-ratio.md) is also defined:

$$
\boxed{\widehat{\mathrm{OR}}=\frac{0/1515}{53/75004}=0.}
$$

Its [log odds ratio](../../../../../../log-odds-ratio.md) is $-\infty$, so the ordinary [normal approximation](../../../../../../normal-approximation.md) for a log-odds [confidence interval](../../../../../../confidence-interval.md) is unavailable. Exact likelihood-based limits can still describe uncertainty; a specified continuity correction would instead yield a finite, method-dependent point estimate.

In an unpenalized [logistic regression](../../../../../../logistic-regression.md) with a separate coefficient for elective exposure, every exposed death outcome is zero. Decreasing that coefficient toward $-\infty$ increases the exposed observations' likelihood contributions and leaves the reference observations unchanged. This is [quasi-complete separation](../../../../../../quasi-complete-separation.md): there is no finite ordinary [maximum-likelihood estimate](../../../../../../maximum-likelihood-estimator.md) of the exposure coefficient, even after adding background predictors. It is reasonable to say that the usual finite adjusted coefficient could not be fitted; it is too strong to say that no risk estimate or statistical information is possible. A specified penalized likelihood or [Bayesian inference](../../../../../../bayesian-statistics.md) with proper coefficient priors can provide a finite adjusted estimate, whose dependence on the regularization must be reported.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
