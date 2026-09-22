<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $v=f[0,N-1]$, assuming $M,N>0$. By [monotonicity](../../../../../monotonic-function.md), $v$ is at least every value in the first row and at most every value in the last column. Hence

$$
\boxed{\begin{aligned}
v=x&\implies (0,N-1)\text{ is a solution},\\
v<x&\implies \text{discard row }0,\\
v>x&\implies \text{discard column }N-1.
\end{aligned}}
$$

The same observation applies to the top-right corner of any remaining rectangular [subarray](../../../../../subarray.md) of this [monotone matrix](../../../../../monotone-matrix.md).

## ↑ Ancestors (12)

1. [C](../c.md)
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
