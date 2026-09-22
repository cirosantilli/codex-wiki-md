<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In additive notation every element $(a,b)\in\mathbb Z_2\times\mathbb Z_4$ obeys $4(a,b)=(0,0)$. Its [order of a group element](../../../../../order-of-a-group-element.md) therefore divides four, whereas $1\in\mathbb Z_8$ has order eight. A [group isomorphism](../../../../../group-isomorphism.md) preserves element orders, so

$$
\boxed{\mathbb Z_2\times\mathbb Z_4\not\cong\mathbb Z_8.}
$$

For the second product, define the [group homomorphism](../../../../../group-homomorphism.md)

$$
\Psi:\mathbb Z_6\longrightarrow\mathbb Z_2\times\mathbb Z_3,\qquad
[t]_6\longmapsto([t]_2,[t]_3).
$$

It is well-defined because multiples of six are divisible by both two and three. Its [kernel](../../../../../kernel-of-a-linear-map-split.md) contains only zero: simultaneous divisibility by two and three implies divisibility by six. Thus $\Psi$ is injective, and equal finite [group orders](../../../../../order-of-a-finite-group.md) make it surjective. Explicitly the six images are

$$
(0,0),(1,1),(0,2),(1,0),(0,1),(1,2).
$$

Therefore

$$
\boxed{\mathbb Z_2\times\mathbb Z_3\cong\mathbb Z_6.}
$$

For general positive integers $n,m$, the [order of a direct-product element](../../../../../order-of-a-direct-product-element.md) is the [least common multiple](../../../../../least-common-multiple.md) of its component orders. Hence every element order divides $\operatorname{lcm}(n,m)=nm/\gcd(n,m)$, while $(1,1)$ attains this order. It generates the whole product precisely when $n,m$ are [coprime](../../../../../coprime-integers.md):

$$
\boxed{\mathbb Z_n\times\mathbb Z_m\cong\mathbb Z_{nm}\quad\Longleftrightarrow\quad\gcd(n,m)=1.}
$$

This is the [cyclicity of a product of two finite cyclic groups](../../../../../cyclicity-of-a-product-of-two-finite-cyclic-groups.md), with the explicit isomorphism furnished by the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [9](../../9.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
