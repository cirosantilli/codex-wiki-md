# Logistic random-intercept model for repeated binary outcomes

↑ **Parent:** [Generalized linear mixed model](generalized-linear-mixed-model.md)

A subject has a [random intercept](random-intercept.md) $B_i\sim N(0,\tau^2)$, with responses conditionally independent given $B_i$ and their [covariates](covariate.md). Integrating the product of [Bernoulli](bernoulli-distribution.md) [likelihoods](likelihood-function.md) over $B_i$ defines the joint subject [likelihood](likelihood-function.md) and induces within-subject dependence. Its coefficients describe conditional [odds ratios](odds-ratio.md) for a fixed latent subject effect. Under [missing at random](missing-at-random.md) with [distinct parameters](distinct-parameters.md), the observed-response likelihood integrates over the same random effect and sums out unobserved responses. Dependence of dropout on $B_i$ is not generally ignorable merely because conditional independence holds given $B_i$.

**Table of contents**

- [Random-intercept attenuation of marginal logistic slopes](random-intercept-attenuation-of-marginal-logistic-slopes.md)

## ↑ Ancestors (8)

1. [Generalized linear mixed model](generalized-linear-mixed-model.md)
2. [Generalized linear model](generalized-linear-model.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-38/5/ii/b/solution.md)
