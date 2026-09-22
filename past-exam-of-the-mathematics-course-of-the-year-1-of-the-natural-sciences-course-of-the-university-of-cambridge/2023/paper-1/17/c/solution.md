<h1 id="17/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $L=1$, the [even function](../../../../../even-function.md) $h(x)=x^2$ has $b_n=0$, because $x^2\sin(n\pi x)$ is an [odd function](../../../../../odd-function.md). Its constant coefficient is $a_0=\int_{-1}^1x^2dx=2/3$. The remaining [Fourier coefficients](../../../../../fourier-coefficient.md) are

$$
a_n=2\int_0^1x^2\cos(n\pi x)\,dx.
$$

Two applications of [integration by parts](../../../../../integration-by-parts.md) give the [antiderivative](../../../../../antiderivative.md), with $k=n\pi$,

$$
\frac{x^2\sin(kx)}k+\frac{2x\cos(kx)}{k^2}-\frac{2\sin(kx)}{k^3}.
$$

Its endpoint difference is $2(-1)^n/(n\pi)^2$, so $a_n=4(-1)^n/(n^2\pi^2)$. Therefore

$$
\boxed{x^2=\frac13+\frac4{\pi^2}\sum_{n=1}^{\infty}\frac{(-1)^n}{n^2}\cos(n\pi x),\qquad-1\leq x\leq1.}
$$

The periodic extension is continuous and piecewise smooth, so [pointwise convergence of a piecewise smooth Fourier series](../../../../../pointwise-convergence-of-a-piecewise-smooth-fourier-series.md) gives equality, including at the endpoints.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [17](../../17.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
