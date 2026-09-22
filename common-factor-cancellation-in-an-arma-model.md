# Common factor cancellation in an ARMA model

↑ **Parent:** [Autoregressive moving-average model](autoregressive-moving-average-model.md)

An [ARMA](autoregressive-moving-average-model.md) equation need not be a minimal-order representation when its [autoregressive polynomial](autoregressive-polynomial.md) and [moving-average polynomial](moving-average-polynomial.md) have a common factor. For a stationary causal solution, a common stable factor can be cancelled using its convergent inverse filter. For example, $(1-0.5B)X=(1-0.5B)(1-0.9B)W$ reduces to $X=(1-0.9B)W$, an MA(1). Its [autocorrelation function](autocorrelation.md) vanishes beyond lag one, despite the displayed ARMA(1,2) equation. Root conditions should be applied to a reduced representation when asserting necessary and sufficient [causality and invertibility root criteria for an ARMA model](causality-and-invertibility-root-criteria-for-an-arma-model.md).

## ↑ Ancestors (6)

1. [Autoregressive moving-average model](autoregressive-moving-average-model.md)
2. [Time series](time-series-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [ARMA(1,1) causal and inverse coefficients](arma-1-1-causal-and-inverse-coefficients.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-33/1/i/solution.md)
