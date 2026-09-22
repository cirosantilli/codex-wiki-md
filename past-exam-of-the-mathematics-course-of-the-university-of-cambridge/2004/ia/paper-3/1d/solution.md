<h1 id="1d/solution">Solution</h1>

↑ **Parent:** [1D](../1d.md)

For a [subgroup](../../../../../subgroup.md) $H$ of a finite [group](../../../../../group-split.md) $G$, [Lagrange's theorem](../../../../../lagrange-s-theorem.md) states $|G|=[G:H]|H|$. Thus a subgroup's order, and in particular the [order of a group element](../../../../../order-of-a-group-element.md), divides $|G|$.

For $|G|=10$, if every element had order one or two, the [order of a finite group of exponent two](../../../../../order-of-a-finite-group-of-exponent-two.md) would make $|G|$ a power of two, a contradiction. Hence an element has order five or ten. In the latter case **$G$ is the cyclic group $C_{10}$**. Otherwise choose $a$ of order five. Its [cyclic subgroup](../../../../../cyclic-subgroup.md) $H=\langle a\rangle$ has index two and is therefore a [normal subgroup](../../../../../normal-subgroup.md).

In the noncyclic case an element $b$ outside $H$ has order two: its order divides ten, it cannot have order ten, and an element of order five has trivial image in the order-two [quotient group](../../../../../quotient-group.md) $G/H$. Every element of $G$ is then $a^j$ or $a^jb$. [Conjugation](../../../../../conjugation.md) by $b$ restricts to an [automorphism](../../../../../automorphism.md) of $H$, say $bab^{-1}=a^r$. Since $b^2=1$, $r^2\equiv1\pmod5$, so $r=1$ or $-1$ modulo five.

For $r=1$, the generators commute and $ab$ has order ten, yielding the cyclic case. For $r=-1$, these are the relations of the [dihedral group](../../../../../dihedral-group.md) of the pentagon. The [classification of groups of order ten](../../../../../classification-of-groups-of-order-ten.md) is therefore **exactly $C_{10}$ and $D_{10}$**, where the subscript on $D_{10}$ denotes its order. They are not [isomorphic](../../../../../isomorphism.md) because one is [Abelian](../../../../../abelian-group.md) and the other is not.

## ↑ Ancestors (10)

1. [1D](../1d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
