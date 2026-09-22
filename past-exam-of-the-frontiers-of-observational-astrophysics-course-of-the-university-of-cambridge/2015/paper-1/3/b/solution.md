<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Atmospheric turbulence](../../../../../atmospheric-turbulence.md) produces time-dependent refractive-index fluctuations and phase errors across the telescope pupil. A large aperture's long-exposure [point spread function](../../../../../point-spread-function-split.md) is broadened approximately to $0.98\lambda/r_0$, where $r_0$ is the [Fried parameter](../../../../../fried-parameter.md), rather than the [diffraction](../../../../../diffraction.md) scale $\lambda/D$. For fixed turbulence, $r_0\propto\lambda^{6/5}$, so the [seeing](../../../../../astronomical-seeing.md) angle improves weakly as $\lambda^{-1/5}$. The [atmospheric coherence time](../../../../../atmospheric-coherence-time.md) scales with $r_0$ divided by an effective wind speed. This temporal scale concerns changing turbulence, not the optical [bandwidth](../../../../../bandwidth-signal-processing.md)'s coherence time.

**Reduce the disturbance.** A good high-altitude site, favourable weather, observing near the zenith, thermal control and dome ventilation reduce atmospheric and local [seeing](../../../../../astronomical-seeing.md). They improve the uncorrected image but do not remove all high-order wavefront distortion. [Active optics](../../../../../active-optics.md) slowly maintains the main mirror's figure and alignment; it is distinct from the rapid adaptive correction of atmospheric phase errors.

**Correct the wavefront.** [Adaptive optics](../../../../../adaptive-optics.md) uses a nearby natural [guide star](../../../../../guide-star-adaptive-optics.md) or artificial [laser guide star](../../../../../laser-guide-star.md), a [wavefront sensor](../../../../../wavefront-sensor.md), a real-time controller and a [deformable mirror](../../../../../deformable-mirror.md). A Shack-Hartmann sensor estimates local wavefront slopes; mirror actuators apply the opposite optical-path distortion fast enough to track the atmosphere. A separate fast steering element or the mirror can correct image motion. In an ideal well-corrected direction this approaches [diffraction-limited resolution](../../../../../diffraction-limited-resolution.md) and increases the concentration of light in the central image.

Finite guide-star [flux](../../../../../flux.md), actuator sampling, control latency and [anisoplanatism](../../../../../anisoplanatism.md) leave residual errors. A laser beacon samples a finite-height cone rather than the full distant-source cylinder, and a conventional laser reference does not determine absolute tip-tilt, so a natural reference remains useful. Multiple [guide stars](../../../../../guide-star-adaptive-optics.md) and multiple conjugate mirrors can widen the corrected field, with extra sensing and reconstruction complexity. These are fundamental geometry and control limits, not claims of a universal corrected sky fraction.[Single Conjugate Adaptive Optics and Multi-Conjugate Adaptive Optics sections: bandwidth, fitting, anisoplanatism, laser-beacon tilt and cone limitations](../../../../../adaptive-optics-by-european-southern-observatory.md)

**Freeze and reconstruct.** Short exposures can freeze the instantaneous [speckle pattern](../../../../../speckle-pattern.md). [Speckle interferometry](../../../../../speckle-interferometry.md) uses calibrated Fourier statistics to recover diffraction-scale structure; power-spectrum information alone loses phase, while [bispectrum](../../../../../bispectrum.md) or other phase-sensitive measurements support image reconstruction. [Lucky imaging](../../../../../lucky-imaging.md) selects sharp short frames, registers them and combines them, trading [photon](../../../../../photon.md) efficiency for improved image quality. Tip-tilt alignment alone removes image motion rather than all high-order aberration. These methods require sufficiently bright sources or references and can incur substantial read-noise penalties. Deconvolving a long-exposure image is useful only where a known [point spread function](../../../../../point-spread-function-split.md) and adequate signal preserve information; it cannot recover arbitrarily lost [spatial frequencies](../../../../../spatial-frequency.md). Moving to space avoids atmospheric [seeing](../../../../../astronomical-seeing.md), although it changes the observing platform and its limitations rather than correcting a ground-based telescope.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
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
