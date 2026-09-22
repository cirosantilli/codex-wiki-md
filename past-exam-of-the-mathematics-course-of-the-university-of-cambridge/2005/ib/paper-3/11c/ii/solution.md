<h1 id="11c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The polynomial $p=x^5-4x+2$ satisfies the [Eisenstein criterion](../../../../../../eisenstein-criterion.md) at the prime two: every nonleading coefficient is even, the leading coefficient is not, and the constant term is not divisible by four. Hence it is irreducible over $\mathbb Q$. Its ideal is maximal in $\mathbb Q[x]$; explicitly, for any polynomial not divisible by $p$, the Euclidean algorithm gives $ag+bp=1$, furnishing the inverse of its residue class. Thus

$$
\boxed{\mathbb Q[x]/(p)\text{ is a field}.}
$$

For the integer quotient, division by the monic polynomial $p$ gives a unique remainder of degree below five with integer coefficients. If an integer polynomial becomes zero in the rational quotient, its integer remainder is still divisible by $p$ over $\mathbb Q$, so must be zero. This gives an injective ring map $\mathbb Z[x]/(p)\to\mathbb Q[x]/(p)$, proving the [monic irreducible integer-polynomial quotient is a domain](../../../../../../monic-irreducible-integer-polynomial-quotient-is-a-domain.md).

The same unique-remainder argument makes the integer quotient a free abelian group with basis $1,x,x^2,x^3,x^4$. The class of two is nonzero and cannot have an inverse: twice an integer remainder cannot equal the remainder one. Consequently

$$
\boxed{\mathbb Z[x]/(p)\text{ is an integral domain but not a field}.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [11C](../../11c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
