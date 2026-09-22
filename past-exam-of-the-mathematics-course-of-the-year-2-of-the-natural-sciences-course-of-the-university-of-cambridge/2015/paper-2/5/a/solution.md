<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Fourier transform](../../../../../fourier-transform-split.md) convention $\widetilde y(\omega)=\int_{\mathbb R}y(t)e^{-i\omega t}dt$. For a transformable response with the necessary boundary terms vanishing, [integration by parts](../../../../../integration-by-parts.md) gives

$$
\widetilde{\dot y}=i\omega\widetilde y,\qquad\widetilde{\ddot y}=-\omega^2\widetilde y.
$$

Transforming the differential equation therefore gives $(5-\omega^2+2i\omega)\widetilde y=\widetilde f$, so

$$
\boxed{\widetilde y(\omega)=\frac{-\widetilde f(\omega)}{\omega^2-2i\omega-5}.}
$$

The identities also hold for [tempered distributions](../../../../../tempered-distribution.md). The denominator factors as $(\omega-i-2)(\omega-i+2)$; its two poles are in the upper half-plane, corresponding under inverse factor $e^{i\omega t}$ to the [causal Green function of a damped oscillator](../../../../../causal-green-function-of-a-damped-oscillator.md).

The frequency-domain formula selects the Fourier-transformable response. Decay of the force alone would not remove arbitrary homogeneous solutions, which grow towards negative time and do not have an ordinary bilateral Fourier transform.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
