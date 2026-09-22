<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**Transform pair.** In the paper's symmetric normalization, the inverse [Fourier transform](../../../../fourier-transform-split.md) is

$$
\boxed{g(x)=\frac1{\sqrt{2\pi}}\int_{-\infty}^{\infty}\widetilde g(k)e^{ikx}\,dk.}
$$

Split the transform of $e^{-c|x|}$ at zero, with $c>0$:

$$
\begin{aligned}
\mathcal F[e^{-c|x|}](k)&=\frac1{\sqrt{2\pi}}\left[\int_{-\infty}^0e^{(c-ik)x}\,dx+\int_0^\infty e^{-(c+ik)x}\,dx\right]\\
&=\frac1{\sqrt{2\pi}}\left(\frac1{c-ik}+\frac1{c+ik}\right)=\boxed{\sqrt{\frac2\pi}\frac c{c^2+k^2}}.
\end{aligned}
$$

The inverse formula applied to this result gives

$$
e^{-c|x|}=\frac c\pi\int_{-\infty}^{\infty}\frac{e^{ikx}}{c^2+k^2}\,dk.
$$

Because the kernel is even, replacing the transform variable by $x$ and the argument by $k$ yields

$$
\boxed{\mathcal F\left[\frac1{x^2+c^2}\right](k)=\frac{\sqrt{2\pi}}{2c}e^{-c|k|}.}
$$

The factors of $\sqrt{2\pi}$ depend on the normalization and will also enter the [convolution theorem](../../../../convolution-theorem.md).

**Convolution theorem.** For integrable [functions](../../../../function-split.md) define the [convolution](../../../../convolution.md)

$$
(f*g)(x)=\int_{-\infty}^{\infty}f(x-y)g(y)\,dy.
$$

Substitute this into the [Fourier transform](../../../../fourier-transform-split.md), interchange the two absolutely integrable factors using [Fubini's theorem](../../../../fubini-s-theorem.md), and set $z=x-y$:

$$
\begin{aligned}
\widetilde{f*g}(k)&=\frac1{\sqrt{2\pi}}\int_{-\infty}^{\infty}\int_{-\infty}^{\infty}f(x-y)g(y)e^{-ikx}\,dy\,dx\\
&=\frac1{\sqrt{2\pi}}\left(\int f(z)e^{-ikz}\,dz\right)\left(\int g(y)e^{-iky}\,dy\right).
\end{aligned}
$$

Therefore

$$
\boxed{\widetilde{f*g}(k)=\sqrt{2\pi}\,\widetilde f(k)\widetilde g(k).}
$$

**Integral equation.** Put $f_a(x)=1/(x^2+a^2)$. Since this is even, the left side is $f_a*g$. The transformed equation is

$$
\frac\pi a e^{-a|k|}\widetilde g(k)=\frac{\sqrt{2\pi}}{2b}e^{-b|k|},
$$

so

$$
\widetilde g(k)=\frac a{b\sqrt{2\pi}}e^{-(b-a)|k|}.
$$

The assumption $b>a$ makes the new scale $d=b-a$ positive. Inverting with the previously established transform pair gives

$$
\boxed{g(x)=\frac{a(b-a)}{\pi b\,[x^2+(b-a)^2]}.}
$$

The [Cauchy convolution semigroup](../../../../cauchy-convolution-semigroup.md) gives a quick verification. With $K_c(x)=c/[\pi(x^2+c^2)]$, the formula is $g=(a/b)K_{b-a}$ and $f_a=(\pi/a)K_a$. Hence $f_a*g=(\pi/b)K_b=1/(x^2+b^2)$, as required. The solution is unique among integrable [functions](../../../../function-split.md) because the multiplier $\widetilde f_a(k)$ never vanishes.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2001](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
