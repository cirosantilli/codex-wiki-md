<h1 id="7a/solution">Solution</h1>

↑ **Parent:** [7A](../7a.md)

By the [real spectral theorem](../../../../../real-spectral-theorem.md), a real symmetric matrix has an orthogonal diagonalization

$$
A=Q\operatorname{diag}(\lambda_1,\ldots,\lambda_n)Q^T.
$$

Writing $y=Q^Tx$ gives

$$
x^TAx=\sum_i\lambda_i y_i^2.
$$

This is nonnegative for every $x$ exactly when every $\lambda_i\geq0$. Thus the quadratic-form and eigenvalue definitions of a [positive semidefinite matrix](../../../../../positive-semidefinite-matrix.md) agree.

When $A$ is positive semidefinite, define

$$
\boxed{
\sqrt A
=Q\operatorname{diag}(\sqrt{\lambda_1},\ldots,\sqrt{\lambda_n})Q^T}.
$$

This matrix is symmetric and positive semidefinite, and its square is $A$, so it is the [principal square root of a positive semidefinite matrix](../../../../../principal-square-root-of-a-positive-semidefinite-matrix.md).

For nonsingular $M$, the matrix $M^TM$ is symmetric and

$$
x^TM^TMx=\|Mx\|^2>0
$$

for every nonzero $x$. Thus $M^TM$ is positive definite, and

$$
P=\sqrt{M^TM}
$$

exists and is nonsingular. Let $R=MP^{-1}$. Since $P$ is symmetric,

$$
R^TR=P^{-1}M^TMP^{-1}
=P^{-1}P^2P^{-1}=I.
$$

Hence $R$ is an [orthogonal matrix](../../../../../orthogonal-matrix.md) and

$$
\boxed{M=RP},
$$

the [polar decomposition of an invertible real matrix](../../../../../polar-decomposition-of-an-invertible-real-matrix.md).

In three dimensions, $P$ stretches or contracts along three mutually perpendicular eigenvector directions by its positive eigenvalues. The orthogonal map $R$ is then applied: it is a rotation when $\det M>0$, and a rotation combined with a reflection when $\det M<0$.

## ↑ Ancestors (10)

1. [7A](../7a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
