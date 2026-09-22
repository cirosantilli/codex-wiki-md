<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [trigonometric identity](../../../../../trigonometric-identity.md) $2\cos^2(ax)=1+\cos(2ax)$ and express the cosine as a sum of two [complex exponentials](../../../../../complex-exponential-function.md). The [Fourier transform](../../../../../fourier-transform-split.md) of each exponential is a shifted [Dirac delta distribution](../../../../../dirac-delta-function.md):

$$
\mathcal F[1]=2\pi\delta(k),\qquad\mathcal F[e^{\pm2iax}]=2\pi\delta(k\mp2a).
$$

By [linearity](../../../../../linearity.md),

$$
\boxed{\widetilde f(k)=2\pi\delta(k)+\pi\delta(k-2a)+\pi\delta(k+2a).}
$$

The original function does not decay and is not absolutely integrable on the real line, so this answer is a [tempered distribution](../../../../../tempered-distribution.md), rather than an ordinary convergent Fourier integral. Its three lines represent the constant part and the two opposite spatial [frequencies](../../../../../frequency.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
