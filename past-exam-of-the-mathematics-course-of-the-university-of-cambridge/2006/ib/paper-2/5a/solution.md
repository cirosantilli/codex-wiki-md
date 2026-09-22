<h1 id="5a/solution">Solution</h1>

↑ **Parent:** [5A](../5a.md)

At a constrained [stationary point](../../../../../stationary-point.md) where $\nabla g\ne0$, every tangent direction to $g=0$ is orthogonal to $\nabla g$. Vanishing of the directional derivative of $f$ in all such directions forces $\nabla f=\lambda\nabla g$ for a [Lagrange multiplier](../../../../../lagrange-multiplier.md) $\lambda$. Solve these equations together with the [constraint](../../../../../constraint-mechanics.md), then check the candidates and any singular or limiting cases for minima or maxima.

Let a closed cylinder have radius $r>0$ and height $h>0$, with fixed $V>0$. Its area is $A=2\pi r^2+2\pi rh$ and the [constraint](../../../../../constraint-mechanics.md) is $\pi r^2h=V$. The [Lagrange multiplier](../../../../../lagrange-multiplier.md) equations give

$$
4\pi r+2\pi h=\lambda\,2\pi rh,\qquad2\pi r=\lambda\pi r^2.
$$

The second yields $\lambda=2/r$; substituting into the first gives $h=2r$. Thus the [minimum-area closed cylinder at fixed volume](../../../../../minimum-area-closed-cylinder-at-fixed-volume.md) has

$$
\boxed{r=\left(\frac V{2\pi}\right)^{1/3},\qquad h=2\left(\frac V{2\pi}\right)^{1/3},\qquad A_{\min}=3(2\pi)^{1/3}V^{2/3}.}
$$

To prove it is the [global minimum](../../../../../global-minimum.md), eliminate $h$ to obtain $A(r)=2\pi r^2+2V/r$. Its derivative is $4\pi r-2V/r^2$, negative before the displayed radius and positive afterwards; the area tends to infinity both as $r\downarrow0$ and as $r\to\infty$. This establishes uniqueness and rules out limiting smaller areas.

## ↑ Ancestors (10)

1. [5A](../5a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
