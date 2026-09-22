<h1 id="s/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take a shortest allowed simple [graph path](../../../../../path-in-a-graph.md). If it does not use $k$ as an intermediate [vertex](../../../../../vertex-graph-theory.md), its length is at least $u_{ij}^{(k-1)}$. If it does, simplicity makes $k$ occur only once. Splitting there gives an $i$--$k$ path and a $k$--$j$ path whose intermediate [vertices](../../../../../vertex-graph-theory.md) are in $\{1,\ldots,k-1\}$. Their lengths are at least the respective two minima. In either case,

$$
\boxed{u_{ij}^{(k)}\ge\min\{u_{ij}^{(k-1)},u_{ik}^{(k-1)}+u_{kj}^{(k-1)}\}.}
$$

For identical endpoints use the usual empty path of length zero.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [S](../../../s.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
