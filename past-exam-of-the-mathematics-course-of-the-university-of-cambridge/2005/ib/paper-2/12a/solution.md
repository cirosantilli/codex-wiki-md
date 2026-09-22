<h1 id="12a/solution">Solution</h1>

↑ **Parent:** [12A](../12a.md)

For a [Riemannian metric](../../../../../riemannian-metric.md) $g$, write $s(t)=\sqrt{g_{\gamma(t)}(\dot\gamma(t),\dot\gamma(t))}$. Use the [energy of a curve](../../../../../energy-of-a-curve.md) normalization compatible with the requested inequality:

$$
L(\gamma)=\int_0^1s(t)\,dt,\qquad E(\gamma)=\int_0^1s(t)^2\,dt.
$$

The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) here has the direct variance form

$$
E-L^2=\int_0^1(s(t)-L)^2\,dt\geq0.
$$

Equality holds exactly when $s$ is constant almost everywhere, hence everywhere for a smooth [curve](../../../../../curve.md). With the alternative [energy of a curve](../../../../../energy-of-a-curve.md) convention containing a factor $1/2$, the same assertion reads $L^2\leq2E$.

In the upper half-plane write $\gamma=u+iv$, $v>0$, and use $ds^2=(du^2+dv^2)/v^2$. Let the endpoints be $P=ip$, $Q=iq$, $p,q>0$. Then

$$
L=\int_0^1\frac{\sqrt{\dot u^2+\dot v^2}}v\,dt
\geq\int_0^1\frac{|\dot v|}v\,dt
\geq\left|\log\frac qp\right|.
$$

The first equality requires $\dot u=0$ throughout. Endpoint values force $u=0$. The second equality requires the [derivative](../../../../../derivative.md) of $\log v$ to have one sign, so $v$ is [monotone](../../../../../monotonic-function.md). Conversely every smooth [monotone](../../../../../monotonic-function.md) positive $v$ with these endpoints attains this bound. Consequently **the absolute length minimizers are precisely the vertical [curves](../../../../../curve.md) with [monotone](../../../../../monotonic-function.md) height**, including a constant [curve](../../../../../curve.md) when $P=Q$, and the distance is $|\log(q/p)|$.

For [curves](../../../../../curve.md) stationary for the [energy of a curve](../../../../../energy-of-a-curve.md), fixed-endpoint variations give the Euler–Lagrange equations for $F=(\dot u^2+\dot v^2)/v^2$:

$$
\frac d{dt}\left(\frac{\dot u}{v^2}\right)=0,\qquad v\ddot v-\dot v^2+\dot u^2=0.
$$

Thus $\dot u=cv^2$ for a constant $c$. Since $u(1)-u(0)=0$, integration gives $c\int_0^1v^2dt=0$, hence $c=0$. The second equation then becomes $(\dot v/v)'=0$. Therefore

$$
\boxed{\gamma(t)=ip\exp\left[t\log(q/p)\right],\qquad \dot v/v=\log(q/p).}
$$

It has constant hyperbolic speed, is one of the absolute length minimizers, and also has minimum [energy of a curve](../../../../../energy-of-a-curve.md) $E=[\log(q/p)]^2$.

## ↑ Ancestors (10)

1. [12A](../12a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
