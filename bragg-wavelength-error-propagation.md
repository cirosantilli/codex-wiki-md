# Bragg wavelength error propagation

↑ **Parent:** [Crystal X-ray spectrometer](crystal-x-ray-spectrometer.md)

Differentiate [Bragg's law](bragg-s-law.md) at fixed correctly assigned [diffraction order](diffraction-order.md):

$$
n\lambda=2d\sin\theta,\qquad
n\,d\lambda=2\sin\theta\,dd+2d\cos\theta\,d\theta.
$$

Divide the second equality by the first. For small signed changes,

$$
\frac{\delta\lambda}{\lambda}\simeq
\frac{\delta d}{d}+\cot\theta\,\delta\theta.
$$

The [Bragg angle](bragg-angle.md) error $\delta\theta$ must be in [radians](radian.md). An error quoted for detector deflection $2\theta$ must first be halved. The expression is a first-order [Taylor expansion](taylor-expansion.md); an unknown [diffraction order](diffraction-order.md) is a discrete assignment error, not an infinitesimal perturbation.

For error bounds, add magnitudes. For independent zero-mean random errors with [standard deviations](standard-deviation.md) $\sigma_d,\sigma_\theta$, [variance](variance-split.md) addition instead gives

$$
\left(\frac{\sigma_\lambda}{\lambda}\right)^2\simeq
\left(\frac{\sigma_d}{d}\right)^2+\cot^2\theta\,\sigma_\theta^2.
$$

Correlated errors require a [covariance](covariance.md) term. A shared calibration bias does not become independent merely because many line positions are measured.

With a chosen angular error $10$ [arcseconds](arcsecond.md), $\delta\theta=4.84814\times10^{-5}\,\mathrm{rad}$, the angular contribution is $8.3972\times10^{-5}$ at $30^\circ$ and $1.7646\times10^{-5}$ at $70^\circ$. Larger [Bragg angles](bragg-angle.md) reduce this contribution because $\cot\theta$ decreases. For a nearby [spectral doublet](spectral-doublet.md), the inverse relation is $\Delta\theta\simeq\tan\theta\,\Delta\lambda/\lambda$: a fixed fractional separation spreads farther apart angularly at large [Bragg angle](bragg-angle.md).

This does not permit unlimited improvement. The geometry requires $n\lambda\leq2d$; a desired [wavelength](wavelength.md) might not have an accessible large-angle reflection with the chosen [crystal](crystal.md). Higher [diffraction orders](diffraction-order.md) can reach larger [Bragg angles](bragg-angle.md) but their strengths depend on the [crystal lattice structure factor](crystal-lattice-structure-factor.md). Finite crystal response, slit widths and source size remain relevant. An error in $d$, including uncorrected [thermal expansion](thermal-expansion.md), remains even when the angular term is small. Very near $90^\circ$, the leading angular derivative vanishes and the second-order [Taylor expansion](taylor-expansion.md) matters.

## ↑ Ancestors (11)

1. [Crystal X-ray spectrometer](crystal-x-ray-spectrometer.md)
2. [Siegbahn precision X-ray wavelength spectroscopy](siegbahn-precision-x-ray-wavelength-spectroscopy.md)
3. [X-ray emission spectroscopy](x-ray-emission-spectroscopy.md)
4. [Characteristic X-ray](characteristic-x-ray.md)
5. [X-ray tube](x-ray-tube.md)
6. [X-ray](x-ray.md)
7. [Electromagnetic radiation](electromagnetic-radiation-split.md)
8. [Electromagnetism](electromagnetism-split.md)
9. [Branches of physics](branches-of-physics.md)
10. [Physics](physics-split.md)
11. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Gaussian spectral doublet resolution](gaussian-spectral-doublet-resolution.md)
