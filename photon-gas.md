# Photon gas

↑ **Parent:** [Statistical physics](statistical-physics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Photon_gas)

A [photon gas](photon-gas.md) is a collection of [photons](photon.md) described statistically as radiation. Here the equilibrium model is homogeneous, isotropic [electromagnetic radiation](electromagnetic-radiation.md) in vacuum at [temperature](temperature.md) $T>0$: each [photon](photon.md) has [energy](energy.md) $E=c|\mathbf p|=h\nu$, with [momentum](momentum.md) $\mathbf p$ and [frequency](frequency.md) $\nu$, and there are two independent transverse states of [electromagnetic polarization](polarization-of-an-electromagnetic-wave.md). An absorbing cavity with walls at a common [temperature](temperature.md) provides a way to establish this [thermal equilibrium](thermal-equilibrium.md). The bulk formulas assume cavity dimensions much larger than the typical [wavelength](wavelength.md) $hc/(k_BT)$, so the [electromagnetic mode density in a box](electromagnetic-mode-density-in-a-box.md) can replace individual cavity modes by a continuum. [David Tong, Statistical Physics, §3.2: photon energies, polarizations and cavity equilibrium](https://davidtong.org/teaching/statistical-physics/statmechhtml/S3#S3.SS2)

The crucial constraint is whether [photon emission](photon-emission.md) and [photon absorption](photon-absorption.md), or other number-changing processes, can equilibrate the [photon](photon.md) population. When they can, [photon](photon.md) number is not an independently conserved quantity and the equilibrium [photon chemical potential](photon-chemical-potential.md) is $\mu_\gamma=0$. For each polarization and [frequency](frequency.md), the mean [occupation number](occupation-number.md) then follows the [Bose-Einstein distribution](bose-einstein-distribution.md):

$$
f(\nu)=\frac{1}{\exp[h\nu/(k_BT)]-1}.
$$

If number-changing processes are ineffective but number-conserving interactions redistribute [energy](energy.md), a constrained [Bose-Einstein distribution](bose-einstein-distribution.md) can instead have $f=[\exp((h\nu-\mu_\gamma)/(k_BT))-1]^{-1}$ with [chemical potential](chemical-potential.md) $\mu_\gamma\le0$ fixed by the number constraint. Thus [thermal equilibrium](thermal-equilibrium.md) with respect to [energy](energy.md) exchange alone does not establish $\mu_\gamma=0$. The zero value can also persist in an already prepared [Planck photon distribution](planck-photon-distribution.md) during suitable subsequent evolution; continual [photon emission](photon-emission.md) is not required to preserve it. [Hiroyuki Tashiro, CMB spectral distortions and energy release in the early universe (2014), §3.1: kinetic equilibration without full photon-number equilibration](https://academic.oup.com/ptep/article/2014/6/06B107/1560917)

Combining $f$ with the two-polarization [density of states](density-of-states.md), $g_\nu/V=8\pi\nu^2/c^3$, gives the [Planck photon distribution](planck-photon-distribution.md) and the spectral [photon energy density](photon-energy-density.md):

$$
\frac{dn_\gamma}{d\nu}=\frac{8\pi\nu^2}{c^3}f(\nu),\qquad
u_\nu\equiv\frac{du}{d\nu}=\frac{8\pi h\nu^3}{c^3}f(\nu)=\frac{4\pi}{c}B_\nu(T).
$$

Here $B_\nu$ is the [spectral radiance](spectral-radiance.md) in [Planck's law](planck-s-law.md); $u_\nu$ is stored [energy density](energy-density.md) per unit [frequency](frequency.md), not outgoing [power](power.md) per [area](surface-area.md). Their different units are connected by the full-sphere [solid angle](solid-angle.md) and the [speed of light](speed-of-light.md) $c$. The [Boltzmann constant](boltzmann-constant.md) is $k_B$, and $h$ is the [Planck constant](planck-constant.md). [Richard Fitzpatrick, Planck Radiation Law: two polarizations and radiation energy spectrum](https://farside.ph.utexas.edu/teaching/sm1/Thermalhtml/node103.html)

The equilibrium [equation of state](equation-of-state.md) is particularly simple:

$$
u=a_RT^4,\qquad p=\frac{u}{3},\qquad
 a_R=\frac{8\pi^5k_B^4}{15h^3c^3}=\frac{4\sigma}{c}
 \simeq7.565733250\times10^{-16}\,\mathrm{J\,m^{-3}\,K^{-4}}.
$$

The [radiation constant](radiation-constant.md) $a_R$ is the same constant called $a_{\rm rad}$ in [black-body radiation](black-body-radiation.md); $\sigma$ is the [Stefan-Boltzmann constant](stefan-boltzmann-constant.md). An outline of the [energy density](energy-density.md) calculation substitutes $x=h\nu/(k_BT)$ and uses $\int_0^\infty x^3/(e^x-1)\,dx=\pi^4/15$. The [radiation pressure](radiation-pressure.md) follows because the [angular average](angular-average.md) of the squared directional component of [photon](photon.md) [momentum](momentum.md) is $1/3$ for [isotropy](isotropy.md); the [thermodynamic derivation of blackbody radiation pressure](thermodynamic-derivation-of-blackbody-radiation-pressure.md) supplies an independent route. These formulas describe the radiation contribution, not the cavity walls. The isotropic massless relation $p=u/3$ survives a different isotropic spectrum, whereas the coefficient in $u=a_RT^4$ requires the zero-[chemical potential](chemical-potential.md) [Planck photon distribution](planck-photon-distribution.md).

For a computed example with stipulated $T=2.725\,\mathrm K$, the [photon energy density](photon-energy-density.md) is $u\simeq4.17174\times10^{-14}\,\mathrm{J\,m^{-3}}$ and the [radiation pressure](radiation-pressure.md) is $p\simeq1.39058\times10^{-14}\,\mathrm{Pa}$. The [photon number density](photon-number-density.md) in the [International System of Units](international-system-of-units.md) is

$$
n_\gamma=16\pi\zeta(3)\left(\frac{k_BT}{hc}\right)^3
 \simeq4.10501\times10^8\,\mathrm{m^{-3}},\qquad
\frac{u}{n_\gamma}=\frac{\pi^4}{30\zeta(3)}k_BT\simeq2.70118\,k_BT.
$$

Here $\zeta$ is the [Riemann zeta function](riemann-zeta-function.md). The mean [photon](photon.md) [energy](energy.md) differs from the [energy](energy.md) at the peak of a spectral curve: counting [photons](photon.md) and weighting them by [energy](energy.md) emphasize different [frequencies](frequency.md). The calculations use the exact [International System of Units](international-system-of-units.md) values of the [Planck constant](planck-constant.md), [Boltzmann constant](boltzmann-constant.md) and [speed of light](speed-of-light.md). [NIST, Meet the Constants: exact SI defining constants](https://www.nist.gov/si-redefinition/meet-constants)

<a id="image-analytic-photon-gas-spectra-counting-photons-and-weighting-their-energies"></a>
![](photon-gas-entropy-spectral-weights.png)

**[Figure 1](#image-analytic-photon-gas-spectra-counting-photons-and-weighting-their-energies). Analytic photon gas spectra: counting photons and weighting their energies**. Original equilibrium model, not measured data. The left panel evaluates $u_\nu$ at stipulated $T=2.725\,\mathrm K$ per gigahertz. The right panel uses $x=h\nu/(k_BT)$ and plots the normalized spectral fractions $F_n=x^2/[2\zeta(3)(e^x-1)]$ and $F_u=15x^3/[\pi^4(e^x-1)]$, each with total [integral](integral.md) one on $0<x<\infty$. Their different shapes show why a photon-counting spectrum and an [energy density](energy-density.md) spectrum have different peaks.

A motivating observation is the [cosmic microwave background](cosmic-microwave-background.md) spectrum measured by the Far Infrared Absolute Spectrophotometer (FIRAS) aboard COBE. Its apparatus used a polarizing [Michelson interferometer](michelson-interferometer.md), with one input viewing a roughly seven-degree sky patch and the other an internal [blackbody](blackbody.md). Scanning mirrors changed the [optical path length](optical-path-length.md) difference; heat-sensitive detectors recorded the varying [power](power.md), and [Fourier transform spectroscopy](fourier-transform-spectroscopy.md) recovered the spectral difference. Operation outside the [terrestrial atmosphere](terrestrial-atmosphere.md) removed atmospheric emission and absorption, while shielding and cooling the optics in a helium cryostat suppressed the instrument's own radiation. [Mather, Fixsen and Shafer, Design for the COBE Far Infrared Absolute Spectrophotometer, apparatus and systematic-error controls](https://lambda.gsfc.nasa.gov/data/cobe/firas/doc/FES4_APP_B.pdf)

Absolute calibration came from moving an external [blackbody](blackbody.md) into the sky aperture, filling the same beam used for the sky. This was an iron-loaded epoxy absorber shaped as a re-entrant cone. Repeated reflections made it a close approximation to a [blackbody](blackbody.md), while thermometers supplied its [temperature](temperature.md). Mather and colleagues explicitly evaluated reflections, [temperature](temperature.md) gradients, radiation leaking through the material and leakage around its edge. These are limits on how faithfully the calibrator realizes [thermal equilibrium](thermal-equilibrium.md) radiation, rather than details that can be eliminated merely by calling it black. [Mather et al., Calibrator Design for COBE FIRAS (1999): absorber geometry and calibration error budget](https://arxiv.org/abs/astro-ph/9810373)

During sky observations the internal [blackbody](blackbody.md) [temperature](temperature.md) was adjusted to nearly null the spectral difference, reducing gain and drift errors. Fixsen and colleagues' 1996 analysis used calibrated spectra over [wavenumbers](wavenumber.md) $2$ to $21\,\mathrm{cm^{-1}}$, about $60$ to $630\,\mathrm{GHz}$. They separated the sky's spatially uniform component, its dipole and Galactic emission, and varied sky cuts and foreground templates as controls. The resulting [cosmic microwave background](cosmic-microwave-background.md) spectrum agreed with a single [Planck function](planck-function.md), with reported RMS deviations below 50 parts per million of its peak brightness. This is a residual statistic over the analyzed spectrum, not a pointwise relative error bound at every [frequency](frequency.md). [Fixsen et al., The Cosmic Microwave Background Spectrum from the Full COBE/FIRAS Data Set (1996), §§2, 5 and 5.3](https://arxiv.org/abs/astro-ph/9605054)

The observation motivates using a [photon gas](photon-gas.md) as a physical model rather than merely a formal counting exercise. Its interpretation has a clear boundary: agreement with [Planck's law](planck-s-law.md) constrains departures from an equilibrium spectral shape within the calibrated band and foreground assumptions; it does not directly measure [radiation pressure](radiation-pressure.md) or [entropy density of a photon gas](entropy-density-of-a-photon-gas.md). Nor does it establish that today's [cosmic microwave background](cosmic-microwave-background.md) is continually re-equilibrating with matter. A previously thermal spectrum can retain its [Planck function](planck-function.md) shape as [expansion of the universe](expansion-of-the-universe.md) lowers every [photon](photon.md) [frequency](frequency.md) in the same proportion. The usefulness of the model is that one measured spectral [temperature](temperature.md), together with its equilibrium assumptions, predicts [energy density](energy-density.md), [radiation pressure](radiation-pressure.md), [photon number density](photon-number-density.md) and [entropy density of a photon gas](entropy-density-of-a-photon-gas.md) consistently.

**Table of contents**

- [Entropy density of a photon gas](entropy-density-of-a-photon-gas.md)

## ↑ Ancestors (4)

1. [Statistical physics](statistical-physics-split.md)
2. [Branches of physics](branches-of-physics.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Black-body radiation](black-body-radiation.md)
- [Entropy density of a photon gas](entropy-density-of-a-photon-gas.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3/10e/solution.md)
- [Photon gas](photon-gas.md)
- [Statistical physics](statistical-physics-split.md)
