# Ornstein-Uhlenbeck process

↑ **Parent:** [Gaussian process](gaussian-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ornstein–Uhlenbeck_process)

An Ornstein-Uhlenbeck process combines [mean reversion](mean-reversion.md) with continuing random fluctuations. In the scalar model, its [stochastic differential equation](stochastic-differential-equation.md) is

$$
dX_t=-\theta(X_t-\mu)\,dt+\sigma\,dW_t,\qquad \theta>0,\quad \sigma>0,\quad \mu\in\mathbb R,
$$

where $W$ is a standard [Brownian motion](brownian-motion-split.md). The [drift](drift-coefficient.md) points towards $\mu$: it is negative above $\mu$ and positive below it. The coefficient $\theta$ sets the speed of [mean reversion](mean-reversion.md), while $\sigma$ sets the strength of the random forcing. We consider a fixed or [normal](normal-distribution.md) initial value independent of future [Brownian increments](brownian-increment.md), giving a [Gaussian process](gaussian-process.md) and a [Markov process](markov-process-split.md).

For a stipulated example, use $\theta=1$, $\mu=2$, $\sigma=\sqrt2$ and the fixed initial value $X_0=6$, in arbitrary consistent state and time units. Then the [expected value](expected-value.md) relaxes as $2+4e^{-t}$ and the [variance](variance-split.md) grows as $1-e^{-2t}$. At time one they are about $3.4715$ and $0.8647$; the limiting [variance](variance-split.md) is one. The [sample paths](sample-path.md) keep fluctuating even after the [expected value](expected-value.md) is close to two. The [Ornstein-Uhlenbeck transition distribution](ornstein-uhlenbeck-transition-distribution.md) describes this evolving uncertainty; [Ornstein-Uhlenbeck stationary initialization](ornstein-uhlenbeck-stationary-initialization.md) instead starts with that limiting [normal distribution](normal-distribution.md) already in place.

A physical motivation is the [velocity](velocity.md) of a particle undergoing [Brownian motion](brownian-motion-split.md): [linear drag](linear-drag.md) removes a persistent initial [velocity](velocity.md), while random forcing continually renews it. The original calculation gives a [normal distribution](normal-distribution.md) for the [velocity](velocity.md) after subtracting its exponentially decaying initial contribution, with decay rate equal to the friction coefficient divided by the particle's [mass](mass.md).[On the Theory of the Brownian Motion, abstract: velocity minus its decaying initial contribution; friction coefficient divided by mass](on-the-theory-of-the-brownian-motion-by-g-e-uhlenbeck-and-l-s-ornstein.md) A position coordinate in an overdamped [harmonic optical trap](harmonic-optical-trap.md) gives another interpretation of the same scalar equation, with $\theta=k/\zeta$ for [spring constant](spring-constant.md) $k$ and drag coefficient $\zeta$. Its physical assumptions and connection to measurements are developed in [thermal calibration of an optical trap](thermal-calibration-of-an-optical-trap.md).

**Table of contents**

- [Ornstein-Uhlenbeck transition distribution](ornstein-uhlenbeck-transition-distribution.md)
- [Ornstein-Uhlenbeck stationary initialization](ornstein-uhlenbeck-stationary-initialization.md)
- [Exact sampling of an Ornstein-Uhlenbeck process](exact-sampling-of-an-ornstein-uhlenbeck-process.md)
- [Stationary drift saturation](stationary-drift-saturation.md)
  - [Same-noise stationary Ornstein-Uhlenbeck processes](same-noise-stationary-ornstein-uhlenbeck-processes.md)
- [Exponential Brownian time change to a stationary Ornstein-Uhlenbeck process](exponential-brownian-time-change-to-a-stationary-ornstein-uhlenbeck-process.md)
- [Ornstein-Uhlenbeck stochastic differential equation](ornstein-uhlenbeck-stochastic-differential-equation.md)
- [Ornstein-Uhlenbeck multiplicative amplification](ornstein-uhlenbeck-multiplicative-amplification.md)
  - [Tilted Ornstein-Uhlenbeck oscillator transformation](tilted-ornstein-uhlenbeck-oscillator-transformation.md)
- [Integrated Ornstein-Uhlenbeck displacement](integrated-ornstein-uhlenbeck-displacement.md)
- [Explicit Ornstein-Uhlenbeck solution](explicit-ornstein-uhlenbeck-solution.md)
  - [Zero-start Ornstein-Uhlenbeck covariance](zero-start-ornstein-uhlenbeck-covariance.md)
- [Multivariate Ornstein-Uhlenbeck process](multivariate-ornstein-uhlenbeck-process.md)
  - [Ornstein-Uhlenbeck power spectrum](ornstein-uhlenbeck-power-spectrum.md)
- [Colored noise](colored-noise.md)

## ↑ Ancestors (7)

1. [Gaussian process](gaussian-process.md)
2. [Stochastic process](stochastic-process-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (49)

- [Continuous-time autoregressive residual correlation](continuous-time-autoregressive-residual-correlation.md)
- [Exponential Brownian time change to a stationary Ornstein-Uhlenbeck process](exponential-brownian-time-change-to-a-stationary-ornstein-uhlenbeck-process.md)
- [Exponential covariance function](exponential-covariance-function.md)
- [Gaussian Model A quench](gaussian-model-a-quench.md)
- [Gaussian volatility exponential-quadratic transform](gaussian-volatility-exponential-quadratic-transform.md)
- [Hull-White model](hull-white-model.md)
- [Intrawell phase autocorrelation](intrawell-phase-autocorrelation.md)
- [Linear fluctuating interface](linear-fluctuating-interface.md)
- [Mean reversion](mean-reversion.md)
- [Ornstein-Uhlenbeck fluctuation limit at a stable population equilibrium](ornstein-uhlenbeck-fluctuation-limit-at-a-stable-population-equilibrium.md)
- [Ornstein-Uhlenbeck Fokker-Planck equation](ornstein-uhlenbeck-fokker-planck-equation.md)
- [Ornstein-Uhlenbeck semigroup](ornstein-uhlenbeck-semigroup.md)
- [Ornstein-Uhlenbeck stationary initialization](ornstein-uhlenbeck-stationary-initialization.md)
- [Ornstein-Uhlenbeck transition distribution](ornstein-uhlenbeck-transition-distribution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-51/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-32/6/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-30/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-48/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-39/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-69/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-81/4/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-29/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-43/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-39/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-75/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-344/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-344/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202/3/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-219/3/i/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-344/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-219/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-344/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1/6b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1/6b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-344/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-202/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-219/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-216/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-344/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-344/3/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-219/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-219/3/a/solution.md)
- [Quadratic Ornstein-Uhlenbeck state-price density](quadratic-ornstein-uhlenbeck-state-price-density.md)
- [Same-noise stationary Ornstein-Uhlenbeck processes](same-noise-stationary-ornstein-uhlenbeck-processes.md)
- [Square root of a CIR diffusion](square-root-of-a-cir-diffusion.md)
- [Stationary Gaussian forward curve](stationary-gaussian-forward-curve.md)
- [Vasicek model](vasicek-model.md)
- [Weak-noise relaxation of gyrotactic alignment](weak-noise-relaxation-of-gyrotactic-alignment.md)
- [Zero-start Ornstein-Uhlenbeck covariance](zero-start-ornstein-uhlenbeck-covariance.md)
