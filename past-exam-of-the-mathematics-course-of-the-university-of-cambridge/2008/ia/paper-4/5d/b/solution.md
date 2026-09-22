<h1 id="5d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [countable set](../../../../../../countable-set.md) $A$, the [polynomials](../../../../../../polynomial-split.md) of [polynomial degree](../../../../../../degree-of-a-polynomial.md) at most $d$ with coefficients in $A$ are described by coefficient tuples in $A^{d+1}$. The [finite Cartesian power of a countable set](../../../../../../finite-cartesian-power-of-a-countable-set.md) result makes this a [countable set](../../../../../../countable-set.md). Taking the union over $d\geq0$ shows there are only countably many such [polynomials](../../../../../../polynomial-split.md) altogether; restricting to the nonzero [polynomials](../../../../../../polynomial-split.md) preserves countability.

A nonzero [polynomial](../../../../../../polynomial-split.md) of [polynomial degree](../../../../../../degree-of-a-polynomial.md) $d$ has at most $d$ distinct [roots of a polynomial](../../../../../../root-of-a-polynomial.md). To see the bound, a root $r$ gives the factorization $P(x)=(x-r)Q(x)$ by the [factor theorem](../../../../../../factor-theorem.md), and each other root is a root of $Q$, whose degree is $d-1$; induction starts with a nonzero constant, which has no roots. Thus $\phi(A)$ is a [countable union of countable sets](../../../../../../countable-union-of-countable-sets.md), each of them finite, and is a [countable set](../../../../../../countable-set.md).

Starting with the given [countable set](../../../../../../countable-set.md) $A_0$, [mathematical induction](../../../../../../mathematical-induction.md) now shows that every $A_n=\phi(A_{n-1})$ is countable. A final application of the [countable union of countable sets](../../../../../../countable-union-of-countable-sets.md) theorem gives

$$
\boxed{\bigcup_{n=1}^{\infty}A_n\text{ is countable}.}
$$

This countability argument does not require that the sequence of [sets](../../../../../../set-split.md) be increasing.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5D](../../5d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
