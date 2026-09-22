<h1 id="6d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [columnwise partial pivoting](../../../../../../columnwise-partial-pivoting.md): select the largest absolute entry in the current column and interchange rows. In the first column the pivot is $4$, so interchange rows 1 and 2. The multipliers are $1/2$ and $-1/2$, and elimination gives

$$
\begin{pmatrix}4&1&0\\0&1/2&1\\0&5/2&1\end{pmatrix}.
$$

The second pivot is $5/2$, so interchange the two remaining rows. Their previously stored first-column multipliers must also be interchanged. The final multiplier is $(1/2)/(5/2)=1/5$, giving the [LU decomposition](../../../../../../lu-decomposition.md)

$$
\boxed{PA=LU,\qquad
P=\begin{pmatrix}0&1&0\\0&0&1\\1&0&0\end{pmatrix},\quad
L=\begin{pmatrix}1&0&0\\-1/2&1&0\\1/2&1/5&1\end{pmatrix},\quad
U=\begin{pmatrix}4&1&0\\0&5/2&1\\0&0&4/5\end{pmatrix}.}
$$

The [permutation matrix](../../../../../../permutation-matrix.md) orders the original rows as $2,3,1$. Multiplication verifies the displayed identity.

If “column pivoting” instead denotes interchanging columns rather than searching within a column, that convention gives $AQ=\widetilde L\widetilde U$ with

$$
Q=\begin{pmatrix}1&0&0\\0&0&1\\0&1&0\end{pmatrix},\quad
\widetilde L=\begin{pmatrix}1&0&0\\2&1&0\\-1&-1&1\end{pmatrix},\quad
\widetilde U=\begin{pmatrix}2&1&1\\0&-2&-1\\0&0&2\end{pmatrix}.
$$

This second identity uses a different pivot convention; it does not change the row-pivoted answer above.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6D](../../6d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
