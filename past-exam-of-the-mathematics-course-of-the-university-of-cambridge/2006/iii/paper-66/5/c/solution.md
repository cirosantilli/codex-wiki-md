<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In a regular region, moving one [control point](../../../../../../control-point.md) adds its displacement multiplied by a translate of the [twice-smoothed four-direction box spline](../../../../../../twice-smoothed-four-direction-box-spline.md). Measure parameter distances in original grid-edge units, with the affected [control point](../../../../../../control-point.md) at the origin. The convex hull of the binary mask offsets is

$$
Z=[-1,1](1,0)+[-1,1](0,1)+[-1,1](1,1)+[-1,1](1,-1).
$$

After successive binary refinements the physical displacements are scaled by $2^{-1},2^{-2},\ldots$. Their possible accumulated offsets therefore form $\sum_{j\geq1}2^{-j}Z=Z$. The [box spline](../../../../../../box-spline.md) description confirms that this [zonotope](../../../../../../zonotope.md) is the actual support, not merely a loose enclosure. Equivalently,

$$
\boxed{Z=\{(u,v): |u|\leq3,\ |v|\leq3,\ |u|+|v|\leq4\}}.
$$

It is an octagon with vertices $(3,1),(1,3),(-1,3),(-3,1),(-3,-1),(-1,-3),(1,-3),(3,-1)$. Its enclosing square is six original grid intervals wide in each direction. Cutting four right triangles of area two from this $6\times6$ square gives area $36-8=28$ parameter-square units. Outside this octagon the control-point displacement has no effect; its closure is the support, although the basis function can vanish on its boundary.

**The regular influence footprint is this width-six, area-28 parameter octagon.** For a nonplanar control mesh, the affected part of the spatial surface is the image of the octagon, not necessarily a planar octagon of the same metric size. Near an [extraordinary subdivision vertex](../../../../../../extraordinary-subdivision-vertex.md), use the actual refinement neighborhood instead of assuming a globally regular lattice footprint.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
