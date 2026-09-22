# Counting sort

↑ **Parent:** [Sorting algorithm](sorting-algorithm.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Counting_sort)

[Counting sort](counting-sort.md) uses [integer](integer.md) [sort keys](sort-key.md) in $\{0,\ldots,K-1\}$ directly as indices into an [array](array-data-structure.md) of counts. Constant-cost counting and indexing give $O(n+K)$ [time complexity](time-complexity.md) in [Big O notation](big-o-notation.md). To retain complete [sorting records](sorting-record.md), cumulative counts locate their [output](output-computing.md) ranges; filling each range from its end while scanning the [input](input-computer-science.md) backwards gives [stable sorting](stable-sorting.md). Emitting bare [sort keys](sort-key.md) from counts would discard associated data. The $K$ term matters when the key range is large.[Theorem 11.7 and stability](open-data-structures-an-introduction-by-pat-morin/11-2-counting-sort-and-radix-sort.md)

## ↑ Ancestors (4)

1. [Sorting algorithm](sorting-algorithm.md)
2. [Algorithm](algorithm.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Comparison sort](comparison-sort.md)
- [Counting sort](counting-sort.md)
- [Radix sort](radix-sort.md)
