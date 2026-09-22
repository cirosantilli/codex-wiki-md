<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [closed-box model of galactic chemical evolution](../../../../../closed-box-model-of-galactic-chemical-evolution.md) assumes a fixed total baryonic mass, no gas inflow or outflow, instantaneous and homogeneous mixing, a constant [stellar yield](../../../../../stellar-yield.md), a fixed [initial mass function](../../../../../initial-mass-function.md), and usually the [instantaneous recycling approximation](../../../../../instantaneous-recycling-approximation.md). It predicts $Z=y\log(1/\mu)$ for gas fraction $\mu$, but real galaxies violate these assumptions.

Evidence for [galactic outflows](../../../../../galactic-outflow.md) includes blueshifted absorption, broad or split emission lines, extraplanar ionized and molecular gas, X-ray bubbles, and metal-enriched circumgalactic material. The low baryon fractions and low effective yields of dwarf galaxies, together with the [galaxy mass--metallicity relation](../../../../../galaxy-mass-metallicity-relation.md), provide indirect evidence for preferential gas and metal loss. Sustained star formation for longer than a closed reservoir's depletion time, low-metallicity high-velocity clouds, metallicity dilution during starbursts, the G-dwarf problem, and circumgalactic or intergalactic accretion signatures imply continuing [galactic gas inflow](../../../../../galactic-gas-inflow.md).

Let $f(t)=Ae^{-t/\tau}$ be the inflow rate, let the outflow rate be $\lambda\psi$, and let $R$ be the promptly returned fraction. The total baryonic, gas, and metal masses obey

$$
\boxed{\dot M_{\rm tot}=f-\lambda\psi},
$$



$$
\boxed{\dot M_g=-(1-R+\lambda)\psi+f},
$$



$$
\boxed{\frac d{dt}(ZM_g)
=y_Z(1-R)\psi-Z(1-R+\lambda)\psi+Z_{\rm prim}f}.
$$

The first metal term is newly synthesized material; the second locks existing metals into long-lived stars and removes them in an ambient-composition wind. Expanding the final derivative and substituting $\dot M_g$ cancels those common terms, leaving

$$
\boxed{\dot Z
=\frac{y_Z(1-R)\psi
+Ae^{-t/\tau}(Z_{\rm prim}-Z)}{M_g}}.
$$

The observed [Kennicutt–Schmidt law](../../../../../kennicutt-schmidt-law.md) relates star-formation and gas surface densities approximately by $\Sigma_{\rm SFR}\propto\Sigma_g^{1.4}$, with a nearly linear relation to molecular gas over many resolved regimes. For the simple integrated model requested here, take a constant depletion coefficient $S$ so that

$$
\psi(t)=SM_g(t).
$$

Then, with $\alpha=S(1-R+\lambda)$,

$$
\dot M_g+\alpha M_g=Ae^{-t/\tau}.
$$

The [integrating factor](../../../../../integrating-factor.md) $e^{\alpha t}$ gives, for $\alpha\ne1/\tau$,

$$
\boxed{M_g(t)=M_g(0)e^{-\alpha t}
+\frac{A}{\alpha-1/\tau}
\left(e^{-t/\tau}-e^{-\alpha t}\right)}.
$$

At resonance, $\alpha=1/\tau$, the continuous limit is

$$
\boxed{M_g(t)=[M_g(0)+At]e^{-\alpha t}}.
$$

The first term is depletion of the initial reservoir; the second is gas supplied by the exponentially declining inflow and subsequently consumed or expelled.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 349](../../paper-349-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
