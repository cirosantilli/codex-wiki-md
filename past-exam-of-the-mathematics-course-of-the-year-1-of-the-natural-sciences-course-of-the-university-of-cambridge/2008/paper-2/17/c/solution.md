<h1 id="17/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The periodic ramp is an [odd function](../../../../../odd-function.md), so $a_0=a_n=0$. [Integration by parts](../../../../../integration-by-parts.md) gives

$$
b_n=\frac2\pi\int_0^\pi x\sin(nx)\,dx=\frac{2(-1)^{n+1}}n.
$$

Thus the [Fourier series of a periodic sawtooth](../../../../../fourier-series-of-a-periodic-sawtooth.md) is

$$
\boxed{x=2\sum_{n=1}^{\infty}\frac{(-1)^{n+1}}n\sin(nx),\qquad-\pi<x<\pi.}
$$

The periodic function is smooth at $x=\pi/2$, so the [Dirichlet-Jordan convergence theorem](../../../../../dirichlet-jordan-convergence-theorem.md) permits evaluation there. Even-index terms vanish and odd-index sines alternate in sign, giving

$$
\boxed{1-\frac13+\frac15-\frac17+\cdots=\frac\pi4.}
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [17](../../17.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
