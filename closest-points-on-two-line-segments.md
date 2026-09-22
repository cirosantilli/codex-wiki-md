# Closest points on two line segments

↑ **Parent:** [Line segment](line-segment.md)

For [line segments](line-segment.md) $P+sd$ and $Q+te$, $0\leq s,t\leq1$, the squared [Euclidean distance](euclidean-distance.md) is a [convex quadratic function](convex-quadratic-function.md) on a square. Its minimum is either an admissible stationary point or a minimum on one of the four edges. Each edge minimum is a point-to-segment [orthogonal projection](orthogonal-projection.md), restricted to the interval. Testing these five candidates gives a complete algorithm; when the directions are parallel, the edge candidates suffice. Independently restricting both coordinates of the unconstrained stationary point is generally incorrect because the variables are coupled by $d\cdot e$.

**Table of contents**

- [Contact time of translating line segments](contact-time-of-translating-line-segments.md)
  - [Proximity time of translating line segments](proximity-time-of-translating-line-segments.md)

## ↑ Ancestors (6)

1. [Line segment](line-segment.md)
2. [Convex set](convex-set.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-68/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66/1/solution.md)
