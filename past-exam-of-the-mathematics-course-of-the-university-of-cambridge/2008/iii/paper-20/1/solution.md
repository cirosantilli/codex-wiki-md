<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the nonnegative [Laplacian](../../../../../laplacian.md) convention $\widetilde\Delta=-\sum_{j=1}^{d+1}\partial_j^2$ and $\Delta=-\operatorname{div}\operatorname{grad}$ on the unit [sphere](../../../../../sphere.md). In [polar coordinates](../../../../../polar-coordinates.md) the Euclidean [Riemannian metric](../../../../../riemannian-metric.md) is $dr^2+r^2g_{S^d}$, its [volume form](../../../../../volume-form.md) is $r^d\,dr\,dV_{S^d}$, and therefore the [Laplacian in polar coordinates](../../../../../laplacian-in-polar-coordinates.md) is

$$
\widetilde\Delta=-\partial_r^2-\frac d r\partial_r+\frac1{r^2}\Delta.
$$

Consequently the required restriction identity is

$$
\boxed{\Delta\bar f=\overline{\widetilde\Delta f}+\left.(\partial_r^2f+d\partial_rf)\right|_{r=1}.}
$$

For the opposite sign convention all [eigenvalues](../../../../../eigenvalue.md) below change sign, and the restriction identity changes accordingly.

Let $\mathcal P_n$ be the [vector space](../../../../../vector-space-split.md) of degree-$n$ [homogeneous polynomials](../../../../../homogeneous-polynomial.md) in $d+1$ variables, and let $\mathcal H_n$ be its subspace of [harmonic polynomials](../../../../../harmonic-polynomial.md). Write $H(r\omega)=r^nY(\omega)$ for $H\in\mathcal H_n$. Substitution in the [Laplacian](../../../../../laplacian.md) identity gives

$$
0=r^{n-2}\bigl(\Delta Y-n(n+d-1)Y\bigr).
$$

Thus each restricted [harmonic polynomial](../../../../../harmonic-polynomial.md) is a [spherical harmonic](../../../../../spherical-harmonic.md) with [eigenvalue](../../../../../eigenvalue.md) $\lambda_n=n(n+d-1)$.

To count these [spherical harmonics](../../../../../spherical-harmonic.md), give [polynomials](../../../../../polynomial-split.md) the [Fischer inner product](../../../../../fischer-inner-product.md) $\langle x^\alpha,x^\beta\rangle_F=\alpha!\delta_{\alpha\beta}$. Multiplication by $x_j$ is adjoint to $\partial_j$, so multiplication by $r^2$ is adjoint to the ordinary signed [Laplacian](../../../../../laplacian.md) $\sum_j\partial_j^2$. In these finite-dimensional [inner product spaces](../../../../../inner-product-space.md), the orthogonal complement of $r^2\mathcal P_{n-2}$ is exactly $\mathcal H_n$. Hence the [Fischer decomposition](../../../../../harmonic-decomposition-of-homogeneous-polynomials.md) is

$$
\mathcal P_n=\mathcal H_n\oplus r^2\mathcal P_{n-2}.
$$

Multiplication by $r^2$ is injective, while restriction of a [homogeneous polynomial](../../../../../homogeneous-polynomial.md) to the [sphere](../../../../../sphere.md) is injective: homogeneity recovers its value at every nonzero point. Counting [monomials](../../../../../monomial.md) now gives the [eigenvalue multiplicity](../../../../../eigenvalue-multiplicity.md)

$$
\boxed{m_n=\dim\mathcal H_n=\binom{n+d}{d}-\binom{n+d-2}{d},\qquad n=0,1,2,\ldots,}
$$

where the second term is zero for $n<2$.

It remains to establish that these are all the [eigenvalues](../../../../../eigenvalue.md) and their full [multiplicities](../../../../../multiplicity-mathematics.md). Iterating the [Fischer decomposition](../../../../../harmonic-decomposition-of-homogeneous-polynomials.md) expresses every restricted [polynomial](../../../../../polynomial-split.md) as a sum of the restricted [harmonic polynomials](../../../../../harmonic-polynomial.md). Restricted [polynomials](../../../../../polynomial-split.md) separate points and contain the constants, so the [Stone-Weierstrass theorem](../../../../../stone-weierstrass-theorem.md) makes their span dense in continuous functions on the [sphere](../../../../../sphere.md), hence dense in its [L2 space](../../../../../l2-space-is-a-hilbert-space.md). The [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md) is self-adjoint, and the distinct numbers $\lambda_n$ strictly increase for $d\geq1$. Its different [eigenspaces](../../../../../eigenspace.md) are therefore orthogonal. Any additional [eigenfunction](../../../../../eigenfunction.md), or any additional vector in one of these [eigenspaces](../../../../../eigenspace.md) orthogonal to its known [spherical harmonics](../../../../../spherical-harmonic.md), would be orthogonal to a dense subspace and hence zero. The standard compact elliptic [spectral theorem](../../../../../spectral-theorem.md) then shows that the [spectrum of the round sphere](../../../../../spectrum-of-the-round-sphere.md) is precisely **$\lambda_n=n(n+d-1)$ with multiplicity $m_n$**. For $S^1$ this gives multiplicity one at zero and two at $n^2$ for $n\geq1$. If the degenerate case $d=0$ is included, $S^0$ has two points and its [Laplacian](../../../../../laplacian.md) is zero on a two-dimensional function space.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
