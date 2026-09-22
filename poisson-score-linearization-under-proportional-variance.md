# Poisson score linearization under proportional variance

↑ **Parent:** [Quasi-Poisson regression](quasi-poisson-regression.md)

With $\mu_i=e^{\beta x_i}$, define $U=\sum_i x_i(Y_i-\mu_i)$ and $I=\sum_i x_i^2\mu_i$. The estimating equation and a [Taylor expansion](taylor-expansion.md) give $\widehat\beta-\beta_0\approx I(\beta_0)^{-1}U(\beta_0)$. If responses are independent with correct means and $\operatorname{Var}(Y_i)=\phi\mu_i$, then $EU=0$ and $\operatorname{Var}U=\phi I$. Consequently the first-order estimator [variance](variance-split.md) is $\phi/I$, even if the working [Poisson distribution](poisson-distribution.md) is wrong. Regular asymptotics require growing information and control of leverage and the Taylor remainder.

## ↑ Ancestors (8)

1. [Quasi-Poisson regression](quasi-poisson-regression.md)
2. [Generalized linear model](generalized-linear-model.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-37/1/ii/solution.md)
