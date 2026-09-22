<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $f=0.46$. At [Roche-lobe overflow](../../../../../roche-lobe-overflow.md) contact, the supplied equilibrium radius relation gives

$$
a=\frac{R_\odot}{f}\frac{M_2}{M_\odot}\left(\frac M{M_2}\right)^{1/3}.
$$

[Kepler's third law](../../../../../kepler-s-third-law.md) then implies

$$
P^2=\frac{4\pi^2a^3}{GM}=\frac{4\pi^2R_\odot^3}{f^3GM_\odot}\left(\frac{M_2}{M_\odot}\right)^2.
$$

Thus the **[Roche-lobe period-mass relation for a linear donor radius law](../../../../../roche-lobe-period-mass-relation-for-a-linear-donor-radius-law.md)** is

$$
\boxed{\frac P{P_0}=\frac{M_2}{M_\odot},\qquad P_0=2\pi\sqrt{\frac{R_\odot^3}{f^3GM_\odot}}.}
$$

Here $R_\odot$ and $M_\odot$ denote the [solar radius](../../../../../solar-radius.md) and [solar mass](../../../../../solar-mass.md). Cancellation of the total mass is the special [Roche-lobe-filling period-density relation](../../../../../roche-lobe-filling-period-density-relation.md) combined with $R_2\propto M_2$.

Between eruptions the [conservative binary mass transfer](../../../../../conservative-binary-mass-transfer.md) has $M$ constant and $\dot M_1=-\dot M_2$. Neglecting spin, write

$$
J=M_1M_2\sqrt{\frac{Ga}{M}}.
$$

Its logarithmic derivative gives

$$
\frac{\dot a}{a}=2\frac{\dot J}{J}-2(1-q)\frac{\dot M_2}{M_2},\qquad q=\frac{M_2}{M_1}.
$$

Differentiating the [Roche lobe](../../../../../roche-lobe.md) relation consequently gives

$$
\boxed{\frac{\dot R_L}{R_L}=2\frac{\dot J}{J}+\left(2q-\frac53\right)\frac{\dot M_2}{M_2}.}
$$

For $\dot J=0$, the [Roche-lobe radius response exponent](../../../../../roche-lobe-radius-response-exponent.md) is $\zeta_L=2q-5/3$. If the donor follows its specified equilibrium radius sequence, $\dot R_2/R_2=\dot M_2/M_2$. Its logarithmic overflow therefore changes by

$$
\frac d{dt}\log\frac{R_2}{R_L}=\left(\frac83-2q\right)\frac{\dot M_2}{M_2}.
$$

Since $\dot M_2<0$, **$q<4/3$ gives negative feedback in this equilibrium-response model, whereas $q>4/3$ gives increasing overflow**. For $q>4/3$, loss of donor mass shrinks its [Roche lobe](../../../../../roche-lobe.md) faster than its modeled stellar radius, increasing transfer and hence amplifying the original disturbance. The $q>4/3$ comparison is a formal extension; the initial system is specified to have $q<1$.

The word dynamically needs a qualification. [Thermal equilibrium](../../../../../thermal-equilibrium.md) specifies $\zeta_{\mathrm{eq}}=1$, but actual [dynamical stability of binary mass transfer](../../../../../dynamical-stability-of-binary-mass-transfer.md) depends on the adiabatic [stellar radius response exponent](../../../../../stellar-radius-response-exponent.md) $\zeta_{\mathrm{ad}}$, which need not equal one. Stability after a rapid small mass loss requires $\zeta_{\mathrm{ad}}>\zeta_L$, because $d\log M_2<0$. The equilibrium relation alone does not supply this adiabatic response. As a formal counterexample to deriving a universal dynamical threshold from it, a radius model with a dimensionless entropy label $S$, $R(M_2,S)=C M_2^2e^S$, can have equilibrium $S_{\mathrm{eq}}=S_0-\log(M_2/M_*)$, giving $R_{\mathrm{eq}}\propto M_2$ but $\zeta_{\mathrm{ad}}=2$ at fixed $S$. At $q=3/2$, $\zeta_L=4/3<2$, so that model is dynamically stable despite the extrapolated $q>4/3$ condition. This shows the missing response hypothesis, not a claim that this toy radius law describes the given low-mass star.

A more relevant illustration is an ideal fully convective [adiabatic stellar polytrope](../../../../../adiabatic-stellar-polytrope.md) of index $3/2$. At fixed entropy its [polytropic mass-radius relation](../../../../../polytropic-mass-radius-relation.md) is $R\propto M_2^{-1/3}$, giving $\zeta_{\mathrm{ad}}=-1/3$ and a dynamical critical ratio $q=2/3$ under the same [Roche lobe](../../../../../roche-lobe.md) approximation. For example, $q=0.9<4/3$ can be unstable dynamically even though the equilibrium comparison has negative feedback. **The requested $4/3$ threshold is the intended result with instantaneous response $R_2\propto M_2$; it is not a universal dynamical criterion.** The subsequent cycle calculation uses the supplied equilibrium sequence and presumes a physically stable, sufficiently slow transfer regime.

Two important angular-momentum-loss mechanisms are [gravitational-wave emission from a binary system](../../../../../gravitational-wave-emission-from-a-binary-system.md) and [magnetic braking of a binary star](../../../../../magnetic-braking-of-a-binary-star.md). [Gravitational waves](../../../../../gravitational-wave.md) directly remove orbital energy and [angular momentum](../../../../../angular-momentum.md). A magnetized [stellar wind](../../../../../stellar-wind.md) removes donor spin angular momentum with a large magnetic lever arm; [tidal synchronization](../../../../../synchronous-rotation.md) replenishes that spin from the orbit, so the net effect is orbital angular-momentum loss. Treating the wind mass loss as small compared with the Roche-transfer flow is consistent with the conservative approximation used here; otherwise the mass and angular-momentum equations must both be modified. Neglecting the stored spin does not eliminate the torque transmitted through it.

Such losses shrink the [Roche lobe](../../../../../roche-lobe.md) and offset the donor's tendency to move inside it. Maintaining contact on the equilibrium sequence requires $\dot R_L/R_L=\dot M_2/M_2$, hence the [binary mass-transfer contact equation](../../../../../binary-mass-transfer-contact-equation.md) becomes

$$
\boxed{\frac{\dot M_2}{M_2}=\frac{3}{4-3q}\frac{\dot J}{J}.}
$$

For $q<4/3$ and $\dot J<0$, this drives $\dot M_2<0$ and maintains the modeled [semi-detached binary](../../../../../semidetached-binary.md).

Now take $\delta m>0$ for the mass expelled from the accretor in one [classical nova](../../../../../classical-nova.md). The [white dwarf](../../../../../white-dwarf.md) loses $\delta M_1=-\delta m$, while the donor has $\delta M_2=0$ and the total mass change is $\delta M=-\delta m$. Isotropic ejection in the accretor rest frame supplies no mean kick and carries the accretor's specific orbital angular momentum. Its orbital radius is $a_1=aM_2/M$, so

$$
j_1=a_1^2\Omega,\qquad\frac{j_1}{J}=\frac{M_2}{MM_1}=\frac qM,\qquad
\frac{\delta J}{J}=-q\frac{\delta m}{M}.
$$

This is the angular-momentum budget for [isotropic re-emission from a binary star](../../../../../isotropic-re-emission-from-a-binary-star.md), without an additional spin or frictional torque on the ejecta. The general logarithmic change of $J=M_1M_2\sqrt{Ga/M}$ is

$$
\frac{\delta J}{J}=\frac{\delta M_1}{M_1}+\frac{\delta M_2}{M_2}+\frac12\frac{\delta a}{a}-\frac12\frac{\delta M}{M}.
$$

Using $M/M_1=1+q$ gives the **first-order nova changes**

$$
\boxed{\frac{\delta a}{a}=\frac{\delta m}{M},\qquad
\frac{\delta R_L}{R_L}=\frac{\delta a}{a}+\frac13\left(\frac{\delta M_2}{M_2}-\frac{\delta M}{M}\right)=\frac{4\delta m}{3M}.}
$$

The donor mass and its assumed equilibrium radius are unchanged during the eruption. It is therefore left inside the enlarged [Roche lobe](../../../../../roche-lobe.md), and **[Roche-lobe overflow](../../../../../roche-lobe-overflow.md) ceases in this sharp-contact model**. An extended atmosphere, irradiation-induced donor expansion or additional ejecta torques would require a different treatment.

The stipulated circular orbit is an important idealization. Isotropic loss that is slow compared with the orbital period can preserve circularity. If it is truly impulsive compared with that period, an initially circular point-mass orbit instead acquires eccentricity. With unchanged velocity and position, its new [specific orbital energy](../../../../../specific-orbital-energy.md) is $\varepsilon'=GM/(2a)-G(M-\delta m)/a=-G(M-2\delta m)/(2a)$ and its squared [specific angular momentum](../../../../../specific-angular-momentum.md) stays $h^2=GMa$. The [Kepler orbit](../../../../../kepler-orbit.md) energy and eccentricity relations then give $a'=a(M-\delta m)/(M-2\delta m)$ and $e'=\delta m/(M-\delta m)$. The latter still has the same first-order separation increase. The question assumes circularity; its first-order circular budget is consistent with adiabatic orbital mass loss or with subsequent circularization that changes the separation only at second order. Work symbolically with $\delta m$, since the printed numerical layer mass has no explicit unit.

Finally put $\mathcal L_J=-\dot J>0$, constant over both intervals as specified, and let $J,M,q$ denote their leading-order values over one small cycle. While detached, masses and donor radius are fixed, so $\dot R_L/R_L=2\dot J/J=-2\mathcal L_J/J$. The fractional gap $4\delta m/(3M)$ closes after

$$
\boxed{t_d=\frac{2J\delta m}{3M\mathcal L_J}.}
$$

Once contact resumes, the contact equation gives $-\dot M_2=3M_2\mathcal L_J/[J(4-3q)]$. Accumulation of the next layer takes

$$
\boxed{t_s=\frac{J(4-3q)\delta m}{3M_2\mathcal L_J}.}
$$

Dividing yields the **detached-to-semidetached time ratio**

$$
\boxed{\frac{t_d}{t_s}=\frac{2M_2}{M(4-3q)}=\frac{2q}{(4-3q)(1+q)}.}
$$

Both times are first-order in $\delta m/M$. Corrections to either time are second-order in that small mass fraction, so the displayed ratio has relative corrections of order $\delta m/M$. The positive denominator, negligible eruption duration relative to the cycle, fixed donor radius during detachment and common external loss rate are all essential to this idealized [nova-induced binary detachment](../../../../../nova-induced-binary-detachment.md) cycle.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
