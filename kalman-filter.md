# Kalman filter

↑ **Parent:** [State estimation](state-estimation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kalman_filter)

The [Kalman filter](kalman-filter.md) alternates a [Kalman prediction step](kalman-prediction-step.md) with a [Kalman measurement update](kalman-measurement-update.md). It carries a state estimate forward using a [state-space model](state-space-model-time-series.md), then adjusts it by the part of the new observation that was not predicted: the [innovation](innovation-process.md). The [Kalman gain](kalman-gain.md) determines the adjustment from the uncertainty of the prediction and the [measurement noise](measurement-noise.md). A noisy measurement should have less influence than an equally surprising precise one.

For a precise discrete-time statement, let the state and observation be [vectors](vector.md) in [real vector spaces](real-vector-space.md) obeying the linear [state-space model](state-space-model-time-series.md)

$$
x_t=A_tx_{t-1}+B_tu_{t-1}+w_t,\qquad
y_t=H_tx_t+v_t.
$$

The [matrices](matrix.md) and [control inputs](control-input.md) are known. Assume a [Gaussian random vector](gaussian-random-vector.md) $x_0$ with mean $m_0$ and [covariance matrix](covariance-matrix.md) $P_0$, and mutually [independent](independent-random-variables.md) centered [Gaussian](normal-distribution.md) noises $w_t,v_t$, independent of $x_0$, with [covariance matrices](covariance-matrix.md) $Q_t,R_t$. Suppose $R_t$ is [positive-definite](positive-definite-bilinear-form.md), so the observation [innovation covariance](innovation-covariance.md) is invertible. Then the recursions below give the exact [posterior mean](posterior-mean.md) $m_t=\mathbb E[x_t\mid y_1,\ldots,y_t]$ and [posterior covariance matrix](posterior-covariance-matrix.md) $P_t$, hence the full [conditional multivariate normal distribution](conditional-multivariate-normal-distribution.md). They also minimize [mean squared error](mean-squared-error.md). Without the [Gaussian](normal-distribution.md) assumptions, suitable second-order assumptions still give [best affine state estimates](best-affine-state-estimate.md), but do not generally give an exact [posterior distribution](bayesian-posterior.md). [Welch and Bishop, An Introduction to the Kalman Filter, section 1, UNC technical report TR 95-041, 2004 revision](https://www.cs.utexas.edu/~pstone/Courses/393Rfall15/readings/Welch%2BBishop-TR-95.pdf).

For an exact scalar example, suppose the predicted state has [normal distribution](normal-distribution.md) $N(10,4)$ and a measurement reports $y=14$ in the same units. With [measurement noise](measurement-noise.md) [variance](variance-split.md) $R=1$, the [Kalman gain](kalman-gain.md) is $4/(4+1)=4/5$ and the [posterior distribution](bayesian-posterior.md) is

$$
x\mid y=14\sim N(13.2,0.8).
$$

With the same prediction and observed value but [measurement noise](measurement-noise.md) [variance](variance-split.md) $R=16$, the [Kalman gain](kalman-gain.md) becomes $1/5$ and the [posterior distribution](bayesian-posterior.md) is instead $N(10.8,3.2)$. Both updates move toward the observation; the more precise measurement moves the estimate further and reduces uncertainty more.

<a id="image-the-same-observed-value-produces-different-kalman-measurement-updates-when-its-uncertainty-changes"></a>
![](kalman-measurement-uncertainty.png)

**[Figure 9](#image-the-same-observed-value-produces-different-kalman-measurement-updates-when-its-uncertainty-changes). The same observed value produces different Kalman measurement updates when its uncertainty changes**. Both panels start from $N(10,4)$ and observe $14$. The green curve is the [likelihood function](likelihood-function.md) normalized over the scalar state for this unit-coefficient observation model. The orange curve is the [posterior density](posterior-density.md); its narrower width reflects reduced [variance](variance-split.md). The vertical dotted line marks the observed value, rather than a known true state.

The useful compression is exact under the stated model: the two objects $m_t,P_t$ contain everything from the past observations needed for the next update. Their size depends on the state dimension, not on the length of the observation history. This makes [causal state filtering](causal-state-filtering.md) practical when observations arrive continually. It also gives [Linear-quadratic-Gaussian control](linear-quadratic-gaussian-control.md) an estimate of the state on which to act.

Rudolf E. Kalman's 1960 paper organized linear filtering around state transitions, error [covariance](covariance.md) and recursive computation, connecting estimation with optimal regulation. Its introduction acknowledges earlier work by Wiener, Bode, Shannon and others; the useful historical claim is this particular formulation, rather than that estimation began in 1960. [Kalman, A New Approach to Linear Filtering and Prediction Problems, Journal of Basic Engineering 82 (1960), pp. 35–45](https://www.cs.cmu.edu/~motionplanning/papers/sbp_papers/k/Kalman1960.pdf).

**Table of contents**

- [Kalman prediction step](kalman-prediction-step.md)
- [Innovation covariance](innovation-covariance.md)
- [Kalman gain](kalman-gain.md)
- [Kalman measurement update](kalman-measurement-update.md)
- [Gaussian filtering with exact observations](gaussian-filtering-with-exact-observations.md)
- [Scalar Gaussian Kalman recursion](scalar-gaussian-kalman-recursion.md)
  - [Steady-state local-level Kalman gain](steady-state-local-level-kalman-gain.md)
- [Scalar static-state Kalman update](scalar-static-state-kalman-update.md)
- [Kalman filtering of a moving scalar state](kalman-filtering-of-a-moving-scalar-state.md)

## ↑ Ancestors (5)

1. [State estimation](state-estimation.md)
2. [Control theory](control-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (16)

- [Causal state filtering](causal-state-filtering.md)
- [Gaussian filtering with exact observations](gaussian-filtering-with-exact-observations.md)
- [Gaussian innovation likelihood](gaussian-innovation-likelihood.md)
- [Innovation covariance](innovation-covariance.md)
- [Kalman filter](kalman-filter.md)
- [Kalman filtering of a moving scalar state](kalman-filtering-of-a-moving-scalar-state.md)
- [Linear-quadratic-Gaussian control](linear-quadratic-gaussian-control.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-33/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2/29j/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2/29j/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-33/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/30k/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/30k/c/solution.md)
- [Scalar Gaussian Kalman recursion](scalar-gaussian-kalman-recursion.md)
- [State estimation](state-estimation.md)
