# Rayleigh scattering by a small sphere

↑ **Parent:** [Rayleigh scattering](rayleigh-scattering.md)

Consider a fixed, homogeneous, nonabsorbing, nonmagnetic [sphere](sphere.md) of [radius](radius.md) $a$ in [vacuum](vacuum.md). Let $m$ be its relative [refractive index](refractive-index.md), a fixed [real number](real-number.md); in [vacuum](vacuum.md) this equals the [sphere](sphere.md)'s [refractive index](refractive-index.md). Treat $m$ as independent of [wavelength](wavelength.md) over the range being compared, neglecting [optical dispersion](dispersion-optics.md). Air can be approximated by [vacuum](vacuum.md) here because its [refractive index](refractive-index.md) is close to one. These assumptions describe a toy particle, rather than a literal model of an individual air [molecule](molecule-split.md).

The [Rayleigh scattering cross-section](rayleigh-scattering-by-a-small-sphere.md) $\sigma$ is an effective [area](surface-area.md): the total scattered [power](power.md) is $P_{\rm sca}=I_{\rm inc}\sigma$, where $I_{\rm inc}$ is the incident [light intensity](light-intensity.md). For $ka\ll1$ its leading approximation is

$$
\sigma=\frac{8\pi}{3}k^4a^6\left(\frac{m^2-1}{m^2+2}\right)^2,\qquad k=\frac{2\pi}{\lambda}.
$$

The units are [area](surface-area.md), since $k^4a^6$ has units $\mathrm{m}^{-4}\mathrm{m}^6=\mathrm{m}^2$. This [Rayleigh scattering cross-section](rayleigh-scattering-by-a-small-sphere.md) measures scattering, not conversion of the incident [electromagnetic radiation](electromagnetic-radiation-split.md) into [heat](heat-split.md). The definition follows [Fitzpatrick, Thomson Scattering: total and differential scattering cross-sections](https://farside.ph.utexas.edu/teaching/jk1/lectures/node107.html).

To see the mechanism, the nearly uniform applied [electric field](electric-field-split.md) produces an [electric dipole moment](electric-dipole-moment.md) with peak magnitude

$$
p_0=4\pi\epsilon_0a^3\frac{m^2-1}{m^2+2}E_0,
$$

where $E_0$ is the incident [electric field](electric-field-split.md) peak [wave amplitude](wave-amplitude.md) and $\epsilon_0$ is [vacuum permittivity](vacuum-permittivity.md). This is the [sphere](sphere.md)'s response in [electrostatics](electrostatics-split.md), with its [permittivity](permittivity-split.md) divided by [vacuum permittivity](vacuum-permittivity.md) equal to $m^2$ under the nonmagnetic assumption. [Fitzpatrick, Boundary Value Problems with Dielectrics, equation 554: induced sphere dipole](https://farside.ph.utexas.edu/teaching/jk1/lectures/node42.html). The averaged [electric dipole radiation](electric-dipole-radiation.md) [power](power.md) is $P_{\rm sca}=\omega^4p_0^2/(12\pi\epsilon_0c^3)$, with [angular frequency](angular-frequency.md) $\omega=ck$ and [speed of light](speed-of-light.md) $c$. Dividing by $I_{\rm inc}=\epsilon_0cE_0^2/2$ gives the displayed [Rayleigh scattering cross-section](rayleigh-scattering-by-a-small-sphere.md). Thus doubling [radius](radius.md) multiplies the [electric dipole moment](electric-dipole-moment.md) by eight and the scattered [power](power.md) by $64$, provided the larger [sphere](sphere.md) still satisfies $ka\ll1$. [Fitzpatrick, Electric dipole radiation: angular power and its integral](https://farside.ph.utexas.edu/teaching/em/lectures/node95.html).

## ↑ Ancestors (6)

1. [Rayleigh scattering](rayleigh-scattering.md)
2. [Electromagnetic radiation](electromagnetic-radiation-split.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Rayleigh scattering](rayleigh-scattering.md)
- [Rayleigh scattering angular pattern](rayleigh-scattering-angular-pattern.md)
- [Scattering efficiency](scattering-efficiency.md)
