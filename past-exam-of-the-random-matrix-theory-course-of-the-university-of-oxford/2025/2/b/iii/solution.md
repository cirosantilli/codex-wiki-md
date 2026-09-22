<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the symmetric [joint probability density function](../../../../../joint-probability-density.md) of exchangeably labelled [eigenvalues](../../../../../eigenvalue.md), normalized over all of $\mathbb R^3$. The [finite-rank projection kernel](../../../../../finite-rank-projection-kernel.md) has

$$
\int\widetilde K_3(x,x)\,dx
=\sum_{\ell=0}^2\lVert\phi_\ell\rVert_2^2=3.
$$

Successive applications of [Gaudin's lemma](../../../../../projection-kernel-determinant-integration.md) therefore give

$$
\int_{\mathbb R^3}\det[\widetilde K_3(\lambda_i,\lambda_j)]_{i,j=1}^3
\,d\lambda_1d\lambda_2d\lambda_3
=1\cdot2\cdot3=6.
$$

It follows that

$$
\boxed{\widetilde c_3=\frac1{3!}=\frac16.}
$$

As a normalization check, the [weighted Vandermonde determinant](../../../../../weighted-vandermonde-determinant.md) yields

$$
\det[\widetilde K_3(\lambda_i,\lambda_j)]
=\frac{\prod_{i<j}(\lambda_i-\lambda_j)^2e^{-\sum_i\lambda_i^2/2}}
{\kappa_0^2\kappa_1^2\kappa_2^2},
\qquad
\boxed{c_3=\frac1{12(2\pi)^{3/2}}.}
$$

If instead one uses ordered [eigenvalues](../../../../../eigenvalue.md) on $\lambda_1<\lambda_2<\lambda_3$, the normalized density on that chamber is six times the labelled density. In that convention the determinant prefactor on the chamber is one.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the random matrix theory course of the University of Oxford](../../../../split.md)
6. [Random matrix theory course of the University of Oxford](../../../../../random-matrix-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
