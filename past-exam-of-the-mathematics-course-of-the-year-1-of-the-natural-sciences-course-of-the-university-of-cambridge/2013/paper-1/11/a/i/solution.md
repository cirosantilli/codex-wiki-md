<h1 id="11/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use [Gaussian elimination](../../../../../../gaussian-elimination.md) on the [augmented matrix](../../../../../../augmented-matrix.md). First take $R_2\leftarrow R_2-R_1$ and $R_3\leftarrow R_3-2R_1$, then $R_3\leftarrow4R_3-3R_2$:

$$
\left(\begin{array}{ccc|c}1&2&3&14\\1&-2&1&0\\2&1&-1&1\end{array}\right)
\longrightarrow
\left(\begin{array}{ccc|c}1&2&3&14\\0&-4&-2&-14\\0&-3&-7&-27\end{array}\right)
\longrightarrow
\left(\begin{array}{ccc|c}1&2&3&14\\0&-4&-2&-14\\0&0&-22&-66\end{array}\right).
$$

By [back substitution](../../../../../../back-substitution.md), the last row gives $z=3$, the second gives $-4y-6=-14$ and hence $y=2$, and the first gives $x+4+9=14$. Thus

$$
\boxed{(x,y,z)=(1,2,3).}
$$

The right-hand side has been transformed in every row operation, preserving the solution set.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [11](../../../11.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
