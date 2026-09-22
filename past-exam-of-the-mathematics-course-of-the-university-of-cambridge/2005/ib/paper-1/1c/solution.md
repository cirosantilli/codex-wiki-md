<h1 id="1c/solution">Solution</h1>

↑ **Parent:** [1C](../1c.md)

The [minimal polynomial](../../../../../minimal-polynomial.md) $m_\beta(t)$ of the [linear map](../../../../../linear-map.md) $\beta$ is the unique [monic polynomial](../../../../../monic-polynomial.md) of smallest degree satisfying $m_\beta(\beta)=0$. An annihilating [polynomial](../../../../../polynomial-split.md) exists because the powers $I,\beta,\beta^2,\ldots$ lie in the finite-dimensional [vector space](../../../../../vector-space-split.md) $\operatorname{End}(V)$ and are therefore [linearly dependent](../../../../../linear-dependence.md). If two monic annihilating [polynomials](../../../../../polynomial-split.md) had the same least degree, their difference would be an annihilating [polynomial](../../../../../polynomial-split.md) of smaller degree, so they coincide.

Write $m_\beta(t)=a_0+tq(t)$. If $a_0\ne0$, evaluation at the [linear map](../../../../../linear-map.md) gives $\beta q(\beta)=-a_0I$. Since $\beta$ commutes with every [polynomial](../../../../../polynomial-split.md) in itself, this is a two-sided inverse:

$$
\boxed{\beta^{-1}=-\frac{q(\beta)}{a_0}}.
$$

Conversely, if $\beta$ is an [invertible linear map](../../../../../invertible-linear-map.md) and $a_0=0$, then $m_\beta(t)=tq(t)$ and multiplication of $\beta q(\beta)=0$ by $\beta^{-1}$ gives $q(\beta)=0$, contradicting the defining least degree. Thus **invertibility is equivalent to a nonzero constant term of the minimal polynomial**. In the zero-dimensional case the [minimal polynomial](../../../../../minimal-polynomial.md) is $1$ and the same conclusion holds.

## ↑ Ancestors (10)

1. [1C](../1c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
