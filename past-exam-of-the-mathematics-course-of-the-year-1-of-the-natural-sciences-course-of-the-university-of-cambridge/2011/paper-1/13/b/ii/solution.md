<h1 id="13/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $Q=(x_1\ x_2)$ for the normalized [eigenvectors](../../../../../../eigenvector.md) already chosen. Then $Q^TQ=I$, $(x,y)^T=Q(x',y')^T$, and [orthogonal diagonalization](../../../../../../orthogonal-diagonalization-of-a-real-symmetric-matrix.md) gives

$$
Q^TAQ=\begin{pmatrix}2&0\\0&8\end{pmatrix},\qquad
\boxed{2(x')^2+8(y')^2=1.}
$$

The [ellipse](../../../../../../ellipse.md) has semi-axis lengths $1/\sqrt2$ and $1/\sqrt8$ along $x_1$ and $x_2$, respectively. Rescale $x''=\sqrt2x'$ and $y''=\sqrt8y'$ to obtain the [unit circle](../../../../../../complex-unit-circle.md) $(x'')^2+(y'')^2=1$. Since $(x',y')^T=Q^T(x,y)^T$,

$$
\boxed{\begin{pmatrix}x''\\y''\end{pmatrix}
=B\begin{pmatrix}x\\y\end{pmatrix},\qquad
B=\begin{pmatrix}\sqrt2&0\\0&\sqrt8\end{pmatrix}Q^T
=\begin{pmatrix}1&1\\2&-2\end{pmatrix}.}
$$

The identity $B^TB=A$ checks the rescaling directly. Swapping or reversing [eigenvectors](../../../../../../eigenvector.md) gives other valid coordinate matrices; the displayed one follows the explicit choices in part (a).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [13](../../../13.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
