<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [solid angle](../../../solid-angle.md) is the intercepted [surface area](../../../surface-area.md) on a sphere of radius $R$, divided by $R^2$. Take the cone axis as the polar axis of [spherical coordinates](../../../spherical-coordinate-system.md), and call its half-opening [angle](../../../angle.md) $\theta$. With polar integration variable $\vartheta$,

$$
\Omega=\frac1{R^2}\int_0^{2\pi}\int_0^\theta R^2\sin\vartheta\,d\vartheta\,d\phi
=\boxed{2\pi(1-\cos\theta).}
$$

For small $\theta$ measured in radians, the [Taylor series](../../../taylor-series.md) of the [cosine](../../../cosine.md) gives

$$
\boxed{\Omega=\pi\theta^2-\frac{\pi\theta^4}{12}+O(\theta^6)\simeq\pi\theta^2.}
$$

This is the [solid angle of a circular cone](../../../solid-angle-of-a-circular-cone.md), measured in [steradians](../../../steradian.md).

The supplied angular diameter is twice the half-opening [angle](../../../angle.md), so

$$
\theta=\frac{0.533}{2}\frac\pi{180}=0.00465130246\ldots\ \mathrm{rad}.
$$

Hence either apparent disc subtends

$$
\boxed{\Omega\simeq6.797\times10^{-5}\ \mathrm{sr},\qquad
\frac{\Omega}{4\pi}\simeq5.409\times10^{-6}.}
$$

The fraction is about $0.0005409\%$ of the entire celestial sphere. Using the angular diameter directly in $\pi\theta^2$ would give four times the correct small-angle answer.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2019](../../2019-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
