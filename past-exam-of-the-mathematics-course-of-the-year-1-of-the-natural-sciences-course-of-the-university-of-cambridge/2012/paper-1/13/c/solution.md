<h1 id="13/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [integrating factor](../../../../../integrating-factor.md) is $e^{kx}$, giving $(e^{kx}y)'=ae^{kx}\sin(mx)$. The required [antiderivative](../../../../../antiderivative.md) is

$$
\int e^{kx}\sin(mx)\,dx
=\frac{e^{kx}}{k^2+m^2}[k\sin(mx)-m\cos(mx)].
$$

After dividing by $e^{kx}$, the [general solution](../../../../../general-solution.md) is the oscillatory term plus $Ce^{-kx}$. The [initial condition](../../../../../initial-condition.md) fixes $C=1+am/(k^2+m^2)$, so

$$
\boxed{y(x)=\left(1+\frac{am}{k^2+m^2}\right)e^{-kx}
+\frac{a[k\sin(mx)-m\cos(mx)]}{k^2+m^2}.}
$$

The real, nonzero parameters ensure $k^2+m^2>0$; direct substitution verifies both the equation and $y(0)=1$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [13](../../13.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
