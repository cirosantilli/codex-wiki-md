<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Separate inactive and active [optimization constraints](../../../../../optimization-constraint.md). At an interior feasible point with $h>0$, a differentiable [local minimum](../../../../../local-minimum.md) must satisfy $\nabla f=0$. Retain only solutions lying in the interior.

On the boundary $h=0$, if $\nabla h\ne0$, apply the [Lagrange multiplier](../../../../../lagrange-multiplier.md) condition. Using the [optimization Lagrangian](../../../../../optimization-lagrangian.md) $L=f-\lambda h$, the [Karush-Kuhn-Tucker conditions](../../../../../karush-kuhn-tucker-conditions.md) are

$$
\nabla f=\lambda\nabla h,\qquad h\geq0,\qquad
\lambda\geq0,\qquad\lambda h=0.
$$

The sign follows from feasible motion into $h>0$: the directional [derivative](../../../../../derivative.md) along $\nabla h$ at a minimum cannot be negative. Thus a boundary candidate has $h=0$ and a nonnegative [Lagrange multiplier](../../../../../lagrange-multiplier.md). Boundary points with $\nabla h=0$ must be examined separately, because the usual constraint qualification fails there.

Solve the interior and boundary systems, check membership in the [feasible set](../../../../../feasible-region.md), and establish which candidates are minima using second-order tests or a direct global comparison. The [Karush-Kuhn-Tucker conditions](../../../../../karush-kuhn-tucker-conditions.md) alone are not sufficient for general nonconvex [functions](../../../../../function-split.md) or [feasible sets](../../../../../feasible-region.md). On an unbounded [feasible set](../../../../../feasible-region.md), also check whether an infimum is attained and whether escaping [sequences](../../../../../sequence.md) can improve the objective.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
