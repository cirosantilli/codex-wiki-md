<h1 id="section-b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

**Definitions**. The [torque](../../../../torque.md) of a [force](../../../../force-split.md) $\mathbf F$ about an origin is $\boldsymbol\tau=\mathbf r\times\mathbf F$, where $\mathbf r$ runs from that origin to the force's point of application. Its component about a fixed axis changes [angular momentum](../../../../angular-momentum.md) about that axis. The [moment of inertia](../../../../moment-of-inertia.md) about that axis is

$$
\boxed{I=\int s^2\,dm,}
$$

where $s$ is perpendicular distance to the axis. It measures resistance to [angular acceleration](../../../../angular-acceleration.md); for fixed-axis rigid rotation, $\tau_{\rm net}=I\alpha$. The units are $\mathrm{N\,m}$ for [torque](../../../../torque.md) and $\mathrm{kg\,m^2}$ for [moment of inertia](../../../../moment-of-inertia.md).

**Mass and axial inertia**. Slice the shaft perpendicular to its common axis. A slice of radius $r(z)$ has [mass](../../../../mass.md) $dm=\rho\pi r(z)^2dz$ and [moment of inertia](../../../../moment-of-inertia.md) $dI=\tfrac12r(z)^2dm$, using the [moment of inertia of a uniform disc](../../../../moment-of-inertia-of-a-uniform-disc.md). Thus the [axial moment of inertia of a solid of revolution](../../../../axial-moment-of-inertia-of-a-solid-of-revolution.md) uses the second and fourth powers of its radius:

$$
M=\rho\pi\int r(z)^2dz,\qquad
I=\frac{\rho\pi}{2}\int r(z)^4dz.
$$

For the tapered section, take $z$ from its narrow end toward its wide end, so $r(z)=a(1+z/l)$ for $0\leq z\leq l$. Its contributions are

$$
M_{\rm taper}=\rho\pi a^2l\int_0^1(1+u)^2du
=\frac73\rho\pi a^2l,
\qquad
I_{\rm taper}=\frac{\rho\pi a^4l}{2}\int_0^1(1+u)^4du
=\frac{31}{10}\rho\pi a^4l.
$$

The two cylinders contribute $4\rho\pi a^2l$ and $\rho\pi a^2l$ to [mass](../../../../mass.md), and $8\rho\pi a^4l$ and $\tfrac12\rho\pi a^4l$ to [moment of inertia](../../../../moment-of-inertia.md). Adding the three sections gives

$$
\boxed{M=\left(4+\frac73+1\right)\rho\pi a^2l
=\frac{22}{3}\rho\pi a^2l,}
$$



$$
I=\left(8+\frac{31}{10}+\frac12\right)\rho\pi a^4l
=\frac{58}{5}\rho\pi a^4l,
\qquad
\boxed{I=\frac{58/5}{22/3}Ma^2=\frac{87}{55}Ma^2.}
$$

All slice rotation axes coincide with the shaft axis, so the moments add directly.

**Frictional torque**. The normal load on the narrow circular end is $Mg$. With the stipulated uniform [pressure](../../../../pressure-split.md), $p_N=Mg/(\pi a^2)$. A contact annulus of radius $s$ and width $ds$ has area $dA=2\pi s\,ds$, normal [force](../../../../force-split.md) $p_NdA$ and tangential [kinetic friction](../../../../kinetic-friction.md) $dF=\mu p_NdA$. Multiplying by its lever arm $s$ and integrating gives the [uniform-pressure friction torque on a circular contact](../../../../uniform-pressure-friction-torque-on-a-circular-contact.md):

$$
G_f=\int_0^a s\,\mu\frac{Mg}{\pi a^2}\,2\pi s\,ds
=\frac{2\mu Mg}{a^2}\frac{a^3}{3},
\qquad
\boxed{G_f=\frac{2M\mu ga}{3}.}
$$

Here $G_f$ is the positive magnitude; its [torque](../../../../torque.md) opposes the [angular velocity](../../../../angular-velocity.md).

**Steady speed and stopping rotations**. Mechanical [power](../../../../power.md) in rotation is $P=\tau\omega$. At steady [angular velocity](../../../../angular-velocity.md), the driving and frictional torques balance, so [constant-power rotation against dry friction](../../../../constant-power-rotation-against-dry-friction.md) gives

$$
\boxed{\omega_*=\frac{P}{G_f}=\frac{3P}{2M\mu ga}.}
$$

Using $g=9.81\,\mathrm{m\,s^{-2}}$ and $a=0.100\,\mathrm m$,

$$
I=0.0316364\,\mathrm{kg\,m^2},\qquad
G_f=0.3924\,\mathrm{N\,m},\qquad
\boxed{\omega_*=25.4842\,\mathrm{rad\,s^{-1}}\simeq25.5\,\mathrm{rad\,s^{-1}}.}
$$

Once the motor is removed, the speed-independent [kinetic friction](../../../../kinetic-friction.md) gives constant [angular acceleration](../../../../angular-acceleration.md) $-G_f/I$. Equivalently, the initial [rotational kinetic energy](../../../../rotational-kinetic-energy.md) is dissipated as frictional work. The [stopping angle under constant resisting torque](../../../../stopping-angle-under-constant-resisting-torque.md) is therefore

$$
G_f\Delta\phi=\frac12I\omega_*^2,\qquad
\Delta\phi=\frac{I\omega_*^2}{2G_f}=26.1800\,\mathrm{rad}.
$$

The total [angular displacement](../../../../angular-displacement.md) corresponds to

$$
N=\frac{\Delta\phi}{2\pi}=\frac{IP^2}{4\pi G_f^3}=4.16668\ \text{revolutions}.
$$

Hence the shaft completes

$$
\boxed{\lfloor N\rfloor=4\ \text{complete rotations},}
$$

and then another $0.16668$ of a rotation. Its stopping time is $I\omega_*/G_f=2.05461\,\mathrm s$. Using the rounded value $g=9.8\,\mathrm{m\,s^{-2}}$ changes the fractional rotation slightly but leaves four complete rotations.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [Section B](../../section-b.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
