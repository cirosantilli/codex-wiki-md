<h1 id="section-d/d13/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [lock-in amplifier](../../../../../../lock-in-amplifier.md) multiplies the measured [signal](../../../../../../signal.md) by a synchronized reference and [low-pass filters](../../../../../../low-pass-filter.md) the product. For $s(t)=A\cos(\omega t+\phi)+n(t)$ and reference $2\cos\omega t$, the [signal](../../../../../../signal.md) product is $A\cos\phi+A\cos(2\omega t+\phi)$. Averaging away the second harmonic gives $X=A\cos\phi$ in this peak-amplitude convention. A second reference $-2\sin\omega t$ gives $Y=A\sin\phi$, so

$$
\boxed{A=\sqrt{X^2+Y^2},\qquad\phi=\operatorname{atan2}(Y,X).}
$$

A single quadrature could read zero for a substantial [signal](../../../../../../signal.md) $90^\circ$ from its reference. Two quadratures avoid that blind spot; the phase is undefined at zero [amplitude](../../../../../../wave-amplitude.md). Instrument RMS calibrations can include a different constant normalization.

The reference shifts the wanted [frequency](../../../../../../frequency.md) to zero, where a narrow low-pass [bandwidth](../../../../../../bandwidth-signal-processing.md) can select it. Uncorrelated broadband [noise](../../../../../../noise-signal-processing.md) averages down, whereas a simple amplifier would enlarge [signal](../../../../../../signal.md) and [noise](../../../../../../noise-signal-processing.md) together. Longer averaging improves narrow-band sensitivity but slows the response to changing [amplitude](../../../../../../wave-amplitude.md). The [signal](../../../../../../signal.md) must remain phase coherent with the reference; [frequency](../../../../../../frequency.md) mismatch creates a beat instead of a constant output. [interference](../../../../../../interference-wave-propagation.md) at the same reference [frequency](../../../../../../frequency.md) survives, so shielding and independent background measurements remain necessary.[printed pp.3-1–3-3, multiplication, dual-phase detection and RMS-versus-peak conventions](../../../../../../model-sr830-dsp-lock-in-amplifier-manual-by-stanford-research-systems.md)

## ↑ Ancestors (15)

1. [B](../b.md)
2. [D13](../../d13.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2014](../../../../split.md)
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
