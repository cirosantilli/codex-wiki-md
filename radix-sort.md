# Radix sort

↑ **Parent:** [Sorting algorithm](sorting-algorithm.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radix_sort)

[Radix sort](radix-sort.md) sorts encoded [sort keys](sort-key.md) a digit at a time. Its least-significant-digit version uses [stable sorting](stable-sorting.md) on each successive digit, often by [counting sort](counting-sort.md). For $d$ digits with $R$ possible values each, it takes $O(d(n+R))$ [time complexity](time-complexity.md) in [Big O notation](big-o-notation.md), assuming constant-cost digit extraction and indexing. [Stable sorting](stable-sorting.md) retains the ordering established by earlier digits when a later digit ties. Both digit access and the direct indexing in [counting sort](counting-sort.md) lie outside the [comparison sort](comparison-sort.md) model, so these bounds do not contradict the [comparison sorting lower bound](comparison-sorting-lower-bound.md).[Open Data Structures: An Introduction by Pat Morin; Theorem 11.8](open-data-structures-an-introduction-by-pat-morin/11-2-counting-sort-and-radix-sort.md)

**Table of contents**

- [Least-significant-digit radix sort](least-significant-digit-radix-sort.md)
  - [Radix sort suffix invariant](radix-sort-suffix-invariant.md)
- [Stable digit sort](stable-digit-sort.md)
- [Radix sort key encoding](radix-sort-key-encoding.md)

## ↑ Ancestors (4)

1. [Sorting algorithm](sorting-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Comparison sort](comparison-sort.md)
- [Least-significant-digit radix sort](least-significant-digit-radix-sort.md)
- [Radix sort](radix-sort.md)
- [Radix sort key encoding](radix-sort-key-encoding.md)
- [Stable record placement in counting sort](stable-record-placement-in-counting-sort.md)
