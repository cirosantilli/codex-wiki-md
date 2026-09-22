# Finite-exposure Poisson inconsistency

↑ **Parent:** [Poisson exposure model](poisson-exposure-model.md)

Let independent counts satisfy $Y_i\sim\operatorname{Poi}(\theta w_i)$, with positive known exposures $w_i$, $\theta>0$, and $a_n=\sum_{i=1}^nw_i\uparrow a_\infty<\infty$. Their [likelihood](likelihood-function.md) is proportional to $\theta^{S_n}e^{-a_n\theta}$, where $S_n=\sum_{i=1}^nY_i$. If $S_n>0$, the positive [maximum-likelihood estimator](maximum-likelihood-estimator.md) is $S_n/a_n$; when $S_n=0$, no maximum is attained on the open parameter space, while the closed-space maximizer is zero. This extended estimate converges almost surely to $S_\infty/a_\infty$, where $S_\infty\sim\operatorname{Poi}(\theta a_\infty)$. Finiteness follows from $\mathbb E S_\infty=\theta a_\infty$, and the limiting [Poisson distribution](poisson-distribution.md) follows from the finite-sum laws. In particular, the probability of a zero estimate tends to $e^{-\theta a_\infty}>0$, proving failure of [statistical consistency](consistency-statistics.md). The total [Fisher information](fisher-information-matrix.md) tends to $a_\infty/\theta$: infinitely many observations need not provide infinite information.

## ↑ Ancestors (8)

1. [Poisson exposure model](poisson-exposure-model.md)
2. [Generalized linear model](generalized-linear-model.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-32/2/2/solution.md)
