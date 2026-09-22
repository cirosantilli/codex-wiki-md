<h1 id="12c/solution">Solution</h1>

↑ **Parent:** [12C](../12c.md)

For a [Lorentz transformation](../../../../../lorentz-transformation.md) to an [inertial frame](../../../../../inertial-frame.md) moving at speed $v_B$ in the positive $x$ direction, write $\beta_B=v_B/c$ and $\Gamma_B=(1-\beta_B^2)^{-1/2}$. Any [four-vector](../../../../../four-vector.md) transforms as

$$
\boxed{W'^0=\Gamma_B(W^0-\beta_BW^1),\quad W'^1=\Gamma_B(W^1-\beta_BW^0),\quad W'^2=W^2,\quad W'^3=W^3.}
$$

This convention applies to $X=(ct,x,0,0)$ and uses the same $+---$ [Minkowski metric](../../../../../minkowski-metric.md) as the [four-momentum](../../../../../four-momentum.md) calculation.

The definition of [proper time](../../../../../proper-time.md) gives $d\tau=dt\sqrt{1-u^2/c^2}=dt/\gamma$ for $|u|<c$. Hence the [four-velocity](../../../../../four-velocity.md) is

$$
\boxed{U=\gamma(c,u).}
$$

Since $\dot\gamma=\gamma^3u\dot u/c^2$, differentiating with respect to [proper time](../../../../../proper-time.md) gives

$$
A=\gamma\frac{dU}{dt}=\left(\frac{\gamma^4u\dot u}{c},\gamma^2\dot u+\frac{\gamma^4u^2\dot u}{c^2}\right)=\boxed{\gamma^4\dot u\,(u/c,1)}.
$$

Here $1+\gamma^2u^2/c^2=\gamma^2$ simplifies the spatial component of the [four-acceleration](../../../../../four-acceleration.md).

At each event, boost with $v_B=u$ to the instantaneous rest [inertial frame](../../../../../inertial-frame.md). Then $A'^0=0$ and $A'^1=\gamma\gamma^4\dot u(1-u^2/c^2)=\gamma^3\dot u$. Thus the signed [proper acceleration for one-dimensional motion](../../../../../proper-acceleration-for-one-dimensional-motion.md) is

$$
\boxed{a=\gamma^3\dot u=\frac d{dt}(\gamma u).}
$$

The last equality follows by differentiating $\gamma u$; its magnitude is the usual scalar [proper acceleration](../../../../../proper-acceleration.md).

If this signed [proper acceleration](../../../../../proper-acceleration.md) is constant and the particle starts from rest, integration gives $\gamma u=at$, so

$$
u(t)=\frac{at}{\sqrt{1+a^2t^2/c^2}}.
$$

Integrating once more and imposing $x(0)=0$ yields the [hyperbolic motion](../../../../../hyperbolic-motion.md) worldline

$$
\boxed{x(t)=\frac{c^2}{a}\left(\sqrt{1+\frac{a^2t^2}{c^2}}-1\right)\quad(a\ne0).}
$$

For $a=0$ the continuous limiting solution is $x=0$. Finally, the [Taylor series](../../../../../taylor-series.md) of the square root gives

$$
x(t)=\frac12at^2-\frac{a^3t^4}{8c^2}+O(a^5t^6/c^4),\qquad \boxed{x\sim\frac12at^2\quad\text{when }|at|\ll c.}
$$

This recovers constant-acceleration [Newtonian mechanics](../../../../../newtonian-mechanics.md) at low speed while the exact relativistic speed remains less than $c$.

## ↑ Ancestors (10)

1. [12C](../12c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
