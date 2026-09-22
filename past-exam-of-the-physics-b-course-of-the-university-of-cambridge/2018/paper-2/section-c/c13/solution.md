<h1 id="section-c/c13/solution">Solution</h1>

↑ **Parent:** [C13](../c13.md)

**[Entropy](../../../../../entropy-split.md) at [absolute zero](../../../../../absolute-zero.md).** The [third law of thermodynamics](../../../../../third-law-of-thermodynamics.md) concerns the low-temperature limit of equilibrium states. In the zero-[entropy](../../../../../entropy-split.md) formulation, the [entropy](../../../../../entropy-split.md) of a perfect crystal with a nondegenerate [ground state](../../../../../ground-state.md) tends to zero as $T\to0$. The statistical interpretation is $S=k_B\ln\Omega$: a unique accessible [ground state](../../../../../ground-state.md) has $\Omega=1$. The entropy-difference formulation of the [third law of thermodynamics](../../../../../third-law-of-thermodynamics.md) states that [entropy](../../../../../entropy-split.md) differences associated with regular changes of mechanical parameters tend to zero as [absolute zero](../../../../../absolute-zero.md) is approached. These statements require equilibrium and appropriate ground-state assumptions; a frozen disordered material or a degenerate [ground state](../../../../../ground-state.md) can carry [residual entropy](../../../../../residual-entropy.md).

For a phase of fixed composition and [pressure](../../../../../pressure-split.md),

$$
S(T,p)-S(0,p)=\int_0^T\frac{C_p(t,p)}{t}\,dt.
$$

A finite limiting [entropy](../../../../../entropy-split.md) constrains this [integral](../../../../../integral-split.md). Ordinary equilibrium [heat capacities](../../../../../heat-capacity.md) therefore vanish as [temperature](../../../../../temperature-split.md) approaches zero, with familiar examples $C\propto T^3$ for three-dimensional acoustic [phonons](../../../../../phonon.md) and $C\propto T$ for a normal degenerate [Fermi liquid](../../../../../fermi-liquid-split.md). A constant positive [heat capacity](../../../../../heat-capacity.md) extrapolated to zero would give a logarithmically divergent [entropy](../../../../../entropy-split.md) difference and is impossible in this regime. Discontinuous transitions and anomalous limits need separate treatment rather than extending a high-temperature approximation indefinitely.

**[Gibbs free energy](../../../../../gibbs-free-energy.md).** For fixed particle numbers,

$$
dG=-S\,dT+V\,dp,
\qquad
\boxed{S=-\left(\frac{\partial G}{\partial T}\right)_p.}
$$

Thus, when $S\to0$, the [Gibbs free energy](../../../../../gibbs-free-energy.md) approaches its zero-temperature value with a horizontal tangent:

$$
\boxed{G(T,p)\to H(0,p),\qquad
\left(\frac{\partial G}{\partial T}\right)_p\to0,
\qquad G-H=-TS\to0.}
$$

The equality $G(0,p)=H(0,p)$ uses the [enthalpy](../../../../../enthalpy-split.md) $H=U+pV$; neither limiting value needs to be zero. The [low-temperature Gibbs free-energy expansion](../../../../../low-temperature-gibbs-free-energy-expansion.md) makes the approach quantitative. For $C_p=aT^r$ with $r>0$ and $S(0)=0$,

$$
S=\frac{a}{r}T^r,\qquad
G(T,p)=G(0,p)-\frac{a}{r(r+1)}T^{r+1}.
$$

The second [derivative](../../../../../derivative.md) is $\partial_T^2G=-C_p/T\leq0$, although it need not tend to zero. For a reaction between such equilibrium phases, $\partial_T\Delta G=-\Delta S\to0$, and $\Delta G$ and $\Delta H$ approach one another. If a genuine [residual entropy](../../../../../residual-entropy.md) $S_0$ is retained instead, $G=G(0,p)-S_0T+\cdots$ has limiting slope $-S_0$. A horizontal tangent cannot be asserted without the zero-entropy condition.

**Why [helium](../../../../../helium.md) remains a [liquid](../../../../../liquid.md).** [Helium](../../../../../helium.md) atoms attract each other weakly and are exceptionally light. Their [zero-point energy](../../../../../zero-point-energy.md) is large compared with the binding that would localize them in a [solid](../../../../../solid.md). Both [helium-4](../../../../../helium-4.md) and [helium-3](../../../../../helium-3.md) can therefore remain [liquid](../../../../../liquid.md) down to the lowest [temperatures](../../../../../temperature-split.md) at low [pressure](../../../../../pressure-split.md); substantial applied [pressure](../../../../../pressure-split.md) is needed to solidify them. This is not a violation of the third law. A quantum [liquid](../../../../../liquid.md) can have a unique low-entropy [ground state](../../../../../ground-state.md), and [zero-point motion](../../../../../zero-point-motion.md) does not itself imply thermal [entropy](../../../../../entropy-split.md). The third law does not require every substance to crystallize at atmospheric [pressure](../../../../../pressure-split.md).

