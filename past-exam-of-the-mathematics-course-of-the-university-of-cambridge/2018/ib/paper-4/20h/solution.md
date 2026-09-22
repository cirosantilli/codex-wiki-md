<h1 id="20h/solution">Solution</h1>

↑ **Parent:** [20H](../20h.md)

A cut is a partition $(S,T)$ of the vertices with the source in $S$ and sink in $T$; its capacity is the sum of capacities of directed edges from $S$ to $T$. The [max-flow min-cut theorem](../../../../../max-flow-min-cut-theorem.md) says that maximum flow value equals minimum cut capacity. With integral capacities, there is an [integral max-flow theorem](../../../../../integral-max-flow-theorem.md) attaining the maximum.

Construct a [bipartite graph](../../../../../bipartite-graph.md) with one vertex for each row and column and an edge $r_i\to c_j$ whenever $A_{ij}=1$. Add source-to-row and column-to-sink edges of capacity $1$, and give row-to-column edges infinite capacity. An integral flow is precisely a set of independent $1$s, so its maximum value is the largest such set.

A finite-capacity cut places some rows on the sink side and some columns on the source side; these lines cover every $1$, since an uncovered row-to-column edge would cross the cut with infinite capacity. Its capacity is the number of selected lines. Conversely every line cover defines such a cut. Max-flow min-cut therefore proves **the maximum number of independent $1$s equals the minimum number of covering lines**, the matrix form of [Kőnig's theorem for bipartite matching](../../../../../konig-s-theorem-graph-theory.md).

## ↑ Ancestors (10)

1. [20H](../20h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
