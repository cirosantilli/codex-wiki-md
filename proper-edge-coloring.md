# Proper edge coloring

↑ **Parent:** [Edge coloring](edge-coloring.md)

A [proper edge colouring](proper-edge-coloring.md) gives different labels to any two distinct [edges](edge-of-a-graph.md) sharing a [vertex](vertex-graph-theory.md). We work with finite [undirected graphs](undirected-graph.md) without [self-loops](loop-graph-theory.md); distinct parallel [edges](edge-of-a-graph.md) in a [multigraph](multigraph.md) must also have different colours. For a [simple graph](simple-graph.md), whose [edges](edge-of-a-graph.md) are two-element [sets](set-split.md), the condition is

$$
e\ne f,\quad e\cap f\ne\varnothing\quad\Longrightarrow\quad c(e)\ne c(f).
$$

Every [colour class](colour-class.md) $M_i=\{e\in E(G):c(e)=i\}$ is a [matching in a graph](matching-graph-theory.md). Conversely, a [set partition](set-partition.md) of the [edges](edge-of-a-graph.md) into [matchings in a graph](matching-graph-theory.md) supplies a [proper edge colouring](proper-edge-coloring.md). Thus minimizing colours means grouping all the [edges](edge-of-a-graph.md) into as few [matchings in a graph](matching-graph-theory.md) as possible.

The [line graph](line-graph.md) makes the relationship with [proper vertex colouring](proper-vertex-coloring.md) explicit: replace each original [edge](edge-of-a-graph.md) by a [vertex](vertex-graph-theory.md), joining two new [vertices](vertex-graph-theory.md) exactly when their original [edges](edge-of-a-graph.md) share an endpoint. A [proper edge colouring](proper-edge-coloring.md) of $G$ becomes a [proper vertex colouring](proper-vertex-coloring.md) of its [line graph](line-graph.md) $L(G)$, so $\chi\prime(G)=\chi(L(G))$. For a [multigraph](multigraph.md), retain a distinct new [vertex](vertex-graph-theory.md) for each parallel [edge](edge-of-a-graph.md).[Line graphs and edge coloring, slide 1: line graph identity](line-graphs-and-edge-coloring.md)

**Table of contents**

- [Edge coloring as scheduling](edge-coloring-as-scheduling.md)

## ↑ Ancestors (7)

1. [Edge coloring](edge-coloring.md)
2. [Graph coloring](graph-coloring.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
