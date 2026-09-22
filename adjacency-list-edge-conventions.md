# Adjacency list edge conventions

↑ **Parent:** [Adjacency list](adjacency-list.md)

For a [directed graph](directed-graph.md), store $v$ in $\mathrm{Adj}[u]$ for the [edge](edge-of-a-graph.md) $u\to v$. The reverse [edge](edge-of-a-graph.md) $v\to u$ is separate and is stored only if it exists. Consequently, list length is [outdegree](outdegree.md), not [indegree](indegree.md), and each directed [edge](edge-of-a-graph.md) contributes one entry in total. An incoming-list index is additional storage.[Digraph.java, addEdge, adj and outdegree: one entry in the tail's collection; indegree is maintained separately](algorithms-4th-edition-by-robert-sedgewick-and-others/digraph-java.md)

Orient the seven [edges](edge-of-a-graph.md) of our example from earlier to later labels. The resulting [directed graph](directed-graph.md) has

$$
\begin{aligned}
\mathrm{Adj}[A]&=(B,C), & \mathrm{Adj}[B]&=(C), & \mathrm{Adj}[C]&=(D),\\
\mathrm{Adj}[D]&=(E,F), & \mathrm{Adj}[E]&=(F), & \mathrm{Adj}[F]&=().
\end{aligned}
$$

There are now seven entries, with [outdegrees](outdegree.md) $(2,1,1,2,1,0)$. In particular, $F$ needs an empty list even though it is reached from $D,E$: incoming [edges](edge-of-a-graph.md) do not make $F$'s outgoing list nonempty. Replacing each directed [edge](edge-of-a-graph.md) by an [undirected graph](undirected-graph.md) connection would lose this distinction.

Our running [simple graph](simple-graph.md) excludes [self-loops](loop-graph-theory.md) and repeated [edges](edge-of-a-graph.md). If those restrictions are relaxed, specify how the [adjacency list](adjacency-list.md) encodes them. Here an undirected [self-loop](loop-graph-theory.md) at $u$ contributes two copies of $u$ to $\mathrm{Adj}[u]$, matching its contribution of two to the [degree of a vertex](degree-graph-theory.md). A directed [self-loop](loop-graph-theory.md) contributes one copy, and one each to [outdegree](outdegree.md) and [indegree](indegree.md). Distinct parallel [edges](edge-of-a-graph.md) retain distinct entries; a [multigraph](multigraph.md)'s list length can therefore exceed its number of distinct [neighbours](neighbour-of-a-vertex.md).[Graph.java, class documentation: parallel edges and two-entry undirected self-loop convention; addEdge applies both insertions even when v equals w](algorithms-4th-edition-by-robert-sedgewick-and-others/graph-java.md)[Digraph.java, class documentation and addEdge: parallel edges permitted; a directed self-loop adds one outgoing entry and increments indegree once](algorithms-4th-edition-by-robert-sedgewick-and-others/digraph-java.md)

For example, add one undirected [self-loop](loop-graph-theory.md) at $A$ to the seven-[edge](edge-of-a-graph.md) example. Its list becomes $(B,C,A,A)$, the [vertex degree](degree-graph-theory.md) of $A$ becomes four, and the total entry count becomes sixteen for eight [edges](edge-of-a-graph.md). If an application instead stores a [self-loop](loop-graph-theory.md) once, it must account for its doubled undirected [vertex degree](degree-graph-theory.md) separately. In a [weighted graph](weighted-graph.md), an entry can be an [ordered pair](ordered-pair.md) $(v,w)$ meaning destination $v$ and weight $w$; the weight belongs to the [edge](edge-of-a-graph.md), not to the destination [vertex](vertex-graph-theory.md).

## ↑ Ancestors (4)

1. [Adjacency list](adjacency-list.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
