<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Insert the inverse [Fourier transforms](../../../../../fourier-transform-split.md) of $f$ and its complex conjugate, initially under enough decay to justify interchanging [integrals](../../../../../integral-split.md):

$$
\begin{aligned}
\int_{\mathbb R}|f(x)|^2\,dx
&=\frac1{(2\pi)^2}\int_{\mathbb R}\int_{\mathbb R}\widetilde f(k)\overline{\widetilde f(\ell)}\left[\int_{\mathbb R}e^{i(k-\ell)x}\,dx\right]dk\,d\ell\\
&=\frac1{2\pi}\int_{\mathbb R}\int_{\mathbb R}\widetilde f(k)\overline{\widetilde f(\ell)}\delta(k-\ell)\,dk\,d\ell\\
&=\boxed{\frac1{2\pi}\int_{\mathbb R}|\widetilde f(k)|^2\,dk}.
\end{aligned}
$$

The middle step uses the stated [Dirac delta distribution](../../../../../dirac-delta-function.md) identity, and the last uses its sampling property. This is the [Parseval identity](../../../../../parseval-identity.md) for the chosen normalization. Approximation extends the result to [square-integrable functions](../../../../../square-integrable-function.md), including the function used below.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
