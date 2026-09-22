<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The transformed values are [Cox–Snell residuals](../../../../../../cox-snell-residual.md). Under a correct common [survival function](../../../../../../survival-function.md) and a good fitted [cumulative hazard function](../../../../../../cumulative-hazard-function.md), the complete transformed failure times should have unit [exponential distribution](../../../../../../exponential-distribution.md). Transform the observed times and retain their original [censoring](../../../../../../censoring-statistics.md) indicators, then estimate residual survival with a [Kaplan–Meier estimator](../../../../../../kaplan-meier-estimator.md). Its target is

$$
\boxed{S_u(u)=e^{-u},\qquad u\geq0,}
$$

so a plot of its logarithm against $u$ should lie approximately on a line of slope $-1$. Censored residuals must not be treated as fully observed failure times.

There is a useful caution for this particular common nonparametric fit. The [shared-fit Cox–Snell residuals reproduce the fitted survival curve](../../../../../../shared-fit-cox-snell-residuals-reproduce-the-fitted-survival-curve.md) property means that the pooled residual plot is largely built into the transformation. With event ordering and compatible tie processing preserved, at a transformed failure time $u_j=\widehat H(t_j)$ its residual [Kaplan–Meier estimator](../../../../../../kaplan-meier-estimator.md) equals $\widehat S(t_j)=e^{-u_j}$. Finite steps, coalesced [censoring](../../../../../../censoring-statistics.md) times and estimation uncertainty still matter, and an infinite final residual arises if the fitted survivor becomes zero. Separate group plots are more informative about a common-distribution assumption than this pooled fit alone.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
