<h1 id="12j/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Under fit.2, observations in each period are independent [Poisson random variables](../../../../../../poisson-distribution.md) with a common mean, so each [sample variance](../../../../../../sample-variance.md) should fluctuate around its [sample mean](../../../../../../sample-mean.md). The plot instead has [variances](../../../../../../variance-split.md) roughly 130–300 for means roughly 80–120, well above the line [variance](../../../../../../variance-split.md) equals mean. This is [overdispersion](../../../../../../overdispersion.md).

Day-to-day traffic variation can produce a [Poisson mixture](../../../../../../poisson-mixture.md): a random daily intensity increases the marginal [variance](../../../../../../variance-split.md) and can correlate observations from the same day. A useful replacement is a [negative binomial regression](../../../../../../negative-binomial-regression.md), with [variance](../../../../../../variance-split.md) $\mu+\mu^2/\kappa$, or a [Poisson generalized linear mixed model](../../../../../../poisson-generalized-linear-mixed-model.md) with a day [random intercept](../../../../../../random-intercept.md). A day-factor effect can also be included if inference is restricted to the observed days. A [Quasi-Poisson regression](../../../../../../quasi-poisson-regression.md) estimates a dispersion multiplier for uncertainty, but does not itself explain the shared-day dependence and has no ordinary likelihood-based AIC. The means can retain the period-factor or selected jump structure.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [12J](../../12j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
