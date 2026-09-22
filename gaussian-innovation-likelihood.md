# Gaussian innovation likelihood

↑ **Parent:** [State-space model (time series)](state-space-model-time-series.md)

In a linear [Gaussian](normal-distribution.md) [state-space model](state-space-model-time-series.md), let the predicted state mean and [covariance](covariance.md) be $m_t^-,P_t^-$. The observation [innovation process](innovation-process.md) has conditional mean zero and [covariance](covariance.md) $\Sigma_t=AP_t^-A^\top+R$, with innovation $\epsilon_t=y_t-Am_t^-$. The [conditional multivariate normal distribution](conditional-multivariate-normal-distribution.md) gives the predictive observation density. Multiplying these conditional densities by the chain rule gives the displayed [likelihood function](likelihood-function.md); equivalently the innovations are independent [Gaussian](normal-distribution.md) vectors. The [Kalman filter](kalman-filter.md) supplies $m_t^-,P_t^-$ recursively, so one evaluates the exact observed-data [likelihood function](likelihood-function.md) without integrating all latent states jointly.

## ↑ Ancestors (6)

1. [State-space model (time series)](state-space-model-time-series.md)
2. [Time series](time-series-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-33/2/solution.md)
