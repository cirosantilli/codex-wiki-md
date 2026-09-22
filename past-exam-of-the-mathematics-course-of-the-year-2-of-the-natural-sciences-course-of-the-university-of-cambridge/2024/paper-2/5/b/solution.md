<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take the causal solution, extending the input and output by zero before the device starts at $t=0$. The two zero [initial conditions](../../../../../initial-condition.md) ensure that this extension adds no impulsive terms to the first two [distributional derivatives](../../../../../distributional-derivative.md). The [Fourier transform of a derivative](../../../../../fourier-transform-of-a-derivative.md) is multiplication by $i\omega$, so

$$
\left[(p+i\omega)^2+q^2\right]\widetilde\phi(\omega)=\widetilde I(\omega).
$$

Factoring the quadratic and taking [partial fraction decomposition](../../../../../partial-fraction-decomposition.md) yields

$$
\boxed{\widetilde\phi=\widetilde R\widetilde I,\qquad
\widetilde R(\omega)=\frac1{2iq}\left(\frac1{p+i\omega-iq}-\frac1{p+i\omega+iq}\right).}
$$

The inverse [Fourier transform](../../../../../fourier-transform-split.md) follows directly by integrating decaying exponentials:

$$
\boxed{R(t)=H(t)\frac{e^{-pt}\sin(qt)}q,}
$$

where $H$ is the [Heaviside step function](../../../../../heaviside-step-function.md). This [damped-oscillator impulse response](../../../../../causal-green-function-of-a-damped-oscillator.md) has $R(0^+)=0$ and $R'(0^+)=1$, as required for a unit impulse.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
