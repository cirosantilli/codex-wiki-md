# Multivariate moving-average model

↑ **Parent:** [Moving-average model](moving-average-model.md)

A multivariate [moving-average model](moving-average-model.md) filters vector [white noise](white-noise.md) through fixed matrix coefficients. If the noise has zero [mean](expected-value.md) and lag-zero [covariance matrix](covariance-matrix.md) $D$, with all nonzero-lag cross-covariances zero, then the filtered process is a [weakly stationary process](weakly-stationary-process.md). With the convention $\Gamma(h)=\mathbb E[Z_tZ_{t+h}^T]$, its [covariance matrix](covariance-matrix.md) is $\Gamma(h)=\sum_j\Theta_jD\Theta_{j+h}^T$, omitting terms outside the filter range. Positive and negative lags satisfy $\Gamma(-h)=\Gamma(h)^T$.

**Table of contents**

- [Covariance and cross-spectrum of a vector MA(1)](covariance-and-cross-spectrum-of-a-vector-ma-1.md)

## ↑ Ancestors (7)

1. [Moving-average model](moving-average-model.md)
2. [Autoregressive moving-average model](autoregressive-moving-average-model.md)
3. [Time series](time-series-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48/2/solution.md)
