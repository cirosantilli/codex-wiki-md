<h1 id="12/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Evenness removes every sine coefficient. In the period-two [Fourier cosine series](../../../../../fourier-cosine-series.md) convention $f=a_0/2+\sum_{n\geq1}a_n\cos(n\pi x)$, the constant coefficient is $a_0=2\int_0^1(1-x)dx=1$. [Integration by parts](../../../../../integration-by-parts.md) gives

$$
a_n=2\int_0^1(1-x)\cos(n\pi x)dx=\frac{2[1-(-1)^n]}{n^2\pi^2}.
$$

Thus the [Fourier cosine series of a triangular wave](../../../../../fourier-cosine-series-of-a-triangular-wave.md) is

$$
\boxed{f(x)=\frac12+\frac4{\pi^2}\sum_{m=0}^\infty\frac{\cos((2m+1)\pi x)}{(2m+1)^2}.}
$$

The periodic function is continuous and piecewise smooth, so the [Dirichlet-Jordan convergence theorem](../../../../../dirichlet-jordan-convergence-theorem.md) gives its value at every point. The summable absolute coefficient bound also gives [uniform convergence](../../../../../uniform-convergence.md) by the [Weierstrass M-test](../../../../../weierstrass-m-test.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [12](../../12.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
