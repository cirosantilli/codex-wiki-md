# Wavelet regression estimator

↑ **Parent:** [Fixed-design nonparametric regression](fixed-design-nonparametric-regression.md)

At design sites $i/n$, let $\widetilde Y_n$ be the step function taking response $Y_i$ on $((i-1)/n,i/n]$. Project it onto an [interval-adapted wavelet basis](interval-adapted-wavelet-basis.md) through resolution $J$. Each coefficient is $\widehat c_\lambda=\sum_iY_i\int_{I_i}b_\lambda(t)dt$. Its [expectation](expected-value.md) is the corresponding coefficient of the step function of sampled regression means. For a [Haar wavelet](haar-wavelet.md) basis, dyadic sample size and resolution at most the sampling scale, this is exactly $n^{-1}\sum_iY_i b_\lambda(i/n)$ with right-closed pointwise versions. Independent errors of [variance](variance-split.md) $\sigma^2$ give coefficient variance at most $\sigma^2/n$: [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) on each sampling cell yields $\sum_i(\int_{I_i}b_\lambda)^2\leq\|b_\lambda\|_2^2/n$.

**Table of contents**

- [Wavelet coefficient thresholding](wavelet-coefficient-thresholding.md)
  - [Simultaneous wavelet coefficient noise bound](simultaneous-wavelet-coefficient-noise-bound.md)

## ↑ Ancestors (8)

1. [Fixed-design nonparametric regression](fixed-design-nonparametric-regression.md)
2. [Nonparametric regression](nonparametric-regression.md)
3. [Nonparametric statistics](nonparametric-statistics-split.md)
4. [Statistical inference](statistical-inference-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Discrete wavelet transform](discrete-wavelet-transform.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-31/3/solution.md)
