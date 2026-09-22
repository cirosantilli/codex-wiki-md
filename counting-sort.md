# Counting sort

↑ **Parent:** [Sorting algorithm](sorting-algorithm.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Counting_sort)

[Counting sort](counting-sort.md) uses [integer](integer-split.md) [sort keys](sort-key.md) in $\{0,\ldots,K-1\}$ directly as indices into an [array](array-data-structure.md) of counts. Constant-cost counting and indexing give $O(n+K)$ [time complexity](time-complexity.md) in [Big O notation](big-o-notation.md). To retain complete [sorting records](sorting-record.md), cumulative counts locate their [output](output-computing.md) ranges; filling each range from its end while scanning the [input](input-computer-science.md) backwards gives [stable sorting](stable-sorting.md). Emitting bare [sort keys](sort-key.md) from counts would discard associated data. The $K$ term matters when the key range is large.[Open Data Structures: An Introduction by Pat Morin; Theorem 11.7 and stability](open-data-structures-an-introduction-by-pat-morin/11-2-counting-sort-and-radix-sort.md)

For an original worked example, take $n=7$ complete [sorting records](sorting-record.md) and $K=4$ possible [integer](integer-split.md) [sort keys](sort-key.md):

$$
A=\bigl((2,\mathrm A),(0,\mathrm B),(2,\mathrm C),(1,\mathrm D),(0,\mathrm E),(3,\mathrm F),(2,\mathrm G)\bigr).
$$

The letters label the associated data, and are never compared. Both [input](input-computer-science.md) and [output](output-computing.md) [array indices](array-index.md) start at zero, so their valid positions are $0,\ldots,6$; the count [array](array-data-structure.md) has [array indices](array-index.md) $0,\ldots,3$. [Stable sorting](stable-sorting.md) must produce

$$
B=\bigl((0,\mathrm B),(0,\mathrm E),(1,\mathrm D),(2,\mathrm A),(2,\mathrm C),(2,\mathrm G),(3,\mathrm F)\bigr).
$$

The equal-[sort key](sort-key.md) groups retain $\mathrm B,\mathrm E$ and $\mathrm A,\mathrm C,\mathrm G$ in arrival order. [Counting sort prefix ranges](counting-sort-prefix-ranges.md) explain where those groups belong; [stable record placement in counting sort](stable-record-placement-in-counting-sort.md) explains how to fill them without losing that order or the complete [sorting records](sorting-record.md).

**Table of contents**

- [Counting sort prefix ranges](counting-sort-prefix-ranges.md)
- [Stable record placement in counting sort](stable-record-placement-in-counting-sort.md)

## ↑ Ancestors (4)

1. [Sorting algorithm](sorting-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Comparison sort](comparison-sort.md)
- [Counting sort](counting-sort.md)
- [Counting sort prefix ranges](counting-sort-prefix-ranges.md)
- [Radix sort](radix-sort.md)
- [Stable digit sort](stable-digit-sort.md)
- [Stable record placement in counting sort](stable-record-placement-in-counting-sort.md)
