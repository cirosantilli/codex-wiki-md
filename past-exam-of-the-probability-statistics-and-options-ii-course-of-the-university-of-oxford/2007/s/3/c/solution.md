<h1 id="s/3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Initialize an $n\times n$ array $d$ with $d_{ii}=0$ and $d_{ij}=a_{ij}$ for $i\ne j$. For $k=1,\ldots,n$, replace every entry in place by

$$
d_{ij}\leftarrow\min\{d_{ij},d_{ik}+d_{kj}\}.
$$

This is the [Floyd-Warshall algorithm](../../../../../floyd-warshall-algorithm.md). At the start of stage $k$, the induction hypothesis is $d_{ij}=u_{ij}^{(k-1)}$. During that stage, row $k$ and column $k$ do not change: $d_{kk}=0$ and no negative cycle can lower it. Hence the operands $d_{ik},d_{kj}$ remain the stage-start values even with in-place updates. Part (b) proves that after the stage every entry is $u_{ij}^{(k)}$. Induction gives all shortest path lengths after stage $n$. The algorithm uses $n^2$ stored lengths and $O(n^3)$ arithmetic operations, with only a fixed number of loop counters beyond the array.

## ↑ Ancestors (13)

1. [C](../c.md)
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
