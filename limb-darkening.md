# Limb darkening

↑ **Parent:** [Spectral radiance](spectral-radiance.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Limb_darkening)

Limb darkening is the decrease of emergent [specific intensity](spectral-radiance.md) toward the apparent edge of a stellar disc. A transit depth then depends on the intensity sampled by the planet as well as its projected area; the uniform-disc area ratio is only an approximation.

For a spherical [star](star.md) of [radius](radius.md) $R_\star$, let $r$ be distance from the centre of its projected disk and let $\theta$ be the [angle](angle.md) between the outward [unit normal](unit-normal.md) and the [line of sight](line-of-sight.md). The angular coordinate is

$$
\mu=\cos\theta=\sqrt{1-(r/R_\star)^2}.
$$

Disk centre has $\mu=1$; the apparent edge approaches $\mu=0$. A resolved image measures [specific intensity](spectral-radiance.md) in each direction. [Limb darkening](limb-darkening.md) means that this [specific intensity](spectral-radiance.md) itself falls toward the edge; the [projected area](projected-area.md) factor used when collecting [radiant flux](radiant-flux.md) is a separate geometric effect.

A simple explanation assumes a horizontally uniform [plane-parallel atmosphere](plane-parallel-atmosphere.md), a sufficiently deep [optically thick medium](optically-thick-medium.md), negligible [scattering of light](scattering-of-light.md), and thermal absorption and emission in [local thermodynamic equilibrium](local-thermodynamic-equilibrium.md). Let $\tau_\nu$ be inward vertical [optical depth](optical-depth.md) at fixed [frequency](frequency.md) $\nu$. An oblique [light ray](light-ray.md) has [line of sight](line-of-sight.md) [optical depth](optical-depth.md) $\tau_\nu/\mu$, so it encounters the same attenuation at a smaller vertical [optical depth](optical-depth.md). The [formal solution of the radiative transfer equation](formal-solution-of-the-radiative-transfer-equation.md) gives

$$
I_\nu(0,\mu)=\int_0^\infty S_\nu(\tau_\nu)e^{-\tau_\nu/\mu}\frac{d\tau_\nu}{\mu},\qquad 0<\mu\le1.
$$

Here $S_\nu$ is the [source function](radiative-transfer-source-function.md); under these assumptions it is the [Planck function](planck-function.md) $B_\nu[T(\tau_\nu)]$. If [temperature](temperature-split.md) increases inward, an oblique view preferentially samples cooler layers and hence lower [specific intensity](spectral-radiance.md). [§2.2.2, pp. 17–19, equations (2.37)–(2.44) and Figure 2.4](radiative-transfer-in-stellar-atmospheres-by-robert-j-rutten-8th-edition.md)

The weight $e^{-\tau_\nu/\mu}/\mu$ is an [exponential distribution](exponential-distribution.md) in vertical [optical depth](optical-depth.md), with [expected value](expected-value-split.md) $\mu$ and [standard deviation](standard-deviation.md) $\mu$. Thus “seeing down to [optical depth](optical-depth.md) one” refers to the [line of sight](line-of-sight.md), and represents a broad sampling of layers rather than a sharp emitting surface. For a [source function](radiative-transfer-source-function.md) that is linear throughout the atmosphere, the [Eddington-Barbier relation](eddington-barbier-relation.md) is exact:

$$
S_\nu(\tau_\nu)=a_\nu+b_\nu\tau_\nu
\quad\Longrightarrow\quad
I_\nu(0,\mu)=a_\nu+b_\nu\mu=S_\nu(\mu).
$$

This follows by integrating the constant and linear terms separately. A constant [source function](radiative-transfer-source-function.md) instead gives constant [specific intensity](spectral-radiance.md), as in the [blackbody limit of an isothermal atmosphere](blackbody-limit-of-an-isothermal-atmosphere.md). An outward-rising [temperature](temperature-split.md) or important [scattering of light](scattering-of-light.md) changes the argument. Close enough to the actual edge, a [plane-parallel atmosphere](plane-parallel-atmosphere.md) also loses validity because of curvature. Neither one [limb-darkening coefficient](limb-darkening-coefficient.md) nor a universal dependence on [wavelength](wavelength.md) follows from this simple model.

**Table of contents**

- [Linear limb-darkening law](linear-limb-darkening-law.md)
  - [Limb-darkening coefficient](limb-darkening-coefficient.md)
- [Limb-darkened disk flux](limb-darkened-disk-flux.md)
- [Small-planet transit weighting](small-planet-transit-weighting.md)
- [Solar limb-darkening drift-scan experiment](solar-limb-darkening-drift-scan-experiment.md)

## ↑ Ancestors (7)

1. [Spectral radiance](spectral-radiance.md)
2. [Radiance](radiance.md)
3. [Radiometry](radiometry-split.md)
4. [Optics](optics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (20)

- [Exoplanet transit photometry](exoplanet-transit-photometry.md)
- [Light curve](light-curve.md)
- [Limb darkening](limb-darkening.md)
- [Linear limb-darkening law](linear-limb-darkening-law.md)
- [Michelson stellar interferometer](michelson-stellar-interferometer.md)
- [Solution](past-exam-of-the-exoplanets-and-planetary-systems-course-of-the-university-of-cambridge/2015/paper-1/1/solution.md)
- [Solution](past-exam-of-the-exoplanets-and-planetary-systems-course-of-the-university-of-cambridge/2016/paper-1/1/solution.md)
- [Solution](past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2014/paper-1/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-53/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-59/1/c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-315/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-315/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-316/1/vii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-317/1/solution.md)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2014/paper-1/4/solution.md)
- [Solution](past-exam-of-the-optics-and-electrodynamics-course-of-the-university-of-cambridge/2022/section-a/3/solution.md)
- [Total duration of a circular planetary transit](total-duration-of-a-circular-planetary-transit.md)
- [Transit dimming by an optically thin orbital wire](transit-dimming-by-an-optically-thin-orbital-wire.md)
- [Uniform-disc binary-star visibility](uniform-disc-binary-star-visibility.md)
- [Uniform-disk stellar visibility](uniform-disk-stellar-visibility.md)
