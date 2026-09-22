# Why the 2-core is unique

↑ **Parent:** [2-core of a graph](2-core-of-a-graph.md)

Suppose $T$ is any [vertex set](vertex-set.md) whose [induced subgraph](induced-subgraph.md) has every [degree of a vertex](degree-graph-theory.md) at least two. No [vertex](vertex-graph-theory.md) of $T$ can be the first one deleted from $T$: before such a deletion it still has its two [graph neighbours](neighbour-of-a-vertex.md) within $T$, contradicting eligibility for deletion. Consequently every qualifying $T$ survives every legal deletion sequence. Once deletion stops, its remainder $R$ itself qualifies, because every surviving [vertex](vertex-graph-theory.md) has at least two surviving [graph neighbours](neighbour-of-a-vertex.md). Therefore $T\subseteq R$ for every qualifying $T$: $G[R]$ is the unique maximum and the final remainder is independent of deletion order. The intermediate [FIFO queues](fifo-queue.md) and deletion orders can differ.

There is also a direct existence argument. If $A$ and $B$ qualify, then $A\cup B$ qualifies: each [vertex](vertex-graph-theory.md) retains at least the two [graph neighbours](neighbour-of-a-vertex.md) it already had in $A$ or in $B$. Taking the [union](set-union.md) of all qualifying [vertex sets](vertex-set.md) produces the maximum. This rules out a collection of competing, incomparable inclusion-maximal answers. It also explains why restricting the search to connected [subgraphs](subgraph.md) would change the question.

## ↑ Ancestors (6)

1. [2-core of a graph](2-core-of-a-graph.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [2-core of a graph](2-core-of-a-graph.md)
