<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The closed boundary includes the curved unit hemisphere and the disk at $y=0$. On the disk, $F=(0,y,0)=0$, so that contribution vanishes. On the curved part the outward normal is $n=(x,y,z)$, giving $F\times n=(yz,0,-xy)$.

Use [spherical coordinates](../../../../spherical-coordinate-system.md) with the polar axis along positive $y$:

$$
x=\sin\theta\cos\phi,\quad y=\cos\theta,\quad z=\sin\theta\sin\phi,
\quad 0\le\theta\le\frac\pi2,\quad0\le\phi\le2\pi.
$$

The area element is $\sin\theta\,d\theta\,d\phi$. Consequently

$$
\iint_SF\times dS
=\int_0^{\pi/2}\cos\theta\sin^2\theta\,d\theta
\int_0^{2\pi}(\sin\phi,0,-\cos\phi)\,d\phi
=\boxed{(0,0,0).}
$$

This directly performs the surface integral and includes the planar cap, rather than applying the closed-surface theorem to only an open hemisphere.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
3. [2017 resit](../../../2017-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
