<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With an [adjacency list](../../../../../adjacency-list.md), initialization and the outer loop cost $O(|V|)$. Each [vertex](../../../../../vertex-graph-theory.md) is visited once, and the adjacency scans inspect each [edge of a graph](../../../../../edge-of-a-graph.md) twice, once from each endpoint. The total worst-case time is therefore **$O(|V|+|E|)$**, with $O(|V|)$ labels and recursion-stack space. An [adjacency matrix](../../../../../adjacency-matrix.md) representation instead incurs $O(|V|^2)$ scanning time.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
