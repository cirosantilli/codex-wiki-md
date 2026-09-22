<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Material conservation of [shallow-water potential vorticity](../../../../../../shallow-water-potential-vorticity.md) carries $P=0$ from the reservoir into the channel. At leading order in a long, slowly varying channel, $v$ and $v_x$ are negligible, so $\zeta\simeq-u_y$. Zero [absolute vorticity](../../../../../../absolute-vorticity.md) therefore implies $u_y=f$. Integration from $y=0$, followed by cross-channel [geostrophic balance](../../../../../../geostrophic-balance.md), gives the [zero-potential-vorticity rotating channel flow](../../../../../../zero-potential-vorticity-rotating-channel-flow.md):

$$
\boxed{u(x,y)=u_1(x)+fy,\qquad h(x,y)=h_1(x)-\frac f g\left[u_1(x)y+\frac12fy^2\right].}
$$

In particular, $u_2=u_1+fb$ and $h_2=h_1-(fb/g)(u_1+fb/2)$. The velocity increases towards the shallower wall. Differentiating the depth-based specific energy confirms

$$
\partial_y\left(h+\frac{u^2}{2g}\right)=h_y+\frac{u u_y}{g}=-\frac{fu}{g}+\frac{fu}{g}=0.
$$

This cross-channel constancy is also the $P=0$ consequence of $\nabla B=-P\nabla\psi$.

For a reservoir of finite depth, exact $P=0$ requires relative [vorticity](../../../../../../vorticity.md) $\zeta=-f$, an anticyclonic rotation cancelling the planetary [vorticity](../../../../../../vorticity.md). A reservoir at rest in the rotating frame has $\zeta=0$ and $P=f/h$, so it does not have exactly zero [shallow-water potential vorticity](../../../../../../shallow-water-potential-vorticity.md). A very deep, nearly quiescent reservoir can nevertheless supply the approximation $P\simeq0$ because $f/h$ is small. The idealization must describe vanishing [absolute vorticity](../../../../../../absolute-vorticity.md) or this deep-reservoir limit, rather than ordinary finite-depth rest in the rotating frame.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
