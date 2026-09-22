# Red-black tree

↑ **Parent:** [Binary search tree](binary-search-tree.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Red–black_tree)

A [red-black tree](red-black-tree.md) colours each stored node red or black, treats absent-child sentinels as black, permits no red node to have a red child, and gives every path from a node to an absent-child sentinel the same number of black nodes. We also require a black root. These invariants bound its [height of a binary tree](height-of-a-binary-tree.md) by $2\log_2(n+1)$ for $n$ stored keys: a path has at most twice as many real nodes as black nodes, and a [subtree](subtree.md) of [black height](black-height.md) $b$ has at least $2^b-1$ real nodes by [mathematical induction](mathematical-induction.md). The structure therefore supports logarithmic-time directed [binary search tree](binary-search-tree.md) lookup.

**Table of contents**

- [Red-black tree insertion](red-black-tree-insertion.md)
- [All-black red-black tree size criterion](all-black-red-black-tree-size-criterion.md)
- [Black height](black-height.md)

## ↑ Ancestors (5)

1. [Binary search tree](binary-search-tree.md)
2. [Binary tree](binary-tree.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [All-black red-black tree size criterion](all-black-red-black-tree-size-criterion.md)
- [Black height](black-height.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2018/algorithms/1/c/solution.md)
- [Red-black tree](red-black-tree.md)
- [Red-black tree insertion](red-black-tree-insertion.md)
