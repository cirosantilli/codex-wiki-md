# Latent-normal Gibbs sampler for probit regression

↑ **Parent:** [Probit model](probit-model.md)

For binary observations with success probability $\Phi(\beta x_i)$, introduce latent $Z_i\sim N(\beta x_i,1)$ and let the sign determine the observation. Given $\beta$ and the observed sign, each latent variable has a [truncated normal distribution](truncated-normal-distribution.md). With a standard normal prior, the [full conditional distribution](full-conditional-distribution.md) of $\beta$ is normal with precision $1+\sum_i x_i^2$ and mean $\sum_i x_iZ_i/(1+\sum_i x_i^2)$. Alternating these blocks is [Gibbs sampling](gibbs-sampler.md) with the required marginal posterior.

## ↑ Ancestors (8)

1. [Probit model](probit-model.md)
2. [Generalized linear model](generalized-linear-model.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-29/3/solution.md)
