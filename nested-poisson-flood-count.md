# Nested Poisson flood count

↑ **Parent:** [Compound Poisson distribution](compound-poisson-distribution.md)

If a [Poisson distribution](poisson-distribution.md) count $M$ of clusters has mean $\nu$, and each cluster independently contains a Poisson number of claims of mean $\lambda$, then the total count is a [compound Poisson distribution](compound-poisson-distribution.md) with the displayed [probability generating function](probability-generating-function.md). Conditioning gives $\mathbb EN=\nu\lambda$ and $\operatorname{Var}N=\nu\lambda(1+\lambda)$, so it is not Poisson for positive parameters. With independent severities of mean $\mu$ and variance $\sigma^2$, the aggregate payment has mean $\nu\lambda\mu$ and variance $\nu[\lambda(\sigma^2+\mu^2)+\lambda^2\mu^2]$. Independent validity thinning replaces the per-cluster count mean by $\lambda(1-p)$ and multiplies expected payment by $1-p$.

## ↑ Ancestors (8)

1. [Compound Poisson distribution](compound-poisson-distribution.md)
2. [Random sum of independent claims](random-sum-of-independent-claims.md)
3. [Aggregate claims model](aggregate-claims-model.md)
4. [Actuarial statistics](actuarial-statistics-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-27/1/solution.md)
