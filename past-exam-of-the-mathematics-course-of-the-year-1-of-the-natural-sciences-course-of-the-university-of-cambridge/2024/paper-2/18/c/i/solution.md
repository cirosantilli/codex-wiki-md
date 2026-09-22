<h1 id="18/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [function](../../../../../../function-split.md) is an [odd function](../../../../../../odd-function.md), so $a_0=a_n=0$. Here $L=1$, and the [Fourier coefficients](../../../../../../fourier-coefficient.md) are

$$
b_n=2\int_0^1x(1-x)\sin(n\pi x)\,dx.
$$

Write $k=n\pi$. One [integration by parts](../../../../../../integration-by-parts.md) has zero endpoint terms because $x(1-x)$ vanishes at both endpoints:

$$
b_n=\frac2k\int_0^1(1-2x)\cos(kx)\,dx.
$$

A second [integration by parts](../../../../../../integration-by-parts.md) gives

$$
\int_0^1(1-2x)\cos(kx)\,dx
=\frac2k\int_0^1\sin(kx)\,dx
=\frac{2(1-\cos k)}{k^2}.
$$

Therefore $b_n=4(1-(-1)^n)/(n^3\pi^3)$, zero for even $n$ and $8/(n^3\pi^3)$ for odd $n$. The [Fourier series](../../../../../../fourier-series-split.md) is

$$
\boxed{f(x)=\frac8{\pi^3}\sum_{m=0}^\infty\frac{\sin((2m+1)\pi x)}{(2m+1)^3}}.
$$

The coefficients are absolutely summable, and the periodic [function](../../../../../../function-split.md) is continuous even at the joins $x=\pm1$, so the displayed [Fourier series](../../../../../../fourier-series-split.md) represents it everywhere.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [C](../../c.md)
3. [18](../../../18.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
