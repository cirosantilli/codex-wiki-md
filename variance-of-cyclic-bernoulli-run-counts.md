# Variance of cyclic Bernoulli run counts

↑ **Parent:** [Bernoulli distribution](bernoulli-distribution.md)

On a cyclic sequence of $n$ independent [Bernoulli random variables](bernoulli-distribution.md) with success probability $p$, count all runs of $k$ consecutive successes, allowing overlaps and taking $1\le k\le n/2$. The count has [expected value](expected-value-split.md) $np^k$. Its [variance](variance-split.md) is the displayed expression: each starting indicator has variance $p^k(1-p^k)$; two starts at cyclic distance $j<k$ have joint probability $p^{k+j}$; nonoverlapping starts are independent. There are $2n$ ordered overlapping pairs at each such distance, because the two ranges do not meet when $k\le n/2$.

For $p\le1/2$, summing a [geometric series](geometric-series.md) gives $\operatorname{Var}X\le np^k(1+2p/(1-p))\le3np^k$. [Markov's inequality](markov-s-inequality.md) therefore proves absence with high probability when $np^k\to0$, and [Chebyshev's inequality](chebyshev-s-inequality.md) proves existence and relative concentration when $np^k\to\infty$. This remains valid for varying probabilities eventually at most one half.

## ↑ Ancestors (8)

1. [Bernoulli distribution](bernoulli-distribution.md)
2. [Discrete probability distribution](discrete-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
