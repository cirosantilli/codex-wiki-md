# Virial theorem on a Kepler ellipse

↑ **Parent:** [Virial theorem](virial-theorem.md)

Consider the exact [two-body problem](two-body-problem.md) with [masses](mass.md) $m_1,m_2$. In the inertial [centre of mass](center-of-mass.md) frame, its internal [kinetic energy](kinetic-energy.md) is $K=m|\dot{\mathbf r}|^2/2$, where $\mathbf r$ is their relative [position](position.md), $m=m_1m_2/(m_1+m_2)$ is the [reduced mass](reduced-mass.md), and $U=-\kappa/r$ with $\kappa=G_{\!N}m_1m_2$. Take a noncollision [elliptic Kepler orbit](elliptic-orbit.md) with [semi-major axis](semi-major-axis.md) $a$ and [orbital eccentricity](orbital-eccentricity.md) $0<e<1$. Write $\eta$ for [eccentric anomaly](eccentric-anomaly.md), to avoid confusing it with total [energy](energy-split.md) $E$. With [mean motion](mean-motion.md) $n=\sqrt{\kappa/(ma^3)}$ and [orbital period](orbital-period.md) $P=2\pi/n$, [Kepler's equation](kepler-s-equation.md) and the [orbit](orbit-dynamical-system.md) geometry give

$$
nt=\eta-e\sin\eta,\qquad r=a(1-e\cos\eta),\qquad
K=\frac{\kappa}{r}-\frac{\kappa}{2a},\qquad U=-\frac{\kappa}{r},\qquad E=-\frac{\kappa}{2a}.
$$

The [time](time-in-physics.md) origin is [periapsis](periapsis.md). Since $dt=(1-e\cos\eta)\,d\eta/n$, the [time](time-in-physics.md) average of $1/r$ over one [orbital period](orbital-period.md) is exactly $1/a$. Therefore $\langle K\rangle_P=\kappa/(2a)$ and $\langle U\rangle_P=-\kappa/a$, independently of [orbital eccentricity](orbital-eccentricity.md). Equal steps in [eccentric anomaly](eccentric-anomaly.md) are not equal [time](time-in-physics.md) steps; unweighted averaging of a drawing of the [ellipse](ellipse.md) gives the wrong answer.

<a id="virial-kepler-ellipse-energy-time-averages"></a>
![](virial-kepler-ellipse-energy-time-averages.png)

**[Figure 8](#virial-kepler-ellipse-energy-time-averages). Instantaneous kinetic energy and potential energy, their orbital period averages, and the finite-window virial residual on an eccentric Kepler orbit**.

The original dimensionless example in both diagrams has $m=a=\kappa=1$ and $e=0.6$. At [periapsis](periapsis.md), $r=0.4$, $K=2$, $U=-2.5$; at [apoapsis](apoapsis.md), $r=1.6$, $K=0.125$, $U=-0.625$. Both have $E=-0.5$, but $2K+U$ is respectively $1.5$ and $-0.375$. Only the [orbital period](orbital-period.md) averages are $\langle K\rangle_P=0.5$ and $\langle U\rangle_P=-1$. The instantaneous zero of $2K+U$ occurs at $r=a$, not at every point of the [orbit](orbit-dynamical-system.md).

<a id="virial-kepler-ellipse-orbit-configuration"></a>
![](virial-kepler-ellipse-orbit-configuration.png)

**[Figure 9](#virial-kepler-ellipse-orbit-configuration). Relative orbit of the same two-body problem, with equal-time markers, the attracting focus, and periapsis and apoapsis energies**.

The endpoint term can also be evaluated exactly: $G=m\mathbf r\cdot\dot{\mathbf r}=mna^2e\sin\eta$. Starting at [periapsis](periapsis.md), a window ending at [eccentric anomaly](eccentric-anomaly.md) $\eta$ has

$$
2\langle K\rangle_T+\langle U\rangle_T
=\frac{\kappa}{a}\frac{e\sin\eta}{\eta-e\sin\eta}.
$$

At $T=P/4$, [Kepler's equation](kepler-s-equation.md) gives $\eta\simeq2.09133$ and a positive residual $\simeq0.3314\kappa/a$. At $T=P/2$ or $P$, $G$ returns to zero and the residual vanishes exactly. The lower panel shows the running residual and its endpoint expression coinciding; the shaded quarter-[orbital period](orbital-period.md) window explains why a short observation need not satisfy the infinite-[time](time-in-physics.md) theorem.

## ↑ Ancestors (5)

1. [Virial theorem](virial-theorem.md)
2. [Classical mechanics](classical-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)
