# Conditional cure-weight equations for paired Poisson counts

↑ **Parent:** [Paired Poisson conditional likelihood](paired-poisson-conditional-likelihood.md)

Consider an approximate [conditional likelihood](conditional-likelihood.md) in which a paired total $t_i$ leads to a structural zero with probability $\theta$, and otherwise a [binomial distribution](binomial-distribution.md) with success probability $p$. For an observed zero, the posterior cure weight is $q_i=\theta/[\theta+(1-\theta)(1-p)^{t_i}]$; for a positive count it is zero. Differentiating the [log-likelihood](log-likelihood.md) gives the displayed equations at an interior [maximum-likelihood estimator](maximum-likelihood-estimator.md), with the weights evaluated at that estimator. Recomputing the weights and then updating the parameters is an [expectation-maximization algorithm](expectation-maximization-algorithm.md). Boundary fits must also be considered. These equations describe a conditional mixture: if cure is instead specified before two [Poisson distributions](poisson-distribution.md) are conditioned on their total, its conditional probability generally depends on the total and on the baseline nuisance rate. A zero observed in a short interval is not by itself proof of permanent biological cure.

## ↑ Ancestors (10)

1. [Paired Poisson conditional likelihood](paired-poisson-conditional-likelihood.md)
2. [Two-group Poisson ratio conditional likelihood](two-group-poisson-ratio-conditional-likelihood.md)
3. [Poisson regression](poisson-regression.md)
4. [Generalized linear model](generalized-linear-model.md)
5. [Statistical modelling](statistical-modelling-split.md)
6. [Statistical model](statistical-model-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-44/5/b/solution.md)
