<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [optical telescope](../../../../optical-telescope.md) supplies collecting area and spatial selection, the spectral selector supplies a passband, and the [photodetector](../../../../photodetector.md) converts received [radiant flux](../../../../radiant-flux.md) into a measured signal. For an extended source, a useful schematic photon count is

$$
N_s\simeq\eta\tau A\Omega\int_{\rm band}\frac{L_\lambda\lambda}{hc}\,d\lambda,
$$

where $A\Omega$ is the [etendue](../../../../etendue.md), $\tau$ the integration time, $\eta$ the net transmission and [quantum efficiency](../../../../quantum-efficiency.md), and $L_\lambda$ the [spectral radiance](../../../../spectral-radiance.md). An illustrative independent-noise model gives

$$
\mathrm{SNR}\simeq\frac{N_s}{\sqrt{N_s+N_b+N_d+\sigma_{\rm read}^2}}.
$$

Here $N_b$ and $N_d$ denote background and dark counts, and $\sigma_{\rm read}$ is readout [standard deviation](../../../../standard-deviation.md). This makes the roles of the three components explicit.

A larger [optical telescope](../../../../optical-telescope.md) collects more photons at fixed angular pixel size and improves the [diffraction-limited resolution](../../../../diffraction-limited-resolution.md). Its limits include [optical aberrations](../../../../optical-aberration.md), alignment, launch size, [stray light](../../../../stray-light.md) and pointing. Conservation of [etendue](../../../../etendue.md) constrains simultaneous collecting area and angular acceptance. Increasing spatial resolution by narrowing a pixel's [solid angle](../../../../solid-angle.md) reduces its photons.

A narrower spectral passband or higher [spectral resolving power](../../../../spectral-resolving-power.md) separates diagnostic features and rejects unwanted background, but usually reduces photons per channel and hence [signal-to-noise ratio](../../../../signal-to-noise-ratio.md). Selector transmission, leakage, slit width, detector format and the required time cadence limit the trade. A wider band helps only insofar as it adds useful signal rather than mostly background.

The [photodetector](../../../../photodetector.md)'s [quantum efficiency](../../../../quantum-efficiency.md), dark current, read noise, dynamic range and response time determine conversion losses and added noise. Cooling can suppress thermal background and dark current, but cannot remove [photon shot noise](../../../../photon-shot-noise.md). Longer integration improves a stationary signal's [signal-to-noise ratio](../../../../signal-to-noise-ratio.md) until motion, saturation, drift or required cadence becomes limiting.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
