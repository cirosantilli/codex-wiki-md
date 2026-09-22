<h1 id="6c/solution">Solution</h1>

↑ **Parent:** [6C](../6c.md)

The [divergence](../../../../../divergence.md) is $\partial_x(kty)+\partial_y0+\partial_z0=0$, so this is an [incompressible flow](../../../../../incompressible-flow.md). With the planar convention $(u,v)=(\psi_y,-\psi_x)$, one [stream function](../../../../../stream-function.md) is

$$
\boxed{\psi(x,y,t)=\frac12kty^2}.
$$

At a fixed nonzero $kt$, the [streamlines](../../../../../streamline.md) have $y=\mathrm{constant}$ and $z=\mathrm{constant}$, since the instantaneous [velocity](../../../../../velocity.md) is purely axial. If $kt=0$, every point is instantaneously stationary and there is no distinguished [streamline](../../../../../streamline.md) direction.

Follow a marked particle initially at $(0,y_0,0)$. Its trajectory satisfies $\dot y=\dot z=0$ and $\dot x=kty_0$, so

$$
(x,y,z)=\left(\frac12kt^2y_0,y_0,0\right),\qquad0\leq y_0\leq a.
$$

These points form a straight segment on $x=(kt^2/2)y$, $z=0$, not an instantaneous horizontal [streamline](../../../../../streamline.md). Its length is

$$
\boxed{\ell(t)=a\sqrt{1+\frac14k^2t^4}}.
$$

The directed angle of its vector from the origin to the marked endpoint is

$$
\boxed{\theta(t)=\operatorname{atan2}(1,kt^2/2)}.
$$

For $k>0$ and $t>0$, this is $\arctan[2/(kt^2)]$; it equals $\pi/2$ at $t=0$. If an unoriented acute angle to the axis is intended, use $\arctan[2/(|k|t^2)]$, with $\pi/2$ when $kt=0$. This distinction handles a negative value of the given constant as well. If $a=0$, the marked set is a single point: the length formula gives zero and no line direction is defined.

## ↑ Ancestors (10)

1. [6C](../6c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
