<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

**The fitted age slope is very small and negative, about $-0.00319$ efficacy points per year, with no conventional evidence against a zero linear slope: $t\approx-0.951$, $p\approx0.342$. The model explains only about 0.0367% of the observed efficacy variation. These results concern a linear association, not proof of no possible age relationship or a [causal effect](../../../causal-effect.md) of ageing.**

The [descriptive statistics](../../../descriptive-statistics.md) report 2466 observed ages and efficacy scores, with no missing values for either variable. Age ranges from 14 to 97 years, with [sample mean](../../../sample-mean.md) 52.689 years and [sample standard deviation](../../../sample-standard-deviation.md) 19.064 years. Efficacy ranges from 0 to 16, with [sample mean](../../../sample-mean.md) 9.348 and [sample standard deviation](../../../sample-standard-deviation.md) 3.176 scale points. The [standard deviations](../../../standard-deviation.md) use different units and should not be compared as though their numerical ratio measured relative substantive variability. The efficacy mean retains the conflict with Question 1's group summaries; that conflict is not resolved by this separate regression output.

A [simple linear regression](../../../simple-linear-regression.md) models $\mathbb E(Y\mid x)=\beta_0+\beta_1x$, where $Y$ is efficacy and $x$ is age in years. [Ordinary least squares](../../../ordinary-least-squares.md) chooses the coefficients to minimize the [residual sum of squares](../../../residual-sum-of-squares.md). From the printed coefficients the fitted line is

$$
\boxed{\widehat y=9.516515-0.003192\,x.}
$$

Holding to this model, ten additional years correspond to $-0.03192$ fitted scale points. For example, the fitted mean is about 9.453 at age 20 and 9.261 at age 80, a difference of about $-0.192$ points. These are fitted means, not exact predictions of individual scores. The line does not imply that every person's efficacy falls at that rate, nor that cross-sectional age differences identify within-person changes over time.

The [intercept](../../../regression-intercept.md) is the predicted mean at age zero, about 9.517. Since zero is outside the observed 14–97 age range, its direct interpretation requires extrapolation. The printed [standard error](../../../standard-error.md) of 0.188043 and $t\approx50.608$ yield the extremely small displayed [p-value](../../../p-value.md) for a zero [intercept](../../../regression-intercept.md). That test does not test whether age is a useful predictor. Recentring age at its observed [sample mean](../../../sample-mean.md) would put the [intercept](../../../regression-intercept.md) near $9.516515-0.003192(52.689)\approx9.34833$, the fitted mean at a substantively relevant reference age. This agrees with the rounded overall efficacy mean.

The age [standard error](../../../standard-error.md) is 0.003356 points per year. The coefficient divided by this [standard error](../../../standard-error.md) gives $-0.003192/0.003356\approx-0.9511$, agreeing with the printed t value. Estimating an [intercept](../../../regression-intercept.md) and one [regression slope](../../../regression-slope.md) from 2466 observations leaves $2466-2=2464$ residual [statistical degrees of freedom](../../../statistical-degrees-of-freedom.md). Under a correctly specified [normal linear model](../../../normal-linear-model-split.md), the [Student t-distribution](../../../student-s-t-distribution.md) provides the stated two-sided [p-value](../../../p-value.md). At 5%, or 1%, it does not reject $H_0:\beta_1=0$. The [p-value](../../../p-value.md) is not a 34.2% [probability](../../../probability.md) that age has no effect, and nonrejection does not establish a practically negligible [effect size](../../../effect-size.md).[Value: coefficient estimate, standard error, two-sided t and p columns; residual degrees of freedom](../../../summarizing-linear-model-fits-in-the-r-documentation.md)

A 95% [confidence interval](../../../confidence-interval.md) calculated from the printed estimate and [standard error](../../../standard-error.md) is approximately

$$
\boxed{\beta_1\in[-0.009773,\ 0.003389]\text{ scale points per year},}
$$

or about $[-0.09773,0.03389]$ points per decade. It includes zero and gives the scale of slopes compatible with these summaries and assumptions. Assessing a practically negligible effect would require an explicit substantive tolerance and an appropriate [equivalence test](../../../equivalence-test.md), not simply the fact that $p>0.05$. A nonlinear association could also coexist with a near-zero overall linear slope.

