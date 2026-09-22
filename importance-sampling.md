# Importance sampling

↑ **Parent:** [Monte Carlo method](monte-carlo-method-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Importance_sampling)

To estimate $\mathbb E_f[g(X)]$, sample $Y_1,\ldots,Y_m$ independently from a reference density $h$ whose support covers that of $gf$, and use

$$
\frac1m\sum_{i=1}^m g(Y_i)\frac{f(Y_i)}{h(Y_i)}.
$$

The summands have expectation $\int g(x)f(x)\,dx$, and the [strong law of large numbers](strong-law-of-large-numbers.md) gives almost-sure convergence under integrability.

**Table of contents**

- [Optimal normal shift for normal-tail importance sampling](optimal-normal-shift-for-normal-tail-importance-sampling.md)
- [Normal variance mismatch in importance sampling](normal-variance-mismatch-in-importance-sampling.md)
- [Likelihood weighting](likelihood-weighting.md)
- [Reciprocal importance sampling](reciprocal-importance-sampling.md)
- [Importance sampling of a Cauchy tail](importance-sampling-of-a-cauchy-tail.md)
- [Rao-Blackwell identity for a fixed-denominator rejection estimator](rao-blackwell-identity-for-a-fixed-denominator-rejection-estimator.md)
- [Bounded-weight importance-sampling moment bound](bounded-weight-importance-sampling-moment-bound.md)
- [Minimum-variance importance distribution](minimum-variance-importance-distribution.md)
- [Support condition for importance sampling](support-condition-for-importance-sampling.md)
- [Importance weight](importance-weight.md)
- [Self-normalized importance sampling](self-normalized-importance-sampling.md)
- [Optimal importance density for a single integral](optimal-importance-density-for-a-single-integral.md)
- [Effective sample size of importance sampling](effective-sample-size-of-importance-sampling.md)

## ↑ Ancestors (5)

1. [Monte Carlo method](monte-carlo-method-split.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (38)

- [Change of measure](change-of-measure.md)
- [Importance sampling of a Cauchy tail](importance-sampling-of-a-cauchy-tail.md)
- [Minimum-variance importance distribution](minimum-variance-importance-distribution.md)
- [Solution](past-exam-of-the-advanced-topics-in-statistical-machine-learning-course-of-the-university-of-oxford/2025/1/a/i/solution.md)
- [Solution](past-exam-of-the-advanced-topics-in-statistical-machine-learning-course-of-the-university-of-oxford/2025/1/b/iv/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/7/b/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/7/c/solution.md)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/7/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/2/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-40/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-40/4/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-40/4/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-45/3/vi/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-33/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-36/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-36/4/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-219/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/28k/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-219/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-219/4/e/solution.md)
- [Solution](past-exam-of-the-msc-in-advanced-computer-science-course-of-the-university-of-oxford/2021/bayesian-statistical-probabilistic-programming/2/a/solution.md)
- [Solution](past-exam-of-the-msc-in-advanced-computer-science-course-of-the-university-of-oxford/2021/bayesian-statistical-probabilistic-programming/3/e/solution.md)
- [Solution](past-exam-of-the-probability-statistics-and-options-i-course-of-the-university-of-oxford/2008/s/1/a/solution.md)
- [Solution](past-exam-of-the-simulation-and-statistical-programming-course-of-the-university-of-oxford/2021/1/d/ii/solution.md)
- [Solution](past-exam-of-the-simulation-and-statistical-programming-course-of-the-university-of-oxford/2023/1/c/i/solution.md)
- [Solution](past-exam-of-the-simulation-and-statistical-programming-course-of-the-university-of-oxford/2023/1/c/ii/solution.md)
- [Solution](past-exam-of-the-simulation-and-statistical-programming-course-of-the-university-of-oxford/2023/2/a/iii/solution.md)
- [Probabilistic programming](probabilistic-programming.md)
- [Reciprocal importance sampling](reciprocal-importance-sampling.md)
- [Rejected-proposal distribution](rejected-proposal-distribution.md)
- [Support condition for importance sampling](support-condition-for-importance-sampling.md)
- [Unbiased likelihood estimator](unbiased-likelihood-estimator.md)
