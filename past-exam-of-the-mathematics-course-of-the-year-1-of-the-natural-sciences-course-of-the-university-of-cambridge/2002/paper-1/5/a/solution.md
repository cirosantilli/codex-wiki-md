<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $I=\int_0^\infty e^{-x^2}dx$. Positivity allows the squared integral to be written as a first-quadrant [double integral](../../../../../double-integral.md). In [polar coordinates](../../../../../polar-coordinates.md) the [Jacobian determinant](../../../../../jacobian-determinant.md) is $r$, so

$$
I^2=\int_0^{\pi/2}\int_0^\infty e^{-r^2}r\,dr\,d\theta=\frac\pi4,\qquad \boxed{I=\frac{\sqrt\pi}2.}
$$

Using [integration by parts](../../../../../integration-by-parts.md), with the boundary term $xe^{-x^2}$ vanishing at both endpoints,

$$
\boxed{\int_0^\infty x^2e^{-x^2}dx=\frac12\int_0^\infty e^{-x^2}dx=\frac{\sqrt\pi}4.}
$$

The substitution $u=x^2$ also gives the two [antiderivatives](../../../../../antiderivative.md)

$$
\boxed{\int xe^{-x^2}dx=-\frac12e^{-x^2}+C,\qquad \int x^3e^{-x^2}dx=-\frac12(x^2+1)e^{-x^2}+C.}
$$

These values also follow from the [Gaussian moment recurrence](../../../../../gaussian-moment-recurrence.md) and can be checked by [differentiation](../../../../../differentiation.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
