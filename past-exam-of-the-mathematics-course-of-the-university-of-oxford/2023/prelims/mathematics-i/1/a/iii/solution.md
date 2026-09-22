<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [iii](../iii.md)

Perform the [elementary row operations](../../../../../../../elementary-row-operation.md) $R_2\leftarrow R_2+2R_1$ and $R_3\leftarrow R_3-R_1$, then $R_2\leftarrow R_2/2$, $R_1\leftarrow R_1-R_2$, and finally $R_1\leftarrow R_1+R_3$, $R_2\leftarrow R_2-3R_3$:

$$
\begin{pmatrix}1&1&2\\-2&0&2\\1&1&3\end{pmatrix}
\longrightarrow
\begin{pmatrix}1&1&2\\0&2&6\\0&0&1\end{pmatrix}
\longrightarrow
\begin{pmatrix}1&0&-1\\0&1&3\\0&0&1\end{pmatrix}
\longrightarrow I_3.
$$

Consequently the [reduced row echelon form](../../../../../../../reduced-row-echelon-form.md) is $I_3$. Applying the same operations to the augmented column $b=(b_1,b_2,b_3)^T$ gives

$$
\boxed{v=\begin{pmatrix}
b_3-b_1-\tfrac12b_2\\
4b_1+\tfrac12b_2-3b_3\\
b_3-b_1
\end{pmatrix}.}
$$

Thus **every** $b\in\mathbb R^3$ admits exactly one solution. This follows because the [elementary row operations](../../../../../../../elementary-row-operation.md) preserve the solution set of the augmented [linear system](../../../../../../../system-of-linear-equations.md), and the reduced coefficient [matrix](../../../../../../../matrix.md) is the [identity matrix](../../../../../../../identity-matrix.md).

## ↑ Ancestors (13)

1. [iii](../iii.md)
2. [a](../../a.md)
3. [1](../../../1.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
