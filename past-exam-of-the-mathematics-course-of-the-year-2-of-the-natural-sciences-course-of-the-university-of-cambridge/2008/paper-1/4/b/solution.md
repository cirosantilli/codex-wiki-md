<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the chosen [Fourier transform](../../../../../fourier-transform-split.md) convention, [Parseval's identity](../../../../../parseval-identity.md) is $\int|f|^2dx=(2\pi)^{-1}\int|\widetilde f|^2dk$. For smooth rapidly decaying functions its bilinear form follows by inserting the inverse transform of $g$ into $\int f\overline g\,dx$ and interchanging the integrals:

$$
\int f(x)\overline{g(x)}dx=\frac1{2\pi}\int\widetilde f(k)\overline{\widetilde g(k)}dk.
$$

Take $g=f$. Approximation by such functions extends the identity to [L2 space](../../../../../l2-space-is-a-hilbert-space.md), which includes the compact triangular function here.

For that triangle, $\int|f|^2dx=2\int_0^1(1-x)^2dx=2/3$, while $\widetilde f(k)=[\sin(k/2)/(k/2)]^2$. Thus

$$
\frac23=\frac1{2\pi}\int_{-\infty}^{\infty}\left(\frac{\sin(k/2)}{k/2}\right)^4dk
=\frac2\pi\int_0^\infty\left(\frac{\sin u}u\right)^4du,
$$

giving

$$
\boxed{\int_0^\infty\frac{\sin^4u}{u^4}du=\frac\pi3.}
$$

The continuous limiting integrand at zero is one. This is the [sinc fourth-power integral](../../../../../sinc-fourth-power-integral.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
