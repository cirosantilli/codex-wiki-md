<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\mathcal T(G)$ be the [finite set](../../../../../../finite-set.md) of [spanning trees](../../../../../../spanning-tree.md) of the [connected graph](../../../../../../connected-graph.md). A [spanning tree](../../../../../../spanning-tree.md) has all the [graph vertices](../../../../../../vertex-graph-theory.md), is connected, and contains no [graph cycle](../../../../../../cycle-in-a-graph.md). Connectedness ensures that at least one exists, for example by repeatedly deleting an [edge](../../../../../../edge-of-a-graph.md) of a [graph cycle](../../../../../../cycle-in-a-graph.md) while retaining connectedness. The [uniform spanning tree](../../../../../../uniform-spanning-tree.md) is the random [edge](../../../../../../edge-of-a-graph.md) set $T$ with

$$
\boxed{\mathbb P(T=t)=\frac1{|\mathcal T(G)|}\quad\text{for each }t\in\mathcal T(G).}
$$

Every [tree](../../../../../../tree-graph-theory.md) has $|V|-1$ [edges](../../../../../../edge-of-a-graph.md), so uniformity is over complete [trees](../../../../../../tree-graph-theory.md), not over arbitrary subsets of that size. Such subsets can be disconnected or cyclic and do not belong to $\mathcal T(G)$. Nor are indicators of the [tree](../../../../../../tree-graph-theory.md) [edges](../../../../../../edge-of-a-graph.md) generally independent. The [matrix-tree theorem](../../../../../../kirchhoff-s-theorem.md) gives $|\mathcal T(G)|$ as any cofactor of the unweighted [Graph Laplacian](../../../../../../laplacian-matrix.md) if a numerical normalizing constant is needed.

This definition uses the ordinary undirected unweighted [graph](../../../../../../graph-split.md) convention. With positive conductances the analogous law for [spanning trees](../../../../../../spanning-tree.md) weights $t$ proportionally to $\prod_{e\in t}c_e$ and is generally not uniform. When the [graph](../../../../../../graph-split.md) has one [graph vertex](../../../../../../vertex-graph-theory.md) the empty [edge](../../../../../../edge-of-a-graph.md) set is the unique [spanning tree](../../../../../../spanning-tree.md), so its [probability](../../../../../../probability.md) is one.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 214](../../../paper-214-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
