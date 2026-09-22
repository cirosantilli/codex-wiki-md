<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The periodically extended $x^2$ is [even](../../../../even-function.md), so every sine coefficient is zero. With the convention $f=a_0/2+\sum_{n\geq1}(a_n\cos nx+b_n\sin nx)$, the [Fourier coefficients](../../../../fourier-coefficient.md) are

$$
a_0=\frac2\pi\int_0^\pi x^2dx=\frac{2\pi^2}3,\qquad a_n=\frac2\pi\int_0^\pi x^2\cos nx\,dx=\frac{4(-1)^n}{n^2}.
$$

For the second integral, two applications of [integration by parts](../../../../integration-by-parts.md) give $\int_0^\pi x^2\cos nx\,dx=2\pi(-1)^n/n^2$. Consequently

$$
\boxed{x^2=\frac{\pi^2}3+4\sum_{n=1}^\infty\frac{(-1)^n\cos nx}{n^2},\qquad -\pi\leq x\leq\pi.}
$$

The periodic extension is continuous even at the joined endpoints, where both one-sided values equal $\pi^2$. The [pointwise convergence of a piecewise smooth Fourier series](../../../../pointwise-convergence-of-a-piecewise-smooth-fourier-series.md) therefore gives the displayed values throughout the interval; the coefficient bound also gives [uniform convergence](../../../../uniform-convergence.md) by the [Weierstrass M-test](../../../../weierstrass-m-test.md). Setting $x=\pi$ and then $x=0$ yields

$$
\boxed{\sum_{n=1}^\infty\frac1{n^2}=\frac{\pi^2}6,\qquad \sum_{n=1}^\infty\frac{(-1)^{n+1}}{n^2}=\frac{\pi^2}{12}.}
$$

## ↑ Ancestors (12)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2002](../../split.md)
4. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
