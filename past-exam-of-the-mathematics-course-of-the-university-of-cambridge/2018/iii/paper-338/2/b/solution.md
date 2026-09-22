<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An [integral field spectrograph](../../../../../../integral-field-spectrograph.md) obtains spectra throughout a two-dimensional field instead of along one slit alone. Its reduced [spectral data cube](../../../../../../spectral-data-cube.md) is $I(x,y,\lambda)$: two coordinates locate a spatial sampling element and the third labels [wavelength](../../../../../../wavelength.md). One slice at fixed [wavelength](../../../../../../wavelength.md) is an image; one column at fixed spatial position is an [optical spectrum](../../../../../../optical-spectrum.md). The third axis is spectral, not a third spatial direction.

Six ways to obtain such a cube illustrate the distinction between field reformatting and scanning:

- A [lenslet array](../../../../../../lenslet-array.md) divides the image into spatial elements. The [spectrograph](../../../../../../spectrograph.md) disperses each lenslet’s output into a microspectrum, with spacing and orientation chosen to avoid overlap.
- A [lenslet array](../../../../../../lenslet-array.md) feeding [optical fibers](../../../../../../optical-fiber.md) provides contiguous sampling; the fiber outputs are rearranged into a pseudo-slit for a conventional [spectrograph](../../../../../../spectrograph.md).
- A bare [optical fiber](../../../../../../optical-fiber.md) bundle samples the image and also reformats it into a pseudo-slit. Its packing fraction and coupling can leave spatial gaps or transmission losses.
- An [image slicer](../../../../../../image-slicer.md) divides the image into strips, then rearranges them end to end. Dispersion preserves position along each strip, and the reconstruction restores the second spatial coordinate.
- A scanning [Fabry–Pérot interferometer](../../../../../../fabry-perot-interferometer.md) or tunable narrow-band filter records a sequence of nearly monochromatic images, stepping the transmitted band to assemble the cube.
- Imaging [Fourier transform spectroscopy](../../../../../../fourier-transform-spectroscopy.md) records an interferogram at every spatial pixel while scanning [optical path length](../../../../../../optical-path-length.md) difference. Transforming each interferogram supplies the spectral coordinate.

The first four are simultaneous spatially multiplexed grating arrangements. The last two deliver equivalent cube coordinates by scanning; they are imaging spectrometers rather than simultaneous grating integral-field units, and variability during the scan can corrupt the cube. Detector packing, sampling, calibration and throughput determine the practical tradeoffs.

**A data cube contains one spectrum per spatial element: two sky coordinates plus wavelength.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 338](../../../paper-338-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
