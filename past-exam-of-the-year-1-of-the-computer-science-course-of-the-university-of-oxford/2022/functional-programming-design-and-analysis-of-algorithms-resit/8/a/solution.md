<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Start [Prim's algorithm](../../../../../prim-s-algorithm.md) at [vertex](../../../../../vertex-graph-theory.md) $1$, since the source does not specify a starting [vertex](../../../../../vertex-graph-theory.md). Write every undirected [edge](../../../../../edge-of-a-graph.md) with its smaller endpoint first. With lexicographic tie-breaking, the accepted [edges](../../../../../edge-of-a-graph.md) are **$(1,2),(1,3),(2,4),(4,6),(4,5)$**, of total weight **9**.

Initially $(1,2)$ is the cheapest crossing [edge](../../../../../edge-of-a-graph.md). The next minimum is a weight-two tie between $(1,3)$ and $(2,4)$, so choose $(1,3)$. Then the weight-two tie between $(2,4)$ and $(3,4)$ is resolved in favour of $(2,4)$. Adding [vertex](../../../../../vertex-graph-theory.md) $4$ exposes the weight-one [edge](../../../../../edge-of-a-graph.md) $(4,6)$, which is selected next. Finally $(4,5)$ precedes $(5,6)$ among the weight-three choices. Every accepted [edge](../../../../../edge-of-a-graph.md) crosses from the existing tree to a new [vertex](../../../../../vertex-graph-theory.md), as required by the [minimum spanning tree cut property](../../../../../minimum-spanning-tree-cut-property.md). A different starting [vertex](../../../../../vertex-graph-theory.md) can produce a different accepted-edge order; the displayed answer fixes that unspecified choice. The algorithm is named for [Robert C. Prim](../../../../../robert-c-prim.md).

## ↑ Ancestors (12)

1. [A](../a.md)
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
