# Innovation covariance

↑ **Parent:** [Kalman filter](kalman-filter.md)

For the [Kalman filter](kalman-filter.md) model, the [innovation](innovation-process.md) is $e_t=y_t-H_tm_t^-$. Its conditional [covariance matrix](covariance-matrix.md) before the measurement is

$$
S_t=H_tP_t^-H_t^\top+R_t.
$$

This includes uncertainty in both the predicted state and the [measurement noise](measurement-noise.md). It is a [covariance](covariance.md) in observation coordinates; $P_t^-$ is a [covariance](covariance.md) in state coordinates, and need not even have the same dimensions.

## ↑ Ancestors (6)

1. [Kalman filter](kalman-filter.md)
2. [State estimation](state-estimation.md)
3. [Control theory](control-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Kalman filter](kalman-filter.md)
