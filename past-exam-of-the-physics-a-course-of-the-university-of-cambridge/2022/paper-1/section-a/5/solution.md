<h1 id="section-a/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For the $110\,\mathrm{Hz}$ fundamental alone, the [Nyquist–Shannon sampling theorem](../../../../../nyquist-shannon-sampling-theorem.md) places the limiting [sampling rate](../../../../../sampling-rate.md) at twice that [frequency](../../../../../frequency.md):

$$
\boxed{f_s\gtrsim2(110\,\mathrm{Hz})=220\,\mathrm{samples\,s^{-1}}.}
$$

Use a rate strictly above this boundary for a sinusoid of unknown [phase](../../../../../phase-waves.md): exactly two samples per cycle can, for a particular [phase](../../../../../phase-waves.md), all fall at zero. If higher [Fourier harmonics](../../../../../fourier-harmonic.md) are retained, the [sampling rate](../../../../../sampling-rate.md) must instead exceed twice the highest retained [frequency](../../../../../frequency.md), or those components must be removed to prevent [aliasing](../../../../../aliasing.md).

For a straightforward [discrete Fourier transform](../../../../../discrete-fourier-transform-split.md) estimate, [Fourier frequency resolution](../../../../../fourier-frequency-resolution.md) obeys $\Delta f\sim1/T_{\mathrm{obs}}$. Resolving $0.07\,\mathrm{Hz}$ therefore suggests

$$
\boxed{T_{\mathrm{obs}}\gtrsim\frac1{0.07\,\mathrm{Hz}}=14.3\,\mathrm s.}
$$

At the limiting [sampling rate](../../../../../sampling-rate.md) this is about $f_sT_{\mathrm{obs}}\simeq3143$ samples. These are the usual sampling and spectral-resolution estimates. The $14.3\,\mathrm s$ value is not a universal lower bound on single-tone [frequency estimation](../../../../../frequency-estimation.md): fitting a sinusoidal model with sufficiently low noise can estimate its [frequency](../../../../../frequency.md) more precisely than the spacing of [discrete Fourier transform](../../../../../discrete-fourier-transform-split.md) bins. The question gives no noise level or estimator, so a sharper universal minimum time cannot be deduced.

## ↑ Ancestors (14)

1. [5](../5.md)
2. [Section A](../../section-a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
