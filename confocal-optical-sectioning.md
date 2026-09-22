# Confocal optical sectioning

↑ **Parent:** [Confocal microscopy](confocal-microscopy.md)

At one depth, scan the illumination spot across $x$ and $y$ and assign the detector reading during each dwell interval to a [pixel](pixel.md). Move the specimen or objective [optical lens](lens-optics.md) axially to acquire the next depth. A stack of these optical sections samples three-dimensional structure. With beam scanning, the returning [fluorescence](fluorescence-split.md) commonly retraces the scanning optics: this descanning holds the image of the currently illuminated point at the detection pinhole. With stage scanning, the fixed spot and pinhole remain aligned while the specimen moves. [Introduction, manuscript p. 2; Fig. 3 and caption, pp. 7–8: scanning and stationary return beam](confocal-microscopy-chapter-manuscript-by-brad-amos-and-others.md)

An optical section is a depth-weighted image of an intact specimen, with a finite axial response and tails. A physical cut actually separates a slice of material; its thickness and cutting damage are properties of the preparation. Changing [optical focus](focus-optics.md) selects another optical section without removing a slice, although illumination can still damage a specimen. Neither a thin physical slice nor a sharply displayed optical section makes the imaging [point spread function](point-spread-function-split.md) infinitely narrow. [Fig. 2 discussion: focused-light sections rather than physical sectioning](introductory-confocal-concepts-by-nikon-instruments-inc.md)

Point response and section thickness answer different questions. For a spatially uniform, very thin fluorescent sheet, its response versus axial displacement is proportional to the lateral [integral](integral-split.md) of the three-dimensional confocal response,

$$
R_{\rm sheet}(z)\propto\int_{\mathbb R^2}H_a(x,y,z)\,dx\,dy.
$$

Consequently a trace through a single bead, $H_a(0,0,z)$, does not by itself give the sheet's optical-section thickness. State which object and which [full width at half maximum](full-width-at-half-maximum.md) are being measured. A smaller axial sampling step gives more samples of the same response, rather than automatically improving [diffraction-limited resolution](diffraction-limited-resolution.md). [Appendix §6, manuscript pp. 42–43: thin fluorescent sheet translated through focus](confocal-microscopy-chapter-manuscript-by-brad-amos-and-others.md)

## ↑ Ancestors (8)

1. [Confocal microscopy](confocal-microscopy.md)
2. [Fluorescence microscope](fluorescence-microscope.md)
3. [Fluorescence](fluorescence-split.md)
4. [Physical optics](physical-optics-split.md)
5. [Optics](optics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Confocal microscopy](confocal-microscopy.md)
- [Confocal pinhole throughput](confocal-pinhole-throughput.md)
- [Fluorescence microscope](fluorescence-microscope.md)
- [Fluorescent bead experiment for confocal microscopy](fluorescent-bead-experiment-for-confocal-microscopy.md)
