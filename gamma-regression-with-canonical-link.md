# Gamma regression with canonical link

↑ **Parent:** [Generalized linear model](generalized-linear-model.md)

For a [Gamma distribution](gamma-distribution.md) with fixed shape $\alpha$, choose dispersion $\phi=1/\alpha$, canonical parameter $\theta=-1/\mu$, and cumulant $b(\theta)=-\log(-\theta)$. The [canonical link function](canonical-link-function.md) is the displayed negative reciprocal; reversing its sign is an equivalent regression convention. For independent observations, the [score function](informant-function.md) is $\phi^{-1}X^T(y-\mu)$ and the [Fisher information matrix](fisher-information-matrix.md) is $\phi^{-1}X^T\operatorname{diag}(\mu_i^2)X$. The [deviance](exponential-family-deviance.md) is $2\sum_i[y_i/\widehat\mu_i-1-\log(y_i/\widehat\mu_i)]$, with twice the log-likelihood ratio equal to this divided by $\phi$. The fitted mean is the inverse link applied to $X\widehat\beta$, not $X\widehat\beta$ itself.

## ↑ Ancestors (7)

1. [Generalized linear model](generalized-linear-model.md)
2. [Statistical modelling](statistical-modelling-split.md)
3. [Statistical model](statistical-model-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-4/13i/solution.md)
