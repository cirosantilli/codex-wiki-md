<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $r=g_1$ and $s=g_2$. Direct [matrix multiplication](../../../../matrix-multiplication.md) gives

$$
r^3=s^2=I,\qquad srs=r^{-1}.
$$

Moving every $s$ to the right shows that every word in these [generators of a group](../../../../generator-of-a-group.md) has the form $r^a s^b$, with $a\in\{0,1,2\}$ and $b\in\{0,1\}$. The three $r^a$ are distinct diagonal [matrices](../../../../matrix.md), and the three $r^as$ are distinct off-diagonal [matrices](../../../../matrix.md). Hence

$$
\boxed{G=\{I,r,r^2,s,rs,r^2s\},\qquad |G|=6.}
$$

Since $srs=r^2\ne r$, this is a [non-abelian group](../../../../non-abelian-group.md). Its [group presentation](../../../../group-presentation.md) identifies it with the [dihedral group](../../../../dihedral-group.md) of an equilateral triangle, equivalently the [symmetric group](../../../../symmetric-group.md) $S_3$.

The [conjugacy classes](../../../../conjugacy-class.md) are

$$
\boxed{\{I\},\qquad \{r,r^2\},\qquad \{s,rs,r^2s\}.}
$$

Indeed $s$ interchanges $r$ and $r^2$ by [conjugation](../../../../conjugation.md), while $r^a s r^{-a}=r^{2a}s$ runs through all three reflections. No reflection is conjugate to a rotation, since [conjugation](../../../../conjugation.md) preserves [order of a group element](../../../../order-of-a-group-element.md).

There are three inequivalent complex [irreducible representations](../../../../irreducible-representation.md), one for each [conjugacy class](../../../../conjugacy-class.md). The [sum of squares of irreducible representation dimensions](../../../../sum-of-squares-of-irreducible-representation-dimensions.md) gives $d_1^2+d_2^2+d_3^2=6$. One [representation](../../../../group-representation.md) is trivial, and the only possible positive integer dimensions are

$$
\boxed{d_1,d_2,d_3=1,1,2.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