A [helium-4](../../../../../helium-4.md) atom has integer [spin](../../../../../spin.md) zero and is a [boson](../../../../../boson.md). Below the [lambda point](../../../../../lambda-point.md) near $2.17\,\mathrm K$ at saturated [vapor pressure](../../../../../vapor-pressure.md), its [liquid](../../../../../liquid.md) is [superfluid](../../../../../superfluid.md). Its strong interactions mean that it is not quantitatively an ideal Bose gas, and the [condensate fraction](../../../../../condensate-fraction.md) need not equal the [superfluid fraction](../../../../../superfluid-fraction.md). The [two-fluid model of superfluidity](../../../../../two-fluid-model-of-superfluidity.md) separates an entropy-carrying [normal component of a superfluid](../../../../../normal-component-of-a-superfluid.md) from the [superfluid](../../../../../superfluid.md) component, whose [entropy](../../../../../entropy-split.md) is zero. At sufficiently low [temperature](../../../../../temperature-split.md) the dominant thermal excitations are acoustic [phonons](../../../../../phonon.md): their linear dispersion in three dimensions gives $U-U_0\propto VT^4$, $C_V\propto VT^3$ and $S\propto VT^3$. Higher-energy [rotons](../../../../../roton.md) are exponentially suppressed. Thus the [normal component of a superfluid](../../../../../normal-component-of-a-superfluid.md) and [entropy](../../../../../entropy-split.md) disappear as $T\to0$, while [superfluid](../../../../../superfluid.md) flow and quantum motion can persist.

A [helium-3](../../../../../helium-3.md) atom has [spin](../../../../../spin.md) $1/2$ and is a [fermion](../../../../../fermion.md). Well below its [Fermi temperature](../../../../../fermi-temperature.md), but above its [superfluid](../../../../../superfluid.md) transition, [liquid](../../../../../liquid.md) [helium-3](../../../../../helium-3.md) is a degenerate interacting [Fermi liquid](../../../../../fermi-liquid-split.md). Only [quasiparticles](../../../../../quasiparticle.md) close to the [Fermi surface](../../../../../fermi-surface.md) are thermally excited, giving $C_V\propto T$ and $S\propto T$. At [temperatures](../../../../../temperature-split.md) of order a millikelvin, [helium-3](../../../../../helium-3.md) also becomes [superfluid](../../../../../superfluid.md) through formation of [Cooper pairs](../../../../../cooper-pair.md) of [fermions](../../../../../fermion.md). This is not [Bose-Einstein condensation](../../../../../bose-einstein-condensation.md) of individual [helium-3](../../../../../helium-3.md) atoms. Pairing reorganizes the low-energy excitation spectrum; in the fully gapped bulk B phase, the fermionic [quasiparticle](../../../../../quasiparticle.md) contribution to [heat capacity](../../../../../heat-capacity.md) is exponentially suppressed at [temperatures](../../../../../temperature-split.md) well below the [pairing gap](../../../../../pairing-gap.md). Gapless collective modes can still give thermal terms following a [power law](../../../../../power-law.md). The [entropy](../../../../../entropy-split.md) nevertheless tends to zero. The normal Fermi-liquid law cannot be extrapolated through its pairing transition unchanged.[1996 Nobel lecture, discussion of [helium](../../../../../helium.md) isotopes and paired [superfluid](../../../../../superfluid.md) phases](../../../../../the-extraordinary-phases-of-liquid-3he-by-david-morris-lee.md)

[Helium-3](../../../../../helium-3.md) also illustrates the importance of [nuclear spin](../../../../../nuclear-spin.md) [entropy](../../../../../entropy-split.md). Over an intermediate low-temperature range, localized [spins](../../../../../spin.md) in the [solid](../../../../../solid.md) can retain approximately $k_B\ln2$ of [entropy](../../../../../entropy-split.md) per atom, while the degenerate [liquid](../../../../../liquid.md) has much less. Reversible conversion of [liquid](../../../../../liquid.md) to the higher-entropy [solid](../../../../../solid.md) then absorbs [heat](../../../../../heat-split.md); adiabatic compression along the [melting](../../../../../melting.md) curve can cool the sample. This is [Pomeranchuk cooling](../../../../../pomeranchuk-cooling.md). At still lower [temperature](../../../../../temperature-split.md), interactions between the nuclear [spins](../../../../../spin.md) remove this nearly free-spin [entropy](../../../../../entropy-split.md), so a constant $k_B\ln2$ cannot be extrapolated to [absolute zero](../../../../../absolute-zero.md).[1996 Nobel lecture, [entropy](../../../../../entropy-split.md) comparison and compression cooling](../../../../../the-pomeranchuk-effect-by-robert-coleman-richardson.md)

