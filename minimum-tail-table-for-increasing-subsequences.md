# Minimum-tail table for increasing subsequences

↑ **Parent:** [Longest increasing subsequence](longest-increasing-subsequence.md)

For a processed prefix $(x_1,\ldots,x_i)$, the [minimum-tail table for increasing subsequences](minimum-tail-table-for-increasing-subsequences.md) stores

$$
T_\ell=\min\{x_{j_\ell}:1\leq j_1<\cdots<j_\ell\leq i,\ x_{j_1}\leq\cdots\leq x_{j_\ell}\},\qquad 1\leq\ell\leq L(x_1,\ldots,x_i).
$$

There is no slot for an unattainable length. The table records [minimum](minimum-of-a-subset-of-a-total-order.md) endings, rather than the terms of one [longest increasing subsequence](longest-increasing-subsequence.md). Replacing the value comparisons by $<$ gives the corresponding table for [strictly increasing subsequences](strictly-increasing-subsequence.md), whose entries are strictly increasing.

## ↑ Ancestors (6)

1. [Longest increasing subsequence](longest-increasing-subsequence.md)
2. [Increasing subsequence](increasing-subsequence.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Longest increasing subsequence](longest-increasing-subsequence.md)
- [Minimum-tail table for increasing subsequences](minimum-tail-table-for-increasing-subsequences.md)
