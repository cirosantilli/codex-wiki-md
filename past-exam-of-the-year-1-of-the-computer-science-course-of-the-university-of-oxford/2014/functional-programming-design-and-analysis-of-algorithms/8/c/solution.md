<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Run [Kruskal's algorithm](../../../../../kruskal-s-algorithm.md) in nonincreasing order of [edge weight](../../../../../edge-weight.md), accepting an [edge](../../../../../edge-of-a-graph.md) exactly when its endpoints belong to different current [connected components](../../../../../connected-component.md). Use a [disjoint-set data structure](../../../../../disjoint-set-data-structure.md) to test and merge those components. Stop after accepting $|V|-1$ [edges](../../../../../edge-of-a-graph.md).

Equivalently, apply ordinary [Kruskal's algorithm](../../../../../kruskal-s-algorithm.md) to $w'(e)=-w(e)$. For every [spanning tree](../../../../../spanning-tree.md),

$$
\boxed{\sum_{e\in T}w'(e)=-\sum_{e\in T}w(e),}
$$

so minimizing transformed total weight is exactly maximizing original total weight. Thus the output is a [maximum spanning tree](../../../../../maximum-spanning-tree.md). Equal weights may be processed in any fixed order. Sorting dominates the [time complexity](../../../../../time-complexity.md), giving $O(|E|\log |E|+|V|)$ with the usual efficient [disjoint-set data structure](../../../../../disjoint-set-data-structure.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
