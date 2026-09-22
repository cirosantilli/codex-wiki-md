<h1 id="6/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

[Gaussian elimination](../../../../../../gaussian-elimination.md) gives the [row operations](../../../../../../elementary-row-operation.md) $R_2\leftarrow R_2-3R_1$, $R_3\leftarrow R_3-R_1$, $R_4\leftarrow R_4-2R_1$, producing the lower three rows $(0,1,4,1)$, $(0,1,4,1)$, $(0,-3,2,-1)$. Subtract the new row two from row three and add three times row two to row four; the remaining nonzero row is $(0,0,14,2)$. Move it above the zero row and finish elimination to obtain

$$
\operatorname{rref}(A)=\begin{pmatrix}1&0&0&-2/21\\0&1&0&3/7\\0&0&1&1/7\\0&0&0&0\end{pmatrix}.
$$

The [pivot](../../../../../../pivotal-quantity.md) columns are one, two and three. [Row operations](../../../../../../elementary-row-operation.md) preserve the [linear dependence](../../../../../../linear-dependence.md) relations among columns, so the corresponding columns of the original [matrix](../../../../../../matrix.md) form a [basis](../../../../../../basis.md) for the [column space](../../../../../../column-space.md), which is the image of the [linear map](../../../../../../linear-map.md):

$$
\boxed{\left\{\begin{pmatrix}3\\9\\3\\6\end{pmatrix},\begin{pmatrix}1\\4\\2\\-1\end{pmatrix},\begin{pmatrix}-1\\1\\3\\0\end{pmatrix}\right\}.}
$$

In particular, the [matrix rank](../../../../../../matrix-rank.md) is three. Columns of the reduced [matrix](../../../../../../matrix.md) itself would generally give a different subspace, so the original columns must be used.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
