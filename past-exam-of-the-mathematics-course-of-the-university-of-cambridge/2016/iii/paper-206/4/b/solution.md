<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For independent patients, the [Bernoulli logistic-regression model](../../../../../../bernoulli-logistic-regression-model.md) is

$$
Y_i\sim\operatorname{Bernoulli}(p_i),\qquad
\log\frac{p_i}{1-p_i}=\beta_0+\beta_aa_i+\beta_fd_i,
$$

where $d_i=\mathbf1_{\{\mathrm{frail}_i=1\}}$ with nonfrail patients as the [reference level in a regression factor](../../../../../../reference-level-in-a-regression-factor.md). The fitted [linear predictor](../../../../../../linear-predictor.md) is

$$
\boxed{\widehat\eta_i=4.25375-0.08942a_i-3.15336d_i,\qquad
\widehat p_i=\frac{e^{\widehat\eta_i}}{1+e^{\widehat\eta_i}}.}
$$

The null model fits one intercept, so its 99 [residual degrees of freedom](../../../../../../residual-degrees-of-freedom.md) imply **100 patients**; the full model's $100-3=97$ confirms this. Unit weights correspond to individual binary responses, not grouped binomial counts.

The [Akaike information criterion](../../../../../../akaike-information-criterion.md) estimates expected relative out-of-sample discrepancy, using the maximized [log-likelihood](../../../../../../log-likelihood.md) plus a complexity penalty:

$$
\operatorname{AIC}=-2\ell(\widehat\beta)+2k,
\qquad
\ell(\beta)=\sum_{i=1}^{100}\left[y_i\eta_i-\log(1+e^{\eta_i})\right].
$$

Here $k=3$, since the Bernoulli dispersion is fixed at one. The saturated model puts probability one on each observed binary outcome and has log likelihood zero, so the [binomial deviance](../../../../../../binomial-deviance.md) is $D=-2\ell(\widehat\beta)$. Consequently

$$
\boxed{\widehat{\operatorname{AIC}}=D+6=61.376+6=67.376.}
$$

There is no estimated error-variance parameter to count. The printed name “Aikake” should be read as Akaike.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
