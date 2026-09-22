<h1 id="6d/solution">Solution</h1>

↑ **Parent:** [6D](../6d.md)

The finite-group [Lagrange theorem](../../../../../lagrange-s-theorem.md) states that $|H|$ divides $|G|$ for every subgroup $H\leq G$, since the disjoint left cosets all have size $|H|$. In particular, the order of an element divides the group order.

If $|G|=p$ and $g\ne1$, the [cyclic subgroup](../../../../../cyclic-subgroup.md) $\langle g\rangle$ has order greater than one and dividing $p$, so it has order $p$. Therefore **every group of prime order is cyclic**.

Let $G$ now be abelian of order $p^2$. If an element has order $p^2$, it generates $G$, giving $G\cong C_{p^2}$. Otherwise every nonidentity element has order $p$. Choose $a\ne1$ and $b\notin\langle a\rangle$, which is possible because $|\langle a\rangle|=p<p^2$. Commutativity makes

$$
\Phi:C_p\times C_p\to G,\qquad (i,j)\mapsto a^ib^j
$$

a [group homomorphism](../../../../../group-homomorphism.md). If $a^ib^j=1$ and $j\ne0\pmod p$, choose $t$ with $jt\equiv1\pmod p$. Then $b=(b^j)^t\in\langle a\rangle$, a contradiction. Hence $j=0$ and then $i=0$. The homomorphism is injective and both groups have order $p^2$, so it is an isomorphism. This proves the [abelian group of prime-square order](../../../../../abelian-group-of-prime-square-order.md) classification:

$$
\boxed{G\cong C_{p^2}\quad\text{or}\quad C_p\times C_p.}
$$

Here $D_{12}$ denotes the [dihedral group](../../../../../dihedral-group.md) of order twelve, as specified in the paper: the hexagon's rotation through $\pi/3$ has order six. The possible cycle types in $A_4$ are the identity, three-cycles and double transpositions, of orders one, three and two. It has no element of order six. A [group isomorphism](../../../../../group-isomorphism.md) preserves element orders, so

$$
\boxed{D_{12}\not\cong A_4.}
$$

## ↑ Ancestors (10)

1. [6D](../6d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
