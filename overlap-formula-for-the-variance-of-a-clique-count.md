# Overlap formula for the variance of a clique count

↑ **Parent:** [Clique count in a binomial random graph](clique-count-in-a-binomial-random-graph.md)

For the number $X$ of $k$-[cliques](clique-graph-theory.md) in a [binomial random graph](binomial-random-graph.md) $G(n,p)$, with $0<p<1$ and $\mu=\mathbb EX$,

$$
\frac{\operatorname{Var}X}{\mu^2}=\sum_{j=2}^k\frac{\binom kj\binom{n-k}{k-j}}{\binom nk}\left(p^{-\binom j2}-1\right).
$$

Two $k$-sets overlapping in $j$ vertices share $\binom j2$ edges. Overlaps of zero or one vertex give independent indicators; $j=k$ includes the diagonal terms. The identity is useful for the [second moment method](second-moment-method.md).

**Table of contents**

- [Growing-clique overlap bound](growing-clique-overlap-bound.md)

## ↑ Ancestors (7)

1. [Clique count in a binomial random graph](clique-count-in-a-binomial-random-graph.md)
2. [Binomial random graph](binomial-random-graph.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Fixed-size clique appearance threshold](fixed-size-clique-appearance-threshold.md)
- [Growing-clique overlap bound](growing-clique-overlap-bound.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-12/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-37/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-112/4/solution.md)
