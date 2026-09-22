<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

Let $H_k$ be the open hyperbolic half-plane beyond $\gamma_k$, opposite the central region $U$. These three half-planes have disjoint closures in the disk, and [hyperbolic reflection](../../../../../hyperbolic-reflection.md) $J_k$ exchanges $H_k$ and its complementary half-plane. In particular $J_k(U^\circ)\subset H_k$ and $J_i(H_j)\subset H_i$ when $i\ne j$. A reduced nonempty reflection word therefore sends an interior point of $U$ into the half-plane corresponding to its first letter. It cannot be the identity. This [ping-pong lemma](../../../../../ping-pong-lemma.md) argument proves that the reflection [group](../../../../../group-split.md) is

$$
W=\langle J_1,J_2,J_3\mid J_1^2=J_2^2=J_3^2=1\rangle
\cong C_2*C_2*C_2.
$$

The usual reflection tiling makes $U$ a [fundamental domain](../../../../../fundamental-domain.md) for $W$: successive reflection across an offending side reduces a point to $U$, and the disjoint-side configuration yields locally finite tiles. Equivalently this is the disjoint-geodesic case of the reflection fundamental-domain theorem; there are no vertex relations because the sides never meet.

The orientation-preserving subgroup consists of even words. Every pair $J_iJ_j$ can be expressed in $A=J_2J_1$ and $B=J_3J_2$: the other nontrivial pairs are their inverses and $J_3J_1=BA$, $J_1J_3=A^{-1}B^{-1}$. Thus it is exactly $G$. A fundamental set is **$U\cup J_2U$, with one representative chosen on each paired side**; its interior is a [fundamental domain](../../../../../fundamental-domain.md). To see there are no relations between $A,B$, the reflection-word tree has vertices the reduced words and edges joining $w$ to $wJ_i$. The even subgroup acts freely on this tree; its quotient has two vertices joined by three edges. Choosing the $J_2$ edge as a spanning tree leaves two independent loops, represented by $A$ and $B$. Reduced loops in a [graph](../../../../../graph-split.md) form a [free group](../../../../../free-group.md), so

$$
\boxed{G\cong F_2\text{ freely on }A,B.}
$$

The quotient is the double of the central three-sided region along its geodesic sides: **an orientable pair of pants, topologically a [sphere](../../../../../sphere.md) with three points removed**. Its three ends are hyperbolic funnels, not cusps, because the sides are ultraparallel and the peripheral transformations have positive translation lengths. The compact convex core has three geodesic boundary circles; the complete quotient itself has no boundary.

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
