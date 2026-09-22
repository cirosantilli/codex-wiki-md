<h1 id="15/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the real [Fourier series](../../../../../fourier-series-split.md) convention $g=a_0/2+\sum_{n\geq1}[a_n\cos(n\pi x)+b_n\sin(n\pi x)]$ for period two. Since $g$ is an [even function](../../../../../even-function.md), $b_n=0$, and $a_0=\int_{-1}^1x^2dx=2/3$. Twice applying [integration by parts](../../../../../integration-by-parts.md), with $k=n\pi$, gives

$$
a_n=2\int_0^1x^2\cos(kx)dx
=2\left[\frac{x^2\sin(kx)}k+\frac{2x\cos(kx)}{k^2}-\frac{2\sin(kx)}{k^3}\right]_0^1
=\frac{4(-1)^n}{\pi^2n^2}.
$$

Hence

$$
\boxed{g(x)=\frac13+\frac4{\pi^2}\sum_{n=1}^\infty\frac{(-1)^n}{n^2}\cos(n\pi x).}
$$

The periodic extension is continuous at its endpoints, so the series takes the specified endpoint values as well as the interior values.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [15](../../15.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
