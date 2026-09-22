<h1 id="18/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the period-two [Fourier series](../../../../../fourier-series-split.md) of a [square-integrable function](../../../../../square-integrable-function.md) $w$, [Parseval's identity](../../../../../parseval-identity.md) states

$$
\int_{-1}^1|w(x)|^2\,dx=\frac{|a_0|^2}{2}+\sum_{n=1}^{\infty}\bigl(|a_n|^2+|b_n|^2\bigr).
$$

For $w=f-g$, write $s=\sinh1$. Its coefficients are $a_0=2s$, $a_n=2(-1)^ns/(1+n^2\pi^2)$ and $b_n=n\pi a_n$, because $g$ is subtracted. Therefore

$$
\begin{aligned}
\int_{-1}^1(f-g)^2\,dx
&=2s^2+4s^2\sum_{n=1}^{\infty}\frac{1+n^2\pi^2}{(1+n^2\pi^2)^2}\\
&=2s^2\left[1+2\sum_{n=1}^{\infty}\frac1{1+n^2\pi^2}\right]\\
&=2\sinh1\cosh1=\boxed{\sinh2}.
\end{aligned}
$$

The sum was obtained in part (a). As a separate check, $f-g=e^{-x}$ in the interval, whose square has integral $\int_{-1}^1e^{-2x}\,dx=\sinh2$. Endpoint jumps have no effect on this [integral](../../../../../integral-split.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [18](../../18.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
