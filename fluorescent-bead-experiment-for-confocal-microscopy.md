# Fluorescent bead experiment for confocal microscopy

↑ **Parent:** [Confocal microscopy](confocal-microscopy.md)

A useful motivating experiment moves a bead emitting [fluorescence](fluorescence.md) through the selected [optical focus](focus-optics.md) and records the detector signal against position. [Measurement of point-spread function (PSF) for confocal fluorescence microscopy by InCheon Song and others](measurement-of-point-spread-function-psf-for-confocal-fluorescence-microscopy-by-incheon-song-and-others.md) (2005, §2 and Fig. 1) describes a $543.8\,\mathrm{nm}$ [laser](laser.md) delivered through a single-mode [optical fiber](optical-fiber.md), collimation, beam-size adjustment and a dichroic [beam splitter](beam-splitter.md). A $100\times$, [numerical aperture](numerical-aperture.md) $1.3$ oil-immersion objective [optical lens](lens-optics.md) excites slide-mounted fluorescent beads and collects their emission. Emission passes a filter and collecting [optical lens](lens-optics.md), then a pinhole, before an avalanche [photodiode](photodiode.md). A three-dimensional positioning stage moves the specimen. The apparatus also contains a phase plate for deliberately modified responses.[§2 and Fig. 1, pp. 2–3: apparatus and readout](measurement-of-point-spread-function-psf-for-confocal-fluorescence-microscopy-by-incheon-song-and-others.md)

The published comparison uses nominal bead diameters $0.17,0.5,1\,\mathrm{\mu m}$: larger beads give broader measured spots. This is a control on the finite emitter, because the image is the [convolution](convolution.md) of bead emission with the confocal [point spread function](point-spread-function.md). The smallest bead has weaker [signal](signal.md) relative to [noise](noise-signal-processing.md); incorrect bead size, [defocus](defocus-aberration.md), bleaching and [optical aberrations](optical-aberration.md) limit inference from a restored response. The reported bead-size comparison concerns lateral responses; it is not a measured pinhole-size series or a measured sheet-sectioning curve.[§3.2 and Figs. 4–5, pp. 4–5; p. 6, paragraph before §3.3: error sources](measurement-of-point-spread-function-psf-for-confocal-fluorescence-microscopy-by-incheon-song-and-others.md)

To test axial pinhole selection with this kind of apparatus, the following is a proposed extension, not an additional result from that paper. Choose an isolated bead small relative to the response, centre it laterally, then step $z$ through [optical focus](focus-optics.md) while recording background-subtracted signal at several pinhole settings. Hold excitation [power](power.md), dwell interval, detector gain, emission band and sampling fixed. Preserve raw peaks before also plotting peak-normalized traces. A lower peak and faster relative decay with axial displacement would support the paired-selection mechanism; fitting only normalized widths would miss the throughput cost.

Measure blocked-excitation background, include a bead-free region, avoid detector saturation, and repeat scans in reversed order to reveal drift or bleaching. Check pinhole centring separately, since misalignment can mimic signal loss. Record bead diameter, immersion medium, [refractive index](refractive-index.md), [numerical aperture](numerical-aperture.md), [wavelengths](wavelength.md) and axial step. A finite bead is an approximation to an [optical point source](optical-point-source.md); a point trace does not certify [confocal optical sectioning](confocal-optical-sectioning.md) of a whole fluorescent sheet. Depth-dependent [spherical aberration](spherical-aberration.md), scattering and sample motion can broaden or distort the response. Increasing [magnification](magnification.md) or making a display brighter does not correct those effects.

## ↑ Ancestors (8)

1. [Confocal microscopy](confocal-microscopy.md)
2. [Fluorescence microscope](fluorescence-microscope.md)
3. [Fluorescence](fluorescence.md)
4. [Physical optics](physical-optics.md)
5. [Optics](optics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
