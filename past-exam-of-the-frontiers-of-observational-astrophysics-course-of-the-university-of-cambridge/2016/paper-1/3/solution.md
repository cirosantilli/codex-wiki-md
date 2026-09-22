<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

In a [CCD](../../../../charge-coupled-device.md), absorbed optical [photons](../../../../photon.md) create photoelectrons collected in electrostatic wells beneath gate electrodes. During readout, clock voltages move the charge packets row by row into a serial register; serial clocks move them one [pixel](../../../../pixel.md) at a time to an output node. The node converts charge to a voltage, approximately $\Delta V=Q/C$, which is amplified and digitized. [pixel](../../../../pixel.md) addresses are recovered from the row and serial-clock sequence. Resetting and sampling the output between packets establishes the baseline. Efficient transfer preserves charge; trapping or incomplete transfer produces loss and trailing. This is [CCD clocked charge transfer](../../../../ccd-clocked-charge-transfer.md), not independent wiring of an [amplifier](../../../../amplifier.md) to every imaging [pixel](../../../../pixel.md).[§7, SIS: charge generation, electrode-clock transfer and preamplifier readout](../../../../asca-technical-description-sis-by-nasa-heasarc.md)

[dark current](../../../../dark-current-physics.md) is thermally generated charge accumulated even without illumination. If its mean rate is $d$ [electrons](../../../../electron.md) per [pixel](../../../../pixel.md) per second, a single exposure adds mean $dt$ and Poisson [variance](../../../../variance-split.md) $dt$. Cooling the detector and using low-defect material suppresses this generation. A dark [calibration](../../../../calibration-differential-geometry.md) removes the reproducible mean pattern, but cannot remove the dark [electrons](../../../../electron.md)' random [shot noise](../../../../shot-noise.md) in the science exposure. [read noise](../../../../read-noise.md) comes from measuring the output packet and resetting the sense node, [amplifiers](../../../../amplifier.md) and electronics; write its rms as $r$ [electrons](../../../../electron.md) per read. [correlated double sampling](../../../../correlated-double-sampling.md) reduces reset and correlated offsets by subtracting the baseline measurement from the signal measurement. Low-noise electronics and an appropriate slower readout reduce the remaining contribution. The [CCD noise budget](../../../../ccd-noise-budget.md) for $M$ separate exposures combined over total time $t$ contains independent dark and read contributions $dt+Mr^2$, not $(dt)^2+M^2r^2$. Long exposures reduce repeated [read noise](../../../../read-noise.md), but saturation, cosmic rays and tracking requirements constrain the exposure length. On-chip binning can reduce read-noise penalties for a fixed binned area at the cost of angular sampling.

For the source and sky calculation, define the count conversion factor $K=At\Delta\nu/(h\nu)$ and the source flux per [pixel](../../../../pixel.md) $s_\nu=F_\nu/N_{\rm pix}$. The ideal source and background [electron](../../../../electron.md) counts are $S=Ks_\nu$ and $B=Kb_\nu\Omega_{\rm pix}$. These assume unit throughput and [quantum efficiency](../../../../quantum-efficiency.md), approximately constant quantities across the band and a well-determined mean sky level from many background [pixels](../../../../pixel.md). Source and sky [photons](../../../../photon.md) have independent Poisson fluctuations, so the [variance](../../../../variance-split.md) after subtracting that mean sky is $S+B$. Subtracting a background removes its mean, not its [photon](../../../../photon.md) noise. Therefore

$$
R=\frac S{\sqrt{S+B}}=\frac{F_\nu}{N_{\rm pix}}\left[\frac{At\Delta\nu}{h\nu(F_\nu/N_{\rm pix}+b_\nu\Omega_{\rm pix})}\right]^{1/2}.
$$

Thus **the required expression follows directly from adding photon-count [variances](../../../../variance-split.md)**. Finite sky-estimation noise, [dark current](../../../../dark-current-physics.md) and [read noise](../../../../read-noise.md) would add further [variance](../../../../variance-split.md). A nonunit common efficiency replaces $A$ by the effective collecting area; a nonflat spectrum requires the corresponding [frequency](../../../../frequency.md) integral. For example, estimating the sky from one equally exposed background [pixel](../../../../pixel.md) would add an extra $B$, whereas a large sky region makes that extra term small.

With $A=\pi(1\,\mathrm m)^2$ and the supplied [photon](../../../../photon.md) [frequency](../../../../frequency.md), the sky flux per [pixel](../../../../pixel.md) is $b_\nu\Omega_{\rm pix}=1.75\times10^{-32}\,\mathrm{W\,m^{-2}\,Hz^{-1}}$. Multiplying arcsecond-squared [pixel](../../../../pixel.md) area by brightness per arcsecond squared already gives a flux: no additional steradian conversion belongs in this product. Rearranging gives

$$
\frac t{R^2}=\frac{h\nu}{A\Delta\nu}\frac{F_\nu/N_{\rm pix}+b_\nu\Omega_{\rm pix}}{(F_\nu/N_{\rm pix})^2}.
$$

Using $h=6.62607015\times10^{-34}\,\mathrm{J\,s}$ yields

