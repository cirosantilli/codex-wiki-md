<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

To find a [minimum-weight acyclic subgraph](../../../../../minimum-weight-acyclic-subgraph.md), filter to the subgraph $G_-$ containing only **strictly negative-weight [edges](../../../../../edge-of-a-graph.md)**, and run [Kruskal's algorithm](../../../../../kruskal-s-algorithm.md) on those [edges](../../../../../edge-of-a-graph.md), accepting an [edge](../../../../../edge-of-a-graph.md) exactly when it joins different current components. Return the resulting [forest](../../../../../forest.md), with any omitted [vertices](../../../../../vertex-graph-theory.md) regarded as isolated. Zero-weight [edges](../../../../../edge-of-a-graph.md) may be omitted without worsening the objective.

To prove correctness, first remove all nonnegative [edges](../../../../../edge-of-a-graph.md) from any feasible [acyclic graph](../../../../../forest.md); removing them preserves acyclicity and cannot increase weight. Thus an optimum using only negative [edges](../../../../../edge-of-a-graph.md) exists. Inside a connected component of $G_-$, any [forest](../../../../../forest.md) not yet connected can be extended by a negative crossing [edge](../../../../../edge-of-a-graph.md): some such [edge](../../../../../edge-of-a-graph.md) exists because the original component is connected. Adding it preserves acyclicity and strictly reduces total weight. Consequently an optimum must span each component of $G_-$, and its restriction there must be a [minimum spanning tree](../../../../../minimum-spanning-tree.md). [Kruskal's algorithm](../../../../../kruskal-s-algorithm.md) finds exactly the resulting [minimum spanning forest](../../../../../minimum-spanning-forest.md) of $G_-$. This proves optimality among all acyclic subgraphs, including disconnected ones.

With $m_-$ negative [edges](../../../../../edge-of-a-graph.md), filtering costs $O(|V|+|E|)$, sorting costs $O(m_-\log(m_-+1))$, and the [union-find](../../../../../disjoint-set-data-structure.md) operations take $O((|V|+m_-)\alpha(|V|))$ time. A standard overall bound is **$O(|V|+|E|\log(|E|+1))$ time**. If there are no negative [edges](../../../../../edge-of-a-graph.md), the empty [edge](../../../../../edge-of-a-graph.md) set is optimal.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
