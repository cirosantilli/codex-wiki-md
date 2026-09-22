<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

**The supplied coefficient and slope-test fields support a negative linear age association: about $-0.14645$ media-diversity points per year, or $-1.4645$ per decade. However, the reported $R^2$ and intercept uncertainty are inconsistent with other fields. They cannot all be combined into a single verified regression interpretation.**

The descriptive summaries give 1784 observed ages and diversity scores, with no missing values. Age ranges from 18 to 89 years, with mean 43.035 and [sample standard deviation](../../../sample-standard-deviation.md) 16.862 years. Diversity ranges from 0 to 48, with mean 19.592 and [sample standard deviation](../../../sample-standard-deviation.md) 10.240 points. The scale combines online and offline consumption sources; the output does not say that one point equals one source, so that unit should not be invented. Comparing the numerical standard deviations across these different units does not establish which variable is more variable substantively.

A [simple linear regression](../../../simple-linear-regression.md) posits $\mathbb E(Y\mid x)=\beta_0+\beta_1x$, where Y is diversity and x is age. [Ordinary least squares](../../../ordinary-least-squares.md) fits that conditional mean by minimizing the [residual sum of squares](../../../residual-sum-of-squares.md). If the coefficient estimates are trusted, the fitted line is

$$
\boxed{\widehat y=25.89474-0.14645x.}
$$

It predicts about 23.259 diversity points at age 18 and 12.861 at age 89. At the mean age it predicts $25.89474-0.14645(43.035)\approx19.59226$, agreeing with the rounded outcome mean. This is the mean-fitting identity expected of least squares with an intercept. It does not validate every other output field. Individual scores can deviate substantially from these fitted means, and a cross-sectional age contrast is not an estimate of each person's change as they age.

The [intercept](../../../regression-intercept.md) of about 25.895 is the fitted mean at age zero. Zero lies outside the observed age range, so that direct interpretation is an extrapolation. Its test is not a test of whether age predicts diversity. The source's intercept row is internally inconsistent: $25.89474/6.30222\approx4.10883$, not the displayed 4.13. At 1782 residual [statistical degrees of freedom](../../../statistical-degrees-of-freedom.md), these imply two-sided p-values of about $0.0000416$ and $0.0000380$, respectively, neither of which is the printed 0.00012. These differences exceed the displayed rounding precision, although each isolated p-value would still indicate a nonzero intercept at conventional levels. More importantly, its printed [standard error](../../../standard-error.md) is incompatible with the supplied predictor summary and residual error scale, as checked below.

The slope row is much more internally coherent: $-0.14645/0.01396\approx-10.4907$, agreeing with the displayed $t=-10.49$. There are $1784-2=1782$ residual [statistical degrees of freedom](../../../statistical-degrees-of-freedom.md), matching the output. Under the specified linear-model assumptions, this slope test strongly rejects $H_0:\beta_1=0$; its calculated two-sided [p-value](../../../p-value.md) is about $5.0\times10^{-25}$, consistent with the displayed upper bound $2\times10^{-16}$. The F test with 1 and 1782 degrees of freedom, $F\approx110$, has about the same tail probability and tests the same zero-slope hypothesis. The significance stars merely encode thresholds; these are not independent pieces of evidence.[Value: coefficient estimate, standard-error, t/p columns and F statistic](../../../summarizing-linear-model-fits-in-the-r-documentation.md)

Conditional on the printed slope and its standard error, a 95% [confidence interval](../../../confidence-interval.md) is approximately

$$
\boxed{\beta_1\in[-0.17383,-0.11907]\text{ diversity points per year}.}
$$

That interval is a conditional reading of the coherent slope fields, not a raw-data refit. A [p-value](../../../p-value.md) is not the probability of a causal age effect, and the [confidence interval](../../../confidence-interval.md) relies on the sampling and error model. Even a well-estimated observational association does not isolate age from other measured or unmeasured determinants of media use.

The printed [coefficient of determination](../../../coefficient-of-determination.md), $R^2=0.15816$, would mean that the fitted line accounts for 15.816% of the sample's centred diversity [sum of squares](../../../sum-of-squares.md), relative to an intercept-only fit. It would not mean that age causes 15.816% of diversity or correctly predicts that proportion of respondents. But the [simple-regression output identities](../../../simple-regression-output-identities.md) require

