<h1 id="a/1/i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For each $0<\xi<2\pi$, the [Green's function](../../../../../../green-s-function-split.md) is a [distribution](../../../../../../distribution-mathematical-analysis.md) in $x$ satisfying

$$
\boxed{(\partial_x^2+2\partial_x+2)g(x,\xi)=\delta(x-\xi),\qquad g(0,\xi)=0,\quad g_x(2\pi,\xi)=0.}
$$

Equivalently, $g$ is a classical homogeneous solution on each side of $\xi$, satisfies the same endpoint conditions, and obeys the [Green function jump conditions](../../../../../../green-function-jump-conditions.md)

$$
\boxed{g(\xi^+,\xi)=g(\xi^-,\xi),\qquad g_x(\xi^+,\xi)-g_x(\xi^-,\xi)=1.}
$$

To see equivalence, let $[g]$ and $[g_x]$ denote its jumps. The singular part of $L_xg$ is $[g]\delta'(x-\xi)+([g_x]+2[g])\delta(x-\xi)$. Matching a unit [Dirac delta distribution](../../../../../../dirac-delta-function.md) with no [derivative](../../../../../../derivative.md) first forces [continuity](../../../../../../continuous-function.md), then the unit [derivative](../../../../../../derivative.md) jump. Conversely these conditions produce exactly that [distribution](../../../../../../distribution-mathematical-analysis.md). The solution for a regular forcing is $y(x)=\int_0^{2\pi}g(x,\xi)f(\xi)\,d\xi$. The homogeneous endpoint problem has only the zero solution, which ensures uniqueness of this [kernel](../../../../../../kernel-of-a-linear-map-split.md).

## ↑ Ancestors (14)

1. [B](../b.md)
2. [I](../../i.md)
3. [1](../../../1.md)
4. [A](../../../../a.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the differential equations and applications course of the University of Oxford](../../../../../split.md)
7. [Differential equations and applications course of the University of Oxford](../../../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
