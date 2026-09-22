<h1 id="11h/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $\ell_j$ be the [Lagrange interpolation polynomial](../../../../../../lagrange-polynomial.md) for the roots $\omega_j$, and define

$$
A_j=\int_{-1}^1\ell_j(x)r(x)\,dx.
$$

For $\deg Q\leq2n-1$, [polynomial division](../../../../../../polynomial-division.md) gives $Q=SP_n+R$ with $\deg S,\deg R<n$. Orthogonality kills the first term, while interpolation gives $R=\sum_jR(\omega_j)\ell_j$. Therefore

$$
\int Qr=\sum_jA_jQ(\omega_j).
$$

Taking $Q=\ell_j$ proves uniqueness. Taking $Q=\ell_j^2$ also shows

$$
A_j=\int\ell_j^2r>0,
\qquad
\sum_jA_j=\int r.
$$

This is [Gaussian quadrature](../../../../../../gaussian-quadrature.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [11H](../../11h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
