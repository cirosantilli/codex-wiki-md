# Kalman prediction step

↑ **Parent:** [Kalman filter](kalman-filter.md)

The [Kalman prediction step](kalman-prediction-step.md) advances the previous [posterior mean](posterior-mean.md) and [posterior covariance matrix](posterior-covariance-matrix.md) through the state transition:

$$
m_t^-=A_tm_{t-1}+B_tu_{t-1},\qquad
P_t^-=A_tP_{t-1}A_t^\top+Q_t.
$$

The minus superscript marks information before observing $y_t$. The [transpose](transpose.md) and [matrix multiplication](matrix-multiplication.md) propagate the old uncertainty; $Q_t$ adds the uncertainty of the new [process noise](process-noise.md). A known [control input](control-input.md) changes the mean but contributes no additional [variance](variance-split.md). If the [control input](control-input.md) itself is uncertain, that uncertainty needs its own model.

## ↑ Ancestors (6)

1. [Kalman filter](kalman-filter.md)
2. [State estimation](state-estimation.md)
3. [Control theory](control-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Kalman filter](kalman-filter.md)
- [Kalman filtering of a moving scalar state](kalman-filtering-of-a-moving-scalar-state.md)
- [Kalman prediction step](kalman-prediction-step.md)
- [Scalar static-state Kalman update](scalar-static-state-kalman-update.md)
- [State prediction](state-prediction.md)
