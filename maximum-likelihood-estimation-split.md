# Maximum likelihood estimation

↑ **Parent:** [Statistical modelling](statistical-modelling-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Maximum_likelihood_estimation)

[Maximum likelihood estimation](maximum-likelihood-estimation-split.md) is a method of [statistical estimation](statistical-estimation.md): within a specified [statistical model](statistical-model-split.md), choose the [statistical parameter](statistical-parameter.md) values that maximize the [likelihood function](likelihood-function.md) of the observed data. For a parameter set $\Theta$ and observations $x$, its exact requirement is

$$
\widehat\theta(x)\in\Theta,\qquad L(\widehat\theta(x);x)=\sup_{\theta\in\Theta}L(\theta;x).
$$

The equality requires an attained, finite [maximum](maximum-of-a-subset-of-a-total-order.md); a [supremum](supremum.md) approached only at an excluded boundary is not enough. The resulting rule is a [maximum-likelihood estimator](maximum-likelihood-estimator.md). The [likelihood function](likelihood-function.md) uses a [probability mass function](probability-mass-function.md) for discrete data and a [probability density function](probability-density-function.md) for continuous data. See [MIT 18.05, Reading 10b, sections 3 and 3.2](https://ocw.mit.edu/courses/18-05-introduction-to-probability-and-statistics-spring-2022/mit18_05_s22_class10-prep-b.pdf).

The direction of the comparison is the interesting part: hold the observations fixed and vary the [statistical parameter](statistical-parameter.md). Ten independent [Bernoulli trials](bernoulli-trial.md) with eight successes and two failures give the [maximum-likelihood estimate](maximum-likelihood-estimator.md) $\widehat p=0.8$, as derived in [log-likelihood](log-likelihood.md). This chooses the member of the [statistical model](statistical-model-split.md) that assigns the greatest mass to that outcome. It does not assert an $80\%$ [posterior probability](posterior-probability.md) that this parameter value is true. [Bayesian statistics](bayesian-statistics-split.md) combines the same [likelihood function](likelihood-function.md) with a [prior distribution](prior-probability.md) to obtain a [posterior distribution](bayesian-posterior.md); [maximum a posteriori estimation](maximum-a-posteriori-estimation.md) maximizes that posterior mass or density instead.

The method turns many fitting tasks into one [maximization problem](maximization-problem.md). In the [normal distribution](normal-distribution.md) model with known [variance](variance-split.md), it recovers the [sample mean](sample-mean.md) and [ordinary least squares](ordinary-least-squares.md), while [binomial regression](binomial-regression.md) and [Poisson regression](poisson-regression.md) use different sampling assumptions to build their own [likelihood functions](likelihood-function.md). The [log-likelihood](log-likelihood.md) turns independent contributions into a [sum](sum.md), exposing [score equations](score-equation.md) and [observed information](observed-fisher-information.md). A peak's location gives an estimate; its shape records how much the observed data distinguish nearby parameter values.

Existence, uniqueness, [bias](bias-of-an-estimator.md), and [statistical consistency](consistency-statistics.md) are separate questions. [Normal mean and variance maximum-likelihood estimators](normal-mean-and-variance-maximum-likelihood-estimators.md) include a variance estimate with [bias](bias-of-an-estimator.md), [likelihood supremum at an excluded boundary](likelihood-supremum-at-an-excluded-boundary.md) gives nonexistence, and the [Neyman-Scott incidental parameter problem](neyman-scott-incidental-parameter-problem.md) gives inconsistency. The usual [asymptotic normality of a maximum likelihood estimator](asymptotic-normality-of-a-maximum-likelihood-estimator.md) requires assumptions: a [consistent estimator](consistency-statistics.md) at an interior true parameter in a fixed finite-dimensional model with [identifiability](identifiability.md), sufficient smoothness and control of [log-likelihood](log-likelihood.md) [derivatives](derivative.md), and finite nonsingular [Fisher information](fisher-information-matrix.md). A common parameter-independent [support of a probability distribution](support-of-a-probability-distribution.md) is part of a standard sufficient framework; see [Rigollet, MIT 18.650, Maximum Likelihood Estimation, slides 22-23](https://ocw.mit.edu/courses/18-650-statistics-for-applications-fall-2016/36624c2682b346b07cab3da416b752a7_MIT18_650F16_Maximum_LE.pdf). This is a description of the regular setting, not a complete theorem's hypotheses. The [exact endpoint limit for a shifted exponential distribution](exact-endpoint-limit-for-a-shifted-exponential-distribution.md) shows why changing support can produce a different rate and a nonnormal limit. These properties do not follow just from maximizing a function.

In his 1922 paper in the Royal Society's Philosophical Transactions A, R. A. Fisher explicitly distinguished [likelihood](likelihood-function.md) from [probability](probability.md) and described choosing the parameter values with greatest [likelihood](likelihood-function.md). Section 6 also discusses comparing [likelihoods](likelihood-function.md) after giving the maximum value one, the convention used in the figures here. See [Fisher, On the Mathematical Foundations of Theoretical Statistics, section 6, pp. 326-328, DOI 10.1098/rsta.1922.0009](https://errorstatistics.com/wp-content/uploads/2021/04/fisher-1922.pdf).

**Table of contents**

- [Normal likelihood with variance equal to squared mean](normal-likelihood-with-variance-equal-to-squared-mean.md)
- [Singular covariance and nonexistence of a Gaussian maximum likelihood estimate](singular-covariance-and-nonexistence-of-a-gaussian-maximum-likelihood-estimate.md)
- [Compact-parameter consistency of maximum likelihood](compact-parameter-consistency-of-maximum-likelihood.md)
- [Shifted exponential maximum likelihood](shifted-exponential-maximum-likelihood.md)
  - [Exact endpoint limit for a shifted exponential distribution](exact-endpoint-limit-for-a-shifted-exponential-distribution.md)
- [Maximum-likelihood estimator](maximum-likelihood-estimator.md)
  - [Likelihood supremum at an excluded boundary](likelihood-supremum-at-an-excluded-boundary.md)
  - [Uniform endpoint maximum-likelihood estimator](uniform-endpoint-maximum-likelihood-estimator.md)
  - [Neyman-Scott incidental parameter problem](neyman-scott-incidental-parameter-problem.md)
  - [Endpoint maximum likelihood for a singular location density](endpoint-maximum-likelihood-for-a-singular-location-density.md)
  - [Exponential-rate maximum-likelihood estimator](exponential-rate-maximum-likelihood-estimator.md)
  - [Maximum-likelihood fitted value](maximum-likelihood-fitted-value.md)
    - [Maximum-likelihood fitted probability](maximum-likelihood-fitted-probability.md)
  - [Normal mean and variance maximum-likelihood estimators](normal-mean-and-variance-maximum-likelihood-estimators.md)
  - [Invariance property of maximum likelihood estimation](invariance-property-of-maximum-likelihood-estimation.md)
  - [Likelihood function](likelihood-function.md)
    - [Log-likelihood](log-likelihood.md)
    - [Marginal likelihood from a nuisance-free statistic](marginal-likelihood-from-a-nuisance-free-statistic.md)
    - [Conditional likelihood](conditional-likelihood.md)
      - [Saddlepoint conditional likelihood adjustment](saddlepoint-conditional-likelihood-adjustment.md)
    - [Observed-data likelihood](observed-data-likelihood.md)
    - [Bayesian deviance](bayesian-deviance.md)
    - [Conditional maximum likelihood](conditional-maximum-likelihood.md)
    - [Profile likelihood](profile-likelihood.md)
      - [Modified profile likelihood](modified-profile-likelihood.md)
        - [Modified profile likelihood for inverse Gaussian shape](modified-profile-likelihood-for-inverse-gaussian-shape.md)
        - [Modified profile likelihood for exponential regression](modified-profile-likelihood-for-exponential-regression.md)
      - [Gamma-ratio marginal and profile likelihood identity](gamma-ratio-marginal-and-profile-likelihood-identity.md)
      - [Profile log-likelihood](profile-log-likelihood.md)
  - [Binomial proportion maximum-likelihood estimator](binomial-proportion-maximum-likelihood-estimator.md)
  - [Exponential distribution rate estimator](exponential-distribution-rate-estimator.md)
  - [Asymptotic normality of a maximum likelihood estimator](asymptotic-normality-of-a-maximum-likelihood-estimator.md)

## ↑ Ancestors (6)

1. [Statistical modelling](statistical-modelling-split.md)
2. [Statistical model](statistical-model-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (54)

- [Bayesian model evidence](bayesian-model-evidence.md)
- [Cross-entropy and maximum likelihood](cross-entropy-and-maximum-likelihood.md)
- [Laplace location and scale maximum likelihood](laplace-location-and-scale-maximum-likelihood.md)
- [Laplace regression](laplace-regression.md)
- [Maximum likelihood estimation](maximum-likelihood-estimation-split.md)
- [Pairwise comparison model](pairwise-comparison-model.md)
- [Solution](past-exam-of-the-biochemistry-course-of-the-university-of-cambridge/2025/paper-1/section-ii/4/solution.md)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-1/4/c/solution.md)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-2/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-1/3d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-28/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-33/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-2/12h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-39/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-40/1/b/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-42/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-4/19d/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-45/3/vi/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-1/18c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-44/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48/6/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-4/19h/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-4/19h/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-2/5j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-42/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-38/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-1/28j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-32/2/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-32/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4/4j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-33/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-205/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207/3/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/28k/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207/4/c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207/4/c/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4/19h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/29j/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-1/19h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2/28j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-221/4/c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-342/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-207/5/b/solution.md)
- [Solution](past-exam-of-the-plant-sciences-course-of-the-university-of-cambridge/2025/paper-plm3/2/solution.md)
- [Poisson spike-train likelihood fitting](poisson-spike-train-likelihood-fitting.md)
- [Potential event time](potential-event-time.md)
- [Power law](power-law.md)
- [Statistical estimation](statistical-estimation.md)
- [Uniform-alternative binomial Bayes factor](uniform-alternative-binomial-bayes-factor.md)
