<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Since $\gamma>0$, the causal damped sine has an absolutely convergent [Fourier transform](../../../../../fourier-transform-split.md) for real $\omega$. Resolving the sine into complex exponentials gives

$$
\widetilde f(\gamma,p,\omega)
=\frac1{2i}\int_0^\infty\left[e^{-[\gamma+i(\omega-p)]t}-e^{-[\gamma+i(\omega+p)]t}\right]dt
=\frac1{2i}\left[\frac1{\gamma+i(\omega-p)}-\frac1{\gamma+i(\omega+p)}\right].
$$

Combining the two fractions yields

$$
\boxed{\widetilde f(\gamma,p,\omega)=\frac{p}{(\gamma+i\omega)^2+p^2}.}
$$

The formula also includes $p=0$, for which both the original function and its transform vanish. Its sign reverses when the real parameter $p$ reverses.

## ↑ Ancestors (13)

1. [C](../c.md)
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
