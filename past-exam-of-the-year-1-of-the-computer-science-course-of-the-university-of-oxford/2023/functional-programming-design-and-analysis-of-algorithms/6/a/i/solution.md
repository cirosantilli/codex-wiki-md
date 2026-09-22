<h1 id="6/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Increment a single clock on each discovery and finish, starting with clock zero. Lexicographic [depth-first search](../../../../../../depth-first-search.md) gives

$$
\begin{array}{c|rr}
\text{vertex}&d&f\\\hline
1&1&8\\
2&9&10\\
3&2&7\\
4&11&12\\
5&3&4\\
6&5&6
\end{array}
$$

The first search tree has discovery [edges](../../../../../../edge-of-a-graph.md) $1\to3$, $3\to5$, $3\to6$. The edge $5\to1$ returns to an active ancestor. Once that tree finishes, vertex $2$ is a new root whose neighbour $1$ is already finished, and vertex $4$ is the final root. This accounts for all twelve events in the [DFS discovery and finishing times](../../../../../../dfs-discovery-and-finishing-times.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
