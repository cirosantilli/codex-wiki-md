<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let the first [Bézier curve](../../../../../../bezier-curve.md) have degree $n$ and [control points](../../../../../../control-point.md) $P_0,\ldots,P_n$, and the next have degree $m$ and [control points](../../../../../../control-point.md) $Q_0,\ldots,Q_m$. Use one increasing parameter on the two adjacent intervals. For a continuous join, their endpoints must agree: $P_n=Q_0$. If each interval has length $h$, the endpoint [derivatives](../../../../../../derivative.md) are $n(P_n-P_{n-1})/h$ and $m(Q_1-Q_0)/h$. Therefore the [parametric first-derivative join of Bézier curves](../../../../../../parametric-first-derivative-join-of-bezier-curves.md) is exactly

$$
\boxed{P_n=Q_0,\qquad n(P_n-P_{n-1})=m(Q_1-Q_0).}
$$

For equal degrees, the two polygon edges incident on the common endpoint are equal vectors. Equivalently, $P_{n-1},P_n=Q_0,Q_1$ are collinear with the join as their midpoint. Agreement of edge directions without these lengths gives only geometric tangent [continuity](../../../../../../continuous-function.md) at a nonzero tangent, not equality of [derivatives](../../../../../../derivative.md) in the chosen parameter. The displayed condition also covers zero endpoint [derivatives](../../../../../../derivative.md). With unequal interval lengths $h,k$, the condition is instead $n(P_n-P_{n-1})/h=m(Q_1-Q_0)/k$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
