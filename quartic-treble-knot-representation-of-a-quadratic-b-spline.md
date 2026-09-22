# Quartic treble-knot representation of a quadratic B-spline

↑ **Parent:** [B-spline](b-spline.md)

For a uniform quadratic [B-spline](b-spline.md) with interior [control points](control-point.md) $P_i$, label its $i$th span $[i,i+1]$. A quartic [B-spline](b-spline.md) with interior [spline knot sequence](spline-knot-sequence.md) $\tau_{3i}=\tau_{3i+1}=\tau_{3i+2}=i$ represents the identical curve when

$$
Q_{3i-1}=\frac{P_{i-1}+3P_i}{4},\quad Q_{3i}=\frac{P_{i-1}+10P_i+P_{i+1}}{12},\quad Q_{3i+1}=\frac{3P_i+P_{i+1}}4.
$$

To verify this, raise each quadratic [Bézier curve](bezier-curve.md) span twice by [degree elevation of Bernstein coefficients](degree-elevation-of-bernstein-coefficients.md). The three interior quartic controls are the displayed points. One additional [knot insertion](knot-insertion.md) at each interior knot supplies the shared endpoint as the mean of its two neighboring controls, recovering all five quartic [Bézier curve](bezier-curve.md) controls. Thus the knot multiplicity is three, giving $C^1$ joins rather than imposing unwanted extra smoothness.

## ↑ Ancestors (8)

1. [B-spline](b-spline.md)
2. [Spline approximation](spline-approximation.md)
3. [Spline (mathematics)](spline-mathematics.md)
4. [Uniform approximation](uniform-approximation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66/6/c/solution.md)
