<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take overdots in this question to mean differentiation with respect to the orbiting particle's [proper time](../../../../proper-time.md) $\tau$. Write $\mu=GM/c^2$, $x=r/\mu$ and $\ell=hc/(GM)$, with $h$ the [specific angular momentum](../../../../specific-angular-momentum.md). Then the dimensionless timelike effective potential is

$$
u(x)=\frac{U}{c^2}=-\frac1x+\frac{\ell^2}{2x^2}-\frac{\ell^2}{x^3}.
$$

The last term is the relativistic correction to the Newtonian centrifugal-plus-gravitational potential. At large $r$ the two agree. Newtonian [angular momentum](../../../../angular-momentum.md) gives an infinite inner [centrifugal barrier](../../../../centrifugal-barrier.md) for nonzero $h$; the relativistic correction lowers that barrier and permits plunge. The exterior problem starts at $r=2\mu$, where $U=-c^2/2$; extrapolating the potential towards $r=0$ is not a static exterior description.

Circular orbits obey

$$
U'=0\quad\Longleftrightarrow\quad GMr^2-h^2r+3\mu h^2=0,
\qquad h^2=\frac{GMr^2}{r-3\mu}.
$$

There are two extrema when $h^2>12(GM/c)^2$: an inner maximum representing an unstable circular orbit and an outer minimum representing a stable one. At equality they merge at $r=6\mu$; below it neither exists. More explicitly, evaluate the [curvature](../../../../curvature.md) at a circular orbit:

$$
\left.U''\right|_{\rm circ}=\frac{GM(r-6\mu)}{r^3(r-3\mu)}.
$$

Timelike circular orbits require $r>3\mu$. They are radially stable for $r>6\mu$, so **the marginally stable inner limit is $r_{\rm ISCO}=6GM/c^2$**. The Newtonian potential instead has one stable minimum at $r=h^2/(GM)$, without an [innermost stable circular orbit](../../../../innermost-stable-circular-orbit.md).

<a id="1/image-schwarzschild-and-newtonian-potentials"></a>
![](../../../../past-exam-of-the-relativistic-astrophysics-and-cosmology-course-of-the-university-of-cambridge/2012/paper-1-effective-potential.png)

