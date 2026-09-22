# Paper 36

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper36.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper36.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
  - [iv](#4/iv)
    - [Solution](#4/iv/solution)
- [5](#5)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)

## 1

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Write $\mathbf1$ for the all-ones vector and set

$$
P_0=\frac{\mathbf1\mathbf1^{\mathsf T}}n,\qquad
P_X=X(X^{\mathsf T}X)^{-1}X^{\mathsf T},\qquad
\nu=n-p-1.
$$

The centering assumption makes $P_0P_X=0$. Thus the full [normal linear model](../../../statistical-modelling.md#normal-linear-model) has fitted-value [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) $P_0+P_X$, and its [residual sum of squares](../../../linear-regression.md#residual-sum-of-squares) is $R=Y^{\mathsf T}(I-P_0-P_X)Y$. Assume $\nu>0$, as is needed to estimate the unknown error [variance](../../../variance.md) from residuals.

For the null that all slopes vanish, the reduced fitted value is $\bar Y\mathbf1$, with residual sum of squares $R_0=Y^{\mathsf T}(I-P_0)Y$. The [F-test](../../../probability-and-statistics.md#f-test) is

$$
\boxed{F=\frac{(R_0-R)/p}{R/\nu}
=\frac{Y^{\mathsf T}P_XY/p}{R/\nu}\sim F_{p,\nu}\quad\text{under the null}}.
$$

Reject for an upper-tail value exceeding the $1-\alpha$ quantile of this [F-distribution](../../../continuous-probability-distribution.md#f-distribution). The required theorem is [Cochran's theorem](../../../statistical-modelling.md#cochran-s-theorem): for an isotropic [normal distribution](../../../probability-theory.md#normal-distribution), projections onto orthogonal subspaces are [independent](../../../random-variable.md#independent-random-variables), and the squared norm on a rank-$r$ subspace divided by $\sigma^2$ has a [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) with $r$ degrees of freedom. Here the null makes the projected mean in $\operatorname{col}(X)$ zero, so $(R_0-R)/\sigma^2\sim\chi_p^2$, independently of $R/\sigma^2\sim\chi_\nu^2$.

Let $p_1,p_2$ be the numbers of columns in the two predictor blocks. To test the first block while retaining the second as nuisance, form

$$
P_2=X_2(X_2^{\mathsf T}X_2)^{-1}X_2^{\mathsf T},\qquad
R_2=Y^{\mathsf T}(I-P_0-P_2)Y.
$$

The [partial F-test for nested linear models](../../../probability-and-statistics.md#partial-f-test-for-nested-linear-models) is

$$
\boxed{F_1=\frac{(R_2-R)/p_1}{R/\nu}\sim F_{p_1,\nu}\quad\text{when }\beta_1=0}.
$$

Again reject in the upper tail. The difference of the nested fitted-value projections has rank $p_1$, is orthogonal to the full residual projection, and annihilates the null mean, which gives the same [independent](../../../random-variable.md#independent-random-variables) chi-squared argument. If a block has no columns, the corresponding test is vacuous.

The phrase [orthogonal statistical parameters](../../../statistical-modelling.md#orthogonal-statistical-parameters) refers to zero cross-block [Fisher information](../../../statistical-modelling.md#fisher-information-matrix), not to the numerical parameter vectors being perpendicular. In this model the cross-block information is $X_1^{\mathsf T}X_2/\sigma^2$, so the [orthogonal coefficient blocks in a centered normal linear model](../../../statistical-modelling.md#orthogonal-coefficient-blocks-in-a-centered-normal-linear-model) condition is

$$
\boxed{X_1^{\mathsf T}X_2=0}.
$$

Then the two fitted subspaces are orthogonal, the block [least-squares estimators](../../../statistical-modelling.md#ordinary-least-squares-estimators) have zero [covariance](../../../variance.md#covariance) and are [independent](../../../random-variable.md#independent-random-variables) because they are jointly Gaussian, and each block's [extra sum of squares](../../../probability-and-statistics.md#extra-sum-of-squares) is unchanged by including the other block. Centering also makes both blocks orthogonal to the intercept.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Both fits are the same additive [two-way analysis of variance](../../../linear-regression.md#two-way-analysis-of-variance) model: a common intercept, five country effects represented by four contrasts, and eight item effects represented by seven contrasts. The three missing cells are omitted, leaving $37$ observations and model rank $1+4+7=12$, hence $25$ residual degrees of freedom. The [residual sum of squares](../../../linear-regression.md#residual-sum-of-squares) is $659.44$ in either ordering, giving

$$
\boxed{\widehat\sigma^2=659.44/25=26.3776,\qquad\widehat\sigma\simeq5.136\text{ pounds}}.
$$

These are [sequential sums of squares](../../../linear-regression.md#sequential-sum-of-squares), so each row measures the improvement when that factor is added after the preceding factors. The country-first sum $1115.56$ describes its unadjusted contribution before accounting for item; its displayed $F=10.573$ and $p=3.73\times10^{-5}$ are not the country-adjusted-for-item test. When country is added after item, its extra sum is $1616.74$, giving

$$
\boxed{F_{\text{country}\mid\text{item}}
=\frac{1616.74/4}{659.44/25}=15.323,\qquad p\simeq1.86\times10^{-6}}.
$$

Thus the additive [normal linear model](../../../statistical-modelling.md#normal-linear-model) gives strong evidence of country differences after accounting for the different products. Conversely, item added after country has extra sum $16910.20$, so

$$
\boxed{F_{\text{item}\mid\text{country}}
=\frac{16910.20/7}{659.44/25}=91.583,\qquad p\simeq3.19\times10^{-16}}.
$$

The printed zero for this [probability](../../../probability-theory.md#probability) is numerical formatting, not a [probability](../../../probability-theory.md#probability) literally equal to zero. Product differences are much larger than residual variation, as expected from their different scales.

The explanation for the order dependence is that [missing cells can destroy factor orthogonality in two-way ANOVA](../../../linear-regression.md#missing-cells-can-destroy-factor-orthogonality-in-two-way-anova). A complete equally replicated crossed design would make centered country and item indicator columns orthogonal. Here the missing observations change the item mix across countries and the country mix across items, so the two factor subspaces are not orthogonal. The two sequential partitions still have the same total explained sum: $1115.56+16910.20=16409.02+1616.74=18025.76$ to the displayed precision. For inference about either factor conditional on the other, compare the full model with the reduced model that omits that factor, rather than interpreting its first-entry sum as adjusted evidence.

The omnibus country test does not identify the particular country contrasts. As an extension, fitting the supplied price table gives the item-adjusted UK-minus-US contrast about $21.33$ pounds, with [standard error](../../../statistical-inference.md#standard-error) $2.824$ and an ordinary Gaussian-model $95\%$ [confidence interval](../../../statistical-inference.md#confidence-interval) approximately $[15.51,27.14]$ pounds. This is a derived model contrast, with [Student t-distribution](../../../continuous-probability-distribution.md#student-s-t-distribution) reference on $25$ degrees of freedom; simultaneous exploration of many country pairs requires control for [multiple hypothesis testing](../../../statistical-modelling.md#multiple-hypothesis-testing).

Check residuals against fitted values, product and country, together with a normal [Q-Q plot](../../../probability-and-statistics.md#q-q-plot) and influential observations. The [homoscedasticity](../../../statistical-model.md#homoscedasticity) assumption on absolute prices may be doubtful because expensive products can have larger absolute variation. A model for logarithmic prices gives multiplicative country effects and can make the scale assumption more plausible. Country-by-item [interaction terms](../../../statistical-model.md#interaction-term) would allow discounts to differ by product, but there is at most one observed value per cell: an unrestricted interaction saturates the $37$ observed means and leaves no pure-error degrees of freedom, so it cannot be tested against [independent](../../../random-variable.md#independent-random-variables) measurement noise from these data alone. Additional products or genuine cell replication would support that extension. The selected products and non-random missing entries also limit claims about a whole country's consumer prices; the conditional inference is for the stated additive model and observed price collection.

## 2

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

For [logistic regression](../../../statistical-modelling.md#logistic-regression), set $\eta_i=x_i^{\mathsf T}\beta$ and $p_i=(1+e^{-\eta_i})^{-1}$. Its Bernoulli [log-likelihood](../../../statistical-modelling.md#log-likelihood), [score function](../../../statistical-modelling.md#informant-function) and [Fisher information](../../../statistical-modelling.md#fisher-information-matrix) are

$$
\ell(\beta)=\sum_i\{y_i\eta_i-\log(1+e^{\eta_i})\},\qquad
U(\beta)=X^{\mathsf T}(y-p),\qquad
I(\beta)=X^{\mathsf T}WX,
$$

where $W=\operatorname{diag}\{p_i(1-p_i)\}$. Solve $U(\beta)=0$ by [Fisher scoring](../../../statistical-modelling.md#scoring-algorithm) or [iteratively reweighted least squares](../../../statistical-modelling.md#iteratively-reweighted-least-squares). One scoring step is

$$
\boxed{\beta^{\rm new}=\beta+(X^{\mathsf T}WX)^{-1}X^{\mathsf T}(y-p)}.
$$

Equivalently regress the working response $z_i=\eta_i+(y_i-p_i)/[p_i(1-p_i)]$ on $X$ using weights $p_i(1-p_i)$. Iterate until the [likelihood](../../../statistical-modelling.md#likelihood-function) and coefficients stabilize, with rank and convergence checks. [Separation in logistic regression](../../../statistical-modelling.md#separation-in-logistic-regression) can prevent a finite maximum: if a predictor direction strictly separates the zeros and ones, moving indefinitely along it improves the [likelihood](../../../statistical-modelling.md#likelihood-function) rather than producing a finite root.

Under the unrestricted model, each individual [probability](../../../probability-theory.md#probability) is estimated independently as $\widehat p_i=y_i$. Every observed binary outcome then has [probability](../../../probability-theory.md#probability) one, so, using boundary limits,

$$
\boxed{\max_{0\le p_i\le1}\ell(p_1,\ldots,p_n)=0}.
$$

The resulting [residual deviance](../../../statistical-modelling.md#residual-deviance) is $D=-2\ell(\widehat\beta)$. It is a legitimate [likelihood](../../../statistical-modelling.md#likelihood-function) contrast and can be used to compare fitted models. However, [individual Bernoulli deviance need not have a chi-squared calibration](../../../statistical-modelling.md#individual-bernoulli-deviance-need-not-have-a-chi-squared-calibration): the saturated model has one boundary-valued parameter for each single observation, and its dimension grows with $n$. The fixed-dimensional regularity behind [Wilks theorem](../../../statistical-inference.md#wilks-theorem) does not justify a $\chi^2_{n-p}$ reference here.

For a concrete demonstration, let the true model contain only an intercept and have success [probability](../../../probability-theory.md#probability) $1/2$. Its fitted [probability](../../../probability-theory.md#probability) is $\bar y$, and

$$
\frac Dn=-2\{\bar y\log\bar y+(1-\bar y)\log(1-\bar y)\}
\longrightarrow2\log2,
$$

whereas a $\chi^2_{n-1}$ variable divided by $n$ converges to one. Thus treating the raw Bernoulli [residual deviance](../../../statistical-modelling.md#residual-deviance) as an ordinary absolute goodness-of-fit statistic can reject a correct model systematically. In contrast, [deviance](../../../exponential-family.md#exponential-family-deviance) differences between fixed-dimensional nested logistic models have their usual asymptotic chi-squared reference under the relevant regularity assumptions. For absolute fit use meaningful replicated covariate groups and [grouped-binomial logistic regression](../../../statistical-modelling.md#grouped-binomial-logistic-regression), or assess residual patterns and prediction on held-out data; a model-specific [parametric bootstrap](../../../statistical-modelling.md#parametric-bootstrap) can calibrate a chosen statistic.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The family-history table contains $462$ men, of whom $160$ have the response present, giving an overall observed fraction $160/462=0.3463$. The unadjusted fractions are $96/192=0.5$ with a positive family history and $64/270=0.2370$ without one. Their crude [odds ratio](../../../statistical-modelling.md#odds-ratio) is $(96/96)/(64/206)=3.219$; this is not the covariate-adjusted effect from the fitted [logistic regression](../../../statistical-modelling.md#logistic-regression).

The full model has an intercept and nine slopes, hence $462-10=452$ residual degrees of freedom. The [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) dispersion is fixed at one. Although the software labels coefficient-to-standard-error ratios as t values, here they are asymptotic normal [Wald statistics](../../../statistical-modelling.md#wald-test), not statistics with an estimated Gaussian residual [variance](../../../variance.md) and an exact Student reference. The full conditional coefficients provide evidence for tobacco, cholesterol, family history, behaviour score and age: their absolute Wald ratios are approximately $2.99,2.92,4.06,3.22,3.73$. The other four ratios are smaller in magnitude, especially alcohol at about $0.027$. These are conditional associations; a weak adjusted coefficient does not by itself establish absence of an underlying association, and [multicollinearity](../../../statistical-modelling.md#multicollinearity) can affect the estimates.

The null [deviance](../../../exponential-family.md#exponential-family-deviance) is $596.1084$ on $461$ degrees of freedom and the full [residual deviance](../../../statistical-modelling.md#residual-deviance) is $472.14$ on $452$. Their difference $123.9684$ has a nominal nine-degree-of-freedom [likelihood-ratio test](../../../statistical-modelling.md#likelihood-ratio-test) reference for the nine slopes jointly. The absolute [residual deviance](../../../statistical-modelling.md#residual-deviance) should not automatically be compared with $\chi^2_{452}$ for the reasons in part (i).

The shown [stepwise selection by the Akaike information criterion](../../../statistical-modelling.md#stepwise-selection-by-the-akaike-information-criterion) follows a backward path. For individual binary observations the saturated [log-likelihood](../../../statistical-modelling.md#log-likelihood) is zero, so

$$
\boxed{\operatorname{AIC}=D+2k},
$$

where $k$ includes the intercept. Removing a one-parameter term improves AIC exactly when the increased [deviance](../../../exponential-family.md#exponential-family-deviance) is less than two. The successive deletions are alcohol, adiposity, blood pressure and obesity. The corresponding $(D,k,\operatorname{AIC})$ values are

$$
\begin{aligned}
&(472.1400,10,492.1400),\quad(472.1408,9,490.1408),\\
&(472.5490,8,488.5490),\quad(473.9799,7,487.9799),\\
&(475.6856,6,487.6856).
\end{aligned}
$$

At the final step, every remaining single-term deletion increases AIC. This is a local stopping condition of the search, not a proof that it found the best subset among all possible models. Obesity is retained for several steps because its successive deletion costs differ after the other terms are removed; the procedure does not simply sort the initial Wald ratios.

For the selected fit, write $H=1$ for positive family history and $H=0$ otherwise. The fitted linear predictor is

$$
\boxed{\widehat\eta=-6.446392+0.0803751\,\mathrm{tobacco}
+0.161991\,\mathrm{ldl}+0.908171H
+0.0371149\,\mathrm{typea}+0.0504598\,\mathrm{age},
\qquad\widehat p=\frac{e^{\widehat\eta}}{1+e^{\widehat\eta}}}.
$$

Holding the other predictors fixed, a unit increase multiplies the odds by $e^{\widehat\beta_j}$. In the same variable order, the unit [odds ratios](../../../statistical-modelling.md#odds-ratio) are

$$
\boxed{1.084,\quad1.176,\quad2.480,\quad1.038,\quad1.052}.
$$

A ten-year age difference multiplies the fitted odds by $1.656$, and ten behaviour-score points by $1.449$. Family history has adjusted [odds ratio](../../../statistical-modelling.md#odds-ratio) about $2.48$, with ordinary fitted-model $95\%$ [confidence interval](../../../statistical-inference.md#confidence-interval) $\exp(0.908171\pm1.96\times0.225603)\simeq[1.59,3.86]$. The intercept is the log odds at zero numerical covariates and absent family history; that extrapolated baseline is not a typical man's risk. Odds ratios are not risk ratios.

The selected model's residual degrees of freedom are $456$, consistent with its six coefficients. All five retained slopes have nominal normal-Wald $p$ values below $0.004$ in that model, but these tests and [confidence intervals](../../../statistical-inference.md#confidence-interval) do not incorporate the prior [model selection](../../../statistical-modelling.md#model-selection). Its improvement over the intercept-only fit is $596.1084-475.6856=120.4228$ on five nominal degrees of freedom; it loses only $3.5456$ [deviance](../../../exponential-family.md#exponential-family-deviance) units relative to the nine-slope fit while using four fewer parameters. Selection optimism remains relevant to predictive performance. Check possible nonlinear continuous-predictor effects, influential observations and clinically motivated interactions; assess out-of-sample discrimination and agreement of predicted [probabilities](../../../probability-theory.md#probability) with observed frequencies by [cross-validation](../../../statistical-learning.md#cross-validation) or external data. The printed output alone does not supply those diagnostics, and the selected high-risk male population limits extrapolation to other populations. Nothing here establishes causal effects of these observational predictors.

## 3

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Use $e_{ij}$ for the expected accident count, not for the accident rate. With a design row $z_{ij}$ consisting of an intercept, seven non-reference site indicators and the after-treatment indicator,

$$
e_{ij}=p_{ij}\exp(\mu+\alpha_i+\beta_j),\qquad
\ell=\sum_{ij}\{y_{ij}(\log p_{ij}+z_{ij}^{\mathsf T}\gamma)-e_{ij}-\log(y_{ij}!)\}.
$$

Here $\log p_{ij}$ is a known [generalized linear model offset](../../../statistical-modelling.md#generalized-linear-model-offset), with coefficient fixed at one. Differentiating the [Poisson regression](../../../statistical-modelling.md#poisson-regression) [log-likelihood](../../../statistical-modelling.md#log-likelihood) gives the [score function](../../../statistical-modelling.md#informant-function) equations

$$
\boxed{\sum_{ij}(y_{ij}-e_{ij})=0,\qquad
\sum_{j=1}^2(y_{ij}-e_{ij})=0\ (i=2,\ldots,8),\qquad
\sum_{i=1}^8(y_{i2}-e_{i2})=0}.
$$

These nine equations estimate the intercept, seven site contrasts and one treatment contrast, with the stated reference-level constraints.

The [Fisher information](../../../statistical-modelling.md#fisher-information-matrix) is $Z^{\mathsf T}WZ$, where $W=\operatorname{diag}(e_{ij})$. A [Fisher scoring](../../../statistical-modelling.md#scoring-algorithm) update adds $(Z^{\mathsf T}WZ)^{-1}Z^{\mathsf T}(y-e)$ to the current coefficient vector. In [iteratively reweighted least squares](../../../statistical-modelling.md#iteratively-reweighted-least-squares), the working response is $z^*_{ij}=\log e_{ij}+(y_{ij}-e_{ij})/e_{ij}$; regress $z^*_{ij}-\log p_{ij}$ on the design with weights $e_{ij}$. Thus the reported four iterations solve the [likelihood](../../../statistical-modelling.md#likelihood-function) equations while accounting for unequal exposure periods.

The common adjusted [rate ratio](../../../statistical-modelling.md#rate-ratio) is obtained by exponentiating the after coefficient:

$$
\boxed{\widehat r=e^{-0.7806616}\simeq0.4581}.
$$

This estimates a $54.2\%$ lower accident rate after the intervention, conditional on the additive site model. The [standard error](../../../statistical-inference.md#standard-error) $0.2751810$ gives normal [Wald statistic](../../../statistical-modelling.md#wald-test) $-2.8369$, two-sided $p\simeq0.0046$, and an approximate $95\%$ [confidence interval](../../../statistical-inference.md#confidence-interval) for the [rate ratio](../../../statistical-modelling.md#rate-ratio)

$$
\boxed{\exp[-0.7806616\pm1.96(0.2751810)]\simeq[0.267,0.786]}.
$$

The label t value is again a normal-reference Wald ratio under fixed Poisson dispersion, rather than an exact Student statistic.

The intercept gives the before rate at reference site one: $e^{0.2707792}\simeq1.311$ accidents per year. The seven site coefficients are log baseline-[rate ratios](../../../statistical-modelling.md#rate-ratio) relative to that site. In site order two through eight, their exponentials are about $0.615,2.767,1.711,0.769,1.797,0.615,1.221$. The third site has the largest estimated rate and a nominal Wald ratio about $3.118$ against the reference. These are adjusted baseline comparisons, not differences in absolute accident counts. The overall unadjusted before/after [rate ratio](../../../statistical-modelling.md#rate-ratio) is $(15/18)/(114/68)\simeq0.497$, and it differs from $0.458$ because site risks and their relative exposure weights differ.

An [independent](../../../random-variable.md#independent-random-variables) way to solve the fit is the [profile likelihood for a common Poisson rate ratio with unequal exposures](../../../statistical-modelling.md#profile-likelihood-for-a-common-poisson-rate-ratio-with-unequal-exposures). Put $t_i=y_{i1}+y_{i2}$ and $\lambda_i=\exp(\mu+\alpha_i)$. For fixed $r$, the site score gives $\widehat\lambda_i=t_i/(p_{i1}+rp_{i2})$. The remaining equation is

$$
\sum_i\frac{t_i r p_{i2}}{p_{i1}+rp_{i2}}=15.
$$

Its positive root reproduces the reported treatment estimate. Comparing the same site model with $r=1$ to the fitted model gives a [deviance](../../../exponential-family.md#exponential-family-deviance) improvement about $9.750$ on one degree of freedom, with nominal likelihood-ratio $p\simeq0.0018$.

There are $16$ count observations and $9$ fitted mean parameters, leaving $7$ residual degrees of freedom. The [null deviance](../../../statistical-modelling.md#null-deviance) $132.9485$ on $15$ degrees of freedom is for the intercept-only rate model, still including the exposure offset. The residual [Poisson deviance](../../../statistical-modelling.md#poisson-deviance) is $16.27524$ on $7$ degrees of freedom. A chi-squared comparison gives approximately $p=0.023$, suggesting potential lack of fit of a single common treatment ratio; the extreme [deviance residuals](../../../statistical-modelling.md#deviance-residual) near $-2.03$ and $2.14$ also deserve inspection. Several after-cell expected counts are below one or near two, so this absolute-fit calibration is only approximate. Site-specific treatment effects, [overdispersion](../../../exponential-family.md#overdispersion) or temporal dependence are possible explanations to investigate, with a [parametric bootstrap](../../../statistical-modelling.md#parametric-bootstrap) available to calibrate the sparse-count fit statistic. A before/after association alone does not isolate a causal effect from secular changes or [regression to the mean](../../../statistical-modelling.md#regression-to-the-mean) at selected sites.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

The [Poisson regression margin-matching score equations](../../../statistical-modelling.md#poisson-regression-margin-matching-score-equations) from the site indicator for each $i\ge2$ directly give

$$
\sum_j e_{ij}=\sum_j y_{ij}\qquad(i=2,\ldots,8).
$$

Subtracting these seven row balances from the intercept equation $\sum_{ij}e_{ij}=\sum_{ij}y_{ij}$ gives the missing reference row balance. Therefore

$$
\boxed{\sum_j e_{ij}=\sum_j y_{ij}\quad\text{for every site }i}.
$$

The after-indicator score similarly gives $\sum_i e_{i2}=\sum_i y_{i2}$. Subtracting it from the intercept balance yields the before-column balance, so

$$
\boxed{\sum_i e_{ij}=\sum_i y_{ij}\quad(j=1,2)}.
$$

Thus the fitted before and after count totals are $114$ and $15$, and each fitted site total equals its observed total. These identities concern expected counts $e_{ij}=p_{ij}\widehat\mu_{ij}$; unequal exposures do not imply corresponding unweighted sums of fitted rates equal sums of observed rates. They follow from the unpenalized canonical Poisson [likelihood](../../../statistical-modelling.md#likelihood-function) and the available intercept/factor columns, not from balanced exposure periods.

## 4

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

The first approach specifies marginal means, [variances](../../../variance.md) and an exchangeable correlation for each student's repeated counts. It is a moment model suitable for a [generalized estimating equation](../../../statistical-inference.md#generalized-estimating-equation); equality of the mean and [variance](../../../variance.md) alone does not specify a full Poisson joint distribution. Different students supply [independent](../../../random-variable.md#independent-random-variables) sampling clusters, while the three counts within a student are dependent.

The second approach is a [Poisson generalized linear mixed model](../../../statistical-modelling.md#poisson-generalized-linear-mixed-model) with a positive shared random multiplier $U_i=e^{b_i}$. Conditional on it, the three counts are [independent](../../../random-variable.md#independent-random-variables) Poisson variables; integrating over it gives a fully specified dependent joint law. The [gamma random-intercept Poisson model](../../../statistical-modelling.md#gamma-random-intercept-poisson-model) uses Gamma shape $\tau^2/\theta$ and rate $\tau/\theta$, so $\mathbb E U_i=\tau$ and $\operatorname{Var}(U_i)=\theta$. Treat the covariates as fixed, with the same multiplier distribution across covariate/treatment groups, as required by this model.

Let $a_{ij}=\exp(\beta_0+\beta^{\mathsf T}x_{ij})$ and $m_{ij}=\mathbb E Y_{ij}$. The [law of total expectation](../../../measure-theory.md#law-of-total-expectation), [law of total variance](../../../probability-theory.md#law-of-total-variance) and [law of total covariance](../../../variance.md#law-of-total-covariance) give

$$
\boxed{m_{ij}=\tau a_{ij},\qquad
\operatorname{Var}(Y_{ij})=\tau a_{ij}+\theta a_{ij}^2,\qquad
\operatorname{Cov}(Y_{ij},Y_{ik})=\theta a_{ij}a_{ik}\quad(j\ne k)}.
$$

Thus each marginal is a [negative binomial distribution](../../../discrete-probability-distribution.md#negative-binomial-distribution) by the [Poisson-gamma mixture](../../../discrete-probability-distribution.md#poisson-gamma-mixture), rather than generally a Poisson variable. Put $\kappa=\theta/\tau^2$. Its [variance](../../../variance.md) is $m_{ij}+\kappa m_{ij}^2$, and the marginal correlation is

$$
\boxed{\operatorname{Corr}(Y_{ij},Y_{ik})
=\frac{\kappa\sqrt{m_{ij}m_{ik}}}
{\sqrt{(1+\kappa m_{ij})(1+\kappa m_{ik})}}}.
$$

It is positive but usually depends on the two marginal means, so it need not be the common exchangeable correlation proposed in the first approach. The first method focuses on population mean effects with a chosen [working correlation matrix](../../../statistical-inference.md#working-correlation-matrix); the second models latent student heterogeneity and separates conditional Poisson variation from additional marginal variation. Correctly specified [likelihood](../../../statistical-modelling.md#likelihood-function) inference for the second uses more distributional assumptions, while the first can retain valid mean inference despite a wrong working [covariance](../../../variance.md#covariance) by using a cluster-level sandwich [variance](../../../variance.md).

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

For the marginal mean model, $e^{\beta_0}$ is the expected term count for a student with all recorded covariates at their reference or zero values. If the treatment indicator is one for the new therapy and zero for the reference treatment, then $e^{\beta_1}$ is the ratio of population mean counts under the two treatments, holding the remaining covariates fixed. Values below one mean a reduced expected count; $100(1-e^{\beta_1})\%$ is the corresponding percentage reduction.

For the random-intercept model, $e^{\beta_0}$ is the conditional reference count at $b_i=0$, or multiplier $U_i=1$; the conditional baseline for student $i$ is $U_i e^{\beta_0}$. It is not automatically the mean-population baseline, which is $\tau e^{\beta_0}$. The conditional treatment [rate ratio](../../../statistical-modelling.md#rate-ratio) for students with the same multiplier is $e^{\beta_1}$. Because the multiplier has the same distribution in the treatment groups and the mean uses a [logarithmic link function](../../../statistical-modelling.md#logarithmic-link-function), that is also the marginal treatment [rate ratio](../../../statistical-modelling.md#rate-ratio). This is the property that [marginal and conditional slopes agree for an independent log-link random intercept](../../../statistical-modelling.md#marginal-and-conditional-slopes-agree-for-an-independent-log-link-random-intercept).

The parameter $\theta$ is the [variance](../../../variance.md) of the positive student multiplier, not a Poisson sampling [variance](../../../variance.md) or a treatment coefficient. Greater $\theta$ at fixed $\tau$ means greater heterogeneity in underlying propensity and larger between-term [covariance](../../../variance.md#covariance). Its extra contribution to the count [variance](../../../variance.md) is $\theta a_{ij}^2$. If $\tau=1$ is imposed, $\theta$ is also the relative multiplier [variance](../../../variance.md); otherwise the relative heterogeneity is $\theta/\tau^2$.

There is a necessary [identifiability](../../../statistical-model.md#identifiability) qualification: if the multiplier mean $\tau$ is also unrestricted, [scale identifiability in a gamma random-intercept Poisson model](../../../statistical-modelling.md#scale-identifiability-in-a-gamma-random-intercept-poisson-model) shows that replacing

$$
(U_i,\beta_0,\tau,\theta)\longmapsto
(cU_i,\beta_0-\log c,c\tau,c^2\theta)
$$

leaves the response law unchanged. Consequently only $\beta_0+\log\tau$ and $\theta/\tau^2$, together with the slopes, are identified from these counts without a scale convention. **Fixing the multiplier mean, usually to one, is needed to interpret the conditional intercept and heterogeneity scale separately**.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Integrating the conditional mean in the [gamma random-intercept Poisson model](../../../statistical-modelling.md#gamma-random-intercept-poisson-model) gives

$$
\mathbb E(Y_{ij}\mid x_{ij})
=\mathbb E(e^{b_i})\exp(\beta_0+\beta^{\mathsf T}x_{ij})
=\tau\exp(\beta_0+\beta^{\mathsf T}x_{ij}),
$$

and hence

$$
\boxed{\log\mathbb E(Y_{ij}\mid x_{ij})
=(\beta_0+\log\tau)+\beta^{\mathsf T}x_{ij}}.
$$

The marginal model's logarithmic mean family is therefore correctly specified, with a shifted intercept and identical slopes. Under the usual [independent](../../../random-variable.md#independent-random-variables)-cluster and estimating-equation regularity conditions, fitting that marginal mean consistently estimates

$$
\boxed{\beta_{0,\mathrm{marginal}}=\beta_0+\log\tau,
\qquad\beta_{\mathrm{marginal}}=\beta}.
$$

Thus the treatment and other slopes estimate the intended marginal log [rate ratios](../../../statistical-modelling.md#rate-ratio); indeed they also coincide with the conditional slopes under the stated common random-effect distribution. The intercept consistently estimates the marginal baseline, but not the conditional $b_i=0$ intercept unless $\tau=1$. If the first investigator interprets the intercept as a conditional latent-student baseline without recognizing this shift, that interpretation is incorrect.

The assumed Poisson marginal [variance](../../../variance.md) and constant correlation generally fail under this random-effect law. They need not invalidate mean-coefficient consistency for a suitable [generalized estimating equation](../../../statistical-inference.md#generalized-estimating-equation), because the expected residual vector is still zero at the true marginal mean. They do invalidate naive [standard errors](../../../statistical-inference.md#standard-error) based only on that assumed [covariance](../../../variance.md#covariance); robust inference requires the correction in part (iv). The simple unchanged-slope result relies on the random multiplier distribution not changing with covariates, rather than on a universal equivalence of marginal and conditional regression models.

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#4/iv)

Use a [generalized estimating equation](../../../statistical-inference.md#generalized-estimating-equation) with any well-behaved positive-definite [working correlation matrix](../../../statistical-inference.md#working-correlation-matrix). Let $\gamma$ collect the marginal intercept and slopes, let $m_i(\gamma)$ be the vector of three correct marginal means, and put $D_i=\partial m_i/\partial\gamma^{\mathsf T}$. Write the working [covariance](../../../variance.md#covariance) as $V_i=A_i^{1/2}R_i(\alpha)A_i^{1/2}$, where the proposed Poisson [variance](../../../variance.md) gives $A_i=\operatorname{diag}(m_i)$; working [independence](../../../random-variable.md#independent-random-variables) is also allowed. Solve

$$
\boxed{\sum_{i=1}^mD_i^{\mathsf T}V_i^{-1}(Y_i-m_i)=0}.
$$

At the true mean, each cluster residual has [expectation](../../../probability-theory.md#expected-value) zero, so the estimating equation is unbiased regardless of whether $V_i$ equals the actual [covariance](../../../variance.md#covariance). With [independent](../../../random-variable.md#independent-random-variables) students, sufficient covariate variation and regularity as $m\to\infty$, this gives consistent mean coefficients.

Replace the model-based [covariance](../../../variance.md#covariance) by the cluster-level [sandwich covariance matrix](../../../statistical-inference.md#sandwich-covariance-matrix). Evaluated at the fitted values, define

$$
\widehat A=\sum_iD_i^{\mathsf T}V_i^{-1}D_i,\qquad
\widehat B=\sum_iD_i^{\mathsf T}V_i^{-1}r_ir_i^{\mathsf T}V_i^{-1}D_i,
\qquad r_i=Y_i-\widehat m_i.
$$

Then

$$
\boxed{\widehat{\operatorname{Cov}}(\widehat\gamma)
=\widehat A^{-1}\widehat B\widehat A^{-1}}.
$$

The residual outer products estimate the actual within-student variability, including correlations and extra-Poisson [variance](../../../variance.md) absent from the working model. Use these [standard errors](../../../statistical-inference.md#standard-error) for asymptotic [Wald tests](../../../statistical-modelling.md#wald-test) and [confidence intervals](../../../statistical-inference.md#confidence-interval); exponentiating the treatment coefficient and its interval gives the mean-count [rate ratio](../../../statistical-modelling.md#rate-ratio) and interval. Treating the $3m$ observations as [independent](../../../random-variable.md#independent-random-variables) when forming the sandwich meat would miss the within-student dependence. The effective asymptotic replication is the number of students, so a small number of clusters requires further finite-sample care rather than assuming that three measurements per student repair the large-sample approximation.

## 5

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

For [independent](../../../random-variable.md#independent-random-variables) Poisson counts, the [log-likelihood](../../../statistical-modelling.md#log-likelihood) at mean vector $\mu$ is

$$
\ell(\mu)=\sum_i\{y_i\log\mu_i-\mu_i-\log(y_i!)\}.
$$

The saturated model maximizes each cell separately at $\widehat\mu_i=y_i$, including the boundary value zero. If $e_i$ is the fitted mean under the log-linear regression, twice the saturated-minus-fitted [log-likelihood](../../../statistical-modelling.md#log-likelihood) is the full [Poisson deviance](../../../statistical-modelling.md#poisson-deviance)

$$
D=2\sum_i\left\{y_i\log\frac{y_i}{e_i}-y_i+e_i\right\},
$$

with $0\log(0/e_i)=0$ understood by continuity. The fitted intercept has [score function](../../../statistical-modelling.md#informant-function) $\partial\ell/\partial\mu=\sum_i(y_i-e_i)$, since differentiating the logarithmic mean with respect to that intercept gives one. Its maximum-likelihood equation therefore gives $\sum_i e_i=\sum_i y_i$. This is why [Poisson deviance simplifies when an intercept is fitted](../../../statistical-modelling.md#poisson-deviance-simplifies-when-an-intercept-is-fitted):

$$
\boxed{D=2\sum_i y_i\log(y_i/e_i)}.
$$

Without the fitted unpenalized intercept, one cannot generally discard the two linear terms. The individual logarithmic terms in the simplified sum need not each be positive; nonnegativity belongs to the full [deviance](../../../exponential-family.md#exponential-family-deviance), or to the full cell contributions before cancellation.

For the approximation, write $y_i=e_i+r_i$ and expand $\log(1+r_i/e_i)$. When relative residuals are small,

$$
\begin{aligned}
2\left\{(e_i+r_i)\log\left(1+\frac{r_i}{e_i}\right)-r_i\right\}
&=\frac{r_i^2}{e_i}-\frac{r_i^3}{3e_i^2}
+O\left(\frac{r_i^4}{e_i^3}\right).
\end{aligned}
$$

Consequently the [quadratic Pearson approximation to the Poisson deviance](../../../statistical-modelling.md#quadratic-pearson-approximation-to-the-poisson-deviance) is

$$
\boxed{D\simeq\sum_i\frac{(y_i-e_i)^2}{e_i}},
$$

the [Pearson chi-squared statistic](../../../statistical-modelling.md#pearson-chi-squared-statistic) for unit Poisson dispersion. Adequate expected counts and small relative residuals are what make the quadratic approximation useful; it is not an exact identity and can be poor for sparse cells, especially a zero count with positive fitted mean. Any further chi-squared goodness-of-fit reference needs its own large-count regularity assumptions.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

With the negative-binomial size $\theta>0$ held fixed, collect all mean-[independent](../../../random-variable.md#independent-random-variables) terms into $c(y_i,\theta)$. The cell [log-likelihood](../../../statistical-modelling.md#log-likelihood) is

$$
\ell_i(\mu_i)=c(y_i,\theta)+y_i\log\mu_i-(y_i+\theta)\log(\mu_i+\theta).
$$

Its derivative is

$$
\ell_i'(\mu_i)=\frac{y_i}{\mu_i}-\frac{y_i+\theta}{\mu_i+\theta}
=\frac{\theta(y_i-\mu_i)}{\mu_i(\mu_i+\theta)}.
$$

For $y_i>0$ it is positive below $y_i$ and negative above $y_i$, so the saturated maximum is at $\mu_i=y_i$. For $y_i=0$, the maximum is the boundary limit $\mu_i\downarrow0$. Evaluating the saturated-minus-fitted [log-likelihood](../../../statistical-modelling.md#log-likelihood) gives the [negative binomial deviance](../../../statistical-modelling.md#negative-binomial-deviance)

$$
\boxed{D_n=2\sum_i y_i\log\frac{y_i}{e_i}
-2\sum_i(y_i+\theta)\log\frac{y_i+\theta}{e_i+\theta}}.
$$

All gamma-function and factorial terms cancel because the same known $\theta$ is used in both models. The zero-count logarithmic term is interpreted as zero; its remaining cell contribution is $2\theta\log(1+e_i/\theta)\ge0$. No intercept score cancellation is required for this formula, so it applies to the specified design whether or not its covariates include an intercept.

For completeness, the fitted coefficients obey the score equations of the [fixed-size negative binomial generalized linear model](../../../statistical-modelling.md#fixed-size-negative-binomial-generalized-linear-model),

$$
\sum_i x_i\frac{\theta(y_i-e_i)}{\theta+e_i}=0,\qquad e_i=\exp(\widehat\beta^{\mathsf T}x_i).
$$

The logarithmic link is not the canonical link for this family, but it produces the requested positive means. As a check, when $\theta\to\infty$,

$$
(y_i+\theta)\log\frac{y_i+\theta}{e_i+\theta}\longrightarrow y_i-e_i,
$$

so the formula tends to the full [Poisson deviance](../../../statistical-modelling.md#poisson-deviance), including the linear terms when an intercept-balance equation is unavailable. The size $\theta$ used here is the negative-binomial size parameter; it is distinct from the random-multiplier [variance](../../../variance.md) denoted by the same letter in Question 4.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
