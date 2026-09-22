<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Fourier transform](../../../../../fourier-transform-split.md) convention

$$
\widetilde f(\omega)=\int_{-\infty}^{\infty}e^{-i\omega t}f(t)\,dt,\qquad
f(t)=\frac1{2\pi}\int_{-\infty}^{\infty}e^{i\omega t}\widetilde f(\omega)\,d\omega.
$$

The [convolution](../../../../../convolution.md) is $(f*g)(t)=\int_{-\infty}^{\infty}f(\tau)g(t-\tau)\,d\tau$. For integrable $f,g$, [Fubini's theorem](../../../../../fubini-s-theorem.md) and the substitution $s=t-\tau$ give

$$
\begin{aligned}
\widetilde{f*g}(\omega)
&=\int_{\mathbb R}\int_{\mathbb R}e^{-i\omega t}f(\tau)g(t-\tau)\,d\tau\,dt\\
&=\left(\int_{\mathbb R}e^{-i\omega\tau}f(\tau)\,d\tau\right)\left(\int_{\mathbb R}e^{-i\omega s}g(s)\,ds\right).
\end{aligned}
$$

Hence the [convolution theorem](../../../../../convolution-theorem.md) is

$$
\boxed{\widetilde{f*g}(\omega)=\widetilde f(\omega)\widetilde g(\omega).}
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
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
