<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The first fit is a [Bernoulli logistic-regression model](../../../../../../bernoulli-logistic-regression-model.md) for the probability of a positive response. Its fitted [linear predictor](../../../../../../linear-predictor.md) is

$$
\widehat\eta=-9.772794+0.103181\,\mathrm{npreg}+0.032116\,\mathrm{glu}-0.004767\,\mathrm{bp}-0.001917\,\mathrm{skin}+0.083621\,\mathrm{bmi}+1.820337\,\mathrm{ped}+0.041182\,\mathrm{age},
$$

and its fitted [probability](../../../../../../probability.md) is $\widehat\pi=(1+e^{-\widehat\eta})^{-1}$. There are eight coefficients. The null [degrees of freedom](../../../../../../degree-of-freedom.md) identify $n=200$, and the residual [degrees of freedom](../../../../../../degree-of-freedom.md) are $200-8=192$.

Each slope is a change in the [log odds](../../../../../../log-odds.md) per unit of its [covariate](../../../../../../covariate.md), holding the others fixed. Exponentiating gives conditional [odds ratios](../../../../../../odds-ratio.md); for example a ten-unit glucose increase multiplies fitted odds by $e^{10(0.032115958)}=1.379$, and a ten-year age increase by $e^{10(0.041182353)}=1.510$. These are changes in odds, not multiplicative changes in probability, and the observational associations are not automatically causal effects. The intercept corresponds to all numerical [covariates](../../../../../../covariate.md) being zero, generally an extrapolation beyond meaningful subjects.

The [standard errors](../../../../../../standard-error.md) come from the inverse [Fisher information matrix](../../../../../../fisher-information-matrix.md) of the [logistic regression](../../../../../../logistic-regression.md). With binomial [dispersion parameter](../../../../../../dispersion-parameter.md) fixed at one, the displayed t ratios are asymptotic normal [Wald statistics](../../../../../../wald-test.md). In the full fit, glucose and the pedigree measure have clear individual evidence of nonzero slopes, with two-sided $p\simeq2.09\times10^{-6}$ and $0.00609$. The body-mass and age terms are borderline, with $p\simeq0.0504$ and $0.0618$; pregnancy count is weaker, $p\simeq0.110$. Blood pressure and skinfold have little individual evidence after adjustment. These labels should not be converted into a claim that the weaker predictors have no effect, or used as automatic model-selection rules.

A [deviance residual](../../../../../../deviance-residual.md) here is

$$
r_i^D=\operatorname{sign}(y_i-\widehat\pi_i)\sqrt{-2\{y_i\log\widehat\pi_i+(1-y_i)\log(1-\widehat\pi_i)\}}.
$$

Its square is the observation's contribution to [binomial deviance](../../../../../../binomial-deviance.md), so the squared residuals sum to the printed [residual deviance](../../../../../../residual-deviance.md). The five-number summaries describe the distribution of these signed residuals. The null deviance $256.4142$ belongs to an intercept-only [logistic regression](../../../../../../logistic-regression.md); the full fitted deviance is $178.3907$. Four [Fisher scoring](../../../../../../scoring-algorithm.md) iterations record convergence of the numerical likelihood fit.

The second model uses only glucose:

$$
\widehat\eta=-5.503635+0.03778371\,\mathrm{glu}.
$$

Its two coefficients leave $198$ residual [degrees of freedom](../../../../../../degree-of-freedom.md). A ten-unit glucose increase multiplies its fitted odds by $e^{0.3778371}\simeq1.459$. This differs from the adjusted multiplier $1.379$, because the models condition on different [covariates](../../../../../../covariate.md); both adjustment and [noncollapsibility of the odds ratio](../../../../../../noncollapsibility-of-the-odds-ratio.md) can change logistic coefficients. The glucose-only model has deviance $207.3727$, so its maximized [log-likelihood](../../../../../../log-likelihood.md) is lower than the full model's.

For these fixed-dimensional nested models, [analysis of deviance](../../../../../../analysis-of-deviance-for-nested-generalized-linear-models.md) and [Wilks theorem](../../../../../../wilks-theorem.md) give

$$
\begin{array}{c|c|c|c}
\text{comparison}&\text{deviance reduction}&\text{df}&\text{approximate }p\\\hline
\text{null to full}&78.0235&7&3.48\times10^{-14}\\
\text{null to glucose only}&49.0415&1&2.51\times10^{-12}\\
\text{glucose only to full}&28.9820&6&6.13\times10^{-5}
\end{array}
$$

Thus **the additional six predictors collectively improve the glucose-only model**, even though several individual [Wald tests](../../../../../../wald-test.md) are not significant. These comparisons assume independent subjects, an appropriate logistic mean structure, full rank, and regular finite parameter estimates without [separation](../../../../../../axiom-schema-of-specification.md).

It would be incorrect to infer that absolute fit is good merely because $178.39<192$. [Individual Bernoulli deviance need not have a chi-squared calibration](../../../../../../individual-bernoulli-deviance-need-not-have-a-chi-squared-calibration.md): there is just one binary observation per saturated probability, and the saturated dimension increases with sample size. A simple counterexample is an intercept-only model with true probability $1/2$, for which $D/n\to2\log2$, not one. For absolute adequacy, inspect residual patterns and predicted-risk calibration, use meaningful grouped comparisons when appropriate, or calibrate a chosen fit statistic by [parametric bootstrap](../../../../../../parametric-bootstrap.md). The regular nested-model tests above are not subject to that saturated-model dimensionality problem. Only the displayed summaries and a few example rows are supplied, so patient-level diagnostics or complete numerical refitting cannot be reconstructed from this page alone.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
