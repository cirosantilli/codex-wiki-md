<h1 id="planck-s-law">Planck's law</h1>

↑ **Parent:** [Statistical physics](statistical-physics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Planck's_law)

[Planck's law](planck-s-law.md) gives the [spectral radiance](spectral-radiance.md) of an ideal [blackbody](blackbody.md) in [thermal equilibrium](thermal-equilibrium.md) at absolute [temperature](temperature.md) $T>0$. It predicts how much [power](power.md) is carried in each small [frequency](frequency.md) or [wavelength](wavelength.md) interval, per projected [area](surface-area.md) and per [solid angle](solid-angle.md). The whole curve is determined by $T$: no material-specific parameter enters this ideal [Planck function](planck-function.md).

Writing $\nu$ for [frequency](frequency.md) in hertz and $\lambda$ for [wavelength](wavelength.md) in metres, the two forms of the [Planck function](planck-function.md) are

$$
B_\nu(T)=\frac{2h\nu^3}{c^2}\frac1{e^{h\nu/(k_BT)}-1},
\qquad
B_\lambda(T)=\frac{2hc^2}{\lambda^5}\frac1{e^{hc/(\lambda k_BT)}-1}.
$$

Here $h$ is the [Planck constant](planck-constant.md), $k_B$ the [Boltzmann constant](boltzmann-constant.md), and $c$ the [speed of light](speed-of-light.md) in vacuum. Their exact values in the [International System of Units](international-system-of-units.md) are $h=6.62607015\times10^{-34}\,\mathrm{J\,s}$, $k_B=1.380649\times10^{-23}\,\mathrm{J\,K^{-1}}$, and $c=299792458\,\mathrm{m\,s^{-1}}$. [NIST, Meet the Constants](https://www.nist.gov/si-redefinition/meet-constants)

The units matter: $B_\nu$ is measured in $\mathrm{W\,m^{-2}\,sr^{-1}\,Hz^{-1}}$, whereas $B_\lambda$ is measured in $\mathrm{W\,m^{-2}\,sr^{-1}\,m^{-1}}$. Both are [spectral radiance](spectral-radiance.md), rather than [radiant exitance](radiant-exitance.md) or [energy density](energy-density.md). To report $B_\lambda$ per micrometre, multiply its per-metre value by $10^{-6}$; a micrometre-wide interval is $10^{-6}$ metres wide.

For a computed example, at $T=6000\,\mathrm K$ and $\lambda=0.500\,\mu\mathrm m$, the exponent is $hc/(\lambda k_BT)\approx4.79592$. Substitution into [Planck's law](planck-s-law.md) gives $B_\lambda\approx3.17569\times10^{13}\,\mathrm{W\,m^{-2}\,sr^{-1}\,m^{-1}}$, or $3.17569\times10^7\,\mathrm{W\,m^{-2}\,sr^{-1}}$ per micrometre. At the same [wavelength](wavelength.md), the illustrative [temperatures](temperature.md) $3000\,\mathrm K$ and $4500\,\mathrm K$ give $2.60268\times10^5$ and $6.37793\times10^6$ in the latter units. These are ideal predictions for stipulated [temperatures](temperature.md).

<a id="image-ideal-planck-s-law-spectra-at-three-temperatures"></a>
![](planck-spectral-radiance.png)

**[Figure 18](#image-ideal-planck-s-law-spectra-at-three-temperatures). Ideal Planck's law spectra at three temperatures**. The vertical axis is [spectral radiance](spectral-radiance.md) per micrometre, including the $10^{-6}$ conversion from per metre. Increasing [temperature](temperature.md) raises the curve at every fixed [wavelength](wavelength.md) and moves its marked peak toward shorter [wavelengths](wavelength.md). The peaks are approximately $966$, $644$, and $483\,\mathrm{nm}$ for $3000$, $4500$, and $6000\,\mathrm K$, respectively; only $0.1$ to $3\,\mu\mathrm m$ of each spectrum is shown.

The key [change of variables](change-of-variables-formula.md) is $\nu=c/\lambda$. Corresponding positive intervals carry the same [power](power.md), so $B_\lambda\,d\lambda=B_\nu\,|d\nu|$ and

$$
B_\lambda(T)=B_\nu(T)\big|_{\nu=c/\lambda}\,\frac{c}{\lambda^2}.
$$

Equal-width [wavelength](wavelength.md) intervals have unequal widths in [frequency](frequency.md); the factor $c/\lambda^2$ compensates for this. Merely replacing the horizontal-axis labels of $B_\nu$ by $c/\nu$ does not produce $B_\lambda$. This explains the [frequency and wavelength peaks of Planck's law](frequency-and-wavelength-peaks-of-planck-s-law.md).

A short derivation uses the [Boltzmann distribution](boltzmann-distribution.md) for a single electromagnetic mode with thermal [energies](energy.md) $nh\nu$, $n=0,1,\ldots$. Put $q=e^{-h\nu/(k_BT)}$. The [geometric series](geometric-series.md) gives $Z=\sum_{n\geq0}q^n=(1-q)^{-1}$ and mean thermal [energy](energy.md) $h\nu q/(1-q)$. The [electromagnetic mode density in a box](electromagnetic-mode-density-in-a-box.md), including both independent [polarization of an electromagnetic wave](polarization-of-an-electromagnetic-wave.md) states of a [photon](photon.md), is $8\pi\nu^2/c^3$ per volume per unit [frequency](frequency.md). Multiplication gives spectral [energy density](energy-density.md) $u_\nu=8\pi h\nu^3/[c^3(e^{h\nu/(k_BT)}-1)]$; [isotropy](isotropy.md) gives $B_\nu=cu_\nu/(4\pi)$. This counts thermal excitation [energy](energy.md), excluding [zero-point energy](zero-point-energy.md). [Feynman Lectures, I.41.3, quantum oscillator and radiation](https://www.feynmanlectures.caltech.edu/I_41.html#Ch41-S3)

[Planck's law](planck-s-law.md) connects [quantum mechanics](quantum-mechanics-split.md) to a measurable radiation curve. Its small-$h\nu/(k_BT)$ limit is the [Rayleigh-Jeans law](rayleigh-jeans-law.md), $B_\nu\approx2k_BT\nu^2/c^2$; its large-$h\nu/(k_BT)$ limit is the [Wien approximation](wien-approximation.md), $B_\nu\approx(2h\nu^3/c^2)e^{-h\nu/(k_BT)}$. The suppression at high [frequency](frequency.md) makes the total [energy density](energy-density.md) finite. Integrating the curve gives the [Stefan–Boltzmann law](stefan-boltzmann-law.md), while locating its peak gives [Wien's displacement law](wien-s-displacement-law.md). Thus one formula predicts both the spectral shape and the total emission.

**Table of contents**

- [Frequency and wavelength peaks of Planck's law](frequency-and-wavelength-peaks-of-planck-s-law.md)
- [Planck photon distribution](planck-photon-distribution.md)
  - [Temperature scaling of thermal photon number and energy densities](temperature-scaling-of-thermal-photon-number-and-energy-densities.md)
    - [Photon number density](photon-number-density.md)
      - [Photon number current](photon-number-current.md)
- [Black-body radiation](black-body-radiation.md)
  - [Electromagnetic mode density in a box](electromagnetic-mode-density-in-a-box.md)
  - [Thermodynamic derivation of blackbody radiation pressure](thermodynamic-derivation-of-blackbody-radiation-pressure.md)

## ↑ Ancestors (4)

1. [Statistical physics](statistical-physics-split.md)
2. [Branches of physics](branches-of-physics.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Black-body radiation](black-body-radiation.md)
- [Frequency and wavelength peaks of Planck's law](frequency-and-wavelength-peaks-of-planck-s-law.md)
- [Photon gas](photon-gas.md)
- [Planck function](planck-function.md)
- [Planck photon distribution](planck-photon-distribution.md)
- [Planck's law](planck-s-law.md)
- [Radiant exitance](radiant-exitance.md)
- [Spectral radiance](spectral-radiance.md)
