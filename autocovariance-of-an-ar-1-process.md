<h1 id="autocovariance-of-an-ar-1-process">Autocovariance of an AR(1) process</h1>

↑ **Parent:** [Autoregressive process of order one](autoregressive-process-of-order-one.md)

For the stationary causal [AR(1)](autoregressive-process-of-order-one.md) with $|\phi|<1$, matching terms in its [infinite moving-average representation](infinite-moving-average-representation.md) gives, for $h\ge0$,

$$
\gamma(h)=\sigma^2\sum_{j=0}^{\infty}\phi^j\phi^{j+h}
=\frac{\sigma^2\phi^h}{1-\phi^2}.
$$

Symmetry of the [autocovariance](autocovariance.md) extends this to negative lags. Dividing by $\gamma(0)$ gives the [autocorrelation](autocorrelation.md) $\rho(h)=\phi^{|h|}$. The [geometric series](geometric-series.md) explains both the enlarged stationary [variance](variance-split.md) and the diminishing memory: all past disturbances contribute to the present, but their squared weights have a finite sum. At $\phi=0$, the process reduces to shifted [white noise](white-noise.md) and all nonzero-lag [autocorrelations](autocorrelation.md) vanish. See [Bartlett, lecture 4: AR(1) representation and mean-square convergence](https://www.stat.berkeley.edu/~bartlett/courses/153-fall2010/lectures/4.pdf).

## ↑ Ancestors (8)

1. [Autoregressive process of order one](autoregressive-process-of-order-one.md)
2. [Autoregressive model](autoregressive-model.md)
3. [Autoregressive moving-average model](autoregressive-moving-average-model.md)
4. [Time series](time-series-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Autoregressive process of order one](autoregressive-process-of-order-one.md)
