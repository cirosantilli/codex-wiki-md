<h1 id="2f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Define the [Lagrange interpolation polynomials](../../../../../../lagrange-polynomial.md)

$$
L_j(x)=\prod_{\ell\ne j}\frac{x-x_\ell}{x_j-x_\ell},\qquad\boxed{A_j=\int_{-1}^1L_j(x)\,dx.}
$$

Distinct [interpolation nodes](../../../../../../interpolation-node.md) ensure every denominator is nonzero and $L_j(x_i)=\delta_{ij}$. For a [polynomial](../../../../../../polynomial-split.md) of degree at most $n-1$, the difference $P(x)-\sum_jP(x_j)L_j(x)$ has degree at most $n-1$ and vanishes at $n$ distinct points, so it is zero. Integrating this [Lagrange interpolation](../../../../../../lagrange-polynomial.md) identity proves the required exact quadrature formula. This also covers $n=1$, when the empty product is one and its weight is two.

## ↑ Ancestors (11)

1. [I](../i.md)
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
