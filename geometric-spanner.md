# Geometric spanner

↑ **Parent:** [Graph theory](graph-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Geometric_spanner)

A geometric spanner is a [weighted graph](weighted-graph.md) on points in [Euclidean space](euclidean-norm.md), with edge weights equal to their [Euclidean distances](euclidean-distance.md), in which every pair has a [graph path](path-in-a-graph.md) of [length](length.md) at most $t$ times its direct distance. Its [stretch factor](stretch-factor.md) is the largest ratio $d_G(u,v)/\|u-v\|$, where $d_G$ is shortest-path distance. A square's four perimeter edges, without diagonals, give stretch factor $\sqrt2$: adjacent points have ratio one, and diagonal pairs have route [length](length.md) $2$ instead of $\sqrt2$. The aim is to retain short routes with fewer edges than a [complete graph](complete-graph.md). [Gudmundsson, Narasimhan and Smid, Geometric Spanners, §1](https://people.scs.carleton.ca/~michiel/encyc_geometric_spanners.pdf).

## ↑ Ancestors (5)

1. [Graph theory](graph-theory-split.md)
2. [Foundations of mathematics](foundations-of-mathematics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Stretch factor](stretch-factor.md)
