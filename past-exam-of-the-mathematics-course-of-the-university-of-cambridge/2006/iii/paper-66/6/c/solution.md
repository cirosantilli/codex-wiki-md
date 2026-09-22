<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [quartic treble-knot representation of a quadratic B-spline](../../../../../../quartic-treble-knot-representation-of-a-quadratic-b-spline.md). Specify the indexing as well as the controls: for the interior of the long curve, take the quartic [spline knot sequence](../../../../../../spline-knot-sequence.md)

$$
\tau_{3i}=\tau_{3i+1}=\tau_{3i+2}=i.
$$

With the standard [B-spline](../../../../../../b-spline.md) convention that control $Q_j$ multiplies $N_{j,4}$ supported on $[\tau_j,\tau_{j+5}]$, the answer is

$$
\boxed{Q_{3i-1}=\frac{P_{i-1}+3P_i}{4},\qquad Q_{3i}=\frac{P_{i-1}+10P_i+P_{i+1}}{12},\qquad Q_{3i+1}=\frac{3P_i+P_{i+1}}4.}
$$

In other words, keep the three interior quartic [Bézier curve](../../../../../../bezier-curve.md) controls $E_{1,i},E_{2,i},E_{3,i}$ for each span in that order. The offset $3i-1$ matters for the stated knot indexing; shifting all indices together gives an equivalent convention.

To prove the representation, insert each integer interior knot once, changing multiplicity three to four. A degree-four knot of multiplicity four separates [Bézier curve](../../../../../../bezier-curve.md) spans while leaving their shared endpoint common. The three interior controls $E_{1,i},E_{2,i},E_{3,i}$ remain, and [knot insertion](../../../../../../knot-insertion.md) constructs the shared endpoint from its neighboring controls with weights $1/2,1/2$, since adjacent knot intervals have equal length. In fact,

$$
\frac{E_{3,i-1}+E_{1,i}}2=\frac{(3P_{i-1}+P_i)+(P_{i-1}+3P_i)}8=\frac{P_{i-1}+P_i}2=E_{0,i}.
$$

The right endpoint is obtained in the same way. Hence every extracted quartic span has exactly the five controls proved in part (b). [Knot insertion](../../../../../../knot-insertion.md) leaves the curve unchanged, so the assembled quartic [B-spline](../../../../../../b-spline.md) is identical to the original quadratic one on every span.

There is also a derivative check at each join:

$$
4(E_{4,i}-E_{3,i})=P_{i+1}-P_i=4(E_{1,i+1}-E_{0,i+1}).
$$

This is why treble knots are appropriate: degree four with interior knot multiplicity three permits $C^{4-3}=C^1$ continuity, exactly the generic continuity of the uniform quadratic [B-spline](../../../../../../b-spline.md). For a finite clamped curve, include its endpoint controls and endpoint knot multiplicities using the same [degree elevation of Bernstein coefficients](../../../../../../degree-elevation-of-bernstein-coefficients.md) and [knot insertion](../../../../../../knot-insertion.md); the displayed formulas describe the long interior requested here, without imposing an unstated end condition.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
