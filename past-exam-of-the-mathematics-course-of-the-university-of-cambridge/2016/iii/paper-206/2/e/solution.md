<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Check that the chosen mean structure adequately describes the transformed response. Examine the [residual-versus-fitted plot](../../../../../../residual-versus-fitted-plot.md) and residuals versus each predictor: systematic curvature suggests omitted nonlinear effects or an [interaction term](../../../../../../interaction-term.md). Plot residual spread against fitted values, for example using a [scale-location plot](../../../../../../scale-location-plot.md), to assess [homoscedasticity](../../../../../../homoscedasticity.md). Compare standardized residuals with a [normal distribution](../../../../../../normal-distribution.md) using a [quantile-quantile plot](../../../../../../q-q-plot.md), especially for finite-sample [Student's t-distribution](../../../../../../student-s-t-distribution.md) and [F-test](../../../../../../f-test.md) inference.

Also check [independence](../../../../../../independent-random-variables.md) using the sampling design and residuals versus time, collection site, or other groups; spatially related photovoltaic systems may have correlated errors that are invisible in a residual-versus-fitted plot. Investigate large [standardized regression residuals](../../../../../../standardized-regression-residual.md), high [regression leverage](../../../../../../regression-leverage.md), and influential observations using [Cook's distance](../../../../../../cook-s-distance.md). Check that the [design matrix](../../../../../../design-matrix.md) has full rank and that severe [multicollinearity](../../../../../../multicollinearity.md) is not making estimates unstable. Reassess whether the response transformation and retained predictors improve these diagnostics and prediction; a coefficient [p-value](../../../../../../p-value.md) alone cannot establish model adequacy. If observations are independent only conditional on site effects, use an appropriate dependence model rather than treating correlated systems as independent replicates.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