**Liquefaction and cooling methods.** A gas must be below its [liquid-gas critical point](../../../../../liquid-gas-critical-point.md) to form a distinct [liquid](../../../../../liquid.md) phase by compression. Compression above the [critical temperature](../../../../../critical-temperature.md) alone cannot achieve ordinary liquid-vapour coexistence. Practical liquefaction removes the compression [heat](../../../../../heat-split.md), cools the compressed gas in a [heat exchanger](../../../../../heat-exchanger.md) and uses expansion to lower its [temperature](../../../../../temperature-split.md) further.

A throttling valve operates approximately at constant [specific enthalpy](../../../../../specific-enthalpy.md) when kinetic-energy changes and [heat](../../../../../heat-split.md) leakage are negligible. The [Joule-Thomson coefficient](../../../../../joule-thomson-coefficient.md) is

$$
\mu_{\rm JT}=\left(\frac{\partial T}{\partial p}\right)_H
=\frac{T(\partial V/\partial T)_p-V}{C_p}
$$

using consistent molar quantities, or consistent total quantities for a fixed amount. A [pressure](../../../../../pressure-split.md) drop cools the gas if $\mu_{\rm JT}>0$. An [ideal gas](../../../../../ideal-gas-split.md) has zero [Joule-Thomson coefficient](../../../../../joule-thomson-coefficient.md); real intermolecular interactions are essential. In particular, room-temperature [helium](../../../../../helium.md) warms on throttling, so it must first be brought into a region of positive [Joule-Thomson coefficient](../../../../../joule-thomson-coefficient.md). Expansion through an engine or turbine can instead remove [work](../../../../../work.md) and produce approximately isentropic cooling.

A regenerative liquefier sends the cold returning gas through a [counterflow heat exchanger](../../../../../counterflow-heat-exchanger.md) to precool the incoming compressed gas before its next expansion. Expansion engines and external precooling can supply the initial cooling; repeated operation then produces [liquid](../../../../../liquid.md). Modern [helium](../../../../../helium.md) liquefaction commonly combines work-producing expansion with a final throttle. [Review of Refrigeration Methods, [helium](../../../../../helium.md) liquefiers and Claude cycles](https://trc.nist.gov/cryogenics/Papers/Review/2020-Review_of_Refrigeration_Methods.pdf)

Once [liquid](../../../../../liquid.md) exists, pumping away vapour lowers its [saturation pressure](../../../../../vapor-pressure.md) and boiling [temperature](../../../../../temperature-split.md). The escaping vapour carries [latent heat](../../../../../latent-heat.md) away, cooling the remaining [liquid](../../../../../liquid.md). At still lower [temperatures](../../../../../temperature-split.md), a [dilution refrigerator](../../../../../dilution-refrigerator.md) exploits the different [entropy](../../../../../entropy-split.md) carried by [helium-3](../../../../../helium-3.md) in concentrated and dilute [helium](../../../../../helium.md) mixtures; [adiabatic demagnetization](../../../../../adiabatic-demagnetization.md) and [Pomeranchuk cooling](../../../../../pomeranchuk-cooling.md) provide other routes.

**Approaching zero.** The unattainability formulation of the third law states that regular cooling operations with finite resources cannot reach [absolute zero](../../../../../absolute-zero.md) in finitely many stages. As the [entropy](../../../../../entropy-split.md) available to remove becomes small and thermal couplings weaken, each method loses its ability to take the final step. An isentropic cooling trajectory starting at nonzero [entropy](../../../../../entropy-split.md) cannot reach a common zero-entropy endpoint through regular finite changes of parameters. A fully general finite-time claim also requires assumptions about available controls and heat-transfer rates. **Quantum liquids and refrigeration methods can approach $0\,\mathrm K$ while remaining consistent with vanishing equilibrium [entropy](../../../../../entropy-split.md); they do not provide a finite-operation route to [absolute zero](../../../../../absolute-zero.md).**

## ↑ Ancestors (14)

1. [C13](../c13.md)
2. [Section C](../../section-c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2018](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
