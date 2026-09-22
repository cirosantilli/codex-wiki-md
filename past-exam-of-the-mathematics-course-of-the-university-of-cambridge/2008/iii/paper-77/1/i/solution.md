<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let the [triangles](../../../../../../triangle.md) have vertices $A_0,A_1,A_2$ and $B_0,B_1,B_2$. Work initially with nonzero-area [triangles](../../../../../../triangle.md). A [triangle-triangle intersection algorithm](../../../../../../triangle-triangle-intersection-algorithm.md) begins with the unnormalized [normal vector](../../../../../../normal-vector.md) $N_A=(A_1-A_0)\times(A_2-A_0)$ and the three signed plane evaluations $d_j=N_A\cdot(B_j-A_0)$. If all $d_j$ are strictly positive, or all strictly negative, the second [triangle](../../../../../../triangle.md) lies strictly on one side of the first one's plane, so the [triangles](../../../../../../triangle.md) are disjoint. Otherwise compute $N_B$ and $e_i=N_B\cdot(A_i-B_0)$ and apply the symmetric rejection test. Strict inequalities are important: contact on a vertex or edge counts as intersection.

If the planes are not parallel, put $L=N_A\times N_B$. Each [triangle](../../../../../../triangle.md) meets the other one's plane in an empty set, a point or a [line segment](../../../../../../line-segment.md). Its endpoints are obtained from zero-valued vertices and the edges whose endpoint plane evaluations have opposite signs. For example, an edge $B_jB_k$ contributes

$$
X=B_j+\frac{d_j}{d_j-d_k}(B_k-B_j).
$$

All these points lie on the common line of the two planes. Choose a coordinate $r$ for which $L_r\ne0$ and form the coordinate intervals $I_A=[a_-,a_+]$, $I_B=[b_-,b_+]$ of the two slices. This coordinate is one-to-one along the common line, so the exact final test is

$$
\boxed{\max(a_-,b_-)\le\min(a_+,b_+).}
$$

Only that coordinate of each slice endpoint needs to be evaluated; no full three-dimensional line parameterization is necessary.

Parallel planes which have survived the strict plane tests are coplanar. Drop the coordinate corresponding to the largest component of $N_A$ and test the two projected planar [triangles](../../../../../../triangle.md). For each edge of either projected [triangle](../../../../../../triangle.md), project both vertex sets onto the perpendicular direction. A strictly disjoint pair of projection intervals certifies separation. If none of the six edge directions separates them, the planar [convex sets](../../../../../../convex-set.md) overlap: a separating line for two disjoint convex polygons can be chosen parallel to an edge of one of them. This includes containment and boundary contact.

A zero [normal vector](../../../../../../normal-vector.md) signifies a degenerate [triangle](../../../../../../triangle.md); reduce its [convex hull](../../../../../../convex-hull.md) to a point or its extreme [line segment](../../../../../../line-segment.md) and use point containment or segment intersection instead. For floating-point input, reliable sign predicates and scale-aware error bounds are preferable to treating a tiny signed distance as an arbitrary exact zero. **Plane rejection followed by interval overlap, with a planar test for coplanar input, determines all nondegenerate cases.**

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
