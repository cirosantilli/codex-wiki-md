<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose counterclockwise traversal viewed from $+z$, and span the curve by the disk $z=1$, $x^2+y^2\leq2$ with upward normal. Here

$$
\nabla\phi=(2xy,x^2,0),\qquad \nabla\psi=(z,0,x),\qquad \nabla\phi\times\nabla\psi=(x^3,-2x^2y,-x^2z).
$$

The surface side is therefore $-\iint_Dx^2dxdy$. In polar coordinates it is

$$
-\int_0^{2\pi}\int_0^{\sqrt2}r^3\cos^2\theta\,dr\,d\theta=-\pi.
$$

For the direct boundary integral, $dz=0$ gives $\nabla\psi\cdot d\mathbf l=dx$ on $z=1$. Set $x=\sqrt2\cos\theta$, $y=\sqrt2\sin\theta$, so

$$
\boxed{\oint x^2y\,dx=-4\int_0^{2\pi}\cos^2\theta\sin^2\theta\,d\theta=-\pi.}
$$

The two independent evaluations agree. Clockwise traversal and downward normal give $+\pi$ on both sides.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [2013 resit](../../../2013-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
