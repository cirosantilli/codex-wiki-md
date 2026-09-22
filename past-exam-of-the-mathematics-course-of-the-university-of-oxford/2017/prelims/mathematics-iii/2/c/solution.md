<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [cardioid](../../../../../../cardioid.md) meets the [unit circle](../../../../../../complex-unit-circle.md) where $1+\cos\theta=1$, namely at $\theta=\pi/2,3\pi/2$. The [polar area formula](../../../../../../polar-area-formula.md) gives the [area](../../../../../../surface-area.md) between radii $r_1\le r_2$ as $\frac12\int(r_2^2-r_1^2)\,d\theta$.

For $-\pi/2\le\theta\le\pi/2$, the [cardioid](../../../../../../cardioid.md) lies outside the [unit circle](../../../../../../complex-unit-circle.md). The right-hand region therefore has [area](../../../../../../surface-area.md)

$$
A_R=\frac12\int_{-\pi/2}^{\pi/2}\left((1+\cos\theta)^2-1\right)\,d\theta
=\int_{-\pi/2}^{\pi/2}\cos\theta\,d\theta+\frac12\int_{-\pi/2}^{\pi/2}\cos^2\theta\,d\theta
=2+\frac\pi4.
$$

On $\pi/2\le\theta\le\pi$, the [unit circle](../../../../../../complex-unit-circle.md) lies outside the [cardioid](../../../../../../cardioid.md). The upper left region has [area](../../../../../../surface-area.md)

$$
A_U=\frac12\int_{\pi/2}^{\pi}\left(1-(1+\cos\theta)^2\right)\,d\theta
=-\int_{\pi/2}^{\pi}\cos\theta\,d\theta-\frac12\int_{\pi/2}^{\pi}\cos^2\theta\,d\theta
=1-\frac\pi8.
$$

By [reflection symmetry](../../../../../../reflection-symmetry.md) the lower left region has the same [area](../../../../../../surface-area.md). Thus

$$
\boxed{A_R=2+\frac\pi4,\qquad A_U=A_L=1-\frac\pi8.}
$$

The two left regions touch only at the [cusp](../../../../../../cusp-algebraic-geometry.md); their interiors are disconnected. As a check, the difference between the [cardioid](../../../../../../cardioid.md)'s total [area](../../../../../../surface-area.md) $3\pi/2$ and the [unit circle](../../../../../../complex-unit-circle.md)'s [area](../../../../../../surface-area.md) $\pi$ is $A_R-A_U-A_L=\pi/2$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Mathematics III](../../../mathematics-iii-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
