# Sorting permutation preservation

↑ **Parent:** [Sorting algorithm](sorting-algorithm.md)

The [output](output-computing.md) of a [sorting algorithm](sorting-algorithm.md) must be a [permutation](permutation.md) of the complete [input](input-computer-science.md) [sequence](sequence.md). For equal lengths $n$, require a [permutation](permutation.md) $\pi$ of $\{0,\ldots,n-1\}$ such that

$$
B_i=A_{\pi(i)}\qquad(0\leq i<n).
$$

Equivalently, the [input](input-computer-science.md) and [output](output-computing.md) have the same [multiset](multiset.md) of complete entries: each entry has the same multiplicity. Equality of the underlying [sets](set-split.md) is insufficient; $(1,1,2)$ and $(1,2,2)$ have the same [set](set-split.md) of values and the same length but different [multisets](multiset.md). When tracking occurrences rather than contents, retain original identity labels to check that each one is moved exactly once. A swap preserves this [multiset](multiset.md) automatically; an overwrite need not.

## ↑ Ancestors (4)

1. [Sorting algorithm](sorting-algorithm.md)
2. [Algorithm](algorithm.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Insertion sort](insertion-sort.md)
- [Sorting algorithm](sorting-algorithm.md)
- [Sorting record](sorting-record.md)
