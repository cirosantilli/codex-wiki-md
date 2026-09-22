<h1 id="15/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Again the function is even, so all sine coefficients vanish. Its constant term is $a_0/2=\sinh1$. With $k=n\pi$, an [antiderivative](../../../../../antiderivative.md) is

$$
\int\cosh x\cos(kx)dx=\frac{\sinh x\cos(kx)+k\cosh x\sin(kx)}{1+k^2}.
$$

Thus $a_n=2(-1)^n\sinh1/(1+n^2\pi^2)$. In the requested factored notation,

$$
\boxed{A_0=1,\qquad A_n(x)=\frac{2(-1)^n\cos(n\pi x)}{1+n^2\pi^2}.}
$$

This is the period-two specialization of the [Fourier series of periodic hyperbolic sine and cosine](../../../../../fourier-series-of-periodic-hyperbolic-sine-and-cosine.md). The function values match at the endpoints, although its derivative has a jump in the periodic extension.

## ↑ Ancestors (13)

1. [C](../c.md)
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
