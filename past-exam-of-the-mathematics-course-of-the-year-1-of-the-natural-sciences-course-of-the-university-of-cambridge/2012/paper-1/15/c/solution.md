<h1 id="15/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Differentiate $x=r\cos\theta$, $y=r\sin\theta$:

$$
dx=\cos\theta\,dr-r\sin\theta\,d\theta,\qquad
dy=\sin\theta\,dr+r\cos\theta\,d\theta.
$$

Squaring and adding cancels the mixed terms and uses $\cos^2\theta+\sin^2\theta=1$, giving

$$
\boxed{dx^2+dy^2=dr^2+r^2d\theta^2.}
$$

For this [cardioid](../../../../../cardioid.md), the [polar arc length](../../../../../polar-arc-length.md) integrand is

$$
\sqrt{\sin^2\theta+(1+\cos\theta)^2}
=\sqrt{2+2\cos\theta}=2|\cos(\theta/2)|.
$$

The [cosine](../../../../../cosine.md) inside the [absolute value](../../../../../absolute-value.md) changes sign at $\theta=\pi$. Therefore the perimeter is

$$
\ell=2\int_0^\pi\cos(\theta/2)\,d\theta
-2\int_\pi^{2\pi}\cos(\theta/2)\,d\theta
=\boxed{8}
$$

in coordinate [length](../../../../../length.md) units. The isolated [cusp](../../../../../cusp-algebraic-geometry.md) does not obstruct this piecewise [smooth](../../../../../smooth-function.md) [arc length](../../../../../arc-length.md) integral.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [15](../../15.md)
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
