<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose a real unit [eigenvector](../../../../../eigenvector.md) $e_1$ of the real [symmetric matrix](../../../../../symmetric-matrix.md) $Q$, with [eigenvalue](../../../../../eigenvalue.md) $\lambda_1$. Its [orthogonal complement](../../../../../orthogonal-complement.md) is an [invariant subspace](../../../../../invariant-subspace.md): for any $v$ with $e_1^Tv=0$,

$$
e_1^TQv=(Qe_1)^Tv=\lambda_1e_1^Tv=0.
$$

The restriction of $Q$ to this $(n-1)$-dimensional space is again real and symmetric. Applying the same argument inductively produces an [orthonormal basis](../../../../../orthonormal-basis.md) $e_1,\ldots,e_n$ of real [eigenvectors](../../../../../eigenvector.md). The base case $n=1$ is immediate. This proves the [spectral theorem for real symmetric matrices](../../../../../spectral-theorem-for-real-symmetric-matrices.md) without assuming that distinct [eigenvalues](../../../../../eigenvalue.md) are available.

One can also check that [eigenvectors](../../../../../eigenvector.md) with different [eigenvalues](../../../../../eigenvalue.md) are automatically orthogonal: $\lambda_i e_i^Te_j=(Qe_i)^Te_j=e_i^TQe_j=\lambda_j e_i^Te_j$. Within a repeated [eigenspace](../../../../../eigenspace.md), the [Gram-Schmidt process](../../../../../gram-schmidt-process.md) preserves the eigenvector property. Thus repeated [eigenvalues](../../../../../eigenvalue.md) cause no obstruction, and $\boxed{Q=ODO^T\text{ for an orthogonal }O\text{ and real diagonal }D}$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
