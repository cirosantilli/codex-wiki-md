# Reparameterization invariance of Jeffreys prior

↑ **Parent:** [Jeffreys prior](jeffreys-prior.md)

For a regular scalar model, let $\eta=h(\theta)$ be a smooth invertible change of [statistical parameter](statistical-parameter.md) with nonzero [derivative](derivative.md). The [chain rule](chain-rule.md) makes the [score function](informant-function.md) in the new coordinate equal to the old [score function](informant-function.md) times $d\theta/d\eta$. Therefore the expected [Fisher information](fisher-information-matrix.md) transforms as $I_\eta=I_\theta(d\theta/d\eta)^2$. Taking its square root gives exactly the absolute change-of-variable factor required for a [prior density](prior-density.md).

Consequently, computing the [Jeffreys prior](jeffreys-prior.md) directly in either coordinate produces the same measure after transformation. Its density is not numerically constant across coordinates, nor must either density be uniform. When the [prior distribution](prior-probability.md) is proper, compatible normalization gives identical [prior probabilities](prior-probability.md) for corresponding sets; the resulting [posterior distributions](bayesian-posterior.md) also transform consistently. For an [improper prior](improper-prior.md) the equality concerns measure kernels up to a constant, and [posterior propriety](posterior-propriety.md) still needs checking.

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

- [Solution](past-exam-of-the-statistics-course-of-the-university-of-oxford/2017/3/c/ii/solution.md)
