# Thermal Raman line ratio

↑ **Parent:** [Raman scattering](raman-scattering.md)

Assume one harmonic [normal mode](normal-mode.md) at [thermal equilibrium](thermal-equilibrium-split.md), weak spontaneous excitation far from electronic resonances, the same collection [solid angle](solid-angle.md) and [wave polarization](polarization-waves.md), and matched response after instrumental correction. The [Boltzmann distribution](boltzmann-distribution.md) gives

$$
r=\exp\left(-\frac{h\nu_v}{k_BT}\right),\qquad
P_v=(1-r)r^v,\qquad
\overline v=\frac{r}{1-r}.
$$

Here $k_B$ is the [Boltzmann constant](boltzmann-constant.md), $T>0$ is [temperature](temperature-split.md), and $P_v$ is the probability of vibrational [quantum number](quantum-number.md) $v$. Thus $P_1/P_0=r$. Linear coupling to $Q$ has squared oscillator matrix elements proportional to $v+1$ for [Stokes Raman scattering](stokes-raman-scattering.md) and $v$ for [Anti-Stokes Raman scattering](anti-stokes-raman-scattering.md). Summing over initial levels gives strengths proportional to $\overline v+1$ and $\overline v$ respectively; their ratio is $r$, even when levels above $v=1$ are occupied.

Let $I_{\rm S}$ and $I_{\rm AS}$ denote line-integrated [radiant intensities](radiant-intensity.md), meaning [power](power.md) per collection [solid angle](solid-angle.md). The off-resonant [electric dipole radiation](electric-dipole-radiation.md) law adds the fourth power of emitted [frequency](frequency.md):

$$
\frac{I_{\rm AS}}{I_{\rm S}}
=\left(\frac{\nu_0+\nu_v}{\nu_0-\nu_v}\right)^4
\exp\left(-\frac{h\nu_v}{k_BT}\right).
$$

The [photon](photon.md) rate divides each line's [power](power.md) by its own $h\nu_s$. Consequently, the ideal response-corrected anti-Stokes/Stokes count-rate ratio has the third power of the same [frequency](frequency.md) ratio. Peak heights alone do not give line-integrated [radiant intensities](radiant-intensity.md) if linewidths differ. Uncorrected detector counts can also include unequal detector response and unequal [optical filter](optical-filter.md) transmission. Resonant enhancement, overlapping [spectral lines](spectral-line.md), nonthermal populations and local optical heating can invalidate a [temperature](temperature-split.md) inferred from this simple formula.

**Table of contents**

- [One-mode Raman spectrum example](one-mode-raman-spectrum-example.md)

## ↑ Ancestors (6)

1. [Raman scattering](raman-scattering.md)
2. [Scattering of light](scattering-of-light.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Raman spectroscopy](raman-spectroscopy.md)
