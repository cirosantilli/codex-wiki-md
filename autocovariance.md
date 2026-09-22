# Autocovariance

↑ **Parent:** [Weakly stationary process](weakly-stationary-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Autocovariance)

The [autocovariance](autocovariance.md) measures how two observations of the same [stochastic process](stochastic-process-split.md) vary together. For a real [weakly stationary process](weakly-stationary-process.md) of [mean](expected-value-split.md) $\mu$, it is

$$
\gamma(h)=\operatorname{Cov}(X_{t+h},X_t)
=\mathbb E[(X_{t+h}-\mu)(X_t-\mu)].
$$

Weak stationarity removes dependence on the absolute time $t$. Without it, the [covariance function](covariance-function.md) generally needs two time arguments. Lag zero is the [variance](variance-split.md), $\gamma(0)=\operatorname{Var}(X_t)$; symmetry of real [covariance](covariance.md) gives $\gamma(-h)=\gamma(h)$. Positive values favor deviations from the [mean](expected-value-split.md) in the same direction; negative values favor opposite directions. The units are the square of the observation units. See [Bartlett, lecture 2: autocovariance examples](https://www.stat.berkeley.edu/~bartlett/courses/153-fall2010/lectures/2.pdf).

For example, if $X_t=\varepsilon_t+\tfrac12\varepsilon_{t-1}$ with centered unit-[variance](variance-split.md) [white noise](white-noise.md), expanding the product leaves only matching noise times. Thus $\gamma(0)=1+1/4=5/4$, $\gamma(1)=1/2$, and $\gamma(h)=0$ for $|h|\ge2$. This [MA(1)](moving-average-process-of-order-one.md) has a positive lag-one [autocovariance](autocovariance.md) because adjacent observations share one disturbance. Rescaling every observation by $10$ multiplies every [autocovariance](autocovariance.md) by $100$, while leaving [autocorrelation](autocorrelation.md) unchanged.

The [autocovariance](autocovariance.md) is useful beyond comparing pairs: it determines the [variance](variance-split.md) of any finite linear combination of observations. For the [sample mean](sample-mean.md) $\overline X_n$,

$$
\operatorname{Var}(\overline X_n)=\frac{1}{n^2}\left[n\gamma(0)+2\sum_{h=1}^{n-1}(n-h)\gamma(h)\right].
$$

Each separation $h$ occurs in $n-h$ pairs. For the preceding [MA(1)](moving-average-process-of-order-one.md) and $n=4$, this is $[4(5/4)+2(3)(1/2)]/16=1/2$, compared with $5/16$ for four [uncorrelated random variables](uncorrelated-random-variables.md) of the same [variance](variance-split.md). This is the finite-record counterpart of the [long-run variance of a stationary process](long-run-variance-of-a-stationary-process.md).

**Table of contents**

- [Sample autocovariance function](sample-autocovariance-function.md)
- [Autocorrelation](autocorrelation.md)
  - [Correlation time](correlation-time.md)
  - [Partial autocorrelation function](partial-autocorrelation-function.md)
    - [Sample partial autocorrelation function](sample-partial-autocorrelation-function.md)
  - [Sample autocorrelation function](sample-autocorrelation-function.md)
    - [Correlogram](correlogram.md)

## ↑ Ancestors (7)

1. [Weakly stationary process](weakly-stationary-process.md)
2. [Stationary process](stationary-process.md)
3. [Time series](time-series-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (47)

- [Autocorrelation](autocorrelation.md)
- [Autocovariance](autocovariance.md)
- [Autocovariance of an AR(1) process](autocovariance-of-an-ar-1-process.md)
- [Autocovariance of an MA(1) process](autocovariance-of-an-ma-1-process.md)
- [Autocovariance tail recurrence of a causal ARMA process](autocovariance-tail-recurrence-of-a-causal-arma-process.md)
- [Existence of a time-series spectral density](existence-of-a-time-series-spectral-density.md)
- [Lag of a time series](lag-of-a-time-series.md)
- [Local-level state-space model](local-level-state-space-model.md)
- [Long-memory time series](long-memory-time-series.md)
- [Long-run variance of a stationary process](long-run-variance-of-a-stationary-process.md)
- [Moving-average process of order one](moving-average-process-of-order-one.md)
- [Noncausal stationary autoregression](noncausal-stationary-autoregression.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-43/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-29/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-29/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-36/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37/1/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37/1/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37/3/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208/2/2/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206/5/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218/5/a/solution.md)
- [Periodic Yule-Walker equations](periodic-yule-walker-equations.md)
- [Sample partial autocorrelation function](sample-partial-autocorrelation-function.md)
- [Short-memory time series](short-memory-time-series.md)
- [Shot noise departures from Poisson statistics](shot-noise-departures-from-poisson-statistics.md)
- [Shot noise spectral convention](shot-noise-spectral-convention.md)
- [Spectral density of a stationary process](spectral-density-of-a-stationary-process.md)
- [Spectral measure of a stationary time series](spectral-measure-of-a-stationary-time-series.md)
- [Spectral representation theorem for a stationary time series](spectral-representation-theorem-for-a-stationary-time-series.md)
- [Strong mixing of a stationary process](strong-mixing-of-a-stationary-process.md)
- [Time series](time-series-split.md)
- [Unnormalized time autocorrelation](unnormalized-time-autocorrelation.md)
- [Weak white noise](weak-white-noise.md)
- [Weakly stationary process](weakly-stationary-process.md)
- [White noise](white-noise.md)
- [Yule-Walker equations](yule-walker-equations.md)
- [Yule–Walker estimator for an autoregressive process of order one](yule-walker-estimator-for-an-autoregressive-process-of-order-one.md)
