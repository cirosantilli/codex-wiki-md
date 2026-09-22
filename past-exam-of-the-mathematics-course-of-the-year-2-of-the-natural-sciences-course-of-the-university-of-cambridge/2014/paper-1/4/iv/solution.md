<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For sufficiently rapidly decaying functions, substitute the [inverse Fourier transform](../../../../../inverse-fourier-transform.md) of $g$ and interchange the [integrals](../../../../../integral-split.md):

$$
\begin{aligned}
\int_{-\infty}^{\infty}f(x)^*g(x)\,dx&=\frac1{2\pi}\int_{-\infty}^{\infty}\widetilde g(k)\left[\int_{-\infty}^{\infty}f(x)^*e^{ikx}\,dx\right]dk\\
&=\boxed{\frac1{2\pi}\int_{-\infty}^{\infty}\widetilde f(k)^*\widetilde g(k)\,dk.}
\end{aligned}
$$

The bracketed [integral](../../../../../integral-split.md) is the [complex conjugate](../../../../../complex-conjugate.md) of $\widetilde f(k)$. This is [Parseval's identity](../../../../../parseval-identity.md) for the chosen normalization. One may first prove it for [Schwartz functions](../../../../../schwartz-function.md), where the interchanges are justified, and then extend it to $L^2$ by the [Plancherel theorem](../../../../../plancherel-theorem.md).

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
