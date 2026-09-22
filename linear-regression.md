# Linear regression

↑ **Parent:** [Normal linear model](statistical-modelling.md#normal-linear-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_regression)

Linear regression models a response mean as a linear combination $X\beta$ of predictors. Ordinary least squares chooses $\beta$ to minimize the sum of squared residuals.

**Table of contents**

- [Multiple linear regression](#multiple-linear-regression)
- [Normal equations for linear least squares](#normal-equations-for-linear-least-squares)
- [Omitted-variable bias](#omitted-variable-bias)
- [Predictor centering](#predictor-centering)
- [Regression diagnostics](#regression-diagnostics)
  - [Influential observation](#influential-observation)
  - [Regression outlier](#regression-outlier)
- [Least angle regression](#least-angle-regression)
  - [Equiangular direction in least angle regression](#equiangular-direction-in-least-angle-regression)
  - [Sign compatibility of LAR and Lasso](#sign-compatibility-of-lar-and-lasso)
  - [LAR active correlation invariant](#lar-active-correlation-invariant)
  - [Entry knot in least angle regression](#entry-knot-in-least-angle-regression)
- [Reciprocal-predictor regression](#reciprocal-predictor-regression)
- [Regression intercept](#regression-intercept)
  - [Student t test for a simple-regression intercept](#student-t-test-for-a-simple-regression-intercept)
- [Polynomial regression](#polynomial-regression)
  - [Independent normal and inverse-gamma regression priors](#independent-normal-and-inverse-gamma-regression-priors)
  - [Quadratic regression](#quadratic-regression)
- [Coefficient of determination](#coefficient-of-determination)
  - [Adjusted coefficient of determination](#adjusted-coefficient-of-determination)
- [Residual-versus-fitted plot](#residual-versus-fitted-plot)
  - [Scale-location plot](#scale-location-plot)
- [Analysis of variance](#analysis-of-variance)
  - [Multivariate analysis of variance](#multivariate-analysis-of-variance)
    - [Within-group and between-group scatter decomposition](#within-group-and-between-group-scatter-decomposition)
    - [Wilks lambda statistic](#wilks-lambda-statistic)
  - [Two-way analysis of variance](#two-way-analysis-of-variance)
    - [Missing cells can destroy factor orthogonality in two-way ANOVA](#missing-cells-can-destroy-factor-orthogonality-in-two-way-anova)
    - [Identifiability of an incomplete two-factor additive design](#identifiability-of-an-incomplete-two-factor-additive-design)
    - [Saturation of an unreplicated two-factor regression](#saturation-of-an-unreplicated-two-factor-regression)
  - [Sequential sum of squares](#sequential-sum-of-squares)
  - [Sum of squares in ANOVA](#sum-of-squares-in-anova)
    - [Mean square in ANOVA](#mean-square-in-anova)
  - [ANOVA stratum](#anova-stratum)
    - [Within-block ANOVA stratum](#within-block-anova-stratum)
  - [Balanced factorial orthogonality](#balanced-factorial-orthogonality)
- [Frisch–Waugh–Lovell theorem](#frisch-waugh-lovell-theorem)
- [Simple linear regression](#simple-linear-regression)
  - [Centred simple linear regression](#centred-simple-linear-regression)
- [Residual sum of squares](#residual-sum-of-squares)
- [Ridge regression](#ridge-regression)
  - [Gaussian posterior representation of ridge regression](#gaussian-posterior-representation-of-ridge-regression)
  - [Unbounded directional risk of fixed ridge shrinkage](#unbounded-directional-risk-of-fixed-ridge-shrinkage)
  - [Uniform directional risk improvement by ridge regression](#uniform-directional-risk-improvement-by-ridge-regression)
  - [Unpenalized intercept in ridge regression](#unpenalized-intercept-in-ridge-regression)
  - [Covariance and bias of a ridge regression estimator](#covariance-and-bias-of-a-ridge-regression-estimator)
  - [Closed-form ridge regression estimator](#closed-form-ridge-regression-estimator)
    - [Vanishing-penalty ridge limit](#vanishing-penalty-ridge-limit)
    - [Primal-dual identity for ridge regression](#primal-dual-identity-for-ridge-regression)
    - [Principal-component shrinkage by ridge regression](#principal-component-shrinkage-by-ridge-regression)
- [Fitted values](#fitted-values)
  - [Linear smoother](#linear-smoother)
    - [Effective degrees of freedom](#effective-degrees-of-freedom)
- [Design matrix](#design-matrix)
  - [Confounding of nested fixed factors](#confounding-of-nested-fixed-factors)
- [Regression coefficient](#regression-coefficient)
- [Attenuation bias from classical measurement error](#attenuation-bias-from-classical-measurement-error)

## Multiple linear regression

↑ **Parent:** [Linear regression](linear-regression.md)

[Multiple linear regression](#multiple-linear-regression) models a scalar response by an intercept and several predictors. It is linear in the [regression coefficients](#regression-coefficient), even when predictors include transformed variables or interactions. In an [observational study](causal-inference.md#observational-study), adjustment can address measured [confounding](causal-inference.md#confounding), but does not automatically identify a [causal effect](causal-inference.md#causal-effect). Improvements in fitted [coefficient of determination](#coefficient-of-determination) require external predictive assessment rather than being treated as proof of improved future prediction.

## Normal equations for linear least squares

↑ **Parent:** [Linear regression](linear-regression.md)

Minimizing $\|y-X\theta\|^2$ gives the displayed equations by differentiation. If the design matrix has full column rank, the minimizer is unique and the fitted vector is the [orthogonal projection](hilbert-space.md#orthogonal-projection) of $y$ onto its column space. For an intercept and one explanatory variable, these equations give $\widehat\beta=S_{xy}/S_{xx}$ and $\widehat\alpha=\bar y-\widehat\beta\bar x$, provided $S_{xx}>0$.

## Omitted-variable bias

↑ **Parent:** [Linear regression](linear-regression.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Omitted-variable_bias)

If the true conditional mean is $\beta_0+\beta_1X+\beta_2Z$, the population slope from regressing on $X$ alone is $\beta_1+\beta_2\operatorname{Cov}(X,Z)/\operatorname{Var}(X)$, assuming a mean-zero error uncorrelated with the predictors. The omitted predictor can steepen, flatten, or reverse the pooled association. The same identity holds for fitted coefficients and empirical [covariances](variance.md#covariance) when comparing nested ordinary least-squares fits. Adjustment changes the comparison being described; a causal interpretation requires additional assumptions.

## Predictor centering

↑ **Parent:** [Linear regression](linear-regression.md)

Replacing a numerical predictor $x$ by $x-c$ preserves the fitted mean space and slope in a [linear regression](linear-regression.md) containing an intercept. The intercept becomes the fitted mean at $x=c$. In [simple linear regression](#simple-linear-regression), centering at the sample mean makes intercept and slope estimates uncorrelated under a [normal linear model](statistical-modelling.md#normal-linear-model). This changes coefficient interpretation, not predictions.

## Regression diagnostics

↑ **Parent:** [Linear regression](linear-regression.md)

Regression diagnostics check assumptions and influential observations in a fitted [regression function](statistical-learning.md#regression-function). [Residual-versus-fitted plots](#residual-versus-fitted-plot) can reveal omitted mean structure or nonconstant [variance](variance.md); a [quantile-quantile plot](probability-and-statistics.md#q-q-plot) checks a specified error distribution. [Regression leverage](statistical-modelling.md#regression-leverage) measures unusual predictor configurations, and [Cook's distance](statistical-modelling.md#cook-s-distance) combines leverage and residual size to measure coefficient sensitivity. Independence may require checking collection order and the study design in addition to residual plots.

### Influential observation

↑ **Parent:** [Regression diagnostics](#regression-diagnostics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Influential_observation)

An [influential observation](#influential-observation) substantially changes a fitted model or its predictions when removed or perturbed. In a [linear regression](linear-regression.md), influence depends jointly on residual size and [regression leverage](statistical-modelling.md#regression-leverage). Large predictor leverage with a small residual and a large residual at ordinary leverage can have different consequences. [Regression diagnostics](#regression-diagnostics) examine this sensitivity; influence is not synonymous with an invalid observation.

### Regression outlier

↑ **Parent:** [Regression diagnostics](#regression-diagnostics)

A [regression outlier](#regression-outlier) has a response unusually far from its fitted conditional mean. A [standardized regression residual](probability-and-statistics.md#standardized-regression-residual) adjusts for [regression leverage](statistical-modelling.md#regression-leverage); an externally studentized residual also estimates noise [variance](variance.md) with the observation deleted. Selecting the largest residual among many observations changes its reference distribution. An outlier need not be an [influential observation](#influential-observation), and unusual valid data should not be discarded solely for being unusual.

## Least angle regression

↑ **Parent:** [Linear regression](linear-regression.md)

A piecewise linear regression-path algorithm which starts at zero, activates a predictor with maximal absolute residual score, and moves in a direction that decreases all active absolute scores equally until another predictor ties them. With $G=X^{\mathsf T}X/n$ and active correlation signs $s_A$, the coefficient direction is $G_{AA}^{-1}s_A$. Ordinary LAR does not drop a predictor when its coefficient crosses zero; [sign compatibility of LAR and Lasso](#sign-compatibility-of-lar-and-lasso) characterizes when its path also obeys the [Lasso](probability-and-statistics.md#lasso) [KKT conditions](mathematical-optimization.md#karush-kuhn-tucker-conditions).

### Equiangular direction in least angle regression

↑ **Parent:** [Least angle regression](#least-angle-regression)

With signed active [covariate](statistical-model.md#covariate) columns $X_A^s=(s_jx_j)_{j\in A}$ and their positive-definite [Gram matrix](linear-algebra.md#gram-matrix) $G_A=(X_A^s)^TX_A^s$, the displayed direction has unit [norm](functional-analysis.md#norm) and $(X_A^s)^Tu=\alpha1$. Thus it makes equal angles with unit-length signed active [covariates](statistical-model.md#covariate), and movement along it reduces their signed residual correlations at the common rate $\alpha$. The [regression coefficient](#regression-coefficient) direction is $d_A=\operatorname{diag}(s_A)w$, with inactive components zero.

### Sign compatibility of LAR and Lasso

↑ **Parent:** [Least angle regression](#least-angle-regression)

If every nonzero active coefficient has the sign of its residual score along the [least angle regression](#least-angle-regression) path, the [LAR active correlation invariant](#lar-active-correlation-invariant) and inactive bounds give the [Karush-Kuhn-Tucker conditions for the Lasso](probability-and-statistics.md#karush-kuhn-tucker-conditions-for-the-lasso). A unique [Lasso](probability-and-statistics.md#lasso) solution then equals the LAR path. Zero coefficients use a [subgradient](real-analysis.md#subgradient) interval; literal sign equality with sign(0)=0 is not appropriate for a newly entering coefficient at a positive knot.

### LAR active correlation invariant

↑ **Parent:** [Least angle regression](#least-angle-regression)

Each [least angle regression](#least-angle-regression) segment starts with all active scores at magnitude $t$. Moving with direction $d_A=G_{AA}^{-1}s_A$ changes the score vector to $t s_A-(t-\lambda)G_{AA}d_A=\lambda s_A$. The first-hit rule bounds every inactive score in magnitude by $\lambda$. This is the key [Lasso](probability-and-statistics.md#lasso) optimality link.

### Entry knot in least angle regression

↑ **Parent:** [Least angle regression](#least-angle-regression)

On a segment starting at residual-score level $t$, an inactive score evolves as $c_j-h a_j$ while the active level is $t-h$. Solving $c_j-h a_j=\pm(t-h)$ gives distances $(t-c_j)/(1-a_j)$ and $(t+c_j)/(1+a_j)$. The smallest positive admissible distance determines the next entry; reaching level zero ends the algorithm.

## Reciprocal-predictor regression

↑ **Parent:** [Linear regression](linear-regression.md)

A reciprocal-predictor [linear regression](linear-regression.md) uses $\mathbb E(Y\mid v)=\alpha+\beta/v$ for nonzero predictor $v$. It remains linear in its coefficients. Its flattening shape can suit a saturating response over a positive predictor range; residual checks and [cross-validation](statistical-learning.md#cross-validation) must assess adequacy, and extrapolation toward zero is hazardous.

## Regression intercept

↑ **Parent:** [Linear regression](linear-regression.md)

The intercept is the coefficient of the constant design column. Adding a constant to a predictor can be absorbed by changing the intercept, leaving fitted values and all slope coefficients unchanged.

### Student t test for a simple-regression intercept

↑ **Parent:** [Regression intercept](#regression-intercept)

For a [Gaussian linear model](statistical-modelling.md#normal-linear-model) with an intercept and one explanatory variable, $n>2$ and $S_{xx}>0$, the [regression intercept](#regression-intercept) estimator is normal with variance $\sigma^2(1/n+\bar x^2/S_{xx})$. The residual variance estimate $s^2=\operatorname{SSE}/(n-2)$ is independent of the coefficient estimators and $(n-2)s^2/\sigma^2$ has a [chi-squared distribution](probability-theory.md#chi-squared-distribution) with $n-2$ degrees of freedom. Consequently the displayed statistic has a [Student t-distribution](continuous-probability-distribution.md#student-s-t-distribution) under $\alpha=\alpha_0$, and a two-sided level-$\eta$ test rejects for $|T|>t_{n-2,1-\eta/2}$.

// Target: mathematical-optimization.bigb

## Polynomial regression

↑ **Parent:** [Linear regression](linear-regression.md)

A [linear regression](linear-regression.md) in the coefficients with a polynomial mean function $\mathbb E(Y\mid t)=\sum_{j=0}^d\beta_jt^j$. Successive degrees define nested models that can be compared by an [F-test](probability-and-statistics.md#f-test).

### Independent normal and inverse-gamma regression priors

↑ **Parent:** [Polynomial regression](#polynomial-regression)

With independent [prior distributions](statistical-inference.md#prior-probability) $\beta\sim N(\mu,\Sigma)$ and $s\sim\operatorname{IG}(a,b)$ in a [normal distribution](probability-theory.md#normal-distribution) regression model, the conditional [posterior distribution](statistical-inference.md#bayesian-posterior) of $\beta$ has [covariance matrix](variance.md#covariance-matrix) $V=(X^TX/s+\Sigma^{-1})^{-1}$ and [mean](probability-theory.md#expected-value) $V(X^Ty/s+\Sigma^{-1}\mu)$. The conditional [posterior distribution](statistical-inference.md#bayesian-posterior) of $s$ is [inverse-gamma distribution](continuous-probability-distribution.md#inverse-gamma-distribution) $\operatorname{IG}(a+n/2,b+\|y-X\beta\|^2/2)$. The shape contains no half-dimension contribution from $\beta$, since its [prior distribution](statistical-inference.md#prior-probability) is independent of $s$. These conditionals give a two-block [Gibbs sampler](statistical-inference.md#gibbs-sampler).

### Quadratic regression

↑ **Parent:** [Polynomial regression](#polynomial-regression)

A [polynomial regression](#polynomial-regression) of degree two is linear in its unknown [regression coefficients](#regression-coefficient) despite being curved in the predictor. Its [design matrix](#design-matrix) has columns $1,x,x^2$; three distinct predictor values give full column [matrix rank](vector-space.md#matrix-rank).

## Coefficient of determination

↑ **Parent:** [Linear regression](linear-regression.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coefficient_of_determination)

In an [ordinary least squares](statistical-modelling.md#ordinary-least-squares) regression with an intercept and a nonconstant response, $R^2=1-\mathrm{RSS}/\sum_i(Y_i-\overline Y)^2$. It measures the fitted proportion of sample variation relative to an intercept-only baseline. It increases when regressors are added, even if those regressors are unhelpful for prediction. A high value does not establish the assumptions of a [normal linear model](statistical-modelling.md#normal-linear-model) or rule out a systematic [regression residual](probability-and-statistics.md#regression-residual) pattern.

### Adjusted coefficient of determination

↑ **Parent:** [Coefficient of determination](#coefficient-of-determination)

In a [normal linear model](statistical-modelling.md#normal-linear-model) with an intercept, $n$ observations and $p$ independent mean coefficients, adjusted $R^2$ is

$$
\overline R^2=1-\frac{\operatorname{RSS}/(n-p)}{\operatorname{SST}/(n-1)}.
$$

It compares the residual [variance](variance.md) estimate with the unmodelled [sample variance](statistical-inference.md#sample-variance), adjusting the raw [coefficient of determination](#coefficient-of-determination) for fitted dimension. It can be negative and is not guaranteed to increase when another regressor is added. In penalized regression a related convention uses the fit's [effective degrees of freedom](#effective-degrees-of-freedom) instead of $p$; the precise smoothing-software [variance](variance.md) convention should be specified.

## Residual-versus-fitted plot

↑ **Parent:** [Linear regression](linear-regression.md)

A [residual-versus-fitted plot](#residual-versus-fitted-plot) displays residuals vertically against predicted responses horizontally. Curvature suggests an incorrect conditional-mean model; a fan-shaped spread suggests [heteroscedasticity](statistical-modelling.md#heteroscedastic), while isolated large residuals may indicate unusual observations. It does not alone measure leverage or influence: [regression leverage](statistical-modelling.md#regression-leverage) records unusual predictor combinations, and [Cook's distance](statistical-modelling.md#cook-s-distance) combines leverage and residual size.

### Scale-location plot

↑ **Parent:** [Residual-versus-fitted plot](#residual-versus-fitted-plot)

A scale-location plot compares the square root of the absolute [standardized regression residual](probability-and-statistics.md#standardized-regression-residual) with the [fitted values](#fitted-values). Systematic changes in level or spread suggest [heteroscedasticity](statistical-modelling.md#heteroscedastic). It assesses the error scale, while a [residual-versus-fitted plot](#residual-versus-fitted-plot) primarily reveals mean patterns as well as changing spread.

## Analysis of variance

↑ **Parent:** [Linear regression](linear-regression.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Analysis_of_variance)

Analysis of variance decomposes variation into contributions associated with model terms and residual error. For nested [normal linear models](statistical-modelling.md#normal-linear-model), differences of residual sums of squares give sequential or partial [F-tests](probability-and-statistics.md#f-test).

### Multivariate analysis of variance

↑ **Parent:** [Analysis of variance](#analysis-of-variance)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multivariate_analysis_of_variance)

Multivariate analysis of variance compares mean vectors of several groups while accounting for correlations between their response variables. In the one-way normal model, independent observations $Y_{ri}\sim N_p(\mu_r,\Sigma)$ share a positive-definite [covariance matrix](variance.md#covariance-matrix). Put $E=\sum_{r,i}(Y_{ri}-\bar Y_r)(Y_{ri}-\bar Y_r)^T$ and $H=\sum_rn_r(\bar Y_r-\bar Y)(\bar Y_r-\bar Y)^T$. Under equal means, these matrices have independent [Wishart distributions](probability-theory.md#wishart-distribution) with degrees of freedom $N-g$ and $g-1$, respectively. This follows by separating the Gaussian data into orthogonal within-group and between-group projections. The [Wilks lambda statistic](#wilks-lambda-statistic) tests equality of the means using both matrices, rather than independently testing each coordinate.

#### Within-group and between-group scatter decomposition

↑ **Parent:** [Multivariate analysis of variance](#multivariate-analysis-of-variance)

For groups with sizes $n_r$, means $\bar x_r$, and overall mean $\bar x$, define $W=\sum_{r,i}(x_{ri}-\bar x_r)(x_{ri}-\bar x_r)^T$ and $B=\sum_r n_r(\bar x_r-\bar x)(\bar x_r-\bar x)^T$. Expanding $x_{ri}-\bar x=(x_{ri}-\bar x_r)+(\bar x_r-\bar x)$ gives total scatter $T=W+B$ because each within-group residual sum vanishes. Both matrices are [positive semidefinite](linear-algebra.md#positive-semidefinite-matrix), and $\operatorname{rank}B\leq\min(p,g-1)$. They separate within-group noise from between-group mean separation.

#### Wilks lambda statistic

↑ **Parent:** [Multivariate analysis of variance](#multivariate-analysis-of-variance)

For nonsingular within-group scatter $E$ and between-group scatter $H$, the statistic is $\prod_j(1+\theta_j)^{-1}$, where $\theta_j$ solve the [generalized eigenvalue problem](linear-operator-theory.md#generalized-eigenvalue-problem) $Hv=\theta Ev$. It is small when the group means differ strongly relative to within-group variation. Maximizing a common-covariance normal likelihood under equal and unrestricted means gives the likelihood ratio $\Lambda^{N/2}$. Its determinant factors cancel under any nonsingular change of response coordinates. For one response it is equivalent to the [analysis of variance](#analysis-of-variance) F-test.

### Two-way analysis of variance

↑ **Parent:** [Analysis of variance](#analysis-of-variance)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Two-way_analysis_of_variance)

An additive two-factor Gaussian model separates row and column effects. With one observation in each of $r c$ cells, constraints fixing one row and column effect leave $r+c-1$ mean parameters and $(r-1)(c-1)$ residual degrees of freedom. Balanced least squares gives fitted values equal to row mean plus column mean minus grand mean. With no cell replication, unrestricted interactions are confounded with residual error; the additive interpretation requires an assumption that those interactions are absent or negligible.

#### Missing cells can destroy factor orthogonality in two-way ANOVA

↑ **Parent:** [Two-way analysis of variance](#two-way-analysis-of-variance)

In a fully balanced crossed design, centered indicator columns for the two factors are orthogonal because each pair of levels occurs equally often. Missing cells can change the level-pair counts so that the displayed cross-product becomes nonzero. Then [sequential sums of squares](#sequential-sum-of-squares) depend on term order, although the final additive fit is unchanged. Testing either factor conditional on the other requires its [extra sum of squares](probability-and-statistics.md#extra-sum-of-squares) from the appropriate reduced model.

#### Identifiability of an incomplete two-factor additive design

↑ **Parent:** [Two-way analysis of variance](#two-way-analysis-of-variance)

For observed cells with means $a_i+b_j$, form a bipartite graph joining row $i$ to column $j$ when that cell is observed. If all levels occur, the design rank is $r+c-k$, where $k$ is the number of connected components. Indeed a coefficient perturbation in the kernel satisfies $a_i=-b_j$ on every observed edge, and hence has exactly one freely chosen constant on each component. A connected design has rank $r+c-1$ and is identifiable after a single reference constraint. Missing cells destroy the balanced-design orthogonality of row and column effects, so [sequential sums of squares](#sequential-sum-of-squares) can depend on order.

#### Saturation of an unreplicated two-factor regression

↑ **Parent:** [Two-way analysis of variance](#two-way-analysis-of-variance)

A [two-way analysis of variance](#two-way-analysis-of-variance) with the full [interaction](statistical-model.md#interaction-statistics) and one observation in each observed factor cell has one independently varying fitted cell mean per observation. A cell-indicator [design matrix](#design-matrix) has full row [matrix rank](vector-space.md#matrix-rank), even when some combinations are missing, so the model is a [saturated statistical model](statistical-modelling.md#saturated-statistical-model). Its [residual sum of squares](#residual-sum-of-squares) is zero and its [residual degrees of freedom](statistical-modelling.md#residual-degrees-of-freedom) are zero. Missing combinations make some coefficients nonidentifiable; they do not restore a pure-error estimate. Standard errors and an ordinary residual-based [F-test](probability-and-statistics.md#f-test) for interactions therefore cannot be recovered merely by fitting this larger model.

### Sequential sum of squares

↑ **Parent:** [Analysis of variance](#analysis-of-variance)

For an ordered sequence of nested [linear regression](linear-regression.md) models $M_0\subset M_1\subset\cdots$, the sequential sum of squares for the $j$th added term is $\operatorname{RSS}(M_{j-1})-\operatorname{RSS}(M_j)$. These are also called type-I sums of squares. They depend on term order when the design is not orthogonal. Dividing by the number of newly added coefficients and the full model's residual mean square gives the sequential [F-test](probability-and-statistics.md#f-test). A covariate added first is tested before adjustment for later terms, whereas a treatment added after the covariate is tested with that covariate already included.

### Sum of squares in ANOVA

↑ **Parent:** [Analysis of variance](#analysis-of-variance)

For an [orthogonal projection matrix](linear-algebra.md#orthogonal-projection-matrix) $P$, a [sum of squares in ANOVA](#sum-of-squares-in-anova) is $Y^TPY=\|PY\|^2$. Mutually orthogonal projections yield an additive decomposition of total squared response magnitude. Removing the grand mean gives the corrected total.

#### Mean square in ANOVA

↑ **Parent:** [Sum of squares in ANOVA](#sum-of-squares-in-anova)

A [mean square in ANOVA](#mean-square-in-anova) divides a [sum of squares in ANOVA](#sum-of-squares-in-anova) by its positive number $d$ of [statistical degrees of freedom](statistical-inference.md#statistical-degrees-of-freedom). If the corresponding residual subspace has scalar error [covariance](variance.md#covariance) $\lambda I$, its [expectation](probability-theory.md#expected-value) is $\lambda$. Its scale depends on whether raw observations or group means were projected.

### ANOVA stratum

↑ **Parent:** [Analysis of variance](#analysis-of-variance)

An [ANOVA stratum](#anova-stratum) is an [orthogonal](linear-algebra.md#orthogonal-vectors) response subspace representing one level of experimental variation, such as between blocks or within blocks. In a covariance model scalar on each such subspace, its [eigenvalue](linear-operator-theory.md#eigenvalue) supplies the common variance scale for its projected coordinates. Treatment and residual [sums of squares in ANOVA](#sum-of-squares-in-anova) must be compared within appropriate strata.

#### Within-block ANOVA stratum

↑ **Parent:** [ANOVA stratum](#anova-stratum)

The [within-block ANOVA stratum](#within-block-anova-stratum) contains response vectors whose coordinates sum to zero separately in every block. For $b$ blocks of size $k$ its dimension is $b(k-1)$. A shared additive block effect cancels in every vector in this subspace.

### Balanced factorial orthogonality

↑ **Parent:** [Analysis of variance](#analysis-of-variance)

In a complete two-factor design with equal cell replication, centred factor indicator columns for different factors have zero cross-products. Consequently the two main effects in an additive [normal linear model](statistical-modelling.md#normal-linear-model) are [orthogonal](linear-algebra.md#orthogonal-vectors), and their extra sums of squares do not depend on the order in which these main effects are entered. An omitted [interaction term](statistical-model.md#interaction-term) can still require a separate adequacy check.

<h2 id="frisch-waugh-lovell-theorem">Frisch–Waugh–Lovell theorem</h2>

↑ **Parent:** [Linear regression](linear-regression.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Frisch–Waugh–Lovell_theorem)

The Frisch–Waugh–Lovell theorem says that a regression coefficient can be obtained by residualizing both the response and its predictor against the remaining predictors and then regressing one residual on the other.

## Simple linear regression

↑ **Parent:** [Linear regression](linear-regression.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simple_linear_regression)

Simple linear regression uses one predictor and an intercept, $Y_i=\alpha+\beta x_i+\varepsilon_i$.

### Centred simple linear regression

↑ **Parent:** [Simple linear regression](#simple-linear-regression)

In [simple linear regression](#simple-linear-regression) written as $Y_i=\alpha+\beta(x_i-\bar x)+\varepsilon_i$, the constant and centred predictor columns are orthogonal. Differentiating the sum of squared residuals gives the displayed [ordinary least squares estimators](statistical-modelling.md#ordinary-least-squares-estimators), provided $S_{xx}=\sum_i(x_i-\bar x)^2>0$. For independent mean-zero errors of common variance $\sigma^2$, both estimators are unbiased, their variances are $\sigma^2/n$ and $\sigma^2/S_{xx}$, and their covariance is zero. The uncentred intercept is $\widehat\alpha-\widehat\beta\bar x$.

## Residual sum of squares

↑ **Parent:** [Linear regression](linear-regression.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Residual_sum_of_squares)

The residual sum of squares is

$$
\operatorname{RSS}=\sum_i(Y_i-\widehat Y_i)^2.
$$

## Ridge regression

↑ **Parent:** [Linear regression](linear-regression.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ridge_regression)

Ridge regression minimizes a squared-error loss plus the quadratic penalty $\lambda\lVert\beta\rVert_2^2$. Its positive penalty stabilizes inversion in collinear or high-dimensional designs.

### Gaussian posterior representation of ridge regression

↑ **Parent:** [Ridge regression](#ridge-regression)

For likelihood $Y\mid\beta\sim N(X\beta,\sigma^2I)$ and independent prior $\beta\sim N(0,\tau^2I)$, the [posterior distribution](statistical-inference.md#bayesian-posterior) is Gaussian with covariance $V$ as displayed and mean $(X^TX+\lambda I)^{-1}X^TY$. Its mean and mode therefore coincide with the [ridge regression](#ridge-regression) coefficient estimate. A Gaussian prior alone does not imply this conclusion without the stated likelihood.

// Target: foundations-of-mathematics.bigb

### Unbounded directional risk of fixed ridge shrinkage

↑ **Parent:** [Ridge regression](#ridge-regression)

For fixed positive [ridge regression](#ridge-regression) penalty, choose a unit [eigenvector](linear-operator-theory.md#eigenvector) $v$ of $X^{\mathsf T}X$ with eigenvalue $d>0$, and signal $\beta^0=Bv$. The directional ridge risk is $(\lambda^2B^2+\sigma^2d)/(d+\lambda)^2$, whereas [ordinary least squares](statistical-modelling.md#ordinary-least-squares) has risk $\sigma^2/d$. Letting $|B|$ grow makes the ridge squared bias arbitrarily large.

### Uniform directional risk improvement by ridge regression

↑ **Parent:** [Ridge regression](#ridge-regression)

For a full-rank centred design, unscaled [ridge regression](#ridge-regression) and zero-mean errors with covariance $\sigma^2I$, put $S=X^{\mathsf T}X$ and $A=(S+\lambda I)^{-1}$. The ordinary-least-squares risk matrix minus the ridge risk matrix is $\lambda A(2\sigma^2I+\lambda\sigma^2S^{-1}-\lambda\beta^0\beta^{0\mathsf T})A$. It is positive definite whenever $\lambda\|\beta^0\|_2^2<2\sigma^2$, including every positive $\lambda$ when $\beta^0=0$. Thus one signal-dependent small penalty improves every nonzero-direction [mean squared error](statistical-modelling.md#mean-squared-error).

### Unpenalized intercept in ridge regression

↑ **Parent:** [Ridge regression](#ridge-regression)

In [ridge regression](#ridge-regression), penalize slopes but ordinarily leave the [regression intercept](#regression-intercept) free. Centering gives $\widehat\beta=(X_c^TX_c+\lambda I)^{-1}X_c^TY_c$ and $\widehat\alpha=\overline Y-\overline x^T\widehat\beta$. An exactly centered predictor matrix has $\widehat\alpha=\overline Y$ for every penalty. A table with a penalty-dependent intercept therefore cannot arise from exactly centered columns under this convention.

### Covariance and bias of a ridge regression estimator

↑ **Parent:** [Ridge regression](#ridge-regression)

For a fixed centered [design matrix](#design-matrix) $X$, independent errors of [variance](variance.md) $\sigma^2$, and objective $\lVert Y-X\beta\rVert^2+a\lVert\beta\rVert^2$, put $G=X^TX$ and $M=G+aI$. The [ridge regression](#ridge-regression) estimator has

$$
\operatorname{Cov}(\widehat\beta)=\sigma^2M^{-1}GM^{-1},\qquad \mathbb E\widehat\beta-\beta=-aM^{-1}\beta.
$$

Thus its standard error alone does not justify centering a [confidence interval](statistical-inference.md#confidence-interval) for $\beta$ at the biased estimator. A penalty chosen from the responses also changes its [sampling distribution](statistical-modelling.md#sampling-distribution).

### Closed-form ridge regression estimator

↑ **Parent:** [Ridge regression](#ridge-regression)

For $\lambda>0$, the [ridge regression](#ridge-regression) objective $\lVert Y-X\beta\rVert_2^2+\lambda\lVert\beta\rVert_2^2$ has [gradient](calculus.md#gradient) $2(X^TX+\lambda I)\beta-2X^TY$. The matrix $X^TX+\lambda I$ is [positive definite](linear-algebra.md#positive-definite-matrix), so the unique minimizer is $\widehat\beta_\lambda=(X^TX+\lambda I)^{-1}X^TY$.

#### Vanishing-penalty ridge limit

↑ **Parent:** [Closed-form ridge regression estimator](#closed-form-ridge-regression-estimator)

In an eigenbasis of $G=X^TX$, [ridge regression](#ridge-regression) divides the corresponding component of $X^TY$ by $\gamma+\lambda$. If $\gamma=0$, its [eigenvector](linear-operator-theory.md#eigenvector) $v$ satisfies $Xv=0$, and hence $v^TX^TY=0$ exactly. Only positive [eigenvalues](linear-operator-theory.md#eigenvalue) contribute to the limit, giving the [Moore-Penrose inverse](linear-algebra.md#moore-penrose-inverse) expression for the [minimum-norm least-squares solution](inverse-problem.md#minimum-norm-least-squares-solution). No full-rank or sample-size assumption is needed.

#### Primal-dual identity for ridge regression

↑ **Parent:** [Closed-form ridge regression estimator](#closed-form-ridge-regression-estimator)

For any real [design matrix](#design-matrix) $X$ and $\lambda>0$, $(X^TX+\lambda I)^{-1}X^T=X^T(XX^T+\lambda I)^{-1}$. Multiplication by $X$ identifies the primal [ridge regression](#ridge-regression) fitted values with $K(K+\lambda I)^{-1}Y$, $K=XX^T$, the [kernel-ridge hat matrix](probability-and-statistics.md#kernel-ridge-hat-matrix) for the [linear kernel](probability-and-statistics.md#linear-kernel). No rank assumption is needed.

#### Principal-component shrinkage by ridge regression

↑ **Parent:** [Closed-form ridge regression estimator](#closed-form-ridge-regression-estimator)

For $X^TX=V\Lambda V^T$, [ridge regression](#ridge-regression) multiplies the fitted response along the $i$th [normalized sample principal component](statistical-learning.md#normalized-sample-principal-component) by the shrinkage factor $\Lambda_{ii}/(\Lambda_{ii}+\lambda)$. Directions with variance much larger than $\lambda$ are nearly retained, while directions with variance much smaller than $\lambda$ are nearly removed.

## Fitted values

↑ **Parent:** [Linear regression](linear-regression.md)

Fitted values are the responses predicted at the training covariates by a fitted regression model.

### Linear smoother

↑ **Parent:** [Fitted values](#fitted-values)

A linear smoother has fitted-value vector $\widehat Y=HY$, where the smoother matrix $H$ depends on the covariates and tuning parameters but not on the response vector.

#### Effective degrees of freedom

↑ **Parent:** [Linear smoother](#linear-smoother)

For a linear smoother $\widehat Y=HY$, its effective degrees of freedom are $\operatorname{tr}(H)$. This measures sensitivity of fitted values to responses even when $H$ is not an orthogonal projection.

## Design matrix

↑ **Parent:** [Linear regression](linear-regression.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Design_matrix)

The design matrix has one row for each observation and one column for each regression coefficient, so the linear predictor is $X\beta$.

### Confounding of nested fixed factors

↑ **Parent:** [Design matrix](#design-matrix)

If each level of one [categorical variable](statistical-modelling.md#categorical-variable) belongs to exactly one level of another, indicators for the coarser levels are sums of indicators for the finer levels. Including unrestricted fixed effects for both therefore gives a [rank-deficient ordinary least squares](statistical-modelling.md#rank-deficient-ordinary-least-squares): the separate effects lack [identifiability](statistical-model.md#identifiability) without additional constraints.

## Regression coefficient

↑ **Parent:** [Linear regression](linear-regression.md)

A regression coefficient is a component of $\beta$ measuring the change in the linear predictor associated with its design-matrix column.

These are the parameters of a [linear regression](linear-regression.md) predictor, rather than the regression procedure itself.

## Attenuation bias from classical measurement error

↑ **Parent:** [Linear regression](linear-regression.md)

If $Y=\beta Z+\varepsilon$ but the predictor is observed as $X=Z+\eta$, with independent centred errors, the population regression slope is

$$
\frac{\operatorname{Cov}(X,Y)}{\operatorname{Var}(X)}
=\beta\frac{\operatorname{Var}(Z)}
{\operatorname{Var}(Z)+\operatorname{Var}(\eta)}.
$$

Measurement error in the predictor therefore shrinks the slope toward zero, while independent response noise changes its uncertainty but not its population value.

## ↑ Ancestors (7)

1. [Normal linear model](statistical-modelling.md#normal-linear-model)
2. [Statistical modelling](statistical-modelling.md)
3. [Statistical model](statistical-model.md)
4. [Probability and statistics](probability-and-statistics.md)
5. [Area of mathematics](mathematics.md#area-of-mathematics)
6. [Mathematics](mathematics.md)
7. [Codex Wiki](README.md)

## ← Incoming links (40)

- [Approximate experimental design](statistical-modelling.md#approximate-experimental-design)
- [Efficiency (statistics)](statistical-inference.md#efficiency-statistics)
- [Estimability from within-block differences](statistical-modelling.md#estimability-from-within-block-differences)
- [Influential observation](#influential-observation)
- [Information matrix of an experimental design](statistical-modelling.md#information-matrix-of-an-experimental-design)
- [Interaction plot](statistical-model.md#interaction-plot)
- [Interaction (statistics)](statistical-model.md#interaction-statistics)
- [Mutually orthogonal Latin squares](statistical-modelling.md#mutually-orthogonal-latin-squares)
- [Observed heterogeneity](statistical-modelling.md#observed-heterogeneity)
- [Ordinary least squares estimators](statistical-modelling.md#ordinary-least-squares-estimators)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-1.md#13i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-46.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-41.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4.md#19c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-41.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4.md#5i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-4.md#5j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-32.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-33.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-41.md#1/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-41.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-32.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-32.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-33.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208.md#2/2/3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#5j/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4.md#28k/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-2.md#5j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-219.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4.md#13j/iv/solution)
- [Polynomial regression](#polynomial-regression)
- [Post-randomization adjustment changes a treatment estimand](causal-inference.md#post-randomization-adjustment-changes-a-treatment-estimand)
- [Predictor centering](#predictor-centering)
- [Reciprocal-predictor regression](#reciprocal-predictor-regression)
- [Regression analysis](statistical-modelling.md#regression-analysis)
- [Regression coefficient](#regression-coefficient)
- [Regression model](statistical-model.md#regression-model)
- [Residual estimate of Gaussian noise variance](statistical-modelling.md#residual-estimate-of-gaussian-noise-variance)
- [Sequential sum of squares](#sequential-sum-of-squares)
