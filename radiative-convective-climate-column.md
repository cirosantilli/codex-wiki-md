# Radiative-convective climate column

↑ **Parent:** [Climate model](climate-model.md)

A [radiative-convective climate column](radiative-convective-climate-column.md) applies a [radiative-convective equilibrium model](radiative-convective-equilibrium-model.md) to the vertical thermal structure relevant to [climate change](climate-change.md). [Radiative transfer](radiative-transfer.md) determines heating and cooling; [convective adjustment](convective-adjustment.md) represents unresolved vertical redistribution when the chosen [atmospheric lapse rate](lapse-rate-atmosphere.md) is too steep. [Radiative equilibrium](radiative-equilibrium.md) alone need not give a physically admissible lower-atmospheric profile.

In 1967, [Syukuro Manabe](syukuro-manabe.md) and [Richard T. Wetherald](richard-t-wetherald.md) computed equilibrium with prescribed [relative humidity](relative-humidity.md), allowing atmospheric [water vapor](water-vapor.md) to change with [temperature](temperature-split.md). Their average-cloud case warmed by $2.36\,\mathrm K$ for [carbon dioxide](carbon-dioxide.md) increasing from 300 to 600 parts per million, versus $1.33\,\mathrm K$ with fixed absolute humidity. These are model outputs, not measured warming. The comparison isolates an important [water-vapor feedback](water-vapor-feedback.md).[Manabe and Wetherald, 1967, abstract; Section 4b, Table 5 and Fig. 16](thermal-equilibrium-of-the-atmosphere-with-a-given-distribution-of-relative-humidity-by-syukuro-manabe-and-richard-t-wetherald.md)

An original two-temperature calculation exposes the bookkeeping. Let an opaque surface absorb solar [irradiance](irradiance.md) $Q$ and emit [blackbody](blackbody.md) [thermal radiation](thermal-radiation.md) $\sigma T_s^4$. A single isothermal atmospheric layer transmits all sunlight and absorbs a fraction $\epsilon$ of surface infrared emission, emitting $\epsilon\sigma T_a^4$ both upward and downward. This is a grey thermal-band [emissivity](emissivity.md), with $0<\epsilon\leq1$. Let $H$ be upward nonradiative [heat flux](heat-flux-density.md), and let $C_s,C_a>0$ be [heat capacities](heat-capacity.md) per unit [area](surface-area.md). Then [conservation of energy](conservation-of-energy.md) gives

$$
C_s\dot T_s=Q+\epsilon\sigma T_a^4-\sigma T_s^4-H,
\qquad
C_a\dot T_a=\epsilon\sigma T_s^4-2\epsilon\sigma T_a^4+H.
$$

The two equations sum to

$$
\frac{d}{dt}(C_sT_s+C_aT_a)=Q-L,
\qquad
L=(1-\epsilon)\sigma T_s^4+\epsilon\sigma T_a^4.
$$

Here $L$ is [outgoing longwave radiation](outgoing-longwave-radiation.md). Both $H$ and downward atmospheric emission cancel internally: they redistribute [energy](energy-split.md) without creating it. The factor two in atmospheric emission counts two faces. Dropping the downward face would spoil the surface budget. Each right-hand term has units $\mathrm{W\,m^{-2}}$; each $C$ has units $\mathrm{J\,m^{-2}\,K^{-1}}$.

Choose $Q=240\,\mathrm{W\,m^{-2}}$, $H=80\,\mathrm{W\,m^{-2}}$ and $\epsilon=1$. At [equilibrium](equilibrium-point-of-a-dynamical-system.md), $L=\sigma T_a^4=240\,\mathrm{W\,m^{-2}}$ and $\sigma T_s^4=400\,\mathrm{W\,m^{-2}}$, giving $T_a\simeq255.06\,\mathrm K$ and $T_s\simeq289.81\,\mathrm K$. Direct substitution gives surface balance $240+240-400-80=0$ and atmospheric balance $400-480+80=0$. These deliberately chosen fluxes illustrate the model; they are not an observed global budget or a reconstruction of the 1967 calculation. Prescribing $H$ illustrates [heat transfer](heat-transfer.md) accounting but does not close a realistic [convection](convection-split.md) law.

<a id="image-a-conserving-climate-model-column-and-the-route-from-outgoing-radiance-to-a-spectral-comparison"></a>
![](climate-column-energy-and-spectral-readout.png)

**[Figure 3](#image-a-conserving-climate-model-column-and-the-route-from-outgoing-radiance-to-a-spectral-comparison). A conserving climate model column and the route from outgoing radiance to a spectral comparison**. The left panel uses the stipulated opaque-layer fluxes in watts per square metre. The right panel is a functional measurement diagram, not an observed spectrum. Broadband energy accounting and a directional spectral readout test different parts of the description.

For fixed $Q,H,\epsilon$, the positive-[temperature](temperature-split.md) [equilibrium](equilibrium-point-of-a-dynamical-system.md) is locally stable. Put $a=4\sigma T_s^3>0$ and $b=4\epsilon\sigma T_a^3>0$. The [Jacobian matrix](jacobian-matrix.md) of the temperature equations has [trace](matrix-trace.md) $-a/C_s-2b/C_a<0$ and [determinant](determinant.md) $ab(2-\epsilon)/(C_sC_a)>0$. Thus both [eigenvalues](eigenvalue.md) have negative real part. Temperature-dependent [climate feedbacks](climate-feedback.md) alter this test. A single grey layer also omits the [optical spectrum](optical-spectrum.md), cloud structure and the independent thermal behavior of the [troposphere](troposphere.md) and [stratosphere](stratosphere.md).

**Table of contents**

- [Convective adjustment](convective-adjustment.md)

## ↑ Ancestors (6)

1. [Climate model](climate-model.md)
2. [Climate change](climate-change.md)
3. [Geophysics](geophysics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Climate change](climate-change.md)
- [Climate model](climate-model.md)
- [Radiative-convective climate column](radiative-convective-climate-column.md)
