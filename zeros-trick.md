# Zeros trick

↑ **Parent:** [BUGS](bugs.md)

A [zeros trick](zeros-trick.md) implements a positive [likelihood function](likelihood-function.md) $L(\theta)$ by adding an observed zero with [Poisson distribution](poisson-distribution.md) mean $K-\log L(\theta)$. If this mean is nonnegative throughout the parameter support, its likelihood is $e^{-K}L(\theta)$ and yields the intended [Bayesian posterior](bayesian-posterior.md). The constant $K$ must be independent of the parameter; arbitrary clipping changes the target.

## ↑ Ancestors (7)

1. [BUGS](bugs.md)
2. [Bayesian statistics](bayesian-statistics.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35/1/h/solution.md)
- [Zeros trick](zeros-trick.md)
