<h1 id="8d/solution">Solution</h1>

↑ **Parent:** [8D](../8d.md)

For a nontrivial [finite p-group](../../../../../finite-p-group.md) $G$ of order $p^m$ with $m\ge1$, partition into [conjugacy classes](../../../../../conjugacy-class.md). A noncentral class has size $[G:C_G(x)]$, a positive power of $p$ larger than one by [Lagrange's theorem](../../../../../lagrange-s-theorem.md). The [class equation](../../../../../class-equation.md) therefore says

$$
|G|=|Z(G)|+\sum_{\text{noncentral classes}}[G:C_G(x)],\qquad |Z(G)|\equiv0\pmod p.
$$

The [center of a group](../../../../../center-of-a-group.md) contains the identity, so **$|Z(G)|\ge p$**, proving its nontriviality. The positive-exponent qualification matters: the one-element [group](../../../../../group-split.md) has no nonidentity central element.

If $|G|=p^2$, its [center of a group](../../../../../center-of-a-group.md) has order $p$ or $p^2$. In the first case, the [quotient group](../../../../../quotient-group.md) $G/Z(G)$ has prime order and is cyclic. Whenever a central [quotient group](../../../../../quotient-group.md) is cyclic, writing all elements as $g^iz$ with $z$ central shows that they commute: $(g^iz)(g^jw)=g^{i+j}zw=(g^jw)(g^iz)$. Thus that case would already make $G$ [Abelian](../../../../../abelian-group.md) and its [center of a group](../../../../../center-of-a-group.md) all of $G$, a contradiction. Hence **every [group](../../../../../group-split.md) of order $p^2$ is [Abelian](../../../../../abelian-group.md)**.

If there is an element of order $p^2$, it is a [generator of a group](../../../../../generator-of-a-group.md) for $G$, giving $C_{p^2}$. Otherwise every nonidentity element has order $p$. Pick $a\ne1$ and $b\notin\langle a\rangle$. Their [cyclic subgroups](../../../../../cyclic-subgroup.md) have trivial intersection, and they commute; the $p^2$ distinct products $a^ib^j$ exhaust $G$. Hence the [classification of groups of order p squared](../../../../../classification-of-groups-of-order-p-squared.md) is

$$
\boxed{G\cong C_{p^2}\quad\text{or}\quad G\cong C_p\times C_p.}
$$

Both [groups](../../../../../group-split.md) exist and are nonisomorphic, since only the first has an element of order $p^2$.

## ↑ Ancestors (10)

1. [8D](../8d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
