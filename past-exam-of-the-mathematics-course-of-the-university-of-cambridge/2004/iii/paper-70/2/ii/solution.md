<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A degree-$p$ [B-spline](../../../../../../b-spline.md) basis keeps the positive [partition of unity](../../../../../../partition-of-unity.md) and [convex hull](../../../../../../convex-hull.md) properties while introducing local support. At a generic parameter value, only $p+1$ consecutive basis functions are nonzero. Moving one [control point](../../../../../../control-point.md) therefore changes only its support interval, unlike a generic interior [Bézier curve](../../../../../../bezier-curve.md) control, which affects the whole polynomial segment.

Many low-degree pieces can represent a long curve with automatic continuity. At a knot of multiplicity $m$, the generic continuity is $C^{p-m}$; simple cubic knots give $C^2$. Knot positions and multiplicities control the placement of detail and joins. Knot insertion can refine the representation without changing the curve, and local refinement avoids raising the global polynomial degree. Thus **B-splines combine geometric bounds, local editing and controlled smoothness with a fixed low degree**. Clamped end knots can also give endpoint interpolation.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
