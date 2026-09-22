# Mixture model

↑ **Parent:** [Statistical modelling](statistical-modelling-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mixture_model)

A mixture model represents a population [probability distribution](probability-distribution-split.md) by choosing one [mixture component](mixture-component.md) at random and then drawing from its [probability distribution](probability-distribution-split.md). For a [finite mixture model](finite-mixture-model.md) whose [mixture components](mixture-component.md) have [probability density functions](probability-density-function.md) $f_j$, the resulting [mixture distribution](mixture-distribution.md) has [probability density function](probability-density-function.md)

$$
f(x)=\sum_{j=1}^K\pi_jf_j(x),\qquad \pi_j\geq0,\qquad \sum_{j=1}^K\pi_j=1.
$$

The [mixture weights](mixture-weight.md) ensure $f\geq0$ and $\int f(x)\,dx=\sum_j\pi_j=1$. For [discrete random variables](discrete-random-variable.md) the same formula uses [probability mass functions](probability-mass-function.md); without either kind of density, write $\mathbb P(X\in A)=\sum_j\pi_jP_j(A)$ for [component distributions](mixture-component.md) $P_j$. A zero [mixture weight](mixture-weight.md) makes that [mixture component](mixture-component.md) inactive.[Finite Mixtures, sections Latent discrete parameterization and Summing out the responsibility parameter: nonnegative normalized weights, categorical labels, and the sum of weighted normal densities](stan-user-s-guide-by-stan-development-team/finite-mixtures.md)

The [mixture components](mixture-component.md) need not occupy disjoint bins of $x$. Two [normal distributions](normal-distribution.md) both have positive [probability density functions](probability-density-function.md) everywhere, so the same value can plausibly come from either [mixture component](mixture-component.md). The [Two-Gaussian mixture example](two-gaussian-mixture-example.md) makes this overlap visible, and its [mixture responsibilities](mixture-responsibility.md) quantify the remaining uncertainty about the [latent variable](latent-variable-split.md). This is useful when a single [normal distribution](normal-distribution.md) cannot represent the population's shape, but a fitted [mixture model](mixture-model.md) alone does not establish that its [mixture components](mixture-component.md) are real biological or social groups.

**Table of contents**

- [Threshold inference for a mixture proportion](threshold-inference-for-a-mixture-proportion.md)
- [Gaussian scale mixture](gaussian-scale-mixture.md)
  - [Rayleigh-normal scale mixture](rayleigh-normal-scale-mixture.md)
- [Finite mixture model](finite-mixture-model.md)
  - [Mixture component](mixture-component.md)
  - [Mixture allocation indicator](mixture-allocation-indicator.md)
  - [Two-Gaussian mixture example](two-gaussian-mixture-example.md)
  - [Observed and latent mixture labels](observed-and-latent-mixture-labels.md)
  - [Mixture identifiability](mixture-identifiability.md)
  - [Label switching](label-switching.md)
  - [Gaussian mixture Gibbs updates with independent priors](gaussian-mixture-gibbs-updates-with-independent-priors.md)
  - [Mixture responsibility](mixture-responsibility.md)
    - [Responsibility curve for a two-Gaussian mixture](responsibility-curve-for-a-two-gaussian-mixture.md)
  - [Finite Gaussian mixture with a common variance](finite-gaussian-mixture-with-a-common-variance.md)
    - [Mixture regression with shared slopes](mixture-regression-with-shared-slopes.md)
    - [Residual mixture clustering](residual-mixture-clustering.md)
      - [Two-stage residual mixture fitting](two-stage-residual-mixture-fitting.md)
    - [EM for Gaussian mixtures with a common variance](em-for-gaussian-mixtures-with-a-common-variance.md)
  - [Mixture weight](mixture-weight.md)
- [Dirichlet process mixture model](dirichlet-process-mixture-model.md)

## ↑ Ancestors (6)

1. [Statistical modelling](statistical-modelling-split.md)
2. [Statistical model](statistical-model-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (15)

- [Chi-squared testing lower bound](chi-squared-testing-lower-bound.md)
- [EM likelihood monotonicity](em-likelihood-monotonicity.md)
- [Mixture model](mixture-model.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-36/4/g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-33/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35/3/g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35/3/h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-2/3f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-210/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-210/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-210/2/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216/1/c/solution.md)
- [Second moment of a mixture likelihood ratio](second-moment-of-a-mixture-likelihood-ratio.md)
- [Threshold inference for a mixture proportion](threshold-inference-for-a-mixture-proportion.md)
- [Two-stage residual mixture fitting](two-stage-residual-mixture-fitting.md)
