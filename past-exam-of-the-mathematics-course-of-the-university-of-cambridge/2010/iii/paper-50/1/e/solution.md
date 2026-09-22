<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

[Spectral pulse shaping](../../../../../../spectral-pulse-shaping.md) implements a calculated optical control by modifying its complex frequency spectrum. If the available input pulse has spectrum $\widetilde E_{\mathrm{in}}(\omega)$, program a calibrated mask $M(\omega)=a(\omega)e^{i\varphi(\omega)}$ so that

$$
\boxed{\widetilde E_{\mathrm{out}}(\omega)=M(\omega)\widetilde E_{\mathrm{in}}(\omega),\qquad E_{\mathrm{out}}(t)=\frac1{2\pi}\int\widetilde E_{\mathrm{out}}(\omega)e^{-i\omega t}\,d\omega}.
$$

The temporal waveform follows from [Fourier inversion](../../../../../../fourier-inversion-theorem.md). For a real applied field, its spectrum has conjugate symmetry, so the mask must satisfy $M(-\omega)=M(\omega)^*$. Spectral phase controls interference between frequencies and hence their arrival times, chirp and temporal subpulses; spectral attenuation changes their weights. The optimized field envelope is translated into this complex mask, with compensation for known phase shifts and losses in the optical system.

A typical [4f pulse shaper](../../../../../../4f-pulse-shaper.md) contains a first [diffraction grating](../../../../../../diffraction-grating.md), a focusing lens, a mask or [spatial light modulator](../../../../../../spatial-light-modulator.md) in the common focal plane, a second lens and a second grating. The first grating separates the frequencies by angle. The first lens converts those angles into different transverse positions at the spectral Fourier plane. The pixels of the [spatial light modulator](../../../../../../spatial-light-modulator.md) modify the amplitude and phase of the corresponding frequency bins. The second lens and grating reverse this spatial dispersion and recombine the components into one shaped output beam. In the ideal symmetric layout the four consecutive propagation distances are $f,f,f,f$, giving the name $4f$.

<a id="1/e/image-spectral-pulse-shaping-with-gratings-lenses-and-a-programmable-mask-in-a-4f-arrangement"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-50-pulse-shaper.png)

**[Figure 1](#1/e/image-spectral-pulse-shaping-with-gratings-lenses-and-a-programmable-mask-in-a-4f-arrangement). Spectral pulse shaping with gratings, lenses and a programmable mask in a 4f arrangement**.

A phase-only [spatial light modulator](../../../../../../spatial-light-modulator.md) needs suitable polarization optics or another modulation stage for independent amplitude shaping. A passive mask has $0\le a(\omega)\le1$ and cannot create frequencies absent from the input; finite bandwidth and finite pixel resolution limit temporal features and the useful shaping window. These constraints must be included when converting a mathematical optimum into a laboratory pulse. The programmed mask is an [open-loop control](../../../../../../open-loop-control.md), although repeated measurements of the output pulse or system performance can be used to calibrate or optimize it experimentally.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
