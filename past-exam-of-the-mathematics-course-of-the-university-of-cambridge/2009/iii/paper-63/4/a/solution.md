<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Since the donor fills its [Roche lobe](../../../../../../roche-lobe.md), use $R_2=R_L$ and substitute its equilibrium mass-radius relation into the lobe approximation:

$$
a=\frac{R_\odot}{0.46}\frac{M_2}{M_\odot}
\left(\frac M{M_2}\right)^{1/3}.
$$

[Kepler's third law](../../../../../../kepler-s-third-law.md) then gives

$$
P^2=\frac{4\pi^2a^3}{GM}
=\frac{4\pi^2R_\odot^3}{0.46^3GM_\odot}
\left(\frac{M_2}{M_\odot}\right)^2,
$$

so the [Roche-lobe period-mass relation for a linear donor radius law](../../../../../../roche-lobe-period-mass-relation-for-a-linear-donor-radius-law.md) is

$$
\boxed{\frac P{P_0}=\frac{M_2}{M_\odot},\qquad
P_0=2\pi\sqrt{\frac{R_\odot^3}{0.46^3GM_\odot}}.}
$$

The total binary [mass](../../../../../../mass.md) cancels, rather than being assumed equal to the white-dwarf [mass](../../../../../../mass.md).

The orbital radii about the [center of mass](../../../../../../center-of-mass.md) are $a_1=aM_2/M$ and $a_2=aM_1/M$. Summing the two orbital angular momenta gives

$$
J=(M_1a_1^2+M_2a_2^2)\Omega
=\boxed{\frac{M_1M_2}{M}a^2\Omega}
=M_1M_2\sqrt{\frac{Ga}{M}}.
$$

With transferred matter retained by the accretor, total [mass](../../../../../../mass.md) is fixed. Logarithmic differentiation gives

$$
\frac{\dot J}J=\frac{\dot M_1}{M_1}+\frac{\dot M_2}{M_2}
+\frac12\frac{\dot a}a
=(1-q)\frac{\dot M_2}{M_2}+\frac12\frac{\dot a}a.
$$

For $\dot J=0$, the separation response is $\dot a/a=2(q-1)\dot M_2/M_2$. Since $R_L\propto aM_2^{1/3}$ at fixed total [mass](../../../../../../mass.md),

$$
\boxed{\frac{\dot R_L}{R_L}=\left(2q-\frac53\right)\frac{\dot M_2}{M_2},
\qquad \frac{\dot R_2}{R_2}=\frac{\dot M_2}{M_2}.}
$$

The second relation uses the supplied equilibrium donor sequence. As the donor loses [mass](../../../../../../mass.md), $\dot M_2<0$. If $q>4/3$, its [Roche lobe](../../../../../../roche-lobe.md) shrinks fractionally faster than this donor radius, so the excess filling increases and drives more transfer: it is positive feedback. If $q<4/3$, infinitesimal loss instead reduces overfill on that assumed sequence, so some continuing driver is needed to retain contact.

There are two limits to the literal dynamical interpretation. The given initial range is $q<1$, so $q>4/3$ is an extrapolated instability test, not a state inside that range. Also, a true [dynamical stability of binary mass transfer](../../../../../../dynamical-stability-of-binary-mass-transfer.md) test needs the donor's adiabatic [stellar radius response exponent](../../../../../../stellar-radius-response-exponent.md) $\zeta_{\mathrm{ad}}$, rather than its thermal-equilibrium exponent. In general,

$$
\frac{d}{dt}\log\frac{R_2}{R_L}
=(\zeta_* -2q+5/3)\frac{\dot M_2}{M_2},\qquad
q_{\mathrm{crit}}=\frac{\zeta_*+5/3}{2}.
$$

Thus $4/3$ is the result for the assumed $\zeta_*=1$ response. A fully convective idealized donor has $\zeta_{\mathrm{ad}}=-1/3$, giving a dynamical threshold $2/3$, already below $4/3$. The equilibrium radius law alone should not be used to assert a universal dynamical threshold.

One continuing driver is [magnetic braking of a binary star](../../../../../../magnetic-braking-of-a-binary-star.md). A magnetized wind carries away the donor's spin [angular momentum](../../../../../../angular-momentum.md); tides that maintain near-synchronous rotation replenish that spin from the orbit, removing orbital [angular momentum](../../../../../../angular-momentum.md). With an external $\dot J<0$, the lobe response becomes

$$
\frac{\dot R_L}{R_L}=2\frac{\dot J}J+
\left(2q-\frac53\right)\frac{\dot M_2}{M_2}.
$$

Equating this to the donor response proves the [binary mass-transfer contact equation](../../../../../../binary-mass-transfer-contact-equation.md) in this model:

$$
\boxed{\frac{\dot M_2}{M_2}=\frac{\dot J/J}{4/3-q}.}
$$

A negative [torque](../../../../../../torque.md) therefore drives [mass](../../../../../../mass.md) loss while maintaining contact for $q<4/3$, subject to the chosen donor response and braking assumptions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
