<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Parseval identity](../../../../../parseval-identity.md) for this [Fourier transform](../../../../../fourier-transform-split.md) convention is

$$
\boxed{\int_{\mathbb R}|h(x)|^2dx=\frac1{2\pi}\int_{\mathbb R}|\widetilde h(k)|^2dk.}
$$

Apply it to $h=g$. Its squared [norm](../../../../../norm.md) is $2\int_0^1(1-x)^2dx=2/3$, so

$$
\frac23=\frac1{2\pi}\int_{\mathbb R}\frac{16\sin^4(k/2)}{k^4}\,dk.
$$

Under $k=2x$, the last integrand times $dk$ becomes $2\sin^4x\,dx/x^4$. Consequently

$$
\boxed{\int_{-\infty}^{\infty}\frac{\sin^4x}{x^4}dx=\frac{2\pi}{3}.}
$$

The integrand has continuous value $1$ at zero and decays integrably at infinity, so this is an ordinary convergent [improper integral](../../../../../improper-integral.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
