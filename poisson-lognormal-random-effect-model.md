# Poisson-lognormal random-effect model

↑ **Parent:** [Random effect](random-effect.md)

Let $Y\mid\Lambda\sim\operatorname{Poisson}(e^{\eta+\Lambda})$, with $\Lambda\sim N(0,\tau^2)$. The [lognormal distribution](log-normal-distribution.md) of the random mean gives marginal mean $m=e^{\eta+\tau^2/2}$. The [law of total variance](law-of-total-variance.md) gives $\operatorname{Var}(Y)=m+m^2(e^{\tau^2}-1)$, strictly larger than $m$ when $\tau>0$. Thus independent observation-level [random effects](random-effect.md) produce [overdispersion](overdispersion.md) even though the conditional [Poisson distributions](poisson-distribution.md) have variance equal to their means.

## ↑ Ancestors (8)

1. [Random effect](random-effect.md)
2. [Latent variable](latent-variable.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-36/3/b/solution.md)
