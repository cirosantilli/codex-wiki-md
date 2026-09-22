<h1 id="3c/solution">Solution</h1>

↑ **Parent:** [3C](../3c.md)

Outside a spherical planet, [Newtonian mechanics](../../../../../newtonian-mechanics.md) gives the inverse-square [central force](../../../../../central-force.md) equation

$$
\ddot{\mathbf r}=-\frac{GM}{r^3}\mathbf r.
$$

The satellite's mass cancels. The [angular momentum](../../../../../angular-momentum.md) is conserved, so the orbit lies in a plane. In that plane the general equations in [polar coordinates](../../../../../polar-coordinates.md) are

$$
\ddot r-r\dot\theta^2=-\frac{GM}{r^2},\qquad
r\ddot\theta+2\dot r\dot\theta=0.
$$

A [synchronous circular orbit](../../../../../synchronous-circular-orbit.md) fixed above a surface point must be equatorial, prograde and have [angular velocity](../../../../../angular-velocity.md) $\omega=2\pi/T$. Substitution of constant $r$ into the radial equation gives

$$
\boxed{r_s=\left(\frac{GMT^2}{4\pi^2}\right)^{1/3},\qquad
v_s=\frac{2\pi r_s}{T}=\left(\frac{2\pi GM}{T}\right)^{1/3}.}
$$

The radius is measured from the planet's centre; an external orbit requires it to exceed the planet's radius.

Now let the release speed be $v=(1+\eta)v_s$, with $0<\eta\ll1$, in the same tangential direction. At release $\dot r=0$, but

$$
\ddot r(0)=\frac{v^2-v_s^2}{r_s}>0.
$$

Thus the satellite initially moves outward. Its specific total [energy](../../../../../energy.md) is $v^2/2-GM/r_s<0$ for this small increase, so the [Kepler orbit](../../../../../kepler-orbit.md) is an [ellipse](../../../../../ellipse.md), with the release point its [pericentre](../../../../../periapsis.md). To make this explicit, put $b=v^2/v_s^2\in(1,2)$. The radial turning-point equation from energy and [angular momentum](../../../../../angular-momentum.md) conservation has roots

$$
r_{{\min}}=r_s,\qquad r_{{\max}}=\frac{b}{2-b}r_s.
$$

Its [semi-major axis](../../../../../semi-major-axis.md) is $a=r_s/(2-b)>r_s$. The speed follows from the same conserved energy:

$$
v(r)^2=GM\left(\frac2r-\frac1a\right).
$$

**It is greatest at pericentre and least at apocentre.** In particular, the tangential speed at the two turning points satisfies $r_{{\min}}v_{{\max}}=r_{{\max}}v_{{\min}}$. The orbital period becomes $2\pi\sqrt{a^3/(GM)}>T$, so the orbit is no longer fixed over the same surface point.

## ↑ Ancestors (10)

1. [3C](../3c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
