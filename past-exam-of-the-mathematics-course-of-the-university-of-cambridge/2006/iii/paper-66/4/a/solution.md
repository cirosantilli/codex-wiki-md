<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [subdivision curve](../../../../../../subdivision-curve.md) should support [subdivision curve interrogation](../../../../../../subdivision-curve-interrogation.md) rather than merely supply successively larger [control polygons](../../../../../../control-polygon.md). Its interface should provide the parameter interval, orientation and open/closed status; endpoint and limit-point evaluation to a prescribed accuracy; and [tangent vector](../../../../../../tangent-vector.md) or derivative evaluation where defined. It should be possible to split a parameter interval, commonly at its midpoint, into equivalent restricted curve definitions while retaining all neighboring controls needed by the refinement rule.

For geometric algorithms, request a certified [bounding volume](../../../../../../bounding-volume.md) for each restricted curve, such as a [convex hull](../../../../../../convex-hull.md) or an [axis-aligned bounding box](../../../../../../axis-aligned-bounding-box.md), and the minimum and maximum of a plane's linear function over that bound. Request also a certified flatness bound: the maximum distance of the restricted limit curve from its endpoint chord, together with its spatial extent. These allow safe rejection, adaptive drawing and accuracy control. A positive, constant-reproducing [subdivision mask](../../../../../../subdivision-mask.md) often makes a control-point [convex hull](../../../../../../convex-hull.md) a valid bound. With negative mask coefficients this must be proved separately or replaced by a padded bound; it cannot simply be assumed.

Further useful enquiries include roots of a scalar function along the curve, closest-point searches, [arc length](../../../../../../arc-length.md), and inversion of an [arc-length parametrization](../../../../../../arc-length-parametrization.md). They can be implemented through evaluation, differentiation, certified bounds and recursive subdivision. **Evaluation, restriction, enclosure and error bounds are the essential primitives** needed for reliable clipping and rendering; an unqualified control-polygon approximation is insufficient.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
