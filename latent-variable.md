# Latent variable

↑ **Parent:** [Statistical modelling](statistical-modelling.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Latent_variable)

A latent variable is an unobserved random quantity introduced to describe dependence, hidden structure, or an indirect data-generating mechanism in a statistical model.

**Table of contents**

- [Unobserved heterogeneity](#unobserved-heterogeneity)
- [Factor analysis](#factor-analysis)
  - [Latent factor](#latent-factor)
  - [Orthogonal factor model](#orthogonal-factor-model)
    - [Factor rotation](#factor-rotation)
      - [Varimax rotation](#varimax-rotation)
    - [Communality](#communality)
    - [Factor loading](#factor-loading)
  - [EM update for a single-factor Gaussian model](#em-update-for-a-single-factor-gaussian-model)
- [Random effect](#random-effect)
  - [Poisson-lognormal random-effect model](#poisson-lognormal-random-effect-model)
  - [Crossed random effects](#crossed-random-effects)
  - [Random slope](#random-slope)
    - [Between-person slope quantile](#between-person-slope-quantile)
    - [Random-slope linear mixed model](#random-slope-linear-mixed-model)
- [Expectation-maximization algorithm](#expectation-maximization-algorithm)
  - [EM expectation step](#em-expectation-step)
  - [EM maximization step](#em-maximization-step)
  - [Known-variance Gaussian mixture EM example](#known-variance-gaussian-mixture-em-example)
    - [Identical-mean EM trap](#identical-mean-em-trap)
  - [Ordered-rate exponential M-step](#ordered-rate-exponential-m-step)
  - [EM for merged multinomial cells](#em-for-merged-multinomial-cells)
  - [EM for an independent missing normal coordinate](#em-for-an-independent-missing-normal-coordinate)
  - [EM transition-count update on a tree](#em-transition-count-update-on-a-tree)
  - [EM for a missing observation in a Gaussian AR1 process](#em-for-a-missing-observation-in-a-gaussian-ar1-process)
  - [EM likelihood monotonicity](#em-likelihood-monotonicity)

## Unobserved heterogeneity

↑ **Parent:** [Latent variable](latent-variable.md)

Persistent unmeasured differences between individuals can generate outcome dependence after adjusting for observed [covariates](statistical-model.md#covariate). A [random intercept](generalized-linear-model.md#random-intercept) is one representation. Conditional independence given that [latent variable](latent-variable.md) need not persist after it is integrated out; apparent history dependence can therefore occur without [true state dependence](generalized-linear-model.md#true-state-dependence).

## Factor analysis

↑ **Parent:** [Latent variable](latent-variable.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Factor_analysis)

Factor analysis writes an observation as $Y=\Lambda Z+\xi$, where the low-dimensional [latent variable](latent-variable.md) $Z$ describes shared variation. In the isotropic Gaussian model $Z\sim N(0,I)$ and $\xi\sim N(0,\sigma^2I)$ independently, the observation has covariance $\Lambda\Lambda^T+\sigma^2I$.

### Latent factor

↑ **Parent:** [Factor analysis](#factor-analysis)

A [latent factor](#latent-factor) is an unobserved coordinate introduced to explain shared variation among measurements. In an [orthogonal factor model](#orthogonal-factor-model), [latent factors](#latent-factor) have [variance](variance.md) one and are mutually uncorrelated, with coefficients specified by the [factor loadings](#factor-loading). They differ from a [regression factor](statistical-modelling.md#regression-factor), which is a categorical predictor. A fitted [covariance](variance.md#covariance) alone generally leaves the [latent factor](#latent-factor) orientation undetermined; [factor rotation](#factor-rotation) gives equivalent representations.

### Orthogonal factor model

↑ **Parent:** [Factor analysis](#factor-analysis)

The latent factor vector has mean zero and covariance $I_q$, the specific errors have mean zero and diagonal covariance $\Psi$, and the two are uncorrelated. Thus the off-diagonal covariance is explained by shared factors. Normality additionally gives a likelihood model, but the covariance identity needs only these second-moment assumptions. Positive diagonal entries of $\Psi$ describe variation not explained by the factors. Unlike [principal component analysis](statistical-learning.md#principal-component-analysis), the model separates shared and specific variation rather than only maximizing total projected variance.

#### Factor rotation

↑ **Parent:** [Orthogonal factor model](#orthogonal-factor-model)

An orthogonal rotation of factors leaves $LL^T$ unchanged and hence preserves the model covariance. It proves rotational nonidentifiability of the unrestrained [factor loadings](#factor-loading). Choose an orientation for interpretability, for example [varimax rotation](#varimax-rotation), or impose identifying restrictions in a confirmatory model. An oblique transformation permits correlated factors: if $L$ becomes $LH$, their covariance becomes $H^{-1}H^{-T}$, preserving the same shared covariance.

##### Varimax rotation

↑ **Parent:** [Factor rotation](#factor-rotation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Varimax_rotation)

An orthogonal factor rotation maximizing, over factor axes, the variance across variables of their squared loadings. It seeks an interpretable pattern with some large and many small loadings on each factor without changing the covariance fit.

#### Communality

↑ **Parent:** [Orthogonal factor model](#orthogonal-factor-model)

The communality is the variance of the shared-factor contribution to variable $i$. In an [orthogonal factor model](#orthogonal-factor-model), $\operatorname{Var}(X_i)=h_i^2+\psi_i$, where $\psi_i$ is its specific variance. For standardized variables, $h_i^2\leq1$. It measures variance shared through the modeled factors, not variance in a chosen [principal component](statistical-learning.md#principal-component).

#### Factor loading

↑ **Parent:** [Orthogonal factor model](#orthogonal-factor-model)

A factor loading is the coefficient of latent factor $F_j$ in observed variable $X_i$. In the [orthogonal factor model](#orthogonal-factor-model), $\operatorname{Cov}(X_i,F_j)=L_{ij}$. If $X_i$ has variance one, this is also its correlation with the variance-one factor. Its sign and size depend on the factor-coordinate convention; [factor rotation](#factor-rotation) preserves the implied covariance while changing individual loadings.

### EM update for a single-factor Gaussian model

↑ **Parent:** [Factor analysis](#factor-analysis)

In [factor analysis](#factor-analysis) with one factor and fixed noise variance $v>0$, let $\lambda$ be the current loading vector, $s=v+|\lambda|^2$, and $S=n^{-1}\sum_iY_iY_i^T$. The [expectation-maximization algorithm](#expectation-maximization-algorithm) update is

$$
\lambda_{\mathrm{new}}=\frac{sS\lambda}{vs+\lambda^TS\lambda}.
$$

The conditional factor means are $\lambda^TY_i/s$ and their variances are $v/s$; maximizing the expected complete-data log-likelihood gives the formula.

## Random effect

↑ **Parent:** [Latent variable](latent-variable.md)

A random effect is a [latent variable](latent-variable.md) used to describe variation between observational units or dependence among related observations. Its distribution supplements the fixed effects used in [statistical modelling](statistical-modelling.md). Independent random effects produce extra variability; correlated random effects can produce serial dependence.

### Poisson-lognormal random-effect model

↑ **Parent:** [Random effect](#random-effect)

Let $Y\mid\Lambda\sim\operatorname{Poisson}(e^{\eta+\Lambda})$, with $\Lambda\sim N(0,\tau^2)$. The [lognormal distribution](probability-distribution.md#log-normal-distribution) of the random mean gives marginal mean $m=e^{\eta+\tau^2/2}$. The [law of total variance](probability-theory.md#law-of-total-variance) gives $\operatorname{Var}(Y)=m+m^2(e^{\tau^2}-1)$, strictly larger than $m$ when $\tau>0$. Thus independent observation-level [random effects](#random-effect) produce [overdispersion](exponential-family.md#overdispersion) even though the conditional [Poisson distributions](discrete-probability-distribution.md#poisson-distribution) have variance equal to their means.

### Crossed random effects

↑ **Parent:** [Random effect](#random-effect)

Random effects are crossed when an observation can belong to levels of two grouping factors without one grouping factor being nested within the other. Independent location intercepts and incubator slopes, for example, contribute separate terms to the observation [covariance matrix](variance.md#covariance-matrix).

### Random slope

↑ **Parent:** [Random effect](#random-effect)

A [random slope](#random-slope) multiplies a predictor by a group-specific latent coefficient. With $b_j\sim N(0,\tau^2)$, a contribution $b_jt_i$ induces [covariance](variance.md#covariance) $\tau^2t_it_k$ for two observations in group $j$. A [random slope](#random-slope) does not necessarily include a [random intercept](generalized-linear-model.md#random-intercept).

#### Between-person slope quantile

↑ **Parent:** [Random slope](#random-slope)

When a person's latent slope has [normal distribution](probability-distribution.md#normal-distribution) $N(\beta_1,\tau_1^2)$, its $u$th [quantile](probability-distribution.md#quantile-function) is $\beta_1+\tau_1\Phi^{-1}(u)$. Multiply by an elapsed time to obtain the corresponding latent change [quantile](probability-distribution.md#quantile-function). This describes population variation between people; it is distinct from a [confidence interval](statistical-inference.md#confidence-interval) for the mean slope and from a [prediction interval](statistical-inference.md#prediction-interval) that includes measurement error.

#### Random-slope linear mixed model

↑ **Parent:** [Random slope](#random-slope)

The Gaussian model $Y=X\beta+Zb+\varepsilon$ with $b\sim N(0,D)$ and independent $\varepsilon\sim N(0,\sigma^2I)$ has marginal law $N(X\beta,ZDZ^T+\sigma^2I)$. Its group coefficients are integrated out of the marginal [likelihood function](maximum-likelihood-estimation.md#likelihood-function). The special random-slope model uses predictor values in the grouping columns of $Z$.

## Expectation-maximization algorithm

↑ **Parent:** [Latent variable](latent-variable.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Expectation-maximization_algorithm)

The [expectation-maximization algorithm](#expectation-maximization-algorithm) fits a [latent-variable model](statistical-modelling.md#latent-variable-model) by alternating a [conditional expectation](measure-theory.md#conditional-expectation) over the [latent variables](latent-variable.md) with a maximization over the [statistical parameters](statistical-model.md#statistical-parameter). Its target is the observed-data [likelihood function](maximum-likelihood-estimation.md#likelihood-function), although its updates use the simpler complete-data [log-likelihood](maximum-likelihood-estimation.md#log-likelihood).[Section 2, printed p. 6, equation (2.17) and the general E-step/M-step definition](mathematics-bibliography.md#maximum-likelihood-from-incomplete-data-via-the-em-algorithm-by-arthur-pentland-dempster-and-others)

Write $y$ for the observations, $z$ for the [latent variables](latent-variable.md), and $p_\theta(y,z)$ for their joint [probability density function](continuous-probability-distribution.md#probability-density-function) or [probability mass function](probability-distribution.md#probability-mass-function). The observed-data [log-likelihood](maximum-likelihood-estimation.md#log-likelihood) is

$$
\ell(\theta)=\log p_\theta(y),\qquad p_\theta(y)=\int p_\theta(y,z)\,dz,
$$

where the [integral](integral.md) becomes a sum for discrete $z$. Directly maximizing a [logarithm](calculus.md#logarithm) of this sum can be awkward. The [E-step](#em-expectation-step) instead computes a [conditional distribution](probability-theory.md#conditional-distribution) at the current [statistical parameters](statistical-model.md#statistical-parameter) $\theta^{(t)}$; the [M-step](#em-maximization-step) uses it to construct a new fit. The attractive idea is to retain uncertainty about the hidden labels while recovering simple [weighted means](arithmetic.md#weighted-arithmetic-mean) and other complete-data updates. The [Known-variance Gaussian mixture EM example](#known-variance-gaussian-mixture-em-example) shows the mechanism without estimating a [variance](variance.md) or [mixture weight](statistical-modelling.md#mixture-weight).

[Arthur Pentland Dempster](probability-and-statistics.md#arthur-pentland-dempster), [Nan M. Laird](probability-and-statistics.md#nan-m-laird), and [Donald B. Rubin](probability-and-statistics.md#donald-b-rubin) gave the general framework its name in their 1977 paper, which also discusses earlier special-case algorithms.[Section 1, printed pp. 1 and 3: naming of the two steps and earlier special cases](mathematics-bibliography.md#maximum-likelihood-from-incomplete-data-via-the-em-algorithm-by-arthur-pentland-dempster-and-others)

### EM expectation step

↑ **Parent:** [Expectation-maximization algorithm](#expectation-maximization-algorithm)

Hold the old [statistical parameters](statistical-model.md#statistical-parameter) fixed when taking the [conditional expectation](measure-theory.md#conditional-expectation), while keeping the candidate [statistical parameters](statistical-model.md#statistical-parameter) $\theta$ variable:

$$
q_t(z)=p_{\theta^{(t)}}(z\mid y),\qquad Q(\theta\mid\theta^{(t)})=\mathbb E_{q_t}[\log p_\theta(y,Z)].
$$

For [independent](random-variable.md#independent-random-variables) observations in a [finite mixture model](statistical-modelling.md#finite-mixture-model), $Z_i$ is a hidden component label. [Bayes' theorem](probability-theory.md#bayes-theorem) gives its [mixture responsibilities](statistical-modelling.md#mixture-responsibility):

$$
r_{ij}^{(t)}=\mathbb P_{\theta^{(t)}}(Z_i=j\mid Y_i=y_i)=\frac{\pi_j^{(t)}f_j(y_i;\theta^{(t)})}{\sum_k\pi_k^{(t)}f_k(y_i;\theta^{(t)})},\qquad \sum_jr_{ij}^{(t)}=1.
$$

These [posterior probabilities](bayesian-statistics.md#posterior-probability) are the [conditional expectations](measure-theory.md#conditional-expectation) of the [mixture allocation indicators](statistical-modelling.md#mixture-allocation-indicator); they turn hidden counts into fractional counts.[Section 4.3, printed pp. 15-16, especially the paragraph following equation (4.3.3): conditional indicator probabilities and weighted counts](mathematics-bibliography.md#maximum-likelihood-from-incomplete-data-via-the-em-algorithm-by-arthur-pentland-dempster-and-others) They condition on a current fixed fit, rather than averaging over a [posterior distribution](bayesian-statistics.md#bayesian-posterior) of the [statistical parameters](statistical-model.md#statistical-parameter). Taking the [conditional expectation](measure-theory.md#conditional-expectation) of the complete-data [log-likelihood](maximum-likelihood-estimation.md#log-likelihood) is essential: substituting a single guessed label, or merely substituting the [conditional mean](measure-theory.md#conditional-expectation) into a nonlinear complete-data expression, generally gives a different algorithm.

### EM maximization step

↑ **Parent:** [Expectation-maximization algorithm](#expectation-maximization-algorithm)

Maximize $Q(\theta\mid\theta^{(t)})$ over the permitted [statistical parameters](statistical-model.md#statistical-parameter), with the [E-step](#em-expectation-step) [conditional distribution](probability-theory.md#conditional-distribution) held fixed.[Section 2, printed p. 6: general maximization step](mathematics-bibliography.md#maximum-likelihood-from-incomplete-data-via-the-em-algorithm-by-arthur-pentland-dempster-and-others) A [finite mixture model](statistical-modelling.md#finite-mixture-model) has

$$
Q(\theta\mid\theta^{(t)})=\sum_{i,j}r_{ij}^{(t)}\bigl(\log\pi_j+\log f_j(y_i;\theta)\bigr).
$$

For [normal distributions](probability-distribution.md#normal-distribution) with known common [variance](variance.md) $\sigma^2>0$ and fixed positive [mixture weights](statistical-modelling.md#mixture-weight), only the [means](expected-value.md) are fitted. Dropping terms independent of these candidate [means](expected-value.md) gives

$$
Q(\mu\mid\theta^{(t)})=C-\frac{1}{2\sigma^2}\sum_{i,j}r_{ij}^{(t)}(y_i-\mu_j)^2,\qquad N_j^{(t)}=\sum_ir_{ij}^{(t)},\qquad \mu_j^{(t+1)}=\frac{\sum_ir_{ij}^{(t)}y_i}{N_j^{(t)}}.
$$

The [derivative](calculus.md#derivative) in $\mu_j$ is $\sum_ir_{ij}^{(t)}(y_i-\mu_j)/\sigma^2$, and its second [derivative](calculus.md#derivative) is $-N_j^{(t)}/\sigma^2$. Thus a positive weighted count gives a unique maximizing [weighted mean](arithmetic.md#weighted-arithmetic-mean). This is a maximization of the surrogate $Q$; the observed-data [log-likelihood](maximum-likelihood-estimation.md#log-likelihood) need not be [concave](real-analysis.md#concave-function). Recompute the [mixture responsibilities](statistical-modelling.md#mixture-responsibility) after updating the [means](expected-value.md). The broader [EM for Gaussian mixtures with a common variance](statistical-modelling.md#em-for-gaussian-mixtures-with-a-common-variance) also estimates [mixture weights](statistical-modelling.md#mixture-weight) and the shared [variance](variance.md).

### Known-variance Gaussian mixture EM example

↑ **Parent:** [Expectation-maximization algorithm](#expectation-maximization-algorithm)

Choose six illustrative values $y=(-2.2,-1.8,-1,1,1.8,2.2)$, fixed [mixture weights](statistical-modelling.md#mixture-weight) $\pi_1=\pi_2=1/2$, known [standard deviation](variance.md#standard-deviation) $\sigma=1$, and initial [means](expected-value.md) $(\mu_1^{(0)},\mu_2^{(0)})=(-1,1)$. These are constructed data for a [Gaussian mixture distribution](probability-distribution.md#gaussian-mixture-distribution), not measurements. With $\phi$ the [standard normal distribution](probability-distribution.md#standard-normal-distribution) [probability density function](continuous-probability-distribution.md#probability-density-function), the fitted [log-likelihood](maximum-likelihood-estimation.md#log-likelihood) is

$$
\ell(\mu_1,\mu_2)=\sum_{i=1}^6\log\left(\frac{\phi(y_i-\mu_1)+\phi(y_i-\mu_2)}{2}\right).
$$

At the initial [means](expected-value.md), the component density ratio is $\phi(y_i-1)/\phi(y_i+1)=e^{2y_i}$. The first [E-step](#em-expectation-step) therefore gives

$$
r_{i2}^{(0)}=\frac{1}{1+e^{-2y_i}},\qquad r_{i1}^{(0)}=1-r_{i2}^{(0)},\qquad (r_{12}^{(0)},\ldots,r_{62}^{(0)})\approx(0.012128,0.026597,0.119203,0.880797,0.973403,0.987872).
$$

<a id="image-the-first-e-step-retains-two-soft-label-probabilities-at-each-chosen-data-point"></a>
![](expectation-maximization-soft-data-weights.png)

**[Figure 1](#image-the-first-e-step-retains-two-soft-label-probabilities-at-each-chosen-data-point). The first E-step retains two soft label probabilities at each chosen data point**. Initial means are minus one and one, mixture weights are one half, and the known standard deviation is one. Stacked bars show the two conditional label probabilities; every row sums to one. Small but nonzero probabilities remain visible in the numerical labels.

The paired values $y$ and $-y$ have complementary [mixture responsibilities](statistical-modelling.md#mixture-responsibility), so $N_1^{(0)}=N_2^{(0)}=3$ exactly. The first [M-step](#em-maximization-step) gives

$$
\mu_2^{(1)}=\frac{2.2\tanh(2.2)+1.8\tanh(1.8)+\tanh(1)}{3}\approx1.537493288,\qquad \mu_1^{(1)}=-\mu_2^{(1)}.
$$

The [hyperbolic tangent](calculus.md#hyperbolic-tangent) expression follows by pairing the contributions at $y$ and $-y$. Assigning every negative value wholly to the first [mixture component](statistical-modelling.md#mixture-component) and every positive value wholly to the second would instead give [means](expected-value.md) $\pm5/3$. Those hard assignments discard the overlap: the [expectation-maximization algorithm](#expectation-maximization-algorithm) is not the same update as [K-means clustering](statistical-learning.md#k-means-clustering).

The observed-data [log-likelihood](maximum-likelihood-estimation.md#log-likelihood) rises from $-11.420338905$ initially to $-10.368745063$ after one update and $-10.340655142$ after two. Further updates approach [means](expected-value.md) $\pm1.638023833$, with [log-likelihood](maximum-likelihood-estimation.md#log-likelihood) approximately $-10.340509617$. These values describe this initialization; [EM likelihood monotonicity](#em-likelihood-monotonicity) supplies no certificate of a global maximum.

<a id="image-likelihood-ascent-and-mean-updates-for-the-chosen-data-compared-with-an-identical-means-initialization"></a>
![](expectation-maximization-likelihood-mean-iterations.png)

**[Figure 2](#image-likelihood-ascent-and-mean-updates-for-the-chosen-data-compared-with-an-identical-means-initialization). Likelihood ascent and mean updates for the chosen data, compared with an identical-means initialization**. Iteration zero is the initial fit; each subsequent point follows one E-step and one M-step. Starting at minus one and one increases the likelihood. Starting both means at zero leaves them at zero with a lower constant likelihood. All runs keep variance one and weights one half.

For stable numerical evaluation, put $a_{ij}=\log(1/2)-\tfrac12\log(2\pi)-\tfrac12(y_i-\mu_j)^2$ and $b_i=\max_j a_{ij}$. The [log-sum-exp function](convex-optimization.md#log-sum-exp-function) gives

$$
\log p_\mu(y_i)=b_i+\log\sum_j e^{a_{ij}-b_i},\qquad r_{ij}=e^{a_{ij}-\log p_\mu(y_i)}.
$$

Subtracting $b_i$ keeps at least one exponential equal to one, avoiding the all-zero sum that direct evaluation of tiny component densities can produce.

#### Identical-mean EM trap

↑ **Parent:** [Known-variance Gaussian mixture EM example](#known-variance-gaussian-mixture-em-example)

In the [Known-variance Gaussian mixture EM example](#known-variance-gaussian-mixture-em-example), initialize both [means](expected-value.md) at the same value $m$. The [mixture responsibilities](statistical-modelling.md#mixture-responsibility) are then $1/2$ for every observation. Each [M-step](#em-maximization-step) sets both [means](expected-value.md) to the sample [mean](expected-value.md), zero here; the next [E-step](#em-expectation-step) again gives $1/2$. Thus $(0,0)$ is a [fixed point](function.md#fixed-point) with [log-likelihood](maximum-likelihood-estimation.md#log-likelihood) $-14.593631199$, despite the better fit found from $(-1,1)$.

One can check the failure without trusting an iteration plot. Separate the [means](expected-value.md) as $(-a,a)$ and use the [hyperbolic cosine](calculus.md#hyperbolic-cosine) identity:

$$
\ell(-a,a)-\ell(0,0)=-3a^2+\sum_{i=1}^6\log\cosh(ay_i)=\frac{\sum_iy_i^2-6}{2}a^2+O(a^4)=6.08a^2+O(a^4).
$$

The [Taylor expansion](calculus.md#taylor-expansion) uses $\sum_iy_i^2=18.16$. Small nonzero separation therefore improves the [log-likelihood](maximum-likelihood-estimation.md#log-likelihood), whereas translating both [means](expected-value.md) to $m$ changes it by $-3m^2$. This [stationary point](calculus-of-variations.md#stationary-point) has both improving and worsening directions. Identical initialization cannot discover the separation because every observation keeps identical label probabilities. Trying several distinct initial fits and comparing their final [log-likelihoods](maximum-likelihood-estimation.md#log-likelihood) is useful, but does not prove global optimality.

Keeping the [variance](variance.md) fixed also removes a different pathology. With known $\sigma=1$, every component [probability density function](continuous-probability-distribution.md#probability-density-function) is at most $(2\pi)^{-1/2}$, so $\ell\leq-3\log(2\pi)$. If separate component [variances](variance.md) are allowed to shrink without restriction, one [mixture component](statistical-modelling.md#mixture-component) can concentrate at an observation while another retains positive density at the other observations, making the [likelihood function](maximum-likelihood-estimation.md#likelihood-function) unbounded. The fixed positive [variance](variance.md) in this example prevents that collapse; it does not remove initialization traps.

### Ordered-rate exponential M-step

↑ **Parent:** [Expectation-maximization algorithm](#expectation-maximization-algorithm)

For $N$ observations from each of two labeled [exponential distributions](continuous-probability-distribution.md#exponential-distribution), an E-step may produce positive completed time totals $U,V$. Its expected complete-data [log-likelihood](maximum-likelihood-estimation.md#log-likelihood) is $Q=N\log\lambda_1+N\log\lambda_2-U\lambda_1-V\lambda_2$. This is strictly [concave](real-analysis.md#concave-function). On the closed ordering constraint $\lambda_1\geq\lambda_2>0$, its maximum is $(N/U,N/V)$ when $U<V$; otherwise it lies at $\lambda_1=\lambda_2=2N/(U+V)$. To see the boundary case, first maximize along the equality line. At that maximum, moving into either feasible rate-separating direction has directional [derivative](calculus.md#derivative) $(V-U)/2\leq0$, so [concavity](real-analysis.md#concave-function) proves global optimality. For the open constraint $\lambda_1>\lambda_2$, this boundary value is a supremum rather than an attained M-step.

// Target: probability-and-statistics.bigb

### EM for merged multinomial cells

↑ **Parent:** [Expectation-maximization algorithm](#expectation-maximization-algorithm)

For a [multinomial distribution](discrete-probability-distribution.md#multinomial-distribution) with two unobserved cells merged into one observed count, the conditional allocation is a [binomial distribution](discrete-probability-distribution.md#binomial-distribution) with probabilities proportional to the two cell probabilities. The [expectation-maximization algorithm](#expectation-maximization-algorithm) replaces the missing counts by their conditional [expectations](expected-value.md) in the parameter-dependent part of the complete-data [log-likelihood](maximum-likelihood-estimation.md#log-likelihood). The [expectation](expected-value.md) of a log-factorial normalization generally differs from its value at the expected count, but this difference is independent of the candidate parameter and does not affect the maximization step.

### EM for an independent missing normal coordinate

↑ **Parent:** [Expectation-maximization algorithm](#expectation-maximization-algorithm)

For independent normal coordinates, an unobserved first coordinate has conditional law equal to its current marginal [normal distribution](probability-distribution.md#normal-distribution), even when the second coordinate of that observation is known. Thus its E-step first moment is $\mu_1^{(t)}$ and second moment is $(\mu_1^{(t)})^2+v_1^{(t)}$. With three observed first coordinates and one missing value, the mean update is $(\sum_{i=1}^3x_{i1}+\mu_1^{(t)})/4$ and the [variance](variance.md) update is $[\sum_{i=1}^3(x_{i1}-\mu_1^{(t+1)})^2+v_1^{(t)}+(\mu_1^{(t)}-\mu_1^{(t+1)})^2]/4$. The [conditional variance](variance.md#conditional-variance) term is essential: filling in only the conditional mean is not the [expectation-maximization algorithm](#expectation-maximization-algorithm).

### EM transition-count update on a tree

↑ **Parent:** [Expectation-maximization algorithm](#expectation-maximization-algorithm)

For a common unconstrained [Markov kernel](markov-chain.md#markov-kernel) on the edges of a rooted [tree](tree-graph-theory.md), let $N_{ab}$ be the [conditional expectation](measure-theory.md#conditional-expectation) of the number of transitions $a\to b$, given observed leaves and the old [Markov kernel](markov-chain.md#markov-kernel). The [expectation-maximization algorithm](#expectation-maximization-algorithm) maximizes $\sum_{a,b}N_{ab}\log K_{ab}$ over row [probability distributions](probability-distribution.md), giving $K_{ab}^{\mathrm{new}}=N_{ab}/\sum_cN_{ac}$. A row with zero total count is unrestricted by this objective. [Belief propagation](statistical-model.md#belief-propagation) computes the counts exactly on a [tree](tree-graph-theory.md).

### EM for a missing observation in a Gaussian AR1 process

↑ **Parent:** [Expectation-maximization algorithm](#expectation-maximization-algorithm)

In the [expectation-maximization algorithm](#expectation-maximization-algorithm) for a stationary [autoregressive process of order one](time-series.md#autoregressive-process-of-order-one), a single missing interior value has a [normal distribution](probability-distribution.md#normal-distribution) conditional on its neighbors. The E-step uses both its conditional mean and its conditional second moment, not just mean imputation. The M-step maximizes the expected stationary complete-data [log-likelihood](maximum-likelihood-estimation.md#log-likelihood), including the initial-observation density and the conditional-variance contribution to the two adjacent innovation squares.

### EM likelihood monotonicity

↑ **Parent:** [Expectation-maximization algorithm](#expectation-maximization-algorithm)

For $Q(\theta\mid\theta_0)=\mathbb E_{\theta_0}[\log p_\theta(Y,Z)\mid Y]$, the [Jensen inequality](real-analysis.md#jensen-s-inequality) gives

$$
\log p_\theta(Y)-\log p_{\theta_0}(Y)\geq Q(\theta\mid\theta_0)-Q(\theta_0\mid\theta_0).
$$

Thus any [expectation-maximization algorithm](#expectation-maximization-algorithm) [M-step](#em-maximization-step) that increases $Q$ cannot decrease the observed-data [likelihood function](maximum-likelihood-estimation.md#likelihood-function).[Section 3, printed pp. 6-7, Lemma 1 and Theorem 1, especially equation (3.10)](mathematics-bibliography.md#maximum-likelihood-from-incomplete-data-via-the-em-algorithm-by-arthur-pentland-dempster-and-others)

For a short proof, assume common support and finite expressions, and keep the [E-step](#em-expectation-step) [conditional distribution](probability-theory.md#conditional-distribution) $q_t(z)=p_{\theta^{(t)}}(z\mid y)$ fixed. The [concavity](real-analysis.md#concave-function) of the [logarithm](calculus.md#logarithm) and [Jensen's inequality](real-analysis.md#jensen-s-inequality) give

$$
\ell(\theta)=\log\mathbb E_{q_t}\left[\frac{p_\theta(y,Z)}{q_t(Z)}\right]\geq\mathbb E_{q_t}[\log p_\theta(y,Z)-\log q_t(Z)]=F(q_t,\theta).
$$

This [evidence lower bound](bayesian-statistics.md#evidence-lower-bound) equals $Q(\theta\mid\theta^{(t)})-\mathbb E_{q_t}\log q_t(Z)$. At $\theta=\theta^{(t)}$, the ratio inside the [expectation](expected-value.md) is the constant $p_{\theta^{(t)}}(y)$, so equality holds. During the [M-step](#em-maximization-step), the second term is constant; increasing $Q$ raises a lower bound that touches the current [log-likelihood](maximum-likelihood-estimation.md#log-likelihood). Hence

$$
\ell(\theta^{(t+1)})\geq F(q_t,\theta^{(t+1)})\geq F(q_t,\theta^{(t)})=\ell(\theta^{(t)}).
$$

Increasing [likelihood](maximum-likelihood-estimation.md#likelihood-function) values alone do not establish convergence of the [statistical parameters](statistical-model.md#statistical-parameter) or attainment of a global maximum. In a differentiable finite [mixture model](statistical-modelling.md#mixture-model), the [gradient](multivariable-calculus.md#gradient) of $\ell$ equals the candidate-parameter [gradient](multivariable-calculus.md#gradient) of $Q$ evaluated at the current fit. Thus an interior [fixed point](function.md#fixed-point) of an exact [M-step](#em-maximization-step) is a [stationary point](calculus-of-variations.md#stationary-point), which need not be a [local maximum](analysis.md#local-maximum); the [Identical-mean EM trap](#identical-mean-em-trap) is an explicit counterexample. Small changes in [log-likelihood](maximum-likelihood-estimation.md#log-likelihood) can also occur before the [means](expected-value.md) have settled, so inspecting both is useful.

## ↑ Ancestors (6)

1. [Statistical modelling](statistical-modelling.md)
2. [Statistical model](statistical-model.md)
3. [Probability and statistics](probability-and-statistics.md)
4. [Area of mathematics](mathematics.md#area-of-mathematics)
5. [Mathematics](mathematics.md)
6. [Codex Wiki](README.md)

## ← Incoming links (37)

- [Bühlmann–Straub model](actuarial-statistics.md#buhlmann-straub-model)
- [Conditional independence](random-variable.md#conditional-independence)
- [Covariance induced by a shared latent variable](random-variable.md#covariance-induced-by-a-shared-latent-variable)
- [Data augmentation](bayesian-statistics.md#data-augmentation)
- [Expectation-maximization algorithm](#expectation-maximization-algorithm)
- [Factor analysis](#factor-analysis)
- [Gaussian process classification](gaussian-process.md#gaussian-process-classification)
- [Hierarchical Bayesian model](bayesian-statistics.md#hierarchical-bayesian-model)
- [Law of total covariance](variance.md#law-of-total-covariance)
- [Mixture allocation indicator](statistical-modelling.md#mixture-allocation-indicator)
- [Mixture model](statistical-modelling.md#mixture-model)
- [Non-centered Gaussian random-effect parameterization](bayesian-statistics.md#non-centered-gaussian-random-effect-parameterization)
- [Observed and latent mixture labels](statistical-modelling.md#observed-and-latent-mixture-labels)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40.md#4/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-41.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48.md#6/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-44.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-44.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-36.md#4/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30.md#5/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35.md#2/e/2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35.md#2/h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-216.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-219.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2.md#5j/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-219.md#3/b/solution)
- [Phylogenetic tree](biology.md#phylogenetic-tree)
- [Random effect](#random-effect)
- [Repeated-measurement latent signal model](probability-and-statistics.md#repeated-measurement-latent-signal-model)
- [Selection on an extreme first measurement](probability-and-statistics.md#selection-on-an-extreme-first-measurement)
- [Unobserved heterogeneity](#unobserved-heterogeneity)
- [WinBUGS](bayesian-statistics.md#winbugs)
