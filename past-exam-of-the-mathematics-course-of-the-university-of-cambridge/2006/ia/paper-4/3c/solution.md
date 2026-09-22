<h1 id="3c/solution">Solution</h1>

↑ **Parent:** [3C](../3c.md)

Let $m$ be the car's mass and let $v(t)$ be its forward speed. Initially the driven contact surfaces slip backward relative to the ground because $v<r\Omega$. Thus [kinetic friction](../../../../../kinetic-friction.md) on the car acts forward. On the horizontal surface the total [normal force](../../../../../normal-force.md) is $mg$, so [Newton's second law](../../../../../newton-s-second-law.md) gives $m\dot v=\mu mg$. While slipping persists,

$$
v(t)=\mu gt.
$$

The contact slip speed is $r\Omega-v(t)$. Its first zero is the onset of [rolling without slipping](../../../../../rolling-without-slipping.md), hence

$$
\boxed{T=\frac{r\Omega}{\mu g}.}
$$

The engine maintains the prescribed wheel speed, so wheel spin-down is not part of this calculation.

On a slope of angle $\alpha>0$, directed uphill, the [normal force](../../../../../normal-force.md) is $mg\cos\alpha$ and gravity contributes $-mg\sin\alpha$ along the slope. Therefore the uphill acceleration while slipping is $g(\mu\cos\alpha-\sin\alpha)$. If it is positive, the onset of [rolling without slipping](../../../../../rolling-without-slipping.md) occurs at

$$
\boxed{T_\alpha=\frac{r\Omega}{g(\mu\cos\alpha-\sin\alpha)}>T.}
$$

The inequality follows because $\mu\cos\alpha-\sin\alpha<\mu$. If $\mu\cos\alpha\leq\sin\alpha$, the car does not accelerate uphill to $r\Omega$, so there is no finite catch-up time in this sliding-friction model. The finite-time conclusion presumes positive traction sufficient to climb the slope.

## ↑ Ancestors (10)

1. [3C](../3c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
