# Kalman gain

↑ **Parent:** [Kalman filter](kalman-filter.md)

The [Kalman gain](kalman-gain.md) maps an observation [innovation](innovation-process.md) into a state correction:

$$
K_t=P_t^-H_t^\top S_t^{-1}.
$$

For a scalar state observed directly, it reduces to $K=P^-/(P^-+R)$. With positive [variances](variance-split.md), $0<K<1$, and the [Kalman measurement update](kalman-measurement-update.md) is the [weighted mean](weighted-arithmetic-mean.md) $(1-K)m^-+Ky$. That interpretation belongs to the scalar unit-coefficient case; a general [Kalman gain](kalman-gain.md) is a rectangular [matrix](matrix.md), not a collection of weights necessarily between zero and one.

## ↑ Ancestors (6)

1. [Kalman filter](kalman-filter.md)
2. [State estimation](state-estimation.md)
3. [Control theory](control-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Gaussian filtering with exact observations](gaussian-filtering-with-exact-observations.md)
- [Kalman filter](kalman-filter.md)
- [Kalman filtering of a moving scalar state](kalman-filtering-of-a-moving-scalar-state.md)
- [Kalman gain](kalman-gain.md)
- [Kalman measurement update](kalman-measurement-update.md)
- [Scalar Gaussian Kalman recursion](scalar-gaussian-kalman-recursion.md)
- [Scalar static-state Kalman update](scalar-static-state-kalman-update.md)
