<h1 id="6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

First distinguish the ordinary set distance from a signed overlap convention. Ordinary $d(A,B)$ is zero whenever the bodies intersect, and is never negative. Without the positive-separation assumption, test boundary intersections using the subdivision search, and test containment when the boundaries are disjoint. In particular, concentric spheres of unequal radii have positive boundary separation but overlapping enclosed bodies. Include every connected component in the containment tests.

For a meaningful negative result choose [translational penetration depth](../../../../../../translational-penetration-depth.md), with orientation fixed:

$$
\delta(A,B)=\inf\{\|t\|:\operatorname{int}(A+t)\cap\operatorname{int}B=\varnothing\}.
$$

Define signed separation as ordinary positive distance for disjoint bodies, zero at contact, and $-\delta$ when their interiors overlap. This is explicit; the source does not specify which penetration convention its word “distance” intends. Simply negating the closest-boundary distance fails when boundaries cross, because that distance is already zero despite genuine interior overlap.

One implementable extension searches translation space. Obtain an initial separating translation by moving $A$ beyond $B$ along a coordinate direction, using the bodies' enclosing boxes; its norm is an upper bound $U_t$ on $\delta$. Cover a translation box containing the radius-$U_t$ ball, subdividing it into cells. Each cell has a lower bound on $\|t\|$, given by its box distance from the origin. At a sampled translation, perform certified boundary-intersection and containment queries. A nonoverlapping sample improves $U_t$.

To discard a whole colliding cell, certify an interior witness: if $x$ lies inside $B$ and $x-t_0$ lies inside $A$ with inward clearance $r$, then every translation with $\|t-t_0\|<r$ still overlaps. Boundary-distance and inside tests establish this certificate. Conversely, a separated sample with clearance $c$ remains separated under translations of norm less than $c$ away from it, by the [triangle inequality](../../../../../../triangle-inequality.md). For a wholly free cell, use its point nearest the origin as a feasible translation, attaining its cell-norm lower bound. Refine cells whose status is uncertain and whose minimum norm is below $U_t$; discard certified-colliding cells and irrelevant farther cells. Keep the minimum cell-norm bound among cells that might contain a separating translation as $L_t$. Stop when $U_t-L_t\leq\varepsilon$, reporting

$$
\boxed{-U_t\leq d_{\rm signed}(A,B)\leq-L_t.}
$$

Refinement/inside certificates can be implemented from the same surface hierarchy with conservative geometric bounds. Exact contact may require further refinement to decide topology; at finite numerical tolerance report a contact/uncertainty interval instead of inferring overlap from intersecting boxes. This handles crossing and containment and searches for the smallest separating translation, rather than an arbitrary visible intersection depth.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
