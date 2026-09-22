<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Suppose initially that $f,g$ are absolutely integrable, so [Fubini's theorem](../../../../../fubini-s-theorem.md) justifies exchanging the integrations. The transform of their [convolution](../../../../../convolution.md) is

$$
\widetilde h(\omega)=\int_{-\infty}^{\infty}\int_{-\infty}^{\infty}f(t)g(z-t)e^{-i\omega z}\,dt\,dz.
$$

Set $s=z-t$, so $z=s+t$ and $dz=ds$. The exponential separates:

$$
\widetilde h(\omega)=\left[\int_{-\infty}^{\infty}f(t)e^{-i\omega t}\,dt\right]
\left[\int_{-\infty}^{\infty}g(s)e^{-i\omega s}\,ds\right].
$$

Therefore the [convolution theorem](../../../../../convolution-theorem.md) is

$$
\boxed{\widetilde{f*g}(\omega)=\widetilde f(\omega)\widetilde g(\omega).}
$$

No extra $2\pi$ occurs in this direction with the specified normalization.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
