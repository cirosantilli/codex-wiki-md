# Finite-row electron diffraction model

↑ **Parent:** [Electron diffraction](electron-diffraction.md)

Take $N$ equally spaced scattering sites at $x_j=jd$ on a line, a normally incident [plane wave](plane-wave.md), equal site [scattering amplitudes](scattering-amplitude.md), and observation far enough away that outgoing directions are effectively parallel. Retain only one scattering event per amplitude, as in the [Born approximation](born-approximation.md). For angle $\phi$ from the outward normal, write the adjacent-site [quantum phase](quantum-phase.md) difference as $\delta=kd\sin\phi$, with $k=2\pi/\lambda$; reversing its overall sign leaves the intensity unchanged. Summing a [geometric series](geometric-series.md) gives

$$
\frac{I(\phi)}{I(0)}=\frac{1}{N^2}\left|\sum_{j=0}^{N-1}e^{ij\delta}\right|^2
=\left[\frac{\sin(N\delta/2)}{N\sin(\delta/2)}\right]^2,\qquad \delta=\frac{2\pi d}{\lambda}\sin\phi.
$$

At $\delta=2\pi m$ use the continuous limit $I/I(0)=1$, rather than treating $0/0$ as a missing peak. The integer $m$ is the [diffraction order](diffraction-order.md): $d\sin\phi=m\lambda$. This is a surface-row spacing, not the plane spacing in [Bragg's law](bragg-s-law.md). The plotted intensity is normalized to its central value; it is not an integrated detection probability or an absolute collector [electric current](electric-current.md).

<a id="image-surface-row-geometry-and-calculated-electron-diffraction-intensity"></a>
![](electron-diffraction-row-geometry-intensity.png)

**[Figure 20](#image-surface-row-geometry-and-calculated-electron-diffraction-intensity). Surface-row geometry and calculated electron diffraction intensity**. [Source](electron-diffraction-row-geometry-intensity.py). Original idealized model: $N=12$, row spacing $d=0.250\,\mathrm{nm}$, equal site [scattering amplitudes](scattering-amplitude.md), normal incidence and field-free nonrelativistic [Electron](electron.md) [wavelengths](wavelength.md) at $54$, $100$ and $400\,\mathrm V$. Straight arrows denote propagation directions, not sinusoidal particle paths. The first-order peak angles are about $41.9^\circ$, $29.4^\circ$ and $14.2^\circ$. Curves are calculated phase sums, not measured data or a fit to the [Davisson–Germer experiment](davisson-germer-experiment.md).

At $100\,\mathrm V$, $\lambda\simeq0.12264\,\mathrm{nm}$ and the positive first-order angle is $\arcsin(\lambda/d)\simeq29.4^\circ$. At $400\,\mathrm V$, the [wavelength](wavelength.md) halves and this angle becomes about $14.2^\circ$. Increasing $N$ narrows each peak through more selective [interference](interference-wave-propagation.md), while increasing [momentum](momentum.md) brings a fixed-order peak nearer the normal. Unequal site amplitudes, multiple scattering, a three-dimensional [crystal lattice structure factor](crystal-lattice-structure-factor.md), and finite detector acceptance can change this simple picture; it is an explanatory model with hypothetical inputs.

## ↑ Ancestors (8)

1. [Electron diffraction](electron-diffraction.md)
2. [Diffraction](diffraction.md)
3. [Scattering amplitude](scattering-amplitude.md)
4. [Quantum scattering](quantum-scattering.md)
5. [Quantum mechanics](quantum-mechanics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Davisson–Germer experiment](davisson-germer-experiment.md)
- [Electron diffraction](electron-diffraction.md)
