<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The complete classification up to [group isomorphism](../../../../../../group-isomorphism.md) is

$$
\boxed{\begin{array}{c|l}
|G|&G\\\hline
1&C_1\\
2&C_2\\
3&C_3\\
4&C_4,\ C_2\times C_2\\
5&C_5\\
6&C_6,\ S_3
\end{array}}
$$

Here $C_1$ is the [trivial group](../../../../../../trivial-group.md). The [prime number](../../../../../../prime-number-split.md) cases follow from [i](../a/i.md). For four elements, an element of [order of a group element](../../../../../../order-of-a-group-element.md) four generates $C_4$. If there is none, [Lagrange's theorem](../../../../../../lagrange-s-theorem.md) makes every nonidentity element have [order of a group element](../../../../../../order-of-a-group-element.md) two. Then [iv](../a/iv.md) produces a four-element [subgroup](../../../../../../subgroup.md), which must be all of $G$, giving the [Klein four-group](../../../../../../klein-four-group.md).

For six elements, an element of [order of a group element](../../../../../../order-of-a-group-element.md) six gives $C_6$. Suppose there is none. If there were no element of [order of a group element](../../../../../../order-of-a-group-element.md) three either, all nonidentity elements would have [order of a group element](../../../../../../order-of-a-group-element.md) two. Part [iv](../a/iv.md) would then produce a [subgroup](../../../../../../subgroup.md) of [cardinality](../../../../../../cardinality.md) four, contradicting [Lagrange's theorem](../../../../../../lagrange-s-theorem.md). Thus choose $a$ of [order of a group element](../../../../../../order-of-a-group-element.md) three. There is also an [involution](../../../../../../involution.md) $b$: otherwise the five nonidentity elements could be paired into distinct pairs $\{g,g^{-1}\}$, impossible for an odd number of elements.

The [subgroup](../../../../../../subgroup.md) $H=\langle a\rangle$ has [index of a subgroup](../../../../../../index-of-a-subgroup.md) two, so it is a [normal subgroup](../../../../../../normal-subgroup.md). Indeed, for $g\notin H$, both $gH$ and $Hg$ are the complement of $H$, and for $g\in H$ both equal $H$. Consequently $bab^{-1}$ is either $a$ or $a^{-1}$. The first possibility makes $a,b$ commute, and $ab$ then has [order of a group element](../../../../../../order-of-a-group-element.md) six: $(ab)^k=e$ forces $a^k=b^{-k}\in\langle a\rangle\cap\langle b\rangle=\{e\}$, so both $3$ and $2$ divide $k$. This contradicts our assumption. Therefore

$$
bab^{-1}=a^{-1}.
$$

Every element is uniquely $a^i$ or $a^ib$, with $0\leq i<3$, and the relation $ba=a^{-1}b$ determines all their products. Sending $a$ to $(123)$ and $b$ to $(12)$ gives a [group isomorphism](../../../../../../group-isomorphism.md) with the [symmetric group](../../../../../../symmetric-group.md) $S_3$. This completes the classification of [groups of order at most six](../../../../../../groups-of-order-at-most-six.md).

Of these [groups](../../../../../../group-split.md), **exactly $C_1,C_2,C_3,C_4,C_2\times C_2,S_3$ embed in $S_4$**. Concrete [subgroups](../../../../../../subgroup.md) are

$$
\{e\},\quad\langle(12)\rangle,\quad\langle(123)\rangle,\quad
\langle(1234)\rangle,\quad
\{e,(12)(34),(13)(24),(14)(23)\},\quad
\{\sigma\in S_4:\sigma(4)=4\}.
$$

There is no $C_5$ [subgroup](../../../../../../subgroup.md), since $5$ does not divide $24$. There is no $C_6$ [subgroup](../../../../../../subgroup.md) either: the [order of a group element](../../../../../../order-of-a-group-element.md) in a [symmetric group](../../../../../../symmetric-group.md) is the [least common multiple](../../../../../../least-common-multiple.md) of the lengths in its [disjoint cycle decomposition](../../../../../../disjoint-cycle-decomposition.md), and on four letters the only possibilities are $1,2,3,4$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Mathematics I](../../../mathematics-i-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
