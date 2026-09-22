# Common versus factor-specific slopes in Poisson regression

↑ **Parent:** [Poisson regression](poisson-regression.md)

For a continuous predictor $x$ and a categorical [factor](regression-factor.md), an additive [Poisson regression](poisson-regression.md) with [log link](logarithmic-link-function.md) has $\log\mu_j(x)=a_j+b x$. The log-mean curves are parallel and $\mu_j(x)/\mu_k(x)=e^{a_j-a_k}$ is constant in $x$. Adding a predictor-by-factor [interaction](interaction-statistics.md) gives $\log\mu_j(x)=a_j+b_jx$, so this ratio becomes $e^{a_j-a_k+(b_j-b_k)x}$. With $J$ factor levels, the common-slope restriction has $J-1$ independent constraints. A [likelihood-ratio test](likelihood-ratio-test.md) compares the two [deviances](exponential-family-deviance.md) with an asymptotic [chi-squared distribution](chi-squared-distribution.md) on $J-1$ [degrees of freedom](degree-of-freedom.md). Evidence against common slopes establishes varying effects on the log scale; it does not by itself determine their signs or the ordering of the mean curves.

## ↑ Ancestors (8)

1. [Poisson regression](poisson-regression.md)
2. [Generalized linear model](generalized-linear-model.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-41/3/solution.md)
