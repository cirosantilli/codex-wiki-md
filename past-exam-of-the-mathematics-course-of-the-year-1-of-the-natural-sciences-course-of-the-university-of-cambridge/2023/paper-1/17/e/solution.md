<h1 id="17/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Evaluate the [Fourier sine series](../../../../../fourier-sine-series.md) of part (d) at the interior [point](../../../../../point-geometry.md) $x=1/2$. Only odd indices remain, with alternating signs:

$$
\frac12=\frac2\pi\left(1-\frac13+\frac15-\cdots\right),\qquad \pi=4\sum_{k=0}^{\infty}\frac{(-1)^k}{2k+1}.
$$

Thus $\boxed{A=4}$.

For the second identity, apply [Parseval's identity](../../../../../parseval-identity.md) to $h(x)=x^2$. From part (c), $a_0=2/3$, $a_n=4(-1)^n/(n^2\pi^2)$ and $b_n=0$, so

$$
\int_{-1}^1x^4\,dx=\frac12\left(\frac23\right)^2+\frac{16}{\pi^4}\sum_{n=1}^{\infty}\frac1{n^4}.
$$

The left side is $2/5$, giving $\frac{16}{\pi^4}\sum n^{-4}=2/5-2/9=8/45$. Consequently

$$
\boxed{\pi^4=90\sum_{n=1}^{\infty}\frac1{n^4},\qquad B=90.}
$$

The first [series](../../../../../series-mathematics.md) is conditionally convergent, while the second converges absolutely by the [P-series](../../../../../p-series.md) criterion.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [17](../../17.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