**[Figure 1](#1/image-schwarzschild-and-newtonian-potentials). Schwarzschild and Newtonian potentials**.

For the [Schwarzschild circular-orbit local speed](../../../../schwarzschild-circular-orbit-local-speed.md) in the question, $\gamma$ is the [Lorentz factor](../../../../lorentz-factor.md) relative to a local [Schwarzschild static observer](../../../../schwarzschild-static-observer.md), not $dt/d\tau$. That observer's clock obeys $dT=\sqrt{1-2\mu/r}\,dt$. Since the particle passes with local speed $v$, $r\,d\phi/d\tau=\gamma v$. Circular normalization gives

$$
\frac{(r\dot\phi)^2}{c^2}=\frac{\mu}{r-3\mu},\qquad
\gamma^2=1+\frac{(r\dot\phi)^2}{c^2}=\frac{r-2\mu}{r-3\mu},
\qquad \frac{v^2}{c^2}=\frac{\mu}{r-2\mu}.
$$

Thus **$v=c/2$ at the [innermost stable circular orbit](../../../../innermost-stable-circular-orbit.md)**. Using [Schwarzschild time](../../../../schwarzschild-time.md) in place of the local clock would give a different speed.

For the conserved particle [energy](../../../../energy-split.md) measured at infinity, substitute $h^2$ in the circular [energy](../../../../energy-split.md) equation. Setting $y=\mu/r$ gives

$$
k^2=1-2y+\frac{y(1-2y)}{1-3y}
=\frac{(1-2y)^2}{1-3y},
\qquad\boxed{E=mc^2\frac{1-2\mu/r}{\sqrt{1-3\mu/r}}}.
$$

Take the positive root for a future-directed exterior orbit. It approaches $mc^2-GMm/(2r)$ at large radius. The [marginally bound circular Schwarzschild orbit](../../../../marginally-bound-circular-schwarzschild-orbit.md) solves $k=1$, giving $y(4y-1)=0$ and hence **$r_{\rm mb}=4GM/c^2$** at finite radius. It is unstable; strictly bound circular orbits have $r>4\mu$, with $E<mc^2$. The phrase smallest bound orbit here denotes this marginal circular limit, not a prohibition on a bound-energy trajectory plunging below it.

At the [innermost stable circular orbit](../../../../innermost-stable-circular-orbit.md),

$$
\boxed{E_{\rm ISCO}=\sqrt{\frac89}\,mc^2\simeq0.94281mc^2},\qquad
\eta=1-\sqrt{\frac89}\simeq\boxed{0.0572}.
$$

A radiatively efficient [thin disc](../../../../thin-disk.md) with a [zero-torque inner boundary condition](../../../../zero-torque-inner-boundary-condition.md) can therefore release about 5.7% of the accreted [rest energy](../../../../rest-energy.md) before the plunge. [energy](../../../../energy-split.md) advection, stress at the inner edge and [photon](../../../../photon.md) capture can alter the escaping [luminosity](../../../../luminosity.md), so this is a model efficiency rather than a universal emitted fraction.

For the [Kerr ISCO spin limits](../../../../kerr-isco-spin-limits.md) of an equatorial prograde disc around a rapidly rotating [Kerr black hole](../../../../kerr-black-hole.md), the [innermost stable circular orbit](../../../../innermost-stable-circular-orbit.md) moves inward and its specific [energy](../../../../energy-split.md) decreases. In the ideal extremal limit its Boyer-Lindquist radius tends to $\mu$, $E/(mc^2)\to1/\sqrt3$, and the corresponding binding-energy efficiency tends to 42.3%. Retrograde rotation has the opposite trend: the extremal limit is $r_{\rm ISCO}=9\mu$, $E/(mc^2)=5/(3\sqrt3)$, giving about 3.8%. The prograde limiting coordinate radius does not identify a massive orbit with the null horizon generator.[§II, Eqs. 2.20–2.23 and Fig. 1, pp. 351–353](../../../../rotating-black-holes-locally-nonrotating-frames-energy-extraction-and-scalar-synchrotron-radiation-by-james-m-bardeen-and-others.md)

Finally $\dot t=k/(1-2\mu/r)=1/\sqrt{1-3\mu/r}$. Dividing $\dot\phi=h/r^2$ by this gives

$$
\boxed{\Omega_\infty=\frac{d\phi}{dt}=\sqrt{\frac{GM}{r^3}}}.
$$

Its algebraic form is exactly Newtonian, but $r$ is the [Schwarzschild spacetime](../../../../schwarzschild-spacetime-split.md) [areal radius](../../../../areal-radius.md) and $t$ [Schwarzschild time](../../../../schwarzschild-time.md), normalized at infinity. Local clock rates, orbit stability and [binding energy](../../../../binding-energy.md) remain relativistic. With $GM_\odot\simeq1.3271\times10^{20}\,\mathrm{m^3\,s^{-2}}$,

$$
\boxed{f_{\rm ISCO,\infty}=\frac{c^3}{2\pi6^{3/2}G(10M_\odot)}\simeq0.220\,\mathrm{kHz}},
\qquad\boxed{\frac{f_{\rm ISCO}}{f_{\rm mb}}=\left(\frac46\right)^{3/2}\simeq0.544}.
$$

The marginally bound circular-orbit [frequency](../../../../frequency.md) is about $0.404\,\mathrm{kHz}$. These [Schwarzschild ISCO orbital frequencies](../../../../schwarzschild-isco-orbital-frequency.md) and marginally bound [frequencies](../../../../frequency.md) are rotation [frequencies](../../../../frequency.md) per distant stationary observer's time, as intended by using $d\phi/dt$. A static observer at finite radius $r_o$ instead divides both [frequencies](../../../../frequency.md) by $\sqrt{1-2\mu/r_o}$, leaving their ratio unchanged. Identifying an observed [quasi-periodic oscillation](../../../../quasi-periodic-oscillation.md) with the [innermost stable circular orbit](../../../../innermost-stable-circular-orbit.md) orbital [frequency](../../../../frequency.md) is an additional astrophysical assumption.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2012](../../split.md)
4. [Past exam of the relativistic Astrophysics and Cosmology course of the University of Cambridge](../../../split.md)
5. [Relativistic Astrophysics and Cosmology course of the University of Cambridge](../../../../relativistic-astrophysics-and-cosmology-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
