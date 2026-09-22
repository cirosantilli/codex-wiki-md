<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

For a satellite of [mass](../../../mass.md) $m$ moving in the [Newtonian gravitational field](../../../newtonian-gravitational-field.md) of a much larger, effectively fixed [mass](../../../mass.md) $M$, put $\mu=GM$. Its conserved [mechanical energy](../../../mechanical-energy.md), with [gravitational potential energy](../../../gravitational-energy.md) zero at infinity, is

$$
\boxed{E=\frac12mv^2-\frac{GMm}{r}=-\frac{GMm}{2a}.}
$$

Here $r$ is the instantaneous centre-to-centre [distance](../../../distance.md), $v$ the satellite's [speed](../../../speed.md), $G$ the [gravitational constant](../../../gravitational-constant.md), and $a$ the [semi-major axis](../../../semi-major-axis.md) of its bound [elliptic orbit](../../../elliptic-orbit.md). The [kinetic energy](../../../kinetic-energy.md) and [potential energy](../../../potential-energy.md) vary around the [orbit](../../../orbit-dynamical-system.md), while their sum remains constant. Dividing by $m$ and solving for $v$ gives the [vis-viva equation](../../../vis-viva-equation.md), $v^2=\mu(2/r-1/a)$.

For this [Hohmann transfer orbit](../../../hohmann-transfer-orbit.md), the [periapsis](../../../periapsis.md) and [apoapsis](../../../apoapsis.md) [distances](../../../distance.md) are $r_1=1\,\mathrm{AU}$ and $r_2=1.52\,\mathrm{AU}$, so

$$
a=\frac{r_1+r_2}{2}=1.26\,\mathrm{AU},\qquad
v_1=\sqrt{\frac{\mu}{r_1}}.
$$

The [vis-viva equation](../../../vis-viva-equation.md) gives the endpoint [speeds](../../../speed.md)

$$
\boxed{v_{\rm p}=v_1\sqrt{2-\frac1{1.26}}=v_1\sqrt{\frac{76}{63}},\qquad
v_{\rm a}=v_1\sqrt{\frac2{1.52}-\frac1{1.26}}.}
$$

As a check, [conservation of angular momentum](../../../conservation-of-angular-momentum.md) at the two endpoints gives $r_1v_{\rm p}=r_2v_{\rm a}$ because each [velocity](../../../velocity.md) is perpendicular to its radius. Using $1\,\mathrm{AU}=1.49598\times10^{11}\,\mathrm m$ and $\mu=1.32712\times10^{20}\,\mathrm{m^3\,s^{-2}}$ gives $v_1=29.78\,\mathrm{km\,s^{-1}}$ and

$$
\boxed{v_{\rm p}=32.71\,\mathrm{km\,s^{-1}},\qquad
v_{\rm a}=21.52\,\mathrm{km\,s^{-1}}.}
$$

The departure [impulse](../../../impulse.md) must increase the [speed](../../../speed.md) in the direction of the initial [circular orbit](../../../circular-orbit.md):

$$
\boxed{\Delta v_1=v_{\rm p}-v_1=2.93\,\mathrm{km\,s^{-1}}.}
$$

These are [Sun](../../../sun.md)-centred [speeds](../../../speed.md); leaving the [Earth](../../../earth.md)'s own [gravitational field](../../../gravitational-field.md) would require an additional calculation beyond this idealized solar [orbit](../../../orbit-dynamical-system.md) transfer.

At $r_2$, the desired [circular orbit](../../../circular-orbit.md) [speed](../../../speed.md) is $v_2=\sqrt{\mu/r_2}=24.16\,\mathrm{km\,s^{-1}}$. The arrival [impulse](../../../impulse.md) is therefore

$$
\boxed{\Delta v_2=v_2-v_{\rm a}=2.64\,\mathrm{km\,s^{-1}}.}
$$

The required thrust on the spacecraft is forward, tangent to its [orbit](../../../orbit-dynamical-system.md), to accelerate it. The rocket ejects exhaust backwards, opposite to the spacecraft's [velocity](../../../velocity.md); this distinguishes the direction of thrust from the direction in which the exhaust is fired.

The [Hohmann transfer time](../../../hohmann-transfer-time.md) is half the [orbital period](../../../orbital-period.md) of the transfer [ellipse](../../../ellipse.md). From [Kepler's third law](../../../kepler-s-third-law.md), relative to the [Earth](../../../earth.md)'s one-year [orbital period](../../../orbital-period.md),

$$
t_H=\frac12(1.26)^{3/2}\,\mathrm{yr}=0.7072\,\mathrm{yr}\simeq258\,\text{days}.
$$

Meanwhile [Mars](../../../mars.md)'s [orbital period](../../../orbital-period.md) is $T_M=1.52^{3/2}\,\mathrm{yr}=1.8740\,\mathrm{yr}$. The spacecraft arrives $\pi$ [radians](../../../radian.md) from its departure [position](../../../position.md). For a rendezvous, [Mars](../../../mars.md) must reach that same [position](../../../position.md) after advancing through $2\pi t_H/T_M$. Thus its initial lead [angle](../../../angle.md) over the departing spacecraft is

$$
\boxed{\phi_0=\pi-\frac{2\pi t_H}{T_M}
=\pi\left[1-\left(\frac{1.26}{1.52}\right)^{3/2}\right]
=44.15^\circ.}
$$

[Mars](../../../mars.md) must be ahead by this [angle](../../../angle.md) in the common direction of [motion](../../../motion.md) around their [orbits](../../../orbit-dynamical-system.md). At departure the spacecraft and the [Earth](../../../earth.md) share the inner [orbital position](../../../orbital-position.md); arrival occurs on the opposite side of the [Sun](../../../sun.md).

## ↑ Ancestors (11)

1. [8](../8.md)
2. [2021](../../2021-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
