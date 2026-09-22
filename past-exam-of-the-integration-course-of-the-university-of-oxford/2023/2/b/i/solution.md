<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $J=\int_0^\infty e^{-x^2}\,dx$. It is positive and finite: on $(0,1)$ the integrand is at most one, and on $[1,\infty)$ it is at most $e^{-x}$. Since the planar integrand is nonnegative and measurable, [Tonelli's theorem](../../../../../tonelli-theorem.md) gives

$$
J^2=\int_{(0,\infty)^2}e^{-(x^2+y^2)}\,dx\,dy.
$$

The [change of variables formula](../../../../../change-of-variables-formula.md) in [polar coordinates](../../../../../polar-coordinates.md), with $x=r\cos\theta$, $y=r\sin\theta$ and absolute [Jacobian determinant](../../../../../jacobian-determinant.md) $r$, yields

$$
J^2=\int_0^{\pi/2}\int_0^\infty e^{-r^2}r\,dr\,d\theta
=\frac\pi2\cdot\frac12=\frac\pi4.
$$

One can apply the formula first on $\delta<r<R$, $0<\theta<\pi/2$, where the coordinate map is a [diffeomorphism](../../../../../diffeomorphism.md), and then exhaust the quadrant using the [monotone convergence theorem](../../../../../monotone-convergence-theorem.md). Taking the positive square root proves the half-line [Gaussian integral](../../../../../gaussian-integral.md):

$$
\boxed{J=\frac{\sqrt\pi}{2}.}
$$

Here $dx$ is understood in the one-dimensional integral; it is missing from the printed question.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the integration course of the University of Oxford](../../../../split.md)
6. [Integration course of the University of Oxford](../../../../../integration-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
