<h1 id="18/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

At a fixed radius, [Parseval's identity](../../../../../parseval-identity.md) applied to the preceding [Fourier series](../../../../../fourier-series-split.md) gives

$$
\int_{-\pi}^{\pi}[y_{f_0}(r,\theta)]^2\,d\theta
=\pi\sum_{\substack{n\ge1\\n\text{ odd}}}\frac{16r^{2n}}{\pi^2n^2}
=\frac{16}{\pi}\sum_{\substack{n\ge1\\n\text{ odd}}}\frac{r^{2n}}{n^2}.
$$

In [polar coordinates](../../../../../polar-coordinates.md), $dA=r\,dr\,d\theta$. Integrating over radius and interchanging the nonnegative sum and [integral](../../../../../integral-split.md) gives

$$
\begin{aligned}
\int_D[y_{f_0}]^2\,dA
&=\frac{16}{\pi}\sum_{\substack{n\ge1\\n\text{ odd}}}\frac1{n^2}\int_0^1r^{2n+1}\,dr\\
&=\boxed{\frac8\pi\sum_{\substack{n\ge1\\n\text{ odd}}}\frac1{n^2(n+1)},\qquad p=2.}
\end{aligned}
$$

The interchange follows from the [monotone convergence theorem](../../../../../monotone-convergence-theorem.md). This is the special case of the [area norm of the Poisson extension in the unit disk](../../../../../area-norm-of-the-poisson-extension-in-the-unit-disk.md) for the odd step boundary data.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [18](../../18.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
