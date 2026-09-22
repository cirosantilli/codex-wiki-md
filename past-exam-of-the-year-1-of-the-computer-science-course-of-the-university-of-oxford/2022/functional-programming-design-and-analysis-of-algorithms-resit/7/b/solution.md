<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The intermediate states of the [Bellman-Ford algorithm](../../../../../bellman-ford-algorithm.md) depend on [edge](../../../../../edge-of-a-graph.md) order. Specify in-place [edge relaxation](../../../../../edge-relaxation.md) in lexicographic directed-edge order:

$$
(1,2),(1,3),(2,3),(2,4),(3,5),(5,2),(5,4).
$$

Starting with $(0,\infty,\infty,\infty,\infty)$, the first pass changes the vector as follows; omitted relaxations make no change:

$$
\begin{array}{c|ccccc}
\text{after edge}&d_1&d_2&d_3&d_4&d_5\\\hline
(1,2)&0&3&\infty&\infty&\infty\\
(1,3)&0&3&2&\infty&\infty\\
(2,4)&0&3&2&6&\infty\\
(3,5)&0&3&2&6&4\\
(5,4)&0&3&2&5&4
\end{array}
$$

The next pass makes no change, allowing early termination. If all $|V|-1=4$ passes are performed, passes two through four retain **$(0,3,2,5,4)$**.

For the synchronous convention, where every relaxation reads only the previous row, the [Synchronous Bellman-Ford recurrence](../../../../../synchronous-bellman-ford-recurrence.md) instead gives

$$
\begin{array}{c|ccccc}
\text{allowed edges}&d_1&d_2&d_3&d_4&d_5\\\hline
0&0&\infty&\infty&\infty&\infty\\
1&0&3&2&\infty&\infty\\
2&0&3&2&6&4\\
3&0&3&2&5&4\\
4&0&3&2&5&4
\end{array}
$$

Both conventions reach the same shortest distances. The algorithm's eponyms are [Richard Bellman](../../../../../richard-bellman.md) and [L. R. Ford Jr.](../../../../../l-r-ford-jr.md).

## ↑ Ancestors (12)

1. [B](../b.md)
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
