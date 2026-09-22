# Spatial Bernoulli infection model

↑ **Parent:** [Statistical model](statistical-model-split.md)

Given the currently infected set $I_t$ and susceptible set $S_t$, define $A_{it}(\eta)=\sum_{j\in I_t}K_\eta(d_{ij})$ and $P_{it}=1-e^{-\alpha A_{it}}$. Conditionally [independent](independent-random-variables.md) new-infection indicators $Y_{it}$ have [likelihood](likelihood-function.md)

$$
L(\alpha,\eta)=\prod_t\prod_{i\in S_t}(1-e^{-\alpha A_{it}(\eta)})^{Y_{it}}e^{-\alpha A_{it}(\eta)(1-Y_{it})}.
$$

A nonnegative infection intensity requires $\alpha\geq0$; an unrestricted [normal distribution](normal-distribution.md) [prior distribution](prior-probability.md) for $\alpha$ must therefore be restricted or replaced. With $K_\beta(d)=d^{-\beta}$ or $K_\gamma(d)=e^{-\gamma d}$ and positive distances, the conditional [posterior](bayesian-posterior.md) kernels are not generally conjugate normal [probability densities](probability-density.md). [Metropolis–Hastings algorithm](metropolis-hastings-algorithm.md) updates, optionally on $\log\alpha$ with its [Jacobian determinant](jacobian-determinant.md), provide a direct sampling method.

## ↑ Ancestors (5)

1. [Statistical model](statistical-model-split.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47/5/b/solution.md)
