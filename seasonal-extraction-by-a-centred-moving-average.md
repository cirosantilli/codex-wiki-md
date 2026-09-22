# Seasonal extraction by a centred moving average

↑ **Parent:** [Seasonality](seasonality.md)

For an additive [time series](time-series-split.md) $X_t=T_t+S_t+\varepsilon_t$ with period-$m$ seasonal component and $\sum_{j=1}^mS_j=0$, a centred average spanning one complete period removes the seasonal component while estimating the slowly varying trend. When $m$ is even, average two adjacent length-$m$ averages to centre the filter on an observation; the endpoints receive half the usual weights. Estimate each seasonal phase by averaging the corresponding detrended residuals across cycles, then subtract the mean of those phase averages to enforce the zero-sum convention. Multiplicative seasonality instead uses ratios and a mean-one convention. Repeated averaging is filter composition and induces serial dependence even from [white noise](white-noise.md).

## ↑ Ancestors (6)

1. [Seasonality](seasonality.md)
2. [Time series](time-series-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/5/solution.md)
