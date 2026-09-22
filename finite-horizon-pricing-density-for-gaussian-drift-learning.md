# Finite-horizon pricing density for Gaussian drift learning

↑ **Parent:** [Innovation exponential for Gaussian drift filtering](innovation-exponential-for-gaussian-drift-filtering.md)

For the [Gaussian Brownian drift filter](gaussian-brownian-drift-filter.md) $Y_t=\alpha t+W_t$, with independent prior $\alpha\sim N(m_0,\tau_0^{-1})$, the observation law has density

$$
L_t(y)=\sqrt{\frac{\tau_0}{\tau_0+t}}\exp\left(\frac{(\tau_0m_0+y)^2}{2(\tau_0+t)}-\frac{\tau_0m_0^2}{2}\right)
$$

relative to driftless [Wiener measure](wiener-measure.md). The law having fixed observation drift $k$ has density $e^{kY_t-k^2t/2}$ relative to the same reference. Their ratio is therefore a positive mean-one density on every finite horizon. In the observation [filtration](filtration-probability-theory.md) it satisfies $dD_t=-D_t(m_t-k)d\widehat W_t$, where $m_t$ is the posterior mean and $\widehat W$ the [innovation process](innovation-process.md). This density-ratio argument establishes a true [martingale](martingale-split.md) without an unsupported global [Novikov condition](novikov-s-condition.md) for the unbounded posterior mean.

## ↑ Ancestors (8)

1. [Innovation exponential for Gaussian drift filtering](innovation-exponential-for-gaussian-drift-filtering.md)
2. [Gaussian Brownian drift filter](gaussian-brownian-drift-filter.md)
3. [Innovation process](innovation-process.md)
4. [Time series](time-series-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Log-optimal investment with Gaussian drift learning](log-optimal-investment-with-gaussian-drift-learning.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-40/3/solution.md)
