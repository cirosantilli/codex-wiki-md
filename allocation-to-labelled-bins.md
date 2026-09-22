# Allocation to labelled bins

↑ **Parent:** [Combinatorics](combinatorics-split.md)

Allocate $n$ distinct objects to $k$ labelled bins of specified nonnegative sizes $n_1,\ldots,n_k$, with $\sum_i n_i=n$. Order within a bin is ignored. The number of allocations is the [multinomial coefficient](multinomial-coefficient.md)

$$
N(n_1,\ldots,n_k)=\frac{n!}{n_1!\cdots n_k!}.
$$

To prove this, order all the objects in a [permutation](permutation.md) and assign the first $n_1$ to the first bin, the next $n_2$ to the second, and so on. Every allocation comes from exactly $n_1!\cdots n_k!$ internal orderings. These disjoint classes exhaust the $n!$ [permutations](permutation.md), proving the formula by the [multiplication principle](rule-of-product.md). Empty bins are allowed because $0!=1$.

For two bins of sizes $m$ and $n-m$, the count is $\binom nm$ and every allocation has multiplicity $m!(n-m)!$ in the [permutation](permutation.md) sample space. Exchanging two equal-sized labelled bins generally gives a different allocation. In contrast, a [set partition](set-partition.md) uses unlabelled nonempty blocks; forgetting bin labels changes the counting problem and must not be done silently.

## ↑ Ancestors (4)

1. [Combinatorics](combinatorics-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)
