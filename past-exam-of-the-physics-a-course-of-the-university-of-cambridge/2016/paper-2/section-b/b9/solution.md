<h1 id="section-b/b9/solution">Solution</h1>

↑ **Parent:** [B9](../b9.md)

Let the first transmitted [complex amplitude](../../../../../complex-amplitude.md) be $T E_{\rm in}e^{ikd}$: two amplitude transmission factors each of magnitude $\sqrt T$ give magnitude $T$. Each extra internal round trip adds two amplitude [reflections](../../../../../reflection-mathematics.md), with combined magnitude $R$, and phase $\delta$. With the [mirror](../../../../../mirror.md) phase convention already incorporated in the stipulated $\delta$,

$$
E_{\rm out}=TE_{\rm in}e^{ikd}\sum_{j=0}^{\infty}(Re^{i\delta})^j
=\frac{TE_{\rm in}e^{ikd}}{1-Re^{i\delta}}.
$$

Taking the squared modulus gives

$$
\boxed{B=\frac{T^2}{1+R^2-2R\cos\delta}.}
$$

It is $R$, not $R^2$, that multiplies the field after a round trip; $R^2$ would be the corresponding round-trip intensity fraction.

At resonance $\delta=2m\pi$, $B_{\max}=T^2/(1-R)^2$. If $h$ is the positive phase [displacement](../../../../../displacement.md) to half maximum,

$$
\sin(h/2)=\frac{1-R}{2\sqrt R},\qquad
h=2\arcsin\frac{1-R}{2\sqrt R}
\simeq\frac{1-R}{\sqrt R}.
$$

For $R=0.80$, **the stipulated high-reflectivity approximation gives $h=0.2236\ {\rm rad}$**, while the exact value is $0.2241\ {\rm rad}$. The full width is twice this value. With $T=0.20$, $B_{\max}=1$, $B_{\min}=T^2/(1+R)^2=1/81$ and the pattern repeats every $2\pi$. Its ideal [finesse](../../../../../finesse.md) is approximately $\pi\sqrt R/(1-R)=14.05$.

A [wavelength](../../../../../wavelength.md) component resonates at $d=m\lambda/2$. Within the scan interval, the individual resonances are

$$
\boxed{
\begin{array}{c|c|c}
\lambda\ ({\rm nm})&m&d\ ({\rm mm})\\
1000.0&1000&0.500000\\
1000.2&1000&0.500100
\end{array}}
$$

No neighboring orders of these lines fall within the stated interval. The observed signal is the sum of their two Airy transmissions, since different spectral components add intensities. Individual resonance positions identify the two peaks to the plotted precision; the tails cause very small shifts of the maxima of the sum.

The gap-coordinate full width is

$$
\Delta d_{\rm FWHM}=\frac{\lambda h}{2\pi}\simeq0.0357\ \mu{\rm m}.
$$

The separation is $0.100\ \mu{\rm m}$, about $2.8$ full widths, so **the two components can be resolved by the ideal etalon**. The equivalent [wavelength](../../../../../wavelength.md) resolution near order $1000$ is about $\lambda/(m\mathcal F)\simeq0.071\ {\rm nm}$, smaller than their $0.2\ {\rm nm}$ separation.

The added [wavelength](../../../../../wavelength.md) has an order-$999$ resonance at

$$
\boxed{d=\frac{999(1001.1\ {\rm nm})}{2}
=0.50004945\ {\rm mm}.}
$$

It lies between the preceding two peaks; its adjacent orders are outside the scan. Its input strength was not specified, so the third peak's height cannot be uniquely assigned. The original plot uses equal strength only as a declared illustration.

This is an order-identification problem: the [free spectral range](../../../../../free-spectral-range.md) near $d=0.5\ {\rm mm}$ is $\Delta\lambda_{\rm FSR}\simeq\lambda^2/(2d)\simeq1\ {\rm nm}$. A line more than one [free spectral range](../../../../../free-spectral-range.md) away can appear among peaks of another order. A lower-resolution prefilter or additional dispersive spectrometer is needed to identify the order; a narrow peak alone does not identify an absolute [wavelength](../../../../../wavelength.md). [mirror](../../../../../mirror.md) parallelism, beam collimation and detector angular acceptance must also be controlled before attributing a measured width entirely to reflectivity.[pp.2–5, instrument finesse and free spectral range; central-spot scanning discussion](../../../../../fabry-perot-interferometer-university-of-washington-physics-331.md)

## ↑ Ancestors (14)

1. [B9](../b9.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2016](../../../split.md)
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
