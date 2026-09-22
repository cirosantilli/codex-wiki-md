<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The residual smooth rises from negative values, arches above zero, then falls at high fitted values. This suggests a nonlinear altitude effect on the log mean. Since the fitted log mean in the linear model increases with altitude, the horizontal fitted-value axis is also an increasing rescaling of altitude. A [generalized additive model](../../../../../../generalized-additive-model.md) with [Quasi-Poisson regression](../../../../../../quasi-poisson-regression.md) is therefore a reasonable candidate:

$$
\log\mu_i=\alpha+f(a_i),\qquad
\operatorname{Var}(Y_i)=\phi\mu_i,\qquad\sum_i f(a_i)=0.
$$

The centering constraint identifies the intercept. Here `bs="cr"` uses a penalized [cubic regression spline](../../../../../../cubic-regression-spline.md). The plotted count residuals are [deviance residuals](../../../../../../deviance-residual.md), with the Q-Q panel using leverage-standardized versions. The [quantile-quantile plot](../../../../../../q-q-plot.md) also shows tail discrepancies, but [normality](../../../../../../normal-distribution.md) of count residuals is not a distributional assumption of this model: its main requirements are an adequate mean, variance relation, and [independence](../../../../../../independent-random-variables.md). Investigate the labelled islands and possible excess variation as well.

The estimated smooth in the second plot increases fairly rapidly at low altitude, flattens around altitude 20 to 25, and is nearly level at the upper end. The pointwise bands widen where there are fewer observations. **A penalized spline can describe a rise followed by a plateau without forcing a global parabola.** A quadratic log mean has slope $\beta_1+2\beta_2a$, so negative curvature eventually forces a decline and its curvature is constant everywhere. A [cubic regression spline](../../../../../../cubic-regression-spline.md) allows different curvature over different ranges, with a penalty controlling unnecessary wiggles and natural linear tails outside its boundary knots. The displayed smooth supports this greater flexibility, but it is not by itself a formal rejection of every quadratic model. Select complexity and compare predictive performance using [cross-validation](../../../../../../cross-validation.md), then reassess residuals and the [Pearson dispersion estimator](../../../../../../pearson-dispersion-estimator.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
