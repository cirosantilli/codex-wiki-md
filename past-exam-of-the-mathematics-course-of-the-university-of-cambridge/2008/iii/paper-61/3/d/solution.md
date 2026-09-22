<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A [4f pulse shaper](../../../../../../4f-pulse-shaper.md) supplies an experimental realization of [spectral pulse shaping](../../../../../../spectral-pulse-shaping.md). A first [diffraction grating](../../../../../../diffraction-grating.md) separates the frequencies of a broadband coherent pulse; a lens maps them to distinct transverse positions in its back focal plane. Place an amplitude-and-phase mask, or calibrated [spatial light modulator](../../../../../../spatial-light-modulator.md) with appropriate polarization optics, in that Fourier plane. A second lens and grating recombine the shaped spectrum into one output beam. The original schematic below shows the frequency channels and the four focal-length separations.

<a id="3/d/image-original-4f-spectral-pulse-shaping-schematic-showing-dispersing-and-recombining-gratings-two-lenses-and-a-frequency-resolved-complex-mask"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-61-spectral-shaper.png)

**[Figure 1](#3/d/image-original-4f-spectral-pulse-shaping-schematic-showing-dispersing-and-recombining-gratings-two-lenses-and-a-frequency-resolved-complex-mask). Original 4f spectral pulse-shaping schematic showing dispersing and recombining gratings, two lenses, and a frequency-resolved complex mask**.

If the mask is $M(\omega)=A(\omega)e^{i\varphi(\omega)}$, then $\widetilde E_{\rm out}=M\widetilde E_{\rm in}$. In principle choose $M=\widetilde E_{\rm target}/\widetilde E_{\rm in}$ wherever the input spectrum is nonzero and recover the temporal waveform by inverse [Fourier transform](../../../../../../fourier-transform.md). Set the desired real physical field by conjugate symmetry of its positive and negative frequency components; its envelope and carrier phase implement the optimized control in the appropriate interaction frame.

A passive mask cannot amplify spectral components or create frequencies absent from the input, so the desired waveform must respect available bandwidth and may need overall rescaling or amplification elsewhere. Finite spectral resolution limits the useful temporal window, while total bandwidth limits the shortest temporal features. A phase-only modulator cannot in general implement independent amplitude and phase shaping without extra optics. These are hardware admissibility constraints, not corrections supplied by the variational calculation after the fact.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
