# Bounding volume

↑ **Parent:** [Computer aided geometric design](computer-aided-geometric-design.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bounding_volume)

A [bounding volume](bounding-volume.md) is a simple enclosing [set](set-split.md) $B$ for an object $S$: every [point](point-geometry.md) of $S$ belongs to $B$. Its purpose is to make a cheap rejection possible before examining the object itself. For example, an [axis-aligned bounding box](axis-aligned-bounding-box.md) can enclose a [triangle](triangle.md) using just its smallest and largest [coordinates](coordinate-linear-algebra.md).

The guarantee is one-sided. If $S\subseteq B_S$ and $T\subseteq B_T$, then

$$
S\cap T\ne\varnothing\ \Longrightarrow\ B_S\cap B_T\ne\varnothing.
$$

Thus an empty [set intersection](set-intersection.md) of the [bounding volumes](bounding-volume.md) certifies an empty [set intersection](set-intersection.md) of the objects. An overlap of the [bounding volumes](bounding-volume.md) is necessary for actual intersection, but does not prove it. This is a [conservative enclosure test](conservative-enclosure-test.md): rejection is conclusive, acceptance means further examination is needed.

Consider the filled [triangles](triangle.md) $A$ with [vertices of a polygon](vertex-of-a-polygon.md) $(0,0),(2,0),(0,2)$ and $B$ with [vertices of a polygon](vertex-of-a-polygon.md) $(3/2,3/2),(7/2,3/2),(7/2,7/2)$. Their [axis-aligned bounding boxes](axis-aligned-bounding-box.md) overlap in $[3/2,2]\times[3/2,2]$. Nevertheless, every [point](point-geometry.md) of $A$ satisfies $x+y\leq2$, whereas every [point](point-geometry.md) of $B$ satisfies $x+y\geq3$. The two [triangles](triangle.md) are disjoint. The shaded square in the [bounding volume hierarchy](bounding-volume-hierarchy.md) illustration makes this false candidate visible.

For [collision detection](collision-detection.md), a [broad phase](broad-phase.md) produces possible object pairs from [bounding volume](bounding-volume.md) tests; a [narrow phase](narrow-phase.md) examines the actual shapes, for example with a [triangle-triangle intersection algorithm](triangle-triangle-intersection-algorithm.md). Scott Le Grand's [Chapter 32. Broad-Phase Collision Detection with CUDA](gpu-gems-3/chapter-32-broad-phase-collision-detection-with-cuda.md) explains this separation in its opening paragraphs. Whether touching counts as a [collision](collision.md) must be specified by the application.

An enclosure must cover the entire object being queried. A box fitted to samples of a [parametric curve](parametric-curve.md) only guarantees enclosure of the sampled [points](point-geometry.md), unless a separate bound covers the whole [parametric curve](parametric-curve.md). For a [Bézier curve](bezier-curve.md), the [convex hull](convex-hull.md) of its [control points](control-point.md) provides such a bound on its defining parameter [interval](interval-mathematics.md). In [floating-point arithmetic](floating-point-arithmetic.md), [outward rounding](outward-rounding.md) can preserve certified [coordinate](coordinate-linear-algebra.md) bounds; an inward [roundoff error](round-off-error.md) can invalidate a rejection. Bounds must also be updated when objects move.

**Table of contents**

- [Conservative enclosure test](conservative-enclosure-test.md)
- [Collision detection](collision-detection.md)
  - [Broad phase](broad-phase.md)
  - [Narrow phase](narrow-phase.md)
- [Bounding volume hierarchy](bounding-volume-hierarchy.md)
  - [Bounding volume hierarchy traversal](bounding-volume-hierarchy-traversal.md)
- [Axis-aligned bounding box](axis-aligned-bounding-box.md)

## ↑ Ancestors (6)

1. [Computer aided geometric design](computer-aided-geometric-design.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (26)

- [Bounding volume](bounding-volume.md)
- [Bounding volume hierarchy](bounding-volume-hierarchy.md)
- [Closest-point search on a subdivision curve](closest-point-search-on-a-subdivision-curve.md)
- [Collision detection](collision-detection.md)
- [Intersection of subdivision limit surfaces](intersection-of-subdivision-limit-surfaces.md)
- [Minimum distance between subdivision bodies](minimum-distance-between-subdivision-bodies.md)
- [Non-uniform rational B-spline](non-uniform-rational-b-spline.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-56/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-56/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-59/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-59/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-68/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-68/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-70/5/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-70/5/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-70/6/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-70/6/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-66/5/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-66/6/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-77/1/iii/solution.md)
- [Plane section of a subdivision surface](plane-section-of-a-subdivision-surface.md)
- [Recursive half-space clipping of a subdivision curve](recursive-half-space-clipping-of-a-subdivision-curve.md)
- [Subdivision curve interrogation](subdivision-curve-interrogation.md)
