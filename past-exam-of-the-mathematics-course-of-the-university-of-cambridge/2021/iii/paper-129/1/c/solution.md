<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In the vector space $\mathbb F_2^n$, addition and subtraction agree. Put $V=\langle Y\rangle$, the [vector subspace](../../../../../../vector-subspace.md) spanned by $Y$, and

$$
H=A+A+V.
$$

Part b gives $4A\subseteq2A+V=H$. Conversely $2A\subseteq4A$, because two copies of any fixed element of $A$ sum to zero. Hence

$$
H+H=4A+V\subseteq2A+V=H,
$$

and $0\in H$, so $H$ is a [subgroup](../../../../../../subgroup.md). For any $a_0\in A$, every $a\in A$ satisfies $a-a_0=a+a_0\in H$, and therefore $A\subseteq a_0+H$.

Because $y_1=0$, the [dimension of a vector space](../../../../../../dimension-vector-space.md) $V$ is at most $|Y|-1\leq2K^2-2$. Consequently

$$
|H|\leq|A+A|\,|V|
\leq K2^{2K^2-2}|A|
\leq K^2 2^{2K^2-2}|A|,
$$

where the last inequality uses $K\geq1$. This is the requested bound.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 129](../../../paper-129-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
