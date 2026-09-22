# Shared zero-inflated Gamma-Poisson count model

↑ **Parent:** [Zero-inflated negative binomial model](zero-inflated-negative-binomial-model.md)

Let $B=0$ with probability $\pi$, and otherwise let $B$ have a [Gamma distribution](gamma-distribution.md) with mean one and [variance](variance-split.md) $\tau$. Given $B$, counts $Y_j$ are [conditionally independent](conditional-independence.md) [Poisson random variables](poisson-distribution.md) with means $B\mu_j$. For $q=1-\pi$, the [law of total variance](law-of-total-variance.md) and [law of total covariance](law-of-total-covariance.md) give

$$
\mathbb EY_j=q\mu_j,\qquad\operatorname{Cov}(Y)=\operatorname{diag}(q\mu)+q(\tau+\pi)\mu\mu^T.
$$

Each component has a [zero-inflated negative binomial distribution](zero-inflated-negative-binomial-model.md), but the components are not independent after marginalizing $B$. The zero component is shared by the whole profile. At $\tau=0$, interpret the positive Gamma component as a [point mass](point-mass.md) at one.

**Table of contents**

- [Mean-ratio preservation under a multiplicative random effect](mean-ratio-preservation-under-a-multiplicative-random-effect.md)

## ↑ Ancestors (8)

1. [Zero-inflated negative binomial model](zero-inflated-negative-binomial-model.md)
2. [Zero inflation](zero-inflation.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Moment aliasing in a shared zero-inflated count model](moment-aliasing-in-a-shared-zero-inflated-count-model.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-37/6/a/solution.md)
