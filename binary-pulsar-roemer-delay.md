# Binary-pulsar Roemer delay

↑ **Parent:** [Projected pulsar semimajor axis](projected-pulsar-semimajor-axis.md)

The geometric light-travel contribution from the [pulsar](pulsar.md)'s position within the binary [orbit](orbit-dynamical-system.md). To construct an eccentric [Kepler orbit](kepler-orbit.md), use [eccentric anomaly](eccentric-anomaly.md) $E$, [orbital eccentricity](orbital-eccentricity.md) $e$, [mean anomaly](mean-anomaly.md) $M=2\pi(t-T_0)/P_b$, and [argument of periapsis](argument-of-periapsis.md) $\omega$. Here $T_0$ is passage through [periapsis](periapsis.md). Coordinates in the [orbital plane](orbital-plane.md) are $X=a_1(\cos E-e)$ and $Y=a_1\sqrt{1-e^2}\sin E$. Rotate through $\omega$ and project by $\sin i$ to obtain

$$
E-e\sin E=M,\qquad
\Delta_R=x\left[\sin\omega(\cos E-e)+\sqrt{1-e^2}\cos\omega\sin E\right].
$$

The first equation is [Kepler's equation](kepler-s-equation.md): equal time intervals give equal increments of $M$, not of $E$. Since $1-e\cos E>0$ for $0\le e<1$, each $M$ has a unique $E$ on the corresponding unwrapped orbit. A constant delay is absorbed into the arbitrary arrival-time origin. The circular limit is $\Delta_R=x\sin(M+\omega)$, so its amplitude measures $x$. For $e>0$, the delay's offset and amplitude also depend on $\omega$; its maximum is not generally $x$.

## ↑ Ancestors (10)

1. [Projected pulsar semimajor axis](projected-pulsar-semimajor-axis.md)
2. [Binary pulsar](binary-pulsar.md)
3. [Pulsar](pulsar.md)
4. [Neutron star](neutron-star.md)
5. [Stellar evolution](stellar-evolution.md)
6. [Stellar astrophysics](stellar-astrophysics-split.md)
7. [Astrophysics](astrophysics-split.md)
8. [Branches of physics](branches-of-physics.md)
9. [Physics](physics-split.md)
10. [Codex Wiki](split.md)
