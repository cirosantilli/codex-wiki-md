# Rejection sampling

↑ **Parent:** [Monte Carlo method](monte-carlo-method.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rejection_sampling)

Suppose $f$ is a target probability density and $h$ is a proposal density with $f(x)\leq Mh(x)$. Draw $X\sim h$ and an independent $U\sim\operatorname{Uniform}[0,1]$, and accept $X$ when

$$
U\leq\frac{f(X)}{Mh(X)}.
$$

The accepted value has density $f$, the acceptance probability is $1/M$, and the expected number of proposals is $M$.

**Table of contents**

- [Acceptance mass for an unnormalized rejection envelope](acceptance-mass-for-an-unnormalized-rejection-envelope.md)
- [Truncated gamma rejection sampling with a Pareto envelope](truncated-gamma-rejection-sampling-with-a-pareto-envelope.md)
- [Uniform-envelope rejection sampling for a beta distribution](uniform-envelope-rejection-sampling-for-a-beta-distribution.md)
- [Bayesian rejection sampling for a segregating-site count](bayesian-rejection-sampling-for-a-segregating-site-count.md)
  - [Joint posterior of mutation rate and coalescent times](joint-posterior-of-mutation-rate-and-coalescent-times.md)
- [Match-biased reshuffling preserves uniform rank marginals](match-biased-reshuffling-preserves-uniform-rank-marginals.md)
- [Exponential-envelope rejection sampling for a chi-squared variable](exponential-envelope-rejection-sampling-for-a-chi-squared-variable.md)
- [Ratio-of-uniforms method](ratio-of-uniforms-method.md)
  - [Laplace ratio-of-uniforms envelope](laplace-ratio-of-uniforms-envelope.md)
  - [Normal ratio-of-uniforms envelope](normal-ratio-of-uniforms-envelope.md)
  - [Finite-area envelope for a ratio-of-uniforms region](finite-area-envelope-for-a-ratio-of-uniforms-region.md)
- [Normal rejection sampling with an exponential envelope](normal-rejection-sampling-with-an-exponential-envelope.md)
- [Marsaglia polar method](marsaglia-polar-method.md)
- [Binomial count and iid values in fixed-budget rejection sampling](binomial-count-and-iid-values-in-fixed-budget-rejection-sampling.md)
  - [Random-count central limit theorem for accepted rejection samples](random-count-central-limit-theorem-for-accepted-rejection-samples.md)
- [Rejected-proposal distribution](rejected-proposal-distribution.md)
- [Adaptive rejection sampling](adaptive-rejection-sampling.md)

## ↑ Ancestors (5)

1. [Monte Carlo method](monte-carlo-method.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (21)

- [Exponential-envelope rejection sampling for a chi-squared variable](exponential-envelope-rejection-sampling-for-a-chi-squared-variable.md)
- [Log-concave probability density](log-concave-probability-density.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/1/a/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-43/1/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-43/1/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-45/3/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-2/11f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-47/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/3/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-33/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-32/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-36/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-216/3/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4/28k/b/solution.md)
- [Ratio-of-uniforms method](ratio-of-uniforms-method.md)
- [Symmetric rational mixture sampler](symmetric-rational-mixture-sampler.md)
