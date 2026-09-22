<h1 id="18/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [function](../../../../../function-split.md) is odd, so its constant and [cosine](../../../../../cosine.md) coefficients are zero. Its [sine](../../../../../sine.md) coefficient is

$$
b_n=\frac2\pi I_n,\qquad I_n=\int_0^\pi(x^3-\pi^2x)\sin nx\,dx.
$$

The [polynomial](../../../../../polynomial-split.md) vanishes at both integration endpoints. Two [integrations by parts](../../../../../integration-by-parts.md) therefore give

$$
I_n=\frac1n\int_0^\pi(3x^2-\pi^2)\cos nx\,dx
=-\frac1{n^2}\int_0^\pi6x\sin nx\,dx.
$$

One more integration yields

$$
\int_0^\pi x\sin nx\,dx
=\left[-\frac{x\cos nx}{n}+\frac{\sin nx}{n^2}\right]_0^\pi
=-\frac{\pi(-1)^n}{n}.
$$

Consequently $I_n=6\pi(-1)^n/n^3$ and $b_n=12(-1)^n/n^3$. Hence

$$
\boxed{g(x)=12\sum_{n=1}^\infty\frac{(-1)^n}{n^3}\sin nx,\qquad p=3}.
$$

The periodic continuation is [continuous](../../../../../continuous-function.md) at $\pm\pi$, where its values are zero, so the series represents it there as well as in the open interval.

## ↑ Ancestors (13)

1. [B](../b.md)
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
