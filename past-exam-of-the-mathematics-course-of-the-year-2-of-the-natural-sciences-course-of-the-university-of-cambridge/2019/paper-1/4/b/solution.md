<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume initially that $f,g$ are integrable, so [Fubini's theorem](../../../../../fubini-s-theorem.md) justifies interchanging the integrals. Transform the [convolution](../../../../../convolution.md) and put $u=x-z$:

$$
\begin{aligned}
\widetilde h(k)&=\int_{\mathbb R}\!\int_{\mathbb R}f(z)g(x-z)e^{-ikx}\,dz\,dx\\
&=\int_{\mathbb R}f(z)e^{-ikz}\,dz\int_{\mathbb R}g(u)e^{-iku}\,du\\
&=\boxed{\widetilde f(k)\widetilde g(k)}.
\end{aligned}
$$

This is the [convolution theorem](../../../../../convolution-theorem.md). No factor $2\pi$ appears in this direction because the forward transform in the question is unnormalized.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
