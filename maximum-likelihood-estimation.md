# Maximum likelihood estimation

↑ **Parent:** [Statistical modelling](statistical-modelling.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Maximum_likelihood_estimation)

[Maximum likelihood estimation](maximum-likelihood-estimation.md) is a method of [statistical estimation](statistical-inference.md#statistical-estimation): within a specified [statistical model](statistical-model.md), choose the [statistical parameter](statistical-model.md#statistical-parameter) values that maximize the [likelihood function](#likelihood-function) of the observed data. For a parameter set $\Theta$ and observations $x$, its exact requirement is

$$
\widehat\theta(x)\in\Theta,\qquad L(\widehat\theta(x);x)=\sup_{\theta\in\Theta}L(\theta;x).
$$

The equality requires an attained, finite [maximum](set.md#maximum-of-a-subset-of-a-total-order); a [supremum](real-analysis.md#supremum) approached only at an excluded boundary is not enough. The resulting rule is a [maximum-likelihood estimator](#maximum-likelihood-estimator). The [likelihood function](#likelihood-function) uses a [probability mass function](probability-distribution.md#probability-mass-function) for discrete data and a [probability density function](continuous-probability-distribution.md#probability-density-function) for continuous data. See [MIT 18.05, Reading 10b, sections 3 and 3.2](https://ocw.mit.edu/courses/18-05-introduction-to-probability-and-statistics-spring-2022/mit18_05_s22_class10-prep-b.pdf).

The direction of the comparison is the interesting part: hold the observations fixed and vary the [statistical parameter](statistical-model.md#statistical-parameter). Ten independent [Bernoulli trials](discrete-probability-distribution.md#bernoulli-trial) with eight successes and two failures give the [maximum-likelihood estimate](#maximum-likelihood-estimator) $\widehat p=0.8$, as derived in [log-likelihood](#log-likelihood). This chooses the member of the [statistical model](statistical-model.md) that assigns the greatest mass to that outcome. It does not assert an $80\%$ [posterior probability](bayesian-statistics.md#posterior-probability) that this parameter value is true. [Bayesian statistics](bayesian-statistics.md) combines the same [likelihood function](#likelihood-function) with a [prior distribution](bayesian-statistics.md#prior-probability) to obtain a [posterior distribution](bayesian-statistics.md#bayesian-posterior); [maximum a posteriori estimation](bayesian-statistics.md#maximum-a-posteriori-estimation) maximizes that posterior mass or density instead.

The method turns many fitting tasks into one [maximization problem](mathematical-optimization.md#maximization-problem). In the [normal distribution](probability-distribution.md#normal-distribution) model with known [variance](variance.md), it recovers the [sample mean](variance.md#sample-mean) and [ordinary least squares](normal-linear-model.md#ordinary-least-squares), while [binomial regression](generalized-linear-model.md#binomial-regression) and [Poisson regression](generalized-linear-model.md#poisson-regression) use different sampling assumptions to build their own [likelihood functions](#likelihood-function). The [log-likelihood](#log-likelihood) turns independent contributions into a [sum](arithmetic.md#sum), exposing [score equations](statistical-modelling.md#score-equation) and [observed information](statistical-modelling.md#observed-fisher-information). A peak's location gives an estimate; its shape records how much the observed data distinguish nearby parameter values.

Existence, uniqueness, [bias](statistical-modelling.md#bias-of-an-estimator), and [statistical consistency](statistical-inference.md#consistency-statistics) are separate questions. [Normal mean and variance maximum-likelihood estimators](#normal-mean-and-variance-maximum-likelihood-estimators) include a variance estimate with [bias](statistical-modelling.md#bias-of-an-estimator), [likelihood supremum at an excluded boundary](#likelihood-supremum-at-an-excluded-boundary) gives nonexistence, and the [Neyman-Scott incidental parameter problem](#neyman-scott-incidental-parameter-problem) gives inconsistency. The usual [asymptotic normality of a maximum likelihood estimator](#asymptotic-normality-of-a-maximum-likelihood-estimator) requires assumptions: a [consistent estimator](statistical-inference.md#consistency-statistics) at an interior true parameter in a fixed finite-dimensional model with [identifiability](statistical-model.md#identifiability), sufficient smoothness and control of [log-likelihood](#log-likelihood) [derivatives](calculus.md#derivative), and finite nonsingular [Fisher information](statistical-modelling.md#fisher-information-matrix). A common parameter-independent [support of a probability distribution](probability-distribution.md#support-of-a-probability-distribution) is part of a standard sufficient framework; see [Rigollet, MIT 18.650, Maximum Likelihood Estimation, slides 22-23](https://ocw.mit.edu/courses/18-650-statistics-for-applications-fall-2016/36624c2682b346b07cab3da416b752a7_MIT18_650F16_Maximum_LE.pdf). This is a description of the regular setting, not a complete theorem's hypotheses. The [exact endpoint limit for a shifted exponential distribution](#exact-endpoint-limit-for-a-shifted-exponential-distribution) shows why changing support can produce a different rate and a nonnormal limit. These properties do not follow just from maximizing a function.

In his 1922 paper in the Royal Society's Philosophical Transactions A, R. A. Fisher explicitly distinguished [likelihood](#likelihood-function) from [probability](probability-theory.md#probability) and described choosing the parameter values with greatest [likelihood](#likelihood-function). Section 6 also discusses comparing [likelihoods](#likelihood-function) after giving the maximum value one, the convention used in the figures here. See [Fisher, On the Mathematical Foundations of Theoretical Statistics, section 6, pp. 326-328, DOI 10.1098/rsta.1922.0009](https://errorstatistics.com/wp-content/uploads/2021/04/fisher-1922.pdf).

**Table of contents**

- [Normal likelihood with variance equal to squared mean](#normal-likelihood-with-variance-equal-to-squared-mean)
- [Singular covariance and nonexistence of a Gaussian maximum likelihood estimate](#singular-covariance-and-nonexistence-of-a-gaussian-maximum-likelihood-estimate)
- [Compact-parameter consistency of maximum likelihood](#compact-parameter-consistency-of-maximum-likelihood)
- [Shifted exponential maximum likelihood](#shifted-exponential-maximum-likelihood)
  - [Exact endpoint limit for a shifted exponential distribution](#exact-endpoint-limit-for-a-shifted-exponential-distribution)
- [Maximum-likelihood estimator](#maximum-likelihood-estimator)
  - [Likelihood supremum at an excluded boundary](#likelihood-supremum-at-an-excluded-boundary)
  - [Uniform endpoint maximum-likelihood estimator](#uniform-endpoint-maximum-likelihood-estimator)
  - [Neyman-Scott incidental parameter problem](#neyman-scott-incidental-parameter-problem)
  - [Endpoint maximum likelihood for a singular location density](#endpoint-maximum-likelihood-for-a-singular-location-density)
  - [Exponential-rate maximum-likelihood estimator](#exponential-rate-maximum-likelihood-estimator)
  - [Maximum-likelihood fitted value](#maximum-likelihood-fitted-value)
    - [Maximum-likelihood fitted probability](#maximum-likelihood-fitted-probability)
  - [Normal mean and variance maximum-likelihood estimators](#normal-mean-and-variance-maximum-likelihood-estimators)
  - [Invariance property of maximum likelihood estimation](#invariance-property-of-maximum-likelihood-estimation)
  - [Likelihood function](#likelihood-function)
    - [Log-likelihood](#log-likelihood)
    - [Marginal likelihood from a nuisance-free statistic](#marginal-likelihood-from-a-nuisance-free-statistic)
    - [Conditional likelihood](#conditional-likelihood)
      - [Saddlepoint conditional likelihood adjustment](#saddlepoint-conditional-likelihood-adjustment)
    - [Observed-data likelihood](#observed-data-likelihood)
    - [Bayesian deviance](#bayesian-deviance)
    - [Conditional maximum likelihood](#conditional-maximum-likelihood)
    - [Profile likelihood](#profile-likelihood)
      - [Modified profile likelihood](#modified-profile-likelihood)
        - [Modified profile likelihood for inverse Gaussian shape](#modified-profile-likelihood-for-inverse-gaussian-shape)
        - [Modified profile likelihood for exponential regression](#modified-profile-likelihood-for-exponential-regression)
      - [Gamma-ratio marginal and profile likelihood identity](#gamma-ratio-marginal-and-profile-likelihood-identity)
      - [Profile log-likelihood](#profile-log-likelihood)
  - [Binomial proportion maximum-likelihood estimator](#binomial-proportion-maximum-likelihood-estimator)
  - [Exponential distribution rate estimator](#exponential-distribution-rate-estimator)
  - [Asymptotic normality of a maximum likelihood estimator](#asymptotic-normality-of-a-maximum-likelihood-estimator)

## Normal likelihood with variance equal to squared mean

↑ **Parent:** [Maximum likelihood estimation](maximum-likelihood-estimation.md)

For independent [normal distribution](probability-distribution.md#normal-distribution) observations with mean $\mu>0$ and variance $\mu^2$, put $S_1=\sum_iX_i$, $S_2=\sum_iX_i^2$. The [Fisher-Neyman factorization theorem](probability-and-statistics.md#fisher-neyman-factorization-theorem) makes $(S_1,S_2)$ a [sufficient statistic](probability-and-statistics.md#sufficient-statistic), since the [likelihood](#likelihood-function) is proportional to $\mu^{-n}\exp[-S_2/(2\mu^2)+S_1/\mu]$. Its logarithmic [derivative](calculus.md#derivative) has numerator $S_2-S_1\mu-n\mu^2$. When $S_2>0$, this changes sign once on the positive half-line and gives the displayed global [maximum-likelihood estimator](#maximum-likelihood-estimator). The zero sample is a probability-zero exception with unbounded [likelihood](#likelihood-function) as $\mu\downarrow0$.

## Singular covariance and nonexistence of a Gaussian maximum likelihood estimate

↑ **Parent:** [Maximum likelihood estimation](maximum-likelihood-estimation.md)

For independent $p$-variate [multivariate normal](probability-and-statistics.md#multivariate-normal-distribution) observations with unknown mean and unrestricted [positive-definite](bilinear-form.md#positive-definite-bilinear-form) [covariance matrix](variance.md#covariance-matrix), the centered scatter has [rank](quadratic-form.md#rank-one-quadratic-form) at most $n-1$. If it is singular, choose the mean to be the [sample mean](variance.md#sample-mean) and shrink the [covariance](variance.md#covariance) on a null direction of the scatter. The quadratic [likelihood](#likelihood-function) term stays fixed while the [determinant](multilinear-algebra.md#determinant) tends to zero, so the density [likelihood](#likelihood-function) tends to infinity. Thus a nonsingular [covariance](variance.md#covariance) maximum [likelihood](#likelihood-function) estimate exists only when the centered scatter is positive definite; for a nonsingular [Gaussian](probability-distribution.md#normal-distribution) population this occurs almost surely exactly when $n>p$.

## Compact-parameter consistency of maximum likelihood

↑ **Parent:** [Maximum likelihood estimation](maximum-likelihood-estimation.md)

On a compact parameter space, suppose the expected log-likelihood is continuous, uniquely maximized at the true parameter, and the normalized empirical log-likelihood converges uniformly in probability to its expectation. On the compact complement of every neighbourhood of the truth, the expected criterion has a strictly positive gap below its maximum. Uniform approximation by less than one-third of this gap excludes every empirical maximizer from that complement. [Identifiability](statistical-model.md#identifiability) and nonnegativity of [Kullback-Leibler divergence](f-divergence.md#kullback-leibler-divergence) supply the unique expected maximizer. The proof works for any measurable choice of maximizer.

## Shifted exponential maximum likelihood

↑ **Parent:** [Maximum likelihood estimation](maximum-likelihood-estimation.md)

A shifted [exponential distribution](continuous-probability-distribution.md#exponential-distribution) has location estimate equal to the sample minimum and rate estimate given above, for a nondegenerate sample of at least two observations. The minimum exceeds the true location on average by $1/(n\lambda)$. The residual sum above the minimum is gamma with shape $n-1$, so the rate estimate has expectation $n\lambda/(n-2)$ for $n>2$ and infinite expectation at $n=2$. The estimated location plus reciprocal rate is the unbiased sample mean.

### Exact endpoint limit for a shifted exponential distribution

↑ **Parent:** [Shifted exponential maximum likelihood](#shifted-exponential-maximum-likelihood)

For independent observations $Y_i=\theta+E_i$ with $E_i$ having [exponential distribution](continuous-probability-distribution.md#exponential-distribution) of known rate $\lambda>0$, the [likelihood](#likelihood-function) increases in $\theta$ until the smallest observation, so the [maximum-likelihood estimator](#maximum-likelihood-estimator) is $Y_{(1)}$. Its survival function is $\mathbb P(Y_{(1)}-\theta>t)=e^{-n\lambda t}$ for $t\ge0$. Therefore $n\lambda(Y_{(1)}-\theta)$ has exactly the unit-rate [exponential distribution](continuous-probability-distribution.md#exponential-distribution) for every sample size. This gives [statistical consistency](statistical-inference.md#consistency-statistics) and a one-sided nonnormal limit with rate $n$, illustrating how a support endpoint changes usual regular likelihood asymptotics.

## Maximum-likelihood estimator

↑ **Parent:** [Maximum likelihood estimation](maximum-likelihood-estimation.md)

A [maximum-likelihood estimator](#maximum-likelihood-estimator) is an [estimator](statistical-modelling.md#estimator) whose value maximizes the [likelihood function](#likelihood-function) for each sample where a finite maximizer exists. Before observation, $\widehat\theta(X)$ is a [random variable](random-variable.md) (the choice of maximizer must be a [measurable function](measure-theory.md#measurable-function)); after observation, $\widehat\theta(x)$ is the numerical [maximum-likelihood estimate](#maximum-likelihood-estimator). A formula must specify the allowed parameter set, including whether its endpoints belong to it.

For ten independent [Bernoulli trials](discrete-probability-distribution.md#bernoulli-trial), write $K=\sum_{i=1}^{10}X_i$. On the closed parameter interval $[0,1]$, the [binomial proportion maximum-likelihood estimator](#binomial-proportion-maximum-likelihood-estimator) is $\widehat p=K/10$. Eight successes give the estimate $0.8$. If $K=0$, the [likelihood](#likelihood-function) is $(1-p)^{10}$ and has its unique maximum at $p=0$; if $K=10$, it is $p^{10}$ and has its unique maximum at $p=1$. On the open interval $(0,1)$ these two samples have no [maximum-likelihood estimate](#maximum-likelihood-estimator): the [supremum](real-analysis.md#supremum) is one, but it is not attained. This is the same issue as [likelihood supremum at an excluded boundary](#likelihood-supremum-at-an-excluded-boundary).

A complete continuous example uses [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables) $X_i\sim N(\mu,1)$ with unknown [mean](expected-value.md) $\mu\in\mathbb R$ and known [standard deviation](variance.md#standard-deviation) one. Their [likelihood function](#likelihood-function) and [log-likelihood](#log-likelihood) are

$$
L(\mu;x)=(2\pi)^{-n/2}\exp\left[-\frac12\sum_{i=1}^n(x_i-\mu)^2\right],\qquad \ell(\mu;x)=-\frac n2\log(2\pi)-\frac12\sum_{i=1}^n(x_i-\mu)^2.
$$

The [sum](arithmetic.md#sum) of squared deviations separates as

$$
\sum_{i=1}^n(x_i-\mu)^2=\sum_{i=1}^n(x_i-\bar x)^2+n(\mu-\bar x)^2,
$$

because $\sum_i(x_i-\bar x)=0$. The first term is fixed in $\mu$, so the unique [maximum-likelihood estimator](#maximum-likelihood-estimator) is the [sample mean](variance.md#sample-mean) $\widehat\mu=\overline X$. This also proves the equivalence with [ordinary least squares](normal-linear-model.md#ordinary-least-squares) for this model. With the constructed observations $[-1,0,2,3]$, the [sample mean](variance.md#sample-mean) is one and the residual sum of squares is ten; hence

$$
\ell(\mu;x)=-2\log(2\pi)-5-2(\mu-1)^2,\qquad \widehat\mu=1.
$$

At $\mu=0$ or $2$, the [log-likelihood](#log-likelihood) is two below its peak, so the [likelihood ratio](statistical-hypothesis-test.md#likelihood-ratio) to the fitted value is $e^{-2}\approx0.135335$. The absolute [likelihood](#likelihood-function) at the peak is $(2\pi)^{-2}e^{-5}\approx0.000170674$, a joint density value, not the [probability](probability-theory.md#probability) of observing exactly those four real numbers.

The following figure compares that sample with a constructed sixteen-observation sample consisting of four repetitions of the displayed four values, modeled as sixteen independent draws. Both fits have [sample mean](variance.md#sample-mean) one, but

$$
\ell_n(\mu)-\ell_n(1)=-\frac n2(\mu-1)^2,\qquad \frac{L_n(\mu)}{L_n(1)}=e^{-n(\mu-1)^2/2},\qquad -\ell_n''(\mu)=n.
$$

Thus the [observed information](statistical-modelling.md#observed-fisher-information) is four times as large for $n=16$ as for $n=4$. The distance from the peak at relative height $e^{-2}$ decreases from one to $1/2$: the width scales as $1/\sqrt n$. This is a comparison of two stipulated samples; merely copying recorded observations would not create new independent evidence.

<a id="image-known-variance-normal-mean-the-same-fitted-mean-with-different-likelihood-curvature"></a>
![](gaussian-mean-likelihood.png)

**[Figure 1](#image-known-variance-normal-mean-the-same-fitted-mean-with-different-likelihood-curvature). Known-variance normal mean: the same fitted mean with different likelihood curvature**.

Even uniqueness needs checking. If the [Bernoulli distribution](discrete-probability-distribution.md#bernoulli-distribution) success parameter is written $p=\theta^2$ with $\theta\in[-1,1]$, eight successes give two [maximum-likelihood estimates](#maximum-likelihood-estimator), $\theta=\pm\sqrt{0.8}$, because both give the same [probability distribution](probability-distribution.md). The problem is a failure of [identifiability](statistical-model.md#identifiability). The special cases below show other ways an [MLE](#maximum-likelihood-estimator) can have [bias](statistical-modelling.md#bias-of-an-estimator) or fail the usual [asymptotic normality](statistical-inference.md#asymptotic-normality).

### Likelihood supremum at an excluded boundary

↑ **Parent:** [Maximum-likelihood estimator](#maximum-likelihood-estimator)

A likelihood need not attain its supremum when the parameter space excludes a boundary point. For example, with parameter $0<\theta\leq1$ and a zero Poisson count, the likelihood $e^{-\theta}$ is strictly decreasing and has no maximum. Extending the parameter space to include zero gives an extended maximum-likelihood estimate there. A proposed estimator formula involving that boundary value must distinguish the extended estimate from an actual maximizer in the original space.

### Uniform endpoint maximum-likelihood estimator

↑ **Parent:** [Maximum-likelihood estimator](#maximum-likelihood-estimator)

For independent $U[0,\theta]$ observations, the likelihood decreases as $\theta^{-n}$ on $[\max_iY_i,\infty)$, so its maximizer is the [sample maximum](probability-theory.md#sample-maximum) almost surely. Its exact distribution is $\mathbb P_\theta(\widehat\theta_n\leq y)=(y/\theta)^n$ for $0\leq y\leq\theta$. This proves consistency and an endpoint error of order $1/n$, with the displayed exponential limit. Parameter-dependent support violates the usual regularity condition behind nondegenerate square-root-sample-size normal limits; the ordinary interior score is not centered.

### Neyman-Scott incidental parameter problem

↑ **Parent:** [Maximum-likelihood estimator](#maximum-likelihood-estimator)

A growing number of nuisance parameters can prevent a [maximum-likelihood estimator](#maximum-likelihood-estimator) of a common parameter from being [consistent](statistical-inference.md#consistency-statistics). With two independent normal observations of mean $\mu_i$ per group, the profiled variance estimate $\sum_i(X_{1i}-X_{2i})^2/(4n)$ tends to half the true variance, because each unknown mean is estimated using only two observations.

### Endpoint maximum likelihood for a singular location density

↑ **Parent:** [Maximum-likelihood estimator](#maximum-likelihood-estimator)

For density $r(x-\theta)^{r-1}$ on $[\theta,\theta+1]$, $0<r<1$, the interior [likelihood function](#likelihood-function) increases without bound as $\theta$ approaches the sample minimum. The extended-likelihood estimator is that minimum. An arbitrary finite reassignment of the density at the endpoint can eliminate an attained finite maximum, so the endpoint convention must be stated.

### Exponential-rate maximum-likelihood estimator

↑ **Parent:** [Maximum-likelihood estimator](#maximum-likelihood-estimator)

For independent observations from the [exponential distribution](continuous-probability-distribution.md#exponential-distribution) with rate $\theta$, the log-likelihood is $n\log\theta-\theta\sum_iX_i$, so

$$
\widehat\theta=\frac n{\sum_iX_i}=\frac1{\overline X}.
$$

The [central limit theorem](convergence-of-random-variables.md#central-limit-theorem) and [delta method](statistical-inference.md#delta-method) give

$$
\sqrt n(\widehat\theta-\theta)\xrightarrow dN(0,\theta^2).
$$

### Maximum-likelihood fitted value

↑ **Parent:** [Maximum-likelihood estimator](#maximum-likelihood-estimator)

A maximum-likelihood fitted value is a response mean or probability evaluated at a [maximum-likelihood estimate](#maximum-likelihood-estimator). In a parametric mean model $\mu_i(\theta)$ it is $\widehat\mu_i=\mu_i(\widehat\theta)$.

#### Maximum-likelihood fitted probability

↑ **Parent:** [Maximum-likelihood fitted value](#maximum-likelihood-fitted-value)

### Normal mean and variance maximum-likelihood estimators

↑ **Parent:** [Maximum-likelihood estimator](#maximum-likelihood-estimator)

For [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables) $X_1,\ldots,X_n\sim N(\mu,\sigma^2)$, the [maximum-likelihood estimators](#maximum-likelihood-estimator) are

$$
\widehat\mu=\overline X,
\qquad
\widehat{\sigma}^2=\frac1n\sum_{i=1}^n(X_i-\overline X)^2.
$$

The first is [unbiased](statistical-modelling.md#unbiased-estimator), while $\mathbb E\widehat{\sigma}^2=(n-1)\sigma^2/n$.

### Invariance property of maximum likelihood estimation

↑ **Parent:** [Maximum-likelihood estimator](#maximum-likelihood-estimator)

If $\widehat\theta$ maximizes a likelihood and the target parameter is $\eta=g(\theta)$, a maximum-likelihood estimate of $\eta$ is $g(\widehat\theta)$, with the usual interpretation when $g$ is not one-to-one.

### Likelihood function

↑ **Parent:** [Maximum-likelihood estimator](#maximum-likelihood-estimator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Likelihood_function)

For a fixed observed sample $x$, a [likelihood function](#likelihood-function) is

$$
L(\theta;x)=f_\theta(x),\qquad \theta\in\Theta,
$$

where $f_\theta$ is the [probability mass function](probability-distribution.md#probability-mass-function) or [probability density function](continuous-probability-distribution.md#probability-density-function) of the observations under the [statistical parameter](statistical-model.md#statistical-parameter) $\theta$. All densities must be defined relative to the same parameter-independent [dominating measure](measure-theory.md#dominating-measure). The sample is fixed; the parameter is the function's argument. With [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables), the joint mass or density factors as $L(\theta;x)=\prod_{i=1}^n f_\theta(x_i)$. This definition and the distinction between sampling [probability](probability-theory.md#probability) and parameter uncertainty are explained in [MIT 18.05, Reading 10b, sections 3 and 3.2](https://ocw.mit.edu/courses/18-05-introduction-to-probability-and-statistics-spring-2022/mit18_05_s22_class10-prep-b.pdf).

For an observed ordered sequence of ten independent [Bernoulli trials](discrete-probability-distribution.md#bernoulli-trial) containing eight successes and two failures, each success contributes $p$ and each failure contributes $1-p$, giving

$$
L_{\mathrm{ordered}}(p)=p^8(1-p)^2,\qquad 0\leq p\leq1.
$$

If the observation is instead only the total count $K=8$, its [binomial distribution](discrete-probability-distribution.md#binomial-distribution) [probability mass function](probability-distribution.md#probability-mass-function) sums over the $\binom{10}{8}=45$ possible ordered sequences:

$$
L_{\mathrm{count}}(p)=\binom{10}{8}p^8(1-p)^2=45L_{\mathrm{ordered}}(p).
$$

The raw heights differ: at $p=0.8$ they are approximately $0.0067108864$ and $0.301989888$. Their [maximum-likelihood estimates](#maximum-likelihood-estimator) are identical. More generally, multiplication by any finite positive constant $c(x)$ independent of $\theta$ leaves the maximizing parameter values and all [likelihood ratios](statistical-hypothesis-test.md#likelihood-ratio) unchanged. Multiplication by a parameter-dependent factor can change the [MLE](#maximum-likelihood-estimator); dropping such a factor is not justified. Relative likelihood height $L(\theta;x)/L(\widehat\theta;x)$ sets the peak to one, without making the area under the curve one.

Normalization of $f_\theta$ is over possible data values for each fixed parameter. It imposes no requirement that $\int_\Theta L(\theta;x)\,d\theta=1$. For example, the ordered [Bernoulli trials](discrete-probability-distribution.md#bernoulli-trial) [likelihood](#likelihood-function) above has

$$
\int_0^1p^8(1-p)^2\,dp=\frac19-\frac2{10}+\frac1{11}=\frac1{495}.
$$

Its integral is not one, and its values are not [posterior probabilities](bayesian-statistics.md#posterior-probability) for $p$. When the [Bayesian posterior](bayesian-statistics.md#bayesian-posterior) is defined, [Bayes' theorem](probability-theory.md#bayes-theorem) multiplies the [likelihood](#likelihood-function) by a [prior density](bayesian-statistics.md#prior-density) and normalizes that product. Choosing to normalize a [likelihood function](#likelihood-function) alone is an additional choice, such as using a [uniform prior](bayesian-statistics.md#uniform-prior) in those parameter coordinates, rather than part of the definition of [likelihood](#likelihood-function).

For observations with a [probability density function](continuous-probability-distribution.md#probability-density-function), the [probability](probability-theory.md#probability) of an exact sample point is zero. If a scalar density is continuous at the observed value $x$, then

$$
\mathbb P_\theta\bigl(x\leq X\leq x+\varepsilon\bigr)=f_\theta(x)\varepsilon+o(\varepsilon),\qquad \varepsilon\downarrow0.
$$

Thus the density compares probabilities of small, equal observation intervals at different parameter values; it is not itself the [probability](probability-theory.md#probability) of that exact real number. The equal-width factor is independent of the parameter. This gives visual intuition for density [likelihoods](#likelihood-function), as in [MIT 18.05, Reading 10b, section 4](https://ocw.mit.edu/courses/18-05-introduction-to-probability-and-statistics-spring-2022/mit18_05_s22_class10-prep-b.pdf). The [normal distribution](probability-distribution.md#normal-distribution) example in [maximum-likelihood estimator](#maximum-likelihood-estimator) makes the comparison explicit. If only rounded intervals are recorded, their integrated probabilities give the exact observation [likelihood](#likelihood-function); using midpoint densities is an approximation.

#### Log-likelihood

↑ **Parent:** [Likelihood function](#likelihood-function)

The [log-likelihood](#log-likelihood) is the [natural logarithm](calculus.md#natural-logarithm) of the [likelihood function](#likelihood-function):

$$
\ell(\theta;x)=\log L(\theta;x).
$$

For positive finite [likelihood](#likelihood-function), the [natural logarithm](calculus.md#natural-logarithm) is a [strictly increasing function](calculus.md#strictly-increasing-function), so the maximizing parameter values are unchanged. Set $\ell=-\infty$ where $L=0$; the same ordering then includes zero-likelihood boundaries whenever a positive finite maximum exists. For [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables), a product becomes a sum,

$$
L(\theta;x)=\prod_{i=1}^n f_\theta(x_i),\qquad \ell(\theta;x)=\sum_{i=1}^n\log f_\theta(x_i).
$$

This makes [derivatives](calculus.md#derivative) simpler and avoids forming products of tiny numbers in [floating-point arithmetic](floating-point-arithmetic.md). These equal-maximizer and additive formulas underlie the worked calculations in [MIT 18.05, Reading 10b, section 3.1](https://ocw.mit.edu/courses/18-05-introduction-to-probability-and-statistics-spring-2022/mit18_05_s22_class10-prep-b.pdf).

For the ordered sample of eight successes and two failures in [likelihood function](#likelihood-function), on $0<p<1$,

$$
\ell(p)=8\log p+2\log(1-p),\qquad \ell'(p)=\frac8p-\frac2{1-p},\qquad \ell''(p)=-\frac8{p^2}-\frac2{(1-p)^2}<0.
$$

The [score equation](statistical-modelling.md#score-equation) $\ell'(p)=0$ gives $8(1-p)=2p$, hence $\widehat p=8/10=0.8$. The negative [second derivative](calculus.md#second-derivative) proves [strict concavity](real-analysis.md#strict-concavity), so this is the unique interior maximum. Both counts are positive, so $L(0)=L(1)=0$, while $L(p)>0$ inside: the same point is the unique global [maximum](set.md#maximum-of-a-subset-of-a-total-order) on $[0,1]$. Counting only successes adds $\log45$ to the [log-likelihood](#log-likelihood), leaving both [derivatives](calculus.md#derivative) and the [MLE](#maximum-likelihood-estimator) unchanged. For all-success or all-failure samples, the boundary analysis in [maximum-likelihood estimator](#maximum-likelihood-estimator) applies instead of an interior [score equation](statistical-modelling.md#score-equation).

The two panels below compare $k=2,5,8$ successes out of ten [Bernoulli trials](discrete-probability-distribution.md#bernoulli-trial). Their peaks are at $\widehat p=k/10$. The left panel uses relative height; the right panel uses the [log-likelihood](#log-likelihood) difference from each peak. These are the same comparison on two scales:

$$
\ell(p)-\ell(\widehat p)=\log\frac{L(p)}{L(\widehat p)},\qquad \frac{L(p)}{L(\widehat p)}=\exp\bigl(\ell(p)-\ell(\widehat p)\bigr).
$$

A difference of $-2$ means relative height $e^{-2}$, and a difference of $-10$ means $e^{-10}$; the [log-likelihood](#log-likelihood) scale makes small relative heights easier to see. Neither vertical axis is a parameter [probability density function](continuous-probability-distribution.md#probability-density-function). The zero [likelihood](#likelihood-function) endpoints have [log-likelihood](#log-likelihood) $-\infty$ and are outside the finite vertical range in the right panel.

<a id="image-ten-bernoulli-trials-relative-likelihood-heights-and-log-likelihood-differences-share-the-same-peaks"></a>
![](bernoulli-likelihood-and-log.png)

**[Figure 2](#image-ten-bernoulli-trials-relative-likelihood-heights-and-log-likelihood-differences-share-the-same-peaks). Ten Bernoulli trials: relative likelihood heights and log-likelihood differences share the same peaks**.

Multiplying a [likelihood function](#likelihood-function) by a positive parameter-independent constant adds a constant to its [log-likelihood](#log-likelihood). Subtracting its peak removes that constant. This is why the ordered-data and count-data curves coincide in this figure after rescaling. When differentiable, the [gradient](multivariable-calculus.md#gradient) of the [log-likelihood](#log-likelihood) is the [score function](statistical-modelling.md#informant-function); the negative [Hessian matrix](multivariable-calculus.md#hessian-matrix) is the [observed information](statistical-modelling.md#observed-fisher-information). A solution of a [score equation](statistical-modelling.md#score-equation) still needs checking against other stationary points and boundaries: maximizing the [log-likelihood](#log-likelihood) does not automatically make it [concave](real-analysis.md#concave-function).

#### Marginal likelihood from a nuisance-free statistic

↑ **Parent:** [Likelihood function](#likelihood-function)

If a statistic T has marginal density depending on a parameter of interest but not on a nuisance parameter, that density gives a likelihood for the interest parameter. It is obtained by integrating out other observed coordinates. In contrast, [profile likelihood](#profile-likelihood) maximizes the full likelihood over the nuisance parameter. This sampling-statistic construction is different from Bayesian model evidence, which integrates parameters against a prior. No prior is required for a nuisance-free sampling marginal.

#### Conditional likelihood

↑ **Parent:** [Likelihood function](#likelihood-function)

A conditional likelihood evaluates the conditional distribution of the observed data given a specified statistic. If that distribution does not involve a [nuisance parameter](statistical-model.md#nuisance-parameter), it permits inference about the remaining parameter without estimating the nuisance parameter. The conditioning statistic need not be [ancillary](probability-and-statistics.md#ancillary-statistic); possible information loss must be assessed within the model. [Conditional maximum likelihood](#conditional-maximum-likelihood) maximizes this function.

##### Saddlepoint conditional likelihood adjustment

↑ **Parent:** [Conditional likelihood](#conditional-likelihood)

For a regular two-parameter [exponential family](exponential-family.md), condition on the [sample mean](variance.md#sample-mean) of the nuisance canonical statistic. [Exponential tilting](probability-distribution.md#exponential-tilting) to its observed value and the [saddlepoint density approximation](probability-distribution.md#saddlepoint-density-approximation) give a nuisance-statistic density proportional to $d_{\lambda\lambda}^{-1/2}$ times its large-deviation exponential. Dividing the joint [likelihood](#likelihood-function) by this density gives the [profile log-likelihood](#profile-log-likelihood) plus the displayed adjustment, up to a data-only constant. The sign is positive. This construction assumes an interior saddle with positive curvature and a sufficiently regular nonlattice density; conditioning on a lattice statistic requires the corresponding mass approximation.

#### Observed-data likelihood

↑ **Parent:** [Likelihood function](#likelihood-function)

An observed-data [likelihood](#likelihood-function) integrates the full-data [statistical probability density](continuous-probability-distribution.md#probability-density-function) over unobserved values, rather than inserting arbitrary values or discarding incomplete records. When the observation pattern is random, its mechanism belongs to the joint observation model unless the conditions for an [ignorable missingness mechanism](probability-and-statistics.md#ignorable-missingness-mechanism) permit its factor to be omitted.

#### Bayesian deviance

↑ **Parent:** [Likelihood function](#likelihood-function)

A [Bayesian deviance](#bayesian-deviance) is minus twice the [log-likelihood](#log-likelihood), with any chosen additive data-only constant held consistent across the models being compared. Its [Bayesian posterior](bayesian-statistics.md#bayesian-posterior) expectation measures average fit. In the [deviance information criterion](statistical-modelling.md#deviance-information-criterion), evaluating it at a parameter's [posterior mean](bayesian-statistics.md#posterior-mean) also enters the effective complexity penalty. This likelihood-based convention differs by a data-only constant from a saturated-model [exponential-family deviance](exponential-family.md#exponential-family-deviance) when a common saturated model exists.

#### Conditional maximum likelihood

↑ **Parent:** [Likelihood function](#likelihood-function)

A conditional [likelihood function](#likelihood-function) conditions on an initial observation or another specified statistic. In an [autoregressive model](time-series.md#autoregressive-model), conditioning on the first observed state avoids modeling its initial density. For Gaussian transitions, maximizing this likelihood is a regression problem; treating an autoregressive coefficient as known changes the exact distribution of an estimated mean.

#### Profile likelihood

↑ **Parent:** [Likelihood function](#likelihood-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Profile_likelihood)

For a parameter of interest $\psi$ and nuisance parameter $\lambda$, the profile likelihood is

$$
L_p(\psi)=\sup_\lambda L(\psi,\lambda).
$$

It compares values of $\psi$ after fitting the nuisance parameter as favourably as possible at each value.

##### Modified profile likelihood

↑ **Parent:** [Profile likelihood](#profile-likelihood)

For parameter of interest $\psi$, constrained nuisance fit $\widehat\lambda_\psi$, and suitable ancillary sample coordinates $(\widehat\psi,\widehat\lambda,a)$, this adjustment includes both nuisance [observed information](statistical-modelling.md#observed-fisher-information) and a sample-space [Jacobian determinant](multivariable-calculus.md#jacobian-determinant). The derivative holds $\widehat\psi,a$ fixed. Implicit differentiation of the constrained nuisance [score function](statistical-modelling.md#informant-function) gives the equivalent expression $\ell_p+\tfrac12\log|j_{\lambda\lambda}|-\log|\ell_{\lambda;\widehat\lambda}|$. The semicolon distinguishes data-coordinate differentiation from parameter differentiation. Omitting the Jacobian requires an additional justified simplification; the information adjustment alone is not universal.

###### Modified profile likelihood for inverse Gaussian shape

↑ **Parent:** [Modified profile likelihood](#modified-profile-likelihood)

For independent [Inverse Gaussian distributions](exponential-family.md#inverse-gaussian-distribution) with shape $\psi$ and mean $\lambda$, the constrained and full nuisance [maximum-likelihood estimates](#maximum-likelihood-estimator) both equal $\bar Y$, giving a unit sample-coordinate [Jacobian determinant](multivariable-calculus.md#jacobian-determinant). The nuisance [observed information](statistical-modelling.md#observed-fisher-information) there is $n\psi/\bar Y^3$. Hence subtracting half its logarithm from the [profile log-likelihood](#profile-log-likelihood) replaces the coefficient $n/2$ of $\log\psi$ by $(n-1)/2$. For a nonconstant sample the modified fit is $(n-1)/(\sum_iY_i^{-1}-n/\bar Y)$.

###### Modified profile likelihood for exponential regression

↑ **Parent:** [Modified profile likelihood](#modified-profile-likelihood)

For independent [exponential distributions](continuous-probability-distribution.md#exponential-distribution) with means $\lambda e^{\psi x_i}$ and a nonconstant fixed design, put $A(\psi)=\sum_iY_ie^{-\psi x_i}$. The constrained [maximum-likelihood estimate](#maximum-likelihood-estimator) is $\widetilde\lambda_\psi=A(\psi)/n$ and the [profile log-likelihood](#profile-log-likelihood) is $\ell_p(\psi)=-n\log[A(\psi)/n]-\psi\sum_i x_i-n$. Use the [ancillary statistic](probability-and-statistics.md#ancillary-statistic) $a_i=\log Y_i-\log\widehat\lambda-\widehat\psi x_i$ to specify sample coordinates. At fixed $\widehat\psi,a$, the [Jacobian determinant](multivariable-calculus.md#jacobian-determinant) $\partial\widetilde\lambda_\psi/\partial\widehat\lambda=\widetilde\lambda_\psi/\widehat\lambda$, while $j_{\lambda\lambda}(\psi,\widetilde\lambda_\psi)=n/\widetilde\lambda_\psi^2$. Therefore the [modified profile likelihood](#modified-profile-likelihood) satisfies

$$
\ell_m(\psi)=\ell_p(\psi)-\tfrac12\log j_{\lambda\lambda}-\log\left|\frac{\partial\widetilde\lambda_\psi}{\partial\widehat\lambda}\right|=\ell_p(\psi)+\log\widehat\lambda-\tfrac12\log n.
$$

The adjustment is independent of $\psi$. Keeping only the [observed information](statistical-modelling.md#observed-fisher-information) adjustment would miss this cancellation.

##### Gamma-ratio marginal and profile likelihood identity

↑ **Parent:** [Profile likelihood](#profile-likelihood)

For independent $X\sim\operatorname{Gamma}(m,\psi\lambda)$ and $Y\sim\operatorname{Gamma}(n,\lambda)$ in shape-rate notation, $T=X/Y$ has density proportional to $\psi^m t^{m-1}(1+\psi t)^{-(m+n)}$. Its distribution is nuisance-free in lambda. The nuisance maximum is $(m+n)/(\psi X+Y)$, so substituting into the full likelihood gives the same interest-parameter log-likelihood up to a parameter-free term. Equality here is special to the common-scale structure, not a general equality of profiling and marginalization.

##### Profile log-likelihood

↑ **Parent:** [Profile likelihood](#profile-likelihood)

The logarithm of the [profile likelihood](#profile-likelihood) is the full [log-likelihood](#log-likelihood) evaluated at the nuisance fit constrained to the specified parameter of interest. It preserves [likelihood ratios](statistical-hypothesis-test.md#likelihood-ratio) and maximizers, but is not generally a normalized sampling log-density. Conditioning and integrating out [nuisance parameters](statistical-model.md#nuisance-parameter) are different operations.

### Binomial proportion maximum-likelihood estimator

↑ **Parent:** [Maximum-likelihood estimator](#maximum-likelihood-estimator)

For $X\sim\operatorname{Bin}(n,\theta)$, maximizing $\theta^X(1-\theta)^{n-X}$ gives

$$
\widehat\theta=\frac Xn.
$$

### Exponential distribution rate estimator

↑ **Parent:** [Maximum-likelihood estimator](#maximum-likelihood-estimator)

For independent exponential observations with rate $\theta$, the MLE is $1/\overline X$ and has asymptotic variance $\theta^2/n$.

### Asymptotic normality of a maximum likelihood estimator

↑ **Parent:** [Maximum-likelihood estimator](#maximum-likelihood-estimator)

In a regular $p$-parameter model with one-observation Fisher information $I(\theta_0)$,

$$
\sqrt n(\widehat\theta_n-\theta_0)
\xrightarrow d N_p(0,I(\theta_0)^{-1}).
$$

## ↑ Ancestors (6)

1. [Statistical modelling](statistical-modelling.md)
2. [Statistical model](statistical-model.md)
3. [Probability and statistics](probability-and-statistics.md)
4. [Area of mathematics](mathematics.md#area-of-mathematics)
5. [Mathematics](mathematics.md)
6. [Codex Wiki](README.md)

## ← Incoming links (54)

- [Bayesian model evidence](bayesian-statistics.md#bayesian-model-evidence)
- [Cross-entropy and maximum likelihood](information-entropy.md#cross-entropy-and-maximum-likelihood)
- [Laplace location and scale maximum likelihood](continuous-probability-distribution.md#laplace-location-and-scale-maximum-likelihood)
- [Laplace regression](continuous-probability-distribution.md#laplace-regression)
- [Maximum likelihood estimation](maximum-likelihood-estimation.md)
- [Pairwise comparison model](statistical-modelling.md#pairwise-comparison-model)
- [Solution](past-exam-of-the-biochemistry-course-of-the-university-of-cambridge/2025/paper-1.md#section-ii/4/solution)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-1.md#4/c/solution)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-2.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-1.md#3d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-28.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-33.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-2.md#12h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-39.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-40.md#1/b/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-42.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-4.md#19d/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-45.md#3/vi/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-1.md#18c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-44.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48.md#6/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-4.md#19h/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-4.md#19h/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-2.md#5j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-42.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-38.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-1.md#28j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-32.md#2/2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-32.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4.md#4j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-33.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-205.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207.md#3/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2.md#28k/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207.md#4/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207.md#4/c/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4.md#19h/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1.md#29j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-1.md#19h/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2.md#28j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-221.md#4/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-342.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-207.md#5/b/solution)
- [Solution](past-exam-of-the-plant-sciences-course-of-the-university-of-cambridge/2025/paper-plm3.md#2/solution)
- [Poisson spike-train likelihood fitting](neuroscience.md#poisson-spike-train-likelihood-fitting)
- [Potential event time](survival-analysis.md#potential-event-time)
- [Power law](analysis.md#power-law)
- [Statistical estimation](statistical-inference.md#statistical-estimation)
- [Uniform-alternative binomial Bayes factor](bayesian-statistics.md#uniform-alternative-binomial-bayes-factor)
