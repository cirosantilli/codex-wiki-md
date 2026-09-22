<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Expand the [determinant](../../../../../../determinant.md) of the matrix $A_1$ from part (b) by the [Leibniz formula for determinants](../../../../../../leibniz-formula-for-determinants.md). A matrix entry is a signed sum of [monomials](../../../../../../monomial.md) arising from the possible corners at its crossing. Choosing one summand in every row chooses one corner at every crossing, while choosing distinct columns puts exactly one chosen corner in every region $R_i$ with $i>1$ and none in the two deleted regions $R_0,R_1$. The surviving determinant terms are therefore in bijection with the [Kauffman states](../../../../../../kauffman-state-of-a-knot-diagram.md) $s\in\mathcal S(D)$.

The [sign of a permutation](../../../../../../sign-of-a-permutation.md) in the determinant together with the corner signs gives $(-1)^{\epsilon(s)}$, and multiplying the corner monomials gives $t^{\delta(s)}$. Since part (b) identifies this determinant with the [Alexander polynomial of a knot](../../../../../../alexander-polynomial.md) up to a unit,

$$
\boxed{\Delta_K(t)\doteq\sum_{s\in\mathcal S(D)}(-1)^{\epsilon(s)}t^{\delta(s)}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 112](../../../paper-112-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
