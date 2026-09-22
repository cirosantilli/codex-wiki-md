# Cosmic-ray altitude attenuation model

↑ **Parent:** [Hess cosmic-ray balloon experiment](hess-cosmic-ray-balloon-experiment.md)

An original [cosmic-ray altitude attenuation model](cosmic-ray-altitude-attenuation-model.md) illustrates how competing origins can produce a dip followed by a rise. It is a hypothetical absorption calculation, not a reconstruction or fit of Hess's measurements, and it excludes [air shower](air-shower.md) production. Put $z$ for height above a flat ground surface and assume gas [density](density.md) $\rho(z)=\rho_0e^{-z/H}$ with constant scale $H$. The overlying atmospheric mass per unit area is

$$
X(z)=\int_z^\infty\rho(h)\,dh=\rho_0H e^{-z/H},\qquad X_0=\rho_0H.
$$

Let $G$ denote a ground-origin contribution attenuated by material below the chamber, and $E$ a downward extraterrestrial contribution attenuated by material above it. Assume constant attenuation mass columns $\Lambda_g,\Lambda_e>0$:

$$
G(z)=G_0\exp\left[-\frac{X_0-X(z)}{\Lambda_g}\right],\qquad E(z)=E_{\rm top}\exp\left[-\frac{X(z)}{\Lambda_e}\right],\qquad q_{\rm fixed}(z)=B+G(z)+E(z).
$$

These are rates at a fixed detector gas [density](density.md), in arbitrary common units. The constant $B$ represents residual background. The equation $dI/dX=-I/\Lambda$ gives [exponential function](exponential-function.md) attenuation along each propagation direction. Thus $G$ decreases and $E$ increases as $z$ increases; their sum need not be monotone. The different arguments of the two [exponential functions](exponential-function.md) encode the entire geometric idea.

<a id="image-competing-altitude-trends-and-the-gas-density-confound"></a>
![](cosmic-ray-competing-altitude-models.png)

**[Figure 2](#image-competing-altitude-trends-and-the-gas-density-confound). Competing altitude trends and the gas-density confound**. Original hypothetical curves for the [cosmic-ray altitude attenuation model](cosmic-ray-altitude-attenuation-model.md), with no historical data points. Left: ground-only and ground-plus-extraterrestrial explanations at fixed detector gas [density](density.md). Right: the same mixed radiation field with fixed gas [density](density.md) or a vented chamber, each normalized to its own ground value.

The figure chooses $H=8\,\mathrm{km}$, $G_0=0.8$, $E_{\rm top}=6$, $B=0.15$, $\Lambda_g=0.08X_0$ and $\Lambda_e=0.45X_0$, all for illustration. Differentiation gives

$$
\frac{dq_{\rm fixed}}{dz}=\frac{X(z)}H\left(\frac{E(z)}{\Lambda_e}-\frac{G(z)}{\Lambda_g}\right).
$$

The minimum occurs where $E/\Lambda_e=G/\Lambda_g$, at approximately $1.13\,\mathrm{km}$ for these invented parameters. At $6\,\mathrm{km}$ the fixed-gas response is about $1.41$ times its ground value, but multiplying by $\rho(z)/\rho_0$ gives an uncorrected vented-chamber response of only $0.66$ times its ground value. A real increase in radiation response per gas mass can therefore be hidden by a decrease in target gas [density](density.md). This is the reason to distinguish radiation from the amount of gas being irradiated.

The model treats propagation as attenuation without generating new particles. Real [primary cosmic rays](primary-cosmic-ray.md) interact, redistribute energy and produce [air showers](air-shower.md); an atmospheric profile need not follow either simple [exponential function](exponential-function.md). The model also holds backgrounds and detector response fixed. Its value is to expose the sign of competing effects and the [density](density.md) confound, while Hess's experimental argument depends on his actual comparisons and instrument limitations.

## ↑ Ancestors (9)

1. [Hess cosmic-ray balloon experiment](hess-cosmic-ray-balloon-experiment.md)
2. [Cosmic ray](cosmic-ray.md)
3. [Interstellar medium](interstellar-medium.md)
4. [Milky Way](milky-way.md)
5. [Galaxy](galaxy-split.md)
6. [Astrophysics](astrophysics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Cosmic-ray altitude attenuation model](cosmic-ray-altitude-attenuation-model.md)
