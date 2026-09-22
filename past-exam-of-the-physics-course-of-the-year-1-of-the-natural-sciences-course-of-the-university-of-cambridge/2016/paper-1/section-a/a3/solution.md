<h1 id="section-a/a3/solution">Solution</h1>

↑ **Parent:** [A3](../a3.md)

Use an [RC low-pass filter](../../../../../rc-low-pass-filter.md): put the [resistor](../../../../../resistor.md) in series with the input and the [capacitor](../../../../../capacitor.md) between the output node and the return conductor. Measure the output [voltage](../../../../../voltage.md) across the [capacitor](../../../../../capacitor.md), with negligible output loading. The [voltage divider](../../../../../voltage-divider.md) then has [transfer function](../../../../../transfer-function.md)

$$
H(\omega)=\frac{1/(i\omega C)}{R+1/(i\omega C)}=\frac1{1+i\omega RC},\qquad |H|=\frac1{\sqrt{1+(\omega RC)^2}}.
$$

At the high [frequency](../../../../../frequency.md), the attenuation requirement is

$$
2\pi f_hRC>\sqrt{500^2-1},\qquad C>\frac{\sqrt{500^2-1}}{2\pi(20000)(330)}\simeq12.1\ \mu\mathrm F.
$$

At the low [frequency](../../../../../frequency.md), approximately unchanged [amplitude](../../../../../wave-amplitude.md) means $2\pi f_lRC\ll1$, so

$$
\boxed{12.1\ \mu\mathrm F<C\ll482\ \mu\mathrm F.}
$$

The upper relation is an asymptotic design condition, because “approximately” specifies no numerical tolerance. For example, retaining at least $99\%$ of the low-[frequency](../../../../../frequency.md) [amplitude](../../../../../wave-amplitude.md) would sharpen the upper bound to approximately $68.7\ \mu\mathrm F$.

**A practical illustrative choice is $C=22\ \mu\mathrm F$.** Its [voltage gain](../../../../../voltage-gain.md) is approximately $0.99896$ at $1\ \mathrm{Hz}$ and $0.001096$ at $20\ \mathrm{kHz}$: the latter [amplitude](../../../../../wave-amplitude.md) is reduced by a factor of about $912$. Its [cutoff frequency](../../../../../cutoff-frequency.md) is $1/(2\pi RC)\simeq21.9\ \mathrm{Hz}$.

<a id="section-a/a3/image-an-original-rc-low-pass-circuit-and-its-amplitude-response-for-a-22-microfarad-capacitor"></a>
![](../../../../../past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1-low-pass.png)

**[Figure 1](#section-a/a3/image-an-original-rc-low-pass-circuit-and-its-amplitude-response-for-a-22-microfarad-capacitor). An original RC low-pass circuit and its amplitude response for a 22 microfarad capacitor**.

## ↑ Ancestors (13)

1. [A3](../a3.md)
2. [Section A](../../section-a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
