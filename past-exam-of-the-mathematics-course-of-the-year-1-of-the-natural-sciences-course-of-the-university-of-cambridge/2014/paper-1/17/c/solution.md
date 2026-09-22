<h1 id="17/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take the odd extension $H(x)=x(\pi-|x|)$ on $[-\pi,\pi]$ and then extend with period $2\pi$. It agrees with the required arch for $0\leq x\leq\pi$ and is continuous at its joins. Its [Fourier sine series](../../../../../fourier-sine-series.md) has

$$
b_n=\frac2\pi\int_0^\pi x(\pi-x)\sin nx\,dx.
$$

For clarity, let $h=x(\pi-x)$, so $h'=\pi-2x$ and $h''=-2$. Two integrations by parts, with the first endpoint term zero, give

$$
\begin{aligned}
\int_0^\pi h\sin nx\,dx
&=\frac1n\int_0^\pi h'\cos nx\,dx\\
&=-\frac1{n^2}\int_0^\pi h''\sin nx\,dx
=\frac{2[1-(-1)^n]}{n^3}.
\end{aligned}
$$

Consequently $b_n=4[1-(-1)^n]/(\pi n^3)$: the even coefficients vanish and the odd ones are $8/(\pi n^3)$. This proves

$$
\boxed{h(x)=\frac8\pi\sum_{n=0}^{\infty}\frac{\sin((2n+1)x)}{(2n+1)^3},\qquad0\leq x\leq\pi.}
$$

The [Fourier sine series of an odd quadratic arch](../../../../../fourier-sine-series-of-an-odd-quadratic-arch.md) converges to this continuous extension; its coefficients are also absolutely summable. Finally evaluate at $x=\pi/2$. The left side is $\pi^2/4$ and the [sine](../../../../../sine.md) factors are $(-1)^n$, so

$$
\boxed{\sum_{n=0}^{\infty}\frac{(-1)^n}{(2n+1)^3}=\frac{\pi^3}{32}.}
$$

The evaluation is at a [continuity](../../../../../continuous-function.md) point, so it does not invoke a jump midpoint.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [17](../../17.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
