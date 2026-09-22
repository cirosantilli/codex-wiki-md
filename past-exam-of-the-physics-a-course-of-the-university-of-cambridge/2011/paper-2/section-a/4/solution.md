<h1 id="section-a/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The central estimate is $z=3.2743$. [propagation of uncertainty](../../../../../propagation-of-uncertainty.md) must include the occurrence of $x$ in both numerator and denominator. With angular [derivatives](../../../../../derivative.md) measured per [radian](../../../../../radian.md),

$$
z_x=\frac{\sec^2(x+y)}{\tan x}-\frac{\tan(x+y)}{\sin^2x}=-3.5382,\qquad
z_y=\frac{\sec^2(x+y)}{\tan x}=6.6497.
$$

Interpreting the two quoted errors as independent [standard deviations](../../../../../standard-deviation.md), convert them to [radians](../../../../../radian.md) before calculating

$$
\sigma_z^2=z_x^2(4\pi/180)^2+z_y^2(3\pi/180)^2,
\qquad \boxed{z\simeq3.27\pm0.43}.
$$

If the quoted errors are instead absolute bounds, the first-order worst-case estimate is $|\delta z|\lesssim |z_x|\delta x+|z_y|\delta y=0.60$. Correlated errors add $2z_xz_y\operatorname{Cov}(x,y)$ to the [variance](../../../../../variance-split.md). Treating $x+y$ and $x$ as independent would lose their shared [measurement uncertainty](../../../../../measurement-uncertainty.md).

## ↑ Ancestors (14)

1. [4](../4.md)
2. [Section A](../../section-a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2011](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
