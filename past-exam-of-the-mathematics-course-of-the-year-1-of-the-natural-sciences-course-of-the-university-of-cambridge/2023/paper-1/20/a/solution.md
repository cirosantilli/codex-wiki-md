<h1 id="20/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a differentiable objective $f$ and regular constraint $g=r$, a constrained [stationary point](../../../../../stationary-point.md) satisfies

$$
\boxed{\nabla f=\lambda\nabla g,\qquad g=r,}
$$

where $\lambda$ is a [Lagrange multiplier](../../../../../lagrange-multiplier.md). Solve these equations for both the coordinates and $\lambda$.

Geometrically, the [gradient](../../../../../gradient.md) $\nabla g$ is normal to the constraint [level set](../../../../../level-set.md) when $\nabla g\ne0$. Every feasible infinitesimal displacement $\mathbf v$ is tangent to that [level set](../../../../../level-set.md), so $\nabla g\cdot\mathbf v=0$. At a constrained [stationary point](../../../../../stationary-point.md), the directional change $\nabla f\cdot\mathbf v$ must also vanish for every such tangent displacement. Thus $\nabla f$ is normal to the same tangent [plane](../../../../../plane.md) and is a [scalar multiple](../../../../../scalar-multiple.md) of $\nabla g$. This is the geometric basis of the [Lagrange multiplier](../../../../../lagrange-multiplier.md) method.

For a second constraint $h=s$, with [linearly independent vectors](../../../../../linear-independence.md) $\nabla g$ and $\nabla h$, the feasible tangent directions are perpendicular to both. Their normal space is the [linear span](../../../../../linear-span.md) of these two [gradients](../../../../../gradient.md), so introduce a second [Lagrange multiplier](../../../../../lagrange-multiplier.md):

$$
\boxed{\nabla f=\lambda\nabla g+\mu\nabla h,\qquad g=r,\quad h=s.}
$$

These equations find candidates; deciding whether they are maxima, minima or [saddle points](../../../../../saddle-point.md) requires further analysis. Constraint [points](../../../../../point-geometry.md) where the required gradient independence fails must be examined separately.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [20](../../20.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
