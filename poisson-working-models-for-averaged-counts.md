# Poisson working models for averaged counts

↑ **Parent:** [Poisson regression](poisson-regression.md)

If $C_i\sim\operatorname{Poisson}(T_i\lambda_i)$ counts events over $T_i$ days, then the daily average $C_i/T_i$ has mean $\lambda_i$ and variance $\lambda_i/T_i$. It is not itself a Poisson variable unless $T_i=1$. Known observation periods allow count modelling with a log-exposure [offset](generalized-linear-model-offset.md); otherwise [Quasi-Poisson regression](quasi-poisson-regression.md) may be used as a working mean-variance model, with uncertainty qualified by the missing exposure information.

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

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-102/3/b/solution.md)
