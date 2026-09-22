<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Perform the [elementary row operations](../../../../../elementary-row-operation.md) $R_2\gets R_2-R_1$ and $R_3\gets R_3+R_1$, then $R_3\gets R_3-R_2$:

$$
A\sim\begin{pmatrix}1&2&-1&4\\0&0&5&-3\\0&0&5&-3\end{pmatrix}\sim\begin{pmatrix}1&2&-1&4\\0&0&5&-3\\0&0&0&0\end{pmatrix}.
$$

These operations preserve the [row space](../../../../../row-space.md). The two nonzero rows of this [row echelon form](../../../../../row-echelon-form.md) are [linearly independent](../../../../../linear-independence.md): only the first has a nonzero first entry, and the second is nonzero. Hence

$$
\boxed{\text{a row-space basis is }\{(1,2,-1,4),(0,0,5,-3)\},\qquad\operatorname{rank}A=2.}
$$

Further [Gaussian elimination](../../../../../gaussian-elimination.md) gives the [reduced row echelon form](../../../../../reduced-row-echelon-form.md)

$$
\begin{pmatrix}1&2&0&17/5\\0&0&1&-3/5\\0&0&0&0\end{pmatrix},
$$

which will also identify the [free variables](../../../../../free-variable.md) in the [null space](../../../../../kernel-of-a-linear-map-split.md) calculation.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
