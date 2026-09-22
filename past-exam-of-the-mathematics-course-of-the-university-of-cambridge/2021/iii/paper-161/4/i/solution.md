<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For each $A\in\mathcal A$, define over $\mathbb F_p$

$$
P_A(x_1,\ldots,x_n)
=\prod_{e\in E}\left(\sum_{i\in A}x_i-e\right).
$$

Replace every power $x_i^r$ with $r\geq1$ by $x_i$; this does not change the values on [characteristic vectors of sets](../../../../../../characteristic-vector-of-a-set.md) and produces a multilinear polynomial of degree at most $m$.

At the characteristic vector of $B\in\mathcal A$,

$$
P_A(\mathbf1_B)=\prod_{e\in E}(|A\cap B|-e).
$$

This is zero when $A\ne B$, whereas

$$
P_A(\mathbf1_A)=\prod_{e\in E}(|A|-e)\ne0.
$$

The evaluation matrix is diagonal with nonzero diagonal, so the polynomials $P_A$ are [linearly independent](../../../../../../linear-independence.md). The space of multilinear polynomials of degree at most $m$ has the monomial basis $\prod_{i\in S}x_i$ for $|S|\leq m$ and dimension $\sum_{i=0}^m\binom ni$. Hence the [modular intersection bound for a set family](../../../../../../modular-intersection-bound-for-a-set-family.md) gives

$$
\boxed{|\mathcal A|\leq\binom n0+\binom n1+\cdots+\binom nm}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 161](../../../paper-161-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
