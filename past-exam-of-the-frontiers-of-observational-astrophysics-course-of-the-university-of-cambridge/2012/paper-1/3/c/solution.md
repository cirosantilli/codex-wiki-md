<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [charge-coupled device](../../../../../charge-coupled-device.md) converts absorbed [photons](../../../../../photon.md) into stored charge in semiconductor potential wells. An exposure accumulates a pixelated image; clocked electrodes transfer rows toward a serial register and output amplifier. [Quantum efficiency](../../../../../quantum-efficiency.md), pixel sampling and optical throughput connect collected [photons](../../../../../photon.md) to the expected signal. In ordinary optical imaging it primarily counts photoelectrons rather than independently measuring every [photon](../../../../../photon.md)'s [energy](../../../../../energy-split.md).

The [CCD noise budget](../../../../../ccd-noise-budget.md) combines source and sky [shot noise](../../../../../shot-noise.md), dark-current fluctuations and [read noise](../../../../../read-noise.md). For an aperture containing $n$ pixels, known background expectation $N_b$, total dark expectation $N_d$, source expectation $N_s$ and per-pixel [read noise](../../../../../read-noise.md) $r$,

$$
\mathrm{SNR}=\frac{N_s}{\sqrt{N_s+N_b+N_d+nr^2}}.
$$

Estimating the background from a finite separate region adds its own uncertainty. Cooling reduces [dark current](../../../../../dark-current-physics.md); longer integration reduces the relative importance of one read but can encounter saturation, cosmic rays or changing conditions. [Full well capacity](../../../../../full-well-capacity.md), amplifier gain, [linearity](../../../../../linearity.md), blooming and charge-transfer efficiency limit useful [detector dynamic range](../../../../../detector-dynamic-range.md).

Bias frames establish the electronic offset; matched dark frames characterize time- and temperature-dependent dark signal. Flat fields calibrate pixel-to-pixel response and illumination, with appropriate attention to [wavelength](../../../../../wavelength.md). Bad-pixel masks, repeated exposures and dithering help reject defects and cosmic rays. A calibrated [PSF](../../../../../point-spread-function-split.md) and astrometric solution are needed for reliable [photometry](../../../../../photometry-optics.md) and positions. High [quantum efficiency](../../../../../quantum-efficiency.md) and stable linear integration are advantages, but an uncalibrated count array is not yet an astronomical [flux](../../../../../flux.md) map.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the frontiers of Observational Astrophysics course of the University of Cambridge](../../../../split.md)
6. [Frontiers of Observational Astrophysics course of the University of Cambridge](../../../../../frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
