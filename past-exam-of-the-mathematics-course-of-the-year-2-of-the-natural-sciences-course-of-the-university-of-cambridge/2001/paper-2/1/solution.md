<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For the nonconstant boundary data, use [separation of variables](../../../../separation-of-variables.md) in [polar coordinates](../../../../polar-coordinates.md) and put $\phi=R(r)\cos2\theta$. [Laplace's equation](../../../../laplace-equation.md) reduces to

$$
r^2R''+rR'-4R=0.
$$

This [Cauchy-Euler equation](../../../../cauchy-euler-equation.md) has independent solutions $r^2$ and $r^{-2}$. Unlike a disk containing the origin, the [annulus](../../../../annulus-mathematics.md) permits both. The zero inner boundary value requires $R=A(r^2-a^4r^{-2})$, and the outer value requires $A=Vb^2/(b^4-a^4)$. Hence

$$
\boxed{\phi_0(r,\theta)=V\frac{b^2(r^4-a^4)}{r^2(b^4-a^4)}\cos2\theta,\qquad a<r<b.}
$$

Substituting $r=a$ gives zero, while $r=b$ gives $V\cos2\theta$. This is the [Dirichlet problem on an annulus for one Fourier mode](../../../../dirichlet-problem-on-an-annulus-for-one-fourier-mode.md); no other angular mode is needed.

For the changed inner boundary value, use [superposition](../../../../superposition-principle.md) to add a radial [harmonic function](../../../../harmonic-function.md) that is $-V$ at $a$ and zero at $b$. The radial zero-mode equation is $(rR')'=0$, giving $R=C+D\log r$. Imposing the two constant boundary values gives

$$
R(r)=-V\frac{\log(b/r)}{\log(b/a)}.
$$

Therefore the second answer is

$$
\boxed{\phi(r,\theta)=V\frac{b^2(r^4-a^4)}{r^2(b^4-a^4)}\cos2\theta-V\frac{\log(b/r)}{\log(b/a)}.}
$$

The logarithmic term is independent of $\theta$, so it changes only the angular average of the [electric potential](../../../../electric-potential.md). Both answers are unique for these [Dirichlet boundary conditions](../../../../dirichlet-boundary-condition.md), by uniqueness for [Laplace's equation](../../../../laplace-equation.md).

## ↑ Ancestors (12)

1. [1](../1.md)
2. [Paper 2](../../paper-2-split.md)
3. [2001](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
