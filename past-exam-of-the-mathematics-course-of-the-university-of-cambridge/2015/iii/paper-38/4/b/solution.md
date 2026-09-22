<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Run [Breadth-first search](../../../../../../breadth-first-search.md) separately in every component of the [undirected graph](../../../../../../undirected-graph.md). Give a starting vertex colour zero and each newly discovered neighbour the opposite colour. Reject if an edge joins two vertices with the same assigned colour; otherwise accept after all components have been explored.

If the algorithm accepts, its assignments constitute a [graph colouring](../../../../../../graph-coloring.md) with two colours. If it rejects, the two search-tree paths and the conflicting edge contain an [odd cycle](../../../../../../odd-cycle.md), on which alternating two colours cannot close consistently. Equivalently, a valid [graph colouring](../../../../../../graph-coloring.md) with two colours fixes the parity of every path from a component's root, so the detected conflict is impossible in a two-colourable graph. The [Breadth-first search](../../../../../../breadth-first-search.md) work is $O(|V|+|E|)$ with adjacency lists. Therefore

$$
\boxed{\text{two-colourability is in }\mathbf P.}
$$

This is also the [two-colourability criterion for bipartite graphs](../../../../../../two-colourability-criterion-for-bipartite-graphs.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
