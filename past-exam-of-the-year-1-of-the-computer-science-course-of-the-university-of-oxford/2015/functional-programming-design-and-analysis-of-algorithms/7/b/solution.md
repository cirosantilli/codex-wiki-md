<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In a [bipartite graph](../../../../../bipartite-graph-split.md), successive vertices along an edge lie in opposite parts. Following a [cycle](../../../../../permutation-cycle.md) alternates parts at each step, so returning to the starting part requires an [even](../../../../../even-function.md) number of edges. Thus a bipartite graph contains no [odd cycle](../../../../../odd-cycle.md).

Conversely, choose a rooted [spanning forest](../../../../../spanning-forest.md) and colour each vertex by the parity of its depth in its component's tree. Suppose an edge $uv$ had equally coloured endpoints. The unique tree path from $u$ to $v$ has length

$$
\operatorname{depth}(u)+\operatorname{depth}(v)
-2\operatorname{depth}(\operatorname{LCA}(u,v)),
$$

which is even. Adjoining $uv$ makes an [odd cycle](../../../../../odd-cycle.md). Therefore, if there are no odd cycles, every edge joins opposite colours, which supplies the required [bipartition](../../../../../bipartition-of-a-graph.md).

$$
\boxed{G\text{ is bipartite}\iff G\text{ has no odd cycle}.}
$$

This is the [odd-cycle characterization of bipartite graphs](../../../../../odd-cycle-characterization-of-bipartite-graphs.md). The argument applies separately to every [connected component](../../../../../connected-component.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
