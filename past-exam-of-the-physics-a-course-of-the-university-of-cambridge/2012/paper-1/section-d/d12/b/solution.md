<h1 id="section-d/d12/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an experimental-noise interpretation of Nyquist's theorem, a [resistor](../../../../../../resistor.md) $R$ in thermal equilibrium at [temperature](../../../../../../temperature-split.md) $T$ has one-sided open-circuit voltage-noise [spectral density](../../../../../../spectral-density-of-a-stationary-process.md)

$$
\boxed{S_V(f)=4k_BTR},\qquad
\boxed{\langle v_n^2\rangle=4k_BTR\,\Delta f}
$$

in the classical range $hf\ll k_BT$, over an approximately rectangular [bandwidth](../../../../../../bandwidth-signal-processing.md) $\Delta f$. Across a matched load, half the open-circuit voltage appears, giving available noise [power](../../../../../../power.md) $k_BT\Delta f$. This is thermal agitation, present without a mean current, and is distinct from [shot noise](../../../../../../shot-noise.md). A real readout weights the spectrum with its [transfer function](../../../../../../transfer-function.md): $\langle v_{\rm out}^2\rangle=\int_0^\infty S_V(f)|H(f)|^2df$. Cooling, reduced [bandwidth](../../../../../../bandwidth-signal-processing.md) and suitable impedance/noise matching reduce measured noise; the [resistor](../../../../../../resistor.md)'s noise does not simply disappear in an ideal amplifier model.[Printed p. 113, equations 4–8, thermal emf and bandwidth](../../../../../../thermal-agitation-of-electric-charge-in-conductors-by-harry-nyquist.md)

The bare name also has a sampling interpretation. The [Nyquist–Shannon sampling theorem](../../../../../../nyquist-shannon-sampling-theorem.md) permits exact reconstruction of a bandlimited signal from sufficiently fast uniform samples. The practical condition is **$f_s>2f_{\max}$**, with an [anti-aliasing filter](../../../../../../anti-aliasing-filter.md) before sampling; otherwise distinct continuous [frequencies](../../../../../../frequency.md) produce identical samples. Ideal reconstruction uses shifted [sinc functions](../../../../../../sinc-function.md). Critical-rate equality needs an appropriate signal class and can fail for unrestricted edge-frequency sinusoids with unknown [phase](../../../../../../phase-waves.md). Sampling fast enough prevents [aliasing](../../../../../../aliasing.md), but does not remove [thermal noise](../../../../../../thermal-noise.md). This distinction covers the source's unspecified use of “Nyquist's theorem”.[MT-002, sampled spectra and anti-aliasing discussion](../../../../../../what-the-nyquist-criterion-means-to-your-sampled-data-system-design-by-walt-kester.md)

## ↑ Ancestors (15)

1. [B](../b.md)
2. [D12](../../d12.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2012](../../../../split.md)
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
