<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the optical system's spectral response as $A(\omega)e^{i\phi(\omega)}$. Expanding its [spectral phase](../../../../spectral-phase.md) around the pulse's central [angular frequency](../../../../angular-frequency.md) gives

$$
\phi(\omega)=\phi(\omega_0)+\phi^{(1)}(\omega_0)(\omega-\omega_0)+\frac12\phi^{(2)}(\omega_0)(\omega-\omega_0)^2+\cdots.
$$

The [group delay](../../../../group-delay.md) is $\phi^{(1)}=d\phi/d\omega$, with units of time. The linear [spectral phase](../../../../spectral-phase.md) term delays the pulse envelope by this amount. The [group delay dispersion](../../../../group-delay-dispersion.md) is $\phi^{(2)}=d^2\phi/d\omega^2$, with units of time squared. It makes the [group delay](../../../../group-delay.md) [frequency](../../../../frequency.md) dependent: $t_g(\omega)\simeq\phi^{(1)}+\phi^{(2)}(\omega-\omega_0)$. Positive [group delay dispersion](../../../../group-delay-dispersion.md) delays higher [frequencies](../../../../frequency.md) more and gives positive [chirp](../../../../chirp.md). A nonzero quadratic [spectral phase](../../../../spectral-phase.md) broadens an initially transform-limited pulse; applied to an already chirped pulse, a suitable opposite sign can compress it.

In [chirped pulse amplification](../../../../chirped-pulse-amplification.md), an ultrashort seed pulse first passes through a dispersive stretcher, often a grating-based system. This correlates [frequency](../../../../frequency.md) with arrival time and increases pulse duration while approximately preserving pulse [energy](../../../../energy-split.md), thereby lowering peak [intensity](../../../../intensity-physics.md). An optical amplifier can then increase pulse [energy](../../../../energy-split.md) without exposing the gain medium to the original short pulse's enormous peak [intensity](../../../../intensity-physics.md), reducing optical damage and unwanted nonlinear [phase](../../../../phase-waves.md) accumulation. A final dispersive compressor, typically using gratings, cancels the accumulated [spectral phase](../../../../spectral-phase.md) to recover a short, high-energy pulse. The essential components are therefore a short-pulse source, stretcher, amplifier and matched compressor; spectral gain bandwidth and higher-order [dispersion](../../../../wave-dispersion.md) limit the achievable compression.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
