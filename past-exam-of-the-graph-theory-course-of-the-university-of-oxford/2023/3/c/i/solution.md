<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Add two new [vertices](../../../../../vertex-graph-theory.md) $s,t$ to $G$, joining $s$ to every [vertex](../../../../../vertex-graph-theory.md) of $U$ and $t$ to every [vertex](../../../../../vertex-graph-theory.md) of $W$, with no other new [edges](../../../../../edge-of-a-graph.md). The [vertices](../../../../../vertex-graph-theory.md) $s,t$ are nonadjacent. Suppose $S\subseteq V(G)$ has $|S|<k$. Since $G$ is a [k-connected graph](../../../../../k-connected-graph.md), $G-S$ is a [connected graph](../../../../../connected-graph.md). Both $U\setminus S$ and $W\setminus S$ are nonempty because each original [set](../../../../../set-split.md) has [cardinality](../../../../../cardinality.md) $k$. Choose $u\in U\setminus S$ and $w\in W\setminus S$; a [graph path](../../../../../path-in-a-graph.md) between them in $G-S$ extends to an $s$–$t$ [graph path](../../../../../path-in-a-graph.md) avoiding $S$.

Consequently no fewer than $k$ [vertices](../../../../../vertex-graph-theory.md) can form an $s$–$t$ [vertex separator](../../../../../vertex-separator.md). By [Menger's theorem](../../../../../menger-theorem.md), there are at least $k$ [internally vertex-disjoint paths](../../../../../internally-vertex-disjoint-paths.md) from $s$ to $t$. There cannot be more than $k$, since $s$ has only $k$ [neighbours](../../../../../neighbour-of-a-vertex.md).

Remove $s,t$ from these $k$ [graph paths](../../../../../path-in-a-graph.md). The resulting [graph paths](../../../../../path-in-a-graph.md) in $G$ start at distinct [vertices](../../../../../vertex-graph-theory.md) of $U$, end at distinct [vertices](../../../../../vertex-graph-theory.md) of $W$, and are pairwise [vertex-disjoint paths](../../../../../vertex-disjoint-paths.md): any shared [vertex](../../../../../vertex-graph-theory.md) would have been an internal [vertex](../../../../../vertex-graph-theory.md) common to two of the original [graph paths](../../../../../path-in-a-graph.md). Because there are exactly $k$ [graph paths](../../../../../path-in-a-graph.md), they use every [vertex](../../../../../vertex-graph-theory.md) of $U$ and $W$ as an endpoint. None can pass through another terminal internally, since that terminal already occurs as an endpoint of one of the [vertex-disjoint paths](../../../../../vertex-disjoint-paths.md). Thus there are $k$ [vertex-disjoint paths](../../../../../vertex-disjoint-paths.md) from $U$ to $W$, with some pairing of the endpoints. This is also an immediate application of the [Set version of Menger theorem](../../../../../set-version-of-menger-theorem.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the graph theory course of the University of Oxford](../../../../split.md)
6. [Graph theory course of the University of Oxford](../../../../../graph-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
