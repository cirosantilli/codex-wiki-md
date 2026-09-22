<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

A [group](../../../../group-split.md) is a nonempty [set](../../../../set-split.md) with a closed [binary operation](../../../../binary-operation.md) that is [associative](../../../../associative-property.md), has an [identity element](../../../../identity-element.md), and gives every element an [inverse element](../../../../inverse-element.md). A [subgroup](../../../../subgroup.md) is a subset that is itself a [group](../../../../group-split.md) under the inherited operation. The left [coset](../../../../coset.md) of $H$ represented by $g$ is $gH=\{gh:h\in H\}$; right [cosets](../../../../coset.md) are defined analogously. Left [cosets](../../../../coset.md) partition a finite [group](../../../../group-split.md), and $h\mapsto gh$ is a [bijection](../../../../bijection.md) from $H$ to $gH$. Therefore $|G|=[G:H]|H|$, proving [Lagrange's theorem](../../../../lagrange-s-theorem.md) and the required divisibility.

For the given [matrices](../../../../matrix.md), put $a=A$ and $c=AB=iI$. Since $B=iA$, the generators commute; $a^2=I$, $c^4=I$, and the generated elements are

$$
G=\{I,c,c^2,c^3,a,ca,c^2a,c^3a\},\qquad B=ca.
$$

They are distinct, and $(c^ra^s)(c^{r'}a^{s'})=c^{r+r'}a^{s+s'}$, with exponents reduced modulo four and two. The [Cayley table](../../../../cayley-table.md) is

$$
\begin{array}{c|cccccccc}
&I&c&c^2&c^3&a&ca&c^2a&c^3a\\\hline
I&I&c&c^2&c^3&a&ca&c^2a&c^3a\\
c&c&c^2&c^3&I&ca&c^2a&c^3a&a\\
c^2&c^2&c^3&I&c&c^2a&c^3a&a&ca\\
c^3&c^3&I&c&c^2&c^3a&a&ca&c^2a\\
a&a&ca&c^2a&c^3a&I&c&c^2&c^3\\
ca&ca&c^2a&c^3a&a&c&c^2&c^3&I\\
c^2a&c^2a&c^3a&a&ca&c^2&c^3&I&c\\
c^3a&c^3a&a&ca&c^2a&c^3&I&c&c^2\\
\end{array}
$$

The table proves closure and identifies $I$ as the identity. The [inverse element](../../../../inverse-element.md) of $c^ra^s$ is $c^{-r}a^s$, and [associativity](../../../../associative-property.md) follows from [matrix multiplication](../../../../matrix-multiplication.md). Thus this is the [direct product of cyclic groups of orders four and two](../../../../direct-product-of-cyclic-groups-of-orders-four-and-two.md), an [abelian group](../../../../abelian-group.md) of order eight.

Its [subgroups](../../../../subgroup.md) are exactly

$$
\{I\},\quad\{I,c^2\},\quad\{I,a\},\quad\{I,c^2a\},
$$



$$
\{I,c,c^2,c^3\},\quad\{I,ca,c^2,c^3a\},\quad\{I,c^2,a,c^2a\},\quad G.
$$

To see the list is complete, [Lagrange's theorem](../../../../lagrange-s-theorem.md) leaves orders one, two, four and eight. There are exactly three elements of order two, giving the three order-two [subgroups](../../../../subgroup.md). An order-four [subgroup](../../../../subgroup.md) containing an element of order four must be one of the two [cyclic groups](../../../../cyclic-group.md) displayed; without such an element it must be the four-element set of elements whose squares are $I$. This is the enumeration in [subgroups of C4 times C2](../../../../subgroups-of-c4-times-c2.md).

For example choose $H=\{I,c,c^2,c^3\}$. A complete set of [cosets](../../../../coset.md) is $\boxed{H,\qquad aH=\{a,ca,c^2a,c^3a\}}$. Since $G$ is [Abelian](../../../../abelian-group.md), the left and right [cosets](../../../../coset.md) coincide.

## ↑ Ancestors (12)

1. [8](../8.md)
2. [Paper 2](../../paper-2-split.md)
3. [2003](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
