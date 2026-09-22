<h1 id="18/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Separate the already finite sine terms from the even part $g(x)=x^2-\pi|x|$. Since $g$ is an [even function](../../../../../even-function.md), it has no sine coefficients. Its constant coefficient is

$$
a_0=\frac2\pi\int_0^\pi(x^2-\pi x)dx=-\frac{\pi^2}{3}.
$$

For $n\geq1$, [integration by parts](../../../../../integration-by-parts.md) gives

$$
\int_0^\pi x\cos nx\,dx=\frac{(-1)^n-1}{n^2},\qquad
\int_0^\pi x^2\cos nx\,dx=\frac{2\pi(-1)^n}{n^2}.
$$

Therefore the cosine [Fourier coefficients](../../../../../fourier-coefficient.md) are

$$
a_n=\frac2\pi\int_0^\pi(x^2-\pi x)\cos nx\,dx
=\frac{2(1+(-1)^n)}{n^2}.
$$

Only even frequencies survive: $a_{2m}=1/m^2$. The sine [Fourier coefficients](../../../../../fourier-coefficient.md) are $b_1=1$, $b_2=-2$, with all others zero. Hence

$$
\boxed{f(x)=\sin x-2\sin2x-\frac{\pi^2}{6}
+\sum_{m=1}^\infty\frac{\cos2mx}{m^2}}.
$$

The periodic function is continuous at zero and at its endpoint joins, and its coefficients are absolutely summable. Thus this [Fourier series](../../../../../fourier-series-split.md) represents it everywhere, including those joins.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [18](../../18.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
