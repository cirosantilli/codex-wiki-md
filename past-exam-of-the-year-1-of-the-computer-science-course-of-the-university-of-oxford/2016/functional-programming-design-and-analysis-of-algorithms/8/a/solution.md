<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [greedy algorithm](../../../../../greedy-algorithm.md) **commits to a locally best available choice and then continues on the remaining problem without revising earlier choices**. Correctness requires proving that such choices can belong to an optimal solution; local attractiveness alone is insufficient.

[Kruskal's algorithm](../../../../../kruskal-s-algorithm.md) processes the edges of an undirected weighted graph in nondecreasing weight order. It accepts the next edge exactly when its endpoints lie in different components of the currently chosen forest, thereby preserving the absence of a [cycle](../../../../../permutation-cycle.md). This is greedy because it always chooses a cheapest available edge compatible with the forest constraint and never retracts an accepted edge.

The [Kruskal safe edge](../../../../../kruskal-safe-edge.md) argument explains why the choice works: if a minimum [spanning tree](../../../../../spanning-tree.md) extending the current forest lacks the chosen edge, adding that edge creates a [cycle](../../../../../permutation-cycle.md); an edge on that cycle crossing the same component boundary can be removed without decreasing connectivity. Such a crossing edge cannot be lighter than the chosen eligible edge, so the exchange does not increase total weight. The new minimum [spanning tree](../../../../../spanning-tree.md) includes the greedy choice. For a disconnected graph the same construction yields a minimum spanning forest rather than a single [spanning tree](../../../../../spanning-tree.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
