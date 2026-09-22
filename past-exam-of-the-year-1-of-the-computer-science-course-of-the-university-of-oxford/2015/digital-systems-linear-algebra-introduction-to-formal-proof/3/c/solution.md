<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use [Gaussian elimination](../../../../../gaussian-elimination.md) without row exchanges. First apply $R_2\gets R_2-3R_1$ and $R_3\gets R_3-2R_1$; then apply $R_3\gets R_3-R_2$:

$$
\begin{pmatrix}1&2&4\\3&8&14\\2&6&13\end{pmatrix}\longrightarrow\begin{pmatrix}1&2&4\\0&2&2\\0&2&5\end{pmatrix}\longrightarrow U=\begin{pmatrix}1&2&4\\0&2&2\\0&0&3\end{pmatrix}.
$$

The elimination multipliers are $m_{21}=3$, $m_{31}=2$ and $m_{32}=1$. Put them below the diagonal of a [unit lower triangular matrix](../../../../../unit-lower-triangular-matrix.md):

$$
\boxed{L=\begin{pmatrix}1&0&0\\3&1&0\\2&1&1\end{pmatrix},\qquad U=\begin{pmatrix}1&2&4\\0&2&2\\0&0&3\end{pmatrix},\qquad A=LU.}
$$

To see why these multipliers reconstruct the rows, row 2 of $LU$ is three times row 1 of $U$ plus row 2 of $U$, giving $(3,8,14)$. Row 3 of $LU$ is twice row 1 plus row 2 plus row 3 of $U$, giving $(2,6,13)$. This directly verifies the [LU factorization](../../../../../lu-decomposition.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
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
