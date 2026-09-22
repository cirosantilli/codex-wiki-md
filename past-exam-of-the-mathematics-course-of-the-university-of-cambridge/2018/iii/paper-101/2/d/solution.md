<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**Yes: $R$ can have nonzero zero divisors.** Let $R=k\times k$, a [direct product of rings](../../../../../../direct-product-of-rings.md), where $k$ is any [field](../../../../../../field.md). The nonzero [idempotents](../../../../../../idempotent.md) $e_1=(1,0)$ and $e_2=(0,1)$ satisfy $e_1e_2=0$, so both are [zero divisors](../../../../../../zero-divisor.md).

There are exactly two [prime ideals](../../../../../../prime-ideal.md):

$$
P_1=0\times k,\qquad P_2=k\times0.
$$

Indeed, any [prime ideal](../../../../../../prime-ideal.md) must contain $e_1$ or $e_2$, since their product is zero. If it contains $e_1$, it contains $k\times0$ and corresponds to a [prime ideal](../../../../../../prime-ideal.md) of the [quotient ring](../../../../../../quotient-ring.md) $k$, whose only [prime ideal](../../../../../../prime-ideal.md) is zero; hence it equals $P_2$. The other case gives $P_1$.

For the [localization at a prime ideal](../../../../../../localization-at-a-prime-ideal.md) $P_1$, every denominator $(u,v)\notin P_1$ has $u\ne0$, and

$$
R_{P_1}\longrightarrow k,\qquad
\frac{(a,b)}{(u,v)}\longmapsto\frac a u
$$

is an isomorphism. It is surjective using constant first-coordinate fractions. It is injective because a numerator with first coordinate zero is annihilated by $e_1\notin P_1$, so its fraction is zero. Interchanging the coordinates proves $R_{P_2}\cong k$.

Thus the [localization at a prime ideal](../../../../../../localization-at-a-prime-ideal.md) is a [field](../../../../../../field.md) in every case, although $R$ has [zero divisors](../../../../../../zero-divisor.md). The obstruction to using the previous part's argument is that the two nonzero factors of a zero product can survive at different [prime ideals](../../../../../../prime-ideal.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
