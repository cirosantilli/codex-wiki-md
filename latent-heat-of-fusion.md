# Latent heat of fusion

↑ **Parent:** [Statistical physics](statistical-physics-split.md)

An ice bath can absorb [heat](heat-split.md) while its [temperature](temperature-split.md) barely changes: the [heat](heat-split.md) converts [ice](ice.md) into [water](water.md). The [latent heat of fusion](latent-heat-of-fusion.md) quantifies this [melting](melting.md) budget. For a pure substance at its equilibrium [melting](melting.md) [temperature](temperature-split.md) $T_m(p)$ and specified [pressure](pressure-split.md) $p$, define it here per unit [mass](mass.md):

$$
L(p)=h_l(T_m(p),p)-h_s(T_m(p),p),\qquad h=H/m.
$$

Here $h_l$ and $h_s$ are the [specific enthalpies](specific-enthalpy.md) of the coexisting bulk [liquid](liquid.md) and [solid](solid.md), and $H$ is [enthalpy](enthalpy-split.md). For ordinary [melting](melting.md), $L>0$, in $\mathrm{J\,kg^{-1}}$; an amount $m$ has a total fusion [enthalpy](enthalpy-split.md) $mL$ in [joules](joule.md). A molar fusion [enthalpy](enthalpy-split.md) instead has units $\mathrm{J\,mol^{-1}}$ and equals $ML$, where $M=m/n$ is [mass](mass.md) divided by [amount of substance](amount-of-substance.md) in $\mathrm{kg\,mol^{-1}}$. Always check the normalization before inserting a tabulated value into an [energy](energy-split.md) balance.[§1.5: fusion and specific latent heat](university-physics-volume-2-by-samuel-j-ling-and-others/1-5-phase-changes.md) [IUPAC Gold Book, mass divided by amount of substance](https://goldbook.iupac.org/terms/view/12214)

For a [closed system](closed-system.md) converting completely from [solid](solid.md) to [liquid](liquid.md) at fixed [pressure](pressure-split.md), with only [pressure](pressure-split.md)-[volume](volume-thermodynamics.md) [work](work.md) and negligible changes in bulk [kinetic energy](kinetic-energy.md) and [potential energy](potential-energy.md), the [first law of thermodynamics](first-law-of-thermodynamics-split.md) gives $Q_p=\Delta H=mL$. Both endpoints are at $T_m(p)$: warming initially colder [ice](ice.md) or subsequently warming the resulting [water](water.md) requires additional [sensible heat](sensible-heat.md). Since $H=U+pV$, the corresponding [specific internal energy](specific-internal-energy.md) jump is $\Delta u=L-p\Delta v$, where $v=V/m$; $L$ includes the [work](work.md) associated with the change in [volume](volume-thermodynamics.md). [Heat](heat-split.md) is transferred [energy](energy-split.md), whereas [enthalpy](enthalpy-split.md) is a [state function](state-function.md). [David Tong, Statistical Physics, §4.4.1 and the first law](https://davidtong.org/teaching/statistical-physics/statmechhtml/S4#S4.SS4.SSS1)

<a id="image-during-equilibrium-melting-added-heat-changes-the-phase-fraction-while-temperature-stays-fixed"></a>
![](fusion-latent-heat-plateau.png)

**[Figure 3](#image-during-equilibrium-melting-added-heat-changes-the-phase-fraction-while-temperature-stays-fixed). During equilibrium melting, added heat changes the phase fraction while temperature stays fixed**. An original idealized ice-inspired model, not measured data: $m=0.100\,\mathrm{kg}$, $T_m=273.15\,\mathrm K$, constant [specific heat capacity at constant pressure](specific-heat-capacity-at-constant-pressure.md) in each phase, $c_s=2100$ and $c_l=4180\,\mathrm{J\,kg^{-1}\,K^{-1}}$, and $L=334000\,\mathrm{J\,kg^{-1}}$. The initial [solid](solid.md) is $10\,\mathrm K$ below $T_m$; the final [liquid](liquid.md) is $10\,\mathrm K$ above it. The horizontal axis is net sample [enthalpy](enthalpy-split.md) input, excluding the container.

Let $x=m_l/m$ be the [liquid](liquid.md) [phase fraction](phase-fraction.md) by [mass](mass.md), rather than by [volume](volume-thermodynamics.md). Neglecting interfacial contributions to [enthalpy](enthalpy-split.md), equilibrium [phase coexistence](phase-coexistence.md) at fixed [pressure](pressure-split.md) gives

$$
h=(1-x)h_s+xh_l=h_s+xL,\qquad Q_p=mL(x_2-x_1),\qquad T=T_m(p).
$$

In the model above, reaching $T_m$ takes $2.10\,\mathrm{kJ}$ of [sensible heat](sensible-heat.md); the plateau then absorbs $33.40\,\mathrm{kJ}$, ending at a cumulative $35.50\,\mathrm{kJ}$. At $18.80\,\mathrm{kJ}$, half the [mass](mass.md) is [liquid](liquid.md) and the [temperature](temperature-split.md) is still $T_m$. The final warming takes another $4.18\,\mathrm{kJ}$. The rounded $L$ and $c_l$ are inspired by the introductory [ice-melting calorimetry](ice-melting-calorimetry.md) values in Case Western's demonstration; constant properties and exact equilibrium throughout are stipulated model assumptions. [Case Western Reserve University, specific heat and heat of fusion demonstration](https://case.edu/artsci/phys/courses/demos/spec.htm)

Within one [thermodynamic phase](thermodynamic-phase.md), [specific heat capacity at constant pressure](specific-heat-capacity-at-constant-pressure.md) is $c_p=(\partial h/\partial T)_p$, in $\mathrm{J\,kg^{-1}\,K^{-1}}$; a sample's [heat capacity at constant pressure](heat-capacity-at-constant-pressure.md) is $C_p=mc_p$, in $\mathrm{J\,K^{-1}}$. The plateau is a finite [enthalpy](enthalpy-split.md) change at zero [temperature](temperature-split.md) change through varying $x$, so neither a finite single-phase $c_p$ nor $Q=mc_p\Delta T$ represents it. The [heating curve](heating-curve.md) needs separate [sensible heat](sensible-heat.md) intervals and a fusion contribution. [IUPAC Gold Book, heat capacity](https://goldbook.iupac.org/terms/view/H02753)

The plateau assumes a pure substance, a stable bulk [solid](solid.md)-[liquid](liquid.md) [phase coexistence](phase-coexistence.md) pair, fixed [pressure](pressure-split.md), and sufficiently slow, uniform heating to remain near [thermodynamic equilibrium](thermodynamic-equilibrium.md). The total [mass](mass.md) and composition must remain fixed, with negligible evaporation and no other [phase transition](phase-transition.md). A fast heater can produce [temperature](temperature-split.md) gradients, so a local [thermometer](thermometer.md) need not read the equilibrium $T_m$. Neither $T_m$ nor $L$ is universal across [pressures](pressure-split.md) or compositions: [common-pressure melting-point slope](common-pressure-melting-point-slope.md) describes the pressure dependence of $T_m$, while mixtures can melt over a [temperature](temperature-split.md) range as their coexisting compositions change. Their [liquidus](liquidus.md) must be consulted instead of assuming a pure-substance plateau. [Stephen A. Nelson, Tulane, Two Component Phase Diagrams, pp. 2–4: melting ranges and liquidus](https://www2.tulane.edu/~sanelson/eens211/2compphasdiag.pdf#page=3)

This makes [ice](ice.md) useful as a [temperature](temperature-split.md) buffer: under these conditions it can absorb $m_sL$ before the remaining [solid](solid.md) [mass](mass.md) $m_s$ disappears, after which the [water](water.md) warms. If a stipulated constant net input [power](power.md) $P$ goes entirely into [melting](melting.md), that buffer lasts $m_sL/P$. Reversing the equilibrium conversion releases the same fusion [enthalpy](enthalpy-split.md) during [freezing](freezing.md). The beautiful thermodynamic connection is $L=T_m(s_l-s_s)$, with $s$ the [specific entropy](specific-entropy.md) and $T_m$ absolute [temperature](temperature-split.md): equal [Gibbs free energies](gibbs-free-energy.md) at [phase coexistence](phase-coexistence.md) allow different [enthalpies](enthalpy-split.md) and [entropies](entropy-split.md). The nearly stationary [thermometer](thermometer.md) hides a finite, measurable change of state. [Tong, Statistical Physics, §5.1.2: coexistence and latent heat](statistical-physics-by-david-tong.md)

**Table of contents**

- [Ice-melting calorimetry](ice-melting-calorimetry.md)
  - [Wet-ice bias in fusion calorimetry](wet-ice-bias-in-fusion-calorimetry.md)

## ↑ Ancestors (4)

1. [Statistical physics](statistical-physics-split.md)
2. [Branches of physics](branches-of-physics.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Common-pressure melting-point slope](common-pressure-melting-point-slope.md)
- [Iceberg melt heat budget](iceberg-melt-heat-budget.md)
- [Latent heat of fusion](latent-heat-of-fusion.md)
- [Negative melting-point slope of water](negative-melting-point-slope-of-water.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-77/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-77/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-69/1/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-1/section-a/a4/solution.md)
- [Pomeranchuk cooling](pomeranchuk-cooling.md)
- [Sensible heat](sensible-heat.md)
- [Wet-ice bias in fusion calorimetry](wet-ice-bias-in-fusion-calorimetry.md)
