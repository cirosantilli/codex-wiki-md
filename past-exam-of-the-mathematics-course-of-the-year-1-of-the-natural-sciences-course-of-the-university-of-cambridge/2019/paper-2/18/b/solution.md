<h1 id="18/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

On the open interval, $g=f'$. It is an [odd function](../../../../../odd-function.md) there, so its constant and cosine coefficients vanish; assigned values at the endpoints do not affect these [integrals](../../../../../integral-split.md). For its sine coefficient, [integration by parts](../../../../../integration-by-parts.md) gives

$$
b_n^{(g)}=\int_{-1}^1 f'(x)\sin(n\pi x)\,dx
=\left[f(x)\sin(n\pi x)\right]_{-1}^1-n\pi\int_{-1}^1 f(x)\cos(n\pi x)\,dx
=-n\pi a_n.
$$

Consequently

$$
\boxed{g(x)=2\pi\sinh1\sum_{n=1}^{\infty}\frac{(-1)^{n+1}n\sin(n\pi x)}{1+n^2\pi^2}},\qquad -1<x<1.
$$

The endpoint qualification matters. The periodic $g$ has a [jump discontinuity](../../../../../jump-discontinuity.md) at every odd integer, with one-sided limits $\pm\sinh1$. By the [Dirichlet-Jordan convergence theorem](../../../../../dirichlet-jordan-convergence-theorem.md), the [Fourier series](../../../../../fourier-series-split.md) converges to their average, zero, there, not to the assigned value $g(1)=\sinh1$. The [integration by parts](../../../../../integration-by-parts.md) argument also avoids assuming unrestricted termwise differentiation of the first series.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [18](../../18.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
