<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use $R_2\gets R_2+2R_1$ and $R_3\gets R_3-3R_1$, followed by $R_3\gets R_3+R_2$. These [elementary row operations](../../../../../elementary-row-operation.md) give

$$
\begin{pmatrix}1&4&1\\-2&-4&0\\3&8&0\end{pmatrix}\sim\begin{pmatrix}1&4&1\\0&4&2\\0&-4&-3\end{pmatrix}\sim\underbrace{\begin{pmatrix}1&4&1\\0&4&2\\0&0&-1\end{pmatrix}}_U.
$$

The elimination multipliers are $m_{21}=-2$, $m_{31}=3$, $m_{32}=-1$. Record them in the [unit lower triangular matrix](../../../../../unit-lower-triangular-matrix.md) $L$:

$$
\boxed{A=LU,\qquad L=\begin{pmatrix}1&0&0\\-2&1&0\\3&-1&1\end{pmatrix},\quad U=\begin{pmatrix}1&4&1\\0&4&2\\0&0&-1\end{pmatrix}.}
$$

To see the [elementary matrix](../../../../../elementary-matrix.md) relation directly, let $F_{21}=I+2e_{21}$, $F_{31}=I-3e_{31}$ and $F_{32}=I+e_{32}$, where $e_{ij}$ has a single 1 in position $(i,j)$. Then $U=F_{32}F_{31}F_{21}A$, and reversing and inverting these operations gives $L=F_{21}^{-1}F_{31}^{-1}F_{32}^{-1}$. Direct [matrix multiplication](../../../../../matrix-multiplication.md) also verifies the stated [LU decomposition](../../../../../lu-decomposition.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
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
