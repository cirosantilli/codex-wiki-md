<h1 id="k/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

[Milne-Thomson's circle theorem](../../../../milne-thomson-circle-theorem.md) states that if $f(z)$ is a [complex potential of a two-dimensional potential flow](../../../../complex-potential-of-a-two-dimensional-potential-flow.md) whose singularities lie outside $|z|=a$, then

$$
w(z)=f(z)+\overline{f(a^2/\bar z)}
$$

has the circle as a [streamline](../../../../streamline.md), with the original exterior singularities unchanged. Additive constants in the potential are immaterial.

Take $f(z)=\Gamma(2\pi i)^{-1}\log(z-z_1)$, using the convention that positive $\Gamma$ is positive [circulation](../../../../circulation-physics.md). Reflection in the circle gives, up to a constant,

$$
\boxed{w(z)=\frac{\Gamma}{2\pi i}
\left[\log(z-z_1)
-\log\left(z-\frac{a^2}{\bar z_1}\right)+\log z\right].}
$$

The reflected [vortex](../../../../phase-vortex.md) at $a^2/\bar z_1$ has strength $-\Gamma$, while the central term has strength $+\Gamma$. Their combined [circulation](../../../../circulation-physics.md) around the cylinder is zero; this is the [circulation](../../../../circulation-physics.md) normalization implicit in the requested equation.

The [vortex](../../../../phase-vortex.md) moves with the [velocity](../../../../velocity.md) induced by the other singularities, excluding its own singular term. Since [complex velocity](../../../../complex-velocity.md) is $dw/dz=u-iv$, its value at the [vortex](../../../../phase-vortex.md) is $d\bar z_1/dt$. Thus

$$
\frac{d\bar z_1}{dt}
=\frac{\Gamma}{2\pi i}
\left[-\frac1{z_1-a^2/\bar z_1}+\frac1{z_1}\right]
=\boxed{\frac{i\Gamma a^2}{2\pi z_1(|z_1|^2-a^2)}.}
$$

Writing $z_1=re^{i\theta}$ and multiplying this equation by $z_1$ gives

$$
r\dot r-ir^2\dot\theta
=\frac{i\Gamma a^2}{2\pi(r^2-a^2)}.
$$

Its real part implies $\dot r=0$, and its imaginary part gives

$$
\boxed{\dot\theta=-\frac{\Gamma a^2}
{2\pi r^2(r^2-a^2)}.}
$$

The radius is constant and the angular [velocity](../../../../velocity.md) is constant on that orbit. For positive $\Gamma$ the orbit is clockwise with this convention. Retaining the conjugate on the time derivative is essential for the sign.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [K](../../k.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
