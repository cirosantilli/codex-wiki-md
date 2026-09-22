# Sensible heat

↑ **Parent:** [Heat](heat.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sensible_heat)

Sensible heat is transferred [heat](heat.md) associated with a [temperature](temperature.md) change within a single [thermodynamic phase](thermodynamic-phase.md). By contrast, [latent heat](latent-heat.md) can change the [phase fraction](phase-fraction.md) while the [temperature](temperature.md) stays fixed during equilibrium [phase coexistence](phase-coexistence.md). Neither name denotes an additional stored substance: both describe how transferred [heat](heat.md) participates in a process.

For fixed [mass](mass.md) $m$ and composition, use the [heat capacity](heat-capacity.md) appropriate to the heating constraint. Under the [quasistatic process](quasistatic-process.md) assumptions in [heat capacity](heat-capacity.md), with only [pressure](pressure.md)-[volume](volume-thermodynamics.md) [work](work.md) and unchanged bulk [kinetic energy](kinetic-energy.md) and [potential energy](potential-energy.md), fixed-[pressure](pressure.md) heating gives

$$
Q_{\rm sens}=m\int_{T_1}^{T_2}c_p(T)\,dT,
\qquad Q_{\rm sens}=mc_p(T_2-T_1)\quad\text{if }c_p\text{ is constant}.
$$

Here $c_p$ is [specific heat capacity at constant pressure](specific-heat-capacity-at-constant-pressure.md); fixed-[volume](volume-thermodynamics.md) heating instead uses [specific heat capacity at constant volume](specific-heat-capacity-at-constant-volume.md) $c_V$. A cooling step has negative $Q_{\rm sens}$ with the sign convention in [heat](heat.md). A [temperature](temperature.md) difference has the same numerical value in units of the [kelvin](kelvin.md) or [degree Celsius](degree-celsius.md). The [integral](integral.md) follows by adding the small transfers $\delta Q=mc_p(T)\,dT$, rather than assuming a constant [heat capacity](heat-capacity.md).

As a stylized [ice](ice.md)-to-[water](water.md) example for a fixed-composition [closed system](closed-system.md) at fixed [pressure](pressure.md) $1\,\mathrm{atm}$, take $m=0.5\,\mathrm{kg}$, an initial [temperature](temperature.md) of $-10\,{}^\circ\mathrm C$, [melting](melting.md) at $0\,{}^\circ\mathrm C$, and a final [temperature](temperature.md) of $20\,{}^\circ\mathrm C$. Assume constant [specific heat capacity at constant pressure](specific-heat-capacity-at-constant-pressure.md) values $c_{\rm ice}=2.1\,\mathrm{kJ\,kg^{-1}\,K^{-1}}$ and $c_{\rm water}=4.18\,\mathrm{kJ\,kg^{-1}\,K^{-1}}$, and [latent heat of fusion](latent-heat-of-fusion.md) $L_f=334\,\mathrm{kJ\,kg^{-1}}$. These are stipulated, rounded model values; ignore the container and [heat](heat.md) losses, retain all the material, and assume only [pressure](pressure.md)-[volume](volume-thermodynamics.md) [work](work.md) under the [quasistatic process](quasistatic-process.md) conditions above. The three steps are

$$
\begin{aligned}
Q_{\rm ice}&=0.5\times2.1\times10=10.5\,\mathrm{kJ},\\
Q_{\rm melt}&=0.5\times334=167\,\mathrm{kJ},\\
Q_{\rm water}&=0.5\times4.18\times20=41.8\,\mathrm{kJ},\\
Q_{\rm total}&=10.5+167+41.8=219.3\,\mathrm{kJ}.
\end{aligned}
$$

Only the first and third terms are [sensible heat](sensible-heat.md); the middle term is [latent heat](latent-heat.md). The plateau begins after $10.5\,\mathrm{kJ}$ and ends after $177.5\,\mathrm{kJ}$ of total supplied [heat](heat.md). At $94\,\mathrm{kJ}$ total input, half the [mass](mass.md) is [liquid](liquid.md) [water](water.md) and the [temperature](temperature.md) remains $0\,{}^\circ\mathrm C$. The equilibrium [phase transition](phase-transition.md) [temperature](temperature.md) depends on [pressure](pressure.md); this example stipulates a single fixed [pressure](pressure.md). [1.5 Phase Changes](university-physics-volume-2-by-samuel-j-ling-and-others/1-5-phase-changes.md)

<a id="image-heating-0-5-mathrm-kg-of-ice-to-water-sensible-heat-and-latent-heat"></a>
![](sensible-and-latent-heating-curve.png)

**[Figure 32](#image-heating-0-5-mathrm-kg-of-ice-to-water-sensible-heat-and-latent-heat). Heating $0.5\,\mathrm{kg}$ of ice to water: sensible heat and latent heat**. Illustrative fixed-[pressure](pressure.md) [heating curve](heating-curve.md) using the constant parameters above. The sloping portions raise [temperature](temperature.md); the long $0\,{}^\circ\mathrm C$ plateau changes the [phase fraction](phase-fraction.md). Total supplied [heat](heat.md) is measured from the initial [ice](ice.md) state and equals the [enthalpy](enthalpy.md) change under the stated assumptions.

This split makes heating budgets easy to interpret: [melting](melting.md) consumes $167/219.3\approx76.2\%$ of the supplied [heat](heat.md) in this model despite causing no [temperature](temperature.md) rise. Within either single [thermodynamic phase](thermodynamic-phase.md), the [heating curve](heating-curve.md) slope is $dT/dQ=1/(mc_p)$; a larger [heat capacity](heat-capacity.md) makes the slope shallower. A flat interval represents changing [phase fraction](phase-fraction.md), so it cannot be modeled by applying $Q=mc_p\Delta T$ across the [phase transition](phase-transition.md). The complementary constructed example in [latent heat](latent-heat.md) tracks that [phase fraction](phase-fraction.md) explicitly.

## ↑ Ancestors (6)

1. [Heat](heat.md)
2. [Thermodynamics](thermodynamics-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Enthalpy](enthalpy.md)
- [Heat](heat.md)
- [Heating curve](heating-curve.md)
- [Ice-melting calorimetry](ice-melting-calorimetry.md)
- [Latent heat](latent-heat.md)
- [Latent heat of fusion](latent-heat-of-fusion.md)
- [Sensible heat](sensible-heat.md)
- [Specific heat capacity at constant pressure](specific-heat-capacity-at-constant-pressure.md)
- [Wet-ice bias in fusion calorimetry](wet-ice-bias-in-fusion-calorimetry.md)
