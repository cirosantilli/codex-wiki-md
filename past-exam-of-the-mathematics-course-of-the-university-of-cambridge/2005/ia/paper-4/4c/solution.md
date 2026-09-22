<h1 id="4c/solution">Solution</h1>

↑ **Parent:** [4C](../4c.md)

On the horizontal road the total [normal reaction](../../../../../normal-force.md) is $Mg$. The [kinetic friction](../../../../../kinetic-friction.md) force has magnitude $\mu Mg$, so [Newtonian mechanics](../../../../../newtonian-mechanics.md) gives $\dot u=-\mu g$ until rest. Thus

$$
\boxed{t_{{\rm dry}}=\frac U{\mu g},\qquad d_{{\rm dry}}=\frac{U^2}{2\mu g}.}
$$

For the wet high-speed stage, add the four tyre drags: the total [linear drag](../../../../../linear-drag.md) is $\lambda u$, not $\lambda u/4$. Hence $M\dot u=-\lambda u$ and $u(t)=Ue^{-\lambda t/M}$. At the switching speed $u_*=U/4$, the elapsed time and distance are

$$
t_*=\frac M\lambda\log4,\qquad
d_*=\int_0^{t_*}Ue^{-\lambda t/M}dt=\frac{3MU}{4\lambda}.
$$

The remaining stage has the same constant [kinetic friction](../../../../../kinetic-friction.md) deceleration as on a dry road, but starts at $U/4$. It therefore contributes time $U/(4\mu g)$ and distance $U^2/(32\mu g)$. Adding both stages of the [two-stage stopping under linear drag and dry friction](../../../../../two-stage-stopping-under-linear-drag-and-dry-friction.md) gives

$$
\boxed{t_{{\rm wet}}=\frac M\lambda\log4+\frac U{4\mu g},\qquad
d_{{\rm wet}}=\frac{3MU}{4\lambda}+\frac{U^2}{32\mu g}.}
$$

The exponential first stage reaches its positive switching speed in finite time; it need not reach zero under [linear drag](../../../../../linear-drag.md).

## ↑ Ancestors (10)

1. [4C](../4c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
