<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use [spectral pulse shaping](../../../../../../spectral-pulse-shaping.md) of a broadband coherent laser pulse. A [4f pulse shaper](../../../../../../4f-pulse-shaper.md) disperses the frequency components with a diffraction grating, maps them to different transverse positions with a lens, applies a programmable complex mask at the Fourier plane, and recombines them with a second lens and grating. A [spatial light modulator](../../../../../../spatial-light-modulator.md) or suitable amplitude-and-phase modulation stages impose the mask.

Compute the desired complex spectral field by [Fourier transform](../../../../../../fourier-transform.md) of the required temporal envelope, including its phase. In the available spectral band, choose

$$
M(\omega)=\frac{\widetilde E_{\rm target}(\omega)}{\widetilde E_{\rm input}(\omega)},\qquad
\widetilde E_{\rm out}(\omega)=M(\omega)\widetilde E_{\rm input}(\omega).
$$

The mask amplitude changes the spectral weights, and its phase changes temporal interference and chirp. **Recombining the masked [spectrum](../../../../../../spectrum-functional-analysis.md) produces the shaped temporal pulse.** A phase-only device needs additional optics to implement independent amplitude control. Calibrate the mask-to-frequency mapping and verify the output pulse experimentally, correcting it iteratively if needed.

The source bandwidth must contain the requested spectral components; a passive mask attenuates rather than supplies missing energy, so an overall rescaling may be needed. Finite spectral resolution determines the accessible time window, and finite bandwidth limits rapid temporal features.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
