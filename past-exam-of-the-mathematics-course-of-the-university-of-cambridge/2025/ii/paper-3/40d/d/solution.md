<h1 id="40d/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $L$ be the tridiagonal matrix with diagonal entries $-2$ and adjacent off-diagonal entries $1$ on the interior grid points. The finite-interval scheme is

$$
\left(I-\frac\mu2L\right)u^{n+1}
=\left(I+\frac\mu2L\right)u^n.
$$

For $J$ interior points, the [dirichlet discrete Laplacian](../../../../../../dirichlet-discrete-laplacian.md) has eigenvalues

$$
\lambda_j=-4\sin^2\left(\frac{j\pi}{2(J+1)}\right)<0,
\qquad 1\leq j\leq J.
$$

The corresponding eigenvalues of the amplification matrix are

$$
q_j=\frac{1+(\mu/2)\lambda_j}
{1-(\mu/2)\lambda_j}.
$$

Since $\lambda_j<0$ and $\mu\geq0$,

$$
|q_j|\leq1
$$

for every $j$. The matrix is real symmetric in the sine eigenbasis, so its induced $2$-norm is the largest $|q_j|$. This proves the [crank-Nicolson stability on a finite Dirichlet interval](../../../../../../crank-nicolson-stability-on-a-finite-dirichlet-interval.md) and gives

$$
\boxed{\text{stability for every }\mu>0}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [40D](../../40d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
