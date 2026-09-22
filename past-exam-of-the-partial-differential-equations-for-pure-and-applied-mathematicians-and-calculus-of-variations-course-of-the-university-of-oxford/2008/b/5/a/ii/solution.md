<h1 id="b/5/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [strictly convex function](../../../../../../strictly-convex-function.md) satisfies that inequality strictly whenever $x\ne y$ and $0<t<1$.

For necessity of the strict supporting-tangent property, [convexity](../../../../../../convex-function.md) gives a nonnegative gap along a segment from $z_0$ to $z$. If the gap at its other endpoint were zero, [convexity](../../../../../../convex-function.md) of the gap and its zero initial value would force it to be zero all along the segment. That would make $F$ affine on this nontrivial segment, contrary to [strict convexity](../../../../../../strictly-convex-function.md). Conversely let $z=(1-t)x+ty$ with distinct endpoints. Apply the strict supporting inequality at $z$ to both endpoints, multiply by $1-t$ and $t$, and add. The linear terms cancel, yielding [strict convexity](../../../../../../strictly-convex-function.md). Thus

$$
\boxed{F\text{ strictly convex}\iff F(z)>F(z_0)+DF(z_0)\cdot(z-z_0)\text{ for }z\ne z_0.}
$$

For strict [Jensen's inequality](../../../../../../jensen-s-inequality.md), put $m=(b-a)^{-1}\int_a^bu$. The supporting gap $F(u)-F(m)-DF(m)\cdot(u-m)$ is nonnegative everywhere and strictly positive where $u\ne m$. That set has positive measure because $u$ is not [almost everywhere](../../../../../../almost-everywhere.md) constant. Its integral is therefore strictly positive. The linear term integrates to zero, giving the requested **strict integral [Jensen inequality](../../../../../../jensen-s-inequality.md)**.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [B](../../../../b.md)
5. [2008](../../../../../2008-split.md)
6. [Past exam of the partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../../../split.md)
7. [Partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../../../../partial-differential-equations-for-pure-and-applied-mathematicians-and-calculus-of-variations-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
