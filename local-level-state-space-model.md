# Local-level state-space model

↑ **Parent:** [State-space model (time series)](state-space-model-time-series.md)

The latent state follows a [random walk](random-walk.md), while observations add [independent](independent-random-variables.md) measurement noise. If the two noises have [variances](variance-split.md) $W,V$, the differences have [autocovariances](autocovariance.md) $W+2V$ at lag zero, $-V$ at lag one, and zero at larger lags. For $V,W>0$, write $q=(W+2V+\sqrt{W^2+4WV})/2$ and $\vartheta=-V/q$. The differenced process is an invertible [moving-average model](moving-average-model.md) with coefficient $\vartheta$ and innovation [variance](variance-split.md) $q$. Its level has a unit root.

## ↑ Ancestors (6)

1. [State-space model (time series)](state-space-model-time-series.md)
2. [Time series](time-series-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-40/2/a/solution.md)
