<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $G=\{e,a,b,c\}$. By [Lagrange's theorem](../../../../../lagrange-s-theorem.md), the [order of a group element](../../../../../order-of-a-group-element.md) divides four. Since no element has order four, all three nonidentity elements have order two. Thus every element is its own inverse. For any $x,y\in G$,

$$
xy=(xy)^{-1}=y^{-1}x^{-1}=yx,
$$

so the [group](../../../../../group-split.md) is [Abelian](../../../../../abelian-group.md). Also $ab$ cannot equal $e,a$ or $b$, by cancellation and the fact that $a,b$ are distinct nonidentity elements. Hence $ab=c$. The remaining products are forced, giving

$$
\boxed{\begin{array}{c|cccc}
&e&a&b&c\\\hline
e&e&a&b&c\\
a&a&e&c&b\\
b&b&c&e&a\\
c&c&b&a&e
\end{array}}
$$

The map $e\mapsto(0,0)$, $a\mapsto(1,0)$, $b\mapsto(0,1)$, $c\mapsto(1,1)$ preserves this table under componentwise addition modulo two. Therefore

$$
\boxed{G\cong C_2\times C_2=V,}
$$

the [Klein four-group](../../../../../klein-four-group.md), also called the Vierergruppe.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [9](../../9.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
