# Normal linear model

↑ **Parent:** [Statistical modelling](statistical-modelling.md)

$Y=X\beta+\varepsilon$, $\varepsilon\sim N(0,\sigma^2I)$, and full-rank $X$ gives $\widehat\beta=(X^TX)^{-1}X^TY$.

**Table of contents**

- [Variance of a fitted regression mean](#variance-of-a-fitted-regression-mean)
- [Analysis of covariance](#analysis-of-covariance)
- [Normal linear model maximum-likelihood sampling distributions](#normal-linear-model-maximum-likelihood-sampling-distributions)
- [Lack of fit](#lack-of-fit)
  - [Lack-of-fit F-test](#lack-of-fit-f-test)
- [Pure error](#pure-error)
- [Two-factor normal linear model](#two-factor-normal-linear-model)
  - [Factor-level pooling test](#factor-level-pooling-test)
- [Joint distribution of least-squares and variance estimators](#joint-distribution-of-least-squares-and-variance-estimators)
- [Restricted maximum likelihood](#restricted-maximum-likelihood)
  - [Restricted likelihood from orthogonal error contrasts](#restricted-likelihood-from-orthogonal-error-contrasts)
- [Gaussian conjugacy for a normal linear model](#gaussian-conjugacy-for-a-normal-linear-model)
  - [Gaussian conjugacy for an initialized AR(2) regression](#gaussian-conjugacy-for-an-initialized-ar-2-regression)
  - [Normal-gamma posterior with a flat prior](#normal-gamma-posterior-with-a-flat-prior)
  - [Gaussian posterior in the zero-noise limit](#gaussian-posterior-in-the-zero-noise-limit)
  - [Gaussian likelihood](#gaussian-likelihood)
- [Cochran's theorem](#cochran-s-theorem)
  - [Rank-sum form of Cochran's theorem](#rank-sum-form-of-cochran-s-theorem)
- [Linear regression](linear-regression.md)
  - [Log-linear exponential-decay fit](linear-regression.md#log-linear-exponential-decay-fit)
  - [Multiple linear regression](linear-regression.md#multiple-linear-regression)
  - [Normal equations for linear least squares](linear-regression.md#normal-equations-for-linear-least-squares)
  - [Omitted-variable bias](linear-regression.md#omitted-variable-bias)
  - [Predictor centering](linear-regression.md#predictor-centering)
  - [Regression diagnostics](linear-regression.md#regression-diagnostics)
    - [Influential observation](linear-regression.md#influential-observation)
    - [Regression outlier](linear-regression.md#regression-outlier)
  - [Least angle regression](linear-regression.md#least-angle-regression)
    - [Equiangular direction in least angle regression](linear-regression.md#equiangular-direction-in-least-angle-regression)
    - [Sign compatibility of LAR and Lasso](linear-regression.md#sign-compatibility-of-lar-and-lasso)
    - [LAR active correlation invariant](linear-regression.md#lar-active-correlation-invariant)
    - [Entry knot in least angle regression](linear-regression.md#entry-knot-in-least-angle-regression)
  - [Reciprocal-predictor regression](linear-regression.md#reciprocal-predictor-regression)
  - [Regression intercept](linear-regression.md#regression-intercept)
    - [Student t test for a simple-regression intercept](linear-regression.md#student-t-test-for-a-simple-regression-intercept)
  - [Polynomial regression](linear-regression.md#polynomial-regression)
    - [Independent normal and inverse-gamma regression priors](linear-regression.md#independent-normal-and-inverse-gamma-regression-priors)
    - [Quadratic regression](linear-regression.md#quadratic-regression)
  - [Coefficient of determination](linear-regression.md#coefficient-of-determination)
    - [Adjusted coefficient of determination](linear-regression.md#adjusted-coefficient-of-determination)
  - [Residual-versus-fitted plot](linear-regression.md#residual-versus-fitted-plot)
    - [Scale-location plot](linear-regression.md#scale-location-plot)
  - [Analysis of variance](linear-regression.md#analysis-of-variance)
    - [Multivariate analysis of variance](linear-regression.md#multivariate-analysis-of-variance)
      - [Within-group and between-group scatter decomposition](linear-regression.md#within-group-and-between-group-scatter-decomposition)
      - [Wilks lambda statistic](linear-regression.md#wilks-lambda-statistic)
    - [Two-way analysis of variance](linear-regression.md#two-way-analysis-of-variance)
      - [Missing cells can destroy factor orthogonality in two-way ANOVA](linear-regression.md#missing-cells-can-destroy-factor-orthogonality-in-two-way-anova)
      - [Identifiability of an incomplete two-factor additive design](linear-regression.md#identifiability-of-an-incomplete-two-factor-additive-design)
      - [Saturation of an unreplicated two-factor regression](linear-regression.md#saturation-of-an-unreplicated-two-factor-regression)
    - [Sequential sum of squares](linear-regression.md#sequential-sum-of-squares)
    - [Sum of squares in ANOVA](linear-regression.md#sum-of-squares-in-anova)
      - [Mean square in ANOVA](linear-regression.md#mean-square-in-anova)
    - [ANOVA stratum](linear-regression.md#anova-stratum)
      - [Within-block ANOVA stratum](linear-regression.md#within-block-anova-stratum)
    - [Balanced factorial orthogonality](linear-regression.md#balanced-factorial-orthogonality)
  - [Frisch–Waugh–Lovell theorem](linear-regression.md#frisch-waugh-lovell-theorem)
  - [Simple linear regression](linear-regression.md#simple-linear-regression)
    - [Centred simple linear regression](linear-regression.md#centred-simple-linear-regression)
  - [Residual sum of squares](linear-regression.md#residual-sum-of-squares)
  - [Ridge regression](linear-regression.md#ridge-regression)
    - [Gaussian posterior representation of ridge regression](linear-regression.md#gaussian-posterior-representation-of-ridge-regression)
    - [Unbounded directional risk of fixed ridge shrinkage](linear-regression.md#unbounded-directional-risk-of-fixed-ridge-shrinkage)
    - [Uniform directional risk improvement by ridge regression](linear-regression.md#uniform-directional-risk-improvement-by-ridge-regression)
    - [Unpenalized intercept in ridge regression](linear-regression.md#unpenalized-intercept-in-ridge-regression)
    - [Covariance and bias of a ridge regression estimator](linear-regression.md#covariance-and-bias-of-a-ridge-regression-estimator)
    - [Closed-form ridge regression estimator](linear-regression.md#closed-form-ridge-regression-estimator)
      - [Vanishing-penalty ridge limit](linear-regression.md#vanishing-penalty-ridge-limit)
      - [Primal-dual identity for ridge regression](linear-regression.md#primal-dual-identity-for-ridge-regression)
      - [Principal-component shrinkage by ridge regression](linear-regression.md#principal-component-shrinkage-by-ridge-regression)
  - [Fitted values](linear-regression.md#fitted-values)
    - [Linear smoother](linear-regression.md#linear-smoother)
      - [Effective degrees of freedom](linear-regression.md#effective-degrees-of-freedom)
  - [Design matrix](linear-regression.md#design-matrix)
    - [Confounding of nested fixed factors](linear-regression.md#confounding-of-nested-fixed-factors)
  - [Regression coefficient](linear-regression.md#regression-coefficient)
  - [Attenuation bias from classical measurement error](linear-regression.md#attenuation-bias-from-classical-measurement-error)
- [R linear-model formula](#r-linear-model-formula)
  - [Treatment coding](#treatment-coding)
  - [Degrees of freedom of a factor predictor](#degrees-of-freedom-of-a-factor-predictor)
- [Hat matrix](#hat-matrix)
  - [Fitted-residual orthogonality](#fitted-residual-orthogonality)
- [Normal linear-model confidence ellipsoid](#normal-linear-model-confidence-ellipsoid)
  - [Cook's distance](#cook-s-distance)
- [Multicollinearity](#multicollinearity)
  - [Variance inflation factor](#variance-inflation-factor)
  - [Two-predictor variance inflation](#two-predictor-variance-inflation)
- [Ordinary least squares](#ordinary-least-squares)
  - [Residual estimate of Gaussian noise variance](#residual-estimate-of-gaussian-noise-variance)
    - [Residual standard error](#residual-standard-error)
  - [Partial regression](#partial-regression)
  - [Rank-deficient ordinary least squares](#rank-deficient-ordinary-least-squares)
    - [Nonidentifiability prevents unbiased coefficient estimation](#nonidentifiability-prevents-unbiased-coefficient-estimation)
  - [Linear regression through the origin](#linear-regression-through-the-origin)
    - [Residual estimate of slope uncertainty through the origin](#residual-estimate-of-slope-uncertainty-through-the-origin)
    - [Student t test for regression through the origin](#student-t-test-for-regression-through-the-origin)
  - [Ordinary least squares estimators](#ordinary-least-squares-estimators)
    - [Residual sum of squares in simple linear regression](#residual-sum-of-squares-in-simple-linear-regression)
- [Gauss-Markov theorem](#gauss-markov-theorem)
- [Weighted least squares](#weighted-least-squares)
  - [Gamma-ray energy-network fit](#gamma-ray-energy-network-fit)
  - [Additional measurements decrease known-error covariance](#additional-measurements-decrease-known-error-covariance)
  - [Fixed-phase sinusoidal least squares](#fixed-phase-sinusoidal-least-squares)
  - [Variable projection](#variable-projection)
  - [Generalized least squares](#generalized-least-squares)
    - [Whitening transformation](#whitening-transformation)
- [Normal equation](#normal-equation)
- [Consistency of least squares](#consistency-of-least-squares)
- [One-way normal linear model](#one-way-normal-linear-model)
  - [Cell-means parametrization](#cell-means-parametrization)
    - [Equal-cell replication variance formula](#equal-cell-replication-variance-formula)
    - [Linear contrast of cell means](#linear-contrast-of-cell-means)
      - [Treatment contrast](#treatment-contrast)
        - [Orthogonal polynomial contrast](#orthogonal-polynomial-contrast)
        - [Variance of a treatment contrast](#variance-of-a-treatment-contrast)
        - [Interaction contrast](#interaction-contrast)
          - [Logistic interaction as a ratio of odds ratios](#logistic-interaction-as-a-ratio-of-odds-ratios)
  - [Full-dominance mean constraint](#full-dominance-mean-constraint)
  - [Additive allele-count model](#additive-allele-count-model)

## Variance of a fitted regression mean

↑ **Parent:** [Normal linear model](normal-linear-model.md)

For a full-column-rank [design matrix](linear-regression.md#design-matrix) in a [normal linear model](normal-linear-model.md), a fitted mean at covariate vector $v$ is $v^T\widehat\beta$. The [covariance matrix](variance.md#covariance-matrix) of the [least-squares estimator](#ordinary-least-squares-estimators) immediately gives the displayed [variance](variance.md). Replacing $\sigma^2$ by the independent unbiased residual [variance](variance.md) gives its squared [standard error](statistical-inference.md#standard-error) and a [Student t confidence interval](statistical-inference.md#student-t-confidence-interval) on $n-p$ [statistical degrees of freedom](statistical-inference.md#statistical-degrees-of-freedom). A future response instead contributes an additional error [variance](variance.md) $\sigma^2$ when its error is independent of the fitted data.

// Target: probability-and-statistics.bigb

## Analysis of covariance

↑ **Parent:** [Normal linear model](normal-linear-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Analysis_of_covariance)

Analysis of covariance combines a categorical treatment and a quantitative covariate in a [normal linear model](normal-linear-model.md). A common-slope model is $Y_i=\alpha+\beta x_i+\sum_{g=2}^G\tau_g\mathbf1_{\{G_i=g\}}+\varepsilon_i$, with independent $N(0,\sigma^2)$ errors. Treatment differences compare fitted means at the same covariate value. Adding treatment-by-covariate interactions permits separate slopes, and a [partial F-test](probability-and-statistics.md#partial-f-test-for-nested-linear-models) compares this extension with the parallel-lines model. The treatment test after adding the covariate differs from an unadjusted comparison, because treatment groups can have different covariate distributions.

## Normal linear model maximum-likelihood sampling distributions

↑ **Parent:** [Normal linear model](normal-linear-model.md)

For a full-column-rank design $X$ and $Y=X\beta+\varepsilon$ with $\varepsilon\sim N_n(0,\sigma^2I)$, the maximum-likelihood estimators are $\widehat\beta=(X^TX)^{-1}X^TY$ and $\widehat\sigma^2=\|Y-X\widehat\beta\|^2/n$. Orthogonal Gaussian projections give their displayed distributions and independence. The [variance](variance.md) maximum-likelihood estimator has expectation $(n-p)\sigma^2/n$; the unbiased residual [variance](variance.md) divides by $n-p$ instead.

## Lack of fit

↑ **Parent:** [Normal linear model](normal-linear-model.md)

Lack of fit is a mismatch between a regression model's mean function and the true mean relationship. Replicated predictor configurations can separate its sum of squares from [pure error](#pure-error). A [residual-versus-fitted plot](linear-regression.md#residual-versus-fitted-plot) can suggest curvature or changing variance even without a formal replication-based test.

### Lack-of-fit F-test

↑ **Parent:** [Lack of fit](#lack-of-fit)

For $n$ independent normal responses of common [variance](variance.md) at $g$ distinct predictor settings, a rank-$p$ [normal linear model](normal-linear-model.md) has residual degrees $n-p$. The saturated setting-mean model has $g$ parameters and [pure error](#pure-error) degrees $n-g$. Splitting orthogonal residual spaces gives [lack of fit](#lack-of-fit) degrees $g-p$. Under the fitted mean model, the two squared lengths divided by the common variance are independent [chi-squared](probability-distribution.md#chi-squared-distribution) variables; their ratio of mean squares has the [F-distribution](continuous-probability-distribution.md#f-distribution) shown. This test is unavailable without repeated settings or positive lack-of-fit degrees.

## Pure error

↑ **Parent:** [Normal linear model](normal-linear-model.md)

With repeated responses at an identical predictor configuration, pure error is their within-configuration variability. Its [residual sum of squares](linear-regression.md#residual-sum-of-squares) can estimate measurement variance independently of a candidate regression mean function. Without replication, a fitted residual can combine pure error and [lack of fit](#lack-of-fit).

## Two-factor normal linear model

↑ **Parent:** [Normal linear model](normal-linear-model.md)

A two-factor [normal linear model](normal-linear-model.md) describes independent responses with factor-specific means and common normal error variance. The additive mean $\mu+\alpha_a+\gamma_j$ assumes no [interaction term](statistical-model.md#interaction-term); the full mean $\mu+\alpha_a+\gamma_j+\delta_{aj}$ permits the first factor effect to vary with the second. Constraints or [treatment coding](#treatment-coding) identify the parameters. In a balanced two-by-five design the full model has ten free cell means.

### Factor-level pooling test

↑ **Parent:** [Two-factor normal linear model](#two-factor-normal-linear-model)

To pool factor levels in a [normal linear model](normal-linear-model.md), impose equality of their fitted means while retaining any needed [interaction terms](statistical-model.md#interaction-term). Compare the resulting nested model with the full model using a [nested-model F-test](probability-and-statistics.md#nested-model-f-test). For two cells each of size $m$, pooling their fitted means adds $(m/2)(\overline Y_1-\overline Y_2)^2$ to the [residual sum of squares](linear-regression.md#residual-sum-of-squares). If pooling two pairs separately within two other-factor levels, there are four restrictions.

## Joint distribution of least-squares and variance estimators

↑ **Parent:** [Normal linear model](normal-linear-model.md)

With a full-column-rank $n\times p$ design and isotropic normal errors, [ordinary least squares](#ordinary-least-squares) gives $\widehat\beta\sim N_p(\beta,\sigma^2(X^TX)^{-1})$, independent of the residual squared length. Orthogonal design and residual projections of the [multivariate normal distribution](probability-and-statistics.md#multivariate-normal-distribution) are independent, and $\operatorname{RSS}/\sigma^2\sim\chi^2_{n-p}$. The maximum likelihood variance estimate is $\operatorname{RSS}/n$, not the unbiased estimate $\operatorname{RSS}/(n-p)$.

## Restricted maximum likelihood

↑ **Parent:** [Normal linear model](normal-linear-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Restricted_maximum_likelihood)

Restricted maximum likelihood estimates [covariance matrix](variance.md#covariance-matrix) parameters from linear combinations of the data whose distribution does not involve the fixed mean coefficients. It differs from a [restricted maximum-likelihood estimator](statistical-hypothesis-test.md#restricted-maximum-likelihood-estimator) obtained by maximizing an ordinary [likelihood function](maximum-likelihood-estimation.md#likelihood-function) under a null hypothesis.

### Restricted likelihood from orthogonal error contrasts

↑ **Parent:** [Restricted maximum likelihood](#restricted-maximum-likelihood)

For $Y\sim N(X\beta,V_\theta)$ and a full-column-rank [design matrix](linear-regression.md#design-matrix) $X\in\mathbb R^{n\times p}$, take $A\in\mathbb R^{n\times(n-p)}$ with $A^TA=I$ and $A^TX=0$. Then $A^TY\sim N(0,A^TV_\theta A)$, so [restricted maximum likelihood](#restricted-maximum-likelihood) maximizes

$$
\ell_R(\theta)=-\frac{n-p}{2}\log(2\pi)-\frac12\log\det(A^TV_\theta A)-\frac12Y^TA(A^TV_\theta A)^{-1}A^TY.
$$

Changing the [orthonormal basis](inner-product.md#orthonormal-basis) by an orthogonal matrix leaves this expression unchanged.

## Gaussian conjugacy for a normal linear model

↑ **Parent:** [Normal linear model](normal-linear-model.md)

If $Y\mid\beta\sim N(X\beta,\Sigma_e)$ and $\beta\sim N(m_0,\Sigma_0)$, then the posterior is normal with [precision matrix](variance.md#precision-matrix) $X^T\Sigma_e^{-1}X+\Sigma_0^{-1}$ and mean equal to the inverse precision times $X^T\Sigma_e^{-1}Y+\Sigma_0^{-1}m_0$.

<h3 id="gaussian-conjugacy-for-an-initialized-ar-2-regression">Gaussian conjugacy for an initialized AR(2) regression</h3>

↑ **Parent:** [Gaussian conjugacy for a normal linear model](#gaussian-conjugacy-for-a-normal-linear-model)

With independent standard-normal priors on the two coefficients, the conditional AR(2) likelihood gives precision $\Lambda=I+\sum_tv_tv_t^T$, where $v_t=(x_{t+1},x_t)^T$, and mean $\Lambda^{-1}\sum_tv_tx_{t+2}$. Positive definiteness holds even for a deficient design. If $\Lambda=\left(\begin{smallmatrix}A&C\\C&D\end{smallmatrix}\right)$ and the linear term is $(r,s)$, the conditional means are $(r-Cb)/A$ and $(s-Ca)/D$, with variances $1/A$ and $1/D$.

### Normal-gamma posterior with a flat prior

↑ **Parent:** [Gaussian conjugacy for a normal linear model](#gaussian-conjugacy-for-a-normal-linear-model)

Let $m\mid u,\gamma\sim\mathcal N(Au,\gamma^{-1}I_k)$, let the [prior distribution](bayesian-statistics.md#prior-probability) of the precision be the shape-rate [Gamma distribution](continuous-probability-distribution.md#gamma-distribution) $\operatorname{Gamma}(\alpha,\beta)$, and use a constant [improper prior](bayesian-statistics.md#improper-prior) for $u\in\mathbb R^d$. Assume $A$ has zero [null space](kernel-of-a-linear-map.md). Write $B=A^TA$, $u_*=B^{-1}A^Tm$, $a=\alpha+k/2$, $b_0=\beta+\|m-Au_*\|^2/2$, and $s=\alpha+(k-d)/2>0$. The proper joint [posterior density](bayesian-statistics.md#posterior-density) is proportional to

$$
\gamma^{a-1}\exp\left[-\gamma\left(b_0+\tfrac12(u-u_*)^TB(u-u_*)\right)\right].
$$

Its [conditional distributions](probability-theory.md#conditional-distribution) are $u\mid\gamma,m\sim\mathcal N(u_*,\gamma^{-1}B^{-1})$ and $\gamma\mid u,m\sim\operatorname{Gamma}(a,\beta+\|m-Au\|^2/2)$. Its marginal precision law is $\operatorname{Gamma}(s,b_0)$. Integration of the displayed kernel gives $(2\pi)^{d/2}\Gamma(s)/(\sqrt{\det B}\,b_0^s)$, proving propriety despite the [improper prior](bayesian-statistics.md#improper-prior).

A joint [maximum a posteriori estimate](bayesian-statistics.md#maximum-a-posteriori-estimate) relative to $du\,d\gamma$ exists exactly when $a>1$, and is $(u_*,(a-1)/b_0)$. If $a=1$, the supremum is approached at $\gamma=0$ but not attained; if $a<1$, the density is unbounded there. Separate marginal maximization gives $u_*$ for the unknown and $(s-1)/b_0$ for the precision when $s>1$. This illustrates that joint and marginal modes need not agree, and that a proper [posterior distribution](bayesian-statistics.md#bayesian-posterior) need not have a mode in its open parameter space.

### Gaussian posterior in the zero-noise limit

↑ **Parent:** [Gaussian conjugacy for a normal linear model](#gaussian-conjugacy-for-a-normal-linear-model)

For $m=Au+\eta$, with independent $u\sim\mathcal N(0,I_d)$ and $\eta\sim\mathcal N(0,\delta^2I_k)$, the [multivariate normal distribution](probability-and-statistics.md#multivariate-normal-distribution) of the [Bayesian posterior](bayesian-statistics.md#bayesian-posterior) has [posterior mean](bayesian-statistics.md#posterior-mean) $b_\delta=(A^TA+\delta^2I_d)^{-1}A^Tm$ and [covariance matrix](variance.md#covariance-matrix) $C_\delta=\delta^2(A^TA+\delta^2I_d)^{-1}$. The [singular value decomposition](linear-algebra.md#singular-value-decomposition) shows that the variance on a right singular vector of nonzero [singular value](linear-algebra.md#singular-value) $s$ is $\delta^2/(s^2+\delta^2)$, while the variance along the [null space](kernel-of-a-linear-map.md) is one. Thus, for fixed data, the mean tends to the [minimum-norm least-squares solution](inverse-problem.md#minimum-norm-least-squares-solution) and the covariance tends to the [orthogonal projection](hilbert-space.md#orthogonal-projection) onto the [null space](kernel-of-a-linear-map.md). Unobserved components retain their [prior distribution](bayesian-statistics.md#prior-probability) even as the noise vanishes.

### Gaussian likelihood

↑ **Parent:** [Gaussian conjugacy for a normal linear model](#gaussian-conjugacy-for-a-normal-linear-model)

A Gaussian likelihood is a [likelihood function](maximum-likelihood-estimation.md#likelihood-function) obtained by modeling the observations conditionally with a [normal distribution](probability-distribution.md#normal-distribution).

<h2 id="cochran-s-theorem">Cochran's theorem</h2>

↑ **Parent:** [Normal linear model](normal-linear-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cochran's_theorem)

Orthogonal projections of an isotropic Gaussian vector are independent. If $P$ is an orthogonal projection of rank $r$ and $Z\sim N(0,I)$, then

$$
\|PZ\|^2\sim\chi_r^2.
$$

<h3 id="rank-sum-form-of-cochran-s-theorem">Rank-sum form of Cochran's theorem</h3>

↑ **Parent:** [Cochran's theorem](#cochran-s-theorem)

Let $A_i$ be real [symmetric matrices](linear-algebra.md#symmetric-matrix) with sum $I_n$. Their [matrix ranks](vector-space.md#matrix-rank) sum to at least $n$, because their ranges span $\mathbb R^n$. If the ranks sum to $n$, those ranges form a [direct sum](vector-space.md#direct-sum). For $y$ in the range of $A_i$, the identity $y=\sum_jA_jy$ and uniqueness of its range decomposition imply $A_jy=\delta_{ij}y$. Thus $A_i^2=A_i$ and $A_iA_j=0$ for $i\ne j$: the matrices are mutually orthogonal [orthogonal projections](hilbert-space.md#orthogonal-projection). In a combined [orthonormal basis](inner-product.md#orthonormal-basis), the forms $Z^TA_iZ$ for $Z\sim N_n(0,I_n)$ use disjoint sets of independent standard normal coordinates. They are independent [chi-squared distributions](probability-distribution.md#chi-squared-distribution) with degrees of freedom equal to the ranks. Conversely, if all these forms have those chi-squared laws, their expectations and their sum give $\sum_i\operatorname{rank}A_i=n$.

## Linear regression

↑ **Parent:** [Normal linear model](normal-linear-model.md)

[This section is present in another page, follow this link to view it.](linear-regression.md)

## R linear-model formula

↑ **Parent:** [Normal linear model](normal-linear-model.md)

In R, `lm(y ~ 1, data=d)` fits an intercept-only linear model, `lm(y ~ x1 + x2, data=d)` adds quantitative predictors, and a factor predictor is expanded into indicator columns.

### Treatment coding

↑ **Parent:** [R linear-model formula](#r-linear-model-formula)

Treatment coding sets one [reference level in a regression factor](generalized-linear-model.md#reference-level-in-a-regression-factor) to zero and represents each other level by an indicator column. With two interacting factors, a main-effect coefficient compares levels at the other factor's reference level; an interaction coefficient is a difference of these contrasts. A joint [nested-model F-test](probability-and-statistics.md#nested-model-f-test) can be significant even when some individual coefficient tests are not.

### Degrees of freedom of a factor predictor

↑ **Parent:** [R linear-model formula](#r-linear-model-formula)

With an intercept present, a categorical predictor having $m$ represented levels adds $m-1$ linearly independent indicator columns and therefore $m-1$ model degrees of freedom.

## Hat matrix

↑ **Parent:** [Normal linear model](normal-linear-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hat_matrix)

The hat matrix

$$
H=X(X^TX)^{-1}X^T
$$

is the orthogonal projection onto the column space of a full-rank design matrix, and the fitted response is $\widehat Y=HY$.

### Fitted-residual orthogonality

↑ **Parent:** [Hat matrix](#hat-matrix)

For a full-rank [ordinary least squares](#ordinary-least-squares) [design matrix](linear-regression.md#design-matrix), the [hat matrix](#hat-matrix) $H$ and residual projection $G=I-H$ satisfy $HG=GH=0$. Hence [fitted values](linear-regression.md#fitted-values) and [regression residuals](probability-and-statistics.md#regression-residual) are perpendicular as observed vectors. Under isotropic errors their cross-[covariance matrix](variance.md#covariance-matrix) is zero, and under a [normal linear model](normal-linear-model.md) the two vectors are independent.

## Normal linear-model confidence ellipsoid

↑ **Parent:** [Normal linear model](normal-linear-model.md)

With $\widehat\sigma^2=\|Y-X\widehat\beta\|^2/(n-p)$, a simultaneous $(1-\alpha)$ confidence region for $\beta$ is

$$
(\beta-\widehat\beta)^TX^TX(\beta-\widehat\beta)
\leq p\widehat\sigma^2F_{p,n-p}(1-\alpha).
$$

<h3 id="cook-s-distance">Cook's distance</h3>

↑ **Parent:** [Normal linear-model confidence ellipsoid](#normal-linear-model-confidence-ellipsoid)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cook's_distance)

If $\widehat\beta_{(i)}$ is the least-squares estimate after deleting observation $i$, Cook's distance is

$$
D_i=\frac{(\widehat\beta_{(i)}-\widehat\beta)^TX^TX
(\widehat\beta_{(i)}-\widehat\beta)}{p\widehat\sigma^2}
=\frac{\|\widehat Y_{(i)}-\widehat Y\|^2}{p\widehat\sigma^2}.
$$

It measures the deleted estimate in the same quadratic metric as the coefficient confidence ellipsoid.

## Multicollinearity

↑ **Parent:** [Normal linear model](normal-linear-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multicollinearity)

Multicollinearity means that predictor columns are strongly linearly related. It inflates coefficient variances and can make individual effects imprecise even when a joint test strongly rejects that all corresponding coefficients vanish.

### Variance inflation factor

↑ **Parent:** [Multicollinearity](#multicollinearity)

For a slope in a regression with an intercept, the variance inflation factor is $1/(1-R_j^2)$, where $R_j^2$ comes from regressing its predictor on all the others. With one other predictor it is $1/(1-r^2)$, quantifying the increase in conditional estimation variance.

### Two-predictor variance inflation

↑ **Parent:** [Multicollinearity](#multicollinearity)

For two centered predictors with squared norms $n$ and [correlation coefficient](variance.md#pearson-correlation-coefficient) $\rho$, the [ordinary least squares](#ordinary-least-squares) estimate of either partial slope has [variance](variance.md) $\sigma^2/[n(1-\rho^2)]$. Compared with the same predictor alone and the same error variance, the inflation factor is $1/(1-\rho^2)$. The [eigenvalues](linear-operator-theory.md#eigenvalue) of the slope [Gram matrix](inner-product.md#gram-matrix) are $n(1+\rho)$ and $n(1-\rho)$.

## Ordinary least squares

↑ **Parent:** [Normal linear model](normal-linear-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ordinary_least_squares)

Ordinary least squares minimizes the unweighted sum of squared residuals between observed and fitted responses.

### Residual estimate of Gaussian noise variance

↑ **Parent:** [Ordinary least squares](#ordinary-least-squares)

For a correctly specified full-rank fixed-design Gaussian [linear regression](linear-regression.md) with $p<n$, dividing the [residual sum of squares](linear-regression.md#residual-sum-of-squares) by the [residual degrees of freedom](statistical-modelling.md#residual-degrees-of-freedom) $n-p$ gives an [unbiased estimator](statistical-modelling.md#unbiased-estimator) of the noise [variance](variance.md). The projection removes the whole deterministic mean, so the numerator's expectation is $(n-p)\sigma^2$. A misspecified subset model need not have this property.

#### Residual standard error

↑ **Parent:** [Residual estimate of Gaussian noise variance](#residual-estimate-of-gaussian-noise-variance)

In a full-rank [normal linear model](normal-linear-model.md) with $n$ observations and $p$ mean coefficients, the residual standard error estimates the common error standard deviation. Its square is the [unbiased estimator](statistical-modelling.md#unbiased-estimator) $\operatorname{RSS}/(n-p)$; the square root itself is not generally unbiased. It measures unexplained response variation, whereas a regression coefficient's [standard error](statistical-inference.md#standard-error) measures uncertainty in that coefficient.

### Partial regression

↑ **Parent:** [Ordinary least squares](#ordinary-least-squares)

Partial regression first projects a response and a selected predictor orthogonally off the remaining design columns. Regressing the residualized response on the residualized predictor yields its coefficient in the full [ordinary least squares](#ordinary-least-squares) fit.

### Rank-deficient ordinary least squares

↑ **Parent:** [Ordinary least squares](#ordinary-least-squares)

If a [design matrix](linear-regression.md#design-matrix) $X$ has deficient [rank](quadratic-form.md#rank-one-quadratic-form), every [ordinary least squares](#ordinary-least-squares) minimizer has the form $X^+Y+z$ with $z\in\ker X$, where $X^+$ is the [Moore-Penrose inverse](matrix-inverse.md#moore-penrose-inverse). Hence the fitted values are unique but the coefficients are not: the minimizers form an [affine subspace](vector-space.md#affine-subspace) of dimension $p-\operatorname{rank}X$.

#### Nonidentifiability prevents unbiased coefficient estimation

↑ **Parent:** [Rank-deficient ordinary least squares](#rank-deficient-ordinary-least-squares)

If a [design matrix](linear-regression.md#design-matrix) $X$ has a nonzero null vector $z$, the [normal linear model](normal-linear-model.md) has identical observation distributions at $\beta$ and $\beta+z$. Any estimator has the same expectation at those two parameters, and therefore cannot be an [unbiased estimator](statistical-modelling.md#unbiased-estimator) of both coefficient vectors. Full column rank is required for unbiased estimation of the entire unconstrained coefficient vector; identifiable linear combinations can still be estimated without it.

### Linear regression through the origin

↑ **Parent:** [Ordinary least squares](#ordinary-least-squares)

In the model $Y_i=\beta x_i+\varepsilon_i$ without an intercept, with $\sum_i x_i^2>0$, the ordinary least-squares estimator is

$$
\widehat\beta=\frac{\sum_i x_iY_i}{\sum_i x_i^2}.
$$

For independent errors of common variance $\sigma^2$, it is unbiased and has variance $\sigma^2/\sum_i x_i^2$.

#### Residual estimate of slope uncertainty through the origin

↑ **Parent:** [Linear regression through the origin](#linear-regression-through-the-origin)

For independent errors of common unknown [variance](variance.md) in $Y_i=\beta x_i+\varepsilon_i$, the [ordinary least squares](#ordinary-least-squares) estimate is $\widehat\beta=\sum_i x_iY_i/\sum_i x_i^2$. Fitting one parameter leaves $n-1$ residual [degrees of freedom](classical-mechanics.md#degree-of-freedom). Therefore $s^2=\sum_i(Y_i-\widehat\beta x_i)^2/(n-1)$ estimates the common error [variance](variance.md), and $s^2/\sum_i x_i^2$ estimates the slope [variance](variance.md). For errors with a [Gaussian distribution](probability-distribution.md#normal-distribution), the slope's standardized deviation follows a [Student's t-distribution](continuous-probability-distribution.md#student-s-t-distribution) with $n-1$ [degrees of freedom](classical-mechanics.md#degree-of-freedom). A common [calibration](differential-geometry.md#calibration-differential-geometry) bias does not appear as independent residual scatter.

#### Student t test for regression through the origin

↑ **Parent:** [Linear regression through the origin](#linear-regression-through-the-origin)

For independent $Y_i\sim N(\beta x_i,\sigma^2)$ with $n\geq2$ and $\sum x_i^2>0$, the [least-squares estimator](#ordinary-least-squares-estimators) is $\widehat\beta=\sum x_iY_i/\sum x_i^2$. The projection of the isotropic [Gaussian vector](probability-and-statistics.md#gaussian-random-vector) onto the design direction is independent of its orthogonal residual; hence $\widehat\beta\sqrt{\sum x_i^2}/\sigma$ is standard normal under $\beta=0$ and $\mathrm{SSE}/\sigma^2$ is independent chi-squared with $n-1$ degrees of freedom. The displayed statistic therefore has [Student's t-distribution](continuous-probability-distribution.md#student-s-t-distribution) with $n-1$ degrees of freedom. A two-sided test rejects at the corresponding upper/lower quantiles. The zero design has no information about the slope; with one observation there is no residual variance degree of freedom.

### Ordinary least squares estimators

↑ **Parent:** [Ordinary least squares](#ordinary-least-squares)

For a [linear regression](linear-regression.md) design matrix $X$ with [full column rank](vector-space.md#full-column-rank), the [ordinary least squares](#ordinary-least-squares) coefficient vector is $\widehat\beta=(X^TX)^{-1}X^TY$. In a [normal linear model](normal-linear-model.md) with error [covariance matrix](variance.md#covariance-matrix) $\sigma^2I$, it is an [unbiased estimator](statistical-modelling.md#unbiased-estimator) with [covariance matrix](variance.md#covariance-matrix) $\sigma^2(X^TX)^{-1}$. Replacing $\sigma^2$ by the residual variance estimate gives the reported coefficient [standard errors](statistical-inference.md#standard-error).

In simple [linear regression](linear-regression.md) with a nonconstant predictor,

$$
\widehat\beta=\frac{\sum_i(x_i-\bar x)(Y_i-\bar Y)}
{\sum_i(x_i-\bar x)^2},
\qquad
\widehat\alpha=\bar Y-\widehat\beta\bar x.
$$

#### Residual sum of squares in simple linear regression

↑ **Parent:** [Ordinary least squares estimators](#ordinary-least-squares-estimators)

For a nonconstant predictor, put

$$
S_{xx}=\sum_i(x_i-\bar x)^2,
\quad
S_{xy}=\sum_i(x_i-\bar x)(y_i-\bar y),
\quad
S_{yy}=\sum_i(y_i-\bar y)^2.
$$

The minimized residual sum of squares is

$$
\operatorname{RSS}=S_{yy}-\frac{S_{xy}^2}{S_{xx}}.
$$

Each centered sum can be recovered in constant time from the five raw sums $\sum x_i$, $\sum y_i$, $\sum x_i^2$, $\sum x_iy_i$, and $\sum y_i^2$.

## Gauss-Markov theorem

↑ **Parent:** [Normal linear model](normal-linear-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gauss-Markov_theorem)

Among linear unbiased estimators in a homoscedastic linear model, least squares has minimum variance.

## Weighted least squares

↑ **Parent:** [Normal linear model](normal-linear-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weighted_least_squares)

Weighted least squares minimizes $\sum_iw_i(Y_i-X_i^T\beta)^2$; inverse-variance weights give the efficient estimator under known heteroscedasticity.

### Gamma-ray energy-network fit

↑ **Parent:** [Weighted least squares](#weighted-least-squares)

For a proposed gamma-transition graph, fix the [ground-state energy](quantum-mechanics.md#ground-state-energy) and fit the remaining level energies with a linear incidence [matrix](vector-space.md#matrix). Loops give consistency constraints and correlated excitation-energy errors. Different transition graphs can have the same minimized residuals if they rearrange the same energy-sum identities; a small chi-squared is not then a unique level assignment.

### Additional measurements decrease known-error covariance

↑ **Parent:** [Weighted least squares](#weighted-least-squares)

Independent observations with known errors add a positive-semidefinite [Fisher information matrix](statistical-modelling.md#fisher-information-matrix) $G$ to the existing information $F$. Writing $F+G=F^{1/2}(I+F^{-1/2}GF^{-1/2})F^{1/2}$ shows its inverse covariance cannot increase in any parameter direction. Improvement can be zero along an uninformative direction. This statement does not assume that data-dependent residual [variance](variance.md) estimates or model [systematic errors](physics.md#systematic-error) must decrease.

### Fixed-phase sinusoidal least squares

↑ **Parent:** [Weighted least squares](#weighted-least-squares)

When [frequency](wave.md#frequency) and phase are known, sinusoidal [amplitude](wave.md#wave-amplitude) and offset fitting is a two-parameter [linear regression](linear-regression.md). For equal known errors $\sigma$, profiling out the offset gives $K=\sum(s_i-\bar s)(y_i-\bar y)/\sum(s_i-\bar s)^2$ and $\operatorname{Var}(K)=\sigma^2/\sum(s_i-\bar s)^2$. Identical phases cannot separate [amplitude](wave.md#wave-amplitude) from offset. Unknown phase instead requires independent sine and cosine coefficients.

### Variable projection

↑ **Parent:** [Weighted least squares](#weighted-least-squares)

In [variable projection](#variable-projection), a prediction has the form $\mathbf G(\mathbf q)\mathbf m$, nonlinear in $\mathbf q$ but [linear](vector-space.md#linearity) in $\mathbf m$. For each trial $\mathbf q$, solve the inner [weighted least squares](#weighted-least-squares) problem for $\mathbf m$, then optimize the resulting residual over $\mathbf q$. This reduces the nonlinear dimension without pretending that the whole [inverse problem](inverse-problem.md) is [linear](vector-space.md#linearity).

### Generalized least squares

↑ **Parent:** [Weighted least squares](#weighted-least-squares)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Generalized_least_squares)

Generalized least squares minimizes $(Y-X\beta)^T\Omega^{-1}(Y-X\beta)$ for a known covariance shape $\Omega$.

#### Whitening transformation

↑ **Parent:** [Generalized least squares](#generalized-least-squares)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Whitening_transformation)

Whitening multiplies a model by a square root of its precision matrix so that the transformed errors have identity covariance.

## Normal equation

↑ **Parent:** [Normal linear model](normal-linear-model.md)

Least-squares differentiation gives $X^TX\widehat\beta=X^TY$, or its precision-weighted analogue.

## Consistency of least squares

↑ **Parent:** [Normal linear model](normal-linear-model.md)

Under finite moments and a nonsingular limiting design moment, laws of large numbers make least-squares estimators converge to the true coefficient.

## One-way normal linear model

↑ **Parent:** [Normal linear model](normal-linear-model.md)

A one-way normal model assigns each factor level its own mean while assuming independent Gaussian errors with a common variance.

This Gaussian model is the setting for a one-way instance of [analysis of variance](linear-regression.md#analysis-of-variance).

### Cell-means parametrization

↑ **Parent:** [One-way normal linear model](#one-way-normal-linear-model)

A cell-means model uses one coefficient per factor level and no intercept, so each coefficient directly equals a group mean.

#### Equal-cell replication variance formula

↑ **Parent:** [Cell-means parametrization](#cell-means-parametrization)

Suppose a [normal linear model](normal-linear-model.md) gives an unrestricted mean to each cell and has $m$ [independent](random-variable.md#independent-random-variables) observations per cell, with common error [variance](variance.md) $\sigma^2$. Each fitted cell mean is its [sample mean](variance.md#sample-mean), with [variance](variance.md) $\sigma^2/m$; different fitted cell means are [independent](random-variable.md#independent-random-variables). Estimate $\sigma^2$ by the pooled within-cell [residual sum of squares](linear-regression.md#residual-sum-of-squares) divided by $n-q$, where $q$ is the number of cells. Thus a cell mean has [standard error](statistical-inference.md#standard-error) $s/\sqrt m$, a difference of two cell means has [standard error](statistical-inference.md#standard-error) $s\sqrt{2/m}$, and a two-by-two difference-of-differences has [standard error](statistical-inference.md#standard-error) $2s/\sqrt m$.

// Target: probability-and-statistics.bigb

#### Linear contrast of cell means

↑ **Parent:** [Cell-means parametrization](#cell-means-parametrization)

A linear contrast is a coefficient-weighted sum of cell means whose coefficients total zero, used to test interpretable differences among groups.

##### Treatment contrast

↑ **Parent:** [Linear contrast of cell means](#linear-contrast-of-cell-means)

A [treatment contrast](#treatment-contrast) is a [linear contrast of cell means](#linear-contrast-of-cell-means) comparing treatment responses, with coefficients adding to zero. Pairwise differences and marginal factorial differences are examples. Its [variance](variance.md) depends on the true allocation units and their [covariance matrix](variance.md#covariance-matrix).

###### Orthogonal polynomial contrast

↑ **Parent:** [Treatment contrast](#treatment-contrast)

At equally replicated quantitative treatment levels, evaluations of [orthogonal polynomials](orthogonal-polynomial.md) generate pairwise [orthogonal](inner-product.md#orthogonal-vectors) [treatment contrasts](#treatment-contrast), using the replication-weighted [inner product](inner-product.md). Five equally spaced levels give four contrast directions representing degrees one through four, besides the constant direction. This decomposes treatment variation without assuming the response has low polynomial degree.

###### Variance of a treatment contrast

↑ **Parent:** [Treatment contrast](#treatment-contrast)

For a vector of estimated treatment means $\widehat\mu$, the [variance of a treatment contrast](#variance-of-a-treatment-contrast) with coefficient vector $c$ is $c^T\operatorname{Cov}(\widehat\mu)c$. Averaging subsamples from a common [experimental unit](design-of-experiments.md#experimental-unit) does not make their shared [variance component](generalized-linear-model.md#variance-component) disappear.

###### Interaction contrast

↑ **Parent:** [Treatment contrast](#treatment-contrast)

An [interaction contrast](#interaction-contrast) compares a treatment difference across levels of another factor. A nonzero difference of differences shows that an additive representation of those cell means is inadequate. Its [standard error](statistical-inference.md#standard-error) must use the error stratum in which that [interaction term](statistical-model.md#interaction-term) is randomized.

###### Logistic interaction as a ratio of odds ratios

↑ **Parent:** [Interaction contrast](#interaction-contrast)

For binary predictors $A,B$, a [logistic regression](generalized-linear-model.md#logistic-regression) with [linear predictor](generalized-linear-model.md#linear-predictor) $a+bA+cB+\delta AB$ has conditional [odds ratios](statistical-modelling.md#odds-ratio) $e^b$ at $B=0$ and $e^{b+\delta}$ at $B=1$. Their ratio is $e^\delta$. The same interaction can be computed from the four cell [logit link](generalized-linear-model.md#logit) values as $\delta=\eta_{11}-\eta_{10}-\eta_{01}+\eta_{00}$. Independent positive event and nonevent counts in each cell give an estimated [variance](variance.md) for this contrast equal to the sum of all eight reciprocal counts. An interaction on the [odds ratio](statistical-modelling.md#odds-ratio) scale is not an interaction on the absolute-risk scale.

### Full-dominance mean constraint

↑ **Parent:** [One-way normal linear model](#one-way-normal-linear-model)

For genotypes $aa,Aa,AA$, full dominance of allele $A$ imposes $\mu_{Aa}=\mu_{AA}$.

### Additive allele-count model

↑ **Parent:** [One-way normal linear model](#one-way-normal-linear-model)

With allele counts $0,1,2$, no dominance makes the genotype mean affine in count and imposes $2\mu_{Aa}=\mu_{aa}+\mu_{AA}$.

## ↑ Ancestors (6)

1. [Statistical modelling](statistical-modelling.md)
2. [Statistical model](statistical-model.md)
3. [Probability and statistics](probability-and-statistics.md)
4. [Area of mathematics](mathematics.md#area-of-mathematics)
5. [Mathematics](mathematics.md)
6. [Codex Wiki](README.md)

## ← Incoming links (104)

- [Adjusted coefficient of determination](linear-regression.md#adjusted-coefficient-of-determination)
- [Analysis of covariance](#analysis-of-covariance)
- [Analysis of variance](linear-regression.md#analysis-of-variance)
- [Balanced factorial orthogonality](linear-regression.md#balanced-factorial-orthogonality)
- [Coefficient of determination](linear-regression.md#coefficient-of-determination)
- [Corner-point constraint](statistical-model.md#corner-point-constraint)
- [Distribution of an internally studentized Gaussian residual](probability-and-statistics.md#distribution-of-an-internally-studentized-gaussian-residual)
- [Distribution of the Akaike information criterion in a normal linear model](statistical-modelling.md#distribution-of-the-akaike-information-criterion-in-a-normal-linear-model)
- [Equal-cell replication variance formula](#equal-cell-replication-variance-formula)
- [Extra sum of squares](probability-and-statistics.md#extra-sum-of-squares)
- [Factor-level pooling test](#factor-level-pooling-test)
- [Fitted-residual orthogonality](#fitted-residual-orthogonality)
- [Gaussian identity design for debiased Lasso](lasso.md#gaussian-identity-design-for-debiased-lasso)
- [Gaussian independence of linear and quadratic statistics](probability-and-statistics.md#gaussian-independence-of-linear-and-quadratic-statistics)
- [Lack-of-fit F-test](#lack-of-fit-f-test)
- [Linear regression](linear-regression.md)
- [Nonidentifiability prevents unbiased coefficient estimation](#nonidentifiability-prevents-unbiased-coefficient-estimation)
- [Normal-inverse-gamma prior](exponential-family.md#normal-inverse-gamma-prior)
- [Normal Q-Q plot](probability-and-statistics.md#normal-q-q-plot)
- [Ordinary least squares estimators](#ordinary-least-squares-estimators)
- [Orthogonal coefficient blocks in a centered normal linear model](statistical-modelling.md#orthogonal-coefficient-blocks-in-a-centered-normal-linear-model)
- [Partial F-test for nested linear models](probability-and-statistics.md#partial-f-test-for-nested-linear-models)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-28.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-28.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-28.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-30.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-36.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-36.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-39.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-38.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-42.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-42.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-37.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-41.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-41.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-41.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-44.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-43.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-44.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3.md#5j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-41.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-41.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-1.md#7h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-102.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-34.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-38.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-4.md#5j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-37.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-37.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-37.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-37.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1.md#13j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-37.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-37.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-37.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-37.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-1.md#19h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30.md#1/f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30.md#2/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-31.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-35.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-4.md#19h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-33.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-33.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-3.md#20h/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-3.md#20h/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#5j/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2.md#5j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-205.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4.md#5j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-205.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218.md#6/f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4.md#5j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3.md#5j/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-3.md#18h/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4.md#5j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4.md#5j/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-218.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-1.md#13l/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-1.md#5k/solution)
- [Solution](past-exam-of-the-systems-biology-course-of-the-university-of-cambridge/2024/paper-3.md#1/e/solution)
- [Power transform](statistical-modelling.md#power-transform)
- [Prediction interval for a ratio of log-normal responses](statistical-inference.md#prediction-interval-for-a-ratio-of-log-normal-responses)
- [Prediction interval in a normal linear model](statistical-inference.md#prediction-interval-in-a-normal-linear-model)
- [Predictor centering](linear-regression.md#predictor-centering)
- [Regression coefficient test power ignores nuisance coefficients](statistical-hypothesis-test.md#regression-coefficient-test-power-ignores-nuisance-coefficients)
- [Residual-score decomposition from square-root Lasso](lasso.md#residual-score-decomposition-from-square-root-lasso)
- [Residual standard error](#residual-standard-error)
- [Simple linear regression](linear-regression.md#simple-linear-regression)
- [Standardized regression residual](probability-and-statistics.md#standardized-regression-residual)
- [Statistical degrees of freedom](statistical-inference.md#statistical-degrees-of-freedom)
- [Stepwise selection by the Akaike information criterion](statistical-modelling.md#stepwise-selection-by-the-akaike-information-criterion)
- [Two-factor normal linear model](#two-factor-normal-linear-model)
- [Variance of a fitted regression mean](#variance-of-a-fitted-regression-mean)
