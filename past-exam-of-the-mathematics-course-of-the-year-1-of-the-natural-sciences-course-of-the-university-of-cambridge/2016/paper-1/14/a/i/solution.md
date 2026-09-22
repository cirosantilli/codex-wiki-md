<h1 id="14/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

By the [spectral theorem for real symmetric matrices](../../../../../../spectral-theorem-for-real-symmetric-matrices.md), choose the normalized [eigenvectors](../../../../../../eigenvector.md) to form an **[orthonormal basis](../../../../../../orthonormal-basis.md)**. With $P_n=\mathbf e_n\mathbf e_n^{\mathsf T}$, orthonormality gives $P_nP_m=\delta_{nm}P_n$ and $\sum_nP_n=I$. For every vector $\mathbf x$, expand $\mathbf x=\sum_n(\mathbf e_n^{\mathsf T}\mathbf x)\mathbf e_n$ and apply $A$:

$$
A\mathbf x=\sum_n\lambda_n\mathbf e_n(\mathbf e_n^{\mathsf T}\mathbf x).
$$

Since this equality holds for every $\mathbf x$, the [spectral decomposition](../../../../../../spectral-decomposition.md) is

$$
\boxed{A=\sum_{n=1}^N\lambda_n\mathbf e_n\mathbf e_n^{\mathsf T}.}
$$

Each $P_n$ is the rank-one [orthogonal projection](../../../../../../orthogonal-projection.md) onto its [eigenvector](../../../../../../eigenvector.md) direction. In a degenerate [eigenspace](../../../../../../eigenspace.md), normalized [eigenvectors](../../../../../../eigenvector.md) must be chosen mutually orthogonal; normalization alone does not guarantee this resolution of the identity.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [14](../../../14.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
