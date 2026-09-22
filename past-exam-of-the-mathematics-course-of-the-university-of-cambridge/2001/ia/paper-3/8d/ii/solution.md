<h1 id="8d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [direct product of groups](../../../../../../direct-product-of-groups.md) uses componentwise multiplication:

$$
(g,h)(g',h')=(gg',hh'),\qquad e=(e_G,e_H),\qquad
(g,h)^{-1}=(g^{-1},h^{-1}).
$$

Associativity follows in each factor. The maps $g\mapsto(g,e_H)$ and $h\mapsto(e_G,h)$ are injective [group homomorphisms](../../../../../../group-homomorphism.md) onto [subgroups](../../../../../../subgroup.md), giving the required copies of $G$ and $H$.

Use the PDF's convention that the subscript in $D_n$ is the [group](../../../../../../group-split.md) order. Write the hexagon [group](../../../../../../group-split.md) as $D_{12}=\langle r,s\mid r^6=s^2=e,\ srs=r^{-1}\rangle$ and the triangle [group](../../../../../../group-split.md) as $D_6=\langle a,b\mid a^3=b^2=e,\ bab=a^{-1}\rangle$. Let $z$ generate $C_2$. In $D_{12}$, $r^2$ has order three and $s$ conjugates it to its inverse, so $\langle r^2,s\rangle$ is a copy of $D_6$. The element $r^3$ has order two and is central, since $sr^3s=r^{-3}=r^3$.

Define

$$
\Phi(a^ib^j,z^k)=r^{2i+3k}s^j,
\qquad 0\le i<3,\quad 0\le j,k<2.
$$

The generator relations are preserved and $r^3$ commutes with the other images, so $\Phi$ is a [group homomorphism](../../../../../../group-homomorphism.md) from the direct product. The six residues $2i+3k$ are distinct modulo six: reduction modulo two first determines $k$, then reduction modulo three determines $i$. Together with $j$, they give all twelve distinct normal forms $r^ms^j$ in $D_{12}$. Thus $\Phi$ is bijective and

$$
\boxed{D_{12}\cong D_6\times C_2.}
$$

This is the [dihedral splitting when the half-rotation order is odd](../../../../../../dihedral-splitting-when-the-half-rotation-order-is-odd.md) with half-rotation order three.

Finally, $D_{12}$ contains an element of order six, namely $r$. The even cycle types on four symbols are the identity, a 3-cycle, and two disjoint transpositions; their orders are respectively one, three and two. Therefore $A_4$ has no element of order six. Since a [group isomorphism](../../../../../../group-isomorphism.md) preserves element orders,

$$
\boxed{D_{12}\not\cong A_4.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [8D](../../8d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
