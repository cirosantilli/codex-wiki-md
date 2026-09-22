<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The corresponding [subdivision surface interrogation](../../../../../../subdivision-surface-interrogation.md) needs mesh connectivity and patch adjacency, boundary and crease flags, local coordinate charts with transition maps, and subdivision into smaller patches with their original-chart mappings. Its evaluation enquiry returns a limit point, tangent [derivatives](../../../../../../derivative.md) and a [normal vector](../../../../../../normal-vector.md); [second derivatives](../../../../../../second-derivative.md) are supplied only where the limit is sufficiently smooth. Certified [bounding volumes](../../../../../../bounding-volume.md) and patch approximation errors allow a hierarchy for intersection and proximity searches. Boundary-curve enquiries complete the interface for clipping.

On regular parts of a [subdivision surface](../../../../../../subdivision-surface.md), these evaluations may use its equivalent tensor-product or [box spline](../../../../../../box-spline.md) patch. Near an [extraordinary subdivision vertex](../../../../../../extraordinary-subdivision-vertex.md), the local [subdivision matrix](../../../../../../subdivision-matrix.md) determines the limit position through its constant [left eigenvector](../../../../../../left-eigenvector.md), and its tangent modes determine the [normal vector](../../../../../../normal-vector.md) under the scheme's [characteristic map of a subdivision surface](../../../../../../characteristic-map-of-a-subdivision-surface.md) regularity conditions. Refinement alone does not establish those conditions. A [subdivision surface](../../../../../../subdivision-surface.md) may have a well-defined [tangent plane](../../../../../../tangent-plane.md) there without possessing [second derivatives](../../../../../../second-derivative.md) or [Gaussian curvature](../../../../../../gaussian-curvature.md). An interrogation interface must distinguish these cases and can work on surrounding regular charts when a higher [derivative](../../../../../../derivative.md) is unavailable at the vertex itself.

Together, subdivision, bounds, topology and limit evaluation support ray–[subdivision surface](../../../../../../subdivision-surface.md) intersection: bounds eliminate irrelevant patches; surviving patches are refined, and regular candidate intersections are corrected using position and first [derivatives](../../../../../../derivative.md). The returned intersection is a point of the limit [subdivision surface](../../../../../../subdivision-surface.md) with an error certificate, rather than automatically a point on the last control mesh.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
