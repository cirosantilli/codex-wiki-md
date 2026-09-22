# Backtracking leaf bound

↑ **Parent:** [Backtracking](backtracking.md)

Suppose [backtracking](backtracking.md) assigns each of finitely many variables once along each branch, branching only on distinct values in its initial nonempty [constraint domain](constraint-domain.md) $D_i$. Then the number of leaves is at most $\prod_i|D_i|$, even if inconsistent partial assignments terminate early. Ignore constraints and associate a leaf with every full domain assignment extending its partial assignment. Each leaf has at least one such extension. Different leaves have disjoint extension families: at their first diverging choice they assigned different values to the same selected variable. These nonempty disjoint families lie in a [Cartesian product](cartesian-product.md) of [cardinality](cardinality.md) $\prod_i|D_i|$, proving the bound. The selected next variable can depend on the preceding assignments, provided each full assignment follows a unique branch.

The bound is exact for an unpruned enumeration tree, but need not be attained when actual constraints cause [search pruning](search-pruning.md). Counting complete satisfying assignments alone also does not count failed partial leaves.

## ↑ Ancestors (4)

1. [Backtracking](backtracking.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/artificial-intelligence/3/e/solution.md)
