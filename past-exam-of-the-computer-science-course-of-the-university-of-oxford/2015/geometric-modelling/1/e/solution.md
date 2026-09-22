<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The tight [axis-aligned bounding box](../../../../../axis-aligned-bounding-box.md) is $Q=[0,2]\times[0,2]$. Bisect vertically at $x=1$, giving a right child $R=[1,2]\times[0,2]$. For a scalar [implicit function](../../../../../implicit-function.md) representing the same [constructive solid geometry](../../../../../constructive-solid-geometry.md) solid, use

$$
\Phi=\max\{f_5,f_6,f_4,f_1,\min(f_2,f_3)\},\qquad P=\{\Phi\le0\}.
$$

With the convention $f_i\le0$ inside, [set intersection](../../../../../set-intersection.md) corresponds to the [maximum](../../../../../maximum-of-a-subset-of-a-total-order.md), and [set union](../../../../../set-union.md) to the [minimum](../../../../../minimum-of-a-subset-of-a-total-order.md). These operations encode membership; $\Phi$ is not a signed [distance function](../../../../../metric.md).

Since every $f_i$ is an [affine function](../../../../../affine-function.md), its extreme values on $R$ occur at corners. Exact real-arithmetic [interval arithmetic](../../../../../interval-arithmetic.md) gives:

| Function | Range on $R$ | $f_1$ | $[-1-\sqrt3,\sqrt3]$ | $f_2$ | $[-1,1]$ | $f_3$ | $[0,1]$ | $f_4$ | $[-2,0]$ | $f_5$ | $[-2,-1]$ | $f_6$ | $[-2,0]$ | $\min(f_2,f_3)$, propagated | $[-1,1]$ | $\Phi$, propagated | $[-1,\sqrt3]$ |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |

Each leaf range is exact, but combining independent [intervals](../../../../../interval-mathematics.md) forgets that the expressions share $x,y$. The final enclosure need not be the exact range of $\Phi$. For example, equality $\Phi=-1$ would require both $f_6\le-1$, hence $y\ge1$, and $\min(f_2,f_3)\le-1$, hence $y\le0$ on $R$, which is impossible. The enclosure is still sufficient for a reliable three-way decision:

$$
\boxed{\sup\Phi(R)<0:\ \text{inside};\quad
\inf\Phi(R)>0:\ \text{outside};\quad
0\in\Phi(R):\ \text{unresolved, so refine}.}
$$

Here the result is unresolved. This is a real mixed box, rather than only a pessimistic test: $(5/4,3/4)$ is strictly inside, whereas $(3/2,3/2)$ is outside. A zero endpoint alone can also mean contact with the boundary, so equality must not be treated as proof of strict interior or strict exterior. In [floating-point arithmetic](../../../../../floating-point-arithmetic-split.md), certified bounds require [outward rounding](../../../../../outward-rounding.md).

Continue splitting unresolved boxes, normally alternating axes or splitting the longest side. Propagate the [interval arithmetic](../../../../../interval-arithmetic.md) results through the [constructive solid geometry tree](../../../../../constructive-solid-geometry-tree.md), discard exterior boxes and stop refining strict interior boxes. In sufficiently small boundary boxes, locate crossings of the active [implicit equations](../../../../../implicit-equation.md) with box edges and connect them into boundary [line segments](../../../../../line-segment.md). Retain corners and resolve ambiguous multiple crossings by further refinement; here every genuine boundary piece is straight, so its supporting [implicit equation](../../../../../implicit-equation.md) allows exact intersection rather than a curved approximation. A maximum boundary-box diagonal $\varepsilon$ gives spatial localization at that scale, provided no boundary components are discarded; corner-sign sampling alone provides no such guarantee.

The tight box saves empty-space work, but it is awkward for extracting [facets](../../../../../facet.md). Entire boundary [line segments](../../../../../line-segment.md), notably $EO$, $OA$ and $DE$, lie on the initial box boundary, and $CD$ lies on the first splitting [straight line](../../../../../straight-line.md). A sign-change-only method may have no exterior sample on the other side and lose such pieces; exact zeros also persist through refinement. A slightly padded initial [axis-aligned bounding box](../../../../../axis-aligned-bounding-box.md), together with an explicit rule for boundary-coincident pieces, makes the faceting more robust. The tight box is therefore economical for enclosure but not the best unqualified choice for a simple faceting implementation.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Geometric modelling](../../../geometric-modelling-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
