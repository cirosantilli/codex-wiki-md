# Sorting algorithm

↑ **Parent:** [Algorithm](algorithm.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sorting_algorithm)

A [sorting algorithm](sorting-algorithm.md) rearranges a finite [sequence](sequence.md) into nondecreasing order under a chosen [total order](total-order.md) on its keys. Its [output](output-computing.md) must contain every [input](input-computer-science.md) entry exactly once, including repetitions: producing ordered values is insufficient if entries are lost. [Merge sort](merge-sort.md) is one such [algorithm](algorithm.md); [stable sorting](stable-sorting.md) adds a requirement about equal keys.

Sorting creates reusable structure: equal [sort keys](sort-key.md) become adjacent, and a [sorted array](sorted-array.md) supports [binary search](binary-search.md). However, an [algorithm correctness](algorithm-correctness.md) check must establish both [sortedness](sortedness.md) and [sorting permutation preservation](sorting-permutation-preservation.md). Replacing every entry by the smallest key can produce ordered keys while destroying the original data. [Stable sorting](stable-sorting.md) imposes a third condition when equal [sort keys](sort-key.md) occur: retain their arrival order.

For example, take complete [sorting records](sorting-record.md) $(2,A),(1,B),(2,C),(1,D)$, with the first component as the [sort key](sort-key.md) and the letter as associated data. A correct [output](output-computing.md) is $(1,B),(1,D),(2,A),(2,C)$. The [sort keys](sort-key.md) are ordered, every complete [sorting record](sorting-record.md) remains, and the equal-key pairs keep $A$ before $C$ and $B$ before $D$. The [output](output-computing.md) $(1,D),(1,B),(2,C),(2,A)$ satisfies [sortedness](sortedness.md) and [sorting permutation preservation](sorting-permutation-preservation.md), but fails [stable sorting](stable-sorting.md). The [output](output-computing.md) $(1,B),(1,B),(2,A),(2,A)$ has the right [multiset](multiset.md) of [sort keys](sort-key.md) but loses $C,D$ and duplicates $A,B$; it fails [sorting permutation preservation](sorting-permutation-preservation.md) of complete [sorting records](sorting-record.md).

To express [stable sorting](stable-sorting.md) precisely, label every [input](input-computer-science.md) occurrence by its original position, even when two complete [sorting records](sorting-record.md) have identical contents. Let $p(i)$ be the [output](output-computing.md) position of the occurrence originally at position $i$. Besides [sortedness](sortedness.md) and [sorting permutation preservation](sorting-permutation-preservation.md), require

$$
i<j\ \text{and}\ k(A_i)=k(A_j)\quad\Longrightarrow\quad p(i)<p(j).
$$

Here $k$ is the [sort key](sort-key.md) [function](function-split.md). Sorting by the pair $(k(A_i),i)$ under [lexicographic order](lexicographic-order.md) gives the same order as [stable sorting](stable-sorting.md) by $k$: the original position breaks ties without discarding associated data. For a two-field ordering, first apply [stable sorting](stable-sorting.md) by the secondary [sort key](sort-key.md), then apply [stable sorting](stable-sorting.md) by the primary [sort key](sort-key.md). The second pass retains the secondary order within each group of equal primary [sort keys](sort-key.md). For instance, $(2,B),(1,C),(2,A),(1,A)$ first becomes $(2,A),(1,A),(2,B),(1,C)$ by letter, then $(1,A),(1,C),(2,A),(2,B)$ by number.

**Table of contents**

- [Sort key](sort-key.md)
  - [Sorting record](sorting-record.md)
- [Sortedness](sortedness.md)
- [Sorting permutation preservation](sorting-permutation-preservation.md)
- [Insertion sort](insertion-sort.md)
- [Comparison sort](comparison-sort.md)
  - [Comparison sorting lower bound](comparison-sorting-lower-bound.md)
- [Counting sort](counting-sort.md)
- [Radix sort](radix-sort.md)
- [Stable sorting](stable-sorting.md)
- [Merge sort](merge-sort.md)

## ↑ Ancestors (3)

1. [Algorithm](algorithm.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Binary heap](binary-heap.md)
- [Information hiding](information-hiding.md)
- [Sorting algorithm](sorting-algorithm.md)
- [Sorting permutation preservation](sorting-permutation-preservation.md)
