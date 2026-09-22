<h1 id="section-b/b5/solution">Solution</h1>

↑ **Parent:** [B5](../b5.md)

Write $A(r)=1-2\mu/r$, with $\mu=GM/c^2$. On the equatorial plane, the [geodesic Lagrangian](../../../../geodesic-lagrangian.md) is

$$
L=\frac12\left(c^2A\dot t^2-A^{-1}\dot r^2-r^2\dot\phi^2\right).
$$

The coordinates $t$ and $\phi$ are cyclic, giving $\boxed{A\dot t=k,\quad r^2\dot\phi=h}$. The conserved physical [energy](../../../../energy-split.md) per unit [rest mass](../../../../invariant-mass.md) is $c^2k$, while $h$ is the signed [angular momentum](../../../../angular-momentum.md) per unit [rest mass](../../../../invariant-mass.md). The radial [Euler-Lagrange equation](../../../../euler-lagrange-equation.md), with $A'=2\mu/r^2$, is

$$
\boxed{A^{-1}\ddot r+\frac{\mu c^2}{r^2}\dot t^2
-\frac{\mu}{r^2A^2}\dot r^2-r\dot\phi^2=0.}
$$

These are the requested [geodesic equations](../../../../geodesic-equation.md). The equatorial condition is consistent with the polar equation by the spherical symmetry of the [Schwarzschild metric](../../../../schwarzschild-spacetime-split.md).

The normalization of the [four-velocity](../../../../four-velocity.md) is $c^2=c^2A\dot t^2-A^{-1}\dot r^2-r^2\dot\phi^2$. Insert the two conserved quantities and multiply by $A$ to obtain

$$
\boxed{\dot r^2+\frac{h^2}{r^2}\left(1-\frac{2\mu}r\right)-\frac{2\mu c^2}r
=c^2(k^2-1).}
$$

This is a one-dimensional radial energy equation. Half of its left side is radial kinetic energy per unit mass plus an [effective potential](../../../../effective-potential.md): the Newtonian centrifugal and gravitational terms acquire the extra attractive contribution $-\mu h^2/r^3$.

A [timelike circular Schwarzschild geodesic](../../../../timelike-circular-schwarzschild-geodesic.md) requires $\dot r=\ddot r=0$. Equivalently, set the derivative of $V(r)=h^2/r^2-2\mu h^2/r^3-2\mu c^2/r$ to zero. At $r=R$ this gives $h^2(R-3\mu)=\mu c^2R^2$, and substitution in the radial energy equation yields

$$
\boxed{h^2=\frac{\mu c^2R^2}{R-3\mu},\qquad
k^2=\frac{(R-2\mu)^2}{R(R-3\mu)}.}
$$

Such timelike circular orbits require $R>3\mu$. Their coordinate [angular velocity](../../../../angular-velocity.md) satisfies $\Omega^2=\mu c^2/R^3$, and their proper clock rate is $d\tau_s/dt=A/k=\sqrt{1-3\mu/R_s}$.

For the static North-Pole clock, $d\tau_E/dt=\sqrt{1-2\mu/R_E}$. Consecutive overhead passages occur one coordinate orbital period apart, and the repeated Earth-satellite geometry gives equal signal travel delays. The [comparison of circular-orbit and static Schwarzschild clocks](../../../../comparison-of-circular-orbit-and-static-schwarzschild-clocks.md) therefore gives

$$
\boxed{\frac{\tau_s}{\tau_E}=\sqrt{\frac{1-3\mu/R_s}{1-2\mu/R_E}}.}
$$

This includes both gravitational and orbital-motion effects; a separate Newtonian time-dilation correction must not be added again.

For an estimate, [Kepler's third law](../../../../kepler-s-third-law.md) gives $R_s=42100\,\mathrm{km}\,(3/24)^{2/3}=10525\,\mathrm{km}$. The same approximate geostationary radius and period give $\mu=4\pi^2R_{\rm geo}^3/(c^2T_{\rm geo}^2)\simeq4.4\,\mathrm{mm}$. Expanding the ratio to first order,

$$
\frac{\tau_s}{\tau_E}\simeq1+\frac\mu{R_E}-\frac{3\mu}{2R_s}
\simeq\boxed{1+6.4\times10^{-11}}.
$$

The satellite clock consequently gains about $0.7\,\mu\mathrm s$ over a three-hour orbit in this approximation. The surface observer is taken to be static, and the spacetime model is the spherical [Schwarzschild metric](../../../../schwarzschild-spacetime-split.md) specified in the problem.

## ↑ Ancestors (13)

1. [B5](../b5.md)
2. [Section B](../../section-b.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the relativity course of the University of Cambridge](../../../split.md)
5. [Relativity course of the University of Cambridge](../../../../relativity-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
