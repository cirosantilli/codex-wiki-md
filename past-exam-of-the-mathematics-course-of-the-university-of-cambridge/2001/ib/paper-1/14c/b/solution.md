<h1 id="14c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $I$ denote the identity endomorphism. The two-root [minimal polynomial](../../../../../../minimal-polynomial.md) gives $(\alpha-\lambda_1I)(\alpha-\lambda_2I)=0$. Every [vector](../../../../../../vector.md) has the decomposition

$$
v=\frac{(\alpha-\lambda_2I)v}{\lambda_1-\lambda_2}+\frac{(\alpha-\lambda_1I)v}{\lambda_2-\lambda_1}.
$$

The first summand lies in the [eigenspace](../../../../../../eigenspace.md) $E_1=\ker(\alpha-\lambda_1I)$, and the second in $E_2$. If a [vector](../../../../../../vector.md) belongs to both, subtracting its two [eigenvalue](../../../../../../eigenvalue.md) equations gives $(\lambda_1-\lambda_2)v=0$, hence $v=0$. Thus $V=E_1\oplus E_2$.

For distinct real roots $\lambda_1,\ldots,\lambda_m$, define [polynomial](../../../../../../polynomial-split.md) projectors

$$
P_i=\prod_{j\ne i}\frac{\alpha-\lambda_jI}{\lambda_i-\lambda_j}.
$$

The [Lagrange interpolation](../../../../../../lagrange-polynomial.md) [polynomials](../../../../../../polynomial-split.md) in this expression sum to one: their sum has degree at most $m-1$ and equals one at the $m$ distinct roots. Hence $\sum_iP_i=I$. Also $(\alpha-\lambda_iI)P_i=0$, because its numerator is the [minimal polynomial](../../../../../../minimal-polynomial.md) evaluated at $\alpha$. Thus every [vector](../../../../../../vector.md) is a sum of [eigenvectors](../../../../../../eigenvector.md), $v=\sum_iP_iv$. On $E_j$, $P_i$ acts as $\delta_{ij}I$, so applying $P_i$ to any zero sum of [vectors](../../../../../../vector.md) from the [eigenspaces](../../../../../../eigenspace.md) shows that every summand is zero. Therefore

$$
\boxed{V=\bigoplus_{i=1}^m\ker(\alpha-\lambda_iI)}.
$$

Choosing a basis in each [eigenspace](../../../../../../eigenspace.md) proves [diagonalizability](../../../../../../diagonalizable-matrix.md) over the reals. Conversely, if a real [matrix](../../../../../../matrix.md) is similar over the reals to a diagonal [matrix](../../../../../../matrix.md), a [polynomial](../../../../../../polynomial-split.md) annihilates it exactly when it vanishes at each distinct real diagonal entry. Its [minimal polynomial](../../../../../../minimal-polynomial.md) is therefore the product of those distinct linear factors. We have proved **real diagonalizability is equivalent to a [minimal polynomial](../../../../../../minimal-polynomial.md) with distinct real roots**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [14C](../../14c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
