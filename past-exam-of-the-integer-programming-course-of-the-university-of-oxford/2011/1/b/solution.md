<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the maximum-weight version of [Kruskal's algorithm](../../../../kruskal-s-algorithm.md): sort the [edges](../../../../edge-of-a-graph.md) by decreasing weight, start with no [edges](../../../../edge-of-a-graph.md), and add an [edge](../../../../edge-of-a-graph.md) exactly when it joins different current [connected components of a graph](../../../../component-graph-theory.md). For the maximum over all [forests](../../../../forest.md), skip negative-weight [edges](../../../../edge-of-a-graph.md); removing a negative [edge](../../../../edge-of-a-graph.md) always preserves a [forest](../../../../forest.md) and increases its weight. Zero-weight [edges](../../../../edge-of-a-graph.md) are optional. The [matroid greedy algorithm](../../../../matroid-greedy-algorithm.md) for the [graphic matroid](../../../../graphic-matroid.md) proves this procedure optimal; it maximizes over independent sets rather than requiring a full basis.

The positive [edges](../../../../edge-of-a-graph.md) are considered in the order

$$
12:9,\quad15:8,\quad25:7,\quad23:4,\quad35:3.
$$

Admit $12$ and $15$. Reject $25$, since it closes the triangle on $1,2,5$. Admit $23$. Reject $35$, since $3$ and $5$ are already joined by the path $3,2,1,5$. Skip both negative [edges](../../../../edge-of-a-graph.md) incident with vertex four. Therefore

$$
\boxed{F^*=\{12,15,23\},\qquad w(F^*)=9+8+4=21.}
$$

Vertex four is isolated. Requiring a [spanning tree](../../../../spanning-tree.md) would force a negative [edge](../../../../edge-of-a-graph.md) and solve a different optimization problem. With a [disjoint-set data structure](../../../../disjoint-set-data-structure.md), sorting dominates the running time, giving $O(|E|\log|E|)$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the integer programming course of the University of Oxford](../../../split.md)
5. [Integer programming course of the University of Oxford](../../../../integer-programming-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
