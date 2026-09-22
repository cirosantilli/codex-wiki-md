# Orientation of a graph

↑ **Parent:** [Graph theory](graph-theory-split.md)

A choice of direction for each edge of an undirected [graph](graph-split.md), producing a [directed graph](directed-graph.md).

An [orientation of a graph](orientation-of-a-graph.md) keeps the same [vertex set](vertex-set.md) and the same individual [edges](edge-of-a-graph.md). For every [edge](edge-of-a-graph.md) $\{u,v\}$ with distinct endpoints, choose exactly one [directed edge](directed-edge.md), either $u\to v$ or $v\to u$. Replacing it by both arrows is a different construction: it doubles the [edges](edge-of-a-graph.md) and permits travel both ways along that connection. In an [orientation of a graph](orientation-of-a-graph.md), the return journey must use another route.[§1.10, printed p. 28: an orientation retains the vertex and edge sets and assigns initial and terminal endpoints](graph-theory-by-reinhard-diestel/the-basics-author-hosted-chapter-preview.md)

All examples below use finite [simple graphs](simple-graph.md): no [self-loops](loop-graph-theory.md) and no [multiple edges](multiple-edges.md). For a [multigraph](multigraph.md), each individual nonloop [edge](edge-of-a-graph.md) receives its own direction, so two [multiple edges](multiple-edges.md) can point in opposite directions. A [self-loop](loop-graph-theory.md) becomes $u\to u$, which is already a [directed cycle](directed-cycle.md) of length one and therefore prevents an [acyclic orientation](acyclic-orientation.md). A finite [simple graph](simple-graph.md) with $m$ [edges](edge-of-a-graph.md) has $2^m$ [orientations of a graph](orientation-of-a-graph.md), since the two choices for each [edge](edge-of-a-graph.md) are independent.

Think of [vertices](vertex-graph-theory.md) as junctions and [edges](edge-of-a-graph.md) as streets. An [orientation of a graph](orientation-of-a-graph.md) makes each street one-way; [reachability](reachability-in-a-graph.md) asks whether a legal journey exists from one specified junction to another. Two useful aims pull in different directions: an [acyclic orientation](acyclic-orientation.md) rules out circular dependencies, while a [strong orientation](strong-orientation.md) permits journeys between every ordered pair of junctions.

**Table of contents**

- [Acyclic orientation](acyclic-orientation.md)
  - [Order-induced acyclic orientation](order-induced-acyclic-orientation.md)
- [Strong orientation](strong-orientation.md)
  - [Robbins' theorem](robbins-theorem.md)
- [Outdegree orientation criterion](outdegree-orientation-criterion.md)

## ↑ Ancestors (5)

1. [Graph theory](graph-theory-split.md)
2. [Foundations of mathematics](foundations-of-mathematics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Acyclic orientation](acyclic-orientation.md)
- [Multiple edges](multiple-edges.md)
- [Orientation of a graph](orientation-of-a-graph.md)
- [Outdegree](outdegree.md)
- [Strong orientation](strong-orientation.md)
