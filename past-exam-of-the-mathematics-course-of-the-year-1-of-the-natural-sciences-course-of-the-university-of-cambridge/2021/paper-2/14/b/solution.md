<h1 id="14/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply the same dimensionless transformation independently to the two cups, giving $X,Y\in[-\pi/2,\pi/2]$. The total-volume condition becomes $X+Y\geq\pi/2$. Since neither variable can exceed $\pi/2$, this region has $0\leq X\leq\pi/2$ and $\pi/2-X\leq Y\leq\pi/2$, the triangle shown above.

By [independence of random variables](../../../../../independent-random-variables.md), the [joint probability density](../../../../../joint-probability-density.md) is $\tfrac14\cos x\cos y$. The desired [double integral](../../../../../double-integral.md) is

$$
\begin{aligned}
P&=\frac14\int_0^{\pi/2}\cos x\int_{\pi/2-x}^{\pi/2}\cos y\,dy\,dx\\
&=\frac14\int_0^{\pi/2}\cos x(1-\cos x)\,dx\\
&=\frac14\left[1-\int_0^{\pi/2}\frac{1+\cos2x}{2}\,dx\right]
=\frac14-\frac\pi{16}.
\end{aligned}
$$

Thus

$$
\boxed{\mathbb P(v_1+v_2\geq630\,\mathrm{mL})=\frac{4-\pi}{16}.}
$$

Boundary equality has [probability](../../../../../probability.md) zero for these continuous random variables.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [14](../../14.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
