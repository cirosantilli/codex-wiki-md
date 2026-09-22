<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Multiply the [Karush-Kuhn-Tucker conditions](../../../../../../karush-kuhn-tucker-conditions.md) on the right by $\widehat\Omega$ and take the [matrix trace](../../../../../../matrix-trace.md):

$$
-p+\operatorname{Tr}(S\widehat\Omega)+\lambda\operatorname{Tr}(Z\widehat\Omega)=0.
$$

Symmetry and the defining property of the [subgradient of the absolute value](../../../../../../subgradient-of-the-absolute-value.md) give

$$
\operatorname{Tr}(Z\widehat\Omega)
=\sum_{i,j}Z_{ij}\widehat\Omega_{ij}
=\sum_{i,j}|\widehat\Omega_{ij}|.
$$

Consequently the last two terms in the objective sum to $p$, and hence

$$
\boxed{Q(\widehat\Omega)=-\log\det\widehat\Omega+p.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
