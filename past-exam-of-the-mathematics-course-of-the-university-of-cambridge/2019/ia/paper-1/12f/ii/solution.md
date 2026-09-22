<h1 id="12f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $C_n$ be the union of the $2^n$ closed intervals remaining after $n$ steps of the [Cantor set](../../../../../../cantor-set.md) construction. Their total length is $(2/3)^n$. Any point outside $C_n$ has a ternary expansion with a $1$ among its first $n$ digits, so $A^c\subseteq C_n$. Endpoints of deleted intervals also belong to $A$ because they have an alternative ternary expansion containing a $1$, as in $2/3=0.1222\ldots{}_3$.

A partition using all endpoints of $C_n$ has lower Darboux sum at least

$$
1-\left(\frac23\right)^n.
$$

Since $A$ is dense, every upper Darboux sum is one. Letting $n\to\infty$ gives equal upper and lower integrals, and therefore

$$
\boxed{f\text{ is Riemann integrable and }\int_0^1f(x)\,dx=1}.
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [12F](../../12f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
