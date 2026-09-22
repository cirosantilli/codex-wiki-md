<h1 id="1i/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

[Lagrange theorem for polynomial congruences](../../../../../../lagrange-theorem-for-polynomial-congruences.md) says that a nonzero [polynomial](../../../../../../polynomial-split.md) of degree $d$ over a [field](../../../../../../field.md) has at most $d$ distinct [roots of a polynomial](../../../../../../root-of-a-polynomial.md). It follows by repeatedly factoring out $x-a$ at a root. Over the [finite field](../../../../../../finite-field.md) $\mathbb F_p$, the only solutions of $x^2=1$ are $1$ and $-1$: these are distinct because $p$ is odd, and the root bound excludes any others.

Every nonzero element has a unique [multiplicative inverse](../../../../../../multiplicative-inverse.md). Pair each element of $\mathbb F_p^\times$ with its inverse. All pairs of distinct elements contribute $1$ to the product; the only unpaired elements are $1$ and $-1$. Thus [Wilson theorem](../../../../../../wilson-s-theorem.md) follows:

$$
\boxed{(p-1)!\equiv-1\pmod p.}
$$

If Lagrange's theorem is formulated for [finite groups](../../../../../../finite-group.md), it states that the order of a [subgroup](../../../../../../subgroup.md) divides the order of the group; in particular every element of $\mathbb F_p^\times$ has order dividing $p-1$. The inverse-pairing proof above establishes the required congruence directly.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1I](../../1i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
