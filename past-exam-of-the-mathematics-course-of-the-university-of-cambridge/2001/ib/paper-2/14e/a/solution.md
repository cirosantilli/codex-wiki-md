<h1 id="14e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a real [symmetric positive-definite matrix](../../../../../../symmetric-positive-definite-matrix.md), the [Cholesky decomposition](../../../../../../cholesky-decomposition.md) is $B=R^TR$, where $R$ is upper triangular with positive diagonal; equivalently $B=LL^T$ with $L=R^T$ lower triangular.

Existence can be proved by induction. Write $B=\begin{pmatrix}b&v^T\\v&C\end{pmatrix}$, where $b>0$. For a nonzero vector $z$, evaluate the quadratic form at $(-v^Tz/b,z)^T$ to obtain $z^T(C-vv^T/b)z>0$. The [Schur complement](../../../../../../schur-complement.md) is therefore positive definite. By induction it has factor $R_0^TR_0$, and

$$
R=\begin{pmatrix}\sqrt b&v^T/\sqrt b\\0&R_0\end{pmatrix}
$$

has $R^TR=B$. The one-dimensional starting case is the positive square root.

For uniqueness, if $R_1^TR_1=R_2^TR_2=B$, then $U=R_2R_1^{-1}$ is upper triangular and satisfies $U^TU=I$. Since $U^{-1}$ is upper triangular and equals $U^T$, which is lower triangular, $U$ is diagonal. Orthogonality makes its diagonal entries $\pm1$, and positivity of the diagonals of $R_1,R_2$ forces $+1$. Hence $U=I$ and **$\boxed{R_1=R_2}$**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [14E](../../14e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
