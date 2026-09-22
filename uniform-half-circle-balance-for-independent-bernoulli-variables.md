# Uniform half-circle balance for independent Bernoulli variables

↑ **Parent:** [Hoeffding inequality](hoeffding-inequality.md)

Let $n$ be even and let $X_1,\ldots,X_n$ be independent [Bernoulli](bernoulli-distribution.md) variables with parameter $1/2$, arranged on a circle. The probability that some consecutive half-circle $I$ has $|\sum_{i\in I}X_i-\sum_{i\notin I}X_i|\geq w$ is at most $2n\exp(-2w^2/n)$. For a fixed $I$, the variable $Z_I=\sum_{i\in I}X_i+\sum_{i\notin I}(1-X_i)$ has the [binomial distribution](binomial-distribution.md) $\operatorname{Bin}(n,1/2)$, and the signed imbalance is $Z_I-n/2$. Apply [Hoeffding inequality](hoeffding-inequality.md) to this single [binomial](binomial-distribution.md) variable, then take a [union bound](boole-s-inequality.md) over the at most $n$ intervals. Consequently $w=c\sqrt{n\log n}$ suffices for uniform balance with probability tending to one whenever $c>1/\sqrt2$.

## ↑ Ancestors (8)

1. [Hoeffding inequality](hoeffding-inequality.md)
2. [Concentration inequality](concentration-inequality.md)
3. [Probability inequality](probability-inequality-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford/2010/b/6/c/solution.md)
