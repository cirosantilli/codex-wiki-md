<h1 id="section-b/b6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The precise [bandwidth](../../../../../../bandwidth-signal-processing.md) depends on the output: this is the distinction between [displacement and current bandwidths of a series RLC circuit](../../../../../../displacement-and-current-bandwidths-of-a-series-rlc-circuit.md). For current output, or voltage across the [resistor](../../../../../../resistor.md), the [electrical impedance](../../../../../../electrical-impedance.md) gives

$$
|i|^2=\frac{|V_0|^2}{R^2+(\omega L-1/(\omega C))^2}.
$$

The half-power points satisfy $|\omega L-1/(\omega C)|=R$. Their positive roots are

$$
\omega_\pm=\frac{\sqrt{R^2+4L/C}\pm R}{2L},\qquad
\boxed{\Delta\omega=\omega_+-\omega_-=R/L},\qquad
\boxed{\Delta f=R/(2\pi L)}.
$$

Changing [capacitance](../../../../../../capacitance.md) shifts the centre without changing this absolute width. For the charge response in part (d), the exact half-height points instead obey

$$
\omega_\pm^2=\omega_0^2-\gamma^2/2\pm\gamma\sqrt{\omega_0^2-\gamma^2/4};
$$

when both exist their separation only approaches $\gamma=R/L$ at large [quality factor](../../../../../../q-factor.md). Therefore the printed capacitance-independence claim is exact for current or resistor-voltage output and an approximation for the preceding charge resonance.

For a narrow [band-pass filter](../../../../../../band-pass-filter.md), use current or resistor-voltage output and make $R/L$ small, counting source, load and inductor losses in the total [electrical resistance](../../../../../../electrical-resistance.md). Increase $Q=\sqrt{L/C}/R$; if a specified centre [frequency](../../../../../../frequency.md) is to remain fixed, adjust $C$ with $L$ to keep $LC$ fixed. Capacitor-voltage output alone is not a band-pass response because it has a nonzero DC limit.

## ↑ Ancestors (15)

1. [E](../e.md)
2. [B6](../../b6.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2018](../../../../split.md)
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
