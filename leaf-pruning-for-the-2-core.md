# Leaf pruning for the 2-core

↑ **Parent:** [2-core of a graph](2-core-of-a-graph.md)

Use [adjacency lists](adjacency-list.md) and a [FIFO queue](fifo-queue.md) to implement the deletion rule in [time complexity](time-complexity.md) $O(|V|+|E|)$. Compute each initial [degree of a vertex](degree-graph-theory.md) once, mark every [vertex](vertex-graph-theory.md) alive, and put all [vertices](vertex-graph-theory.md) of [degree of a vertex](degree-graph-theory.md) zero or one in the [FIFO queue](fifo-queue.md). Each [vertex](vertex-graph-theory.md) is inserted at most once. Repeatedly remove the front [vertex](vertex-graph-theory.md) $v$, mark it dead, and traverse its original [adjacency list](adjacency-list.md). For each still-alive [graph neighbour](neighbour-of-a-vertex.md) $u$, decrease the stored [degree of a vertex](degree-graph-theory.md) of $u$ by one; if it has just become one, append $u$. A [vertex](vertex-graph-theory.md) already queued can drop from one to zero before its turn, but it stays queued and requires no second insertion. Stop when the [FIFO queue](fifo-queue.md) is empty; the alive [vertices](vertex-graph-theory.md) induce $C_2(G)$.

For the displayed example, initially enqueue $(f,g,z)$ in that order. The successive [FIFO queues](fifo-queue.md), after each deletion and all its updates, are

$$
(f,g,z)\xrightarrow{-f}(g,z,e)\xrightarrow{-g}(z,e)\xrightarrow{-z}(e)\xrightarrow{-e}(d)\xrightarrow{-d}().
$$

This explains the delayed deletion of $d$: its initial [degree of a vertex](degree-graph-theory.md) was three, but the relevant [degree of a vertex](degree-graph-theory.md) is always its current one in the surviving [induced subgraph](induced-subgraph.md). Removing only the original [vertices](vertex-graph-theory.md) of [degree of a vertex](degree-graph-theory.md) one would give the wrong answer.

Initialization inspects every [vertex](vertex-graph-theory.md) and every [adjacency list](adjacency-list.md) entry once. During deletion each original [adjacency list](adjacency-list.md) is traversed at most once, so at most $2|E|$ entries are inspected in an [undirected graph](undirected-graph.md). All insertions, removals and stored-degree updates cost constant time each. Thus total [time complexity](time-complexity.md) is $O(|V|+|E|)$ and additional storage, beyond the [adjacency lists](adjacency-list.md), is $O(|V|)$. The cost includes [isolated vertices](isolated-vertex.md); repeatedly rescanning the whole surviving [graph](graph-split.md) after each deletion would lose this bound. The single-threshold [FIFO queue](fifo-queue.md) method is enough for the [2-core](2-core-of-a-graph.md); the full [k-core of a graph](k-core-of-a-graph.md) decomposition computes all thresholds.

## ↑ Ancestors (6)

1. [2-core of a graph](2-core-of-a-graph.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [2-core of a graph](2-core-of-a-graph.md)
