<h1 id="p/p4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [natural cubic spline](../../../../../natural-cubic-spline.md) with the given [knots](../../../../../knot.md) is a $C^2$ function that is [polynomial](../../../../../polynomial-split.md) of [degree](../../../../../degree-of-a-polynomial.md) at most three on each [interval](../../../../../interval-mathematics.md) between consecutive [knots](../../../../../knot.md) and has $S''(x_0)=S''(x_4)=0$. With the usual whole-line convention, it extends affinely outside the extreme [knots](../../../../../knot.md). The word natural refers to these endpoint second-derivative conditions; the [interpolation](../../../../../interpolation-split.md) values must be specified separately.

For $H_k(x)=(x-x_k)^3_+$, direct differentiation on either side of the [knot](../../../../../knot.md) gives

$$
H_k'(x)=3(x-x_k)^2_+,\qquad H_k''(x)=6(x-x_k)_+.
$$

Both one-sided limits of the function and its first two [derivatives](../../../../../derivative.md) at $x_k$ are zero, so these formulas are [continuous](../../../../../continuous-function.md) there and

$$
\boxed{H_k\in C^2(\mathbb R).}
$$

Its third [derivative](../../../../../derivative.md) jumps from zero to six, which is permitted for a [cubic spline](../../../../../cubic-spline.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [P4](../../p4.md)
3. [P](../../../p.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
