<h1 id="8/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Closure of the componentwise operation follows from closure in each factor. For three pairs, [associativity](../../../../../associative-property.md) holds coordinatewise:

$$
\bigl((g_1,g_2)(h_1,h_2)\bigr)(k_1,k_2)
=\bigl((g_1h_1)k_1,(g_2h_2)k_2\bigr)
=\bigl(g_1(h_1k_1),g_2(h_2k_2)\bigr).
$$

The [identity element](../../../../../identity-element.md) is $(e_1,e_2)$ and the [inverse element](../../../../../inverse-element.md) of $(g_1,g_2)$ is $(g_1^{-1},g_2^{-1})$. These verify all [group axioms](../../../../../group-axioms.md) for the [direct product of groups](../../../../../direct-product-of-groups.md). Counting independent choices gives

$$
\boxed{|G_1\times G_2|=|G_1|\,|G_2|.}
$$

The subset $N=G_1\times\{e_2\}$ contains the identity and is closed under products and inverses, so it is a [subgroup](../../../../../subgroup.md). For any $x=(a,b)$ in the product and $(g,e_2)\in N$,

$$
x(g,e_2)x^{-1}=(aga^{-1},be_2b^{-1})=(aga^{-1},e_2)\in N.
$$

Conjugation by $x^{-1}$ gives the reverse inclusion, and hence

$$
\boxed{xNx^{-1}=N,\qquad N\mathrel{\trianglelefteq}G_1\times G_2.}
$$

This is the definition of a [normal subgroup](../../../../../normal-subgroup.md).

## ↑ Ancestors (13)

1. [F](../f.md)
2. [8](../../8.md)
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
