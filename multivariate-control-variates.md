# Multivariate control variates

↑ **Parent:** [Control variates](control-variates.md)

If $Y$ is an unbiased estimator and a vector $C$ has known mean, then $Y-\beta^T(C-\mathbb EC)$ remains unbiased for a deterministic coefficient vector. Its variance is $\operatorname{Var}Y-2\beta^T c+\beta^T\Sigma\beta$, where $c=\operatorname{Cov}(C,Y)$ and $\Sigma=\operatorname{Cov}(C)$. For invertible $\Sigma$, completing the square gives the displayed optimum and minimum variance $\operatorname{Var}Y-c^T\Sigma^{-1}c$. With singular $\Sigma$, use a generalized inverse on its range. Estimating coefficients from the same simulation can introduce finite-sample bias; fixed pilot coefficients or independent training preserve the elementary unbiasedness assertion.

## ↑ Ancestors (7)

1. [Control variates](control-variates.md)
2. [Monte Carlo estimator](monte-carlo-estimator.md)
3. [Monte Carlo method](monte-carlo-method.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-47/4/c/solution.md)
