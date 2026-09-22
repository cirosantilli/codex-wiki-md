# Radiance

↑ **Parent:** [Radiometry](radiometry-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radiance)

[Radiance](radiance.md) resolves both position and direction: it is [radiant flux](radiant-flux.md) per [projected area](projected-area.md) and per [solid angle](solid-angle.md). For a surface element of [area](surface-area.md) $dA$, and a small outgoing cone $d\Omega$ at [angle](angle.md) $0\leq\theta<\pi/2$ to its outward [unit normal](unit-normal.md),

$$
d^2\Phi=L(\mathbf x,\mathbf s)\cos\theta\,dA\,d\Omega,
\qquad [L]=\mathrm{W\,m^{-2}\,sr^{-1}}.
$$

Here $\mathbf x$ locates the patch and $\mathbf s$ is a [unit vector](unit-vector.md) along the outgoing direction. The factor $dA\cos\theta$ is the patch's apparent [area](surface-area.md) viewed along that direction. The same local definition applies to transmitted or received radiation, choosing the positive [projected area](projected-area.md) for the crossing direction. [Marianne Breinig, University of Tennessee, Radiometry: radiance and Lambert's law](https://labs.phys.utk.edu/mbreinig/phys421/modules/m5/Radiometry.html).

For a planar patch of [area](surface-area.md) $A$ with spatially uniform, direction-independent [radiance](radiance.md) $L$, integrating over the patch gives

$$
I(\theta)=LA\cos\theta.
$$

Take $L=10\,\mathrm{W\,m^{-2}\,sr^{-1}}$ and $A=0.020\,\mathrm{m^2}$. The [radiant intensities](radiant-intensity.md) are $I(0)=0.20\,\mathrm{W\,sr^{-1}}$ and $I(60^\circ)=0.10\,\mathrm{W\,sr^{-1}}$. A sufficiently narrow $0.010\,\mathrm{sr}$ cone therefore carries approximately $2.0\,\mathrm{mW}$ or $1.0\,\mathrm{mW}$, respectively. Both views have the same [radiance](radiance.md) $L$: the oblique view presents half the [projected area](projected-area.md). This is [Lambert's cosine law](lambert-s-cosine-law.md), not a loss of [radiance](radiance.md) with viewing [angle](angle.md).

<a id="image-one-uniform-patch-halving-projected-area-halves-radiant-intensity-while-preserving-radiance"></a>
![](projected-area-radiance.png)

**[Figure 3](#image-one-uniform-patch-halving-projected-area-halves-radiant-intensity-while-preserving-radiance). One uniform patch: halving projected area halves radiant intensity while preserving radiance**. The geometric panels show a cross-section of a rectangular patch with the same depth perpendicular to the page. Parallel projection onto a plane perpendicular to the viewing direction changes its width by $\cos\theta$. The graph gives $I(\theta)=LA\cos\theta$ for the stated patch and marks the exact $0^\circ$ and $60^\circ$ cases.

[Radiance](radiance.md) is useful because it separates a source's local directional output from the geometry of an observation. Integrating over outgoing directions gives [radiant exitance](radiant-exitance.md); integrating incoming [radiance](radiance.md) at a receiver gives [irradiance](irradiance.md). In the stationary [vacuum](vacuum.md) setting of [vacuum conservation of specific intensity](vacuum-conservation-of-specific-intensity.md), a resolved uniform source retains its [radiance](radiance.md) along each [light ray](light-ray.md), while the [radiant flux](radiant-flux.md) received from the whole source can decrease as its apparent [solid angle](solid-angle.md) shrinks.

**Table of contents**

- [Projected area](projected-area.md)
- [Spectral radiance](spectral-radiance.md)
  - [Frequency and wavelength spectral radiance conversion](frequency-and-wavelength-spectral-radiance-conversion.md)
  - [Vacuum conservation of specific intensity](vacuum-conservation-of-specific-intensity.md)
  - [Limb darkening](limb-darkening.md)
    - [Linear limb-darkening law](linear-limb-darkening-law.md)
      - [Limb-darkening coefficient](limb-darkening-coefficient.md)
    - [Limb-darkened disk flux](limb-darkened-disk-flux.md)
    - [Small-planet transit weighting](small-planet-transit-weighting.md)
    - [Solar limb-darkening drift-scan experiment](solar-limb-darkening-drift-scan-experiment.md)

## ↑ Ancestors (5)

1. [Radiometry](radiometry-split.md)
2. [Optics](optics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (27)

- [Angular-frequency Planck energy density](angular-frequency-planck-energy-density.md)
- [Aperture truncation of etendue](aperture-truncation-of-etendue.md)
- [Basic radiance](basic-radiance.md)
- [Diffuse thermal emitter](diffuse-thermal-emitter.md)
- [Directional emissivity](directional-emissivity.md)
- [Etendue bench measurement](etendue-bench-measurement.md)
- [Etendue concentration limit](etendue-concentration-limit.md)
- [Etendue of a circular aperture and cone](etendue-of-a-circular-aperture-and-cone.md)
- [Focal ratio](focal-ratio.md)
- [Frequency and wavelength spectral radiance conversion](frequency-and-wavelength-spectral-radiance-conversion.md)
- [Irradiance](irradiance.md)
- [Lambert's cosine law](lambert-s-cosine-law.md)
- [Lambertian reflectance](lambertian-reflectance.md)
- [Linear limb-darkening law](linear-limb-darkening-law.md)
- [Outgoing longwave radiation](outgoing-longwave-radiation.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2014/paper-1/section-c/c10/solution.md)
- [Projected area](projected-area.md)
- [Radiance](radiance.md)
- [Radiant exitance](radiant-exitance.md)
- [Radiant flux](radiant-flux.md)
- [Radiant flux through an oriented surface](radiant-flux-through-an-oriented-surface.md)
- [Radiant intensity](radiant-intensity.md)
- [Radiative-convective climate column](radiative-convective-climate-column.md)
- [Radiometry](radiometry-split.md)
- [Satellite test of greenhouse spectral change](satellite-test-of-greenhouse-spectral-change.md)
- [Spectral radiance](spectral-radiance.md)
- [Stefan–Boltzmann law](stefan-boltzmann-law.md)
