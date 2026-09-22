<h1 id="question-1/d/solution">Solution</h1>

↑ **Parent:** [d](../d.md)

The first boundary is $u=1$. On $y=0$ in the first [quadrant](../../../../../../quadrant-plane-geometry.md), the inverse [parabolic polar coordinates](../../../../../../parabolic-polar-coordinates.md) give $v=0$. To identify the remaining [curve](../../../../../../curve.md), put $t=y^{1/3}\geq0$. Its [Cartesian coordinates](../../../../../../cartesian-coordinate-system.md) satisfy

$$
x=\frac{t^2-t^4}{2},\qquad y=t^3,\qquad
\sqrt{x^2+y^2}=\frac{t^2+t^4}{2}.
$$

Hence $u=t$ and $v=t^2$, so this boundary is $v=u^2$. The condition $x\geq0$ on this [curve](../../../../../../curve.md) requires $0\leq t\leq1$. Its endpoints are $(0,0)$ and $(0,1)$, while $u=1$ meets $v=0$ at $(1/2,0)$. These three arcs enclose exactly

$$
0\leq u\leq1,\qquad0\leq v\leq u^2.
$$

Every point in this region has $v\leq u$, and therefore $x=(u^2-v^2)/2\geq0$, as required. Using the [Jacobian determinant](../../../../../../jacobian-determinant.md), the [area](../../../../../../surface-area.md) is

$$
\begin{aligned}
A&=\int_0^1\int_0^{u^2}(u^2+v^2)\,dv\,du\\
&=\int_0^1\left(u^4+\frac{u^6}{3}\right)\,du
=\frac15+\frac1{21}
=\boxed{\frac{26}{105}}.
\end{aligned}
$$

## ↑ Ancestors (12)

1. [d](../d.md)
2. [Question 1](../../question-1.md)
3. [Mathematics V resit](../../../mathematics-v-resit-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
