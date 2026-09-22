<h1 id="stefan-boltzmann-law">Stefan–Boltzmann law</h1>

↑ **Parent:** [Heat](heat-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stefan–Boltzmann_law)

The [Stefan–Boltzmann law](stefan-boltzmann-law.md) gives the total hemispherical [radiant exitance](radiant-exitance.md) of an ideal [blackbody](blackbody.md) at absolute [temperature](temperature-split.md) $T$:

$$
M_b(T)=\sigma T^4,\qquad [M_b]=\mathrm{W\,m^{-2}}.
$$

Here $\sigma$ is the [Stefan-Boltzmann constant](stefan-boltzmann-constant.md). Total means integrated over all [wavelengths](wavelength.md); hemispherical means integrated over all outward directions with the [projected area](projected-area.md) weighting. Thus $M_b$ is emitted [power](power.md) per actual emitting [area](surface-area.md), rather than directional [radiance](radiance.md) or [spectral radiance](spectral-radiance.md). Absolute [temperature](temperature-split.md) must be in [kelvin](kelvin.md); raising a Celsius reading to the fourth power gives the wrong result. A uniform surface of [area](surface-area.md) $A$ emits [radiant flux](radiant-flux.md) $P_{\rm emit}=AM_b$. A real surface instead has $M=\epsilon(T)\sigma T^4$, where $\epsilon(T)$ is its [total hemispherical emissivity](total-hemispherical-emissivity.md). The older symbol $F$ in the formula above denotes this emitted [radiant exitance](radiant-exitance.md).[§19.1, Ideal Radiators: blackbody emitted power per area, units, spectrum and cavity](thermodynamics-and-propulsion.md)

For an ideal [blackbody](blackbody.md), doubling absolute [temperature](temperature-split.md) multiplies [radiant exitance](radiant-exitance.md) by $16$. With the approximate [Stefan-Boltzmann constant](stefan-boltzmann-constant.md) $5.670374419\times10^{-8}\,\mathrm{W\,m^{-2}\,K^{-4}}$, the [radiant exitances](radiant-exitance.md) at $300\,\mathrm K$ and $600\,\mathrm K$ are approximately $459.300$ and $7348.805\,\mathrm{W\,m^{-2}}$. This steep response explains why [thermal radiation](thermal-radiation.md) becomes so consequential at high [temperature](temperature-split.md). It also enables [heat transfer](heat-transfer.md) through a [vacuum](vacuum.md), where [thermal conduction](thermal-conduction.md) through a gas and [convection](convection-split.md) are absent.

<a id="image-the-fourth-power-rise-of-radiant-exitance-and-the-subtraction-needed-for-net-radiative-heat-exchange"></a>
![](stefan-boltzmann-gross-and-net-power.png)

