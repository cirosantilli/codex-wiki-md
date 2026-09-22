# Jeffreys prior for a Bernoulli parameter

↑ **Parent:** [Jeffreys prior](jeffreys-prior.md)

For a [Bernoulli random variable](bernoulli-distribution.md) with success [probability](probability.md) $0<\theta<1$, the [score function](informant-function.md) is $(X-\theta)/(\theta(1-\theta))$. The [expected value](expected-value-split.md) of its square is $I(\theta)=1/(\theta(1-\theta))$, since the [variance](variance-split.md) of $X$ is $\theta(1-\theta)$. The [Jeffreys prior](jeffreys-prior.md) is therefore the proper [beta distribution](beta-distribution.md) $\operatorname{Beta}(1/2,1/2)$, also called the [arcsine distribution](arcsine-distribution.md). The [Euler beta function](beta-function.md) has $B(1/2,1/2)=\pi$, giving the stated normalized [prior density](prior-density.md).

After $s$ successes in $n$ independent [Bernoulli trials](bernoulli-trial.md), [Beta-binomial conjugacy](beta-binomial-conjugacy.md) gives [posterior distribution](bayesian-posterior.md) $\operatorname{Beta}(s+1/2,n-s+1/2)$ and [posterior predictive probability](posterior-predictive-probability.md) $(s+1/2)/(n+1)$ of one further success. Although its [prior density](prior-density.md) diverges at both boundaries, its integral is finite.

## ↑ Ancestors (9)

1. [Jeffreys prior](jeffreys-prior.md)
2. [Fisher information matrix](fisher-information-matrix.md)
3. [Informant function](informant-function.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-statistics-course-of-the-university-of-oxford/2017/3/c/iii/solution.md)
