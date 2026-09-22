# Gaussian filtering with exact observations

↑ **Parent:** [Kalman filter](kalman-filter.md)

In a linear [Gaussian](normal-distribution.md) [state-space model](state-space-model-time-series.md) with state noise [covariance](covariance.md) $Q$ and exact observation $X_t=FS_t$, the predictive state [covariance](covariance.md) includes $Q$ even though there is no separate observation noise. Its [innovation](innovation-process.md) [variance](variance-split.md) is $V_t=FGP_{t-1}G^\top F^\top+FQF^\top$. Omitting the second term incorrectly removes the current state noise. Conditioning gives the update $P_t=R_t-R_tF^\top FR_t/V_t$, which can be singular because the observed [linear combination](linear-combination.md) is then known exactly.

## ↑ Ancestors (6)

1. [Kalman filter](kalman-filter.md)
2. [State estimation](state-estimation.md)
3. [Control theory](control-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-33/4/solution.md)
