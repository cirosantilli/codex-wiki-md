<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Sort [edges](../../../../../edge-of-a-graph.md) by weight and then lexicographically. [Kruskal's algorithm](../../../../../kruskal-s-algorithm.md) accepts **$(1,2),(4,6),(1,3),(2,4),(4,5)$**, again of total weight **9**.

The two weight-one [edges](../../../../../edge-of-a-graph.md) $(1,2),(4,6)$ join different components. Among weight-two [edges](../../../../../edge-of-a-graph.md), $(1,3)$ is accepted, then $(2,4)$ joins the two larger components; $(3,4)$ would now create a cycle and is rejected. Among weight-three [edges](../../../../../edge-of-a-graph.md), $(1,4)$ is rejected for the same reason, and $(4,5)$ joins the remaining [vertex](../../../../../vertex-graph-theory.md). Five accepted [edges](../../../../../edge-of-a-graph.md) connect all six [vertices](../../../../../vertex-graph-theory.md), so the algorithm can stop. The [disjoint-set data structure](../../../../../disjoint-set-data-structure.md) implements precisely these component tests. The eponym is [Joseph Kruskal](../../../../../joseph-kruskal.md).

## ↑ Ancestors (12)

1. [B](../b.md)
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
