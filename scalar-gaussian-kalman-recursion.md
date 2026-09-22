# Scalar Gaussian Kalman recursion

↑ **Parent:** [Kalman filter](kalman-filter.md)

For $S_t=GS_{t-1}+w_t$ and $X_t=FS_t+v_t$, assume independent Gaussian process and observation noises, independent of the prior state and previous observations. A normal filtering law with mean $m$ and variance $P$ predicts mean $Gm$ and variance $R=G^2P+W$. Gaussian conditioning then gives posterior mean $Gm+K(X-FGm)$ and variance $RV/(F^2R+V)$. Mere [weak white noise](weak-white-noise.md) assumptions do not imply normal posterior laws: independent Rademacher process noise makes the next state a mixture of two shifted normal distributions. The [Kalman filter](kalman-filter.md) can still describe a best linear predictor under appropriate second-order assumptions, but that is distinct from an exact Gaussian conditional law.

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
