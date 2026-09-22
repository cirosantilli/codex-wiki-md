<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**The association is strongly [statistically significant](../../../../../../statistical-significance.md) under the reported regression assumptions, but age alone has only moderate predictive ability.** The reported [confidence interval](../../../../../../confidence-interval.md) for the age [regression coefficient](../../../../../../regression-coefficient.md) excludes zero by a wide margin. If it is the usual two-sided 95% interval from a [normal linear model](../../../../../../normal-linear-model.md) with an intercept and one predictor, there are $206-2=204$ [degrees of freedom](../../../../../../degree-of-freedom.md). Taking $t_{0.975,204}\simeq1.97$ gives

$$
\operatorname{SE}(\widehat\beta)\simeq\frac{0.05}{1.97}=0.0254,
\qquad t_{\rm obs}\simeq\frac{0.22}{0.0254}=8.67.
$$

Thus the two-sided [p-value](../../../../../../p-value.md) against zero slope is far below $0.001$. This conclusion concerns a statistical association in the sampled population; it does not establish an individual growth rate. Clustering by practitioner, nonconstant [variance](../../../../../../variance-split.md) or nonindependent observations would require an appropriate [standard error](../../../../../../standard-error.md) rather than blind reliance on this calculation.

The [scatter plot](../../../../../../scatter-plot.md) has substantial vertical spread at each age. A narrow slope [confidence interval](../../../../../../confidence-interval.md) describes uncertainty about the average trend, whereas a [prediction interval](../../../../../../prediction-interval.md) for a new person's ear length must also include the residual [variance](../../../../../../variance-split.md). The reported interval even permits an approximate numerical assessment: write $S_{xx}=\sum_i(x_i-\bar x)^2$ and let $s_e^2=\mathrm{RSS}/(n-2)$. In [simple linear regression](../../../../../../simple-linear-regression.md), $t^2=\widehat\beta^2S_{xx}/s_e^2$, while the fitted and residual sums of squares are $\widehat\beta^2S_{xx}$ and $(n-2)s_e^2$. Hence the [coefficient of determination](../../../../../../coefficient-of-determination.md) is

$$
\boxed{R^2=\frac{t^2}{t^2+n-2}\simeq0.27.}
$$

Under these assumptions, age explains only about 27% of the sample variation; roughly 73% remains unexplained. The calculation is approximate because the printed slope and interval are rounded. For a new individual aged $x_0$, the usual [prediction interval](../../../../../../prediction-interval.md) is based on

$$
\widehat Y(x_0)\ \pm\ t_{0.975,n-2}s_e
\sqrt{1+\frac1n+\frac{(x_0-\bar x)^2}{S_{xx}}}.
$$

The leading one represents individual residual variation. The provided summaries do not determine $s_e$ and $S_{xx}$ separately, so they do not supply a numerical [prediction interval](../../../../../../prediction-interval.md).

Record sex, height or another measure of body size, ancestry, family characteristics and practitioner or measurement method. Use these [covariates](../../../../../../covariate.md) in a [multiple linear regression](../../../../../../multiple-linear-regression.md), allowing scientifically justified nonlinear age effects or interactions, and assess [prediction error](../../../../../../prediction-error.md) on held-out observations. A guessed overall sex proportion cannot replace individual sex measurements or identify sex-adjusted effects.

There is a source inconsistency: the PDF's numerical ear-length summary is ten times the scale of its plotted measurements and fitted line. Indeed, the fitted line at the reported mean age gives about $67.7$ mm, whereas the printed mean is about ten times larger. Missing decimal points in the summary are a plausible explanation. The significance and approximate $R^2$ above use the mutually consistent slope, interval and graph; they do not treat the inconsistent summary as valid data.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
