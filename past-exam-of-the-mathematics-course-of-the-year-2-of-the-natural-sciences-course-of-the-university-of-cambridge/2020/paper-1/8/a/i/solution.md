<h1 id="8/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

With the stated [Fourier transform](../../../../../../fourier-transform-split.md) convention, [integration by parts](../../../../../../integration-by-parts.md) gives

$$
\widetilde{f'}(\omega)=\int_{-\infty}^\infty f'(t)e^{-i\omega t}\,dt
=\left[f(t)e^{-i\omega t}\right]_{-\infty}^{\infty}
+i\omega\int_{-\infty}^\infty f(t)e^{-i\omega t}\,dt.
$$

The boundary term vanishes, so

$$
\boxed{\widetilde{f'}(\omega)=i\omega\widetilde f(\omega).}
$$

For an [absolutely continuous function](../../../../../../absolutely-continuous-function.md), this calculation requires enough integrability to justify the displayed operations. Under the paper's broader bounded-variation hypothesis, the general identity is the [Fourier transform of a derivative](../../../../../../fourier-transform-of-a-derivative.md) interpreted distributionally: the [derivative](../../../../../../derivative.md) measure includes [Dirac delta functions](../../../../../../dirac-delta-function.md) at jumps and any singular continuous part. If one instead differentiates only the smooth pieces and discards jumps, the formula needs the corresponding jump corrections. Absolute integrability and [bounded variation](../../../../../../total-variation-of-a-function.md) ensure the limits of $f$ at both infinities are zero, but do not by themselves make its ordinary [derivative](../../../../../../derivative.md) capture those singular parts.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [8](../../../8.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
