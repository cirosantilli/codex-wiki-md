<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The core [parametric surface interrogation](../../../../../../parametric-surface-interrogation.md) is evaluation of the position and its [derivatives](../../../../../../derivative.md) through second order:

$$
\boxed{S(u,v),\quad S_u,S_v,\quad S_{uu},S_{uv},S_{vv}.}
$$

Position answers point queries; first [derivatives](../../../../../../derivative.md) give the [differential](../../../../../../differential-of-a-smooth-map.md), tangent directions and [normal vector](../../../../../../normal-vector.md); [second derivatives](../../../../../../second-derivative.md) supply [curvature](../../../../../../curvature.md). An evaluator should also report the parameter domain, patch adjacency, boundary curves and knot or crease locations, and whether these [derivatives](../../../../../../derivative.md) exist at the queried point. At a discontinuity boundary it should provide the relevant [one-sided limits](../../../../../../one-sided-limit.md) rather than silently average them.

For spatial searches, provide restriction or subdivision into equivalent smaller patches and certified [bounding volumes](../../../../../../bounding-volume.md), with error estimates when an approximate mesh is used. These allow intersection and closest-point algorithms to reject remote patches and refine the remaining candidates. A useful interface therefore combines [differential](../../../../../../differential-of-a-smooth-map.md) evaluation with domain/topology and enclosure information. Inverse parameter lookup, ray intersection and nearest-point search can be built from these primitives using subdivision and local root or minimization solves; they need not be presumed exact basic evaluations of every representation.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
