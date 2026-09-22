<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The fitted [simple linear regression](../../../simple-linear-regression.md) is

$$
\boxed{\widehat{\text{trust}}=6.388920-0.006314\,\text{age}.}
$$

Its [regression slope](../../../regression-slope.md) is a predicted decrease of approximately 0.006314 trust-score units per extra year, or 0.06314 units per decade. This is an estimated [statistical association](../../../statistical-association.md) between age and the score. A [cross-sectional study](../../../cross-sectional-study.md) does not establish that the same person's trust decreases at this rate as they age.

The estimated [standard error](../../../standard-error.md) of the slope is 0.005427. Testing a zero [regression slope](../../../regression-slope.md) gives $t\approx-1.163$ on 746 [residual degrees of freedom](../../../residual-degrees-of-freedom.md) and $p\approx0.245$. An approximate 95% [confidence interval](../../../confidence-interval.md) is

$$
-0.006314\pm t_{746,0.975}(0.005427)\approx[-0.016968,\ 0.004340].
$$

**There is insufficient evidence of a nonzero linear age association at the 5% level.** The interval includes both small negative and small positive slopes; failure to reject does not establish an exactly zero relationship or rule out a nonlinear one.

The [regression intercept](../../../regression-intercept.md) 6.388920 predicts the score at age zero. That age is outside the observed 19–89 range, so interpreting it substantively would be [extrapolation](../../../extrapolation.md). Its very small reported [p-value](../../../p-value.md) tests a zero intercept, rather than the age hypothesis. The 746 [residual degrees of freedom](../../../residual-degrees-of-freedom.md) correspond to 748 observations minus the intercept and slope.

The [coefficient of determination](../../../coefficient-of-determination.md) is $R^2=0.001811$, so the fitted line explains approximately **0.1811% of the observed centered variation**, rather than 18.11%. The [adjusted coefficient of determination](../../../adjusted-coefficient-of-determination.md) is approximately 0.0004732. The [residual standard error](../../../residual-standard-error.md) is 2.602 score units, close to the reported response [standard deviation](../../../standard-deviation.md); most variation remains unexplained by the fitted line. With one predictor and an intercept, the slope's [F-test](../../../f-test.md) is the square of its [Student's t-test](../../../student-s-t-test.md) statistic, up to printed rounding, so $F\approx1.354$ and $p\approx0.245$ agree with the slope test.

Output 6 is a [residual-versus-fitted plot](../../../residual-versus-fitted-plot.md): its vertical coordinates should be [regression residuals](../../../regression-residual.md) $e_i=y_i-\widehat y_i$. The fitted values range over only approximately 5.83–6.27, as the weak slope predicts over ages 19–89. The printed scatter shows no obvious strong mean curvature or clear widening funnel, but it has marked horizontal concentrations near its extreme residual levels. An absence of obvious curvature does not prove a correct linear [conditional mean](../../../conditional-expectation.md), and the plot alone cannot establish [homoscedasticity](../../../homoscedasticity.md), independent errors or a [normal distribution](../../../normal-distribution.md). A [normal probability plot](../../../normal-q-q-plot.md) and residuals against observation order address different aspects. Large residuals also do not by themselves establish influential observations; [regression leverage](../../../regression-leverage.md) and [Cook's distance](../../../cook-s-distance.md) matter.

There is an additional inconsistency in the original figure. The descriptive output reports observed responses between zero and ten, so [residual constraints from a bounded response](../../../residual-constraints-from-a-bounded-response.md) require

$$
-\widehat y_i\le e_i\le10-\widehat y_i.
$$

Yet the printed graphic contains points around $(\widehat y,e)=(6.25,4.2)$, which would imply $y\approx10.45$, above the stated observed maximum. Some lower-edge points likewise imply negative responses. This is present in the original PDF, rather than introduced by the transcription. The graphic therefore cannot be treated as a fully consistent diagnostic of the reported dataset. The observations about its visible shape above describe the supplied picture; reliable model checking would require the actual fitted values and residuals.

The printed code has separate typographical problems. The displayed model call supports the intended formula with `~`, and the plot needs one closing parenthesis:

```
model1 <- lm(t_guard ~ age, data = exam)
plot(fitted(model1), residuals(model1),
     xlab = "Fitted values", ylab = "Residuals")
abline(h = 0)
```

These calls correct the syntax; they cannot be rerun on the original observations because the individual-level dataset is not supplied. The regression interpretation above uses the available numerical summaries and states the diagnostic limitation explicitly.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [2022](../../2022-split.md)
3. [Past exam of the digital social research: statistics core course of the University of Oxford](../../split.md)
4. [Digital social research: statistics core course of the University of Oxford](../../../digital-social-research-statistics-core-course-of-the-university-of-oxford.md)
5. [MSc in social science of the internet course of the University of Oxford](../../../msc-in-social-science-of-the-internet-course-of-the-university-of-oxford.md)
6. [Master's course of the University of Oxford](../../../master-s-course-of-the-university-of-oxford.md)
7. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
8. [University of Oxford](../../../university-of-oxford-split.md)
9. [List of universities](../../../list-of-universities.md)
10. [Codex Wiki](../../../split.md)
