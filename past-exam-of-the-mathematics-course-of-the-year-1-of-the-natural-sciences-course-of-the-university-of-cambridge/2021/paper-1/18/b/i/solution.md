<h1 id="18/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [characteristic polynomial](../../../../../../characteristic-polynomial.md) of $A$ is

$$
\det(A-\lambda I)=(-5-\lambda)(5-\lambda)+16=\lambda^2-9.
$$

Its distinct [eigenvalues](../../../../../../eigenvalue.md) are $3$ and $-3$. For $3$, the [eigenvector](../../../../../../eigenvector.md) relation gives $y=-2x$, so choose $(1,-2)^T$. For $-3$, it gives $x=-2y$, so choose $(2,-1)^T$. Put these independent [eigenvectors](../../../../../../eigenvector.md) into columns:

$$
\boxed{B=\begin{pmatrix}1&2\\-2&-1\end{pmatrix},\qquad C=\begin{pmatrix}3&0\\0&-3\end{pmatrix}.}
$$

Then $AB=BC$ column by column. Also $\det B=3\ne0$, so this choice supplies the [diagonalization of a matrix](../../../../../../diagonalization-of-a-matrix.md) $B^{-1}AB=C$. Scaling columns or interchanging their order gives other valid choices, with the matching order in $C$.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [18](../../../18.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
