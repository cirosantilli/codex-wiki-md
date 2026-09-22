<h1 id="10b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Under an orthogonal change of coordinates represented by $Q$, the component matrix changes by

$$
T'=QTQ^T=QTQ^{-1}.
$$

Thus $T'$ is [similar](../../../../../../matrix-similarity.md) to $T$, so its [characteristic polynomial](../../../../../../characteristic-polynomial.md), [eigenvalues](../../../../../../eigenvalue.md), and their [algebraic multiplicities](../../../../../../algebraic-multiplicity.md) are unchanged.

If $T$ is [symmetric](../../../../../../symmetric-matrix.md), the [spectral theorem for real symmetric matrices](../../../../../../spectral-theorem-for-real-symmetric-matrices.md) makes it [diagonalizable](../../../../../../diagonalizable-matrix.md), so algebraic and geometric multiplicities agree. Consequently the dimensions of its eigenspaces are also independent of the coordinate frame.

For the stated tensor, choose a unit eigenvector $n$ belonging to the simple eigenvalue $\mu$. Its perpendicular plane is the eigenspace of $\lambda$, so

$$
T=\lambda(I-nn^T)+\mu nn^T
=\lambda I+(\mu-\lambda)nn^T.
$$

Hence

$$
\boxed{T_{ij}=\alpha\delta_{ij}+\beta n_in_j},
\qquad
\alpha=\lambda,\quad\beta=\mu-\lambda.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10B](../../10b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
