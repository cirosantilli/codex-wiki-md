# Steady-state local-level Kalman gain

↑ **Parent:** [Scalar Gaussian Kalman recursion](scalar-gaussian-kalman-recursion.md)

For the [state-space model](state-space-model-time-series.md) with both scalar coefficients equal to one, $\alpha_t=(P_{t-1}+W)/(P_{t-1}+W+V)$ and $P_t=\alpha_tV$. If the variance converges and $c=W/V$, its limiting gain satisfies $\alpha^2+c\alpha-c=0$. The nonnegative root lies below one for finite $c>0$; it tends to zero with $c$ and to one as $c$ grows. Thus noisier state evolution assigns more weight to the latest observation.

## ↑ Ancestors (7)

1. [Scalar Gaussian Kalman recursion](scalar-gaussian-kalman-recursion.md)
2. [Kalman filter](kalman-filter.md)
3. [State estimation](state-estimation.md)
4. [Control theory](control-theory-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Exponential smoothing](exponential-smoothing.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-40/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40/2/solution.md)
