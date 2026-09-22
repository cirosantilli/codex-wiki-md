# Michelson interferometer

↑ **Parent:** [Temporal optical coherence](temporal-optical-coherence.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Michelson_interferometer)

A [Michelson interferometer](michelson-interferometer.md) divides [light](light.md) at a [beam splitter](beam-splitter.md), reflects the two arms at mirrors and recombines the returning fields. For [vacuum](vacuum.md) arm lengths $\ell_1,\ell_2$, the delay magnitude is $|\tau|=2|\ell_2-\ell_1|/c$. At each coarse delay, a small mirror scan produces maxima and minima of the detected [light intensity](light-intensity.md). A [photodiode](photodiode.md) and its electrical readout resolve these changes; the scan should cover several carrier cycles while changing $|g^{(1)}|$ negligibly. MIT's laboratory guide uses a mirror actuator, [photodiode](photodiode.md) and electrical drive to scan [interference fringes](interference-fringe.md) and extract [interferometric visibility](interferometric-visibility.md).[§§II–IV: apparatus and visibility measurement](mit-8-13-14-experimental-physics-i-and-ii-junior-lab-fall-2016-spring-2017-by-mit-department-of-physics/optical-interferometry.md)

A verified motivating experiment is Shaoul Ezekiel's MIT demonstration of source-spectrum control. A [polarizer](polarizer.md) selects one or several lines from a [laser](laser.md) whose adjacent lines have orthogonal [linear polarizations](linear-polarization.md). A sampled beam goes to a scanning [Fabry–Pérot interferometer](fabry-perot-interferometer.md) to check the [optical spectrum](optical-spectrum.md); the main beam enters a [Michelson interferometer](michelson-interferometer.md), and a lens projects its [interference fringes](interference-fringe.md) onto a screen. With one selected line the fringes retain good contrast through the demonstrated delay range. With several lines their contrast falls and returns as the arm length changes. At a fixed delay with poor contrast, selecting one line restores it; at matched arms both selections give good contrast. This control isolates the role of spectral composition rather than simply the arm position. The presentation is a qualitative demonstration, not a calibrated linewidth measurement. [Shaoul Ezekiel, MIT, Coherence length and source spectrum, demonstration transcript](https://ocw.mit.edu/courses/res-6-006-video-demonstrations-in-lasers-and-optics-spring-2008/203f69980203861f374be32d61f9940e_LixwAXsN8vg.pdf).

A deliberately simpler two-line model explains the return of contrast. Take two stationary, mutually uncorrelated monochromatic contributions of equal power at $\nu_0\pm\delta\nu/2$. Their normalized [wave-field correlation](uncentered-wave-field-correlation.md) is

$$
g^{(1)}(\tau)=e^{-i2\pi\nu_0\tau}\cos(\pi\delta\nu\tau),
\qquad \mathcal V(\tau)=|\cos(\pi\delta\nu\tau)|
$$

for equal detected single-arm [light intensities](light-intensity.md). At $\tau=1/(2\delta\nu)$ the two contributions' [interference fringes](interference-fringe.md) cancel on averaging; at $\tau=1/\delta\nu$ they agree again. This is a deduction from the stipulated spectrum, not a fit to Ezekiel's two- or three-line source. Finite individual linewidths eventually damp these revivals.

For a quantitative version of the experiment, the visibility law suggests explicit controls. Measure each arm separately at every coarse delay, subtract the detector's dark signal and any measured background, then normalize by $2\sqrt{I_1I_2}/(I_1+I_2)$. Keep the returning beams aligned on the same detector region with parallel [linear polarizations](linear-polarization.md); keep detector gain fixed and avoid saturation. Resolve the small mirror scan electrically, rather than averaging over its moving [interference fringes](interference-fringe.md). Repeat scans to identify vibration or drift. These controls follow from the averaging and mode-matching assumptions in [first-order optical coherence](first-order-optical-coherence.md); loss of contrast alone cannot distinguish source decorrelation from apparatus motion, misalignment or insufficient spatial resolution. The finite travel range gives access only to a finite range of delays.

The practical gain is that [wave interference](interference-wave-propagation.md) measures field correlations even when the detector cannot follow the optical oscillation itself. A long [optical coherence length](optical-coherence-length.md) allows unequal-arm measurements; a short one localizes high contrast near matched delays. The beautiful feature is that both fading and reappearance of [interference fringes](interference-fringe.md) are sums of the same rotating [complex amplitudes](complex-amplitude.md).

## ↑ Ancestors (8)

1. [Temporal optical coherence](temporal-optical-coherence.md)
2. [First-order optical coherence](first-order-optical-coherence.md)
3. [Optical coherence](optical-coherence.md)
4. [Physical optics](physical-optics.md)
5. [Optics](optics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Michelson interferometer](michelson-interferometer.md)
- [Optical coherence](optical-coherence.md)
- [Optical coherence length](optical-coherence-length.md)
- [Optical path length](optical-path-length.md)
- [Photon gas](photon-gas.md)
- [Temporal optical coherence](temporal-optical-coherence.md)
