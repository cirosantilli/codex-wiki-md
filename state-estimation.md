# State estimation

↑ **Parent:** [Control theory](control-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/State_estimation)

[State estimation](state-estimation.md) infers an unobserved state of a [dynamical system](dynamical-system.md) from its observations and a model of its evolution. An observed [position](position.md) can help estimate an unobserved [velocity](velocity.md); repeated noisy observations can help distinguish changes in the state from [measurement noise](measurement-noise.md). The result should describe both an estimate and its uncertainty. A [Kalman filter](kalman-filter.md) does this exactly for a linear [Gaussian](normal-distribution.md) [state-space model](state-space-model-time-series.md), maintaining a [conditional expectation](conditional-expectation.md) and [conditional covariance](conditional-covariance.md).

The time at which information is available matters. [Causal state filtering](causal-state-filtering.md) estimates the present state from observations available now. [State prediction](state-prediction.md) estimates a future state from those same observations. Later observations can improve an estimate of a past state, but that is a different information set from the one a live [controller](controller-control-theory.md) had. Kalman explicitly distinguishes these estimation tasks in [A New Approach to Linear Filtering and Prediction Problems (1960), section Optimal Estimates](https://www.cs.cmu.edu/~motionplanning/papers/sbp_papers/k/Kalman1960.pdf).

**Table of contents**

- [Causal state filtering](causal-state-filtering.md)
- [State prediction](state-prediction.md)
- [Process noise](process-noise.md)
- [Best affine state estimate](best-affine-state-estimate.md)
- [Kalman filter](kalman-filter.md)
  - [Kalman prediction step](kalman-prediction-step.md)
  - [Innovation covariance](innovation-covariance.md)
  - [Kalman gain](kalman-gain.md)
  - [Kalman measurement update](kalman-measurement-update.md)
  - [Gaussian filtering with exact observations](gaussian-filtering-with-exact-observations.md)
  - [Scalar Gaussian Kalman recursion](scalar-gaussian-kalman-recursion.md)
    - [Steady-state local-level Kalman gain](steady-state-local-level-kalman-gain.md)
  - [Scalar static-state Kalman update](scalar-static-state-kalman-update.md)
  - [Kalman filtering of a moving scalar state](kalman-filtering-of-a-moving-scalar-state.md)

## ↑ Ancestors (4)

1. [Control theory](control-theory-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [State estimation](state-estimation.md)
