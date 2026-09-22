<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a connected weighted [undirected graph](../../../../../undirected-graph.md), [Kruskal's algorithm](../../../../../kruskal-s-algorithm.md) begins with each vertex as a separate component and no selected edges. Sort all edges into nondecreasing weight order. Inspect them in that order and add an edge exactly when its endpoints lie in different current components. Merge those components after an addition; stop once $|V|-1$ edges have been accepted. A [disjoint-set data structure](../../../../../disjoint-set-data-structure.md) implements the component tests and merges.

The accepted edges always form a [forest](../../../../../forest.md), because an edge whose endpoints were already connected is rejected. To prove optimality, use the invariant that some [minimum spanning tree](../../../../../minimum-spanning-tree.md) contains every accepted edge. It holds initially. Suppose the next accepted edge is $e=uv$, and let $T$ be a [minimum spanning tree](../../../../../minimum-spanning-tree.md) extending the current [forest](../../../../../forest.md). If $e\in T$, nothing changes. Otherwise adding $e$ to $T$ makes a unique [graph cycle](../../../../../cycle-in-a-graph.md). The [graph path](../../../../../path-in-a-graph.md) from $u$ to $v$ in $T$ must cross the [graph cut](../../../../../graph-cut.md) between the current component of $u$ and the remaining vertices, so that [graph cycle](../../../../../cycle-in-a-graph.md) contains an edge $f$ crossing this [graph cut](../../../../../graph-cut.md). No accepted edge crosses it. Furthermore $w(e)\leq w(f)$: any strictly lighter crossing edge would already have been processed and accepted, since its endpoints could not then have been connected without also being connected now.

Replace $f$ by $e$. The resulting [spanning tree](../../../../../spanning-tree.md) still contains all previously accepted edges and has cost at most that of $T$, so it too is a [minimum spanning tree](../../../../../minimum-spanning-tree.md). This is the [exchange argument](../../../../../exchange-argument.md) establishing the invariant. At termination the selected edges themselves form a [spanning tree](../../../../../spanning-tree.md), hence

$$
\boxed{\text{Kruskal's algorithm returns a minimum spanning tree}.}
$$

Equal weights cause no difficulty; they may give several optima. On a disconnected [graph](../../../../../graph-split.md), processing all edges instead returns a [minimum spanning forest](../../../../../minimum-spanning-forest.md). Sorting costs $O(|E|\log |E|)$, with near-linear additional cost using an efficient [disjoint-set data structure](../../../../../disjoint-set-data-structure.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2003](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
