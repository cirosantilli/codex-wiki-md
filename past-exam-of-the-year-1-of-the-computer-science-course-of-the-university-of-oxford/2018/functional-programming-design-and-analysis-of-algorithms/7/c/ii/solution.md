<h1 id="7/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Replace [breadth-first search](../../../../../../breadth-first-search.md) by [Dijkstra's algorithm](../../../../../../dijkstra-algorithm.md) from $s$, using the positive [edge weights](../../../../../../edge-weight.md) to compute $D(v)$. The [strongly connected components](../../../../../../strongly-connected-component.md), the [condensation graph](../../../../../../condensation-graph.md) and the reverse-[topological order](../../../../../../topological-order.md) propagation are unchanged, because reachability ignores weights. Only the label assigned to a reachable [vertex](../../../../../../vertex-graph-theory.md) changes.

With a [binary heap](../../../../../../binary-heap.md), the total time is **$O((|V|+|E|)\log |V|)$**, including the linear component-processing stages. More specialized priority queues give their corresponding shortest-path bounds. The proof still compares the precomputed distances from $s$; it must not add the weight of a path from $u$ to the candidate, which would optimize a different quantity.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [7](../../../7.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
