# Axis-aligned bounding box

↑ **Parent:** [Bounding volume](bounding-volume.md)

An [axis-aligned bounding box](axis-aligned-bounding-box.md) is a [Cartesian product](cartesian-product.md) of [closed intervals](closed-real-interval.md) aligned with a chosen [Cartesian coordinate system](cartesian-coordinate-system.md):

$$
B=\prod_{i=1}^{d}[m_i,M_i],\qquad m_i\leq M_i.
$$

Only the two opposite corners $(m_1,\ldots,m_d)$ and $(M_1,\ldots,M_d)$ need to be stored. In two dimensions it is a [rectangle](rectangle.md). Changing the [Cartesian coordinate system](cartesian-coordinate-system.md) can change how tightly the [axis-aligned bounding box](axis-aligned-bounding-box.md) fits the same object.[§3.7, two-point representation and Figure 3.9](physically-based-rendering-from-theory-to-implementation-4th-edition-by-matt-pharr-and-others/3-7-bounding-boxes.md)

For a nonempty [finite set](finite-set.md) of [points](point-geometry.md) $P$, the smallest such [axis-aligned bounding box](axis-aligned-bounding-box.md) has

$$
m_i=\min_{p\in P}p_i,\qquad M_i=\max_{p\in P}p_i.
$$

These [minimum](minimum-of-a-subset-of-a-total-order.md) and [maximum](maximum-of-a-subset-of-a-total-order.md) values also enclose the [convex hull](convex-hull.md) of $P$: each [coordinate](coordinate-linear-algebra.md) of a [convex combination](convex-combination.md) lies between the smallest and largest input [coordinates](coordinate-linear-algebra.md). In particular, three [vertices of a polygon](vertex-of-a-polygon.md) determine the [axis-aligned bounding box](axis-aligned-bounding-box.md) of a filled [triangle](triangle.md). For a general nonempty [compact set](compact-space.md), the same formulas use all its [points](point-geometry.md); inspecting only an arbitrary finite sample is insufficient.

Given nonempty boxes $B=\prod_i[m_i,M_i]$ and $C=\prod_i[n_i,N_i]$, the [closed interval](closed-real-interval.md) convention gives

$$
B\cap C\ne\varnothing\quad\Longleftrightarrow\quad
\max(m_i,n_i)\leq\min(M_i,N_i)\quad\text{for every }i.
$$

Equivalently, reject as soon as $M_i<n_i$ or $N_i<m_i$ in any [coordinate](coordinate-linear-algebra.md). The surviving [set intersection](set-intersection.md) has endpoints $\max(m_i,n_i)$ and $\min(M_i,N_i)$. This is an exact box test, while its conclusion about enclosed objects remains a [conservative enclosure test](conservative-enclosure-test.md).[§3.7, Intersect() and Overlaps(): coordinate-wise intersection and inclusive comparisons](physically-based-rendering-from-theory-to-implementation-4th-edition-by-matt-pharr-and-others/3-7-bounding-boxes.md)

Equality counts as touching: $[0,1]\times[0,1]$ and $[1,2]\times[0,1]$ share an edge, so their [set intersection](set-intersection.md) is nonempty. Replacing every $\leq$ in the overlap formula by $<$ tests intersection of the [interiors](interior-topology.md) of full-dimensional boxes and excludes this contact. A zero-width [closed interval](closed-real-interval.md) can represent a [point](point-geometry.md) or a lower-dimensional enclosure, and must not automatically be discarded when touching counts. A box with some $m_i>M_i$ is empty; test emptiness before applying rules intended for nonempty boxes. The [broad phase](broad-phase.md) must retain touching candidates whenever the [narrow phase](narrow-phase.md) counts touching as a hit.

For nonempty boxes, the smallest enclosing [axis-aligned bounding box](axis-aligned-bounding-box.md) of their [set union](set-union.md) is

$$
\prod_{i=1}^{d}\bigl[\min(m_i,n_i),\max(M_i,N_i)\bigr].
$$

This operation supplies the parent boxes in a [bounding volume hierarchy](bounding-volume-hierarchy.md). It is an enclosure of the [set union](set-union.md), rather than generally the [set union](set-union.md) itself. In [floating-point arithmetic](floating-point-arithmetic-split.md), comparisons are conclusive only for endpoints that still enclose the intended exact objects; use certified bounds such as [interval arithmetic](interval-arithmetic.md) with [outward rounding](outward-rounding.md) when that guarantee is required.

// Target: analysis.bigb

## ↑ Ancestors (7)

1. [Bounding volume](bounding-volume.md)
2. [Computer aided geometric design](computer-aided-geometric-design-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Axis-aligned bounding box](axis-aligned-bounding-box.md)
- [Bézier curve](bezier-curve.md)
- [Bounding volume](bounding-volume.md)
- [Bounding volume hierarchy](bounding-volume-hierarchy.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-59/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-68/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-70/6/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-77/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-77/1/iii/solution.md)
