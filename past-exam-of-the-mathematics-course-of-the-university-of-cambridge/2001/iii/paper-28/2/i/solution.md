<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The missing output is needed to identify the actual regression formula, response column, transformations and coefficient estimates. A useful possible analysis regresses the maintained-school percentage among acceptances on the corresponding percentage among applications, allowing for year; it must be described as a model of college-level composition, not a direct estimate of individual acceptance probabilities.

For instance, if $a_{jt}$ and $p_{jt}$ are these two percentages, a [normal linear model](../../../../../../normal-linear-model.md) might specify $\mathbb E(a_{jt})=\alpha+\beta p_{jt}+\delta\mathbf1_{\{t=2000\}}$, with a slope-by-year [interaction term](../../../../../../interaction-term.md) if needed. The intercept is the expected response at zero predictor, often an extrapolation; the slope is a percentage-point change in acceptance composition per percentage-point change in application composition. A slope of one is not by itself evidence of equal acceptance chances: equal chances within every college would give the entire relation $a_{jt}=p_{jt}$, including zero intercept and no year shift. A fit with positive slope mainly confirms that applicant composition helps predict acceptance composition.

[Regression diagnostics](../../../../../../regression-diagnostics.md) should include residuals versus fitted values and predictors, a residual [normal Q-Q plot](../../../../../../normal-q-q-plot.md), checks of [heteroscedasticity](../../../../../../heteroscedastic.md), [regression leverage](../../../../../../regression-leverage.md), studentized residuals and [Cook's distance](../../../../../../cook-s-distance.md). The aggregate mature-college category merits an influence check and a sensitivity analysis: combining several colleges can conceal different within-college patterns. Repeated observations from the same college across years may have correlated errors, so treating them as independent needs justification. Check nonlinearity, the year interaction and the effects of excluding no observation except with a substantive reason.

Percentages are bounded, and their precision depends on their denominators. A simple [weighted least squares](../../../../../../weighted-least-squares.md) or binomial analysis requires the underlying numbers accepted, not merely percentages. For a proportion based on $m$ people, the working variance is $\pi(1-\pi)/m$ under independent sampling, rather than constant across colleges. If the predictor percentage is itself estimated, an ordinary regression also ignores its uncertainty. The supplied summaries cannot recover all four cells of each college [contingency table](../../../../../../contingency-table.md) or the actual fitted numerical output.

The [published Cambridge percentage table](https://www.admin.cam.ac.uk/reporter/2000-01/special/07/13.html) nevertheless allows a descriptive comparison of acceptance rates. Write $p$ for the maintained-school proportion among applicants and $a$ for its proportion among acceptances. The [relative risk from group compositions](../../../../../../relative-risk-from-group-compositions.md) gives

$$
\boxed{\frac{P(\text{accepted}\mid\text{maintained})}{P(\text{accepted}\mid\text{other})}=\frac{a(1-p)}{p(1-a)}.}
$$

The overall acceptance [probability](../../../../../../probability.md) cancels by [Bayes' theorem](../../../../../../bayes-theorem.md). This [risk ratio](../../../../../../risk-ratio.md) compares acceptance [probabilities](../../../../../../probability.md); it is not the acceptance [odds ratio](../../../../../../odds-ratio.md), which also needs the overall acceptance [probability](../../../../../../probability.md).

For Christ's, the two published application/acceptance pairs give [risk ratios](../../../../../../risk-ratio.md) $37/77\approx0.481$ and $147/187\approx0.786$. If the displayed percentages were rounded to the nearest whole percentage point, the [relative risk bounds from rounded group compositions](../../../../../../relative-risk-bounds-from-rounded-group-compositions.md) give ranges approximately $[0.461,0.501]$ and $[0.755,0.818]$. Thus both comparisons remain below one under that rounding assumption. These are descriptive comparisons of observed groups, without adjustment for applicant qualifications or a [causal effect](../../../../../../causal-effect.md) interpretation. **The published compositions determine approximate relative acceptance rates, but not their [standard errors](../../../../../../standard-error.md) or the original regression results.**

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
