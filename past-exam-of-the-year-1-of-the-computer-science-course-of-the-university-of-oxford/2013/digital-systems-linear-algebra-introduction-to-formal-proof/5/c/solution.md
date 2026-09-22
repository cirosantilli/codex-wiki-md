<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use [Gaussian elimination](../../../../../gaussian-elimination.md). Subtract twice row 1 from rows 2 and 3:

$$
A\longrightarrow\begin{pmatrix}
1&1&0&2\\0&1&-1&1\\0&-2&2&-2\\0&1&-1&1
\end{pmatrix}.
$$

Now add twice the second row to the third, and subtract the second row from the fourth. This gives the [row echelon form](../../../../../row-echelon-form.md)

$$
\begin{pmatrix}1&1&0&2\\0&1&-1&1\\0&0&0&0\\0&0&0&0\end{pmatrix}.
$$

Its two nonzero rows span the original [row space](../../../../../row-space.md) because reversible [elementary row operations](../../../../../elementary-row-operation.md) preserve that space. They are [linearly independent](../../../../../linear-independence.md), as witnessed by their leading entries in different columns. Thus

$$
\boxed{\operatorname{Row}(A)\text{ has basis }\{(1,1,0,2),(0,1,-1,1)\},\qquad\operatorname{rank}A=2.}
$$

Subtracting the second nonzero row from the first also gives the reduced [row echelon form](../../../../../row-echelon-form.md)

$$
\begin{pmatrix}1&0&1&1\\0&1&-1&1\\0&0&0&0\\0&0&0&0\end{pmatrix},
$$

which is useful for the [null space](../../../../../kernel-of-a-linear-map-split.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