**[Figure 9](#image-the-fourth-power-rise-of-radiant-exitance-and-the-subtraction-needed-for-net-radiative-heat-exchange). The fourth-power rise of radiant exitance and the subtraction needed for net radiative heat exchange**. Original model curves. The left panel is total hemispherical [blackbody](blackbody.md) [radiant exitance](radiant-exitance.md). The right panel uses [emissivity](emissivity.md) $0.8$, emitting [area](surface-area.md) $0.01\,\mathrm{m^2}$ and a black enclosure at $300\,\mathrm K$; gross emitted and absorbed [powers](power.md) remain positive at equal [temperatures](temperature-split.md), while their difference vanishes. The point at $500\,\mathrm K$ is the stipulated example in [net radiative heat exchange](net-radiative-heat-exchange.md), not a measurement.

A short derivation integrates [Planck's law](planck-s-law.md) in its [frequency](frequency.md) form. For a [blackbody](blackbody.md), direction-independent [spectral radiance](spectral-radiance.md) is $B_\nu(T)=2h\nu^3/[c^2(e^{h\nu/(k_BT)}-1)]$, where $h$ is the [Planck constant](planck-constant.md), $k_B$ the [Boltzmann constant](boltzmann-constant.md) and $c$ the [speed of light](speed-of-light.md). The outward [hemisphere](hemisphere.md) contributes $\int\cos\theta\,d\Omega=\pi$, so

$$
M_b=\pi\int_0^\infty B_\nu(T)\,d\nu
=\frac{2\pi k_B^4T^4}{h^3c^2}\int_0^\infty\frac{x^3}{e^x-1}\,dx,
\qquad x=\frac{h\nu}{k_BT}.
$$

Expanding $(e^x-1)^{-1}=\sum_{n=1}^\infty e^{-nx}$, nonnegative terms allow termwise [integration](integral-split.md). Repeated [integration by parts](integration-by-parts.md) gives $\int_0^\infty x^3e^{-nx}\,dx=6/n^4$; the [Riemann zeta function](riemann-zeta-function.md) value $\zeta(4)=\pi^4/90$ gives the remaining [integral](integral-split.md) as $\pi^4/15$. Hence $M_b=\sigma T^4$ with the coefficient in [Stefan-Boltzmann constant](stefan-boltzmann-constant.md). The angular [integral](integral-split.md) is essential: omitting it confuses [radiance](radiance.md) with [radiant exitance](radiant-exitance.md).

**Table of contents**

- [Net radiative heat exchange](net-radiative-heat-exchange.md)
  - [View factor](view-factor.md)
- [Stefan-Boltzmann constant](stefan-boltzmann-constant.md)
- [Emissivity](emissivity.md)
  - [Total hemispherical emissivity](total-hemispherical-emissivity.md)
  - [Spectral emissivity](spectral-emissivity.md)
  - [Directional emissivity](directional-emissivity.md)
  - [Grey body](grey-body.md)
  - [Diffuse thermal emitter](diffuse-thermal-emitter.md)
  - [Comparing surface emission at equal temperature](comparing-surface-emission-at-equal-temperature.md)
- [Radiative equilibrium](radiative-equilibrium.md)

## ↑ Ancestors (6)

1. [Heat](heat-split.md)
2. [Thermodynamics](thermodynamics-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (71)

- [Black-body radiation](black-body-radiation.md)
- [CNO homology with density-dependent inverse-cubic opacity](cno-homology-with-density-dependent-inverse-cubic-opacity.md)
- [Comparing surface emission at equal temperature](comparing-surface-emission-at-equal-temperature.md)
- [Contraction law with density-linear fourth-power stellar opacity](contraction-law-with-density-linear-fourth-power-stellar-opacity.md)
- [Convective contraction with power-law opacity](convective-contraction-with-power-law-opacity.md)
- [Debye T-cubed test](debye-t-cubed-test.md)
- [Effective-temperature profile of a zero-torque disk](effective-temperature-profile-of-a-zero-torque-disk.md)
- [Flaring passive disk](flaring-passive-disk.md)
- [Fully mixed hydrogen-burning evolutionary track](fully-mixed-hydrogen-burning-evolutionary-track.md)
- [Hayashi relation with eighth-power temperature opacity](hayashi-relation-with-eighth-power-temperature-opacity.md)
- [Hayashi relation with thirteenth-power opacity](hayashi-relation-with-thirteenth-power-opacity.md)
- [Hertzsprung-Russell slope of a stellar homology sequence](hertzsprung-russell-slope-of-a-stellar-homology-sequence.md)
- [Negative-hydrogen-opacity alpha-disk thickness scaling](negative-hydrogen-opacity-alpha-disk-thickness-scaling.md)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2017/2/b/solution.md)
- [Solution](past-exam-of-the-atmospheric-physics-course-of-the-university-of-cambridge/2013/paper-1/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-37/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-37/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-42/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-63/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-62/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-70/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-70/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-4/34d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-71/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-63/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-66/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-66/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3/10e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-63/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-70/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-70/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-63/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-68/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-69/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-63/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-80/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-55/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-64/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-64/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-317/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-317/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-315/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-321/1/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-315/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-317/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-317/1/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-317/1/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-317/2/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-347/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-317/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-317/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-332/1/a/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2021/paper-1/section-d/d9/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-1/section-a/a4/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2022/paper-2/section-c/c9/c/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2022/paper-2/section-c/c9/d/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1/section-a/a1/solution.md)
- [Planck's law](planck-s-law.md)
- [Radiant exitance](radiant-exitance.md)
- [Radiation pressure of an isotropic photon gas](radiation-pressure-of-an-isotropic-photon-gas.md)
- [Radiative gravity-darkening law](radiative-gravity-darkening-law.md)
- [Radiative homology with density-half inverse-five-halves opacity](radiative-homology-with-density-half-inverse-five-halves-opacity.md)
- [Radiative homology with proton-proton burning and inverse-fourth-power opacity](radiative-homology-with-proton-proton-burning-and-inverse-fourth-power-opacity.md)
- [Radiative mass loss at fixed luminosity](radiative-mass-loss-at-fixed-luminosity.md)
- [Stationary radiation density](stationary-radiation-density.md)
- [Stefan-Boltzmann constant](stefan-boltzmann-constant.md)
- [Stefan-Boltzmann estimate of Schwarzschild evaporation time](stefan-boltzmann-estimate-of-schwarzschild-evaporation-time.md)
- [Stefan–Boltzmann law](stefan-boltzmann-law.md)
- [Ultraviolet catastrophe](ultraviolet-catastrophe.md)
- [Wien's displacement law](wien-s-displacement-law.md)
- [Zero-dimensional planetary energy balance](zero-dimensional-planetary-energy-balance.md)
