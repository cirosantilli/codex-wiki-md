<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A matrix is [diagonalizable](../../../../diagonalizable-matrix.md) if some invertible $S$ makes $S^{-1}AS$ diagonal, equivalently if it has a basis of [eigenvectors](../../../../eigenvector.md). If $A^p=0$ and $Av=\lambda v$ for $v\ne0$, then $0=A^pv=\lambda^pv$, so every [eigenvalue](../../../../eigenvalue.md) is zero. There is at least one zero eigenvalue: otherwise $A$ and hence $A^p$ would be invertible. A [diagonalizable nilpotent matrix](../../../../diagonalizable-nilpotent-matrix.md) has an all-zero diagonal form and therefore is zero itself.

For the specified matrices, direct determinant expansion gives

$$
\boxed{\det(\lambda I-B)=\lambda^3,\qquad\det(\lambda I-C)=\lambda(\lambda-6)(\lambda+6).}
$$

The [Cayley-Hamilton theorem](../../../../cayley-hamilton-theorem-split.md) gives $B^3=0$. Its entry $B_{12}=-2$ is nonzero for every real $\alpha$, so **$B$ is not diagonalizable for any $\alpha$**. The matrix $C$ has three distinct real eigenvalues and is therefore **diagonalizable over $\mathbb R$**. For an explicit check, take columns $(-1,0,1)^T$, $(2,-3,1)^T$, $(2,3,1)^T$ in $S$; then $S^{-1}CS=\operatorname{diag}(-6,0,6)$.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [Paper 1](../../paper-1-split.md)
3. [2006](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
