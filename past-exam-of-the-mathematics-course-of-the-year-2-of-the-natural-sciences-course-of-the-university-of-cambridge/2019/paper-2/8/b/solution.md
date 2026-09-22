<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

By [Lagrange's theorem](../../../../../lagrange-s-theorem.md), the possible values of the [order of a group element](../../../../../order-of-a-group-element.md) are

$$
\boxed{1,2,4,8}.
$$

These are possibilities across groups of order eight; they need not all occur in one group.

If every element has order at most two, every element equals its own inverse. Thus for any $x,y$,

$$
xy=(xy)^{-1}=y^{-1}x^{-1}=yx,
$$

so $G$ is an [abelian group](../../../../../abelian-group.md). Choose $a\ne e$, and then $b\notin\langle a\rangle$. The four elements $e,a,b,ab$ are distinct and form a [subgroup](../../../../../subgroup.md) $H$: commutativity and $a^2=b^2=e$ prove closure and inverses. Choose $c\notin H$. The elements of $H$ and $Hc$ are disjoint, since $hc\in H$ would imply $c\in H$. These two four-element sets therefore exhaust $G$.

Every element consequently has a unique expression $a^ib^jc^k$, with $i,j,k\in\{0,1\}$. The map from triples to these products is bijective and respects multiplication by addition of exponents modulo two. Hence

$$
\boxed{G\cong C_2\times C_2\times C_2},
$$

a [direct product of groups](../../../../../direct-product-of-groups.md) and an [elementary abelian group](../../../../../elementary-abelian-group.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [8](../../8.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
