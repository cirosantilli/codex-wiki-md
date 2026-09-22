<h1 id="17g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Suppose first that $G$ is [bipartite](../../../../../../bipartite-graph.md). As one traverses any [cycle in a graph](../../../../../../cycle-in-a-graph.md), its vertices alternate between the two vertex classes. Returning to the initial class therefore requires an [even number](../../../../../../even-number.md) of edges, so $G$ contains no [odd cycle](../../../../../../odd-cycle.md).

Conversely, suppose that $G$ has no [odd cycle](../../../../../../odd-cycle.md). Work separately in each [connected component of a graph](../../../../../../component-graph-theory.md), choose a root $r$, and put

$$
A=\{v:d(r,v)\text{ is even}\},
\qquad
B=\{v:d(r,v)\text{ is odd}\},
$$

where $d$ is the [graph distance](../../../../../../distance-graph-theory.md). If adjacent vertices $u,v$ were in the same class, then $|d(r,u)-d(r,v)|\leq1$ and parity would force $d(r,u)=d(r,v)$. Choose a breadth-first [spanning tree](../../../../../../spanning-tree.md). The two tree paths from $r$ to $u$ and $v$ diverge at some last common vertex; their remaining segments have equal length, and adjoining the edge $uv$ gives an odd cycle. This contradiction shows that every edge joins $A$ to $B$, proving the [odd-cycle characterization of bipartite graphs](../../../../../../odd-cycle-characterization-of-bipartite-graphs.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17G](../../17g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
