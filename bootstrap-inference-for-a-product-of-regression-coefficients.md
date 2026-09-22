# Bootstrap inference for a product of regression coefficients

↑ **Parent:** [Bootstrap confidence interval](bootstrap-confidence-interval.md)

For $\theta=\beta_1\beta_2$, use $\widehat\theta=\widehat\beta_1\widehat\beta_2$. Under regular regression assumptions, the [delta method](delta-method.md) gives [standard error](standard-error.md) $\widehat s=(d^\top\widehat Vd)^{1/2}$, where $d=(\widehat\beta_2,\widehat\beta_1)^\top$ and $\widehat V$ estimates the [covariance](covariance.md) of the regression estimate. Resample the observational units, refit, and compute both $\widehat\theta^*$ and $\widehat s^*$. A [percentile bootstrap confidence interval](percentile-bootstrap-confidence-interval.md) uses the .025 and .975 [quantiles](quantile-function.md) of $\widehat\theta^*$. A [bootstrap-t confidence interval](bootstrap-t-confidence-interval.md) uses [quantiles](quantile-function.md) of $(\widehat\theta^*-\widehat\theta)/\widehat s^*$ and reverses them when solving for $\theta$. If both true coefficients vanish, the first derivative is zero and the standard first-order justification is unavailable; product-specific nonregular inference is then needed.

## ↑ Ancestors (8)

1. [Bootstrap confidence interval](bootstrap-confidence-interval.md)
2. [Bootstrapping (statistics)](bootstrapping-statistics.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47/4/b/solution.md)
