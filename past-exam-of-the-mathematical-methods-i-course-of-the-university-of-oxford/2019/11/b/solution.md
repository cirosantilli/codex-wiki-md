<h1 id="11/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The upper-triangular [matrix](../../../../matrix.md) has distinct [eigenvalues](../../../../eigenvalue.md) $2,-1$, with respective [eigenvectors](../../../../eigenvector.md) $(1,0)^T$ and $(-2,1)^T$. Thus

$$
A=S\begin{pmatrix}2&0\\0&-1\end{pmatrix}S^{-1},\qquad
S=\begin{pmatrix}1&-2\\0&1\end{pmatrix},\qquad
S^{-1}=\begin{pmatrix}1&2\\0&1\end{pmatrix}.
$$

The defining [power series](../../../../power-series.md) shows that the [matrix exponential respects similarity](../../../../matrix-exponential-respects-similarity.md). Applying [solution](../a/solution.md) to the diagonal factor gives

$$
\boxed{e^A=S\begin{pmatrix}e^2&0\\0&e^{-1}\end{pmatrix}S^{-1}
=\begin{pmatrix}e^2&2(e^2-e^{-1})\\0&e^{-1}\end{pmatrix}.}
$$

As a direct series check, $(A^m)_{12}=2(2^m-(-1)^m)$ for $m\geq0$; summing this entry divided by $m!$ gives the same off-diagonal expression.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [11](../../11.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
