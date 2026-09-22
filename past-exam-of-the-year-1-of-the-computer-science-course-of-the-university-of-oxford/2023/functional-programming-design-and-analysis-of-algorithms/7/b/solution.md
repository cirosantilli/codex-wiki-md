<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write each undirected [edge](../../../../../edge-of-a-graph.md) with its smaller endpoint first. [Kruskal's algorithm](../../../../../kruskal-s-algorithm.md) orders candidates first by weight and then lexicographically:

$$
\begin{array}{c|r|l}
\text{edge}&\text{weight}&\text{action}\\\hline
(4,6)&1&\text{add}\\
(1,3)&2&\text{add}\\
(3,4)&2&\text{add}\\
(1,4)&3&\text{reject: closes a cycle}\\
(4,5)&3&\text{add}\\
(5,6)&3&\text{reject: closes a cycle}\\
(1,2)&4&\text{add and finish}
\end{array}
$$

Thus the requested addition order is

$$
\boxed{(4,6),\ (1,3),\ (3,4),\ (4,5),\ (1,2),}
$$

and the [minimum spanning tree](../../../../../minimum-spanning-tree.md) has total weight **$12$**. Five accepted edges connect all six vertices, so the remaining weight-four edges need not be scanned.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
