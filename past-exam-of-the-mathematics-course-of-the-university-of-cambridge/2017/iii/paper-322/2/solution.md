<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For [Roche-lobe overflow](../../../../../roche-lobe-overflow.md) in the stipulated [stellar thermal equilibrium](../../../../../stellar-thermal-equilibrium.md), $R_2=R_L$. Using the [mass-radius relation](../../../../../mass-radius-relation.md) and [Kepler's third law](../../../../../kepler-s-third-law.md),

$$
a^3=\frac{R_\odot^3}{0.46^3}\frac{M M_2^2}{M_\odot^3},\qquad P^2=\frac{4\pi^2a^3}{GM}.
$$

The total [mass](../../../../../mass.md) cancels, giving

$$
\boxed{\frac{P}{P_0}=\frac{M_2}{M_\odot},\qquad P_0=2\pi\sqrt{\frac{R_\odot^3}{0.46^3GM_\odot}}\simeq8.91\ \mathrm{h}.}
$$

Here $R_\odot$ is the [solar radius](../../../../../solar-radius.md). This is the [Roche-lobe-filling period-density relation](../../../../../roche-lobe-filling-period-density-relation.md) specialized to $R_2\propto M_2$.

Neglecting spin, the [angular momentum](../../../../../angular-momentum.md) of a [circular orbit](../../../../../circular-orbit.md) is $J=M_1M_2\sqrt{Ga/M}$. Between [classical novae](../../../../../classical-nova.md) the transfer conserves total [mass](../../../../../mass.md), so $\dot M=0$ and $\dot M_1=-\dot M_2$. Its logarithmic derivative gives

$$
\frac{\dot J}{J}=(1-q)\frac{\dot M_2}{M_2}+\frac12\frac{\dot a}{a},\qquad
\frac{\dot R_L}{R_L}=2\frac{\dot J}{J}+\left(2q-\frac53\right)\frac{\dot M_2}{M_2}.
$$

In particular, for [conservation of angular momentum](../../../../../conservation-of-angular-momentum.md),

$$
\boxed{\frac{\dot R_L}{R_L}=\left(2q-\frac53\right)\frac{\dot M_2}{M_2},\qquad \frac{\dot R_2}{R_2}=\frac{\dot M_2}{M_2}.}
$$

The source PDF has $\dot J=0$ here; the TeX's $J=0$ is a transcription defect. For $q>4/3$, the [Roche-lobe radius response exponent](../../../../../roche-lobe-radius-response-exponent.md) exceeds the equilibrium [stellar radius response exponent](../../../../../stellar-radius-response-exponent.md) $1$. Since $\dot M_2<0$, the [Roche lobe](../../../../../roche-lobe.md) then shrinks faster than the [donor star](../../../../../donor-star.md); the overfill increases and drives more transfer, giving positive feedback. Equality at $q=4/3$ is marginal in this linear response test.

Two qualifications matter. First, $q>4/3$ is a formal extrapolation outside the stated $q<1$ range, and the supplied [Roche lobe](../../../../../roche-lobe.md) approximation need not remain accurate there. Second, true [dynamical stability of binary mass transfer](../../../../../dynamical-stability-of-binary-mass-transfer.md) compares $\zeta_L$ with the adiabatic [stellar radius response exponent](../../../../../stellar-radius-response-exponent.md) $\zeta_{\rm ad}$, not $\zeta_{\rm eq}=1$. The [stellar thermal equilibrium](../../../../../stellar-thermal-equilibrium.md) argument supplies the displayed feedback threshold under the imposed radius law, rather than a necessary and sufficient physical dynamical threshold. For example, the [polytropic mass-radius relation](../../../../../polytropic-mass-radius-relation.md) for a fully convective [adiabatic stellar polytrope](../../../../../adiabatic-stellar-polytrope.md) with index $3/2$ gives $\zeta_{\rm ad}=-1/3$; within this same [Roche lobe](../../../../../roche-lobe.md) approximation its dynamical threshold is $q=2/3$. Thus $q<4/3$ by itself does not guarantee dynamical stability.

[Gravitational-wave emission from a binary system](../../../../../gravitational-wave-emission-from-a-binary-system.md) removes orbital [energy](../../../../../energy.md) and [angular momentum](../../../../../angular-momentum.md). [Magnetic braking of a binary star](../../../../../magnetic-braking-of-a-binary-star.md) provides another important loss: a magnetized [stellar wind](../../../../../stellar-wind.md) carries away donor spin, while [tidal locking](../../../../../tidal-locking.md) couples that spin to the orbit. Tides alone redistribute [angular momentum](../../../../../angular-momentum.md) and are not an external sink. Matter expelled from the system can also carry orbital [angular momentum](../../../../../angular-momentum.md), although appreciable continuous mass loss would require nonconservative modifications of the preceding equations. Setting $\dot R_L/R_L=\dot R_2/R_2$ gives the [binary mass-transfer contact equation](../../../../../binary-mass-transfer-contact-equation.md)

$$
\boxed{\frac{\dot M_2}{M_2}=\frac{3\dot J}{J(4-3q)}.}
$$

For $q<4/3$, a negative external $\dot J$ therefore sustains negative $\dot M_2$ along the stipulated [stellar thermal equilibrium](../../../../../stellar-thermal-equilibrium.md) contact sequence, provided the system is otherwise stable and can remain thermally relaxed.

During the [classical nova](../../../../../classical-nova.md), the ejecta carry the [white dwarf](../../../../../white-dwarf.md)'s [specific angular momentum](../../../../../specific-angular-momentum.md), not zero [angular momentum](../../../../../angular-momentum.md). With $\Omega^2=GM/a^3$ and the accretor's distance from the [centre of mass](../../../../../center-of-mass.md) $a_1=aM_2/M$, isotropic escape gives

$$
j_1=a_1^2\Omega,\qquad \frac{j_1}{J}=\frac{M_2}{M_1M}=\frac qM,\qquad \frac{\delta J}{J}=-\frac{q\delta m}{M}.
$$

The slow ejection relative to the [orbital period](../../../../../orbital-period.md) permits the adiabatic [circular orbit](../../../../../circular-orbit.md) approximation; the [donor star](../../../../../donor-star.md) does not transfer appreciable additional mass during it. Take $\delta M_1=-\delta m$, $\delta M_2=0$ and $\delta M=-\delta m$. Differentiating $J=M_1M_2\sqrt{Ga/M}$ gives

$$
-\frac{q\delta m}{M}=-\frac{\delta m}{M_1}+\frac12\frac{\delta a}{a}+\frac{\delta m}{2M}.
$$

Since $M/M_1=1+q$, this yields

$$
\boxed{\frac{\delta a}{a}=\frac{\delta m}{M},\qquad \frac{\delta R_L}{R_L}=\frac{\delta a}{a}+\frac13\left(\frac{\delta M_2}{M_2}-\frac{\delta M}{M}\right)=\frac{4\delta m}{3M}.}
$$

These are first-order formulae with errors of order $(\delta m/M)^2$. The orbital widening agrees with [Jeans-mode mass loss](../../../../../jeans-mode-mass-loss.md). The [donor star](../../../../../donor-star.md)'s radius is unchanged to this order by the assumed ejection, so its [Roche lobe](../../../../../roche-lobe.md) expands away from it, causing [nova-induced binary detachment](../../../../../nova-induced-binary-detachment.md). This idealization neglects changes in the donor from irradiation or interaction with ejecta; those are not supplied in the model.

Let $\Gamma=-\dot J>0$ be the fixed external loss rate. During the [detached binary](../../../../../detached-binary.md) phase both component masses are fixed, and $\dot R_L/R_L=2\dot J/J=-2\Gamma/J$. Closing the fractional gap $4\delta m/(3M)$ takes

$$
t_d=\frac{2J\delta m}{3M\Gamma}.
$$

In the subsequent [semidetached binary](../../../../../semidetached-binary.md), the [binary mass-transfer contact equation](../../../../../binary-mass-transfer-contact-equation.md) gives $-\dot M_2=3M_2\Gamma/[J(4-3q)]$. Accumulating a fresh layer of [mass](../../../../../mass.md) $\delta m$ therefore takes

$$
t_s=\frac{J(4-3q)\delta m}{3M_2\Gamma},\qquad
\boxed{\frac{t_d}{t_s}=\frac{2M_2}{M(4-3q)}=\frac{2q}{(1+q)(4-3q)}.}
$$

Throughout these first-order estimates $J,M,q$ can be evaluated at the start of the cycle: their fractional changes during it are of order $\delta m/M$. The limit $\Gamma=0$ is excluded, since no finite reconnection time follows without an external shrinkage mechanism.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 322](../../paper-322-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
