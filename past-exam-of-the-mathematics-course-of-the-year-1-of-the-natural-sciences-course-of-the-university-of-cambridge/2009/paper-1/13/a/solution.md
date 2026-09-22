<h1 id="13/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [characteristic polynomial](../../../../../characteristic-polynomial.md) is

$$
\det(A-\lambda I)=(2-\lambda)(4-\lambda)+2=(\lambda-3)^2+1.
$$

Thus the [eigenvalues](../../../../../eigenvalue.md) and corresponding [eigenvectors](../../../../../eigenvector.md) over $\mathbb C$ are

$$
\boxed{\lambda_+=3+i,\ v_+=(-1+i,1)^T;\qquad\lambda_-=3-i,\ v_-=(-1-i,1)^T.}
$$

All nonzero scalar multiples of these vectors are also [eigenvectors](../../../../../eigenvector.md). Distinct [eigenvalues](../../../../../eigenvalue.md) make them linearly independent. Put them in the columns of

$$
B=\begin{pmatrix}-1+i&-1-i\\1&1\end{pmatrix},\qquad
B^{-1}=\frac1{2i}\begin{pmatrix}1&1+i\\-1&-1+i\end{pmatrix}.
$$

The equations $Av_\pm=\lambda_\pm v_\pm$ are exactly $AB=BC$, giving the [diagonalization](../../../../../diagonalization-of-a-matrix.md)

$$
\boxed{C=B^{-1}AB=\begin{pmatrix}3+i&0\\0&3-i\end{pmatrix}.}
$$

There is no diagonalization over $\mathbb R$, since the matrix has no real [eigenvalues](../../../../../eigenvalue.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [13](../../13.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
