# Black-body radiation

↑ **Parent:** [Planck's law](planck-s-law.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Black-body_radiation)

[Black-body radiation](black-body-radiation.md) is the [electromagnetic radiation](electromagnetic-radiation.md) in [thermal equilibrium](thermal-equilibrium.md) with an ideal [blackbody](blackbody.md). It can be described as a [photon gas](photon-gas.md): a cavity whose walls are all at the same [temperature](temperature.md) contains radiation with the universal [Planck's law](planck-s-law.md) spectrum. A small opening in such a cavity approximates a [blackbody](blackbody.md) emitter because incoming radiation undergoes repeated absorption inside. The radiation's equilibrium spectrum depends on [temperature](temperature.md), rather than the wall material. [OpenStax, University Physics 3, §6.1, blackbody cavity and emission laws](https://openstax.org/books/university-physics-volume-3/pages/6-1-blackbody-radiation)

There are three useful quantities to keep distinct: directional [spectral radiance](spectral-radiance.md) $B_\nu$ or $B_\lambda$, total [energy density](energy-density.md) $u$ in the cavity, and outward [radiant exitance](radiant-exitance.md) $j^*$ from its opening. [Planck's law](planck-s-law.md) supplies the first; [integrals](integral.md) over [frequency](frequency.md) and directions supply the others. For [isotropy](isotropy.md), every direction has the same $B_\nu$, so the full $4\pi$ [solid angle](solid-angle.md) gives

$$
u(T)=\frac{4\pi}{c}\int_0^\infty B_\nu(T)\,d\nu
=a_{\rm rad}T^4,\qquad
a_{\rm rad}=\frac{8\pi^5k_B^4}{15h^3c^3}
=\frac{\pi^2k_B^4}{15\hbar^3c^3}.
$$

Here $\hbar=h/(2\pi)$ is the reduced [Planck constant](planck-constant.md), and the [radiation constant](radiation-constant.md) is $a_{\rm rad}\approx7.565733250\times10^{-16}\,\mathrm{J\,m^{-3}\,K^{-4}}$. The explicit [Boltzmann constant](boltzmann-constant.md) makes this an SI formula; adopting [natural units](natural-units.md) with $k_B=1$ recovers $u=\pi^2T^4/(15\hbar^3c^3)$.

For a short [integral](integral.md) outline, substitute $x=h\nu/(k_BT)$ and use

$$
\int_0^\infty\frac{x^3}{e^x-1}\,dx
=\sum_{n=1}^\infty\int_0^\infty x^3e^{-nx}\,dx
=6\sum_{n=1}^\infty\frac1{n^4}=\frac{\pi^4}{15}.
$$

The expansion is a [geometric series](geometric-series.md) with nonnegative terms; repeated [integration by parts](integration-by-parts.md) evaluates each [integral](integral.md), and $\zeta(4)=\pi^4/90$ is a value of the [Riemann zeta function](riemann-zeta-function.md). This gives the coefficient above.

The [photon gas](photon-gas.md) also exerts [radiation pressure](radiation-pressure.md), $p=u/3$. The factor $1/3$ comes from the [angular average](angular-average.md) of the squared directional component of [photon](photon.md) [momentum](momentum.md), $\langle\cos^2\theta\rangle=1/3$. The [thermodynamic derivation of blackbody radiation pressure](thermodynamic-derivation-of-blackbody-radiation-pressure.md) gives the same result. In contrast, outgoing [power](power.md) involves one projected-direction factor over an outward hemisphere, yielding [radiant exitance](radiant-exitance.md)

$$
j^*=\pi\int_0^\infty B_\nu(T)\,d\nu
=\frac{cu}{4}=\sigma T^4,
\qquad \sigma=\frac{2\pi^5k_B^4}{15h^3c^2}.
$$

This is the [Stefan–Boltzmann law](stefan-boltzmann-law.md) with unit [emissivity](emissivity.md); $\sigma$ is the [Stefan-Boltzmann constant](stefan-boltzmann-constant.md). The factor $\pi$ follows from [Lambert's cosine law](lambert-s-cosine-law.md), rather than the $4\pi$ full-sphere factor used for [energy density](energy-density.md).

For example, an ideal $6000\,\mathrm K$ cavity has $u\approx0.980519\,\mathrm{J\,m^{-3}}$, [radiation pressure](radiation-pressure.md) $p\approx0.326840\,\mathrm{Pa}$, and outward [radiant exitance](radiant-exitance.md) $j^*\approx7.34881\times10^7\,\mathrm{W\,m^{-2}}$. A stipulated $3000\,\mathrm K$ cavity has one-sixteenth each value because all three scale as $T^4$. These describe stored [energy](energy.md), mechanical [pressure](pressure.md), and outgoing [power](power.md) per [area](surface-area.md), respectively. In a closed equilibrium cavity, equal opposing radiation balances the directional [power](power.md) flow even though $u$ and $p$ are nonzero.

The usefulness of [black-body radiation](black-body-radiation.md) is this common reference: [Planck's law](planck-s-law.md), [Wien's displacement law](wien-s-displacement-law.md), and the [Stefan–Boltzmann law](stefan-boltzmann-law.md) consistently connect spectral measurements, [temperature](temperature.md), and total emission. The three illustrative curves in [Planck's law](planck-s-law.md) are ideal equilibrium spectra; applying them to a material requires considering its [emissivity](emissivity.md) and whether [thermal equilibrium](thermal-equilibrium.md) is a suitable approximation.

**Table of contents**

- [Electromagnetic mode density in a box](electromagnetic-mode-density-in-a-box.md)
- [Thermodynamic derivation of blackbody radiation pressure](thermodynamic-derivation-of-blackbody-radiation-pressure.md)

## ↑ Ancestors (5)

1. [Planck's law](planck-s-law.md)
2. [Statistical physics](statistical-physics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Black-body radiation](black-body-radiation.md)
- [Frequency and wavelength peaks of Planck's law](frequency-and-wavelength-peaks-of-planck-s-law.md)
- [Photon gas](photon-gas.md)
