<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use [geometrized units](../../../../../geometrized-units.md) $G=c=1$ until converting the clock readings. By the [Birkhoff theorem](../../../../../birkhoff-s-theorem.md), the spherical vacuum exterior is a portion of the [Schwarzschild spacetime](../../../../../schwarzschild-spacetime.md) with fixed mass $M$:

$$
\boxed{ds^2_{\rm out}=-\left(1-\frac{2M}{r}\right)dt^2+\left(1-\frac{2M}{r}\right)^{-1}dr^2+r^2d\Omega^2,\qquad r>R(\tau).}
$$

The exterior is not flat and is not radiating merely because the surface moves. When the surface crosses $r=2M$, this exterior must be represented in regular [Ingoing Eddington-Finkelstein coordinates](../../../../../ingoing-eddington-finkelstein-coordinates.md), rather than treating the Schwarzschild-coordinate divergence as a physical barrier.

The [Oppenheimer-Snyder model](../../../../../oppenheimer-snyder-model.md) has a homogeneous [pressureless matter](../../../../../pressureless-matter.md) interior. Since its initial expansion vanishes but its [density](../../../../../density.md) is positive, the [Friedmann equation](../../../../../friedmann-equations.md) requires positive spatial curvature. Choose a comoving radial angle $\chi$ and the boundary's [proper time](../../../../../proper-time.md) $\tau$, with the stopwatch set to zero at release. The interior [FLRW metric](../../../../../friedmann-lemaitre-robertson-walker-metric.md) and [density](../../../../../density.md) are

$$
\boxed{ds^2_{\rm in}=-d\tau^2+a(\tau)^2\bigl(d\chi^2+\sin^2\chi\,d\Omega^2\bigr),\qquad0\le\chi\le\chi_0,}
\qquad \rho(\tau)=\rho_0\left(\frac{a_{\max}}a\right)^3.
$$

The [density](../../../../../density.md) law follows from the [dust stress-energy tensor](../../../../../dust-stress-energy-tensor.md) and its covariant conservation. The [Friedmann equation](../../../../../friedmann-equations.md) and the initial rest condition give

$$
\dot a^2+1=\frac{8\pi}3\rho a^2=\frac{a_{\max}}a,\qquad \frac{8\pi}3\rho_0a_{\max}^2=1.
$$

Its contracting branch has the parameterization

$$
a=\frac{a_{\max}}2(1+\cos\eta),\qquad
\tau=\frac{a_{\max}}2(\eta+\sin\eta),\qquad0\le\eta<\pi.
$$

Indeed $d\tau/d\eta=a$ and $\dot a=-\sin\eta/(1+\cos\eta)$ satisfy the displayed equation; $\eta=0$ is the turning point and $\eta=\pi$ is the final [curvature singularity](../../../../../curvature-singularity.md).

For [homogeneous dust-ball matching](../../../../../homogeneous-dust-ball-matching.md), the boundary has [areal radius](../../../../../areal-radius.md) $R=a\sin\chi_0$. Matching its mass to the exterior gives

$$
M=\frac{4\pi}3\rho R^3=\frac{a_{\max}}2\sin^3\chi_0,\qquad
\sin^2\chi_0=\frac{2M}{R_0},\qquad
\boxed{a_{\max}=\sqrt{\frac{R_0^3}{2M}}.}
$$

This $M$ is the gravitational mass parameter, not the integral of rest [density](../../../../../density.md) over the curved proper-volume element. The matching can also be checked directly. The outward angular [extrinsic curvature](../../../../../extrinsic-curvature.md) inside is $K_{\theta\theta}=R\cos\chi_0$; outside it is $R\sqrt{1-2M/R+\dot R^2}$. The boundary motion has

$$
\dot R^2=\frac{2M}{R}-\frac{2M}{R_0},\qquad E=\sqrt{1-\frac{2M}{R_0}}=\cos\chi_0,
$$

so these curvatures agree. The induced metric is $-d\tau^2+R^2d\Omega^2$ on both sides and $K_{\tau\tau}=0$ because the pressure-free boundary is geodesic. No artificial surface stress layer is required.

The observer moving with this boundary meets the [event horizon](../../../../../event-horizon.md) when $R=2M$. From $R=R_0(1+\cos\eta)/2$, the [proper-time horizon crossing in homogeneous dust collapse](../../../../../proper-time-horizon-crossing-in-homogeneous-dust-collapse.md) occurs at

