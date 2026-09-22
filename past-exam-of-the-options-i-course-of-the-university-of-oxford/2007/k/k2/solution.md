<h1 id="k/k2/solution">Solution</h1>

↑ **Parent:** [K2](../k2.md)

The [Milne-Thomson circle theorem](../../../../milne-thomson-circle-theorem.md) replaces a potential $f$ analytic inside the circle of radius $a$ by $f(z)+\overline{f(a^2/\bar z)}$ outside it, when its original singularities are outside. The circle becomes a [streamline](../../../../streamline.md), the imposed flow at infinity is preserved, and no extra [circulation](../../../../circulation-physics.md) is introduced.

Use the convention that positive [circulation](../../../../circulation-physics.md) is counterclockwise, so a vortex potential is $\Gamma\log(z-z_1)/(2\pi i)$ and its derivative is $u-iv$. With $b=a^2/\bar z_1$, the circle construction gives

$$
\boxed{w(z)=\frac{\Gamma}{2\pi i}\{\log(z-z_1)-\log(z-b)+\log z\}}
$$

up to an additive constant and local logarithm branches. There is an image vortex of strength $-\Gamma$ at $b$ and a central vortex of strength $\Gamma$. Their zero net interior [circulation](../../../../circulation-physics.md) is needed for the specified motion equation.

The original vortex moves with the regular velocity of the image flow, excluding its own singular velocity. Thus

$$
\frac{d\bar z_1}{dt}=\frac{\Gamma}{2\pi i}\left\{-\frac1{z_1-a^2/\bar z_1}+\frac1{z_1}\right\}
=\boxed{\frac{i\Gamma a^2}{2\pi z_1(|z_1|^2-a^2)}}.
$$

The conjugation in this equation matches the printed source. Write $z_1=re^{i\theta}$ and cancel $e^{-i\theta}$ to obtain

$$
\dot r-ir\dot\theta=\frac{i\Gamma a^2}{2\pi r(r^2-a^2)}.
$$

Real and imaginary parts give

$$
\boxed{\dot r=0,\qquad\dot\theta=-\frac{\Gamma a^2}{2\pi r^2(r^2-a^2)}}.
$$

The vortex moves uniformly on the circle determined by its initial radius, clockwise for positive $\Gamma$ in this convention.

## ↑ Ancestors (12)

1. [K2](../k2.md)
2. [K](../../k.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
