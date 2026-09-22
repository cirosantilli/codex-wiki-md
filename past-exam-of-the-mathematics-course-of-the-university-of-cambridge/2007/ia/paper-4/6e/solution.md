<h1 id="6e/solution">Solution</h1>

↑ **Parent:** [6E](../6e.md)

We use these countability facts: the [integers](../../../../../integer.md) are [countable](../../../../../countable-set.md); a finite [Cartesian product](../../../../../cartesian-product.md) of [countable sets](../../../../../countable-set.md) is [countable](../../../../../countable-set.md); a [countable](../../../../../countable-set.md) union of [countable sets](../../../../../countable-set.md) is [countable](../../../../../countable-set.md); and every subset of a [countable set](../../../../../countable-set.md) is [countable](../../../../../countable-set.md). Finite products can be enumerated by listing index tuples in increasing maximum coordinate, and [countable](../../../../../countable-set.md) unions by diagonal enumeration of pairs of indices.

Fix $d\ge1$. For each degree bound $D$, there are finitely many monomials $X_1^{\alpha_1}\cdots X_d^{\alpha_d}$ with $\alpha_1+\cdots+\alpha_d\le D$. An [integer](../../../../../integer.md) [polynomial](../../../../../polynomial-split.md) of total degree at most $D$ is specified by an [integer](../../../../../integer.md) coefficient for each of them, so these [polynomials](../../../../../polynomial-split.md) form a finite [Cartesian product](../../../../../cartesian-product.md) of copies of $\mathbb Z$ and are [countable](../../../../../countable-set.md). Every [polynomial](../../../../../polynomial-split.md) has some finite degree bound. Taking the union over $D=0,1,2,\ldots$ proves the [countability of integer polynomial rings](../../../../../countability-of-integer-polynomial-rings.md):

$$
\boxed{\mathbb Z[X_1,\ldots,X_d]\text{ is countably infinite}.}
$$

It is infinite because it contains all [integer](../../../../../integer.md) constant [polynomials](../../../../../polynomial-split.md).

For $d=1$, each nonzero [polynomial](../../../../../polynomial-split.md) has only finitely many real roots: repeated application of the [factor theorem](../../../../../factor-theorem.md) bounds their number by its degree. The real [algebraic numbers](../../../../../algebraic-number.md) are the union of these finite root sets over the countably many nonzero [integer](../../../../../integer.md) [polynomials](../../../../../polynomial-split.md). Thus they are [countable](../../../../../countable-set.md). If the real [transcendental numbers](../../../../../transcendental-number.md) were [countable](../../../../../countable-set.md) too, their union with the [algebraic numbers](../../../../../algebraic-number.md) would make $\mathbb R$ [countable](../../../../../countable-set.md), contrary to the allowed uncountability assumption. Hence **there are uncountably many real [transcendental numbers](../../../../../transcendental-number.md)**.

To construct an [algebraically independent real sequence](../../../../../algebraically-independent-real-sequence.md), choose $x_1$ outside the [algebraic numbers](../../../../../algebraic-number.md). Suppose $x_1,\ldots,x_d$ already satisfy the required nonvanishing condition. For each nonzero $P\in\mathbb Z[X_1,\ldots,X_d,T]$, write

$$
P(X_1,\ldots,X_d,T)=\sum_{j=0}^sP_j(X_1,\ldots,X_d)T^j.
$$

At least one coefficient [polynomial](../../../../../polynomial-split.md) $P_j$ is nonzero, and the inductive hypothesis makes its value at $(x_1,\ldots,x_d)$ nonzero. Consequently $P(x_1,\ldots,x_d,T)$ is a nonzero one-variable [polynomial](../../../../../polynomial-split.md) and has only finitely many real roots. There are countably many choices of $P$, so the union of all these forbidden roots is [countable](../../../../../countable-set.md). Choose $x_{d+1}$ outside it, which is possible because $\mathbb R$ is uncountable. This extends the nonvanishing condition to $d+1$. Recursion therefore gives

$$
\boxed{f(x_1,\ldots,x_d)\ne0\quad\text{for every }d\ge1
\text{ and nonzero }f\in\mathbb Z[X_1,\ldots,X_d].}
$$

In particular the chosen numbers are distinct, since a relation $X_i-X_j$ is forbidden. Clearing rational denominators shows that every finite initial segment consists of [algebraically independent elements](../../../../../algebraically-independent-elements.md) over $\mathbb Q$.

## ↑ Ancestors (10)

1. [6E](../6e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