$$
F=\frac{(n-2)R^2}{1-R^2}=t_{\mathrm{slope}}^2.
$$

Here the supplied $R^2$ implies $F\approx334.792$, not 110, whereas $F=110$ implies $R^2\approx0.05814$. The printed slope and the two standard deviations independently give correlation $\widehat r=\widehat\beta_1s_x/s_y\approx-0.24116$, whose square is about 0.05816. These mutually compatible fields suggest an explained fraction around 5.8% _if they are trusted_, rather than the printed 15.816%. No unique replacement value is claimed.

The [adjusted coefficient of determination](../../../adjusted-coefficient-of-determination.md) is also inconsistent. Using the printed $R^2$ and sample size gives $1-(1-0.15816)(1783/1782)\approx0.1576876$, which cannot round to the printed 0.15763. Its conceptual purpose is to penalize the unadjusted fit measure for estimating the extra predictor, not to supply a separate effect estimate or significance test. It cannot repair the more substantial F–$R^2$ conflict.

The [residual standard error](../../../residual-standard-error.md) of 9.94 points estimates unexplained response spread, not uncertainty in the slope and not a guaranteed error bound for every prediction. It approximately agrees with the smaller implied $R^2$: $1-(9.94^2\times1782)/(10.240^2\times1783)\approx0.05826$. The printed $R^2=0.15816$ would instead imply residual standard error about 9.398. Rounding on those fields cannot bridge the difference. Thus uncertainty and fit must be read in internally compatible groups rather than mixed indiscriminately.

In a simple ordinary least-squares model, $S_{xx}=(n-1)s_x^2$ and

$$
\operatorname{SE}(\widehat\beta_1)=\frac{s}{\sqrt{S_{xx}}},\qquad
\operatorname{SE}(\widehat\beta_0)=s\sqrt{\frac1n+\frac{\overline x^2}{S_{xx}}}.
$$

With the printed $s=9.94$ and predictor summary, these give slope standard error about 0.0139605, agreeing with the displayed 0.01396, but intercept standard error about 0.64524, not 6.30222. This is a further diagnostic inconsistency, not authority to guess where a decimal point should have been. The [Student t test for a simple-regression intercept](../../../student-t-test-for-a-simple-regression-intercept.md) explains the relevant variance formula.

The residual quantiles extend from about $-23.26$ to $30.31$, with median about $-0.447$ and central quartiles about $-6.799$ and $5.509$. An intercept fit has zero residual mean, not necessarily zero residual median. These five quantiles do not establish a normal error distribution, constant conditional spread or absence of influential observations. A [residual-versus-fitted plot](../../../residual-versus-fitted-plot.md) could assess curvature and changing spread, and a [normal probability plot](../../../normal-q-q-plot.md) could assess error shape; neither can be reconstructed from the supplied summary. An individual [prediction interval](../../../prediction-interval.md) includes residual variation and is wider than a [confidence interval](../../../confidence-interval.md) for a mean response.

Conventional t and F calibration assumes an appropriate linear mean, independent mean-zero errors conditional on age, and [homoscedasticity](../../../homoscedasticity.md); normal errors give the usual exact finite-sample theory. The bounded response scale and observational design call for assessing those assumptions rather than treating significance as model validation. **The coherent coefficient/slope/F fields support a negative association with considerable unexplained individual variation. The printed explanatory-fit and intercept-uncertainty fields require correction before a single definitive numerical summary of the entire model is justified.**

## ↑ Ancestors (10)

1. [6](../6.md)
2. [2018](../../2018-split.md)
3. [Past exam of the digital social research: statistics core course of the University of Oxford](../../split.md)
4. [Digital social research: statistics core course of the University of Oxford](../../../digital-social-research-statistics-core-course-of-the-university-of-oxford.md)
5. [MSc in social science of the internet course of the University of Oxford](../../../msc-in-social-science-of-the-internet-course-of-the-university-of-oxford.md)
6. [Master's course of the University of Oxford](../../../master-s-course-of-the-university-of-oxford.md)
7. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
8. [University of Oxford](../../../university-of-oxford-split.md)
9. [List of universities](../../../list-of-universities.md)
10. [Codex Wiki](../../../split.md)
