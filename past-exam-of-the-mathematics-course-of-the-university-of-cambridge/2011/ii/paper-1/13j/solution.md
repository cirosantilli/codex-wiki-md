<h1 id="13j/solution">Solution</h1>

↑ **Parent:** [13J](../13j.md)

Use a [normal linear model](../../../../../normal-linear-model.md)

$$
T_i=\beta_0+\beta_1d_i+\beta_2h_i+\varepsilon_i,
\qquad\varepsilon_i\overset{\rm iid}{\sim}N(0,\sigma^2).
$$

The distance and climb are treated as fixed predictors; the assumptions are a linear conditional mean, independent errors with common [variance](../../../../../variance-split.md), and normal errors for the exact tests. Fit by [ordinary least squares](../../../../../ordinary-least-squares.md) using
```
hills.lm1 <- lm(time ~ dist + climb, data = hills)
```

The overall [null hypothesis](../../../../../null-hypothesis.md) is $\beta_1=\beta_2=0$, against at least one nonzero slope. The intercept-only and full models have respectively 34 and 32 residual degrees of freedom. Under the null, the [F-test](../../../../../f-test.md) statistic is

$$
F=\frac{(\mathrm{RSS}_0-\mathrm{RSS}_1)/2}{\mathrm{RSS}_1/32}
\simeq181.66\sim F_{2,32}.
$$

The displayed residual sums are rounded; use the reported statistic for the test. Its upper-tail [p-value](../../../../../p-value.md) is below $2.2\times10^{-16}$, so **reject the no-relationship hypothesis overwhelmingly**. At least one predictor adds information beyond a constant mean.

In the coefficient table, Estimate gives one of the [ordinary least squares estimators](../../../../../ordinary-least-squares-estimators.md), Std. Error is the estimated standard deviation of that estimator, t value is the estimate divided by its [standard error](../../../../../standard-error.md), and the last column is the two-sided [p-value](../../../../../p-value.md) for a zero coefficient. Under the corresponding null, the statistic has a [Student's t-distribution](../../../../../student-s-t-distribution.md) with 32 degrees of freedom. The fitted mean is

$$
\boxed{\widehat T=-8.992039+6.217956d+0.011048h.}
$$

At fixed climb, an extra mile predicts about 6.22 extra minutes; at fixed distance, an extra foot of climb predicts about 0.01105 extra minutes. Both slopes have strong evidence of being positive. Specifically the climb test uses $t=5.387$ and $p=6.45\times10^{-6}$, so **climb remains significant after controlling for distance**. The intercept differs from zero at the 5% level, but extrapolating to a zero-distance, zero-climb race has no useful physical interpretation.

The [regression diagnostics](../../../../../regression-diagnostics.md) show a very large positive residual for Knock Hill and a smaller positive outlier for Bens of Jura. The [Q-Q plot](../../../../../q-q-plot.md) has a pronounced upper tail, contradicting the assumed normal-error pattern. These observations can distort both the fitted coefficients and the estimated error variance. Check the source records, units, transcription and any unusual race conditions first, especially for Knock Hill; correct a demonstrated data error and refit. If the records are valid, consider omitted terrain effects, nonlinear distance/climb effects, a suitable response transformation or robust regression, and compare fits with and without influential observations. A diagnostic outlier alone is not a reason to silently delete a valid record.

## ↑ Ancestors (11)

1. [13J](../13j.md)
2. [Section II](../section-ii.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ii](../../split.md)
5. [2011](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
