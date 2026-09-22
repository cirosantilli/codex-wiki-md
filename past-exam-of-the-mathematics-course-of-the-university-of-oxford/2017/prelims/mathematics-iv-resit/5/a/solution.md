<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use $g$ as the [gravitational acceleration](../../../../../../gravitational-acceleration.md), so the weights are $mg$ and $\sqrt2mg$, consistently with the requested equations. The printed introductory phrase calling $g$ a [force](../../../../../../force-split.md) magnitude omits the factor $m$.

For the [particle on a cone coupled to a hanging mass](../../../../../../particle-on-a-cone-coupled-to-a-hanging-mass.md), write $z=-r$ and use the [cylindrical coordinates](../../../../../../cylindrical-coordinate-system.md) [unit vectors](../../../../../../unit-vector.md) $\mathbf e_r,\mathbf e_\theta,\mathbf e_z$. The [ideal string](../../../../../../massless-inextensible-string.md) segment from the cone particle to the hole has length $\sqrt2r$ and direction $(-\mathbf e_r+\mathbf e_z)/\sqrt2$. If $h$ is the downward length of the hanging segment and $s_0$ the fixed total length, then

$$
h=s_0-\sqrt2r=s_0+\sqrt2z,\qquad z_2=-h=-s_0-\sqrt2z.
$$

The light [ideal string](../../../../../../massless-inextensible-string.md) and smooth hole give the same [tension](../../../../../../tension.md) $T$ on both sides. Applying the vertical component of [Newton's second law](../../../../../../newton-s-second-law.md) to the hanging particle gives

$$
\sqrt2m\ddot z_2=T-\sqrt2mg,
\qquad\boxed{T=\sqrt2mg-2m\ddot z.}
$$

Write the [normal reaction](../../../../../../normal-force.md) on the cone particle as $N(\mathbf e_r+\mathbf e_z)/\sqrt2$, allowing $N$ to be signed according to the side of the ideal constraining [surface](../../../../../../topological-surface-split.md). The [acceleration in cylindrical coordinates](../../../../../../acceleration-in-cylindrical-coordinates.md) and [Newton's second law](../../../../../../newton-s-second-law.md) give

$$
\begin{aligned}
m(\ddot r-r\dot\theta^2)&=\frac{N-T}{\sqrt2},\\
m(r\ddot\theta+2\dot r\dot\theta)&=0,\\
m\ddot z&=\frac{N+T}{\sqrt2}-mg.
\end{aligned}
$$

There is no azimuthal [force](../../../../../../force-split.md). Multiplying the middle equation by $r/m$ proves

$$
\frac{d}{dt}(r^2\dot\theta)=0,\qquad
\boxed{r^2\dot\theta=av,}
$$

where the positive angular direction is chosen along the initial [velocity](../../../../../../velocity.md). This is [conservation of angular momentum](../../../../../../conservation-of-angular-momentum.md) about the vertical axis.

Subtract the radial equation from the vertical equation to eliminate the [normal reaction](../../../../../../normal-force.md). Since $\ddot r=-\ddot z$, this gives

$$
m(2\ddot z+r\dot\theta^2)=\sqrt2T-mg.
$$

Substitute the [tension](../../../../../../tension.md) and the conserved [angular momentum](../../../../../../angular-momentum.md), using $r=-z$:

$$
2(1+\sqrt2)\ddot z=g-r\dot\theta^2
=g+\frac{a^2v^2}{z^3}.
$$

Multiplication by $\dot z$ now gives an exact time [derivative](../../../../../../derivative.md):

$$
\frac{d}{dt}\left((1+\sqrt2)\dot z^2+\frac{a^2v^2}{2z^2}-gz\right)=0.
$$

Initially $z=-a$ and $\dot z=0$, because the initial [velocity](../../../../../../velocity.md) is horizontal. Therefore

$$
\boxed{(1+\sqrt2)\dot z^2+\frac{a^2v^2}{2z^2}-gz=\frac{v^2}{2}+ga.}
$$

This is also total [mechanical energy](../../../../../../mechanical-energy.md) divided by $m$, with an irrelevant constant removed: the two particles contribute $(1+\sqrt2)m\dot z^2$ to the radial and vertical [kinetic energy](../../../../../../kinetic-energy.md), while their combined [gravitational potential energy](../../../../../../gravitational-energy.md) is $-mgz$ plus a constant.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [Mathematics IV resit](../../../mathematics-iv-resit-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
