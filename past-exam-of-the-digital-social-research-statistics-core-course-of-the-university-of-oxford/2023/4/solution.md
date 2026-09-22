<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [ordinary least squares](../../../ordinary-least-squares.md) fit estimates the conditional [mean](../../../expected-value-split.md) of the continuous safety response as a [linear function](../../../linear-function.md) of the income coding:

$$
\boxed{\widehat{\mathrm{feelsafe}}=6.5933+0.2369\,\mathrm{income}.}
$$

The [regression coefficient](../../../regression-coefficient.md) for income is positive. Since larger response values [mean](../../../expected-value-split.md) greater safety, one additional coded income unit corresponds to an estimated increase of $0.2369$ safety-scale units in the fitted [mean](../../../expected-value-split.md). Following the question's stated units, a unit is a £10,000 income step. The observed coding also uses income bands with open end categories, so this is a linear trend per coded band step; it is not evidence of a known constant effect for every extra pound, especially within the open top band. The output's abbreviated variable label does not override the stated units.

The [intercept](../../../regression-intercept.md) is the fitted [mean](../../../expected-value-split.md) at income code zero. It is estimated as $6.5933$, but zero is outside the observed income codes, so that value is an extrapolated model baseline, not an observed estimate for a particular income category. Its small [p-value](../../../p-value.md) tests a zero intercept; it is not the main test of the income association.

For the income coefficient, the [standard error](../../../standard-error.md) is $0.0604$. The reported [test statistic](../../../test-statistic.md) and [two-sided test](../../../two-sided-hypothesis-test.md) give

$$
t\simeq3.922,\qquad p=9.13\times10^{-5},
$$

providing strong evidence against the [null hypothesis](../../../null-hypothesis.md) of zero linear slope under the stated model assumptions. A $95\%$ [Student t confidence interval](../../../student-t-confidence-interval.md), using $1727$ residual [statistical degrees of freedom](../../../statistical-degrees-of-freedom.md), is

$$
\boxed{0.2369\pm t_{1727,0.975}(0.0604)\simeq[0.1184,\,0.3554].}
$$

This is an interval for the population linear coefficient under the model, not an interval containing $95\%$ of individual safety scores. The large-sample estimate is precise enough to detect a positive association, but that does not establish substantial individual predictive power.

The [coefficient of determination](../../../coefficient-of-determination.md) is $R^2=0.008828$: the fitted line accounts for about $0.883\%$ of the in-sample variation about the response [sample mean](../../../sample-mean.md). The [adjusted coefficient of determination](../../../adjusted-coefficient-of-determination.md) is about $0.825\%$. Thus **income alone explains very little of the observed variation**, despite the small slope [p-value](../../../p-value.md). The [residual standard error](../../../residual-standard-error.md) of $3.997$ response units describes substantial scatter about the fitted line. This is an estimated residual [standard deviation](../../../standard-deviation.md), rather than the [standard error](../../../standard-error.md) of the slope or a complete individual prediction interval.

The overall [F-test](../../../f-test.md) has $F=15.38$ on $1,1727$ [statistical degrees of freedom](../../../statistical-degrees-of-freedom.md) and $p=9.129\times10^{-5}$. With one predictor and an [intercept](../../../regression-intercept.md), it tests the same zero-slope hypothesis as the coefficient [Student's t-test](../../../student-s-t-test.md); $F=t^2$, up to rounding. It is not an additional independent confirmation. In this [simple linear regression](../../../simple-linear-regression.md), the [Pearson correlation coefficient](../../../pearson-correlation-coefficient.md) has the slope's sign and magnitude $\sqrt{R^2}\simeq0.0940$, another description of the weak linear association.

The regression uses $1729$ complete observations and estimates two coefficients, giving $1729-2=1727$ residual [statistical degrees of freedom](../../../statistical-degrees-of-freedom.md). The deletion of $88$ observations is [complete-case analysis](../../../complete-case-analysis.md); extending its conclusions to the full target population requires suitable assumptions about the [missing-data mechanism](../../../missing-data-mechanism.md). Classical reported [standard errors](../../../standard-error.md) also rely on an adequate linear conditional [mean](../../../expected-value-split.md), independent errors and [homoscedasticity](../../../homoscedasticity.md); a [normal linear model](../../../normal-linear-model-split.md) gives the finite-sample [Student t-distribution](../../../student-s-t-distribution.md) and [F-test](../../../f-test.md) calibration, while large-sample approximations can justify similar tests under weaker distributional assumptions. The printed summary alone does not establish these assumptions. [Regression diagnostics](../../../regression-diagnostics.md) and, where appropriate, [heteroskedasticity-consistent standard errors](../../../heteroskedasticity-consistent-standard-errors.md) address different parts of that assessment.

Finally, this unadjusted [observational study](../../../observational-study.md) estimates an association. Other [covariates](../../../covariate.md), such as age or experience status, may be related to both income and reported safety. Without additional design or [causal identification](../../../causal-identification.md) assumptions, the positive fitted slope does not establish that increasing income would cause an increase in safety.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [2023](../../2023-split.md)
3. [Past exam of the digital social research: statistics core course of the University of Oxford](../../split.md)
4. [Digital social research: statistics core course of the University of Oxford](../../../digital-social-research-statistics-core-course-of-the-university-of-oxford.md)
5. [MSc in social science of the internet course of the University of Oxford](../../../msc-in-social-science-of-the-internet-course-of-the-university-of-oxford.md)
6. [Master's course of the University of Oxford](../../../master-s-course-of-the-university-of-oxford.md)
7. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
8. [University of Oxford](../../../university-of-oxford-split.md)
9. [List of universities](../../../list-of-universities.md)
10. [Codex Wiki](../../../split.md)
