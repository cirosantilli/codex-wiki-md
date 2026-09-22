# Moving-average process of order one

↑ **Parent:** [Moving-average model](moving-average-model.md)

A [moving-average process of order one](moving-average-process-of-order-one.md) has the form

$$
X_t=\mu+\varepsilon_t+\theta\varepsilon_{t-1},\qquad \theta\in\mathbb R,
$$

with centered [white noise](white-noise.md) of finite positive [variance](variance-split.md) $\sigma^2$. Each disturbance enters the current observation with weight $1$ and the next observation with weight $\theta$, then leaves the filter. It is a [weakly stationary process](weakly-stationary-process.md) for every real $\theta$: the [mean](expected-value.md) is $\mu$ and the [autocovariance of an MA(1) process](autocovariance-of-an-ma-1-process.md) depends only on lag. [Strong white noise](strong-white-noise.md) additionally makes it a [strictly stationary process](strictly-stationary-process.md). No $|\theta|<1$ restriction is needed for stationarity.

For a worked observation calculation, take $\mu=10$, $\theta=0.7$, and consecutive noise values $\varepsilon_{t-1}=-1$, $\varepsilon_t=2$, $\varepsilon_{t+1}=0$. Then $X_t=11.3$ and $X_{t+1}=11.4$; the same disturbance $2$ appears in both. If $\sigma^2=1$, the [variance](variance-split.md) is $1.49$, the lag-one [autocovariance](autocovariance.md) is $0.7$, and the lag-one [autocorrelation](autocorrelation.md) is $70/149\simeq0.4698$. All higher-lag [autocorrelations](autocorrelation.md) vanish, as shown in [autocorrelation](autocorrelation.md).

An [MA(1)](moving-average-process-of-order-one.md) is useful for brief dependence caused by overlapping disturbances or measurements. Its name refers to a weighted moving sum of noise; its weights need not be positive or sum to one, and it differs from the data smoother in [seasonal extraction by a centred moving average](seasonal-extraction-by-a-centred-moving-average.md). Under [strong white noise](strong-white-noise.md), observations more than one interval apart depend on disjoint independent noise families and are [independent](independent-random-variables.md). Under [weak white noise](weak-white-noise.md), the same cutoff establishes only [uncorrelated random variables](uncorrelated-random-variables.md).

[Invertibility of a moving-average model](invertibility-of-a-moving-average-model.md) is a separate question: can the specified driving noise be recovered by a stable linear filter of present and past observations? For an [MA(1)](moving-average-process-of-order-one.md) the answer, with the absolutely summable filter convention, is exactly $|\theta|<1$:

$$
\varepsilon_t=\sum_{j=0}^{\infty}(-\theta)^j(X_{t-j}-\mu).
$$

Thus $\theta=2$ gives a stationary [MA(1)](moving-average-process-of-order-one.md) that is not invertible in this sense. At $\theta=\pm1$ it is still stationary, but the inverse coefficients are not absolutely summable. The case $\theta=0$ is simply shifted [white noise](white-noise.md). See [Bartlett, lecture 5: MA(1) and stable invertibility](https://www.stat.berkeley.edu/~bartlett/courses/153-fall2010/lectures/5.pdf).

**Table of contents**

- [Autocovariance of an MA(1) process](autocovariance-of-an-ma-1-process.md)

## ↑ Ancestors (7)

1. [Moving-average model](moving-average-model.md)
2. [Autoregressive moving-average model](autoregressive-moving-average-model.md)
3. [Time series](time-series-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Moving-average process of order one](moving-average-process-of-order-one.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206/5/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206/5/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-218/6/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-218/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-218/2/d/iv/solution.md)
