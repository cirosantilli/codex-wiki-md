<h1 id="2h/solution">Solution</h1>

↑ **Parent:** [2H](../2h.md)

In the [upper half-plane model](../../../../../poincare-half-plane-model.md) $H=\{(x,y):y>0\}$ the [hyperbolic metric](../../../../../hyperbolic-metric.md) is

$$
ds^2=\frac{dx^2+dy^2}{y^2}.
$$

The length of a differentiable curve is $\int\sqrt{\dot x^2+\dot y^2}\,dt/y$. The area element is the square root of the metric determinant times $dx\,dy$, so the [hyperbolic area](../../../../../hyperbolic-area.md) of a measurable region $S$ is $\int_S y^{-2}\,dx\,dy$.

The [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md) for a [geodesic](../../../../../geodesic.md) [hyperbolic triangle](../../../../../hyperbolic-triangle.md) of angles $\alpha,\beta,\gamma$ in [curvature](../../../../../curvature.md) $-1$ gives **area $\pi-\alpha-\beta-\gamma$**; an ideal vertex has angle zero. The horizontal edge in the present region is not a [geodesic](../../../../../geodesic.md), so it is simpler to use the area element directly:

$$
\operatorname{Area}_H(R)=\int_0^{1/2}\int_{\sqrt{1-x^2}}^1\frac{dy\,dx}{y^2}
=\int_0^{1/2}\left(\frac1{\sqrt{1-x^2}}-1\right)dx
=\boxed{\frac\pi6-\frac12}.
$$

The open boundary does not affect the [integral](../../../../../integral.md) because its area is zero.

## ↑ Ancestors (10)

1. [2H](../2h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