$$
\eta_H=2\arccos\sqrt{\frac{2M}{R_0}}=\pi-2\chi_0,
\qquad
\tau_H=\frac{a_{\max}}2(\eta_H+\sin\eta_H).
$$

The singularity is reached at $\tau_s=\pi a_{\max}/2$, so the remaining clock time is

$$
\Delta\tau=\tau_s-\tau_H=\frac{a_{\max}}2(\pi-\eta_H-\sin\eta_H).
$$

These are finite [proper times](../../../../../proper-time.md), even though the external static time diverges at horizon crossing.

Convert the supplied rounded units consistently: $M=10^{38}$ [Planck masses](../../../../../planck-mass.md) and $R_0=6.25\times10^{39}$ [Planck lengths](../../../../../planck-length.md). Thus $2M/R_0=0.032$, $\chi_0\simeq0.17985$, and $a_{\max}\simeq3.4939\times10^{40}$ in [Planck units](../../../../../planck-units.md). Multiplying geometric times by $5\times10^{-44}$ seconds gives

$$
\boxed{\tau_H\simeq2.737\times10^{-3}\ {\rm s},\qquad
\tau_s\simeq2.744\times10^{-3}\ {\rm s},\qquad
\Delta\tau\simeq6.73\times10^{-6}\ {\rm s}.}
$$

At the accuracy justified by the rounded constants, these are **about three milliseconds to horizon crossing and about seven microseconds more to the singularity**. For $R_0\gg2M$, expanding $\eta_H=\pi-2\chi_0$ gives $\Delta\tau\simeq(2/3)a_{\max}\chi_0^3\simeq4M/3$, independently confirming the microsecond scale. The exact expression above retains the finite release-radius correction.

Strictly, this boundary clock reading is when the observer crosses the horizon, not when the horizon first exists anywhere. The [event horizon inside an Oppenheimer-Snyder cloud](../../../../../event-horizon-inside-an-oppenheimer-snyder-cloud.md) is an outgoing radial null ray. Since $d\tau=a\,d\eta$, the interior metric is conformal to $-d\eta^2+d\chi^2+\sin^2\chi\,d\Omega^2$, and that ray has $d\chi/d\eta=1$. Tracing it back from $(\eta_H,\chi_0)$ gives

$$
\chi_{\mathcal H}=\eta-\eta_H+\chi_0,\qquad \eta_{\rm birth}=\eta_H-\chi_0=\pi-3\chi_0.
$$

For this cloud it starts at the centre after release, at comoving time $\tau_{\rm birth}\simeq2.722\times10^{-3}$ seconds. This answers the literal global-formation interpretation as well; it is not an event on the outer observer's worldline. The distinction matters because an [event horizon](../../../../../event-horizon.md) is defined by the entire future causal escape problem, not by a locally detectable signal of formation.

For the observer at infinity, use the boundary's conserved [Killing energy](../../../../../killing-energy.md) $E$ in the exterior:

$$
\frac{dt}{d\tau}=\frac{E}{1-2M/R}.
$$

As $\tau\uparrow\tau_H$, $\dot R\to-E$ and $R-2M\simeq E(\tau_H-\tau)$. Consequently

$$
t=-2M\log\left(\frac{\tau_H-\tau}{\tau_*}\right)+O(1)\longrightarrow+\infty,
$$

where $\tau_*>0$ fixes a harmless dimensionless logarithm. For actual outgoing light signals the relevant retarded time is $u=t-r_*(R)$. Since $r_*\simeq2M\log(R-2M)+O(1)$,

$$
u=-4M\log\left(\frac{\tau_H-\tau}{\tau_*}\right)+O(1)\longrightarrow+\infty.
$$

Therefore **she never receives a signal showing the surface cross the horizon at any finite asymptotic time**. Radiation emitted ever closer to crossing arrives ever later and is increasingly redshifted and diluted; photons emitted at or inside the [event horizon](../../../../../event-horizon.md) cannot reach her. The formal crossing time at infinity is infinite, not the finite boundary stopwatch reading. Nor can the earlier global birth of the horizon be observed directly as a local flash from its central birth event.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 62](../../paper-62-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
