<h1 id="section-c/10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

**Axial moment of inertia.** In the original diagram $R_1$ is the outer radius and $R_2$ the inner radius. For uniform [mass density](../../../../density.md) $\rho$, a coaxial annulus of thickness $dr$ has $dm=2\pi\rho Lr\,dr$. Therefore the [axial moment of inertia of a hollow cylinder](../../../../axial-moment-of-inertia-of-a-hollow-cylinder.md) is

$$
I=\int_{R_2}^{R_1}r^2dm
=2\pi\rho L\int_{R_2}^{R_1}r^3\,dr
=\frac{\pi\rho L}{2}(R_1^4-R_2^4).
$$

Since $M=\pi\rho L(R_1^2-R_2^2)$, factorizing the fourth-power difference gives

$$
\boxed{I=\frac12M(R_1^2+R_2^2).}
$$

For a solid cylinder $R_2\to0$, giving **$I=MR_1^2/2$**. For a thin cylindrical shell with fixed [mass](../../../../mass.md) and $R_1,R_2\to R$, **$I=MR^2$**. The latter limit agrees with every mass element being at radius $R$.

**Undamped rolling oscillations.** Let $x$ be axle [displacement](../../../../displacement.md) from the [spring](../../../../spring.md) equilibrium. [Rolling without slipping](../../../../rolling-without-slipping.md) imposes $|\omega_{\rm roll}|=|\dot x|/R$. The sum of translational and [rotational kinetic energy](../../../../rotational-kinetic-energy.md) is

$$
T=\frac12m\dot x^2+\frac12I\frac{\dot x^2}{R^2}
=\frac12\left(m+\frac I{R^2}\right)\dot x^2.
$$

The [potential energy](../../../../potential-energy.md) is $U=kx^2/2$. Differentiating $T+U$ in the absence of [damping](../../../../damping.md), or applying the force and torque equations below, gives

$$
\left(m+\frac I{R^2}\right)\ddot x+kx=0.
$$

For the thin shell $I=mR^2$, the effective inertia is $2m$, and the [angular frequency](../../../../angular-frequency.md) of the [simple harmonic motion](../../../../simple-harmonic-motion.md) is

$$
\boxed{\omega_0=\sqrt{\frac{k}{2m}}.}
$$

Static contact [friction](../../../../friction.md) supplies the required [torque](../../../../torque.md) but does no work when the contact point is instantaneously stationary.

**Damped force balance.** Take rightward [force](../../../../force-split.md) as positive and counterclockwise rotation as positive. Write $f$ for the signed [static friction](../../../../static-friction.md) at the bottom contact. Then

$$
m\ddot x=-kx-b\dot x+f,\qquad
I\alpha=fR,\qquad\alpha=-\frac{\ddot x}{R}.
$$

Eliminate $f=-I\ddot x/R^2$ and use $I=mR^2$:

$$
2m\ddot x+b\dot x+kx=0,
\qquad
\boxed{\ddot x+B\dot x+Cx=0,\qquad B=\frac b{2m},\quad C=\frac k{2m}.}
$$

Here $b$ has units $\mathrm{kg\,s^{-1}}$, so $B$ has units $\mathrm{s^{-1}}$ and $C$ units $\mathrm{s^{-2}}$. The stated [drag force](../../../../drag-physics.md) is interpreted as acting through the axle, with no additional viscous [torque](../../../../torque.md). An oil bath could also exert such a torque physically, but its magnitude is not specified by this force-only model.

**Light damping.** Substitution of $z=Ae^{-pt}$ into the differential equation gives $p^2-Bp+C=0$. In the [underdamped](../../../../underdamping.md) regime $B^2<4C$,

$$
p=\frac B2\pm i\sqrt{C-\frac{B^2}{4}}
=\frac b{4m}\pm i\omega_d,
\qquad
\omega_d=\sqrt{\frac{k}{2m}-\frac{b^2}{16m^2}}.
$$

Taking real linear combinations gives the general [damped harmonic oscillator](../../../../damped-harmonic-oscillator.md) displacement

$$
\boxed{x(t)=e^{-bt/(4m)}[A_1\cos(\omega_dt)+A_2\sin(\omega_dt)].}
$$

The constants are fixed by the initial [displacement](../../../../displacement.md) and [velocity](../../../../velocity.md). For example, release from rest at $x_0$ gives $A_1=x_0$ and $A_2=bx_0/(4m\omega_d)$. Light damping means $b^2\ll8mk$, in which case $\omega_d\simeq\omega_0$ and the envelope decays slowly compared with an oscillation.

## ↑ Ancestors (12)

1. [10](../10.md)
2. [Section C](../../section-c.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