<a id="3/table-ideal-per-pixel-source-and-sky-rates-and-exposure-divided-by-squared-signal-to-noise-ratio"></a>
| $F_\nu\ (\mathrm{W\,m^{-2}\,Hz^{-1}})$ | Source rate per [pixel](../../../../pixel.md) $\mathrm{s^{-1}}$ | Sky rate per [pixel](../../../../pixel.md) $\mathrm{s^{-1}}$ | $t/R^2\ (\mathrm s)$ |
| --- | --- | --- | --- |
| $10^{-29}$ | $98.8$ | $13.8$ | **$0.0115$** |
| $10^{-30}$ | $9.88$ | $13.8$ | **$0.243$** |
| $10^{-31}$ | $0.988$ | $13.8$ | **$15.2$** |

The first case is mainly source-shot-noise limited, while the last is strongly sky limited. At high source brightness $t/R^2\propto F_\nu^{-1}$; at low source brightness it approaches $F_\nu^{-2}$. Reducing source flux by ten can therefore require nearly a hundred times the exposure once sky noise dominates. These are per-pixel values for the ideal model, not guaranteed integration times including [calibration](../../../../calibration-differential-geometry.md), cosmic rays or [read noise](../../../../read-noise.md).

Increasing the diameter increases both source and sky [photon](../../../../photon.md) rates as $D^2$ for fixed angular [pixels](../../../../pixel.md). In this ideal limit the required exposure decreases as $D^{-2}$, whereas the stated [telescope](../../../../telescope.md) cost increases as $D^{2.5}$: collecting area grows only as cost to the power $0.8$. A larger ground [telescope](../../../../telescope.md) does not remove atmospheric [photons](../../../../photon.md) or recover arbitrary wavefront information lost in a long seeing-limited exposure. Space observations avoid atmospheric airglow, weather and [atmospheric turbulence](../../../../atmospheric-turbulence.md), and offer stable high-resolution imaging and access to very faint structure. They still have zodiacal light, instrumental backgrounds and their own [calibration](../../../../calibration-differential-geometry.md) limits. [adaptive optics](../../../../adaptive-optics.md) can provide excellent ground-based resolution in suitable fields, but its guide-star, [wavelength](../../../../wavelength.md) and field-dependent limitations do not remove the need for space-based continuum imaging. **The need is for complementary low-background, stable and high-resolution measurements; the cost exponent alone is not a proof that every imaging programme is cheaper in space.**

For X rays, one fully absorbed [photon](../../../../photon.md) produces many [electron-hole pairs](../../../../electron-hole-pair.md) in [silicon](../../../../silicon.md), rather than one optical photoelectron count. At moderate [surface brightness](../../../../surface-brightness.md), the [probability](../../../../probability.md) of two [photons](../../../../photon.md) landing in the same event island during one [CCD](../../../../charge-coupled-device.md) frame is small. The charge packet or sum over neighbouring split-event [pixels](../../../../pixel.md) then supplies a pulse height for each [photon](../../../../photon.md), while its [pixel](../../../../pixel.md) position supplies the image coordinate. Calibrating pulse height against energy produces an event list from which a spectrum can be accumulated for any spatial region. [photon pile-up](../../../../photon-pile-up.md) at larger occupancies merges [photon](../../../../photon.md) energies and corrupts both spectra and event grades, so fast enough frames and event-pattern screening are essential.[§7, SIS: silicon electron-hole yield, charge collection and imaging spectroscopy](../../../../asca-technical-description-sis-by-nasa-heasarc.md)

A measured [silicon](../../../../silicon.md) pair-creation energy $w\simeq3.65\,\mathrm{eV}$ gives $N_e=E/w\simeq2.74\times10^3$ [electrons](../../../../electron.md) for a $10\,\mathrm{keV}$ [photon](../../../../photon.md). Let $F$ be the [Fano factor](../../../../fano-factor.md) of pair production, $n_r$ the number of independently read [pixels](../../../../pixel.md) in the event sum, and $r$ the rms [read noise](../../../../read-noise.md) per [pixel](../../../../pixel.md). Then

$$
\sigma_E=w\sqrt{F\frac Ew+n_rr^2+\sigma_d^2+\cdots},\qquad \Delta E_{\rm FWHM}=2\sqrt{2\ln2}\,\sigma_E.
$$

The [Fano-limited X-ray CCD energy resolution](../../../../fano-limited-x-ray-ccd-energy-resolution.md) using the representative [silicon](../../../../silicon.md) value $F\simeq0.12$ gives an ideal Fano-limited **$\Delta E_{\rm FWHM}\simeq0.16\,\mathrm{keV}$ at $10\,\mathrm{keV}$**, or resolving power $E/\Delta E\simeq64$. Finite [read noise](../../../../read-noise.md), charge loss and event summing broaden this; an order-of-magnitude practical estimate is a few tenths of a keV, but the particular detector's value is not determined by the given optical-pixel parameters. These $w$ and $F$ values are external detector properties, not supplied question data. Treating every pair as independent Poisson production instead would give $0.19\,\mathrm{keV}$ rms, or $0.45\,\mathrm{keV}$ FWHM; stating which width is meant avoids conflating those estimates. Radiation-induced charge-transfer inefficiency requires additional gain and spectral-response [calibration](../../../../calibration-differential-geometry.md).[§4.7, non-uniform CTI: silicon yield, Fano factor near 0.12 and FWHM resolution formula](../../../../the-asca-data-reduction-guide-by-nasa-heasarc.md)

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2016](../../split.md)
4. [Past exam of the frontiers of Observational Astrophysics course of the University of Cambridge](../../../split.md)
5. [Frontiers of Observational Astrophysics course of the University of Cambridge](../../../../frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
