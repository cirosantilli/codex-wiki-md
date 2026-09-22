<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Here the [constraint](../../../../../constraint-mechanics.md) surface $x^4+2y^2=3$ is compact and regular, so a [global minimum](../../../../../global-minimum.md) exists and satisfies the [Lagrange multiplier](../../../../../lagrange-multiplier.md) equations

$$
x^3(6x^2-4\lambda)=0,\qquad y(6y^2-4\lambda)=0.
$$

Keep the zero-coordinate cases. If $y=0$, the two points are $(\pm3^{1/4},0)$, with value $3\sqrt3$. If $x=0$, the two points are $(0,\pm\sqrt{3/2})$, with value $27/8$. If both coordinates are nonzero, the equations give $x^2=y^2=t>0$. The [constraint](../../../../../constraint-mechanics.md) becomes $t^2+2t=3$, whose only positive solution is $t=1$. These are the four points $(\pm1,\pm1)$, all with value $5/2$.

These cases exhaust the stated eight constrained [stationary points](../../../../../stationary-point.md). Comparing their values gives

$$
\boxed{\min F=\frac52,\qquad (x,y)\in\{(1,1),(1,-1),(-1,1),(-1,-1)\}.}
$$

For additional classification, substituting $u=x^2\in[0,\sqrt3]$ gives $F(u)=u^3+\tfrac38(3-u^2)^2$, with

$$
F'(u)=\tfrac32u(u-1)(u+3).
$$

It decreases from $u=0$ to $u=1$ and increases from $u=1$ to $u=\sqrt3$. Thus the two $y$-axis points are constrained local maxima, the two $x$-axis points are global maxima, and the four mixed-coordinate points are global minima.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [Discrete mathematics, continuous mathematics and probability resit](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
