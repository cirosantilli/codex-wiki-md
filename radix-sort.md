# Radix sort

↑ **Parent:** [Sorting algorithm](sorting-algorithm.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radix_sort)

[Radix sort](radix-sort.md) sorts encoded [sort keys](sort-key.md) a digit at a time. Its least-significant-digit version uses [stable sorting](stable-sorting.md) on each successive digit, often by [counting sort](counting-sort.md). For $d$ digits with $R$ possible values each, it takes $O(d(n+R))$ [time complexity](time-complexity.md) in [Big O notation](big-o-notation.md), assuming constant-cost digit extraction and indexing. [Stable sorting](stable-sorting.md) retains the ordering established by earlier digits when a later digit ties. Both digit access and the direct indexing in [counting sort](counting-sort.md) lie outside the [comparison sort](comparison-sort.md) model, so these bounds do not contradict the [comparison sorting lower bound](comparison-sorting-lower-bound.md).[Theorem 11.8](open-data-structures-an-introduction-by-pat-morin/11-2-counting-sort-and-radix-sort.md)

## ↑ Ancestors (4)

1. [Sorting algorithm](sorting-algorithm.md)
2. [Algorithm](algorithm.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Comparison sort](comparison-sort.md)
- [Radix sort](radix-sort.md)
