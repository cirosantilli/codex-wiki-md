<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Dijkstra algorithm](../../../../../dijkstra-algorithm.md) finalises [vertices](../../../../../vertex-graph-theory.md) in the order **$1,3,2,5,4$**. After finalising $1$, tentative distances to $2,3$ are $3,2$. Finalising $3$ sets the distance to $5$ to $4$. Finalising $2$ sets the distance to $4$ to $6$. Finalising $5$ improves the distance to $4$ to $5$; its [edge](../../../../../edge-of-a-graph.md) to $2$ proposes $5$ and causes no improvement. The final distance vector in [vertex](../../../../../vertex-graph-theory.md) order is **$(0,3,2,5,4)$**. All weights are positive, so every finalisation is justified by the usual [label-setting shortest-path algorithm](../../../../../label-setting-shortest-path-algorithm.md) invariant. The method is named for [Edsger W. Dijkstra](../../../../../edsger-w-dijkstra.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
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
