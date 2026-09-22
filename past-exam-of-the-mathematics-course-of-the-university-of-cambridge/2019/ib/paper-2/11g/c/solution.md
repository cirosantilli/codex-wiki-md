<h1 id="11g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $q=p^n$. Every extension of $k=\mathbb F_p$ has [characteristic](../../../../../../characteristic-of-a-field.md) $p$, so the iterated [Frobenius endomorphism](../../../../../../frobenius-endomorphism.md) satisfies

$$
(a+b)^q=a^q+b^q,
\qquad
(ab)^q=a^qb^q.
$$

The root set is $K=\{a\in F:a^q=a\}$. It contains $0$ and $1$. If $a,b\in K$, then

$$
(a-b)^q=a^q-b^q=a-b,
\qquad
(ab)^q=a^qb^q=ab,
$$

so it is closed under subtraction and multiplication. If $a\in K$ is nonzero, then

$$
(a^{-1})^q=(a^q)^{-1}=a^{-1}.
$$

Thus $K$ is closed under multiplicative inverses as well, and is therefore a [field](../../../../../../field.md). This is the [polynomial characterization of a finite field](../../../../../../polynomial-characterization-of-a-finite-field.md); in fact it is the [finite field](../../../../../../finite-field.md) with $q$ elements, since $X^q-X$ has degree $q$ and no repeated roots.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11G](../../11g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
