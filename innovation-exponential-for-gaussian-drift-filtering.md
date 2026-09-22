# Innovation exponential for Gaussian drift filtering

↑ **Parent:** [Gaussian Brownian drift filter](gaussian-brownian-drift-filter.md)

For the [Gaussian Brownian drift filter](gaussian-brownian-drift-filter.md) with positive definite $V_0$, define $Z_t=\det(I+tV_0)^{1/2}\exp[-m_t^TV_t^{-1}m_t/2+m_0^TV_0^{-1}m_0/2]$. Because $V_t'=-V_t^2$ and $dm_t=V_t\,d\widehat W_t$, the [Itô formula](ito-s-lemma.md) gives $d\log Z_t=-m_t^T\,d\widehat W_t-|m_t|^2dt/2$. Thus $Z$ is a positive [stochastic exponential](doleans-dade-exponential.md), hence a [nonnegative local martingale](nonnegative-local-martingale.md) and a [supermartingale](supermartingale.md). For a singular prior, the inverse-matrix expression is undefined; the same process can instead be defined by $Z_t=(\mathbb E_{\lambda\sim N(m_0,V_0)}\exp[\lambda^TY_t-t|\lambda|^2/2])^{-1}$, with $Y_t$ treated as fixed inside this Gaussian integral.

**Table of contents**

- [Finite-horizon pricing density for Gaussian drift learning](finite-horizon-pricing-density-for-gaussian-drift-learning.md)

## ↑ Ancestors (7)

1. [Gaussian Brownian drift filter](gaussian-brownian-drift-filter.md)
2. [Innovation process](innovation-process.md)
3. [Time series](time-series-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-42/3/solution.md)
