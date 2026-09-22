<h1 id="finite-initialization-of-an-ar-1-process">Finite initialization of an AR(1) process</h1>

↑ **Parent:** [Autoregressive process of order one](autoregressive-process-of-order-one.md)

For $t\ge1$, iterating an [AR(1)](autoregressive-process-of-order-one.md) from a fixed value $X_0=x_0$ gives the displayed finite sum. With centered [white noise](white-noise.md) of [variance](variance-split.md) $\sigma^2$ and $|\phi|<1$,

$$
\mathbb E[X_t]=\mu+\phi^t(x_0-\mu),\qquad
\operatorname{Var}(X_t)=\frac{\sigma^2(1-\phi^{2t})}{1-\phi^2}.
$$

For $h\ge0$, its [covariance](covariance.md) is $\operatorname{Cov}(X_{t+h},X_t)=\phi^h\operatorname{Var}(X_t)$, which depends on $t$. Even setting $x_0=\mu$ leaves a changing [variance](variance-split.md). At $\phi=0.7$, $\sigma^2=1$, and $x_0=\mu$, the [variances](variance-split.md) at times zero through three are $0,1,1.49,1.7301$, approaching $100/51$; this finite initialized record is not weakly stationary.

To initialize in [weak stationarity](weakly-stationary-process.md), give $X_0$ [mean](expected-value-split.md) $\mu$, [variance](variance-split.md) $\sigma^2/(1-\phi^2)$, and zero [covariance](covariance.md) with every future driving noise value. The full stationary construction sets $X_0-\mu=\sum_{j\ge0}\phi^j\varepsilon_{-j}$. For [discrete Gaussian white noise](discrete-gaussian-white-noise.md), equivalently draw $X_0$ from $N(\mu,\sigma^2/(1-\phi^2))$ independently of future noise. This gives exact [strict stationarity](strictly-stationary-process.md) from the first plotted point; it is the initialization used in the figure in [time series](time-series-split.md). Matching these first two moments alone does not guarantee [strict stationarity](strictly-stationary-process.md) for non-Gaussian inputs. See also [stationary initialization of a scalar linear state-space model](stationary-initialization-of-a-scalar-linear-state-space-model.md).

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
