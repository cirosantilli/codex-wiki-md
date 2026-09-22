# U-tube differential manometer

↑ **Parent:** [Manometer](manometer.md)

A [U-tube differential manometer](u-tube-differential-manometer.md) contains a connected column of [liquid](liquid.md) with one [gas](gas.md) connection above each [liquid meniscus](meniscus-liquid-surface.md). Write $p_L,p_R$ for the left and right [pressures](pressure-split.md), and $z_L,z_R$ for the meniscus heights on an upward vertical coordinate. Assume constant [mass density](density.md) $\rho$ and downward [gravitational acceleration](gravitational-acceleration.md) of magnitude $g$; neglect the [gas](gas.md) column's [mass density](density.md) and differences in [capillary pressure](capillary-pressure.md). The signed vertical [length](length.md) difference $\Delta h=z_R-z_L$ then gives

$$
\Delta p=p_L-p_R=\rho g\Delta h.
$$

Larger left [pressure](pressure-split.md) means a lower left [liquid meniscus](meniscus-liquid-surface.md): $p_L>p_R$ implies $z_L<z_R$. Equal [pressures](pressure-split.md) give equal meniscus heights.

<a id="image-a-u-tube-differential-manometer-higher-left-pressure-lowers-the-left-liquid-meniscus"></a>
![](manometer-u-tube-signed-height.png)

**[Figure 3](#image-a-u-tube-differential-manometer-higher-left-pressure-lowers-the-left-liquid-meniscus). A U-tube differential manometer: higher left pressure lowers the left liquid meniscus**. Original schematic of two same-height [pressure tappings](pressure-tapping.md) connected to a resting [water](water.md) column. The constructed example uses $z_L=-30\,\mathrm{mm}$ and $z_R=30\,\mathrm{mm}$, so the vertical difference is $60\,\mathrm{mm}$. Dashed lines mark both meniscus heights and the equal-pressure datum; the dotted bottom line identifies two equal-height [points](point-geometry.md) within the connected [liquid](liquid.md). The arrow in the pipe indicates [fluid flow](fluid-flow.md); the [manometer](manometer.md) [liquid](liquid.md) has no continuing flow at equilibrium.

The balance follows directly from [hydrostatic pressure](hydrostatic-pressure.md). At a common height $z_0$ below both surfaces, the two [points](point-geometry.md) in the connected homogeneous [liquid](liquid.md) have equal [pressure](pressure-split.md):

$$
p_L+\rho g(z_L-z_0)=p_R+\rho g(z_R-z_0).
$$

Subtracting cancels the common bottom depth and leaves $p_L-p_R=\rho g(z_R-z_L)$. The same-height rule follows from [hydrostatic equilibrium](hydrostatic-equilibrium.md), $\nabla p=-\rho g\mathbf e_z$: a horizontal displacement changes no [pressure](pressure-split.md), and for constant $\rho$ the quantity $p+\rho gz$ is constant throughout the connected [liquid](liquid.md). Equal height alone is insufficient for unrelated vessels or for [fluid flow](fluid-flow.md) with significant [acceleration](acceleration.md).

For an original constructed example, choose [water](water.md) of stipulated [mass density](density.md) $\rho=1000\,\mathrm{kg\,m^{-3}}$, [gravitational acceleration](gravitational-acceleration.md) $g=9.81\,\mathrm{m\,s^{-2}}$, and vertical [length](length.md) difference $\Delta h=0.060\,\mathrm m$. Then

$$
\Delta p=1000\times9.81\times0.060=588.6\,\mathrm{Pa}.
$$

The [SI](international-system-of-units.md) [pressure](pressure-split.md) unit is the [pascal](pascal-unit.md): the product has units $\mathrm{kg\,m^{-3}}\times\mathrm{m\,s^{-2}}\times\mathrm m=\mathrm{kg\,m^{-1}\,s^{-2}}=\mathrm{Pa}$. Swapping the two connections gives $-588.6\,\mathrm{Pa}$ and reverses which [liquid meniscus](meniscus-liquid-surface.md) is lower. In equal-bore arms, [volume conservation](volume-conservation.md) makes each surface move $30\,\mathrm{mm}$ from its initial equal-height position; using only one surface's displacement would halve the inferred [pressure](pressure-split.md). With unequal arm [areas](surface-area.md) $A_L,A_R$, a left fall $a$ and right rise $b$ instead obey $A_La=A_Rb$, while the vertical [length](length.md) difference is still $a+b$.

If the right port is open to the local atmosphere, $p_L-p_R$ is the left [gauge pressure](gauge-pressure.md). Only with that reference and known [atmospheric pressure](atmospheric-pressure.md) can one obtain [absolute pressure](absolute-pressure.md) from

$$
p_{L,\mathrm{abs}}=p_{\mathrm{atmosphere}}+p_{L,\mathrm{gauge}}.
$$

For an explicitly stipulated [atmospheric pressure](atmospheric-pressure.md) of $100000\,\mathrm{Pa}$, the example gives $100588.6\,\mathrm{Pa}$ [absolute pressure](absolute-pressure.md). If the right port is connected to another vessel or a [pressure tapping](pressure-tapping.md), the same reading is a differential [pressure](pressure-split.md) and supplies no [absolute pressure](absolute-pressure.md) without knowing that reference.[§14.2, Gauge Pressure vs. Absolute Pressure, equation 14.11; Manometers](university-physics-volume-1-by-william-moebs-and-others.md)

**Table of contents**

- [Manometer height-to-pressure calibration](manometer-height-to-pressure-calibration.md)
- [Water-column wind-tunnel pressure measurement](water-column-wind-tunnel-pressure-measurement.md)

## ↑ Ancestors (5)

1. [Manometer](manometer.md)
2. [Fluid mechanics](fluid-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [U-tube differential manometer](u-tube-differential-manometer.md)
