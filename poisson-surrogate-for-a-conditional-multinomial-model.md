# Poisson surrogate for a conditional multinomial model

↑ **Parent:** [Log-linear model](log-linear-model.md)

Independent [Poisson distributions](poisson-distribution.md) with a separate nuisance intercept in every stratum become [multinomial distributions](multinomial-distribution.md) after conditioning on their totals. Profiling the intercept gives $e^{\widehat\gamma_s}=N_s/\sum_l e^{x_s^T\beta_l}$. Substitution produces the same parameter-dependent [log-likelihood](log-likelihood.md) as the conditional multinomial model. Both approaches fit $\widehat\mu_{sl}=N_s\widehat p_{sl}$. This exact equivalence differs from approximating a single binomial event count by a rare-event [Poisson distribution](poisson-distribution.md).

## ↑ Ancestors (7)

1. [Log-linear model](log-linear-model.md)
2. [Statistical modelling](statistical-modelling-split.md)
3. [Statistical model](statistical-model-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-28/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-28/5/ii/solution.md)
