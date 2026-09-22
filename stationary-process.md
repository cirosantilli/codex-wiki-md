# Stationary process

↑ **Parent:** [Time series](time-series-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stationary_process)

A [stationary process](stationary-process.md), in the strict sense, has the same [joint probability distribution](joint-probability-distribution.md) after every common shift of its time indices. More precisely, for every positive integer $n$, every choice of times $t_1,\ldots,t_n$, and every integer shift $k$,

$$
(X_{t_1},\ldots,X_{t_n})\overset{d}{=}(X_{t_1+k},\ldots,X_{t_n+k}).
$$

Here equality means equality of [probability distributions](probability-distribution-split.md), not equality of realized observations. A [sample path](sample-path.md) can fluctuate, stay positive for a while, or show accidental runs while its generating law remains stationary. [Strong white noise](strong-white-noise.md) is a basic example: shifting time preserves every joint law of its [independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md).

The distinction between [strict stationarity](strictly-stationary-process.md) and [weak stationarity](weakly-stationary-process.md) is useful. The former preserves all finite joint laws; the latter preserves only the finite [mean](expected-value-split.md) and [covariance](covariance.md) structure. [Strict stationarity](strictly-stationary-process.md) with finite [second moments](second-moment.md) implies [weak stationarity](weakly-stationary-process.md), but strict stationarity itself does not require finite [variance](variance-split.md). A [Gaussian process](gaussian-process-split.md) with [weak stationarity](weakly-stationary-process.md) is also strictly stationary, because each of its [finite-dimensional distributions](finite-dimensional-distribution.md), a joint [normal distribution](normal-distribution.md), is determined by its [mean](expected-value-split.md) vector and [covariance matrix](covariance-matrix.md).

**Table of contents**

- [Strictly stationary process](strictly-stationary-process.md)
  - [Strong mixing of a stationary process](strong-mixing-of-a-stationary-process.md)
  - [Ergodic stationary process](ergodic-stationary-process.md)
- [Nonstationary process](nonstationary-process.md)
- [Weakly stationary process](weakly-stationary-process.md)
  - [Linear filter of a stationary time series](linear-filter-of-a-stationary-time-series.md)
    - [Filter generating function](filter-generating-function.md)
      - [Filter transfer function](filter-transfer-function.md)
    - [Composition of absolutely summable time-series filters](composition-of-absolutely-summable-time-series-filters.md)
    - [Filter gain](filter-gain.md)
    - [Spectral density transformation under a linear filter](spectral-density-transformation-under-a-linear-filter.md)
      - [Repeated symmetric filtering can amplify an oscillation](repeated-symmetric-filtering-can-amplify-an-oscillation.md)
  - [Spectral measure of a stationary time series](spectral-measure-of-a-stationary-time-series.md)
    - [Spectral measure of a random harmonic oscillation](spectral-measure-of-a-random-harmonic-oscillation.md)
    - [Spectral distribution function of a stationary time series](spectral-distribution-function-of-a-stationary-time-series.md)
  - [Spectral measure of a stationary random field](spectral-measure-of-a-stationary-random-field.md)
    - [Infinite-aperture spectral normalization](infinite-aperture-spectral-normalization.md)
  - [Long-run variance of a stationary process](long-run-variance-of-a-stationary-process.md)
    - [Effective sample size of a stationary sample](effective-sample-size-of-a-stationary-sample.md)
  - [Spectral density of a stationary process](spectral-density-of-a-stationary-process.md)
    - [Triangular spectral density of a stationary time series](triangular-spectral-density-of-a-stationary-time-series.md)
    - [Cross-spectrum of two stationary time series](cross-spectrum-of-two-stationary-time-series.md)
    - [One-sided spectral density of a real stationary time series](one-sided-spectral-density-of-a-real-stationary-time-series.md)
    - [Positive-frequency spectral normalization](positive-frequency-spectral-normalization.md)
    - [Existence of a time-series spectral density](existence-of-a-time-series-spectral-density.md)
    - [Cycles-per-time spectral density](cycles-per-time-spectral-density.md)
    - [Spectral representation theorem for a stationary time series](spectral-representation-theorem-for-a-stationary-time-series.md)
    - [Periodogram](periodogram.md)
      - [Exponential limit of a one-sided periodogram](exponential-limit-of-a-one-sided-periodogram.md)
      - [Finite-record Fourier covariance bound](finite-record-fourier-covariance-bound.md)
      - [Local periodogram smoothing](local-periodogram-smoothing.md)
  - [Autocovariance](autocovariance.md)
    - [Sample autocovariance function](sample-autocovariance-function.md)
    - [Autocorrelation](autocorrelation.md)
      - [Correlation time](correlation-time.md)
      - [Partial autocorrelation function](partial-autocorrelation-function.md)
        - [Sample partial autocorrelation function](sample-partial-autocorrelation-function.md)
      - [Sample autocorrelation function](sample-autocorrelation-function.md)
        - [Correlogram](correlogram.md)
  - [White noise](white-noise.md)
    - [Discrete Gaussian white noise](discrete-gaussian-white-noise.md)
    - [Continuous-time Gaussian white noise](continuous-time-gaussian-white-noise.md)
    - [Strong white noise](strong-white-noise.md)
    - [Weak white noise](weak-white-noise.md)

## ↑ Ancestors (5)

1. [Time series](time-series-split.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (18)

- [Autoregressive conditional heteroscedasticity](autoregressive-conditional-heteroscedasticity.md)
- [Bothe-Geiger coincidence experiment](bothe-geiger-coincidence-experiment.md)
- [Mean reversion](mean-reversion.md)
- [Mean-square derivative of a Gaussian process](mean-square-derivative-of-a-gaussian-process.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-30/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208/2/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-209/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-335/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202/3/iii/solution.md)
- [Poisson arrivals see time averages](poisson-arrivals-see-time-averages.md)
- [Queue population](queue-population.md)
- [Return period](return-period.md)
- [Same-noise stationary Ornstein-Uhlenbeck processes](same-noise-stationary-ornstein-uhlenbeck-processes.md)
- [Simple random walk](simple-random-walk.md)
- [Stationary drift saturation](stationary-drift-saturation.md)
- [Stationary increments](stationary-increments.md)
- [Stationary process](stationary-process.md)
