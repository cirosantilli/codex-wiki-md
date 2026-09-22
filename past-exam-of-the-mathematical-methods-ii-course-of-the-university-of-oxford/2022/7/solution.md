<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

The two planes bound $z-1\le y\le1-z$, and the elliptical cross-section has $-1\le z\le1$. Under $x=2r\cos\theta$, $z=r\sin\theta$, the absolute [Jacobian determinant](../../../jacobian-determinant.md) for $(x,z)$ is $2r$. Therefore

$$
V=\int_0^{2\pi}\int_0^1\int_{r\sin\theta-1}^{1-r\sin\theta}2r\,dy\,dr\,d\theta
=\int_0^{2\pi}\int_0^1 4r(1-r\sin\theta)\,dr\,d\theta
=\boxed{4\pi}.
$$

As a check, the cross-sectional [ellipse](../../../ellipse.md) has area $2\pi$, while the part of the thickness proportional to $z$ integrates to zero by reflection. The mean thickness is therefore two.

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2022](../../2022-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
