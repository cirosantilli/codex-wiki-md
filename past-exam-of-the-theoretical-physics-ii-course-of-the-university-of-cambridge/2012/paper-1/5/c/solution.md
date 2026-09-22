<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Fresnel convolution of free-particle time slices](../../../../../fresnel-convolution-of-free-particle-time-slices.md) follows by completing the square:

$$
\frac{(x_k-x_0)^2}{k}+(x_{k+1}-x_k)^2
=\frac{k+1}{k}\left(x_k-\frac{x_0+kx_{k+1}}{k+1}\right)^2
+\frac{(x_{k+1}-x_0)^2}{k+1}.
$$

The second term is independent of $x_k$. The shifted [Fresnel integral](../../../../../fresnel-integral.md) in the first term gives

$$
\boxed{\sqrt{\frac{2\pi i\hbar\epsilon}{m}\frac{k}{k+1}}\,
\exp\left[\frac{im(x_{k+1}-x_0)^2}
{2\hbar\epsilon(k+1)}\right].}
$$

Here $k$ is the positive slice index, not a [wave number](../../../../../wavenumber.md). The phase is fixed by the same convergence prescription as the short-time kernel.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the theoretical physics II course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics II course of the University of Cambridge](../../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
