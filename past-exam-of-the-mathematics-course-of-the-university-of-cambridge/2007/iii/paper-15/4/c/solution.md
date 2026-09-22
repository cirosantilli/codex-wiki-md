<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A connected [smooth manifold](../../../../../../smooth-manifold.md) is path connected because it is locally path connected. Each connected component $C$ of the [orientation double cover](../../../../../../orientation-double-cover.md) is itself path connected. Choose a point of $C$ over $p$. For any $q\in M$, lift a path from $p$ to $q$ starting at that chosen point, using the [path lifting theorem](../../../../../../path-lifting-theorem.md). The lifted path lies in $C$ and ends above $q$. Therefore every component maps onto $M$.

Fix one fibre, containing exactly two points. Every component meets that fibre, and distinct components meet disjoint subsets of it, so **there are at most two connected components**.

If $M$ is orientable, a global continuous choice of tangent-space [orientation](../../../../../../orientation-of-a-simplex.md) $o$ gives two disjoint sheets

$$
M_+=\{(p,o_p):p\in M\},\qquad
M_-=\{(p,-o_p):p\in M\}.
$$

They are open: on a sufficiently small oriented coordinate neighborhood the global choice agrees consistently with one of the two local sheets. Each projects homeomorphically to the connected base, so these are precisely two connected components.

Conversely suppose the cover is disconnected. It has exactly two components $C_+,C_-$. Both project onto the base and each fibre contains only two points, so each component meets every fibre exactly once. The restriction $\pi:C_+\to M$ is consequently a bijective local [diffeomorphism](../../../../../../diffeomorphism.md), hence a global [diffeomorphism](../../../../../../diffeomorphism.md). Transporting the canonical [orientation](../../../../../../orientation-of-a-simplex.md) of $C_+$ through this map or, equivalently, using its smooth inverse section, gives a global [orientation](../../../../../../orientation-of-a-simplex.md) of $M$. Thus the [connectedness criterion for the orientation double cover](../../../../../../connectedness-criterion-for-the-orientation-double-cover.md) is

$$
\boxed{M\text{ is orientable}\iff\widehat M\text{ has two components}\iff\widehat M\text{ is disconnected}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
