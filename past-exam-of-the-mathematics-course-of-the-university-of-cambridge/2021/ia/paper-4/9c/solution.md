<h1 id="9c/solution">Solution</h1>

↑ **Parent:** [9C](../9c.md)

The [work](../../../../../work.md) done along the trajectory is

$$
W=\int_{t_a}^{t_b}F(x(t),t)\dot x(t)\,dt
=\int_a^bF(x,t(x))\,dx.
$$

By [Newton's second law](../../../../../newton-s-second-law.md), $F=m\ddot x$, so

$$
W=m\int_{t_a}^{t_b}\ddot x\dot x\,dt
=\left[\frac12m\dot x^2\right]_{t_a}^{t_b}.
$$

This is the [work-energy theorem](../../../../../work-energy-theorem.md): the work equals the change in [kinetic energy](../../../../../kinetic-energy.md).

A force is [conservative](../../../../../conservative-force.md) when its work between two points is independent of the path, equivalently when it is the negative gradient of a [potential energy](../../../../../potential-energy.md). Here a potential with $V(0)=0$ is

$$
V(x)=F_0\lambda(1-e^{-|x|/\lambda}).
$$

Conservation of [energy](../../../../../energy.md) for $x>0$ gives

$$
\frac12mv^2+F_0\lambda(1-e^{-x/\lambda})=\frac12mv_0^2.
$$

Thus

$$
v(x)=\sqrt{v_0^2+v_e^2(e^{-|x|/\lambda}-1)},
\qquad
\boxed{v_e=\sqrt{\frac{2F_0\lambda}{m}}}.
$$

If $v_0>v_e$, the particle escapes with asymptotic speed $\sqrt{v_0^2-v_e^2}$; the graph decreases from $v_0$ to this horizontal asymptote. At the [escape velocity](../../../../../escape-velocity.md) $v_0=v_e$, it decreases as $v_e e^{-x/(2\lambda)}$ and approaches zero only at infinity. If $v_0<v_e$, it reaches the [turning point](../../../../../turning-point.md)

$$
x_{\max}=-\lambda\log\left(1-\frac{v_0^2}{v_e^2}\right),
$$

where $v=0$, then returns on the negative branch of the same curve and oscillates symmetrically about the origin.

For oscillation put $w=1-v_0^2/v_e^2$. One quarter of the [period](../../../../../period-of-an-oscillation.md) is

$$
\int_0^{x_{\max}}\frac{dx}{v(x)}
=\frac{\lambda}{v_e}\int_w^1\frac{du}{u\sqrt{u-w}}
=\frac{2\lambda}{v_e\sqrt w}\cos^{-1}\sqrt w,
$$

where $u=e^{-x/\lambda}$. Therefore

$$
\boxed{T=\frac{8\lambda}{v_e\sqrt{1-v_0^2/v_e^2}}
\cos^{-1}\sqrt{1-v_0^2/v_e^2}}.
$$

## ↑ Ancestors (10)

1. [9C](../9c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
