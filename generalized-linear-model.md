# Generalized linear model

↑ **Parent:** [Statistical modelling](statistical-modelling.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Generalized_linear_model)

A generalized linear model takes independent responses from an exponential dispersion family and relates their means to linear predictors by $g(\mu_i)=x_i^T\beta$. The response distribution, systematic component, link, dispersion, and known observation weights together specify the model.

**Table of contents**

- [Gamma regression with canonical link](#gamma-regression-with-canonical-link)
- [Generalized linear model offset](#generalized-linear-model-offset)
- [Deviance goodness-of-fit test](#deviance-goodness-of-fit-test)
  - [Individual Bernoulli deviance need not have a chi-squared calibration](#individual-bernoulli-deviance-need-not-have-a-chi-squared-calibration)
- [Deviance residual](#deviance-residual)
- [Generalized additive model](#generalized-additive-model)
  - [Additive regression model](#additive-regression-model)
    - [Identifiability of additive regression components](#identifiability-of-additive-regression-components)
      - [Concurvity](#concurvity)
  - [Backfitting algorithm](#backfitting-algorithm)
    - [Linear backfitting equations](#linear-backfitting-equations)
  - [Generalized additive mixed model](#generalized-additive-mixed-model)
- [Quasi-likelihood](#quasi-likelihood)
  - [Quasibinomial regression](#quasibinomial-regression)
- [Linear predictor](#linear-predictor)
- [Link function](#link-function)
  - [Complementary log-log link](#complementary-log-log-link)
  - [Identity link](#identity-link)
  - [Logit](#logit)
  - [Logarithmic link function](#logarithmic-link-function)
- [Binomial regression](#binomial-regression)
  - [Binomial deviance](#binomial-deviance)
- [Pearson dispersion estimator](#pearson-dispersion-estimator)
  - [Pearson residual](#pearson-residual)
  - [Pearson chi-squared statistic](#pearson-chi-squared-statistic)
- [Canonical link function](#canonical-link-function)
  - [Poisson canonical link](#poisson-canonical-link)
- [Poisson regression](#poisson-regression)
  - [Profile likelihood for a common Poisson rate ratio with unequal exposures](#profile-likelihood-for-a-common-poisson-rate-ratio-with-unequal-exposures)
  - [Concavity of the Poisson regression likelihood](#concavity-of-the-poisson-regression-likelihood)
  - [Poisson slope information after eliminating an intercept](#poisson-slope-information-after-eliminating-an-intercept)
  - [Poisson regression margin-matching score equations](#poisson-regression-margin-matching-score-equations)
  - [Two-group Poisson ratio conditional likelihood](#two-group-poisson-ratio-conditional-likelihood)
    - [Paired Poisson conditional likelihood](#paired-poisson-conditional-likelihood)
      - [Conditional cure-weight equations for paired Poisson counts](#conditional-cure-weight-equations-for-paired-poisson-counts)
  - [Common versus factor-specific slopes in Poisson regression](#common-versus-factor-specific-slopes-in-poisson-regression)
  - [Poisson working models for averaged counts](#poisson-working-models-for-averaged-counts)
  - [Poisson log-rate ratio](#poisson-log-rate-ratio)
  - [Poisson mean saturation at three distinct times](#poisson-mean-saturation-at-three-distinct-times)
  - [Pooling selected slopes in a Poisson regression](#pooling-selected-slopes-in-a-poisson-regression)
  - [Treatment interaction contrast in a Poisson regression](#treatment-interaction-contrast-in-a-poisson-regression)
  - [Poisson deviance](#poisson-deviance)
    - [Quadratic Pearson approximation to the Poisson deviance](#quadratic-pearson-approximation-to-the-poisson-deviance)
    - [Poisson deviance simplifies when an intercept is fitted](#poisson-deviance-simplifies-when-an-intercept-is-fitted)
- [Gamma regression with logarithmic link](#gamma-regression-with-logarithmic-link)
- [Quasi-Poisson regression](#quasi-poisson-regression)
  - [Poisson score linearization under proportional variance](#poisson-score-linearization-under-proportional-variance)
  - [Quasi-score equation](#quasi-score-equation)
- [Negative binomial regression](#negative-binomial-regression)
  - [Fixed-size negative binomial generalized linear model](#fixed-size-negative-binomial-generalized-linear-model)
    - [Negative binomial deviance](#negative-binomial-deviance)
- [Poisson exposure model](#poisson-exposure-model)
  - [Exposure time for a Poisson rate at fixed fractional precision](#exposure-time-for-a-poisson-rate-at-fixed-fractional-precision)
  - [Rate ratio](#rate-ratio)
  - [Finite-exposure Poisson inconsistency](#finite-exposure-poisson-inconsistency)
  - [Estimators for a Poisson exposure model](#estimators-for-a-poisson-exposure-model)
    - [Variance comparison for Poisson exposure estimators](#variance-comparison-for-poisson-exposure-estimators)
  - [Normal-approximation tests for a Poisson exposure model](#normal-approximation-tests-for-a-poisson-exposure-model)
- [Logistic regression](#logistic-regression)
  - [Proportional-odds model](#proportional-odds-model)
  - [Separation in logistic regression](#separation-in-logistic-regression)
  - [Finite maximum-likelihood estimate in a one-parameter logistic model](#finite-maximum-likelihood-estimate-in-a-one-parameter-logistic-model)
  - [Conditional logistic model for longitudinal binary data](#conditional-logistic-model-for-longitudinal-binary-data)
    - [Cumulative-response logistic model](#cumulative-response-logistic-model)
    - [True state dependence](#true-state-dependence)
  - [Multinomial logistic regression](#multinomial-logistic-regression)
    - [Continuation-ratio logits](#continuation-ratio-logits)
    - [Conditional multinomial sufficient statistics](#conditional-multinomial-sufficient-statistics)
  - [Logistic-normal regression with autoregressive random effects](#logistic-normal-regression-with-autoregressive-random-effects)
  - [Logistic model](#logistic-model)
    - [Log odds](#log-odds)
  - [Separation (statistics)](#separation-statistics)
    - [Quasi-complete separation](#quasi-complete-separation)
    - [Complete separation](#complete-separation)
  - [Bernoulli logistic-regression model](#bernoulli-logistic-regression-model)
    - [Fitted-mean balance for logistic regression with an intercept](#fitted-mean-balance-for-logistic-regression-with-an-intercept)
  - [Logistic loss](#logistic-loss)
    - [Positive semidefinite quadratic-form classifier](#positive-semidefinite-quadratic-form-classifier)
  - [L1-penalized logistic regression](#l1-penalized-logistic-regression)
  - [Grouped-binomial logistic regression](#grouped-binomial-logistic-regression)
    - [Baseline logit estimator in a group-factor binomial model](#baseline-logit-estimator-in-a-group-factor-binomial-model)
    - [Denominators in grouped birth-outcome models](#denominators-in-grouped-birth-outcome-models)
  - [Reference level in a regression factor](#reference-level-in-a-regression-factor)
  - [Stochastic block model](#stochastic-block-model)
    - [Spectral norm bound for a centered Bernoulli adjacency matrix](#spectral-norm-bound-for-a-centered-bernoulli-adjacency-matrix)
    - [Logistic stochastic block model](#logistic-stochastic-block-model)
      - [Additive class-effect logistic network model](#additive-class-effect-logistic-network-model)
        - [Degree-sum sufficient statistic for an additive logistic network model](#degree-sum-sufficient-statistic-for-an-additive-logistic-network-model)
- [Probit model](#probit-model)
  - [Latent-normal Gibbs sampler for probit regression](#latent-normal-gibbs-sampler-for-probit-regression)
  - [Threshold observation of a lognormal regression](#threshold-observation-of-a-lognormal-regression)
  - [Probit posterior score](#probit-posterior-score)
- [Iteratively reweighted least squares](#iteratively-reweighted-least-squares)
- [Generalized linear mixed model](#generalized-linear-mixed-model)
  - [Logistic random-intercept model for repeated binary outcomes](#logistic-random-intercept-model-for-repeated-binary-outcomes)
    - [Random-intercept attenuation of marginal logistic slopes](#random-intercept-attenuation-of-marginal-logistic-slopes)
  - [Gaussian linear mixed model](#gaussian-linear-mixed-model)
    - [Correlated random-intercept and random-slope model](#correlated-random-intercept-and-random-slope-model)
    - [Variance component](#variance-component)
      - [Method-of-moments variance component estimate](#method-of-moments-variance-component-estimate)
    - [Best linear unbiased prediction](#best-linear-unbiased-prediction)
    - [Conditional mode of Gaussian random effects](#conditional-mode-of-gaussian-random-effects)
    - [Continuous-time autoregressive residual correlation](#continuous-time-autoregressive-residual-correlation)
    - [Independent random-intercept and random-slope model](#independent-random-intercept-and-random-slope-model)
  - [Poisson generalized linear mixed model](#poisson-generalized-linear-mixed-model)
    - [Gamma random-intercept Poisson model](#gamma-random-intercept-poisson-model)
      - [Scale identifiability in a gamma random-intercept Poisson model](#scale-identifiability-in-a-gamma-random-intercept-poisson-model)
    - [Marginal mean of a Poisson random-slope model](#marginal-mean-of-a-poisson-random-slope-model)
  - [Random intercept](#random-intercept)
    - [Marginal and conditional slopes agree for an independent log-link random intercept](#marginal-and-conditional-slopes-agree-for-an-independent-log-link-random-intercept)
    - [Random-intercept linear mixed model](#random-intercept-linear-mixed-model)

## Gamma regression with canonical link

↑ **Parent:** [Generalized linear model](generalized-linear-model.md)

For a [Gamma distribution](continuous-probability-distribution.md#gamma-distribution) with fixed shape $\alpha$, choose dispersion $\phi=1/\alpha$, canonical parameter $\theta=-1/\mu$, and cumulant $b(\theta)=-\log(-\theta)$. The [canonical link function](#canonical-link-function) is the displayed negative reciprocal; reversing its sign is an equivalent regression convention. For independent observations, the [score function](statistical-modelling.md#informant-function) is $\phi^{-1}X^T(y-\mu)$ and the [Fisher information matrix](statistical-modelling.md#fisher-information-matrix) is $\phi^{-1}X^T\operatorname{diag}(\mu_i^2)X$. The [deviance](exponential-family.md#exponential-family-deviance) is $2\sum_i[y_i/\widehat\mu_i-1-\log(y_i/\widehat\mu_i)]$, with twice the log-likelihood ratio equal to this divided by $\phi$. The fitted mean is the inverse link applied to $X\widehat\beta$, not $X\widehat\beta$ itself.

## Generalized linear model offset

↑ **Parent:** [Generalized linear model](generalized-linear-model.md)

An [offset](#generalized-linear-model-offset) is a known term in a [generalized linear model](generalized-linear-model.md)'s [linear predictor](#linear-predictor), with coefficient fixed to one. With a [log link](#logarithmic-link-function) and exposure $n_i$, choosing $o_i=\log n_i$ gives a mean count $n_i\exp(x_i^T\beta)$. Its role differs from that of a fitted explanatory-variable coefficient.

## Deviance goodness-of-fit test

↑ **Parent:** [Generalized linear model](generalized-linear-model.md)

For a suitably regular [generalized linear model](generalized-linear-model.md), a residual deviance $D$ can be compared approximately with a [chi-squared distribution](probability-distribution.md#chi-squared-distribution) on $n-p$ degrees of freedom to assess fit relative to the saturated model. Sparse or very small expected cell counts can invalidate this reference distribution. A large [p-value](statistical-hypothesis-test.md#p-value) means no detected lack of fit, not proof of correctness; dependence, wrong mean structure or [overdispersion](exponential-family.md#overdispersion) still require diagnostics.

### Individual Bernoulli deviance need not have a chi-squared calibration

↑ **Parent:** [Deviance goodness-of-fit test](#deviance-goodness-of-fit-test)

A [logistic regression](#logistic-regression) fitted to ungrouped [Bernoulli](discrete-probability-distribution.md#bernoulli-distribution) observations has [residual deviance](statistical-hypothesis-test.md#residual-deviance) $D=-2\ell(\widehat\beta)$. Comparing it automatically with $\chi^2_{n-p}$ is generally invalid: the saturated dimension grows with $n$, with one observation per fitted probability. If the true model has only an intercept and success probability $1/2$, then $D/n\to2\log2$, whereas $\chi^2_{n-1}/n\to1$. Fixed-dimensional nested-model [likelihood-ratio tests](statistical-hypothesis-test.md#likelihood-ratio-test) can still use [Wilks theorem](statistical-inference.md#wilks-theorem) under regularity. For absolute fit, use meaningful grouping, residual diagnostics, or a fitted-model [parametric bootstrap](statistical-modelling.md#parametric-bootstrap).

## Deviance residual

↑ **Parent:** [Generalized linear model](generalized-linear-model.md)

A deviance residual is the signed square root of an observation's contribution $d_i$ to fitted-model deviance. For a [Poisson regression](#poisson-regression), $d_i=2[y_i\log(y_i/\widehat\mu_i)-(y_i-\widehat\mu_i)]$, with $0\log0=0$. Its squared sum is the [Poisson deviance](#poisson-deviance). Leverage and estimated dispersion can further standardize these residuals; a normal [quantile-quantile plot](probability-and-statistics.md#q-q-plot) is a diagnostic approximation, not a requirement that count errors have a [normal distribution](probability-distribution.md#normal-distribution).

## Generalized additive model

↑ **Parent:** [Generalized linear model](generalized-linear-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Generalized_additive_model)

A generalized additive model has [linear predictor](#linear-predictor) $g(\mu_i)=\alpha+\sum_j s_j(x_{ij})$. Centering the smooth functions identifies the intercept. The response family and [link function](#link-function) remain part of the model; an unspecified software family must not be inferred from the response name.

### Additive regression model

↑ **Parent:** [Generalized additive model](#generalized-additive-model)

An additive regression model represents a conditional mean as a sum of univariate functions and an intercept. It permits nonlinear effects without estimating a general high-dimensional response surface. The [backfitting algorithm](#backfitting-algorithm) smooths each component's [partial residual](probability-and-statistics.md#partial-residual). Centering separates constants from the intercept, while [concurvity](#concurvity) can still prevent component identification.

// Target: probability-and-statistics.bigb

#### Identifiability of additive regression components

↑ **Parent:** [Additive regression model](#additive-regression-model)

In an [additive regression model](#additive-regression-model), each component can transfer a constant to the [regression intercept](linear-regression.md#regression-intercept), so impose empirical mean-zero constraints, or population mean-zero constraints when appropriate. Even after centering, nonzero component perturbations $h_j$ with $\sum_jh_j(x_{ij})=0$ at every observed point make the additive decomposition nonidentifiable. Extra smoothing penalties may resolve the fitted decomposition, but centering alone does not remove [concurvity](#concurvity).

// Target: probability-and-statistics.bigb

##### Concurvity

↑ **Parent:** [Identifiability of additive regression components](#identifiability-of-additive-regression-components)

Concurvity is the nonlinear analogue of [multicollinearity](normal-linear-model.md#multicollinearity): a function of one predictor is exactly or approximately expressible as a sum of functions of other predictors. Exact concurvity can make an additive decomposition nonunique; approximate concurvity makes components difficult to estimate stably. A unique fitted sum need not imply unique individual components.

// Target: probability-and-statistics.bigb

### Backfitting algorithm

↑ **Parent:** [Generalized additive model](#generalized-additive-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Backfitting_algorithm)

The backfitting algorithm estimates each additive mean function by smoothing its [partial residual](probability-and-statistics.md#partial-residual), obtained after subtracting the current fits of all other terms, and cycling through terms until convergence. Centering each smooth separates its constant part from the intercept. For fixed quadratic smoothness penalties it is block coordinate minimization of a penalized least-squares objective; identifiability and positive definiteness of the constrained problem ensure a unique converged fit. Non-Gaussian [generalized additive models](#generalized-additive-model) can use weighted backfitting inside [iteratively reweighted least squares](#iteratively-reweighted-least-squares).

#### Linear backfitting equations

↑ **Parent:** [Backfitting algorithm](#backfitting-algorithm)

For [linear smoothers](linear-regression.md#linear-smoother), let $C=I-\mathbf1\mathbf1^T/n$ and $T_j=CS_jC$. The centered fixed-point equations of the [backfitting algorithm](#backfitting-algorithm) have diagonal identity blocks and off-diagonal blocks $T_j$. On the centered component space, a consistent system has a unique answer exactly when its homogeneous system has only the zero solution. For two components the reduced equation is $(I-T_1T_2)f_1=T_1(I-T_2)Cy$. A common centered vector reproduced by both smoothers yields opposite perturbations of the components without changing their sum.

// Target: probability-and-statistics.bigb

### Generalized additive mixed model

↑ **Parent:** [Generalized additive model](#generalized-additive-model)

A generalized additive mixed model supplements smooth population effects with latent [random effects](latent-variable.md#random-effect). Given these effects, responses follow a specified response family; integrating them out induces dependence between related observations.

## Quasi-likelihood

↑ **Parent:** [Generalized linear model](generalized-linear-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quasi-likelihood)

[Quasi-likelihood](#quasi-likelihood) specifies a mean and a [variance function](exponential-family.md#variance-function) without necessarily specifying a full response distribution. For independent responses, the estimating equation is $\sum_i (\partial\mu_i/\partial\beta)(y_i-\mu_i)/(\phi V(\mu_i))=0$. A common scalar [dispersion parameter](exponential-family.md#dispersion-parameter) rescales coefficient [covariance](variance.md#covariance) while leaving the roots of the [quasi-score equation](#quasi-score-equation) unchanged.

### Quasibinomial regression

↑ **Parent:** [Quasi-likelihood](#quasi-likelihood)

The logit mean model $p_i=(1+e^{-x_i^T\beta})^{-1}$ with working [variance function](exponential-family.md#variance-function) $\phi p_i(1-p_i)$ has the same coefficient estimates as ordinary binomial [logistic regression](#logistic-regression), but estimates dispersion from residuals. For an actual individual binary random variable, $Y^2=Y$ forces [variance](variance.md) $p(1-p)$, so a nonunit dispersion is a working specification rather than a new independent binary distribution.

## Linear predictor

↑ **Parent:** [Generalized linear model](generalized-linear-model.md)

The linear predictor of a generalized linear model is the linear combination $\eta_i=x_i^T\beta$ of the explanatory variables.

## Link function

↑ **Parent:** [Generalized linear model](generalized-linear-model.md)

A link function connects the response mean to the linear predictor through $g(\mu_i)=\eta_i$.

### Complementary log-log link

↑ **Parent:** [Link function](#link-function)

The [complementary log-log link](#complementary-log-log-link) maps $p\in(0,1)$ to $\ln[-\ln(1-p)]$, with inverse $p=1-\exp(-e^\eta)$. For constant infection hazard $\lambda$ and exposure $e$, $p=1-e^{-\lambda e}$ implies $\operatorname{cloglog}(p)=\ln\lambda+\ln e$. Thus a [binomial regression](#binomial-regression) with a log-exposure [offset](#generalized-linear-model-offset) estimates the log hazard as its intercept.

### Identity link

↑ **Parent:** [Link function](#link-function)

The identity [link function](#link-function) equates the response mean with the [linear predictor](#linear-predictor). In a [generalized linear model](generalized-linear-model.md) it gives $\mu_i=x_i^T\beta$. It is the [canonical link function](#canonical-link-function) for the [normal distribution](probability-distribution.md#normal-distribution). For response families whose means must remain positive or between zero and one, using the identity link requires corresponding restrictions on the [linear predictor](#linear-predictor).

### Logit

↑ **Parent:** [Link function](#link-function)

The logit link maps a mean probability to its [log odds](#log-odds): $g(p)=\log[p/(1-p)]$, $0<p<1$. Its inverse is $p=(1+e^{-\eta})^{-1}$, used in [logistic regression](#logistic-regression).

### Logarithmic link function

↑ **Parent:** [Link function](#link-function)

The logarithmic link maps a positive mean to $\log\mu$. It is the [Poisson canonical link](#poisson-canonical-link).

## Binomial regression

↑ **Parent:** [Generalized linear model](generalized-linear-model.md)

Binomial regression models independent $Y_i\sim\operatorname{Bin}(m_i,p_i)$ and relates $p_i$ to a linear predictor. Logistic and probit regression use the logit and inverse-normal links respectively.

### Binomial deviance

↑ **Parent:** [Binomial regression](#binomial-regression)

For independent binomial counts $Y_i\sim\operatorname{Bin}(m_i,p_i)$ with observed proportions $y_i=Y_i/m_i$ and fitted probabilities $\widehat p_i$, the deviance from the saturated model is

$$
D=2\sum_i m_i\left[y_i\log\frac{y_i}{\widehat p_i}+(1-y_i)\log\frac{1-y_i}{1-\widehat p_i}\right],
$$

with the usual convention $0\log0=0$.

## Pearson dispersion estimator

↑ **Parent:** [Generalized linear model](generalized-linear-model.md)

For a generalized linear model with variance function $V$, the Pearson estimator is

$$
\widehat\phi=\frac1{n-p}\sum_i\frac{(Y_i-\widehat\mu_i)^2}{V(\widehat\mu_i)}.
$$

### Pearson residual

↑ **Parent:** [Pearson dispersion estimator](#pearson-dispersion-estimator)

The Pearson residual is $r_i^P=(Y_i-\widehat\mu_i)/\sqrt{\widehat\phi V(\widehat\mu_i)}$.

### Pearson chi-squared statistic

↑ **Parent:** [Pearson dispersion estimator](#pearson-dispersion-estimator)

The Pearson chi-squared statistic for a generalized linear model is

$$
X_P^2=\sum_i\frac{(Y_i-\widehat\mu_i)^2}{V(\widehat\mu_i)}.
$$

Dividing it by the residual degrees of freedom estimates the dispersion parameter.

## Canonical link function

↑ **Parent:** [Generalized linear model](generalized-linear-model.md)

The canonical link identifies the linear predictor with the exponential family's natural parameter: $g(\mu)=\theta$, where $\mu=b'(\theta)$.

### Poisson canonical link

↑ **Parent:** [Canonical link function](#canonical-link-function)

For a Poisson mean $\mu$, the natural parameter is $\theta=\log\mu$, so the canonical link is the logarithmic link $g(\mu)=\log\mu$.

## Poisson regression

↑ **Parent:** [Generalized linear model](generalized-linear-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poisson_regression)

A Poisson regression models independent count responses by

$$
Y_i\sim\operatorname{Pois}(\mu_i),
\qquad \log\mu_i=x_i^T\beta.
$$

Its likelihood is $\prod_i e^{-\mu_i}\mu_i^{y_i}/y_i!$.

### Profile likelihood for a common Poisson rate ratio with unequal exposures

↑ **Parent:** [Poisson regression](#poisson-regression)

For [independent](random-variable.md#independent-random-variables) counts with means $p_{i1}\lambda_i$ and $p_{i2}\lambda_i r$, let $t_i=y_{i1}+y_{i2}$. Maximizing the [Poisson regression](#poisson-regression) [likelihood](maximum-likelihood-estimation.md#likelihood-function) in each baseline rate gives the displayed estimate. The remaining log-rate-ratio score is

$$
\sum_i\left[y_{i2}-\frac{t_i r p_{i2}}{p_{i1}+rp_{i2}}\right]=0.
$$

Equivalently, conditional on $t_i$, the second count has a [binomial distribution](discrete-probability-distribution.md#binomial-distribution) with success [probability](probability-theory.md#probability) $rp_{i2}/(p_{i1}+rp_{i2})$. Each positive-total term increases strictly with $r$; if both treatment totals are positive, the score has a unique positive root. This reduces a many-parameter fit to a scalar equation.

### Concavity of the Poisson regression likelihood

↑ **Parent:** [Poisson regression](#poisson-regression)

For a full-column-rank design $X$ and positive fitted means $\mu_i=\exp(x_i^T\beta)$, the [log-likelihood](maximum-likelihood-estimation.md#log-likelihood) has Hessian $-X^T\operatorname{diag}(\mu_i)X$, which is negative definite. Thus any finite stationary point is the unique [maximum-likelihood estimator](maximum-likelihood-estimation.md#maximum-likelihood-estimator). Full rank does not guarantee existence: with an intercept and all counts zero, the supremum is approached as the intercept tends to $-\infty$. If every observed count is positive, a full-rank design does give a finite maximum: each function $y_i\eta_i-e^{\eta_i}$ tends to $-\infty$ in either tail and is bounded above, and $\|X\beta\|\to\infty$ as $\|\beta\|\to\infty$, so the negative [log-likelihood](maximum-likelihood-estimation.md#log-likelihood) is coercive.

### Poisson slope information after eliminating an intercept

↑ **Parent:** [Poisson regression](#poisson-regression)

In [Poisson regression](#poisson-regression) with log means $a+\beta x_i$, the [Fisher information matrix](statistical-modelling.md#fisher-information-matrix) is $\begin{pmatrix}S_0&S_1\\S_1&S_2\end{pmatrix}$, where $S_j=\sum_i x_i^j\mu_i$. Inverting this matrix gives slope [variance](variance.md) $S_0/(S_0S_2-S_1^2)$. Writing $\bar x_\mu=S_1/S_0$ reduces it to the displayed reciprocal weighted sum of squares. Thus a common intercept consumes information about the overall rate, while slope information comes from the spread of the covariates under the mean-count weights. Constant covariates make the two parameters unidentifiable.

### Poisson regression margin-matching score equations

↑ **Parent:** [Poisson regression](#poisson-regression)

For [independent](random-variable.md#independent-random-variables) [Poisson distributions](discrete-probability-distribution.md#poisson-distribution) with log means $Z\beta+o$, where $o$ is a known [offset](#generalized-linear-model-offset), differentiation of the [log-likelihood](maximum-likelihood-estimation.md#log-likelihood) gives the [score function](statistical-modelling.md#informant-function) $Z^T(y-\mu)$. An interior [maximum-likelihood estimator](maximum-likelihood-estimation.md#maximum-likelihood-estimator) therefore satisfies the displayed equations. An intercept and categorical indicator columns make fitted count totals equal observed count totals in each represented factor level. These equations match counts, rather than unweighted averages of rates when exposures differ.

// Target: probability-and-statistics.bigb

### Two-group Poisson ratio conditional likelihood

↑ **Parent:** [Poisson regression](#poisson-regression)

For independent aggregate [Poisson distributions](discrete-probability-distribution.md#poisson-distribution) with means $n\lambda$ and $n\lambda e^\beta$, conditioning on the total eliminates $\lambda$. [Independent Poisson conditioning](statistical-modelling.md#independent-poisson-conditioning) gives the displayed [binomial distribution](discrete-probability-distribution.md#binomial-distribution). Its [conditional likelihood](maximum-likelihood-estimation.md#conditional-likelihood) is proportional to $e^{\beta Y_1}(1+e^\beta)^{-m}$, also the [profile likelihood](maximum-likelihood-estimation.md#profile-likelihood) after maximizing over the unrestricted positive baseline rate. Unequal exposures replace the binomial success probability by $n_1e^\beta/(n_0+n_1e^\beta)$.

#### Paired Poisson conditional likelihood

↑ **Parent:** [Two-group Poisson ratio conditional likelihood](#two-group-poisson-ratio-conditional-likelihood)

For conditionally independent paired counts with means $\lambda_i$ and $\lambda_i e^\beta$, condition on every pair total $N_i=Y_{i0}+Y_{i1}$. The joint [conditional likelihood](maximum-likelihood-estimation.md#conditional-likelihood) removes all pair-specific rates, leaving the displayed independent [binomial distributions](discrete-probability-distribution.md#binomial-distribution). A zero-total pair contributes no information. With unrestricted fixed baseline rates, this conditional likelihood has the same parameter-dependent part as the ordinary [profile likelihood](maximum-likelihood-estimation.md#profile-likelihood); a specified [Gamma–Poisson hierarchical model](bayesian-statistics.md#gamma-poisson-hierarchical-model) can retain additional information by imposing structure on those rates.

##### Conditional cure-weight equations for paired Poisson counts

↑ **Parent:** [Paired Poisson conditional likelihood](#paired-poisson-conditional-likelihood)

Consider an approximate [conditional likelihood](maximum-likelihood-estimation.md#conditional-likelihood) in which a paired total $t_i$ leads to a structural zero with probability $\theta$, and otherwise a [binomial distribution](discrete-probability-distribution.md#binomial-distribution) with success probability $p$. For an observed zero, the posterior cure weight is $q_i=\theta/[\theta+(1-\theta)(1-p)^{t_i}]$; for a positive count it is zero. Differentiating the [log-likelihood](maximum-likelihood-estimation.md#log-likelihood) gives the displayed equations at an interior [maximum-likelihood estimator](maximum-likelihood-estimation.md#maximum-likelihood-estimator), with the weights evaluated at that estimator. Recomputing the weights and then updating the parameters is an [expectation-maximization algorithm](latent-variable.md#expectation-maximization-algorithm). Boundary fits must also be considered. These equations describe a conditional mixture: if cure is instead specified before two [Poisson distributions](discrete-probability-distribution.md#poisson-distribution) are conditioned on their total, its conditional probability generally depends on the total and on the baseline nuisance rate. A zero observed in a short interval is not by itself proof of permanent biological cure.

### Common versus factor-specific slopes in Poisson regression

↑ **Parent:** [Poisson regression](#poisson-regression)

For a continuous predictor $x$ and a categorical [factor](statistical-modelling.md#regression-factor), an additive [Poisson regression](#poisson-regression) with [log link](#logarithmic-link-function) has $\log\mu_j(x)=a_j+b x$. The log-mean curves are parallel and $\mu_j(x)/\mu_k(x)=e^{a_j-a_k}$ is constant in $x$. Adding a predictor-by-factor [interaction](statistical-model.md#interaction-statistics) gives $\log\mu_j(x)=a_j+b_jx$, so this ratio becomes $e^{a_j-a_k+(b_j-b_k)x}$. With $J$ factor levels, the common-slope restriction has $J-1$ independent constraints. A [likelihood-ratio test](statistical-hypothesis-test.md#likelihood-ratio-test) compares the two [deviances](exponential-family.md#exponential-family-deviance) with an asymptotic [chi-squared distribution](probability-distribution.md#chi-squared-distribution) on $J-1$ [degrees of freedom](classical-mechanics.md#degree-of-freedom). Evidence against common slopes establishes varying effects on the log scale; it does not by itself determine their signs or the ordering of the mean curves.

### Poisson working models for averaged counts

↑ **Parent:** [Poisson regression](#poisson-regression)

If $C_i\sim\operatorname{Poisson}(T_i\lambda_i)$ counts events over $T_i$ days, then the daily average $C_i/T_i$ has mean $\lambda_i$ and variance $\lambda_i/T_i$. It is not itself a Poisson variable unless $T_i=1$. Known observation periods allow count modelling with a log-exposure [offset](#generalized-linear-model-offset); otherwise [Quasi-Poisson regression](#quasi-poisson-regression) may be used as a working mean-variance model, with uncertainty qualified by the missing exposure information.

### Poisson log-rate ratio

↑ **Parent:** [Poisson regression](#poisson-regression)

For independent samples of $n$ observations from [Poisson distributions](discrete-probability-distribution.md#poisson-distribution) with positive means $a$ and $b$, the [maximum-likelihood estimator](maximum-likelihood-estimation.md#maximum-likelihood-estimator) of $\nu=\log(b/a)$ is the displayed difference when both totals are positive. Its asymptotic variance is $(a^{-1}+b^{-1})/n$, obtained by the [delta method](statistical-inference.md#delta-method) or by inverting the two-parameter [Fisher information matrix](statistical-modelling.md#fisher-information-matrix). A zero group total makes its log-mean estimate a boundary value; finite normal intervals require nonzero totals.

### Poisson mean saturation at three distinct times

↑ **Parent:** [Poisson regression](#poisson-regression)

For three distinct times, the columns $1,t,t^2$ are linearly independent by the [Vandermonde determinant](galois-theory.md#vandermonde-determinant). Thus a quadratic [Poisson regression](#poisson-regression) for the log mean can reproduce any three positive time-group means. A grouped goodness-of-fit test of that mean form has zero residual degrees of freedom. Replicated observations still allow checks of the [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) and [overdispersion](exponential-family.md#overdispersion) within each time group; saturation of the mean does not establish the response distribution.

### Pooling selected slopes in a Poisson regression

↑ **Parent:** [Poisson regression](#poisson-regression)

A categorical covariate can be grouped in an interaction term while retaining its original main effect. This shares selected slopes but keeps separate intercepts. Nested [Poisson deviance](#poisson-deviance) differences test slope pooling and intercept pooling separately.

### Treatment interaction contrast in a Poisson regression

↑ **Parent:** [Poisson regression](#poisson-regression)

In a [Poisson regression](#poisson-regression) with $\log\mu=\beta_0+\beta_TT+\beta_Bb+\beta_{TB}Tb$, the treatment [logarithm](calculus.md#logarithm) of the mean ratio at baseline $b$ is $\beta_T+b\beta_{TB}$. The main treatment coefficient tests the contrast at $b=0$. An overall no-treatment test requires both $\beta_T=0$ and $\beta_{TB}=0$, with their joint [covariance matrix](variance.md#covariance-matrix) for a [Wald test](statistical-hypothesis-test.md#wald-test).

### Poisson deviance

↑ **Parent:** [Poisson regression](#poisson-regression)

For independent Poisson observations with fitted means $\widehat\mu_i$, the deviance from the saturated model is

$$
D=2\sum_i\left\{y_i\log\frac{y_i}{\widehat\mu_i}-(y_i-\widehat\mu_i)\right\},
$$

with $0\log0=0$.

#### Quadratic Pearson approximation to the Poisson deviance

↑ **Parent:** [Poisson deviance](#poisson-deviance)

Write $y_i=e_i+r_i$. For $|r_i|/e_i$ small, the cell contribution to the [Poisson deviance](#poisson-deviance) expands as

$$
2[(e_i+r_i)\log(1+r_i/e_i)-r_i]
=\frac{r_i^2}{e_i}-\frac{r_i^3}{3e_i^2}+O(r_i^4/e_i^3).
$$

Summing gives the [Pearson chi-squared statistic](#pearson-chi-squared-statistic) as the quadratic approximation. The approximation can be inaccurate for sparse expected counts or cells with relative residuals near minus one.

#### Poisson deviance simplifies when an intercept is fitted

↑ **Parent:** [Poisson deviance](#poisson-deviance)

The full [Poisson deviance](#poisson-deviance) is $2\sum_i[y_i\log(y_i/e_i)-y_i+e_i]$. An unpenalized log-mean intercept has [likelihood](maximum-likelihood-estimation.md#likelihood-function) score $\sum_i(y_i-e_i)$, which vanishes at an interior fit. The linear terms then cancel, giving the displayed expression. Without that intercept score equation, discarding the linear terms is not justified. Use the limiting convention $0\log(0/e_i)=0$.

## Gamma regression with logarithmic link

↑ **Parent:** [Generalized linear model](generalized-linear-model.md)

A Gamma regression with logarithmic link models a positive response with $\operatorname{Var}(Y_i\mid X_i)=\phi\mu_i^2$ and $\log\mu_i=x_i^T\beta$.

## Quasi-Poisson regression

↑ **Parent:** [Generalized linear model](generalized-linear-model.md)

Quasi-Poisson regression uses the mean model $\log\mu_i=x_i^T\beta$ and variance relation $\operatorname{Var}(Y_i)=\phi\mu_i$. It estimates $\beta$ through quasi-likelihood and scales its covariance by the estimated dispersion $\phi$.

### Poisson score linearization under proportional variance

↑ **Parent:** [Quasi-Poisson regression](#quasi-poisson-regression)

With $\mu_i=e^{\beta x_i}$, define $U=\sum_i x_i(Y_i-\mu_i)$ and $I=\sum_i x_i^2\mu_i$. The estimating equation and a [Taylor expansion](calculus.md#taylor-expansion) give $\widehat\beta-\beta_0\approx I(\beta_0)^{-1}U(\beta_0)$. If responses are independent with correct means and $\operatorname{Var}(Y_i)=\phi\mu_i$, then $EU=0$ and $\operatorname{Var}U=\phi I$. Consequently the first-order estimator [variance](variance.md) is $\phi/I$, even if the working [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) is wrong. Regular asymptotics require growing information and control of leverage and the Taylor remainder.

### Quasi-score equation

↑ **Parent:** [Quasi-Poisson regression](#quasi-poisson-regression)

For mean $\mu_i(\beta)$ and variance proportional to $V(\mu_i)$, the quasi-score is the sum of $(Y_i-\mu_i)V(\mu_i)^{-1}\partial\mu_i/\partial\beta$. Setting it to zero estimates $\beta$ without requiring a full response likelihood.

## Negative binomial regression

↑ **Parent:** [Generalized linear model](generalized-linear-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Negative_binomial_regression)

Negative binomial regression models overdispersed counts with a [negative binomial distribution](discrete-probability-distribution.md#negative-binomial-distribution), commonly using a logarithmic link for the mean.

### Fixed-size negative binomial generalized linear model

↑ **Parent:** [Negative binomial regression](#negative-binomial-regression)

For known size $\theta>0$, the [negative binomial distribution](discrete-probability-distribution.md#negative-binomial-distribution) is an [exponential family](exponential-family.md) with natural parameter $\eta=\log[\mu/(\theta+\mu)]<0$ and cumulant $b_\theta(\eta)=-\theta\log(1-e^\eta)$. A [generalized linear model](generalized-linear-model.md) can use a [logarithmic link function](#logarithmic-link-function) for its mean, even though that link is not canonical. Jointly estimating the size changes the family and [variance function](exponential-family.md#variance-function), requiring additional updates beyond a single fixed-family GLM fit; this is what `MASS::glm.nb` does.

#### Negative binomial deviance

↑ **Parent:** [Fixed-size negative binomial generalized linear model](#fixed-size-negative-binomial-generalized-linear-model)

With known size $\theta>0$, the mean-dependent log mass of a [negative binomial distribution](discrete-probability-distribution.md#negative-binomial-distribution) is $y\log\mu-(y+\theta)\log(\mu+\theta)$. Its derivative is $\theta(y-\mu)/[\mu(\mu+\theta)]$, so the saturated mean is $y$, including its boundary value zero. Subtracting the fitted log mass from that maximum gives the displayed [deviance](exponential-family.md#exponential-family-deviance). This formula needs no fitted-intercept cancellation. As $\theta\to\infty$, its second term tends to $-2(y_i-e_i)$ and it becomes the full [Poisson deviance](#poisson-deviance).

## Poisson exposure model

↑ **Parent:** [Generalized linear model](generalized-linear-model.md)

For fixed exposures $x_i\geq0$, a Poisson exposure model takes independent observations

$$
Y_i\sim\operatorname{Poisson}(\theta x_i).
$$

It has mean and variance $\theta x_i$ and is therefore heteroscedastic when the exposures differ.

### Exposure time for a Poisson rate at fixed fractional precision

↑ **Parent:** [Poisson exposure model](#poisson-exposure-model)

For an independent count with a [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) of mean $RT$, the rate estimator $N/T$ has [variance](variance.md) $R/T$. Its fractional [standard deviation](variance.md#standard-deviation) is $1/\sqrt{RT}$, so achieving target fractional precision $\epsilon$ requires expected count $RT=\epsilon^{-2}$ and exposure $T=1/(\epsilon^2R)$.

For independently acquired settings with rates $R_i$, the required total exposure is $\epsilon^{-2}\sum_iR_i^{-1}$. Rare settings dominate because they require the same expected count but collect it more slowly. Simultaneous acquisition is a different design, and backgrounds or correlated systematic errors require a different uncertainty calculation.

### Rate ratio

↑ **Parent:** [Poisson exposure model](#poisson-exposure-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rate_ratio)

A rate ratio compares event counts per unit exposure between two conditions. In a [Poisson regression](#poisson-regression) with a [log link](#logarithmic-link-function) and binary indicator coefficient $\beta$, it equals $e^\beta$. Exponentiating an approximate [Wald confidence interval](statistical-inference.md#wald-confidence-interval) for $\beta$ gives an interval for the rate ratio. A rate ratio is distinct from a [relative risk](statistical-modelling.md#risk-ratio) or an [odds ratio](statistical-modelling.md#odds-ratio).

### Finite-exposure Poisson inconsistency

↑ **Parent:** [Poisson exposure model](#poisson-exposure-model)

Let independent counts satisfy $Y_i\sim\operatorname{Poi}(\theta w_i)$, with positive known exposures $w_i$, $\theta>0$, and $a_n=\sum_{i=1}^nw_i\uparrow a_\infty<\infty$. Their [likelihood](maximum-likelihood-estimation.md#likelihood-function) is proportional to $\theta^{S_n}e^{-a_n\theta}$, where $S_n=\sum_{i=1}^nY_i$. If $S_n>0$, the positive [maximum-likelihood estimator](maximum-likelihood-estimation.md#maximum-likelihood-estimator) is $S_n/a_n$; when $S_n=0$, no maximum is attained on the open parameter space, while the closed-space maximizer is zero. This extended estimate converges almost surely to $S_\infty/a_\infty$, where $S_\infty\sim\operatorname{Poi}(\theta a_\infty)$. Finiteness follows from $\mathbb E S_\infty=\theta a_\infty$, and the limiting [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) follows from the finite-sum laws. In particular, the probability of a zero estimate tends to $e^{-\theta a_\infty}>0$, proving failure of [statistical consistency](statistical-inference.md#consistency-statistics). The total [Fisher information](statistical-modelling.md#fisher-information-matrix) tends to $a_\infty/\theta$: infinitely many observations need not provide infinite information.

### Estimators for a Poisson exposure model

↑ **Parent:** [Poisson exposure model](#poisson-exposure-model)

For $S_r=\sum_i x_i^r$, unweighted least squares through the origin and maximum likelihood give

$$
\widehat\theta_{LS}=\frac{\sum_i x_iY_i}{S_2},
\qquad
\widehat\theta_{MLE}=\frac{\sum_iY_i}{S_1}.
$$

Both estimators are unbiased.

#### Variance comparison for Poisson exposure estimators

↑ **Parent:** [Estimators for a Poisson exposure model](#estimators-for-a-poisson-exposure-model)

The two variances are

$$
\operatorname{var}(\widehat\theta_{LS})
=\frac{\theta S_3}{S_2^2},
\qquad
\operatorname{var}(\widehat\theta_{MLE})
=\frac\theta{S_1}.
$$

Since $S_2^2\leq S_1S_3$ by Cauchy-Schwarz, maximum likelihood has no larger variance, with equality when all positive exposures are equal.

### Normal-approximation tests for a Poisson exposure model

↑ **Parent:** [Poisson exposure model](#poisson-exposure-model)

For testing $H_0:\theta=1$ against a larger alternative, approximate size-$0.05$ upper-tail tests reject when

$$
\widehat\theta_{MLE}>1+\frac{1.645}{\sqrt{S_1}}
$$

or, respectively,

$$
\widehat\theta_{LS}>1+1.645\frac{\sqrt{S_3}}{S_2}.
$$

## Logistic regression

↑ **Parent:** [Generalized linear model](generalized-linear-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Logistic_regression)

Logistic regression models the conditional log odds as an affine function of predictors.

### Proportional-odds model

↑ **Parent:** [Logistic regression](#logistic-regression)

For ordered response categories, ordered thresholds $\theta_l$ and a common slope vector define this cumulative [logistic regression](#logistic-regression). Increasing $x^T\beta$ shifts probability toward higher categories. A covariate contrast multiplies all corresponding cumulative odds by the same factor. This model is not a canonical baseline-category [multinomial logistic regression](#multinomial-logistic-regression), so the latter's design-weighted count margins are not generally sufficient for it.

### Separation in logistic regression

↑ **Parent:** [Logistic regression](#logistic-regression)

Complete separation means that a predictor direction $v$ strictly separates the binary outcomes as displayed. In [logistic regression](#logistic-regression), replacing $\beta$ by $\beta+tv$ increases each observed-outcome [probability](probability-theory.md#probability) as $t$ increases, so the [log-likelihood](maximum-likelihood-estimation.md#log-likelihood) has no finite maximizer. Weak inequalities with some equalities can similarly produce quasi-complete separation. Finite coefficient estimates and ordinary information-matrix inference therefore require an existence check rather than relying only on the formal score equations.

### Finite maximum-likelihood estimate in a one-parameter logistic model

↑ **Parent:** [Logistic regression](#logistic-regression)

For nonzero design entries the [Bernoulli logistic-regression model](#bernoulli-logistic-regression-model) has strictly concave log likelihood, since $-\ell''=\sum_i x_i^2\mu_i(1-\mu_i)>0$. A unique finite estimate exists exactly when its score is positive at minus infinity and negative at plus infinity. Perfect agreement of binary outcomes with the signs of the design can instead give a supremum approached at an infinite coefficient. If every design entry is zero, the coefficient is unidentifiable. [Newton method](mathematical-optimization.md#newton-s-method-in-optimization) uses the score divided by this observed information, with damping when needed.

### Conditional logistic model for longitudinal binary data

↑ **Parent:** [Logistic regression](#logistic-regression)

A [logistic regression](#logistic-regression) can specify each binary response conditionally on recorded past outcomes and baseline [covariates](statistical-model.md#covariate). A [chain rule for probabilities](probability-theory.md#chain-rule-for-probabilities) gives the path [likelihood](maximum-likelihood-estimation.md#likelihood-function) as the product of the conditional [Bernoulli distribution](discrete-probability-distribution.md#bernoulli-distribution) masses. This permits dependence within a person's history without treating their outcomes as unconditionally independent. The model must specify the initial history and which past features enter its conditional mean.

#### Cumulative-response logistic model

↑ **Parent:** [Conditional logistic model for longitudinal binary data](#conditional-logistic-model-for-longitudinal-binary-data)

The accumulated number of previous successes may enter the conditional mean in a [history-dependent logistic regression](#conditional-logistic-model-for-longitudinal-binary-data). Its coefficient exponentiates to the conditional success [odds ratio](statistical-modelling.md#odds-ratio) per previous success. For a specified future path, update this cumulative predictor after each outcome before multiplying the conditional [probabilities](probability-theory.md#probability).

#### True state dependence

↑ **Parent:** [Conditional logistic model for longitudinal binary data](#conditional-logistic-model-for-longitudinal-binary-data)

A previous outcome may affect a subsequent outcome after controlling both measured [covariates](statistical-model.md#covariate) and persistent [unobserved heterogeneity](latent-variable.md#unobserved-heterogeneity). This is true state dependence. An observed lagged-outcome association alone does not establish it, because omitted individual propensities can create apparent persistence.

### Multinomial logistic regression

↑ **Parent:** [Logistic regression](#logistic-regression)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multinomial_logistic_regression)

A regression for a categorical response with more than two possible outcomes, parametrizing log probability ratios relative to a baseline category by linear predictors. It preserves categories that a binary [logistic regression](#logistic-regression) would merge.

#### Continuation-ratio logits

↑ **Parent:** [Multinomial logistic regression](#multinomial-logistic-regression)

For ordered response categories, model each displayed conditional probability by a [grouped-binomial logistic regression](#grouped-binomial-logistic-regression). The [multinomial likelihood](discrete-probability-distribution.md#multinomial-likelihood) factors exactly into successive conditional [binomial likelihoods](discrete-probability-distribution.md#binomial-likelihood), using the remaining category total as each stage's denominator. This is a different regression parameterization from baseline-category logits or cumulative odds. Separate cumulative binary indicators from the same person are dependent and cannot be treated as independent likelihood contributions.

#### Conditional multinomial sufficient statistics

↑ **Parent:** [Multinomial logistic regression](#multinomial-logistic-regression)

For independent [multinomial distributions](discrete-probability-distribution.md#multinomial-distribution) with fixed stratum totals $N_s$ and baseline logits $\log(p_{sl}/p_{sL})=x_s^T\beta_l$, the [sufficient statistics](probability-and-statistics.md#sufficient-statistic) are the displayed response-specific design-weighted counts, $l<L$. Expanding the [log-likelihood](maximum-likelihood-estimation.md#log-likelihood) gives $\sum_{l<L}\beta_l^TT_l-\sum_sN_s\log(1+\sum_{l<L}e^{x_s^T\beta_l})$, plus a data-only term. The [Fisher-Neyman factorization theorem](probability-and-statistics.md#fisher-neyman-factorization-theorem) therefore proves sufficiency; with an unrestricted identifiable canonical parameter, a likelihood-ratio argument proves minimal sufficiency. Factor indicators give the corresponding response/covariate margins.

### Logistic-normal regression with autoregressive random effects

↑ **Parent:** [Logistic regression](#logistic-regression)

A logistic-normal count model takes $Y_i\mid\theta_i\sim\operatorname{Bin}(n_i,\operatorname{logit}^{-1}\theta_i)$ and $\theta_i=x_i^T\beta+\lambda Z_i+\eta_i$, where $Z$ is a stationary unit-variance [autoregressive process of order one](time-series.md#autoregressive-process-of-order-one) with coefficient $a$ and the independent $\eta_i$ have [normal distribution](probability-distribution.md#normal-distribution) with variance $v$. The marginal latent variance is $\lambda^2+v$, and its off-diagonal [covariance](variance.md#covariance) is $\lambda^2 a^{|i-j|}$. Random success probabilities produce [overdispersion](exponential-family.md#overdispersion) relative to the [binomial distribution](discrete-probability-distribution.md#binomial-distribution).

### Logistic model

↑ **Parent:** [Logistic regression](#logistic-regression)

A logistic model maps a real-valued score $\eta$ to the probability $p=(1+e^{-\eta})^{-1}$, equivalently $\log(p/(1-p))=\eta$. [Logistic regression](#logistic-regression) takes $\eta$ to be an affine function of the predictors.

#### Log odds

↑ **Parent:** [Logistic model](#logistic-model)

For an event of probability $p$, the log odds are the [natural logarithm](calculus.md#natural-logarithm) of its [odds](probability-theory.md#odds):

$$
\operatorname{logit}(p)=\log\frac{p}{1-p}.
$$

### Separation (statistics)

↑ **Parent:** [Logistic regression](#logistic-regression)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Separation_(statistics))

Separation in a binary regression model occurs when an affine score assigns all observations from one class to one side of a threshold and all observations from the other class to the other side.

#### Quasi-complete separation

↑ **Parent:** [Separation (statistics)](#separation-statistics)

In a binary [logistic regression](#logistic-regression), write the signed directional margin of observation $i$ as $(2y_i-1)x_i^Td$. Quasi-complete separation occurs when a nonzero direction $d$ makes all these margins nonnegative, with some zero and some strictly positive. Along coefficients $\beta+td$, $t\to\infty$, each observation's [log-likelihood](maximum-likelihood-estimation.md#log-likelihood) contribution is nondecreasing, and those with positive margins strictly increase toward their limiting value. Hence the unpenalized fit cannot have a finite maximum in that direction. A group containing only outcome zeros is a simple example: sending its indicator coefficient to $-\infty$ improves that group's likelihood while leaving all other observations unchanged. Zero fitted risk is then a boundary limit, and ordinary finite-coefficient [Wald confidence intervals](statistical-inference.md#wald-confidence-interval) are unavailable.

#### Complete separation

↑ **Parent:** [Separation (statistics)](#separation-statistics)

Complete separation means that every signed training margin is strictly positive for some affine score. In unpenalized logistic regression it causes coefficient norms to diverge and prevents a finite maximum-likelihood estimate.

### Bernoulli logistic-regression model

↑ **Parent:** [Logistic regression](#logistic-regression)

For binary independent responses, logistic regression sets

$$
Y_i\sim\operatorname{Bernoulli}(p_i),
\qquad
\log\frac{p_i}{1-p_i}=\beta_0+x_i^T\beta.
$$

#### Fitted-mean balance for logistic regression with an intercept

↑ **Parent:** [Bernoulli logistic-regression model](#bernoulli-logistic-regression-model)

At an interior maximum-likelihood fit of a logistic-regression model containing an intercept, the intercept [score function](statistical-modelling.md#informant-function) is

$$
\frac{\partial\ell}{\partial\beta_0}=\sum_i(y_i-\widehat p_i)=0.
$$

Consequently the sum of the fitted probabilities equals the number of observed successes exactly.

### Logistic loss

↑ **Parent:** [Logistic regression](#logistic-regression)

For a signed margin $u=yh(x)$, the logistic loss is

$$
\phi(u)=\log(1+e^{-u}).
$$

It is convex and has derivative $\phi'(u)=-e^{-u}/(1+e^{-u})$.

#### Positive semidefinite quadratic-form classifier

↑ **Parent:** [Logistic loss](#logistic-loss)

For a positive semidefinite trace ball $\mathcal S_s$, the quadratic-form hypothesis class is

$$
\mathcal H_s=\{h_M:x\mapsto x^TMx,\ M\in\mathcal S_s\}.
$$

Its empirical logistic risk is convex as a function of $M$.

### L1-penalized logistic regression

↑ **Parent:** [Logistic regression](#logistic-regression)

L1-penalized logistic regression minimizes empirical [logistic loss](#logistic-loss) plus $\lambda\lVert\beta\rVert_1$. Its subgradient optimality conditions set each logistic score coordinate equal to $-\lambda z_j$, where $z_j=\operatorname{sgn}(\beta_j)$ off zero and $z_j\in[-1,1]$ at zero.

### Grouped-binomial logistic regression

↑ **Parent:** [Logistic regression](#logistic-regression)

For independent grouped counts $Y_i\sim\operatorname{Bin}(n_i,p_i)$, grouped-binomial logistic regression specifies

$$
\log\frac{p_i}{1-p_i}=x_i^T\beta.
$$

Fitting the proportions $Y_i/n_i$ with binomial weights $n_i$ gives the same likelihood.

#### Baseline logit estimator in a group-factor binomial model

↑ **Parent:** [Grouped-binomial logistic regression](#grouped-binomial-logistic-regression)

For independent $Y_{ij}\sim\operatorname{Bin}(m,p_i)$ with $k$ replicates per group and $\operatorname{logit}(p_i)=\mu+\alpha_i$, $\alpha_1=0$, let $S_i=\sum_jY_{ij}$ and $N=km$. The likelihood equations give $\widehat p_i=S_i/N$, $\widehat\mu=\log(S_1/(N-S_1))$, and $\widehat\alpha_i=\operatorname{logit}(\widehat p_i)-\widehat\mu$ when $0<S_i<N$. Boundary totals give infinite logits. With $0<p_1<1$ fixed and $N\to\infty$, the [central limit theorem](convergence-of-random-variables.md#central-limit-theorem) and [delta method](statistical-inference.md#delta-method) give

$$
\sqrt N(\widehat\mu-\mu)\ \xrightarrow{d}\ N\left(0,\frac1{p_1(1-p_1)}\right).
$$

The other groups do not increase information about the baseline logit when they have free offsets. For two groups, the information matrix for $(\mu,\alpha_2)$ is $\begin{pmatrix}w_1+w_2&w_2\\w_2&w_2\end{pmatrix}$ with $w_i=Np_i(1-p_i)$, whose inverse has first diagonal entry $1/w_1$.

#### Denominators in grouped birth-outcome models

↑ **Parent:** [Grouped-binomial logistic regression](#grouped-binomial-logistic-regression)

For each treatment year let $C$ be cycles, $S$ singleton deliveries, $T$ twin deliveries and $H$ deliveries of three or more babies. A singleton-per-cycle model uses $S\sim\operatorname{Bin}(C,p)$. A multiple-delivery model conditional on a live delivery instead uses $T+H\sim\operatorname{Bin}(S+T+H,q)$. The latter denominator counts deliveries, not babies, and it excludes failed cycles. Confusing these denominators changes the statistical question.

### Reference level in a regression factor

↑ **Parent:** [Logistic regression](#logistic-regression)

With treatment coding, the intercept describes the reference factor level and each displayed factor coefficient is a contrast against that level. Changing the reference level reparametrizes the same fitted model: fitted probabilities and likelihood do not change, but coefficients representing different pairwise contrasts can have different standard errors and p-values.

### Stochastic block model

↑ **Parent:** [Logistic regression](#logistic-regression)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stochastic_block_model)

A stochastic block model assigns each [vertex of a graph](graph.md#vertex-graph-theory) to a class and, conditional on those classes, makes distinct [edges](graph-theory.md#edge-of-a-graph) [independent random variables](random-variable.md#independent-random-variables) whose probabilities depend only on the classes of their endpoints.

#### Spectral norm bound for a centered Bernoulli adjacency matrix

↑ **Parent:** [Stochastic block model](#stochastic-block-model)

For independent [Bernoulli distribution](discrete-probability-distribution.md#bernoulli-distribution) upper-triangular entries of a symmetric zero-diagonal [adjacency matrix of a graph](graph-theory.md#adjacency-matrix), put $W=A-\mathbb EA$. For a unit vector $x$, $x^\top Wx=2\sum_{i<j}x_ix_jW_{ij}$ has sub-Gaussian variance proxy at most $\sum_{i<j}x_i^2x_j^2\leq1/2$, by the [Hoeffding lemma](probability-inequality.md#hoeffding-lemma). Hence $\mathbb P(|x^\top Wx|>u)\leq2e^{-u^2}$. The [volumetric bound for Euclidean metric nets](topological-analysis.md#volumetric-bound-for-euclidean-metric-nets) gives a $1/4$-[metric net](topological-analysis.md#metric-net) of the [unit sphere](topology.md#unit-sphere) with at most $9^n$ points. The [quadratic form net bound](topological-analysis.md#quadratic-form-net-bound) gives $\|W\|_{\mathrm{op}}\leq2\max_x|x^\top Wx|$ on that net. The [union bound](probability-inequality.md#boole-s-inequality) gives $\mathbb P(\|W\|_{\mathrm{op}}>2\sqrt{n\log9+\log2+s})\leq e^{-s}$; integrating this tail proves the displayed expectation bound.

#### Logistic stochastic block model

↑ **Parent:** [Stochastic block model](#stochastic-block-model)

A logistic stochastic block model parameterizes the edge probability between classes $k$ and $\ell$ as $\operatorname{logit}^{-1}(\beta_{k\ell})$.

##### Additive class-effect logistic network model

↑ **Parent:** [Logistic stochastic block model](#logistic-stochastic-block-model)

An additive class-effect logistic network model gives an edge joining classes $k$ and $\ell$ the log odds $\beta_k+\beta_\ell$. A further coefficient multiplying $\mathbf1_{\{k=\ell\}}$ represents a common within-class log-odds effect.

###### Degree-sum sufficient statistic for an additive logistic network model

↑ **Parent:** [Additive class-effect logistic network model](#additive-class-effect-logistic-network-model)

For independent binary edges with log odds $\beta_{z_i}+\beta_{z_j}+\beta_0\mathbf1_{\{z_i=z_j\}}$, the natural statistics are the sum of the [vertex degrees](graph-theory.md#degree-graph-theory) in each class and the total number of within-class edges. They form a [minimal sufficient statistic](probability-and-statistics.md#minimal-sufficient-statistic) whenever the natural parameter space contains an open subset of $\mathbb R^{C+1}$.

## Probit model

↑ **Parent:** [Generalized linear model](generalized-linear-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Probit_model)

Binary probit regression sets $p_i=\Phi(\beta_0+x_i^T\beta)$, where $\Phi$ is the [standard normal distribution](probability-distribution.md#standard-normal-distribution) function. Its intercept score is a weighted sum of residuals, so an intercept does not generally force $\sum_i\widehat p_i=\sum_i y_i$.

### Latent-normal Gibbs sampler for probit regression

↑ **Parent:** [Probit model](#probit-model)

For binary observations with success probability $\Phi(\beta x_i)$, introduce latent $Z_i\sim N(\beta x_i,1)$ and let the sign determine the observation. Given $\beta$ and the observed sign, each latent variable has a [truncated normal distribution](probability-distribution.md#truncated-normal-distribution). With a standard normal prior, the [full conditional distribution](probability-theory.md#full-conditional-distribution) of $\beta$ is normal with precision $1+\sum_i x_i^2$ and mean $\sum_i x_iZ_i/(1+\sum_i x_i^2)$. Alternating these blocks is [Gibbs sampling](bayesian-statistics.md#gibbs-sampler) with the required marginal posterior.

### Threshold observation of a lognormal regression

↑ **Parent:** [Probit model](#probit-model)

Observing only whether a lognormally modelled output exceeds a known threshold produces a probit link. The latent location and slope are recovered by multiplying the probit coefficients by the known Gaussian scale and adding the log threshold to the intercept.

### Probit posterior score

↑ **Parent:** [Probit model](#probit-model)

For [probit regression](#probit-model) with $s_i=2Y_i-1$ and prior $N(0,\sigma^2I)$, the [posterior score control variate](monte-carlo-method.md#posterior-score-control-variate) is

$$
g(\beta)=-\frac\beta{\sigma^2}+\sum_i s_ix_i\frac{\phi(s_ix_i^T\beta)}{\Phi(s_ix_i^T\beta)}.
$$

For $h(\beta)=\Phi(x_*^T\beta)$, its covariance with the score is $-x_*\mathbb E[\phi(x_*^T\beta)]$. It is nonzero whenever $x_*\ne0$, ensuring strict improvement by the optimal [control variate](monte-carlo-method.md#control-variates).

## Iteratively reweighted least squares

↑ **Parent:** [Generalized linear model](generalized-linear-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Iteratively_reweighted_least_squares)

IRLS fits a generalized linear model by repeatedly solving a weighted least-squares approximation to its score equations.

## Generalized linear mixed model

↑ **Parent:** [Generalized linear model](generalized-linear-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Generalized_linear_mixed_model)

A generalized linear mixed model adds latent random effects to the linear predictor of a [generalized linear model](generalized-linear-model.md).

### Logistic random-intercept model for repeated binary outcomes

↑ **Parent:** [Generalized linear mixed model](#generalized-linear-mixed-model)

A subject has a [random intercept](#random-intercept) $B_i\sim N(0,\tau^2)$, with responses conditionally independent given $B_i$ and their [covariates](statistical-model.md#covariate). Integrating the product of [Bernoulli](discrete-probability-distribution.md#bernoulli-distribution) [likelihoods](maximum-likelihood-estimation.md#likelihood-function) over $B_i$ defines the joint subject [likelihood](maximum-likelihood-estimation.md#likelihood-function) and induces within-subject dependence. Its coefficients describe conditional [odds ratios](statistical-modelling.md#odds-ratio) for a fixed latent subject effect. Under [missing at random](probability-and-statistics.md#missing-at-random) with [distinct parameters](probability-and-statistics.md#distinct-parameters), the observed-response likelihood integrates over the same random effect and sums out unobserved responses. Dependence of dropout on $B_i$ is not generally ignorable merely because conditional independence holds given $B_i$.

#### Random-intercept attenuation of marginal logistic slopes

↑ **Parent:** [Logistic random-intercept model for repeated binary outcomes](#logistic-random-intercept-model-for-repeated-binary-outcomes)

Put $p_B=\operatorname{logit}^{-1}(\eta+B)$ and $M(\eta)=\mathbb E(p_B)$. Differentiation gives $M'=\mathbb E[p_B(1-p_B)]=M(1-M)-\operatorname{Var}(p_B)$. Hence the displayed derivative lies between zero and one, strictly below one for a nondegenerate [random intercept](#random-intercept). A marginal [logit](#logit) is therefore generally nonlinear and its slope differs from the conditional slope even without [confounding](causal-inference.md#confounding). This is a precise instance of [noncollapsibility of the odds ratio](statistical-modelling.md#noncollapsibility-of-the-odds-ratio).

### Gaussian linear mixed model

↑ **Parent:** [Generalized linear mixed model](#generalized-linear-mixed-model)

A Gaussian linear mixed model combines [fixed effects](statistical-modelling.md#fixed-effect), [random effects](latent-variable.md#random-effect) with a [normal distribution](probability-distribution.md#normal-distribution), and independent [Gaussian noise](probability-distribution.md#gaussian-noise). For $b\sim N(0,D)$ and $\varepsilon\sim N(0,R)$ independently, its marginal distribution is $Y\sim N(X\beta,V)$ with $V=ZDZ^T+R$. The [random effects](latent-variable.md#random-effect) induce dependence among observations sharing their design columns. A [random-intercept linear mixed model](#random-intercept-linear-mixed-model) and a [random-slope linear mixed model](latent-variable.md#random-slope-linear-mixed-model) are special cases.

#### Correlated random-intercept and random-slope model

↑ **Parent:** [Gaussian linear mixed model](#gaussian-linear-mixed-model)

A subject-specific [random intercept](#random-intercept) and [random slope](latent-variable.md#random-slope) may have a joint [bivariate normal distribution](probability-and-statistics.md#bivariate-normal-distribution) with arbitrary positive-definite [covariance matrix](variance.md#covariance-matrix) $D$. With independent [normal](probability-distribution.md#normal-distribution) measurement errors of [variance](variance.md) $\sigma^2$, the marginal [covariance](variance.md#covariance) between a person's readings at $s,t$ is $D_{00}+(s+t)D_{01}+stD_{11}$, plus $\sigma^2$ on the diagonal. Different subjects remain independent. Allowing $D_{01}$ distinguishes this model from an [independent random-intercept and random-slope model](#independent-random-intercept-and-random-slope-model).

#### Variance component

↑ **Parent:** [Gaussian linear mixed model](#gaussian-linear-mixed-model)

A variance component is a nonnegative parameter multiplying a specified covariance contribution. In a [Gaussian linear mixed model](#gaussian-linear-mixed-model) with independent standardized group effects, $\tau_k^2Z_kZ_k^T$ describes the covariance induced by one set of [random effects](latent-variable.md#random-effect). Testing whether a component is zero is a [variance-component likelihood-ratio test at a boundary](statistical-hypothesis-test.md#variance-component-likelihood-ratio-test-at-a-boundary); ordinary regular chi-squared likelihood-ratio calibration need not apply.

##### Method-of-moments variance component estimate

↑ **Parent:** [Variance component](#variance-component)

A [method-of-moments variance component estimate](#method-of-moments-variance-component-estimate) equates residual [mean squares in ANOVA](linear-regression.md#mean-square-in-anova) to their model [expectations](expected-value.md) and solves for the [variance components](#variance-component). An unconstrained estimate can be negative even when the model component must be nonnegative; boundary treatment then requires a stated estimation convention. The method gives point estimates, not certainty about future experiments.

#### Best linear unbiased prediction

↑ **Parent:** [Gaussian linear mixed model](#gaussian-linear-mixed-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Best_linear_unbiased_prediction)

With known covariance parameters, best linear unbiased prediction minimizes prediction-error [variance](variance.md) over linear predictors that are unbiased over both observation errors and [random effects](latent-variable.md#random-effect), for every fixed-effect value. In a [Gaussian linear mixed model](#gaussian-linear-mixed-model), the random-effect predictor is $DZ^TV^{-1}(Y-X\widehat\beta_{\mathrm{GLS}})$, where [generalized least squares](normal-linear-model.md#generalized-least-squares) estimates the fixed effects. Plugging in covariance estimates gives an empirical predictor; its uncertainty must also account for estimating those covariance parameters. It differs from a [best linear unbiased estimator](statistical-modelling.md#best-linear-unbiased-estimator) of an unknown fixed coefficient.

#### Conditional mode of Gaussian random effects

↑ **Parent:** [Gaussian linear mixed model](#gaussian-linear-mixed-model)

In a [Gaussian linear mixed model](#gaussian-linear-mixed-model) with $V=ZDZ^T+R$, the [conditional multivariate normal distribution](probability-and-statistics.md#conditional-multivariate-normal-distribution) of $b$ given $Y$ has mean $DZ^TV^{-1}(Y-X\beta)$ and [covariance matrix](variance.md#covariance-matrix) $D-DZ^TV^{-1}ZD$. When nonsingular, its mean is also its mode. Estimated parameters yield empirical conditional modes and shrink group deviations toward zero. At a zero variance component the associated effect is degenerate at zero; the covariance formula still applies, whereas formulas involving $D^{-1}$ require limits.

#### Continuous-time autoregressive residual correlation

↑ **Parent:** [Gaussian linear mixed model](#gaussian-linear-mixed-model)

For $\kappa>0$, this error correlation decreases exponentially with elapsed time and permits irregular observation times. It is the stationary correlation of an [Ornstein-Uhlenbeck process](gaussian-process.md#ornstein-uhlenbeck-process). Within a [Gaussian linear mixed model](#gaussian-linear-mixed-model), apply it to the errors conditional on [random effects](latent-variable.md#random-effect); the marginal correlation also includes those effects. `nlme::corCAR1` parametrizes the same correlation by $\rho=e^{-\kappa}\in(0,1)$ and permits separate grouped time series.

#### Independent random-intercept and random-slope model

↑ **Parent:** [Gaussian linear mixed model](#gaussian-linear-mixed-model)

Independent Gaussian [random intercepts](#random-intercept) $u_j$ and [random slopes](latent-variable.md#random-slope) $v_j$ give marginal within-group [covariance](variance.md#covariance) $\tau_0^2+\tau_1^2t_{ij}t_{kj}+\sigma^2\mathbf1_{\{i=k\}}$. In `lme4`, separate terms `(1 | group)` and `(0 + x | group)` impose zero intercept-slope covariance; `(1 + x | group)` estimates it. This independence restriction depends on the predictor origin: replacing $t$ by $t-c$ transforms the intercept effect to $u_j+cv_j$, generally correlated with $v_j$.

### Poisson generalized linear mixed model

↑ **Parent:** [Generalized linear mixed model](#generalized-linear-mixed-model)

A Poisson generalized linear mixed model gives a count response a conditional [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) whose logarithmic mean contains both fixed effects and latent random effects.

#### Gamma random-intercept Poisson model

↑ **Parent:** [Poisson generalized linear mixed model](#poisson-generalized-linear-mixed-model)

Let the positive multiplier $U_i$ have a [gamma distribution](continuous-probability-distribution.md#gamma-distribution) with mean $\tau$ and [variance](variance.md) $\theta$, and conditionally let the repeated counts be [independent](random-variable.md#independent-random-variables) with means $U_i a_{ij}$. Total [expectation](expected-value.md) and [variance](variance.md) give

$$
\mathbb EY_{ij}=\tau a_{ij},\qquad
\operatorname{Var}(Y_{ij})=\tau a_{ij}+\theta a_{ij}^2,\qquad
\operatorname{Cov}(Y_{ij},Y_{ik})=\theta a_{ij}a_{ik}\quad(j\ne k).
$$

The [Poisson-gamma mixture](discrete-probability-distribution.md#poisson-gamma-mixture) gives negative-binomial marginal counts of size $\tau^2/\theta$. Despite the shared multiplier, the marginal correlations generally depend on both marginal means and need not be exchangeable.

##### Scale identifiability in a gamma random-intercept Poisson model

↑ **Parent:** [Gamma random-intercept Poisson model](#gamma-random-intercept-poisson-model)

When $a_{ij}=\exp(\beta_0+\beta^{\mathsf T}x_{ij})$, replacing $U_i$ by $cU_i$ and the fixed intercept by $\beta_0-\log c$ leaves every conditional count mean and the integrated data law unchanged. Thus without fixing the random multiplier's mean, the [gamma random-intercept Poisson model](#gamma-random-intercept-poisson-model) identifies the marginal intercept $\beta_0+\log\tau$ and relative heterogeneity $\theta/\tau^2$, rather than these three parameters separately. Normalizing $\tau=1$ removes this scale ambiguity.

#### Marginal mean of a Poisson random-slope model

↑ **Parent:** [Poisson generalized linear mixed model](#poisson-generalized-linear-mixed-model)

Given Gaussian [random intercept](#random-intercept) $b_0$ and [random slope](latent-variable.md#random-slope) $b_1$, let the conditional incidence rate be $e^{\beta_0+\beta_1s+b_0+b_1s}$. The normal moment-generating function gives the displayed marginal rate, with $\operatorname{Var}(b_0+b_1s)=\tau_0^2+2s\tau_{01}+s^2\tau_1^2$. Thus the conditional annual [rate ratio](#rate-ratio) for a cluster is $e^{\beta_1+b_1}$, whereas the marginal rate ratio also contains covariance and variance terms. Centering $s$ at a chosen year makes intercept heterogeneity refer directly to that year.

### Random intercept

↑ **Parent:** [Generalized linear mixed model](#generalized-linear-mixed-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Random_intercept)

A random intercept gives every group a latent additive shift, inducing dependence among observations from the same group.

#### Marginal and conditional slopes agree for an independent log-link random intercept

↑ **Parent:** [Random intercept](#random-intercept)

For a conditional count mean $\mathbb E(Y\mid x,b)=\exp(b+\beta_0+\beta^{\mathsf T}x)$, suppose the distribution of $b$ is [independent](random-variable.md#independent-random-variables) of the covariates and has finite $\mathbb E e^b$. Integrating over $b$ gives the displayed [logarithmic link function](#logarithmic-link-function) mean: every slope stays unchanged, and only the intercept shifts. This is an exact property of the log link; it does not hold in this form for the [logit](#logit).

#### Random-intercept linear mixed model

↑ **Parent:** [Random intercept](#random-intercept)

A random-intercept linear mixed model has the form

$$
Y_{ij}=x_{ij}^T\beta+b_i+\varepsilon_{ij},
$$

where independent group effects $b_i$ induce positive covariance among observations from the same group.

## ↑ Ancestors (6)

1. [Statistical modelling](statistical-modelling.md)
2. [Statistical model](statistical-model.md)
3. [Probability and statistics](probability-and-statistics.md)
4. [Area of mathematics](mathematics.md#area-of-mathematics)
5. [Mathematics](mathematics.md)
6. [Codex Wiki](README.md)

## ← Incoming links (34)

- [Deviance goodness-of-fit test](#deviance-goodness-of-fit-test)
- [Fixed-size negative binomial generalized linear model](#fixed-size-negative-binomial-generalized-linear-model)
- [Generalized linear mixed model](#generalized-linear-mixed-model)
- [Generalized linear model offset](#generalized-linear-model-offset)
- [Identity link](#identity-link)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-38.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-1.md#5i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2.md#5i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-1.md#13i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-3.md#5i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-41.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-3.md#5i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-73.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-41.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-42.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-3.md#5j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-37.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-37.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-37.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-33.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-1.md#10j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4.md#4j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4.md#5j/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4.md#5j/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-1.md#13j/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3.md#5j/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1.md#13j/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1.md#5j/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4.md#13j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-2.md#5j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-218.md#3/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-1.md#5l/a/solution)
- [Poisson surrogate for an uncensored proportional-hazards likelihood](survival-analysis.md#poisson-surrogate-for-an-uncensored-proportional-hazards-likelihood)
