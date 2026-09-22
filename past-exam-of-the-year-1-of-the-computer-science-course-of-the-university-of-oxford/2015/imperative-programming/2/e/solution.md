<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

[Monotonicity](../../../../../monotonic-function.md) gives two excluded rectangles:

$$
\boxed{\begin{aligned}
0\leq r\leq i,\quad 0\leq c<j&\implies f[r,c]<x,\\
i\leq r<M,\quad j\leq c<N&\implies f[r,c]>x.
\end{aligned}}
$$

Indeed the first entries are at most $f[i,j-1]$, and the second are at least $f[i,j]$. In particular, the entire splitting row $i$ contains no answer. The only remaining candidates are the upper-right rectangle $r<i,c\geq j$ and the lower-left rectangle $r>i,c<j$. These are the exclusions guaranteed by the given adjacent inequalities; further comparisons may exclude more.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
