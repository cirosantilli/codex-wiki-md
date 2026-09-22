# Limb-darkened disk flux

↑ **Parent:** [Limb darkening](limb-darkening.md)

For a circular stellar disk whose [specific intensity](spectral-radiance.md) is independent of [azimuth](azimuth.md), its mean [specific intensity](spectral-radiance.md) over [projected area](projected-area.md) is

$$
\overline I=\frac{1}{\pi R_\star^2}\int_{\rm disk} I\,dA_{\rm proj}
=2\int_0^1 I(\mu)\mu\,d\mu.
$$

The [polar coordinates](polar-coordinates.md) element is $dA_{\rm proj}=2\pi r\,dr$ after angular integration, and $r\,dr=-R_\star^2\mu\,d\mu$. Substitution of the [linear limb-darkening law](linear-limb-darkening-law.md) gives

$$
\overline I=2I_c\int_0^1(1-u+u\mu)\mu\,d\mu=I_c(1-u/3).
$$

For a distant observer at distance $D\gg R_\star$ receiving [light](light.md) normally to the detecting plane, the [observed radiative flux](observed-radiative-flux.md) is

$$
f_\nu\simeq\frac{\pi R_\star^2}{D^2}\overline I_\nu
=\pi\left(\frac{R_\star}{D}\right)^2I_{\nu,c}(1-u_\nu/3).
$$

It is spectral [irradiance](irradiance.md), with units $\mathrm{W\,m^{-2}\,Hz^{-1}}$ when $I_\nu$ is per hertz. The local outward [radiative flux](radiative-flux.md) per actual surface [area](surface-area.md) is instead $F_\nu=2\pi\int_0^1 I_\nu(\mu)\mu\,d\mu=\pi\overline I_\nu$, a spectral [radiant exitance](radiant-exitance.md). In a spherical model with the same [stellar atmosphere](stellar-atmosphere.md) everywhere, the [luminosity](luminosity.md) is $L_\nu=4\pi R_\star^2F_\nu$ and $f_\nu=L_\nu/(4\pi D^2)$, consistent with the [inverse-square law](inverse-square-law.md). Compare disks at fixed $I_c$ or fixed total [observed radiative flux](observed-radiative-flux.md) explicitly: increasing $u$ lowers the total in the first comparison, while the second requires a larger $I_c$.

## ↑ Ancestors (8)

1. [Limb darkening](limb-darkening.md)
2. [Spectral radiance](spectral-radiance.md)
3. [Radiance](radiance.md)
4. [Radiometry](radiometry-split.md)
5. [Optics](optics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Small-planet transit weighting](small-planet-transit-weighting.md)
