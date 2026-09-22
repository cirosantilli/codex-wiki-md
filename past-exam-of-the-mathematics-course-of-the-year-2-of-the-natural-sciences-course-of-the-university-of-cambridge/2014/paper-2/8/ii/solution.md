<h1 id="8/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write the cyclic factors additively. The [order of a group element](../../../../../order-of-a-group-element.md) $(r,s)$ in a [direct product of groups](../../../../../direct-product-of-groups.md) is the least common multiple of its component orders, since a power is the identity exactly when it is the identity in both coordinates.

In $C_2\times C_3$, $(1,1)$ has order $\operatorname{lcm}(2,3)=6$, so it generates all six pairs. An explicit [group isomorphism](../../../../../group-isomorphism.md) is

$$
\boxed{C_6\longrightarrow C_2\times C_3,\qquad[k]_6\longmapsto([k]_2,[k]_3).}
$$

It is well defined and multiplicative in additive notation; its kernel is zero because an integer divisible by both two and three is divisible by six. Equal finite orders then give bijectivity.

In $C_2\times C_4$, every element has order dividing four. A generator of $C_8$ has order eight, and isomorphisms preserve element orders, so

$$
\boxed{C_2\times C_4\not\cong C_8.}
$$

For positive integers $n,m$, the maximum element order in $C_n\times C_m$ is $\operatorname{lcm}(n,m)=nm/\gcd(n,m)$, attained by a pair of generators. The product is cyclic of order $nm$ exactly when that number is $nm$. Thus [cyclicity of a product of two finite cyclic groups](../../../../../cyclicity-of-a-product-of-two-finite-cyclic-groups.md) gives

$$
\boxed{C_n\times C_m\cong C_{nm}\quad\Longleftrightarrow\quad\gcd(n,m)=1.}
$$

For coprime factors the map $[k]_{nm}\mapsto([k]_n,[k]_m)$ gives the isomorphism, the group form of the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [8](../../8.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
