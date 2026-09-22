<h1 id="10f/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

If $\alpha^*=g(\alpha)$, then $\alpha$ commutes with its adjoint because it commutes with every [polynomial](../../../../../../polynomial-split.md) in itself. Hence $\alpha$ is a [normal operator](../../../../../../normal-operator.md).

Conversely let $\lambda_1,\ldots,\lambda_r$ be the distinct [eigenvalues](../../../../../../eigenvalue.md) of a normal $\alpha$. The [orthonormal eigenbasis](../../../../../../orthonormal-eigenbasis.md) from part (ii) reduces the desired identity to $g(\lambda_j)=\overline\lambda_j$. [Lagrange interpolation polynomial](../../../../../../lagrange-polynomial.md) provides the polynomial

$$
\boxed{g(z)=\sum_{j=1}^{r}\overline\lambda_j
\prod_{\ell\ne j}\frac{z-\lambda_\ell}{\lambda_j-\lambda_\ell},
\qquad \alpha^*=g(\alpha).}
$$

Repeated eigenvalues cause no difficulty because interpolation uses only distinct values. If $V=\{0\}$, use $g=0$. This proves both directions of the third equivalence.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [10F](../../10f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
