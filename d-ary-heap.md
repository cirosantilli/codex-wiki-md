# d-ary heap

↑ **Parent:** [Heap data structure](heap-data-structure.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/d-ary_heap)

A [heap data structure](heap-data-structure.md) stored as a complete rooted tree with up to $d$ children per [vertex](vertex-graph-theory.md), where $d\geq2$. The final level is filled from left to right. For zero-based [array](array-data-structure.md) storage, the parent of entry $i>0$ is $\lfloor(i-1)/d\rfloor$, and its child number $j\in\{0,\ldots,d-1\}$ has index $di+j+1$ when that index is inside the active heap. There are at most $O(1+\log_d n)$ levels containing $n$ entries.

**Table of contents**

- [d-ary min-heap](d-ary-min-heap.md)

## ↑ Ancestors (4)

1. [Heap data structure](heap-data-structure.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [D-ary min-heap](d-ary-min-heap.md)
