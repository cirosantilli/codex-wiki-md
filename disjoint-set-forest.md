# Disjoint-set forest

↑ **Parent:** [Disjoint-set data structure](disjoint-set-data-structure.md)

A [disjoint-set forest](disjoint-set-forest.md) represents each [block of a set partition](block-of-a-set-partition.md) by a [rooted tree](rooted-tree.md). Each [set element](element-of-a-set.md) stores a pointer to its [parent in a rooted tree](parent-in-a-rooted-tree.md); the [root of a tree](root-of-a-tree.md) stores a pointer to itself as a stopping convention. These self-pointers are sentinels, omitted from the [forest](forest.md)'s [edges](edge-of-a-graph.md). Following parent pointers reaches the [disjoint-set representative](disjoint-set-representative.md), the [root of a tree](root-of-a-tree.md). An indexed [array](array-data-structure.md) `parent` suffices when members are numbered consecutively. The [rooted trees](rooted-tree.md) encode membership; their [edges](edge-of-a-graph.md) need not be [edges](edge-of-a-graph.md) of any input [graph](graph-split.md).

To link different [blocks of a set partition](block-of-a-set-partition.md), point one [root of a tree](root-of-a-tree.md) at the other [root of a tree](root-of-a-tree.md). Linking roots preserves every old membership and joins exactly the two [rooted trees](rooted-tree.md). Arbitrarily reparenting a nonroot could detach only part of a [block of a set partition](block-of-a-set-partition.md), so it would not implement the required [disjoint-set union operation](disjoint-set-union-operation.md). The [disjoint-set find operation](disjoint-set-find-operation.md) terminates because each nonroot pointer moves towards the unique [root of a tree](root-of-a-tree.md); linking distinct roots cannot introduce a [graph cycle](cycle-in-a-graph.md).

**Table of contents**

- [Union by rank](union-by-rank.md)
- [Path compression](path-compression.md)

## ↑ Ancestors (4)

1. [Disjoint-set data structure](disjoint-set-data-structure.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Disjoint-set forest](disjoint-set-forest.md)
- [Disjoint-set union operation](disjoint-set-union-operation.md)
- [Path compression](path-compression.md)
