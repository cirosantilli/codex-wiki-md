<h1 id="12/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In [spherical coordinates](../../../../../../spherical-coordinate-system.md), with polar angle $0\le\theta\le\pi$ and azimuth $0\le\varphi<2\pi$, the [volume element](../../../../../../volume-element.md) is

$$
\boxed{dV=r^2\sin\theta\,dr\,d\theta\,d\varphi.}
$$

The [mass density](../../../../../../density.md) is radial, so integrating over both angles gives

$$
\begin{aligned}
M&=4\pi A\int_0^R(1-e^{-r/r_0})\,dr\\
&=4\pi A\left[R-r_0(1-e^{-R/r_0})\right].
\end{aligned}
$$

Writing $q=r_0/R>0$, this becomes

$$
\boxed{M=4\pi ARf(q),\qquad f(q)=1-q+qe^{-1/q}.}
$$

Although the [mass density](../../../../../../density.md) diverges like $A/(r_0r)$ near the origin, multiplication by the spherical [volume element](../../../../../../volume-element.md) gives an integrable expression. Thus the central singularity does not produce infinite [mass](../../../../../../mass.md).

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [12](../../../12.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
