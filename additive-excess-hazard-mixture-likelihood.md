# Additive excess-hazard mixture likelihood

↑ **Parent:** [Survival likelihood](survival-likelihood.md)

Suppose an unobserved class has probabilities $\pi$ and $1-\pi$, with [hazard functions](hazard-function.md) $q$ and $q+r$, and set $Q(t)=\int_0^tq$, $R(t)=\int_0^tr$. For an independently right-censored observation $(x,v)$, its survival-parameter likelihood contribution is

$$
L=e^{-Q(x)}\{\pi q(x)^v+(1-\pi)[q(x)+r(x)]^ve^{-R(x)}\}.
$$

This sums the two class-specific likelihoods before taking a logarithm. All hazards must be nonnegative. A common parameter-free censoring mechanism factors out; class-specific censoring instead alters the mixture weights and cannot silently be discarded.

// Target: probability-and-statistics.bigb

## ↑ Ancestors (6)

1. [Survival likelihood](survival-likelihood.md)
2. [Survival analysis](survival-analysis-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-29/2/c/solution.md)
