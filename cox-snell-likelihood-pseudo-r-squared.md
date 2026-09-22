<h1 id="cox-snell-likelihood-pseudo-r-squared">Cox–Snell likelihood pseudo-R-squared</h1>

↑ **Parent:** [Cox proportional-hazards model](cox-proportional-hazards-model.md)

A likelihood-based analogue of the [coefficient of determination](coefficient-of-determination.md) compares the fitted and intercept-only [log-likelihoods](log-likelihood.md) $\ell_1$ and $\ell_0$:

$$
R^2_{\mathrm{CS}}=1-\exp\left\{-\frac{2(\ell_1-\ell_0)}n\right\}.
$$

For a [Cox proportional-hazards model](cox-proportional-hazards-model.md), these are maximized [partial likelihood](partial-likelihood.md) logarithms with and without the [covariates](covariate.md). The expression measures improvement in fit, rather than the fraction of variation in event times explained. Its attainable maximum can be below one. It does not test the [proportional hazards](proportional-hazards-model.md) assumption or establish predictive calibration.

## ↑ Ancestors (6)

1. [Cox proportional-hazards model](cox-proportional-hazards-model.md)
2. [Survival analysis](survival-analysis-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-41/5/b/ii/solution.md)
