<h1 id="18/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a real $2\pi$-periodic square-integrable [function](../../../../../function-split.md), use the [Fourier series](../../../../../fourier-series-split.md) convention

$$
f(x)\sim\frac{a_0}{2}+\sum_{n=1}^\infty[a_n\cos nx+b_n\sin nx],
$$

with [Fourier coefficients](../../../../../fourier-coefficient.md)

$$
\boxed{a_n=\frac1\pi\int_{-\pi}^{\pi}f(x)\cos nx\,dx\quad(n\geq0),\qquad
b_n=\frac1\pi\int_{-\pi}^{\pi}f(x)\sin nx\,dx\quad(n\geq1)}.
$$

The trigonometric [orthogonality](../../../../../orthogonal-vectors.md) relations are $\int_{-\pi}^{\pi}\cos nx\cos mx\,dx=\pi\delta_{nm}$ for positive $n,m$, with the same formula for sines; sine-cosine products integrate to zero. The constant has squared integral $2\pi$ and is [orthogonal](../../../../../orthogonal-vectors.md) to every positive harmonic. Thus the squared norm of the $N$th partial sum is

$$
\frac1\pi\int_{-\pi}^{\pi}f_N(x)^2\,dx
=\frac{a_0^2}{2}+\sum_{n=1}^N(a_n^2+b_n^2).
$$

Taking the limit in the [L2 space](../../../../../l2-space-is-a-hilbert-space.md) gives the Fourier-series [Parseval identity](../../../../../parseval-identity.md):

$$
\boxed{\frac1\pi\int_{-\pi}^{\pi}f(x)^2\,dx
=\frac{a_0^2}{2}+\sum_{n=1}^\infty(a_n^2+b_n^2)}.
$$

Square integrability is the natural hypothesis for this finite norm identity; additional smoothness can be used when pointwise convergence is required.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [18](../../18.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
