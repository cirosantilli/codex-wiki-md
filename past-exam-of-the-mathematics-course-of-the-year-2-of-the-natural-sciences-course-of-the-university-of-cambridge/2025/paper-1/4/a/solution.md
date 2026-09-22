<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume first that $f$ and $g$ are [integrable functions](../../../../../lebesgue-integrable-function.md), so that [Fubini's theorem](../../../../../fubini-s-theorem.md) justifies changing the order of the two [integrals](../../../../../integral-split.md). In the defining [Fourier transform](../../../../../fourier-transform-split.md) of the [convolution](../../../../../convolution.md), put $y=x-x'$:

$$
\begin{aligned}
\widetilde h(k)
&=\int_{\mathbb R}\int_{\mathbb R}e^{-ikx}f(x-x')g(x')\,dx'\,dx\\
&=\int_{\mathbb R}\int_{\mathbb R}e^{-ik(y+x')}f(y)g(x')\,dy\,dx'\\
&=\left(\int_{\mathbb R}e^{-iky}f(y)\,dy\right)\left(\int_{\mathbb R}e^{-ikx'}g(x')\,dx'\right).
\end{aligned}
$$

This proves the [convolution theorem](../../../../../convolution-theorem.md) with the stated normalization:

$$
\boxed{\widetilde h(k)=\widetilde f(k)\widetilde g(k).}
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
