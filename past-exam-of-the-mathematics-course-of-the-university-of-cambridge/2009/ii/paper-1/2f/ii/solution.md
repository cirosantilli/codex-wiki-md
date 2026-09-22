<h1 id="2f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use [Gaussian quadrature](../../../../../../gaussian-quadrature.md): choose the $n$ nodes as the roots of the degree-$n$ [Legendre polynomial](../../../../../../legendre-polynomial.md), which are distinct and inside $(-1,1)$. Retain the integrated [Lagrange interpolation](../../../../../../lagrange-polynomial.md) weights. With the standard normalization $P_n(1)=1$, they can be written

$$
\boxed{A_j=\frac{2}{(1-x_j^2)[P_n'(x_j)]^2}.}
$$

The [orthogonality](../../../../../../orthogonal-vectors.md) of the [Legendre polynomial](../../../../../../legendre-polynomial.md) against all lower-degree [polynomials](../../../../../../polynomial-split.md) makes this quadrature exact up to degree $2n-1$, twice the arbitrary-node degree apart from the endpoint count. This is the Gauss–Legendre choice of [Gaussian quadrature](../../../../../../gaussian-quadrature.md) nodes and weights.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2F](../../2f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
