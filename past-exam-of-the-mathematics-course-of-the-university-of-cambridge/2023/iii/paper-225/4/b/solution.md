<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\Xi_{ik}=\langle X_i,B_k\rangle$ and define the [roughness penalty matrix](../../../../../../roughness-penalty-matrix.md)

$$
\Omega_{jk}=\langle B_j'',B_k''\rangle
=\int_0^1B_j''(t)B_k''(t)\,dt.
$$

For $c=(c_1,\ldots,c_K)^{\mathsf T}$, the loss is the quadratic function

$$
L(c)=\lVert Y-\Xi c\rVert_2^2+\rho c^{\mathsf T}\Omega c.
$$

Its [normal equations](../../../../../../normal-equation.md) are

$$
(\Xi^{\mathsf T}\Xi+\rho\Omega)c=\Xi^{\mathsf T}Y.
$$

Whenever $\Xi^{\mathsf T}\Xi+\rho\Omega$ is positive definite, the unique minimizer is

$$
\widehat c
=(\Xi^{\mathsf T}\Xi+\rho\Omega)^{-1}\Xi^{\mathsf T}Y,
\qquad
\widehat\beta(t)=\sum_{k=1}^K\widehat c_kB_k(t).
$$

For the usual choice $\rho\geq0$, the penalty matrix is positive semidefinite, so full column rank of $\Xi$ suffices. Since the question permits arbitrary real $\rho$, a sufficiently negative value can make the quadratic form indefinite; then the loss is unbounded below and no minimizer exists. In the singular positive-semidefinite case, the [Moore-Penrose inverse](../../../../../../moore-penrose-inverse.md) describes the minimum-norm solution whenever the normal equations are consistent.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 225](../../../paper-225-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
