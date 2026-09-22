# Gaussian Brownian drift filter

↑ **Parent:** [Innovation process](innovation-process.md)

Observe $Y_t=\lambda t+W_t$, with an independent [Gaussian random vector](gaussian-random-vector.md) $\lambda$ of mean $m_0$ and [covariance matrix](covariance-matrix.md) $V_0$. Its posterior is [Gaussian](normal-distribution.md) with mean $m_t=(I+tV_0)^{-1}(m_0+V_0Y_t)$ and [covariance matrix](covariance-matrix.md) $V_t=V_0(I+tV_0)^{-1}$. These formulas also hold for a singular [positive semidefinite matrix](positive-semidefinite-matrix.md) $V_0$. When $V_0$ is invertible, completing the square in the [Bayes' theorem](bayes-theorem.md) gives $V_t^{-1}=V_0^{-1}+tI$ and $m_t=V_t(V_0^{-1}m_0+Y_t)$. The observed [innovation process](innovation-process.md) $\widehat W_t=Y_t-\int_0^t m_sds$ is a [Brownian motion](brownian-motion-split.md) in the observation [filtration](filtration-probability-theory.md), and $dm_t=V_t\,d\widehat W_t$.

**Table of contents**

- [Innovation exponential for Gaussian drift filtering](innovation-exponential-for-gaussian-drift-filtering.md)
  - [Finite-horizon pricing density for Gaussian drift learning](finite-horizon-pricing-density-for-gaussian-drift-learning.md)
- [Brownian endpoint sufficiency for a constant drift](brownian-endpoint-sufficiency-for-a-constant-drift.md)

## ↑ Ancestors (6)

1. [Innovation process](innovation-process.md)
2. [Time series](time-series-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Finite-horizon pricing density for Gaussian drift learning](finite-horizon-pricing-density-for-gaussian-drift-learning.md)
- [Innovation exponential for Gaussian drift filtering](innovation-exponential-for-gaussian-drift-filtering.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-40/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-42/3/solution.md)
