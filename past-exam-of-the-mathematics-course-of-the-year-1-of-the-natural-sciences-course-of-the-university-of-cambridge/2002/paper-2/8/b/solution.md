<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Call the given [matrix](../../../../../matrix.md) $M$. Its middle coordinate decouples, immediately giving the [eigenvalue](../../../../../eigenvalue.md) $3$ with normalized [eigenvector](../../../../../eigenvector.md) $(0,1,0)^T$. The remaining [characteristic polynomial](../../../../../characteristic-polynomial.md) comes from the $xz$ block:

$$
\det\begin{pmatrix}-1-\lambda&-3\sqrt3\\-3\sqrt3&5-\lambda\end{pmatrix}=(-1-\lambda)(5-\lambda)-27=\lambda^2-4\lambda-32=(\lambda+4)(\lambda-8).
$$

For $\lambda=-4$, the first row of $(M+4I)v=0$ gives $x=\sqrt3z$; for $\lambda=8$, the first row of $(M-8I)v=0$ gives $z=-\sqrt3x$. After [vector normalization](../../../../../vector-normalization.md), one possible complete set is

$$
\boxed{\begin{aligned}
\lambda_1&=-4,&v_1&=\frac12(\sqrt3,0,1)^T,\\
\lambda_2&=3,&v_2&=(0,1,0)^T,\\
\lambda_3&=8,&v_3&=\frac12(-1,0,\sqrt3)^T.
\end{aligned}}
$$

Each has unit [Euclidean norm](../../../../../euclidean-norm.md). The [dot products](../../../../../dot-product.md) with $v_2$ vanish because the other two middle components are zero, and $v_1\cdot v_3=(-\sqrt3+\sqrt3)/4=0$. This explicitly verifies [orthonormality](../../../../../orthonormal-set.md), also predicted by the [spectral theorem](../../../../../spectral-theorem.md) for real [symmetric matrices](../../../../../symmetric-matrix.md) with distinct [eigenvalues](../../../../../eigenvalue.md). Changing any [eigenvector](../../../../../eigenvector.md)'s sign gives an equally valid normalized choice.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [8](../../8.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
