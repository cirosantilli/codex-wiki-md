<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Interpret the positive-distance assumption as disjoint compact enclosed bodies $A,B$, certified for example by disjoint enclosing volumes. Merely having disjoint drawn control meshes is insufficient if one encloses the other or the meshes do not enclose their limit surfaces. For genuinely disjoint bodies, the closest pair lies on their boundaries: an interior point could move toward the other body and decrease the distance. Thus minimize over all pairs of limit-surface patches.

Use [branch and bound](../../../../../../branch-and-bound.md) on patch pairs. For regions $A_i,B_j$, enclosing [bounding volumes](../../../../../../bounding-volume.md) give a lower bound $L_{ij}$ on their true minimum distance. For [axis-aligned bounding boxes](../../../../../../axis-aligned-bounding-box.md), compute this directly as

$$
L_{ij}=\sqrt{\sum_{k=1}^3\max(0,a_k^- -b_k^+,b_k^- -a_k^+)^2}.
$$

Any pair of evaluated limit points provides a feasible upper bound; retain the smallest, $U$. Start with a covering list of all coarse patch pairs. At each step, discard a pair when its lower bound is at least $U$, otherwise refine the region with larger bounding diameter/error and enqueue its child pairs. Prefer the pair with smallest lower bound. Update $U$ with new feasible pairs; a local stationary-distance solve can improve it but cannot replace the global search.

Let $L_*$ be the minimum remaining lower bound, capped by $U$ if the list is empty. The current certificate is

$$
\boxed{L_*\leq d(A,B)\leq U.}
$$

Stop when $U-L_*\leq\varepsilon$. Compactness and shrinking valid patch enclosures ensure convergence to this tolerance under the interface assumptions. An equivalent mesh method must add each mesh's certified limit error; for [Hausdorff distance](../../../../../../hausdorff-distance.md) errors $e_A,e_B$, the separation error is at most $e_A+e_B$. Finite mesh distance without such a bound is not the exact [minimum distance between subdivision bodies](../../../../../../minimum-distance-between-subdivision-bodies.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
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
