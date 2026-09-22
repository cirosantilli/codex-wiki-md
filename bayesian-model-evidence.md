# Bayesian model evidence

↑ **Parent:** [Bayesian statistics](bayesian-statistics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bayesian_model_evidence)

The [Bayesian model evidence](bayesian-model-evidence.md) is the [prior predictive distribution](bayesian-model-evidence.md) evaluated at the data $D$. For a [statistical model](statistical-model-split.md) $H_j$ with a normalized [prior density](prior-density.md) $\pi_j$, its [marginal likelihood](bayesian-model-evidence.md) is

$$
m_j(D)=p(D\mid H_j)=\mathcal Z_j
=\int p(D\mid\theta_j,H_j)\pi_j(\theta_j\mid H_j)\,d\theta_j.
$$

This is an [expected value](expected-value-split.md) of the [likelihood function](likelihood-function.md) under the [prior distribution](prior-probability.md); for discrete [statistical parameters](statistical-parameter.md), replace the [integral](integral-split.md) by a sum. For continuous observations, $m_j(D)$ is a [probability density function](probability-density-function.md) value with respect to a specified data reference measure, rather than a [probability](probability.md) of one exact observation. Comparisons must use the same data and reference measure. The same $m_j(D)$ normalizes the within-model [Bayesian posterior](bayesian-posterior.md) and supplies the between-model comparison in a [Bayes factor](bayes-factor.md).[Kass and Raftery, Bayes Factors (1995), section 3.1, p. 776, equations (1)–(2): integrating over parameter priors](bayes-factors-by-robert-e-kass-and-adrian-e-raftery.md)

A normalized [prior distribution](prior-probability.md) makes the [Bayesian model evidence](bayesian-model-evidence.md) an average, so it cannot exceed the largest [likelihood function](likelihood-function.md) value on its support. A broad [prior distribution](prior-probability.md) can assign little mass to values that predict the data well, even when one value gives an excellent fit. The worked [uniform-alternative binomial Bayes factor](uniform-alternative-binomial-bayes-factor.md) below makes the difference between averaging and [maximum likelihood estimation](maximum-likelihood-estimation-split.md) explicit.

**Table of contents**

- [Evidence averaging under an interval prior](evidence-averaging-under-an-interval-prior.md)
  - [Laplace-likelihood interval evidence](laplace-likelihood-interval-evidence.md)
- [Prior predictive check](prior-predictive-check.md)
- [Harmonic mean estimator of Bayesian model evidence](harmonic-mean-estimator-of-bayesian-model-evidence.md)
- [Bayes factor](bayes-factor.md)
  - [Uniform-alternative binomial Bayes factor](uniform-alternative-binomial-bayes-factor.md)
  - [Gaussian practical-null mixture](gaussian-practical-null-mixture.md)
  - [Savage-Dickey density ratio](savage-dickey-density-ratio.md)

## ↑ Ancestors (6)

1. [Bayesian statistics](bayesian-statistics-split.md)
2. [Statistical inference](statistical-inference-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (22)

- [Bayes factor](bayes-factor.md)
- [Bayesian model evidence](bayesian-model-evidence.md)
- [Bayesian network structure score](bayesian-network-structure-score.md)
- [Bayesian posterior](bayesian-posterior.md)
- [Evidence averaging under an interval prior](evidence-averaging-under-an-interval-prior.md)
- [Nuisance parameter](nuisance-parameter.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-45/3/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-36/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-36/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-34/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-34/1/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-34/1/g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-34/4/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207/2/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-350/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/28j/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-219/4/a/solution.md)
- [Prequential log score identity](prequential-log-score-identity.md)
- [Uniform-alternative binomial Bayes factor](uniform-alternative-binomial-bayes-factor.md)
- [Uniform-Pareto model evidence](uniform-pareto-model-evidence.md)
