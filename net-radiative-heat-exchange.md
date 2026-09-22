# Net radiative heat exchange

↑ **Parent:** [Stefan–Boltzmann law](stefan-boltzmann-law.md)

For a small, uniform surface at [temperature](temperature-split.md) $T$, enclosed by much larger black walls all at [temperature](temperature-split.md) $T_s$, the outward net [heat transfer](heat-transfer.md) by [thermal radiation](thermal-radiation.md) is

$$
\dot Q_{\rm rad}=\epsilon\sigma A(T^4-T_s^4).
$$

Assume an opaque [grey body](grey-body.md) that is a [diffuse thermal emitter](diffuse-thermal-emitter.md), with the same [emissivity](emissivity.md) $\epsilon$ and [radiometric absorptance](radiometric-absorptance.md) at the surface's current [temperature](temperature-split.md). Its emitting [area](surface-area.md) $A$ sees only the enclosure: the [view factor](view-factor.md) to the walls is one, with no self-viewing surface, opening or intervening obstruction. The intervening medium must neither absorb nor emit appreciable [thermal radiation](thermal-radiation.md); a [vacuum](vacuum.md) supplies a useful idealization. The enclosure is maintained at uniform $T_s$. The small-body assumption makes that reservoir description physically reasonable; genuinely black isothermal walls supply the incoming [irradiance](irradiance.md) even without an infinite area ratio. Positive $\dot Q_{\rm rad}$ means net loss by the surface; negative means net gain. This expression counts [thermal radiation](thermal-radiation.md) alone, not all [heat transfer](heat-transfer.md).[§19.1, cavity irradiance; §19.2, grey-body absorptance/emittance; §19.4, enclosed-body view factor one](thermodynamics-and-propulsion.md)

The reasoning is a two-way [energy](energy-split.md) balance. Black walls supply [irradiance](irradiance.md) $E=\sigma T_s^4$, so the surface absorbs $P_{\rm abs}=\epsilon AE$ and emits $P_{\rm emit}=\epsilon A\sigma T^4$. Subtract these to obtain $\dot Q_{\rm rad}$. For an opaque surface the remaining fraction $1-\epsilon$ of incoming [radiant flux](radiant-flux.md) is reflected; counting emitted plus reflected outgoing [radiant flux](radiant-flux.md) minus total incoming [radiant flux](radiant-flux.md) gives the same result. [Kirchhoff's law of thermal radiation](kirchhoff-s-law-of-thermal-radiation.md) justifies equal spectral absorption and emission factors; the [grey body](grey-body.md) assumption lets one factor be taken outside both spectral [integrals](integral-split.md).

Choose $\epsilon=0.8$, $A=0.01\,\mathrm{m^2}$, $T=500\,\mathrm K$ and $T_s=300\,\mathrm K$. These are stipulated model inputs, not measured material properties. Using $\sigma\approx5.670374419\times10^{-8}\,\mathrm{W\,m^{-2}\,K^{-4}}$ gives

$$
P_{\rm emit}\approx28.3519\,\mathrm W,\qquad
P_{\rm abs}\approx3.6744\,\mathrm W,\qquad
\dot Q_{\rm rad}\approx24.6775\,\mathrm W.
$$

The incoming [irradiance](irradiance.md) is $459.300\,\mathrm{W\,m^{-2}}$, corresponding to $4.5930\,\mathrm W$ incident on the surface; only $80\%$ is absorbed. At $T=T_s=300\,\mathrm K$, emitted and absorbed [powers](power.md) are both $3.6744\,\mathrm W$, so [radiative equilibrium](radiative-equilibrium.md) has zero net exchange despite continuing emission. Changing only [emissivity](emissivity.md) to $0.2$ reduces both one-way [powers](power.md) and the net loss by a factor of four, giving $6.1694\,\mathrm W$ net. A low-[emissivity](emissivity.md) coating therefore suppresses both radiative cooling to colder walls and radiative heating from hotter walls.

<a id="image-two-way-exchange-in-a-black-enclosure-and-the-effect-of-emissivity"></a>
![](grey-surface-black-enclosure-exchange.png)

**[Figure 10](#image-two-way-exchange-in-a-black-enclosure-and-the-effect-of-emissivity). Two-way exchange in a black enclosure and the effect of emissivity**. Original schematic, not an experimental apparatus. The central convex body has total emitting [area](surface-area.md) $0.01\,\mathrm{m^2}$, [temperature](temperature-split.md) $500\,\mathrm K$ and [view factor](view-factor.md) one to black walls at $300\,\mathrm K$. Arrows show gross emission, absorbed enclosure radiation and reflected enclosure radiation for [emissivity](emissivity.md) $0.8$; widths are illustrative. The graph compares stipulated [emissivities](emissivity.md) under the same geometry and [temperatures](temperature-split.md).

Near equal [temperatures](temperature-split.md), write $T=T_s+\Delta T$. [Taylor's theorem](taylor-s-theorem.md) gives

$$
\dot Q_{\rm rad}=4\epsilon\sigma AT_s^3\Delta T+O((\Delta T)^2),
\qquad h_{\rm rad}=4\epsilon\sigma T_s^3.
$$

For constant [emissivity](emissivity.md), the radiative [heat transfer coefficient](heat-transfer-coefficient.md) $h_{\rm rad}$ is approximately $4.8992\,\mathrm{W\,m^{-2}\,K^{-1}}$ at $T_s=300\,\mathrm K$ and $\epsilon=0.8$. This local linear approximation is useful for small [temperature](temperature-split.md) differences; the $200\,\mathrm K$ difference in the worked example needs the full fourth-power expression.

A cooling experiment requires a wider [first law of thermodynamics](first-law-of-thermodynamics-split.md) balance. In a uniform-[temperature](temperature-split.md) model without a heater,

$$
C(T)\frac{dT}{dt}=-\dot Q_{\rm rad}-\dot Q_{\rm conv}-\dot Q_{\rm cond},
$$

where $C(T)$ is the sample's [heat capacity](heat-capacity.md) and the last two terms are signed outward [convection](convection-split.md) and [thermal conduction](thermal-conduction.md) losses. A [vacuum](vacuum.md) suppresses [convection](convection-split.md) but does not eliminate [thermal conduction](thermal-conduction.md) through supports or sensor leads. A cooling slope therefore cannot establish [emissivity](emissivity.md) unless these paths and [heat capacity](heat-capacity.md) are independently constrained. Multiple wall [temperatures](temperature-split.md), incomplete [view factors](view-factor.md), wavelength-selective materials or appreciable intervening absorption require a more complete [radiative transfer](radiative-transfer.md) calculation.

**Table of contents**

- [View factor](view-factor.md)

## ↑ Ancestors (7)

1. [Stefan–Boltzmann law](stefan-boltzmann-law.md)
2. [Heat](heat-split.md)
3. [Thermodynamics](thermodynamics-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Comparing surface emission at equal temperature](comparing-surface-emission-at-equal-temperature.md)
- [Grey body](grey-body.md)
- [Stefan–Boltzmann law](stefan-boltzmann-law.md)
