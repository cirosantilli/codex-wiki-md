# Kalman measurement update

↑ **Parent:** [Kalman filter](kalman-filter.md)

The [Kalman measurement update](kalman-measurement-update.md) incorporates the new observation by [Gaussian conditional expectation](gaussian-conditional-expectation.md):

$$
m_t=m_t^-+K_t(y_t-H_tm_t^-),\qquad
P_t=P_t^--K_tS_tK_t^\top.
$$

The [posterior covariance matrix](posterior-covariance-matrix.md) subtracts a [positive semidefinite matrix](positive-semidefinite-matrix.md), reflecting the information supplied by the measurement. Even if the [innovation](innovation-process.md) is zero and the mean does not move, the uncertainty can decrease. In this linear [Gaussian](normal-distribution.md) model the [posterior covariance matrix](posterior-covariance-matrix.md) depends on the observation geometry and its uncertainty, rather than on the numerical observed value.

The derivation is one application of [Gaussian conditional expectation](gaussian-conditional-expectation.md) per measurement. Before observing $y_t$, the state and observation have joint [covariance matrix](covariance-matrix.md)

$$
\operatorname{Cov}\begin{pmatrix}x_t\\y_t\end{pmatrix}
=
\begin{pmatrix}
P_t^-&P_t^-H_t^\top\\
H_tP_t^-&S_t
\end{pmatrix}.
$$

Conditioning the upper block on the lower block gives exactly the two update equations. The upper-right block explains the [Kalman gain](kalman-gain.md): a measured component corrects a state component only to the extent that their prediction errors have [covariance](covariance.md). The measurement can therefore improve an unobserved [velocity](velocity.md) when a [state-space model](state-space-model-time-series.md) correlates its error with an observed [position](position.md).

## ↑ Ancestors (6)

1. [Kalman filter](kalman-filter.md)
2. [State estimation](state-estimation.md)
3. [Control theory](control-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Kalman filter](kalman-filter.md)
- [Kalman gain](kalman-gain.md)
- [Kalman measurement update](kalman-measurement-update.md)
