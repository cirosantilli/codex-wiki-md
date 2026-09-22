<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

**Orbital energy.** Treat the star as stationary to leading order in $m/M$, with Newtonian [gravitational parameter](../../../standard-gravitational-parameter.md) $\mu=GM$. For [velocity](../../../velocity.md) components in [plane polar coordinates](../../../plane-polar-coordinates.md), $v^2=\dot r^2+r^2\dot\phi^2$. The [kinetic energy](../../../kinetic-energy.md) is $mv^2/2$. Integrating [Newton's law of universal gravitation](../../../newton-s-law-of-universal-gravitation-split.md) with zero [gravitational potential energy](../../../gravitational-energy.md) at infinite separation gives $U(r)=-GMm/r$. Thus

$$
\boxed{E=\frac12m\dot r^2+\frac12mr^2\dot\phi^2-\frac{GMm}{r}
=\frac12m\dot r^2+\frac{J^2}{2mr^2}-\frac{GMm}{r},}
$$

where $J=mr^2\dot\phi$ is the satellite's [angular momentum](../../../angular-momentum.md). The first term is radial [kinetic energy](../../../kinetic-energy.md); the second is transverse [kinetic energy](../../../kinetic-energy.md), also the centrifugal contribution to the radial [effective potential](../../../effective-potential.md); the last is the attractive [gravitational potential energy](../../../gravitational-energy.md). These are not three independent sources of energy: the centrifugal term is already part of the ordinary [kinetic energy](../../../kinetic-energy.md).

For an [elliptic Kepler orbit](../../../elliptic-orbit.md) of [semi-major axis](../../../semi-major-axis.md) $a$ and [orbital eccentricity](../../../orbital-eccentricity.md) $e$, the [polar equation of a Kepler orbit](../../../polar-equation-of-a-kepler-orbit.md) $r=p/(1+e\cos\phi)$ has [semilatus rectum](../../../semilatus-rectum.md) $p=J^2/(GMm^2)=a(1-e^2)$. Substituting $\dot r=(Je/(mp))\sin\phi$ into the preceding expression reduces it to

$$
E=\frac{GMm}{2p}(e^2-1),
\qquad
\boxed{E=-\frac{GMm}{2a}.}
$$

For a [circular Kepler orbit](../../../circular-kepler-orbit.md), $a=R$, $v_0^2=GM/R$, $K=GMm/(2R)$, and $U=-GMm/R$. Negative total [energy](../../../energy-split.md) describes a [bound orbit](../../../bound-orbit.md).

**Rapid, symmetric mass loss.** Assume the mass is removed on a timescale short compared with the satellite's [orbital period](../../../orbital-period.md), without an impulsive kick or appreciable wind [drag](../../../drag-physics.md) on the satellite. The post-loss gravitational parameter is $\mu'=G(1-f)M$ with $f=0.01$. At the change, $r=R$, $\dot r=0$, and $v=v_0=\sqrt{GM/R}$ are unchanged. Spherical symmetry keeps the [force](../../../force-split.md) central, so the [specific angular momentum](../../../specific-angular-momentum.md) $j=J/m=\sqrt{GMR}$ is conserved. [Orbital energy](../../../orbital-energy.md) is not conserved across the changing gravitational field:

$$
\varepsilon'=\frac{E'}m=\frac12\frac{GM}{R}-\frac{G(1-f)M}{R}
=-\frac{GM}{2R}(1-2f).
$$

The new [semi-major axis](../../../semi-major-axis.md) is consequently

$$
a'=-\frac{\mu'}{2\varepsilon'}=\frac{1-f}{1-2f}R.
$$

The original [speed](../../../speed.md) now exceeds the new circular [speed](../../../speed.md) at $R$, and the outward radial [acceleration](../../../acceleration.md) is $v_0^2/R-\mu'/R^2=fGM/R^2>0$. Thus the release point is the new [pericentre](../../../periapsis.md), not the [apocentre](../../../apoapsis.md). The [impulsive orbital expansion under isotropic mass loss](../../../impulsive-orbital-expansion-under-isotropic-mass-loss.md) gives

$$
r_{\min}=R,\qquad r_{\max}=2a'-R=\frac{R}{1-2f},\qquad e'=\frac{f}{1-f}.
$$

For the stated one-percent loss,

$$
\boxed{r_{\min}=R,\qquad r_{\max}=\frac{50}{49}R\simeq1.02041R,\qquad e'=\frac1{99}.}
$$

An independent [angular momentum](../../../angular-momentum.md) check is $j^2=\mu'a'(1-e'^2)=GMR$. The impulsive orbit stays bound for $f<1/2$; loss of half the central mass is the zero-[orbital energy](../../../orbital-energy.md) limit.

**What the wind timescale changes.** The source specifies a spherically symmetric wind but does not give its duration. The preceding nearest and furthest distances require the rapid-loss assumption. In the opposite, slow limit, [adiabatic orbital expansion under isotropic mass loss](../../../adiabatic-orbital-expansion-under-isotropic-mass-loss.md) preserves an initially circular orbit to leading adiabatic order. Conserved [specific angular momentum](../../../specific-angular-momentum.md) then gives $j^2=G M(t)r(t)$, hence $M(t)r(t)=MR$. After the same loss,

$$
\boxed{r_{\min}\simeq r_{\max}\simeq\frac{R}{1-f}=\frac{100}{99}R\simeq1.01010R\quad\text{(adiabatic limit)}.}
$$

For a finite intermediate timescale, the orbit depends on the mass-loss history; the percentage alone does not select a unique pair of turning distances. Neglecting wind recoil and wind [drag](../../../drag-physics.md) is common to both idealizations.

## ↑ Ancestors (11)

1. [9](../9.md)
2. [2015 resit](../../2015-resit-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
