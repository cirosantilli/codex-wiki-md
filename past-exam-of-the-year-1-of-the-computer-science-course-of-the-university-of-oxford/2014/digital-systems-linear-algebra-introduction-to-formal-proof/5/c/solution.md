<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Swap the first two rows, then perform $R_2\gets R_2+R_1$ and $R_3\gets R_3-2R_1$. These [elementary row operations](../../../../../elementary-row-operation.md) give

$$
A\sim\begin{pmatrix}1&-2&2&3&-1\\0&0&5&10&-10\\0&0&1&2&-2\end{pmatrix}.
$$

Scale row 2 by $1/5$, subtract it from row 3, and finally subtract twice row 2 from row 1. The [reduced row echelon form](../../../../../reduced-row-echelon-form.md) is

$$
R=\begin{pmatrix}1&-2&0&-1&3\\0&0&1&2&-2\\0&0&0&0&0\end{pmatrix}.
$$

[Elementary row operations](../../../../../elementary-row-operation.md) preserve the [row space](../../../../../row-space.md). The two nonzero rows of $R$ are [linearly independent](../../../../../linear-independence.md), since their leading entries lie in different columns. Hence

$$
\boxed{\text{row-space basis }\{(1,-2,0,-1,3),(0,0,1,2,-2)\},\qquad\operatorname{rank}A=2.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
