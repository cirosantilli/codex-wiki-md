# Autoregressive process of order one

↑ **Parent:** [Autoregressive model](autoregressive-model.md)

An [autoregressive process of order one](autoregressive-process-of-order-one.md) obeys

$$
X_t-\mu=\phi(X_{t-1}-\mu)+\varepsilon_t,
$$

where $\phi$ is real and $\varepsilon_t$ is centered [white noise](white-noise.md) of [variance](variance-split.md) $\sigma^2>0$. The zero-[mean](expected-value-split.md) version is $X_t=\phi X_{t-1}+\varepsilon_t$; in the affine form $X_t=c+\phi X_{t-1}+\varepsilon_t$, the stationary [mean](expected-value-split.md) satisfies $c=(1-\phi)\mu$.

For $|\phi|<1$, its unique [weakly stationary process](weakly-stationary-process.md) solution on all integer times is the [causal time-series representation](causal-time-series-representation.md)

$$
X_t=\mu+\sum_{j=0}^{\infty}\phi^j\varepsilon_{t-j}.
$$

The sum converges in the sense of [mean-square convergence](convergence-in-l2.md) because $\sum_{j\ge0}\phi^{2j}=1/(1-\phi^2)<\infty$. It is an [infinite moving-average representation](infinite-moving-average-representation.md) using only present and past driving noise. [Weak white noise](weak-white-noise.md) suffices for this second-order conclusion; [strong white noise](strong-white-noise.md) also gives [strict stationarity](strictly-stationary-process.md). The [autocovariance of an AR(1) process](autocovariance-of-an-ar-1-process.md) is $\sigma^2\phi^{|h|}/(1-\phi^2)$, so its [variance](variance-split.md) is $\sigma^2/(1-\phi^2)$ and its [ACF](autocorrelation.md) is $\phi^{|h|}$. See [Bartlett, lecture 5: AR(1) representation and causality](https://www.stat.berkeley.edu/~bartlett/courses/153-fall2010/lectures/5.pdf).

The appeal of an [AR(1)](autoregressive-process-of-order-one.md) is that one coefficient expresses how a deviation persists. For $0<\phi<1$, disturbances propagate with weights $1,\phi,\phi^2,\ldots$. For $-1<\phi<0$, these weights alternate sign. With $\mu=10$, $\phi=0.7$, and $X_t=12$, the [recursive forecasts of an autoregressive process](recursive-forecasts-of-an-autoregressive-process.md) give $11.4$ and $10.98$ one and two steps ahead. If $\sigma^2=1$, the stationary [variance](variance-split.md) is $100/51\simeq1.9608$, while the one-step forecast error [variance](variance-split.md) is only $1$. Under [weak white noise](weak-white-noise.md) these are best linear forecasts; independent driving noise also makes them [conditional expectations](conditional-expectation.md) given the observed past.

The condition $|\phi|<1$ describes a stationary causal solution, not every finite recursion with those coefficients. Starting from a prescribed value gives the transient in [finite initialization of an AR(1) process](finite-initialization-of-an-ar-1-process.md). Nor is it a condition for all possible two-sided stationary solutions: when $|\phi|>1$, [noncausal stationary autoregression](noncausal-stationary-autoregression.md) uses future driving noise. See [stationary versus causal solution of a two-sided AR(1) equation](stationary-versus-causal-solution-of-a-two-sided-ar-1-equation.md) for the boundary cases.

**Table of contents**

- [Autocovariance of an AR(1) process](autocovariance-of-an-ar-1-process.md)
- [Finite initialization of an AR(1) process](finite-initialization-of-an-ar-1-process.md)
- [Poisson-kernel expansion of an AR(1) spectrum](poisson-kernel-expansion-of-an-ar-1-spectrum.md)
- [Autocovariance of an AR(1) process observed with white noise](autocovariance-of-an-ar-1-process-observed-with-white-noise.md)
  - [Invertible ARMA factorization of an AR(1)-plus-noise process](invertible-arma-factorization-of-an-ar-1-plus-noise-process.md)
- [Stationary versus causal solution of a two-sided AR(1) equation](stationary-versus-causal-solution-of-a-two-sided-ar-1-equation.md)
- [Gaussian AR1 bridge](gaussian-ar1-bridge.md)
- [Stationary Gaussian AR1 likelihood](stationary-gaussian-ar1-likelihood.md)
  - [Conditional and stationary AR1 likelihood estimators](conditional-and-stationary-ar1-likelihood-estimators.md)
- [Yule–Walker estimator for an autoregressive process of order one](yule-walker-estimator-for-an-autoregressive-process-of-order-one.md)
- [Gaussian autoregressive conditional precision](gaussian-autoregressive-conditional-precision.md)

## ↑ Ancestors (7)

1. [Autoregressive model](autoregressive-model.md)
2. [Autoregressive moving-average model](autoregressive-moving-average-model.md)
3. [Time series](time-series-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (21)

- [Affine autoregressive process](affine-autoregressive-process.md)
- [Autoregressive process of order one](autoregressive-process-of-order-one.md)
- [Causal time series](causal-time-series.md)
- [Conditional and stationary AR1 likelihood estimators](conditional-and-stationary-ar1-likelihood-estimators.md)
- [EM for a missing observation in a Gaussian AR1 process](em-for-a-missing-observation-in-a-gaussian-ar1-process.md)
- [Exact sampling of an Ornstein-Uhlenbeck process](exact-sampling-of-an-ornstein-uhlenbeck-process.md)
- [Gaussian AR1 bridge](gaussian-ar1-bridge.md)
- [Gaussian autoregressive kernel variance correction](gaussian-autoregressive-kernel-variance-correction.md)
- [Gaussian Gibbs sweep autocorrelation](gaussian-gibbs-sweep-autocorrelation.md)
- [Logistic-normal regression with autoregressive random effects](logistic-normal-regression-with-autoregressive-random-effects.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-42/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-101/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-39/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-39/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-211/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-211/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-216/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-218/2/d/i/solution.md)
