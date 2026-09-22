<h1 id="6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A useful [subdivision curve interrogation](../../../../../../subdivision-curve-interrogation.md) supplies the following connected capabilities. It describes the parameter interval, open or closed topology, endpoints and break points; it evaluates the limit point $C(t)$ and, where the scheme guarantees them, $C'(t)$ and $C''(t)$; and it refines or restricts an interval while retaining the mapping to the original parameter. It also provides enclosing bounds and a certified curve-to-chord error on each restricted piece. These are enough to build clipping, intersections, closest-point searches, tangents, [curvature](../../../../../../curvature.md) and adaptive sampling.

The enquiries concern the subdivision limit, not just a finite refined [control polygon](../../../../../../control-polygon.md). For a stationary local refinement [matrix](../../../../../../matrix.md) $A$, a limit vertex can be obtained from a normalized [left eigenvector](../../../../../../left-eigenvector.md) $w^TA=w^T$, $w^T\mathbf1=1$, as $w^TP$. [Derivatives](../../../../../../derivative.md) use the appropriately scaled difference schemes or equivalent spline evaluation on regular intervals. The convergence and [derivative](../../../../../../derivative.md) hypotheses must actually hold for the scheme; no [second derivative](../../../../../../second-derivative.md) can be requested at an intrinsic crease.

If the [subdivision mask](../../../../../../subdivision-mask.md) is nonnegative and preserves constants, descendants and limit points lie in the relevant control-point [convex hull](../../../../../../convex-hull.md), giving a useful enclosing volume. For [subdivision masks](../../../../../../subdivision-mask.md) with negative weights, that hull need not be an enclosure: the interface must supply another valid bound, for example from a proven refinement-error estimate. This distinction is important for safe spatial rejection in an algorithm.

## ↑ Ancestors (11)

1. [I](../i.md)
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
