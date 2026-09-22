<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The integrand has simple poles at $z=ia$ and $z=-ia$. Only the first is inside the upper contour, and its [residue](../../../../../residue.md) is

$$
\operatorname{Res}_{z=ia}\frac{e^{iz}}{z^2+a^2}=\frac{e^{-a}}{2ia}.
$$

The [residue theorem](../../../../../residue-theorem.md) therefore gives, for every $R>a$,

$$
\boxed{\oint_C\frac{e^{iz}}{z^2+a^2}dz=\frac\pi a e^{-a}.}
$$

On the upper semicircle, $|e^{iz}|=e^{-\operatorname{Im}z}\leq1$ and $|z^2+a^2|\geq R^2-a^2$. The [estimation lemma](../../../../../estimation-lemma.md) bounds the arc contribution by $\pi R/(R^2-a^2)\to0$. Hence the real-axis integral has the same limit, and taking its real part gives

$$
\boxed{\int_{-\infty}^{\infty}\frac{\cos x}{a^2+x^2}dx=\frac\pi a e^{-a}.}
$$

The imaginary part vanishes independently because $\sin x/(a^2+x^2)$ is odd. The real integral converges absolutely, since the denominator grows quadratically.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
