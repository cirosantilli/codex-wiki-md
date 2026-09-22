<h1 id="5e/solution">Solution</h1>

↑ **Parent:** [5E](../5e.md)

Restrict the quotient projection $\pi:G\to G/N$ to $H$. This is a [group homomorphism](../../../../../group-homomorphism.md) with

$$
\ker(\pi|_H)=H\cap N.
$$

Its image is a nontrivial [subgroup](../../../../../subgroup.md) of the prime-order [quotient group](../../../../../quotient-group.md), because $H$ is not contained in $N$. By [Lagrange's theorem for finite groups](../../../../../lagrange-s-theorem.md), the image has order $p$ and is all of $G/N$. The [first isomorphism theorem for groups](../../../../../first-isomorphism-theorem.md) therefore gives

$$
\boxed{H\cap N\trianglelefteq H,\qquad [H:H\cap N]=p.}
$$

For the second assertion, partition $C$ into [conjugacy classes](../../../../../conjugacy-class.md) for $N$. Because $N$ is normal, [conjugation](../../../../../conjugation.md) by $G$ permutes these smaller classes: $g\operatorname{Cl}_N(x)g^{-1}=\operatorname{Cl}_N(gxg^{-1})$. This [group action](../../../../../group-action.md) is transitive since any two elements of $C$ are conjugate in $G$. Elements of $N$ fix every $N$-class, so the action factors through $G/N$.

If $m$ is the number of smaller classes, the [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md) for this transitive action gives $m\mid |G/N|=p$. Thus

$$
\boxed{C\text{ is one }N\text{-class, or a disjoint union of }p\text{ such classes}.}
$$

Distinct [conjugacy classes](../../../../../conjugacy-class.md) are disjoint because they are [orbits of a group action](../../../../../orbit-of-a-group-action.md). This proves [conjugacy class splitting in a prime-index normal subgroup](../../../../../conjugacy-class-splitting-in-a-prime-index-normal-subgroup.md) without assuming all $G$-conjugations are already conjugations by $N$.

## ↑ Ancestors (10)

1. [5E](../5e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
