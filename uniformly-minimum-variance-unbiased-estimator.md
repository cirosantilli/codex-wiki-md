# Uniformly minimum-variance unbiased estimator

↑ **Parent:** [Unbiased estimator](unbiased-estimator.md)

An [unbiased estimator](unbiased-estimator.md) $T$ is uniformly minimum-variance unbiased if its [variance](variance-split.md) is no larger than that of every other [unbiased estimator](unbiased-estimator.md) of the same parameter, for every parameter value. The [Lehmann–Scheffé theorem](lehmann-scheffe-theorem.md) gives such an estimator whenever an unbiased function of a [complete sufficient statistic](complete-sufficient-statistic.md) exists. Attaining the [Cramér-Rao bound](cramer-rao-bound.md) is sufficient for this property under its hypotheses, but is not necessary: for $T\sim\Gamma(n,\lambda)$ with $n>2$, $(n-1)/T$ is unbiased and has [variance](variance-split.md) $\lambda^2/(n-2)$, while the information bound is $\lambda^2/n$. Completeness follows from uniqueness of the [Laplace transform](laplace-transform.md) of $h(t)t^{n-1}$, so the estimator is still uniformly optimal among [unbiased estimators](unbiased-estimator.md).

## ↑ Ancestors (7)

1. [Unbiased estimator](unbiased-estimator.md)
2. [Statistical modelling](statistical-modelling-split.md)
3. [Statistical model](statistical-model-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
