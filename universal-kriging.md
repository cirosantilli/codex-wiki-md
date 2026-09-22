# Universal kriging

↑ **Parent:** [Kriging](kriging.md)

For unknown drift $X\beta$, a full-column-rank [design matrix](design-matrix.md) $X$, a known [positive-definite matrix](positive-definite-matrix.md) observation [covariance matrix](covariance-matrix.md) $\Sigma$, and target drift row $x_0^T$, universal kriging minimizes prediction [variance](variance-split.md) subject to $X^Tw=x_0$. Equivalently, with $\widehat\beta=(X^T\Sigma^{-1}X)^{-1}X^T\Sigma^{-1}z$, predict $x_0^T\widehat\beta+c^T\Sigma^{-1}(z-X\widehat\beta)$. The first term is the estimated trend alone; the second is a correlated residual prediction.

## ↑ Ancestors (8)

1. [Kriging](kriging.md)
2. [Geostatistics](geostatistics.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Best linear unbiased estimator](best-linear-unbiased-estimator.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206/6/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206/6/e/solution.md)
