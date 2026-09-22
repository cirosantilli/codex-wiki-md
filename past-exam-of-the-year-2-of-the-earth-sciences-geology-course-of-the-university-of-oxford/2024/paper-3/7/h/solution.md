<h1 id="7/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

Apply a [Fourier transform](../../../../../fourier-transform-split.md) or [discrete Fourier transform](../../../../../discrete-fourier-transform-split.md), retain the desired low-frequency coefficients and attenuate those in the high-frequency noise band with a [low-pass filter](../../../../../low-pass-filter.md), then invert. For a real signal, apply matching gains at positive and negative [frequencies](../../../../../frequency.md) to preserve [Hermitian symmetry](../../../../../hermitian-symmetry.md).

[Parseval identity for Fourier series](../../../../../parseval-identity-for-fourier-series.md) shows what an ideal coefficient cutoff does: the output [mean-square signal power](../../../../../signal-power.md) is the sum of the retained squared coefficients, and cannot exceed that of the unfiltered input. Much of the high-frequency noise can be removed, but a finite cutoff also removes genuine [square wave](../../../../../square-wave.md) harmonics. Its edges become less sharp, and a sharp spectral cutoff can exhibit the [Gibbs phenomenon](../../../../../gibbs-phenomenon.md). There is no claim of exact recovery if the noise overlaps the retained band. Noise already folded into low frequencies by [aliasing](../../../../../aliasing.md) cannot in general be removed merely by discarding the high-frequency bins afterward.

## ↑ Ancestors (12)

1. [H](../h.md)
2. [7](../../7.md)
3. [Paper 3](../../../paper-3-split.md)
4. [2024](../../../split.md)
5. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../split.md)
6. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
7. [Earth sciences (geology) course of the University of Oxford](../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
