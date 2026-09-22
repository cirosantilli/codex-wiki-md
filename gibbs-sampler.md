# Gibbs sampler

↑ **Parent:** [Markov chain Monte Carlo](markov-chain-monte-carlo.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gibbs_sampler)

For a joint density $f_{XY}$, a two-coordinate Gibbs update draws

$$
Y_m\sim f_{Y\mid X}(\,\cdot\mid X_{m-1}),
\qquad
X_m\sim f_{X\mid Y}(\,\cdot\mid Y_m).
$$

**Table of contents**

- [Gaussian Gibbs sweep autocorrelation](gaussian-gibbs-sweep-autocorrelation.md)
- [Gaussian two-coordinate Gibbs recursion](gaussian-two-coordinate-gibbs-recursion.md)
- [WinBUGS](winbugs.md)
- [Linear contraction of a two-coordinate Gaussian Gibbs sweep](linear-contraction-of-a-two-coordinate-gaussian-gibbs-sweep.md)
- [Gibbs sampling for a finite hidden spin field](gibbs-sampling-for-a-finite-hidden-spin-field.md)
  - [Local likelihood factors in a hidden spin field](local-likelihood-factors-in-a-hidden-spin-field.md)
- [Systematic Gibbs sampling need not be reversible](systematic-gibbs-sampling-need-not-be-reversible.md)
- [Blocked Gibbs sampler](blocked-gibbs-sampler.md)
  - [Checkerboard Gibbs sampling](checkerboard-gibbs-sampling.md)
- [Random-scan Gibbs sampler](random-scan-gibbs-sampler.md)
  - [Detailed balance of a random-scan Gibbs sampler](detailed-balance-of-a-random-scan-gibbs-sampler.md)
- [Tempered Gibbs sampler](tempered-gibbs-sampler.md)
- [Stationarity of the two-coordinate Gibbs sampler](stationarity-of-the-two-coordinate-gibbs-sampler.md)
- [Normal mean-precision Gibbs sampler](normal-mean-precision-gibbs-sampler.md)

## ↑ Ancestors (7)

1. [Markov chain Monte Carlo](markov-chain-monte-carlo.md)
2. [Bayesian statistics](bayesian-statistics.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (46)

- [Data augmentation](data-augmentation.md)
- [Detailed balance of a random-scan Gibbs sampler](detailed-balance-of-a-random-scan-gibbs-sampler.md)
- [Empty component under an improper prior](empty-component-under-an-improper-prior.md)
- [Full conditional distribution](full-conditional-distribution.md)
- [Gaussian change-point Gibbs updates](gaussian-change-point-gibbs-updates.md)
- [Gaussian–exponential hierarchical colour model](gaussian-exponential-hierarchical-colour-model.md)
- [Gaussian Gibbs sweep autocorrelation](gaussian-gibbs-sweep-autocorrelation.md)
- [Gibbs updates for a Poisson count change point](gibbs-updates-for-a-poisson-count-change-point.md)
- [Improper posterior from a log-uniform random-effect scale prior](improper-posterior-from-a-log-uniform-random-effect-scale-prior.md)
- [Independent normal and inverse-gamma regression priors](independent-normal-and-inverse-gamma-regression-priors.md)
- [Log-gamma prior for a Poisson log-intercept](log-gamma-prior-for-a-poisson-log-intercept.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-33/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/3/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/3/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/4/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-43/3/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-43/3/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-43/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-43/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-40/5/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48/5/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-44/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/5/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/5/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40/6/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-33/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-38/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-36/3/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208/4/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208/6/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-219/4/iii/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-219/4/iii/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-216/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-219/4/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-219/3/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-219/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-216/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-207/3/c/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-4/28l/b/solution.md)
