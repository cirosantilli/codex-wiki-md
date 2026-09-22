<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First take $f,g\in L^1(\mathbb R)$, so [Fubini's theorem](../../../../../fubini-s-theorem.md) applies to the [cross-correlation](../../../../../cross-correlation.md) double integral. With $s=x+y$, the [Fourier transform](../../../../../fourier-transform-split.md) is

$$
\begin{aligned}
\widehat h(k)&=\int_{\mathbb R}\int_{\mathbb R}e^{-ikx}\overline{f(y)}g(x+y)\,dy\,dx\\
&=\left[\int_{\mathbb R}\overline{f(y)}e^{iky}\,dy\right]\left[\int_{\mathbb R}g(s)e^{-iks}\,ds\right]\\
&=\boxed{\overline{\widehat f(k)}\,\widehat g(k)}.
\end{aligned}
$$

The [complex conjugation](../../../../../complex-conjugation.md) and the sign in $x+y$ are both essential to this convention.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
