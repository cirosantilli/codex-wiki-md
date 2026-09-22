# Poisson surrogate for an uncensored proportional-hazards likelihood

↑ **Parent:** [Proportional hazards model](proportional-hazards-model.md)

For independent uncensored event times $Y_i$ with $h_i(t)=\lambda(t)e^{\beta^Tx_i}$ and baseline cumulative hazard $\Lambda(t)=\int_0^t\lambda(s)\,ds$, maximizing the survival log likelihood over $\beta$ is equivalent to fitting a [Poisson regression](poisson-regression.md) with unit responses and means

$$
\mu_i=\Lambda(Y_i)e^{\beta^Tx_i}.
$$

Thus a log-link [generalized linear model](generalized-linear-model.md) with response $1$, linear predictor $\beta^Tx_i$, and offset $\log\Lambda(Y_i)$ gives the same estimate of $\beta$.

## ↑ Ancestors (6)

1. [Proportional hazards model](proportional-hazards-model.md)
2. [Survival analysis](survival-analysis-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-1/13j/c/solution.md)
