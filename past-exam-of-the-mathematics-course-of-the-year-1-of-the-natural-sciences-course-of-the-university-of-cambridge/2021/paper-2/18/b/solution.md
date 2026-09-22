<h1 id="18/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Evenness makes every sine coefficient zero. For the constant coefficient,

$$
a_0=\frac2L\int_0^Lx\,dx=L.
$$

An [integration by parts](../../../../../integration-by-parts.md) gives, for $n\geq1$,

$$
a_n=\frac2L\int_0^Lx\cos\frac{n\pi x}{L}dx
=\frac{2L}{n^2\pi^2}[(-1)^n-1].
$$

The even coefficients vanish and the odd coefficients are $-4L/(n^2\pi^2)$. Therefore

$$
\boxed{f(x)=\frac L2-\frac{4L}{\pi^2}
\sum_{k=0}^{\infty}\frac{\cos((2k+1)\pi x/L)}{(2k+1)^2}.}
$$

The [periodic function](../../../../../periodic-function.md) is continuous and piecewise smooth, so the [Dirichlet-Jordan convergence theorem](../../../../../dirichlet-jordan-convergence-theorem.md) identifies the [Fourier series](../../../../../fourier-series-split.md) with $f$ at every point, including the endpoints. The absolute summability of the coefficients also gives uniform convergence.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [18](../../18.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
