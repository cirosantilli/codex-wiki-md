<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The squared [norm](../../../../../norm.md) of the original function is

$$
\int_{\mathbb R}|f(x)|^2\,dx=\int_{-\pi/2}^{\pi/2}\sin^2x\,dx=\frac\pi2.
$$

Applying the [Parseval identity](../../../../../parseval-identity.md) to part (c), using the evenness of the squared transform, gives

$$
\frac\pi2=\frac1{2\pi}\int_{\mathbb R}\frac{4k^2\cos^2(\pi k/2)}{(k^2-1)^2}\,dk=\frac4\pi\int_0^{\infty}\frac{k^2\cos^2(\pi k/2)}{(k^2-1)^2}\,dk.
$$

Thus the last [integral](../../../../../integral-split.md) equals $\pi^2/8$. Now set $u=\pi k/2$. Since

$$
\frac{k^2\,dk}{(k^2-1)^2}=\frac\pi2\frac{u^2\,du}{(u^2-\pi^2/4)^2},
$$

we obtain

$$
\boxed{\int_0^{\infty}\frac{u^2\cos^2u}{(u^2-\pi^2/4)^2}\,du=\frac2\pi\frac{\pi^2}{8}=\frac\pi4.}
$$

The apparent singularity at $u=\pi/2$ is removable: the continuous value of the integrand there is $1/4$. No principal-value interpretation is needed.

## ↑ Ancestors (13)

1. [D](../d.md)
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
