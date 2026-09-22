<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In [angular differential imaging](../../../../../../../angular-differential-imaging.md), the instrument is operated in pupil tracking: its pupil and associated quasi-static [speckle patterns](../../../../../../../speckle-pattern.md) remain nearly fixed on the detector, while the sky rotates with the [parallactic angle](../../../../../../../parallactic-angle.md). A reference stellar [point spread function](../../../../../../../point-spread-function.md) is formed from other exposures, preferably excluding frames where a companion remains at almost the same location. Subtract the reference from each exposure, then derotate the residuals into the sky frame and combine them. A companion adds coherently after derotation; the stellar residuals are reduced. This is the technique described in the [original angular-differential-imaging analysis](https://arxiv.org/abs/astro-ph/0512335). At angular separation $\rho$, the approximate displacement is $\rho\Delta\psi$, so useful diversity normally requires $\rho|\Delta\psi|\gtrsim\lambda/D$.

In [simultaneous spectral differential imaging](../../../../../../../simultaneous-spectral-differential-imaging.md), acquire nearby spectral-band images simultaneously, for example with a [beam splitter](../../../../../../../beam-splitter.md) and filters or an [integral field spectrograph](../../../../../../../integral-field-spectrograph.md). Stellar [speckle patterns](../../../../../../../speckle-pattern.md) approximately move radially in proportion to [wavelength](../../../../../../../wavelength.md). Rescale each image by $\lambda_0/\lambda$ and normalize the stellar flux before subtracting bands. The speckles then approximately align, while a companion at a fixed sky position moves in the rescaled coordinates. A companion absorption band can also distinguish its spectrum from the star: methane bands are useful for cool companions, as in the [TRIDENT instrument description](https://arxiv.org/abs/astro-ph/0212033), but methane is not a universal companion property. Positional diversity scales as $\rho|\Delta\lambda|/\lambda$.

**ADI uses sky rotation; SSDI uses simultaneous spectral diversity and wavelength scaling of stellar speckles.**

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 338](../../../../paper-338-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
