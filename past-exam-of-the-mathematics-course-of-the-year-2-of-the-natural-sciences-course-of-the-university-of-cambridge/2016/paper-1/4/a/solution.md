<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Fourier transform](../../../../../fourier-transform-split.md) convention

$$
\widetilde f(\omega)=\int_{-\infty}^{\infty}f(t)e^{-i\omega t}\,dt,\qquad f(t)=\frac1{2\pi}\int_{-\infty}^{\infty}\widetilde f(\omega)e^{i\omega t}\,d\omega.
$$

Since $\mathcal F[e^{i\Omega t}]=2\pi\delta(\omega-\Omega)$ in [distribution theory](../../../../../distribution-theory-split.md), the carrier has transform

$$
\boxed{\widetilde c(\omega)=\pi[\delta(\omega-\Omega)+\delta(\omega+\Omega)].}
$$

The [modulation property of the Fourier transform](../../../../../modulation-property-of-the-fourier-transform.md) translates the message spectrum to the two carrier frequencies. Therefore

$$
\boxed{\widetilde\phi(\omega)=\pi[\delta(\omega-\Omega)+\delta(\omega+\Omega)]+\frac12[\widetilde s(\omega-\Omega)+\widetilde s(\omega+\Omega)].}
$$

The first term represents the unmodulated [carrier wave](../../../../../carrier-wave.md); the other terms are the [amplitude modulation sidebands](../../../../../amplitude-modulation-sidebands.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
