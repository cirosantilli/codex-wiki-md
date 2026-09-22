<h1 id="section-d/d13/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Temperature](../../../../../../temperature-split.md) changes affect measurements through several routes. [Thermal expansion](../../../../../../thermal-expansion.md) changes lengths and alignments; temperature-dependent resistance and [refractive index](../../../../../../refractive-index.md) change electrical and optical calibrations; [temperature](../../../../../../temperature-split.md) differences between dissimilar junctions generate [Seebeck effect](../../../../../../seebeck-effect.md) voltages. These slow environmental changes are distinct from unavoidable equilibrium [thermal fluctuations](../../../../../../thermal-fluctuation.md) and [Johnson-Nyquist noise](../../../../../../thermal-electrical-noise.md). A useful strategy identifies the coupling to the measured signal before choosing a remedy.

Reduce environmental coupling by enclosing the apparatus against drafts, using thermal insulation and radiation shields, isolating heat sources, and minimizing dissipated power. A vacuum enclosure suppresses [convection](../../../../../../convection-split.md) but leaves [thermal conduction](../../../../../../thermal-conduction.md) and [thermal radiation](../../../../../../thermal-radiation.md) paths to control. A large [heat capacity](../../../../../../heat-capacity.md) reduces rapid [temperature](../../../../../../temperature-split.md) excursions. In a simple thermal model with [heat capacity](../../../../../../heat-capacity.md) $C_T$ and [thermal conductance](../../../../../../thermal-conductance.md) $G_T$ to a reservoir, the [relaxation time](../../../../../../relaxation-time.md) is $C_T/G_T$, so adequate settling time is necessary after changing the apparatus. A [temperature](../../../../../../temperature-split.md) sensor close to the sensitive element and stable [negative feedback](../../../../../../negative-feedback.md) heating or cooling can regulate its [temperature](../../../../../../temperature-split.md); poorly placed sensors or excessive feedback gain can leave gradients or cause oscillations.

Electrical [thermal noise](../../../../../../thermal-noise.md) has the classical low-frequency one-sided [voltage](../../../../../../voltage.md) [power spectral density](../../../../../../power-spectral-density.md)

$$
S_V(f)=4k_BTR,\qquad \boxed{V_{\mathrm{rms}}=\sqrt{4k_BTRB}}
$$

for a [resistor](../../../../../../resistor.md) measured over a flat [bandwidth](../../../../../../bandwidth-signal-processing.md) $B$ without significant loading. More generally replace $B$ by the [effective noise bandwidth](../../../../../../effective-noise-bandwidth.md). Lower [temperature](../../../../../../temperature-split.md) or narrower [bandwidth](../../../../../../bandwidth-signal-processing.md) reduces the [noise](../../../../../../noise-signal-processing.md), and resistance choices must account for source loading and the amplifier's own [voltage](../../../../../../voltage.md) and current [noise](../../../../../../noise-signal-processing.md). A [lock-in amplifier](../../../../../../lock-in-amplifier.md) uses modulation and narrowband detection to reject much low-frequency drift and out-of-band [noise](../../../../../../noise-signal-processing.md), while [thermal noise](../../../../../../thermal-noise.md) inside the accepted band remains. [Temperature](../../../../../../temperature-split.md) stabilization does not remove equilibrium fluctuations.

Use a matched reference or differential bridge to reject common environmental changes. Keep junctions isothermal and choose matched materials to reduce thermoelectric offsets. For a resistance measurement, reversing a small test current separates a stable offset from the wanted [voltage](../../../../../../voltage.md):

$$
V(+I)=IR+V_{\mathrm{th}},\qquad V(-I)=-IR+V_{\mathrm{th}},\qquad \boxed{R=\frac{V(+I)-V(-I)}{2I}.}
$$

Reversal must be fast enough that the offset stays approximately fixed, with enough settling time and sufficiently little self-heating. Recording the sample [temperature](../../../../../../temperature-split.md) permits a measured calibration slope $dS/dT$ to correct a signal to a reference [temperature](../../../../../../temperature-split.md); the correction's calibration and [thermometer](../../../../../../thermometer.md) uncertainties must be propagated. Independent [white noise](../../../../../../white-noise.md) fluctuations decrease under averaging, whereas correlated [temperature](../../../../../../temperature-split.md) drift may not decrease as the inverse square root of the number of readings. [Temperature](../../../../../../temperature-split.md) records and repeated reference measurements help distinguish the two.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [D13](../../d13.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
