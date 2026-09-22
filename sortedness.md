# Sortedness

↑ **Parent:** [Sorting algorithm](sorting-algorithm.md)

For an [output](output-computing.md) [sequence](sequence.md) $B$ of length $n$, [sortedness](sortedness.md) means

$$
k(B_i)\leq k(B_{i+1})\qquad(0\leq i<n-1)
$$

under the chosen [total order](total-order.md) on [sort keys](sort-key.md). Its [transitivity](transitive-relation.md) also gives $k(B_i)\leq k(B_j)$ whenever $i<j$. An empty [sequence](sequence.md) and a one-entry [sequence](sequence.md) satisfy [sortedness](sortedness.md) without any adjacent comparison. For longer [sequences](sequence.md), checking adjacent pairs suffices; checking only the first and last [sort keys](sort-key.md) does not. For example, $(1,3,2,4)$ passes an endpoint comparison but fails [sortedness](sortedness.md) at $3,2$. [Sortedness](sortedness.md) alone says nothing about which [input](input-computer-science.md) entries survived.

## ↑ Ancestors (4)

1. [Sorting algorithm](sorting-algorithm.md)
2. [Algorithm](algorithm.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Insertion sort](insertion-sort.md)
- [Sortedness](sortedness.md)
- [Sorting algorithm](sorting-algorithm.md)
