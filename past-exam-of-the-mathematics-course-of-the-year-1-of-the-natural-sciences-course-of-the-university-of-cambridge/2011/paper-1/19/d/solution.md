<h1 id="19/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Choose the upward orientation of the paraboloid cap. Its boundary is the [circle](../../../../../circle.md) $x^2+y^2=4$ at $z=1$, oriented counterclockwise as viewed from above. By [Stokes theorem](../../../../../stokes-theorem.md),

$$
\int_S(\nabla\times A)\cdot dS=\oint_{\partial S}A\cdot dr.
$$

On the boundary, $dz=0$ and $A\cdot dr=y\,dx-3xy\,dy$. Parametrize by $x=2\cos\theta$, $y=2\sin\theta$, $0\leq\theta\leq2\pi$. Then

$$
\oint_{\partial S}A\cdot dr
=\int_0^{2\pi}[-4\sin^2\theta-24\cos^2\theta\sin\theta]d\theta
=\boxed{-4\pi}.
$$

The second term integrates to zero over a full [period](../../../../../period-of-a-function.md), while the first contributes $-4\pi$. Equivalently, replace the cap by the upward disk at $z=1$: there $(\nabla\times A)_z=-3y-1$, whose integral is $-4\pi$ by symmetry.

An orientation is not stated in the original question. The displayed result uses the upward normal, also the outward normal on the curved top of the enclosed cap; the opposite orientation gives **$4\pi$**.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [19](../../19.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
