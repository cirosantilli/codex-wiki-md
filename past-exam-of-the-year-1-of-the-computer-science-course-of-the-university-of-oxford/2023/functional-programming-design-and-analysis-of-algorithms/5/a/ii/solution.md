<h1 id="5/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use source $1$, as in the preceding part. The [Dijkstra algorithm](../../../../../../dijkstra-algorithm.md) extracts vertices in the order **$1,3,4,2$**. Distances after relaxing the outgoing [edges](../../../../../../edge-of-a-graph.md) of each extracted vertex are

$$
\begin{array}{c|rrrr}
\text{extracted vertex}&d[1]&d[2]&d[3]&d[4]\\\hline
\text{initial}&0&\infty&\infty&\infty\\
1&0&6&2&\infty\\
3&0&5&2&3\\
4&0&4&2&3\\
2&0&4&2&3
\end{array}
$$

The [shortest path](../../../../../../shortest-path.md) to $2$ is $1\to3\to4\to2$, with weight $2+1+1=4$; the direct route to $2$ and the route via $3\to2$ are both heavier.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
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
