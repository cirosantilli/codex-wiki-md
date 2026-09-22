<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [triangular function](../../../../../triangular-function.md) is real and even, so its [Fourier transform](../../../../../fourier-transform-split.md) reduces to a cosine integral:

$$
\widetilde f(k)=2\int_0^1(1-x)\cos(kx)dx.
$$

For $k\ne0$, one [integration by parts](../../../../../integration-by-parts.md) gives $\int_0^1(1-x)\cos(kx)dx=(1-\cos k)/k^2$. Therefore the [Fourier transform of a triangular function](../../../../../fourier-transform-of-a-triangular-function.md) is

$$
\boxed{\widetilde f(k)=\frac{2(1-\cos k)}{k^2}=\left(\frac{\sin(k/2)}{k/2}\right)^2,\qquad\widetilde f(0)=1.}
$$

The zero-frequency value is the removable limit and also the area of the triangle. The transform is a [squared sinc function](../../../../../squared-sinc-function.md), which explains its nonnegativity despite the oscillating Fourier exponential.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
