<h1 id="5a/solution">Solution</h1>

↑ **Parent:** [5A](../5a.md)

For the [method of characteristics](../../../../../method-of-characteristics.md), parameterize by $x$; the [characteristic curves](../../../../../characteristic-curve.md) satisfy

$$
\frac{dy}{dx}=-2x,\qquad \frac{du}{dx}=\cos x.
$$

Thus $x^2+y=C$ and $u-\sin x$ is constant on each [characteristic curve](../../../../../characteristic-curve.md). The general form in the quadrant is $u=\sin x+F(x^2+y)$. The [boundary condition](../../../../../boundary-condition.md) gives $F(s^2)=\cos s-\sin s$ for every $s\ge0$.

The [characteristic curve](../../../../../characteristic-curve.md) through $(x,y)$ meets the boundary at $(s,0)$ with $s=\sqrt{x^2+y}\ge x$. Integrating backwards from that boundary value yields

$$
\boxed{u(x,y)=\sin x+\cos\sqrt{x^2+y}-\sin\sqrt{x^2+y}.}
$$

Indeed $\partial_x-2x\partial_y$ annihilates $x^2+y$ and sends $\sin x$ to $\cos x$, while on $y=0$ the expression reduces to $\cos x$. **Every characteristic in the quadrant meets the prescribed boundary, so its value is determined.** The displayed solution is smooth away from the origin. At the origin the boundary is characteristic and the solution is continuous but has a singular inward $y$ derivative; the differential equation is interpreted in the interior, with the boundary data attained continuously.

## ↑ Ancestors (10)

1. [5A](../5a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
