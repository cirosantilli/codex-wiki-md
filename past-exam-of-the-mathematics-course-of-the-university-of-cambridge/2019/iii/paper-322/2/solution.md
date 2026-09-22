<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [cataclysmic variable](../../../../../cataclysmic-variable.md) is a close interacting [binary star](../../../../../binary-star.md) with a [white dwarf](../../../../../white-dwarf.md) accretor and a low-mass [donor star](../../../../../donor-star.md), usually a [red dwarf](../../../../../red-dwarf.md), filling its [Roche lobe](../../../../../roche-lobe.md). Matter crosses by [Roche-lobe overflow](../../../../../roche-lobe-overflow.md) and commonly forms an [accretion disk](../../../../../accretion-disk.md); sufficiently strong white-dwarf magnetism instead permits [magnetically channelled accretion](../../../../../magnetically-channelled-accretion.md). Accretion produces strong variability, while [classical novae](../../../../../classical-nova.md) result from unstable burning of accumulated hydrogen.

The [cataclysmic-variable orbital-period distribution](../../../../../cataclysmic-variable-orbital-period-distribution.md) contains a short-period population between about 82 minutes and two hours, a pronounced [cataclysmic-variable period gap](../../../../../cataclysmic-variable-period-gap.md) around two to three hours, and a longer-period population above the gap. There is an accumulation near the [cataclysmic-variable period minimum](../../../../../cataclysmic-variable-period-minimum.md). These describe ordinary hydrogen-rich systems; evolved donors and helium-rich systems can have shorter periods. Selection by luminosity and outburst activity affects the observed counts, so $N(P)$ is not simply the intrinsic distribution.

For the contact [red dwarf](../../../../../red-dwarf.md), $R_2=R_L\propto a(M_2/M)^{1/3}$. Using its supplied thermal-equilibrium [mass-radius relation](../../../../../mass-radius-relation.md), $R_2\propto M_2$, gives $a\propto M_2^{2/3}M^{1/3}$. [Kepler's third law](../../../../../kepler-s-third-law.md) then gives

$$
\boxed{P\propto a^{3/2}M^{-1/2}\propto M_2},
$$

independent of $M_1$. This is a special case of the [Roche-lobe-filling period-density relation](../../../../../roche-lobe-filling-period-density-relation.md).

To examine rapid mass loss, use the [stellar radius response exponent](../../../../../stellar-radius-response-exponent.md) $\zeta_{\rm ad}=d\log R_2/d\log M_2=-1/3$. During [conservative binary mass transfer](../../../../../conservative-binary-mass-transfer.md), $M$ and $J=M_1M_2\sqrt{Ga/M}$ are fixed, and $dM_1=-dM_2$. Therefore

$$
\frac{d\log a}{d\log M_2}=-2(1-q),\qquad
\zeta_L=\frac{d\log R_L}{d\log M_2}=-2(1-q)+\frac13=2q-\frac53.
$$

The change in overfill is $d\log(R_2/R_L)=(\zeta_{\rm ad}-\zeta_L)d\log M_2$. Since $d\log M_2<0$, overfill grows, and mass loss runs away, when $\zeta_{\rm ad}<\zeta_L$. The [dynamical stability of binary mass transfer](../../../../../dynamical-stability-of-binary-mass-transfer.md) criterion here is consequently

$$
\boxed{q_{\rm crit}=\frac23,\qquad \text{unstable for }q>\frac23,\quad\text{stable for }q<\frac23}.
$$

**The printed instability inequality is reversed.** With the defined $q=M_2/M_1$, the specified radius laws imply the inequality above; $q<q_{\rm crit}$ is the stable side. Equality is marginal, and the supplied Roche-radius approximation restricts this calculation to its stated mass-ratio range.

Long-term contact is maintained by [angular momentum transport](../../../../../angular-momentum-transport.md) out of the orbit. [Gravitational-wave emission from a binary system](../../../../../gravitational-wave-emission-from-a-binary-system.md) provides one loss mechanism. [Magnetic braking of a binary star](../../../../../magnetic-braking-of-a-binary-star.md) uses the donor's [stellar wind](../../../../../stellar-wind.md): its [magnetic field](../../../../../magnetic-field.md) enforces approximate corotation out to the [Alfvén radius](../../../../../alfven-radius.md), so the wind carries much more [specific angular momentum](../../../../../specific-angular-momentum.md) than a nonmagnetic surface outflow. At that radius, roughly

$$
\boxed{v_{\rm wind}\simeq v_A=\frac{B}{\sqrt{\mu_0\rho}},\qquad
\dot M_w\simeq4\pi R_A^2\rho v_{\rm wind}},\qquad
\dot J_w\sim-\dot M_w\Omega R_A^2.
$$

The geometry contributes order-one factors to the torque. Even when $\dot M_w\ll|\dot M_2|$, the large lever arm can remove substantial spin [angular momentum](../../../../../angular-momentum.md). [Tidal locking](../../../../../tidal-locking.md) couples donor spin to orbital motion, so the wind torque ultimately brakes the orbit. In practice [classical novae](../../../../../classical-nova.md) can also eject matter; the conservative calculations here isolate the stated idealization.

For the prescribed $\dot J/J=-\alpha$, now use the supplied equilibrium law $R_2\propto M_2$ for the slowly evolving donor. Contact implies $\dot a/a=(2/3)\dot M_2/M_2$, assuming negligible net wind mass loss. Taking the logarithmic derivative of $J$ gives

$$
-\alpha=(1-q)\frac{\dot M_2}{M_2}+\frac12\frac{\dot a}{a}
=\left(\frac43-q\right)\frac{\dot M_2}{M_2}.
$$

Since $P\propto M_2$ along this equilibrium sequence,

$$
\boxed{\frac{\dot P}{P}=\frac{\dot M_2}{M_2}=\frac{3\alpha}{3q-4}}.
$$

For the dynamically stable mass ratios, this is negative. The result uses thermal equilibrium as well as slow hydrostatic evolution; evolution slow compared only with the dynamical time does not by itself guarantee the radius law $R_2\propto M_2$.

In the [disrupted magnetic braking model](../../../../../disrupted-magnetic-braking-model.md), the donor above the gap loses mass fast enough to be inflated relative to thermal equilibrium. When the donor becomes a [fully convective star](../../../../../fully-convective-star.md), the model assumes a substantial reduction in magnetic braking. The [red dwarf](../../../../../red-dwarf.md) then contracts toward equilibrium on its [Kelvin-Helmholtz cooling time](../../../../../kelvin-helmholtz-cooling-time.md), becoming smaller than its [Roche lobe](../../../../../roche-lobe.md); accretion largely stops. [Gravitational-wave emission from a binary system](../../../../../gravitational-wave-emission-from-a-binary-system.md) continues to reduce the separation, carrying the detached binary through the gap until contact is restored near its lower edge.

This explanation requires strong braking immediately above the gap: the donor must already be out of equilibrium and inflated, so there is room to contract and detach when braking drops. With nearly fixed component masses during detachment, $R_L\propto a\propto P^{2/3}$, giving the illustrative inflation factor

$$
\boxed{\frac{R_{2,\rm upper}}{R_{2,\rm equilibrium}}
\simeq\left(\frac{P_{\rm upper}}{P_{\rm lower}}\right)^{2/3}
\simeq\left(\frac32\right)^{2/3}\simeq1.31}.
$$

A weak braking torque that kept the donor in thermal equilibrium just above the gap would not produce this detachment. The model requires a decrease in the torque, not disappearance of the donor's [magnetic field](../../../../../magnetic-field.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 322](../../paper-322-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
