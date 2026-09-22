<h1 id="6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [subdivision surface interrogation](../../../../../../subdivision-surface-interrogation.md) interface needs the initial [control net](../../../../../../control-net.md), its face/edge/vertex connectivity, the subdivision rule, patch addressing and refinement into child regions that cover the same limit surface. It must supply limit-point evaluation, available tangent/normal data and smoothness information, including the treatment of [extraordinary subdivision vertices](../../../../../../extraordinary-subdivision-vertex.md). A finite refined mesh point is generally not the exact limit point.

For geometric search it must provide certified [bounding volumes](../../../../../../bounding-volume.md) for each descendant region, bounds that shrink under refinement, and a mesh-to-limit or chord/patch error estimate. With positive convex subdivision masks the active-control [convex hull](../../../../../../convex-hull.md) can provide such an enclosure; schemes with negative coefficients need another valid bound. A closed surface also needs consistent orientation, component navigation and containment queries for the enclosed body. The $C^1$ hypothesis supplies first-order tangent information at regular points, not automatically second derivatives or curvature everywhere. These enquiries distinguish an accurate limit-surface algorithm from a calculation only on an approximate control polyhedron.

## ↑ Ancestors (11)

1. [I](../i.md)
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
