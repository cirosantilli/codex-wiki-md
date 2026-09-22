<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a real [symmetric matrix](../../../../../symmetric-matrix.md) $A$, find its real [eigenvalues](../../../../../eigenvalue.md) from $\det(A-\lambda I)=0$, then solve $(A-\lambda I)v=0$ for the corresponding [eigenspaces](../../../../../eigenspace.md). Distinct [eigenspaces](../../../../../eigenspace.md) are orthogonal. Within each repeated [eigenspace](../../../../../eigenspace.md), apply the [Gram-Schmidt process](../../../../../gram-schmidt-process.md) and normalize to obtain an [orthonormal basis](../../../../../orthonormal-basis.md) of [eigenvectors](../../../../../eigenvector.md).

Put these vectors in the columns of $O$. The [spectral theorem for real symmetric matrices](../../../../../spectral-theorem-for-real-symmetric-matrices.md) guarantees a full basis, so $O^TO=I$ and

$$
\boxed{O^TAO=\operatorname{diag}(\lambda_1,\ldots,\lambda_n),\qquad A=O\operatorname{diag}(\lambda_1,\ldots,\lambda_n)O^T.}
$$

This is the [orthogonal diagonalization](../../../../../orthogonal-diagonalization-of-a-real-symmetric-matrix.md) of $A$ and the associated [orthogonal change of coordinates](../../../../../orthogonal-change-of-coordinates.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
