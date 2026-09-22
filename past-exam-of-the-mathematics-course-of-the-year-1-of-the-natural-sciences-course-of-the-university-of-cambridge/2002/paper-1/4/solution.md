<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For two independent smooth constraints $g=h=0$, the tangent direction is orthogonal to both [gradients](../../../../gradient.md). At a constrained [stationary point](../../../../stationary-point.md), the [gradient](../../../../gradient.md) of the objective is also orthogonal to that direction, hence lies in their span: $\nabla f=\lambda\nabla g+\mu\nabla h$. This is the two-constraint [Lagrange multiplier](../../../../lagrange-multiplier.md) condition. Alternatively, [distance extrema on a central plane section of an ellipsoid](../../../../distance-extrema-on-a-central-plane-section-of-an-ellipsoid.md) follow from a two-dimensional [eigenvalue](../../../../eigenvalue.md) problem.

Minimizing distance is equivalent to minimizing $f=x^2+y^2+z^2$. Put $g=x-y+z$ and $h=x^2+(y^2+z^2)/4-1$. The [Lagrange multiplier](../../../../lagrange-multiplier.md) equations are

$$
2(1-\mu)x=\lambda,\qquad (2-\mu/2)y=-\lambda,\qquad (2-\mu/2)z=\lambda.
$$

Adding the latter two gives $(2-\mu/2)(y+z)=0$. If $\mu=4$, those equations give $\lambda=x=0$; the constraints then give $y=z=\pm\sqrt2$ and $f=4$. Otherwise $z=-y$ and $x=2y$. The ellipsoidal constraint gives $y=\pm\sqrt2/3$, and hence

$$
(x,y,z)=\pm\frac{\sqrt2}3(2,1,-1),\qquad f=\frac43.
$$

The intersection is [compact](../../../../compact-space.md). The two constraint [gradients](../../../../gradient.md) are independent there: if $\nabla h=t\nabla g$, then $(x,y,z)=(t/2,-2t,2t)$, and $g=0$ forces $t=0$, contradicting $h=0$. Thus every global extremum is among these candidates. Taking square roots gives

$$
\boxed{d_{\min}=\frac2{\sqrt3},\qquad d_{\max}=2.}
$$

## ↑ Ancestors (12)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [2002](../../split.md)
4. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
