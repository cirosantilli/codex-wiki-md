# Gamma random-intercept Poisson model

↑ **Parent:** [Poisson generalized linear mixed model](poisson-generalized-linear-mixed-model.md)

Let the positive multiplier $U_i$ have a [gamma distribution](gamma-distribution.md) with mean $\tau$ and [variance](variance-split.md) $\theta$, and conditionally let the repeated counts be [independent](independent-random-variables.md) with means $U_i a_{ij}$. Total [expectation](expected-value.md) and [variance](variance-split.md) give

$$
\mathbb EY_{ij}=\tau a_{ij},\qquad
\operatorname{Var}(Y_{ij})=\tau a_{ij}+\theta a_{ij}^2,\qquad
\operatorname{Cov}(Y_{ij},Y_{ik})=\theta a_{ij}a_{ik}\quad(j\ne k).
$$

The [Poisson-gamma mixture](poisson-gamma-mixture.md) gives negative-binomial marginal counts of size $\tau^2/\theta$. Despite the shared multiplier, the marginal correlations generally depend on both marginal means and need not be exchangeable.

**Table of contents**

- [Scale identifiability in a gamma random-intercept Poisson model](scale-identifiability-in-a-gamma-random-intercept-poisson-model.md)

## ↑ Ancestors (9)

1. [Poisson generalized linear mixed model](poisson-generalized-linear-mixed-model.md)
2. [Generalized linear mixed model](generalized-linear-mixed-model.md)
3. [Generalized linear model](generalized-linear-model.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-36/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-36/4/iii/solution.md)
- [Scale identifiability in a gamma random-intercept Poisson model](scale-identifiability-in-a-gamma-random-intercept-poisson-model.md)
