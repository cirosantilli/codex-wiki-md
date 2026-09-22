<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The group is the [direct product of groups](../../../../../direct-product-of-groups.md) $\mathbb Z_p\times\mathbb Z_q$. Repeatedly adding $(1,1)$ returns to $(0,0)$ for the first time when both $p$ and $q$ divide the step number. Its [order of a group element](../../../../../order-of-a-group-element.md) is therefore $\operatorname{lcm}(p,q)$. If $p,q$ are [coprime](../../../../../coprime-integers.md), this is $pq$, so it generates every element:

$$
\boxed{G(p,q)\cong C_{pq}.}
$$

Explicitly, $[t]_{pq}\mapsto([t]_p,[t]_q)$ is the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) [group isomorphism](../../../../../group-isomorphism.md).

If $d=\gcd(p,q)>1$, every pair satisfies

$$
\frac{pq}{d}(n,m)=(0,0).
$$

Thus every element order divides $pq/d<pq$, and no element can generate the whole group. Hence

$$
\boxed{G(p,q)\text{ is cyclic exactly when }\gcd(p,q)=1.}
$$

This is the [cyclicity of a product of two finite cyclic groups](../../../../../cyclicity-of-a-product-of-two-finite-cyclic-groups.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [9](../../9.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
