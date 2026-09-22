# Zero-dimensional planetary energy balance

↑ **Parent:** [Albedo](albedo.md)

Consider an idealized [planet](planet.md) that is a [sphere](sphere.md) of [radius](radius.md) $R$, illuminated by parallel sunlight of [irradiance](irradiance.md) $S$, measured on a plane perpendicular to the rays. Its intercepting [projected area](projected-area.md) is $\pi R^2$, whereas its total surface [area](surface-area.md) is $4\pi R^2$. Therefore the incoming [power](power.md) averaged per unit total surface [area](surface-area.md) is

$$
\frac{S\pi R^2}{4\pi R^2}=\frac S4,
\qquad P_{\rm abs}=(1-\alpha)S\pi R^2,
$$

where $\alpha$ is the broadband [Bond albedo](bond-albedo.md). The factor four is a [sphere](sphere.md) geometry result, not an atmospheric transmission factor. Local sunlight still varies over the illuminated hemisphere and vanishes on the dark side.

Now stipulate a single spatially uniform [temperature](temperature.md) $T$, no atmosphere, no internal heating, and [emissivity](emissivity.md) one for outgoing [thermal radiation](thermal-radiation.md). This is a thermal [blackbody](blackbody.md) model using the [Stefan–Boltzmann law](stefan-boltzmann-law.md); the prescribed solar-band reflection is treated separately, so the body is not a perfect absorber at all [wavelengths](wavelength.md). Let $C>0$ be the effective [heat capacity](heat-capacity.md) per unit surface [area](surface-area.md), in $\mathrm{J\,m^{-2}\,K^{-1}}$. [Conservation of energy](conservation-of-energy.md) gives the [ordinary differential equation](ordinary-differential-equation.md)

$$
C\frac{dT}{dt}=F(T),\qquad
F(T)=\frac S4[1-\alpha(T)]-\sigma T^4.
$$

Here $F$ is net heating per unit surface [area](surface-area.md), in $\mathrm{W\,m^{-2}}$, and $\sigma$ is the [Stefan-Boltzmann constant](stefan-boltzmann-constant.md). Use $\sigma=5.670374419\times10^{-8}\,\mathrm{W\,m^{-2}\,K^{-4}}$, rounded from the exact constant reported by NIST. [NIST, CODATA value: Stefan-Boltzmann constant](https://physics.nist.gov/cgi-bin/cuu/Value?sigma%7Csearch_for=stefan+boltzmann) The uniform [temperature](temperature.md) is a model assumption: generally the surface average of $T^4$ differs from the fourth power of the surface-average [temperature](temperature.md).

For fixed [Bond albedo](bond-albedo.md) $\alpha$, [radiative equilibrium](radiative-equilibrium.md) requires $F(T_*)=0$, giving

$$
T_* = \left[\frac{S(1-\alpha)}{4\sigma}\right]^{1/4}.
$$

With the illustrative [solar constant](solar-constant.md) $S=1360\,\mathrm{W\,m^{-2}}$, the global incoming average is $340\,\mathrm{W\,m^{-2}}$:

| Fixed [Bond albedo](bond-albedo.md) | Reflected average ($\mathrm{W\,m^{-2}}$) | Absorbed average ($\mathrm{W\,m^{-2}}$) | Equilibrium [temperature](temperature.md) ($\mathrm K$) |
| --- | --- | --- | --- |
| $0.30$ | $102$ | $238$ | $254.531$ |
| $0.60$ | $204$ | $136$ | $221.300$ |

Doubling [albedo](albedo.md) here lowers the equilibrium [temperature](temperature.md) by $33.231\,\mathrm K$, rather than halving it: the absorbed fraction changes from $0.7$ to $0.4$, and [thermal radiation](thermal-radiation.md) scales as $T^4$. These stipulated [Bond albedos](bond-albedo.md) are whole-planet examples, not measurements of bare water and ice. The model predicts neither [Earth](earth.md)'s modern surface [temperature](temperature.md) nor its response to actual [climate change](climate-change.md); it omits the [greenhouse effect](greenhouse-effect.md), spatial [heat transfer](heat-transfer.md) and seasons.

<a id="image-from-a-sunlit-disk-to-a-whole-sphere-geometry-and-fixed-albedo-energy-budgets"></a>
![](albedo-planet-energy-balance.png)

**[Figure 1](#image-from-a-sunlit-disk-to-a-whole-sphere-geometry-and-fixed-albedo-energy-budgets). From a sunlit disk to a whole sphere: geometry and fixed-albedo energy budgets**. The disk intercepts sunlight over area pi R squared; a uniform emitting sphere has four times that area. Both fixed-albedo examples use the same 1360 watts per square metre illumination and thermal emissivity one.

Each fixed-[albedo](albedo.md) [equilibrium](equilibrium-point-of-a-dynamical-system.md) is a [stable equilibrium](stable-equilibrium.md): for $T_*>0$, the [derivative](derivative.md) is $F'(T_*)=-4\sigma T_*^3<0$. A small [temperature](temperature.md) increase produces net cooling, and a small decrease produces net heating. This is the simplest expression of the stabilizing [Planck feedback](planck-feedback.md). Allowing [albedo](albedo.md) to fall with [temperature](temperature.md) adds a competing term, as in [ice-ocean albedo feedback](ice-ocean-albedo-feedback.md).

## ↑ Ancestors (5)

1. [Albedo](albedo.md)
2. [Geophysics](geophysics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Albedo](albedo.md)
- [Ice-ocean albedo feedback](ice-ocean-albedo-feedback.md)
