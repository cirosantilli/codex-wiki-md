<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the usual implicit convention that the infinite connected [graph](../../../../../../graph-split.md) is a [locally finite graph](../../../../../../locally-finite-graph.md). This is needed for the [simple random walk](../../../../../../simple-random-walk.md) and the finite wired constructions to be defined. Choose finite vertex sets $V_1\subset V_2\subset\cdots$ exhausting $V$, with each [induced subgraph](../../../../../../induced-subgraph.md) $G[V_k]$ connected.

For the [free uniform spanning forest](../../../../../../free-uniform-spanning-forest.md), sample a [uniform spanning tree](../../../../../../uniform-spanning-tree.md) of $G[V_k]$, using only the internal edges. Its limiting law on edge subsets of $G$ is the [free uniform spanning forest](../../../../../../free-uniform-spanning-forest.md) measure:

$$
\boxed{\mathrm{FSF}=\lim_{k\to\infty}\operatorname{UST}(G[V_k]).}
$$

The limit is [weak convergence of probability measures](../../../../../../weak-convergence-of-probability-measures.md) on $\{0,1\}^E$, equivalently convergence of every finite-edge event.

For the [wired uniform spanning forest](../../../../../../wired-uniform-spanning-forest.md), form $G_k^{\mathrm w}$ by identifying every vertex outside $V_k$ to one boundary vertex $\partial_k$. Retain all edges with at least one endpoint in $V_k$, preserve parallel edges, and discard loops at $\partial_k$. Sample a [uniform spanning tree](../../../../../../uniform-spanning-tree.md) of this finite multigraph and restrict it to the original internal edges. The limiting law is

$$
\boxed{\mathrm{WSF}=\lim_{k\to\infty}\operatorname{UST}(G_k^{\mathrm w})\big|_E.}
$$

For each fixed finite set of edges the restriction is unambiguous once $k$ is large. The standard exhaustion theorem guarantees that both limits exist and do not depend on the chosen connected exhaustion. Both are random spanning [forests](../../../../../../forest.md); despite their names, they need not be connected.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 214](../../../paper-214-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
