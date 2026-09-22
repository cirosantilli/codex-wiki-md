# Lehmer code

↑ **Parent:** [Permutation](permutation.md)

For a [permutation](permutation.md) $p_0,\ldots,p_{n-1}$ of $n$ ordered distinct values, its Lehmer code has entries $c_i=\#\{j>i:p_j<p_i\}$. Its zero-based [lexicographic order](lexicographic-order.md) rank is $\sum_{i=0}^{n-1}c_i(n-1-i)!$. Each entry chooses among the still unused values; the [factorial](factorial.md) weights count all completions with a smaller choice at the first differing position.

## ↑ Ancestors (5)

1. [Permutation](permutation.md)
2. [Combinatorics](combinatorics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
