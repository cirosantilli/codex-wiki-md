<h1 id="18/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [function](../../../../../function-split.md) is even, so each product with a [sine](../../../../../sine.md) is an [odd function](../../../../../odd-function.md) and all the [Fourier coefficients](../../../../../fourier-coefficient.md) $b_n$ vanish. Its constant coefficient is

$$
a_0=\frac2\pi\int_0^\pi e^x\,dx=\frac{2(e^\pi-1)}\pi.
$$

For $n\geq1$, part (a) gives the remaining [Fourier coefficients](../../../../../fourier-coefficient.md):

$$
a_n=\frac2\pi\int_0^\pi e^x\cos(nx)\,dx=\frac{2\left[(-1)^ne^\pi-1\right]}{\pi(1+n^2)}.
$$

Consequently the [Fourier cosine series](../../../../../fourier-cosine-series.md) is

$$
\boxed{f(x)=\frac{e^\pi-1}{\pi}+\frac2\pi\sum_{n=1}^{\infty}\frac{(-1)^ne^\pi-1}{1+n^2}\cos(nx).}
$$

The periodic extension is continuous, including at $\pm\pi$, and piecewise continuously differentiable. Thus the [Fourier series](../../../../../fourier-series-split.md) equals $f$ everywhere. Its coefficients are also bounded in magnitude by a constant times $1/n^2$, which gives [absolute convergence](../../../../../absolute-convergence.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [18](../../18.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
