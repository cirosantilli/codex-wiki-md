<h1 id="2i/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [Lagrange interpolation polynomial](../../../../../../lagrange-polynomial.md)

$$
\ell_j(t)=\prod_{i\ne j}\frac{t-x_i}{x_j-x_i},\qquad \ell_j(x_i)=\delta_{ij}.
$$

Its square has degree $2n-2$, so the exactness already proved gives

$$
\boxed{A_j=\int_{-1}^1\ell_j(t)^2\,dt>0.}
$$

The [positive weights of Gaussian quadrature](../../../../../../positive-weights-of-gaussian-quadrature.md) follow because $\ell_j$ is a nonzero continuous [polynomial](../../../../../../polynomial-split.md). Thus these [Gaussian quadrature](../../../../../../gaussian-quadrature.md) weights are in fact positive, rather than merely nonnegative.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2I](../../2i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
