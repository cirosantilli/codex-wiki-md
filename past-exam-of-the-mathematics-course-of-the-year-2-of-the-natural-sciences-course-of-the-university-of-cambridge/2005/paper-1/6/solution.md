<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For $y''+P(x)y'+Q(x)y=0$, a singular point $x_0$ is a [regular singular point](../../../../regular-singular-point.md) if $(x-x_0)P(x)$ and $(x-x_0)^2Q(x)$ are analytic there. The [Bessel differential equation](../../../../bessel-differential-equation.md) has $xP=1$ and $x^2Q=x^2-\nu^2$, so zero is regular singular.

Use the [Frobenius method](../../../../frobenius-method.md) with $y=x^s\sum_{n\geq0}a_nx^n$, $a_0\ne0$. Matching coefficients gives $(s^2-\nu^2)a_0=0$ and $[(s+n)^2-\nu^2]a_n+a_{n-2}=0$, with missing negative-index coefficients zero. The regular root is $s=\nu$. Then $a_1=0$, all odd coefficients vanish, and the [Frobenius series for Bessel functions](../../../../frobenius-series-for-bessel-functions.md) has recurrence

$$
\boxed{a_{2m}=-\frac{a_{2m-2}}{4m(m+\nu)},\qquad m\geq1.}
$$

For noninteger $\nu$, the root $s=-\nu$ supplies an independent even-power series $y_2=x^{-\nu}\sum_{m\geq0}b_{2m}x^{2m}$ with $b_{2m}=-b_{2m-2}/[4m(m-\nu)]$ and $b_0\ne0$. None of these denominators vanishes. With standard normalization this is $J_{-\nu}(x)$, independent of the [Bessel function of the first kind](../../../../bessel-function-of-the-first-kind.md) $J_\nu(x)$. The real powers here are understood for $x>0$.

For integer $\nu\geq0$ and the stated normalization $a_0=1/(2^\nu\nu!)$, iteration gives

$$
\boxed{a_{2m}=\frac{(-1)^m}{2^{2m+\nu}m!(m+\nu)!},\qquad J_\nu(x)=\sum_{m=0}^\infty\frac{(-1)^m(x/2)^{2m+\nu}}{m!(m+\nu)!}.}
$$

The ratio of consecutive term magnitudes is $|x|^2/[4(m+1)(m+\nu+1)]\to0$. Thus the series converges absolutely for every finite complex $x$, defining an entire function for integer $\nu$. At integer order, $J_{-\nu}=(-1)^\nu J_\nu$; an independent solution is instead the [Bessel function of the second kind](../../../../bessel-function-of-the-second-kind.md).

## ↑ Ancestors (12)

1. [6](../6.md)
2. [Paper 1](../../paper-1-split.md)
3. [2005](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
