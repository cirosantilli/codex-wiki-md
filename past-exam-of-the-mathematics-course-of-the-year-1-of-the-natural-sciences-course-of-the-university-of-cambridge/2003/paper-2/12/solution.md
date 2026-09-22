<h1 id="12/solution">Solution</h1>

↑ **Parent:** [12](../12.md)

Expand $u=3x^2-2xy+3y^2$. The [Lagrange multiplier](../../../../lagrange-multiplier.md) equations for $u-\lambda v$ are $(6-2\lambda)x-2y=0$ and $-2x+6y+\lambda=0$, together with the [constraint](../../../../constraint-mechanics.md) $y=x^2-1/4$. The first two imply $y=(3-\lambda)x$ and $(6\lambda-16)x=\lambda$. The value $\lambda=8/3$ would make the latter equation inconsistent, so division is allowed:

$$
\boxed{x=\frac{\lambda}{6\lambda-16},\qquad y=\frac{\lambda(3-\lambda)}{6\lambda-16}.}
$$

Insert these into $x^2-y-1/4=0$ and multiply by $(6\lambda-16)^2$. Simplification gives $2(3\lambda^3-21\lambda^2+48\lambda-32)=0$, hence

$$
\boxed{3\lambda^3-21\lambda^2+48\lambda-32=0.}
$$

The [gradient](../../../../gradient.md) of the [constraint](../../../../constraint-mechanics.md) $(2x,-1)$ is never zero, so the [Lagrange multiplier](../../../../lagrange-multiplier.md) condition is necessary at every constrained [extremum](../../../../maximum-and-minimum.md). To establish a global [minimum](../../../../minimum-of-a-subset-of-a-total-order.md), parametrize the whole [parabola](../../../../parabola.md) by $y=x^2-1/4$. The restricted [function](../../../../function-split.md) becomes

$$
q(x)=3x^4-2x^3+\frac32x^2+\frac12x+\frac3{16}.
$$

It is [coercive](../../../../coercive-bilinear-form.md): $q(x)\to\infty$ as $|x|\to\infty$, so it attains a global [minimum](../../../../minimum-of-a-subset-of-a-total-order.md). Moreover $q''(x)=36(x-1/6)^2+2>0$, making it [strictly convex](../../../../strictly-convex-function.md) and ensuring that this [minimum](../../../../minimum-of-a-subset-of-a-total-order.md) is unique. This proves more than the permitted assumption of one real multiplier root.

The [level sets](../../../../level-set.md) of $u$ are nested [ellipses](../../../../ellipse.md) centered at the origin. In the rotated coordinates $p=(x+y)/\sqrt2$, $q=(x-y)/\sqrt2$, they have equation $2p^2+4q^2=\text{constant}$, with the longer axis along $x=y$. The smallest one meeting the [parabola](../../../../parabola.md) is tangent to it at the unique minimizing point, approximately $(x,y)=(-0.12654,-0.23399)$, where $u\simeq0.15307$ and $\lambda\simeq1.15085$.

<a id="12/image-the-smallest-quadratic-contour-touching-a-parabolic-constraint"></a>
![](../../../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-2-constrained-ellipse-parabola.png)

**[Figure 2](#12/image-the-smallest-quadratic-contour-touching-a-parabolic-constraint). The smallest quadratic contour touching a parabolic constraint**. Original level-set plot. The highlighted ellipse is tangent to the parabola at the unique global minimum; larger quadratic contours intersect the constraint.

## ↑ Ancestors (12)

1. [12](../12.md)
2. [Paper 2](../../paper-2-split.md)
3. [2003](../../split.md)
4. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
