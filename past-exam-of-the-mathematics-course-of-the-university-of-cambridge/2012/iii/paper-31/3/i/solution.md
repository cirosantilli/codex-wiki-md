<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use [block matrix](../../../../../../block-matrix.md) elimination with the invertible square block $A$:

$$
\begin{pmatrix}I&0\\-CA^{-1}&I\end{pmatrix}\begin{pmatrix}A&B\\C&D\end{pmatrix}=\begin{pmatrix}A&B\\0&D-CA^{-1}B\end{pmatrix}.
$$

The left multiplier is block triangular with identity diagonal blocks, so its [determinant](../../../../../../determinant.md) is $1$. Taking the [determinant](../../../../../../determinant.md) of the block-triangular product proves

$$
\boxed{\det M=\det A\,\det(D-CA^{-1}B).}
$$

The [matrix](../../../../../../matrix.md) $D-CA^{-1}B$ is the [Schur complement](../../../../../../schur-complement.md) of $A$. The proof needs $A$ invertible, but does not assume the [Schur complement](../../../../../../schur-complement.md) or the full [matrix](../../../../../../matrix.md) is invertible.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