The [coefficient of determination](../../../coefficient-of-determination.md) is $R^2=0.000367$, meaning that the fitted line explains about $100R^2=0.0367\%$ of the sample's centred efficacy [sum of squares](../../../sum-of-squares.md) compared with an intercept-only fit. This is not 36.7%, a fraction of people whose efficacy is predicted correctly, or the proportion of efficacy caused by age. The [adjusted coefficient of determination](../../../adjusted-coefficient-of-determination.md), approximately $-0.00003873$, is slightly negative because its penalty for estimating the extra coefficient exceeds the tiny improvement in fit. It need not be constrained to be nonnegative and does not mean a negative amount of explained variation.

The overall $F\approx0.9045$ on 1 and 2464 [statistical degrees of freedom](../../../statistical-degrees-of-freedom.md), with $p\approx0.3417$, tests the same zero-slope hypothesis as the age t test because there is only one predictor. The [simple-regression output identities](../../../simple-regression-output-identities.md) give $F=t_{\mathrm{slope}}^2$ and $F=(2464)R^2/(1-R^2)$; the printed numbers agree allowing their displayed precision. The signed [Pearson correlation coefficient](../../../pearson-correlation-coefficient.md) is consequently about $-\sqrt{R^2}\approx-0.0192$. These are related summaries of the same weak linear association, not [independent](../../../independent-random-variables.md) corroborating tests.

The [residual standard error](../../../residual-standard-error.md) of 3.177 points estimates the typical unexplained error scale under the fitted model. It is close to the efficacy [sample standard deviation](../../../sample-standard-deviation.md), as expected when the line explains almost none of the variation. It is not a [standard error](../../../standard-error.md) of the slope or a guarantee that each individual's prediction error lies within 3.177 points. The residual summary spans roughly $-9.46$ to $6.75$, with [sample median](../../../sample-median.md) about 0.573 and central [quartiles](../../../quartile.md) about $-1.437$ and $2.579$. An ordinary least-squares fit with an [intercept](../../../regression-intercept.md) has zero mean residual, not necessarily zero median residual. These few [quantiles](../../../quantile-function.md) cannot establish [normality](../../../normality-statistics.md), constant conditional spread, absence of outliers or linearity. The apparent last-decimal discrepancies among rounded error scales and other summary fields do not force an additional contradiction: their [rounding](../../../rounding.md) intervals admit compatible regression summaries.

The conventional uncertainty calculations assume [independent](../../../independent-random-variables.md), mean-zero errors conditional on age, an appropriate linear mean, and [homoscedasticity](../../../homoscedasticity.md); normal errors give the usual exact finite-sample t and F calibration. Large samples can relax some distributional requirements but do not remove [confounding](../../../confounding.md), [selection bias](../../../selection-bias.md) or dependence. A [residual-versus-fitted plot](../../../residual-versus-fitted-plot.md) could reveal curvature or changing spread, and a [normal probability plot](../../../normal-q-q-plot.md) could assess error shape; neither plot can be reconstructed from the printed residual [quantiles](../../../quantile-function.md). A [prediction interval](../../../prediction-interval.md) for an individual includes residual variation and is wider than a [confidence interval](../../../confidence-interval.md) for the mean response. **The supplied output supports a very weak, imprecisely signed linear association with little predictive gain from age alone, while leaving nonlinear, causal and design-based questions unresolved.**

## ↑ Ancestors (10)

1. [6](../6.md)
2. [2019](../../2019-split.md)
3. [Past exam of the digital social research: statistics core course of the University of Oxford](../../split.md)
4. [Digital social research: statistics core course of the University of Oxford](../../../digital-social-research-statistics-core-course-of-the-university-of-oxford.md)
5. [MSc in social science of the internet course of the University of Oxford](../../../msc-in-social-science-of-the-internet-course-of-the-university-of-oxford.md)
6. [Master's course of the University of Oxford](../../../master-s-course-of-the-university-of-oxford.md)
7. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
8. [University of Oxford](../../../university-of-oxford-split.md)
9. [List of universities](../../../list-of-universities.md)
10. [Codex Wiki](../../../split.md)
