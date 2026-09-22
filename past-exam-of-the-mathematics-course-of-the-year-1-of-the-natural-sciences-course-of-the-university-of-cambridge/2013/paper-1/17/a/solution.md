<h1 id="17/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With the standard real normalization, the [Fourier series](../../../../../fourier-series-split.md) of a period-$2L$ [function](../../../../../function-split.md) is

$$
f(x)\sim\frac{a_0}{2}+\sum_{n=1}^{\infty}\left[a_n\cos\frac{n\pi x}{L}+b_n\sin\frac{n\pi x}{L}\right],
$$

where

$$
\boxed{a_n=\frac1L\int_{-L}^Lf(x)\cos\frac{n\pi x}{L}\,dx\quad(n\geq0),\qquad
b_n=\frac1L\int_{-L}^Lf(x)\sin\frac{n\pi x}{L}\,dx\quad(n\geq1).}
$$

For the [partial sum](../../../../../partial-sum.md) $S_N$, [Fourier orthogonality](../../../../../fourier-orthogonality.md) eliminates all cross terms. The constant term contributes $2L(a_0/2)^2$, while every squared [sine](../../../../../sine.md) or [cosine](../../../../../cosine.md) integrates to $L$, giving

$$
\int_{-L}^LS_N(x)^2dx=L\frac{a_0^2}{2}+L\sum_{n=1}^N(a_n^2+b_n^2).
$$

For a square-integrable [function](../../../../../function-split.md), completeness of the trigonometric [orthogonal basis](../../../../../orthogonal-basis.md) in the [Hilbert space](../../../../../hilbert-space-split.md) $L^2[-L,L]$ makes $S_N\to f$ in norm. Passing to the limit proves [Parseval's identity](../../../../../parseval-identity.md):

$$
\boxed{\int_{-L}^Lf(x)^2dx=L\left[\frac{a_0^2}{2}
+\sum_{n=1}^{\infty}(a_n^2+b_n^2)\right].}
$$

Square integrability is the needed hypothesis here; periodicity alone is not an integrability or convergence condition.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [17](../../17.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
