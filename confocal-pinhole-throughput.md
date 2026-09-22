# Confocal pinhole throughput

↑ **Parent:** [Confocal microscopy](confocal-microscopy.md)

Opening the pinhole increases accepted in-focus and out-of-focus [photons](photon.md); closing it strengthens [confocal optical sectioning](confocal-optical-sectioning.md) while discarding some useful in-focus [photons](photon.md) too. In the synthetic model, $\alpha=0.5,1.5,4$ transmits approximately $0.1175,0.6753,0.9997$ of the collected in-focus emission. At $t=2$ the corresponding peak-normalized signals are about $0.0420,0.0597,0.1597$. These are calculated fractions under stated assumptions, not instrument measurements.

An Airy unit conventionally specifies a pinhole diameter equal to the first-zero diameter of the emission [Airy disk](airy-disk.md) in that plane. For an ideal circular pupil,

$$
d_{\rm AU}\simeq1.22\,\frac{\lambda_{\rm em}|M|}{\mathrm{NA}},
$$

where $M$ is the total specimen-to-pinhole [magnification](magnification.md), $\lambda_{\rm em}$ the emission [wavelength](wavelength.md) in [vacuum](vacuum.md), and $\mathrm{NA}$ the objective [numerical aperture](numerical-aperture.md). A software setting needs its specified [wavelength](wavelength.md) and relay [magnification](magnification.md); it is not a universal micrometre diameter. [Appendix §6, manuscript pp. 42–43: Airy unit defined between the focal spot's zeros and conversion to real units](confocal-microscopy-chapter-manuscript-by-brad-amos-and-others.md)

For ideal independent counting, accepted source and background means $S$ and $B$ give [photon shot noise](photon-shot-noise.md) with [variance](variance-split.md) $S+B$ and [signal-to-noise ratio in photon counting](signal-to-noise-ratio-in-photon-counting.md) $S/\sqrt{S+B}$. Closing a pinhole need not improve that ratio: it depends on how both $S$ and $B$ change. Increasing exposure or excitation to replace discarded [photons](photon.md) can cause bleaching, an irreversible loss of fluorescent emission capacity, or damage. Detection rejection occurs after excitation and therefore does not undo excitation outside the selected depth. Such material can absorb illumination and emit [photons](photon.md) even when their emission is omitted from the recorded image.

## ↑ Ancestors (8)

1. [Confocal microscopy](confocal-microscopy.md)
2. [Fluorescence microscope](fluorescence-microscope.md)
3. [Fluorescence](fluorescence.md)
4. [Physical optics](physical-optics.md)
5. [Optics](optics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
