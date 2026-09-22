<h1 id="a/1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For [equilateral triangular pipe flow](../../../../../../equilateral-triangular-pipe-flow.md), the [polynomial](../../../../../../polynomial-split.md) vanishes on all three walls, so it satisfies [no-slip boundary conditions](../../../../../../no-slip-boundary-condition.md). Direct differentiation gives

$$
\nabla_\perp^2\bigl[(x^2-3y^2)(x-a)\bigr]=(6x-2a)+(-6x+6a)=4a.
$$

Thus

$$
\boxed{A=\frac{G}{4a\mu},\qquad G=\frac{dp}{dz}.}
$$

For $G<0$, $A<0$ and the [velocity](../../../../../../velocity.md) is positive in the triangular interior.

At the wall $x=a$, the outward normal of the [fluid](../../../../../../fluid.md) is $\mathbf e_x$. The axial [traction](../../../../../../traction.md) exerted by the wall on the [fluid](../../../../../../fluid.md) is $\mu w_x$, so the [fluid](../../../../../../fluid.md) exerts the opposite axial [traction](../../../../../../traction.md) on the wall. Since $w_x(a,y)=A(a^2-3y^2)$, the [force](../../../../../../force-split.md) per unit axial length is

$$
\frac{\mathbf F}{\text{axial length}}=-\mu A\mathbf k\int_{-a/\sqrt3}^{a/\sqrt3}(a^2-3y^2)\,dy
=-\mu A\frac{4a^3}{3\sqrt3}\mathbf k
=\boxed{-\frac{a^2}{3\sqrt3}\frac{dp}{dz}\,\mathbf k.}
$$

It points with the flow for a negative axial [pressure gradient](../../../../../../pressure-gradient.md). As a check, the triangular [area](../../../../../../surface-area.md) is $a^2/\sqrt3$, so the total [pressure](../../../../../../pressure-split.md) driving [force](../../../../../../force-split.md) per unit length is $-Ga^2/\sqrt3$; each of the three equivalent walls receives one third.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [A](../../../../a.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the theoretical mechanics course of the University of Oxford](../../../../../split.md)
7. [Theoretical mechanics course of the University of Oxford](../../../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
