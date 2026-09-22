# Radiant exitance

↑ **Parent:** [Radiometry](radiometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radiant_exitance)

[Radiant exitance](radiant-exitance.md) is total outward emitted [radiant flux](radiant-flux.md) per actual emitting [area](surface-area.md), measured in $\mathrm{W\,m^{-2}}$. Integrate [radiance](radiance.md) over the outward [hemisphere](hemisphere.md), keeping the [projected area](projected-area.md) factor:

$$
M=\int_{\Omega_{\rm outward}}L(\theta,\varphi)\cos\theta\,d\Omega.
$$

If the [radiance](radiance.md) is direction-independent, the [spherical coordinates](spherical-coordinate-system.md) element is $d\Omega=\sin\theta\,d\theta\,d\varphi$, so

$$
M=L\int_0^{2\pi}\!d\varphi\int_0^{\pi/2}\cos\theta\sin\theta\,d\theta=\pi L.
$$

The weighted [solid angle](solid-angle.md) is $\pi\,\mathrm{sr}$, although the whole [hemisphere](hemisphere.md) covers $2\pi\,\mathrm{sr}$. Directions near grazing contribute less because of the [projected area](projected-area.md). This geometric factor is the bridge between [Lambert's cosine law](lambert-s-cosine-law.md) and the total output of a diffuse patch. [Breinig, Radiometry: hemispherical integration of radiance](https://labs.phys.utk.edu/mbreinig/phys421/modules/m5/Radiometry.html).

For the uniform patch with $L=10\,\mathrm{W\,m^{-2}\,sr^{-1}}$, [radiant exitance](radiant-exitance.md) is $M=10\pi\,\mathrm{W\,m^{-2}}$. Its [area](surface-area.md) $0.020\,\mathrm{m^2}$ gives total [radiant flux](radiant-flux.md) $\Phi=MA=0.20\pi\,\mathrm W\approx0.628319\,\mathrm W$ over the outward [hemisphere](hemisphere.md). This total differs from its [radiant intensity](radiant-intensity.md) $I(0)=0.20\,\mathrm{W\,sr^{-1}}$, which describes only one direction.

For an ideal [blackbody](blackbody.md), integrate [Planck's law](planck-s-law.md) over [frequency](frequency.md) as well: $M=M_e=j^*=\sigma T^4$ by the [Stefan–Boltzmann law](stefan-boltzmann-law.md). An ideal $6000\,\mathrm K$ emitting patch of [area](surface-area.md) $1\,\mathrm{mm^2}$ emits about $73.4881\,\mathrm W$ outward. [Irradiance](irradiance.md) counts incoming radiation separately; for purely emitted output the net outward exchange per [area](surface-area.md) is $M-E$. Reflected output must also be included if the surface reflects incident radiation.

## ↑ Ancestors (5)

1. [Radiometry](radiometry.md)
2. [Optics](optics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Black-body radiation](black-body-radiation.md)
- [Irradiance](irradiance.md)
- [Lambertian reflectance](lambertian-reflectance.md)
- [Limb-darkened disk flux](limb-darkened-disk-flux.md)
- [Planck's law](planck-s-law.md)
- [Radiance](radiance.md)
- [Radiant exitance](radiant-exitance.md)
- [Radiant flux through an oriented surface](radiant-flux-through-an-oriented-surface.md)
- [Radiometry](radiometry.md)
