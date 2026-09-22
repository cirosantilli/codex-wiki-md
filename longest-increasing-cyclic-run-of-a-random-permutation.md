# Longest increasing cyclic run of a random permutation

↑ **Parent:** [Uniform random permutation](uniform-random-permutation.md)

Arrange a [uniform random permutation](uniform-random-permutation.md) of $n$ distinct ordered elements around a circle, and let $L$ be the greatest number of consecutive entries that appear in increasing order. Put $k_0=\min\{k:k!\geq n\}$. Then $\mathbb P(k_0-2\leq L\leq k_0)\to1$ as $n\to\infty$.

Let $X_k$ count increasing consecutive blocks of length $k$. Each of the $n$ starting positions succeeds with probability $1/k!$, so $\mathbb EX_k=n/k!$. For $k\leq n/2$, disjoint blocks have independent relative orders; blocks overlapping with a start displacement $s<k$ are both increasing precisely when their length-$k+s$ union is increasing. Thus

$$
\mathbb EX_k^2=\frac n{k!}+2n\sum_{s=1}^{k-1}\frac1{(k+s)!}+\frac{n(n-2k+1)}{(k!)^2}
\leq\frac{n^2}{(k!)^2}+\frac{2n}{k!}.
$$

Consequently [Markov's inequality](markov-s-inequality.md) gives $\mathbb P(L\geq k_0+1)\leq1/(k_0+1)$, while [Chebyshev's inequality](chebyshev-s-inequality.md) gives $\mathbb P(L<k_0-2)\leq2/(k_0-1)$ for sufficiently large $n$. The latter uses $n/(k_0-2)!>k_0-1$. Both bounds vanish. These are consecutive cyclic runs; allowing arbitrary skipped entries is a different permutation statistic.

## ↑ Ancestors (6)

1. [Uniform random permutation](uniform-random-permutation.md)
2. [Permutation](permutation.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford/2009/b/4/b/iii/solution.md)
