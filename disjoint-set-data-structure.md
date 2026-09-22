# Disjoint-set data structure

↑ **Parent:** [Data structure](data-structure-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Disjoint-set_data_structure)

A [disjoint-set data structure](disjoint-set-data-structure.md) maintains a [partition of a set](partition-of-a-set.md). Its find operation returns a representative, equal for two elements exactly when they belong to the same block; its union operation merges two blocks. [Kruskal's algorithm](kruskal-s-algorithm.md) uses it to track [connected components of a graph](component-graph-theory.md).

Start with a [singleton set](singleton-mathematics.md) for every stored [set element](element-of-a-set.md). Each [disjoint-set find operation](disjoint-set-find-operation.md) returns a [disjoint-set representative](disjoint-set-representative.md); a [disjoint-set union operation](disjoint-set-union-operation.md) merges the containing [blocks of a set partition](block-of-a-set-partition.md). The interface does not split a [block of a set partition](block-of-a-set-partition.md) or delete a member.[Algorithms, 4th edition by Robert Sedgewick and others; UF.java, class documentation: initial singletons, representative equality and union interface](algorithms-4th-edition-by-robert-sedgewick-and-others/uf-java.md)

The [partition of a set](partition-of-a-set.md) consists of nonempty disjoint [blocks of a set partition](block-of-a-set-partition.md) covering the stored [set](set-split.md); being in the same [block of a set partition](block-of-a-set-partition.md) defines an [equivalence relation](equivalence-relation.md). A [disjoint-set representative](disjoint-set-representative.md) names a whole [block of a set partition](block-of-a-set-partition.md), without requiring a list of its members.

**Table of contents**

- [Union by size](union-by-size.md)
- [Disjoint-set representative](disjoint-set-representative.md)
- [Disjoint-set find operation](disjoint-set-find-operation.md)
- [Disjoint-set union operation](disjoint-set-union-operation.md)
- [Disjoint-set forest](disjoint-set-forest.md)
  - [Union by rank](union-by-rank.md)
  - [Path compression](path-compression.md)
- [Union-find operation bounds](union-find-operation-bounds.md)

## ↑ Ancestors (3)

1. [Data structure](data-structure-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Disjoint-set data structure](disjoint-set-data-structure.md)
- [Inverse Ackermann function](inverse-ackermann-function.md)
- [Kruskal component merging](kruskal-component-merging.md)
- [Union by size](union-by-size.md)
