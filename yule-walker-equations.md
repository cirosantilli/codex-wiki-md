# Yule-Walker equations

↑ **Parent:** [Autoregressive model](autoregressive-model.md)

For a causal [autoregressive model](autoregressive-model.md) $X_t=\sum_{j=1}^p\phi_jX_{t-j}+\epsilon_t$ with centered [white noise](white-noise.md) of [variance](variance-split.md) $\sigma^2$, multiplying by past values and taking [expectations](expected-value.md) yields $\gamma(h)=\sum_j\phi_j\gamma(h-j)$ for $h\geq1$, and $\gamma(0)=\sum_j\phi_j\gamma(j)+\sigma^2$. These [Yule-Walker equations](yule-walker-equations.md) determine the [autocovariance](autocovariance.md) from the coefficients and noise [variance](variance-split.md), or estimate coefficients from observed [autocovariances](autocovariance.md). Causality supplies the needed orthogonality of the current noise to past observations.

## ↑ Ancestors (7)

1. [Autoregressive model](autoregressive-model.md)
2. [Autoregressive moving-average model](autoregressive-moving-average-model.md)
3. [Time series](time-series-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-40/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/1/solution.md)
- [Yule-Walker equations](yule-walker-equations.md)
