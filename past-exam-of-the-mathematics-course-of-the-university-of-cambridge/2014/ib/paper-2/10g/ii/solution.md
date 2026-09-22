<h1 id="10g/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the [determinant of a complex block representation](../../../../../../determinant-of-a-complex-block-representation.md), put

$$
M=\begin{pmatrix}A&-B\\B&A\end{pmatrix},\qquad
T=\begin{pmatrix}I&I\\-iI&iI\end{pmatrix}.
$$

The [change-of-basis matrix](../../../../../../change-of-basis-matrix.md) $T$ is invertible, and direct block multiplication gives

$$
MT=T\begin{pmatrix}A+iB&0\\0&A-iB\end{pmatrix}.
$$

Thus $T^{-1}MT$ is block diagonal. Using [multiplicativity of the determinant](../../../../../../multiplicativity-of-the-determinant.md) and the preceding block formula,

$$
\boxed{\det M=\det(A+iB)\det(A-iB).}
$$

The identity follows from this constant change of basis for arbitrary complex $A,B$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [10G](../../10g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
