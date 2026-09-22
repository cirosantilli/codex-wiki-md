<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The filter is a real even [triangular function](../../../../../triangular-function.md). Its [Fourier transform](../../../../../fourier-transform-split.md) is

$$
\widetilde f(\omega)=2\int_0^1(1-t)\cos(\omega t)\,dt=\boxed{\frac{2(1-\cos\omega)}{\omega^2}=\left[\frac{\sin(\omega/2)}{\omega/2}\right]^2},
$$

with $\widetilde f(0)=1$. Since the transmitted pulse is the [convolution](../../../../../convolution.md) $b=a*f$, the [convolution theorem](../../../../../convolution-theorem.md) gives

$$
\boxed{\widetilde b(\omega)=\widetilde a(\omega)\widetilde f(\omega)=\frac{4\sin\omega(1-\cos\omega)}{\omega^3},\qquad\widetilde b(0)=2.}
$$

The normalized filter preserves the time [integral](../../../../../integral-split.md) of the pulse, while its extra inverse-frequency factors suppress high-frequency content. It is a smoothing filter rather than an exact compact-bandwidth cutoff.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
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
