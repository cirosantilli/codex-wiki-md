<h1 id="14/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The coefficient matrix is a [Vandermonde matrix](../../../../../vandermonde-matrix.md), with determinant

$$
\det\begin{pmatrix}1&1&1\\a&b&c\\a^2&b^2&c^2\end{pmatrix}=(b-a)(c-a)(c-b).
$$

Therefore a nonzero solution exists exactly when

$$
\boxed{a=b\quad\text{or}\quad a=c\quad\text{or}\quad b=c.}
$$

For example if $a=b$, the first two columns are equal and $(1,-1,0)$ is a solution. If exactly two parameters agree, the distinct remaining column is independent of the repeated one, so the [kernel](../../../../../kernel-of-a-linear-map-split.md) has dimension one. If all three agree, only $x+y+z=0$ remains, giving a two-dimensional [kernel](../../../../../kernel-of-a-linear-map-split.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [14](../../14.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
