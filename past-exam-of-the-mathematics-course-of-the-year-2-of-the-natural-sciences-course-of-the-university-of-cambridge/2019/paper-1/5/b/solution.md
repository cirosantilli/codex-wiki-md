<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An [invertible matrix](../../../../../invertible-matrix.md) is a square matrix for which there is a matrix $A^{-1}$ with $AA^{-1}=A^{-1}A=I$. Write its assumed [diagonalization](../../../../../diagonalization-of-a-matrix.md) as $A=P\Lambda P^{-1}$, where $P$ is invertible and $\Lambda=\operatorname{diag}(\lambda_1,\ldots,\lambda_n)$. Then

$$
\det A=\det\Lambda=\prod_{j=1}^n\lambda_j.
$$

If the [determinant](../../../../../determinant.md) is nonzero, every $\lambda_j$ is nonzero, so $\Lambda^{-1}=\operatorname{diag}(\lambda_j^{-1})$ exists and $A^{-1}=P\Lambda^{-1}P^{-1}$. If the [determinant](../../../../../determinant.md) is zero, at least one [eigenvalue](../../../../../eigenvalue.md) is zero; its nonzero [eigenvector](../../../../../eigenvector.md) is mapped to zero, which an invertible map cannot do. Hence

$$
\boxed{A\text{ is invertible}\quad\Longleftrightarrow\quad\det A\ne0.}
$$

The equivalence holds even without diagonalizability, but the eigenbasis proves the stated case directly.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
