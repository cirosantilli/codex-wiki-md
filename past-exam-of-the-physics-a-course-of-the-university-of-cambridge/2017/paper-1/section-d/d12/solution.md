<h1 id="section-d/d12/solution">Solution</h1>

↑ **Parent:** [D12](../d12.md)

**Ideal spectrum.** Write $P_i(f)=C/(f^2+f_c^2)$, with $C>0$. The [overdamped harmonic-trap power spectrum](../../../../../overdamped-harmonic-trap-power-spectrum.md) is a [Lorentzian line shape](../../../../../lorentzian-line-shape.md):

$$
P_i\simeq\frac C{f_c^2}\quad(f\ll f_c),\qquad
P_i\simeq\frac C{f^2}\quad(f\gg f_c).
$$

Thus its [log-log plot](../../../../../log-log-plot.md) is horizontal at low [frequency](../../../../../frequency.md) and approaches slope $-2$ at high [frequency](../../../../../frequency.md), changing around $f_c$. The left panel below compares two characteristic frequencies with the same illustrative $C$; a common numerator is explicitly assumed for this sketch. Their high-frequency tails coincide and their low-frequency plateaux differ as $f_c^{-2}$.

<a id="section-d/d12/image-ideal-lorentzian-spectra-at-two-corner-frequencies-and-the-measured-spectrum-with-its-graphical-corner-estimate"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-1-d12-noise-spectra.png)

**[Figure 5](#section-d/d12/image-ideal-lorentzian-spectra-at-two-corner-frequencies-and-the-measured-spectrum-with-its-graphical-corner-estimate). Ideal Lorentzian spectra at two corner frequencies and the measured spectrum with its graphical corner estimate**.

The right panel plots all nine original data points, including the very-low-frequency excess and the highest-frequency suppression. It also shows the ideal curve inferred only from the requested intermediate range.

**Graphical corner estimate.** Between roughly $1$ and $100\,\mathrm{Hz}$ the measured [power spectral density](../../../../../power-spectral-density.md) is approximately the plateau $P_0=10^{-6}\,\mathrm{V^2\,Hz^{-1}}$. At $10^4$ and $10^5\,\mathrm{Hz}$,

$$
f^2P_m(f)\simeq1\,\mathrm{V^2\,Hz},
$$

so the descending asymptote is $C/f^2$ with $C\simeq1\,\mathrm{V^2\,Hz}$. The [graphical corner frequency of a Lorentzian spectrum](../../../../../graphical-corner-frequency-of-a-lorentzian-spectrum.md) is where these asymptotes intersect:

$$
\boxed{f_c=\sqrt{\frac C{P_0}}\simeq10^3\,\mathrm{Hz}.}
$$

Independently, the measured value $P_m(1000\,\mathrm{Hz})=5\times10^{-7}\,\mathrm{V^2\,Hz^{-1}}=P_0/2$ is exactly the half-plateau condition $P_i(f_c)=P_0/2$. Both graphical readings agree. The inferred ideal curve is approximately

$$
P_i(f)=\frac{10^{-6}\,\mathrm{V^2\,Hz^{-1}}}{1+(f/1000\,\mathrm{Hz})^2}.
$$

**Low-frequency excess and recording duration.** The two lowest-frequency measurements increase approximately as $1/f$, whereas the ideal trapped oscillator tends to a constant plateau. This resembles [flicker noise](../../../../../flicker-noise.md) or slow apparatus drift superposed on the motion. The [transimpedance amplifier](../../../../../transimpedance-amplifier.md), detector or environment could contribute; the spectrum alone does not identify the source uniquely. It would be incorrect to attribute that whole excess to the ideal Brownian oscillator.

A finite record of duration $T$ has ordinary [Fourier frequency resolution](../../../../../fourier-frequency-resolution.md) of order $1/T$. Resolving the lowest tabulated [frequency](../../../../../frequency.md) $0.01\,\mathrm{Hz}$ therefore requires at least

$$
\boxed{T_{\min}\simeq\frac1{0.01\,\mathrm{Hz}}=100\,\mathrm s.}
$$

This is a formal lower bound corresponding to about one cycle; a reliable noise-spectrum estimate normally needs a substantially longer record and averaging.

**Sampling.** The largest reported [frequency](../../../../../frequency.md) is $f_{\max}=10^6\,\mathrm{Hz}$. The [Nyquist–Shannon sampling theorem](../../../../../nyquist-shannon-sampling-theorem.md) therefore gives the Nyquist lower bound

$$
\boxed{f_s\ge2f_{\max}=2.0\times10^6\,\mathrm{samples\,s^{-1}}.}
$$

In practice choose a rate above $2\,\mathrm{MS\,s^{-1}}$, with an analogue [anti-aliasing filter](../../../../../anti-aliasing-filter.md) suppressing unmeasured content above half the [sampling rate](../../../../../sampling-rate.md). Exact equality cannot recover an arbitrary pure sinusoid precisely at the boundary for every phase; it is the limiting lower-bound answer rather than a comfortable practical sampling design.

**High-frequency departure and [amplifier](../../../../../amplifier.md) design.** Extrapolating the fitted $f^{-2}$ tail to $10^6\,\mathrm{Hz}$ predicts approximately $10^{-12}\,\mathrm{V^2\,Hz^{-1}}$, while the measured value is $10^{-15}\,\mathrm{V^2\,Hz^{-1}}$. The observed drop from $10^5$ to $10^6\,\mathrm{Hz}$ has effective logarithmic slope $-5$, much steeper than the ideal $-2$.

A detector or [amplifier](../../../../../amplifier.md) bandwidth limit, or intentional filtering before digitization, can explain such suppression. For a [linear filter](../../../../../linear-filter.md) the [spectral density transformation under a linear filter](../../../../../spectral-density-transformation-under-a-linear-filter.md) is $P_{\rm out}=|H|^2P_{\rm in}$, so the last point corresponds approximately to an additional relative voltage gain $\sqrt{10^{-3}}=0.0316$, if attributed entirely to the readout transfer function. One additional point does not determine a unique filter order or identify the circuit responsible.

Rolling off an [amplifier](../../../../../amplifier.md)'s gain beyond the useful [signal](../../../../../signal.md) band reduces integrated high-frequency [noise](../../../../../noise-signal-processing.md), suppresses interference, and helps prevent [aliasing](../../../../../aliasing.md) in the [analogue-to-digital converter](../../../../../analog-to-digital-converter.md). Limiting high-frequency loop gain can also improve feedback stability and suppress unwanted oscillation. The cutoff must retain the frequencies needed for the measurement; excessive filtering would distort the desired fluctuation spectrum itself.

## ↑ Ancestors (14)

1. [D12](../d12.md)
2. [Section D](../../section-d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
