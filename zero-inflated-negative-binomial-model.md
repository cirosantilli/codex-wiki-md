# Zero-inflated negative binomial model

↑ **Parent:** [Zero inflation](zero-inflation.md)

With structural-zero probability $\pi$, size $r>0$ and count mean $\lambda$, the model assigns $\pi+(1-\pi)(r/(r+\lambda))^r$ to zero and $(1-\pi)f_{\rm NB}(y;r,\lambda)$ to positive counts. Its [expectation](expected-value.md) is $(1-\pi)\lambda$ and its [variance](variance-split.md) is $(1-\pi)(\lambda+\lambda^2/r)+\pi(1-\pi)\lambda^2$, by the [law of total variance](law-of-total-variance.md). A [logarithmic link function](logarithmic-link-function.md) can relate the count-component mean to predictors.

**Table of contents**

- [Shared zero-inflated Gamma-Poisson count model](shared-zero-inflated-gamma-poisson-count-model.md)
  - [Mean-ratio preservation under a multiplicative random effect](mean-ratio-preservation-under-a-multiplicative-random-effect.md)
- [EM for zero-inflated negative binomial regression](em-for-zero-inflated-negative-binomial-regression.md)

## ↑ Ancestors (7)

1. [Zero inflation](zero-inflation.md)
2. [Statistical modelling](statistical-modelling-split.md)
3. [Statistical model](statistical-model-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206/1/f/solution.md)
