<h1 id="2/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [direct system of abelian groups](../../../../../../direct-system-of-abelian-groups.md) over the directed poset $A$ consists of groups $G_a$ and maps $\phi_{ab}:G_a\to G_b$ for $a\leq b$, satisfying $\phi_{aa}=1$ and $\phi_{bc}\phi_{ab}=\phi_{ac}$. Its [direct limit](../../../../../../direct-limit-of-abelian-groups.md) is the quotient of $\bigoplus_aG_a$ by the relations $g_a\sim\phi_{ab}(g_a)$.

For the displayed sequence, put $P_0=1$ and $P_n=a_0a_1\cdots a_{n-1}$. Map the copy of $\mathbb Z$ at stage $n$ to $\mathbb Q$ by

$$
m\longmapsto \frac{m}{P_n}.
$$

This is compatible with the next transition because $a_nm/P_{n+1}=m/P_n$. The universal property of the [direct limit](../../../../../../direct-limit-of-abelian-groups.md) therefore identifies it with

$$
\boxed{\bigcup_{n\geq0}\frac1{P_n}\mathbb Z.}
$$

In reduced form, these are exactly the rationals whose denominator divides one of the finite products $P_n$. This is the [sequential direct limit of multiplication maps on the integers](../../../../../../sequential-direct-limit-of-multiplication-maps-on-the-integers.md).

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2](../../2.md)
3. [Paper 114](../../../paper-114-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
