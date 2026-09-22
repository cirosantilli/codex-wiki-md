# Fisher information per observation and per trial

↑ **Parent:** [Fisher information matrix](fisher-information-matrix.md)

Precision comparisons using [Fisher information](fisher-information-matrix.md) must specify what one observation records. A [Bernoulli distribution](bernoulli-distribution.md) with success probability $\theta$ gives information $I_{\mathrm{Bern}}=1/[\theta(1-\theta)]$ per trial. A [geometric distribution](geometric-distribution.md) on $1,2,\ldots$ records the number of trials until the first success. Its log-likelihood for one waiting time $X$ is $\log\theta+(X-1)\log(1-\theta)$, so

$$
I_{\mathrm{geom}}=\frac1{\theta^2}+\frac{\mathbb E(X-1)}{(1-\theta)^2}
=\frac1{\theta^2(1-\theta)}.
$$

At equal numbers of observations, geometric waiting times therefore provide $1/\theta$ times as much information, and the asymptotic [variance](variance-split.md) of their [maximum-likelihood estimator](maximum-likelihood-estimator.md) is $\theta$ times the Bernoulli variance. But each waiting time uses an expected $1/\theta$ trials. Information per expected underlying trial is consequently $\theta I_{\mathrm{geom}}=I_{\mathrm{Bern}}$. This separates an observation count from the cost of collecting the observations.

## ↑ Ancestors (8)

1. [Fisher information matrix](fisher-information-matrix.md)
2. [Informant function](informant-function.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-options-i-course-of-the-university-of-oxford/2012/o/o1/d/solution.md)
