<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Because $A$ is a real symmetric [positive-definite matrix](../../../../../../positive-definite-matrix.md), the [finite-dimensional spectral theorem](../../../../../../finite-dimensional-spectral-theorem.md) supplies an orthonormal eigenbasis $u_1,\ldots,u_n$ with

$$
0<\lambda_1\leq\cdots\leq\lambda_n.
$$

Its eigendecomposition is also its [singular value decomposition](../../../../../../singular-value-decomposition.md). If $e=y^{(\delta)}-y$, then

$$
x^{(\delta)}-x=A^{-1}e
=\sum_{j=1}^n\frac{\langle e,u_j\rangle}{\lambda_j}u_j,
$$

so

$$
\boxed{\|x^{(\delta)}-x\|
\leq\frac{\delta}{\lambda_1}}.
$$

The operator norms satisfy $\|A\|_2=\lambda_n$ and $\|A^{-1}\|_2=1/\lambda_1$. Therefore the worst-case relative perturbation bound is

$$
\boxed{
\frac{\|x^{(\delta)}-x\|}{\|x\|}
\leq
\underbrace{\frac{\lambda_n}{\lambda_1}}_{\kappa_2(A)}
\frac{\|y^{(\delta)}-y\|}{\|y\|}}.
$$

The ratio $κ_2(A)$ is the [spectral condition number of a positive-definite matrix](../../../../../../spectral-condition-number-of-a-positive-definite-matrix.md). A large ratio means that data noise aligned with an [eigenvector](../../../../../../eigenvector.md) for the smallest [eigenvalue](../../../../../../eigenvalue.md) is strongly amplified, so the inverse problem is ill conditioned.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
