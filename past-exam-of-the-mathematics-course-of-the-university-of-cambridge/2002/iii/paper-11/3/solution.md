<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [coefficient](../../../../../coefficient.md) form of the [Combinatorial Nullstellensatz](../../../../../combinatorial-nullstellensatz.md) is as follows. Let $F$ be a [field](../../../../../field.md), let $P\in F[x_1,\ldots,x_r]$ have total degree at most $t_1+\cdots+t_r$, and suppose the [coefficient](../../../../../coefficient.md) of $x_1^{t_1}\cdots x_r^{t_r}$ is nonzero. For finite [subsets](../../../../../subset.md) $S_i\subset F$ with $|S_i|>t_i$, there is a point of $S_1\times\cdots\times S_r$ where $P$ is nonzero.

For completeness, restrict to $|S_i|=t_i+1$. The [coefficient](../../../../../coefficient.md) identity is

$$
[x_1^{t_1}\cdots x_r^{t_r}]P
=\sum_{a_i\in S_i}\frac{P(a_1,\ldots,a_r)}{\prod_i\prod_{b\in S_i\setminus\{a_i\}}(a_i-b)}.
$$

By [Lagrange interpolation](../../../../../lagrange-polynomial.md), the one-variable weighted sum on the right kills powers below $t_i$ and equals one on the power $t_i$. Any [monomial](../../../../../monomial.md) of total degree at most $\sum t_i$, other than the specified one, has some exponent below $t_i$ and therefore contributes zero; the specified [monomial](../../../../../monomial.md) contributes its [coefficient](../../../../../coefficient.md). Every denominator is nonzero in the [field](../../../../../field.md). Hence a nonzero [coefficient](../../../../../coefficient.md) forces a nonzero grid value. The two applications below use this [coefficient](../../../../../coefficient.md) form.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
