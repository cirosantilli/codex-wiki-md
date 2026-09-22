<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The half-open intervals $[-\pi+2\pi k,\pi+2\pi k)$ tile the line, so exactly one term contributes to $\sum_k|f(t+2\pi k)|^2$. It equals one almost everywhere.

Choose the [Shannon scaling mask](../../../../../../shannon-scaling-mask.md), a $2\pi$-periodic [low-pass filter of a multiresolution analysis](../../../../../../low-pass-filter-of-a-multiresolution-analysis.md) which equals one on $[-\pi/2,\pi/2)$ and zero on the rest of $[-\pi,\pi)$. On the support of $f$ its product with $f(t)$ equals $f(2t)$; outside that support both sides vanish. Its [Fourier coefficients](../../../../../../fourier-coefficient.md) give

$$
a_0=1,\qquad a_n=\frac{2\sin(n\pi/2)}{\pi n}\quad(n\ne0),
$$

so it also has the required symbol representation. The inverse [Fourier transform](../../../../../../fourier-transform.md) gives **the [Shannon scaling function](../../../../../../shannon-scaling-function.md)**

$$
\boxed{\phi(x)=\frac1{2\pi}\int_{-\pi}^{\pi}e^{ixt}\,dt
=\frac{\sin(\pi x)}{\pi x},\qquad\phi(0)=1.}
$$

This [sinc function](../../../../../../sinc-function.md) has $L^2$ norm one. It illustrates why the [Fourier transform](../../../../../../fourier-transform.md) convention in part B must allow $L^2$ transforms: the [Shannon scaling function](../../../../../../shannon-scaling-function.md) is not absolutely integrable on the line.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
