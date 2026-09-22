# Scalar Gaussian Kalman recursion

↑ **Parent:** [Kalman filter](kalman-filter.md)

For the [state-space model](state-space-model-time-series.md) $S_t=GS_{t-1}+w_t$, $X_t=FS_t+v_t$, assume [independent](independent-random-variables.md) [Gaussian](normal-distribution.md) [process noise](process-noise.md) and [measurement noise](measurement-noise.md) of [variances](variance-split.md) $W,V$, independent of the prior state and previous observations. A [normal distribution](normal-distribution.md) for the filtered state, with mean $m$ and [variance](variance-split.md) $P$, predicts mean $Gm$ and [variance](variance-split.md) $R=G^2P+W$. Here $R$ denotes predicted state [variance](variance-split.md), rather than the observation-noise [covariance](covariance.md) notation used in the vector equations above. [Gaussian conditional expectation](gaussian-conditional-expectation.md) then gives [posterior mean](posterior-mean.md) $Gm+K(X-FGm)$ and [posterior variance](posterior-variance.md) $RV/(F^2R+V)$, where the [Kalman gain](kalman-gain.md) is $K=FR/(F^2R+V)$.

Mere [weak white noise](weak-white-noise.md) assumptions do not imply [normal](normal-distribution.md) [posterior distributions](bayesian-posterior.md): [independent](independent-random-variables.md) [process noise](process-noise.md) with a [Rademacher distribution](rademacher-distribution.md) makes the next state a [mixture](mixture.md) of two shifted [normal distributions](normal-distribution.md). The [Kalman filter](kalman-filter.md) can still describe a [best affine state estimate](best-affine-state-estimate.md) under appropriate second-order assumptions, but that is distinct from an exact [Gaussian](normal-distribution.md) conditional law.

**Table of contents**

- [Steady-state local-level Kalman gain](steady-state-local-level-kalman-gain.md)

## ↑ Ancestors (6)

1. [Kalman filter](kalman-filter.md)
2. [State estimation](state-estimation.md)
3. [Control theory](control-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-40/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40/2/solution.md)
