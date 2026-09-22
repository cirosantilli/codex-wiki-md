<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Apply the [Laplacian](../../../../laplacian.md) in [polar coordinates](../../../../polar-coordinates.md) twice to the proposed separated function. For any real exponent $m$,

$$
\nabla^2(r^m\cos2\theta)=(m^2-4)r^{m-2}\cos2\theta,
$$

so the [biharmonic equation](../../../../biharmonic-equation.md) becomes

$$
\nabla^4(r^m\cos2\theta)=(m^2-4)((m-2)^2-4)r^{m-4}\cos2\theta=0.
$$

Its four distinct roots are $m=-2,0,2,4$. The [separated polar solutions of the biharmonic equation](../../../../separated-polar-solutions-of-the-biharmonic-equation.md) therefore give the complete radial family in this angular sector,

$$
\psi=(Ar^{-2}+B+Cr^2+Dr^4)\cos2\theta.
$$

Equivalently, its radial equation is a fourth-order [Cauchy-Euler equation](../../../../cauchy-euler-equation.md); four distinct powers supply four [linearly independent](../../../../linear-independence.md) solutions, so no logarithmic terms are required.

**Interior.** Continuity with value zero at the origin removes both $r^{-2}\cos2\theta$ and $\cos2\theta$. The latter depends on the approach direction even though it is bounded. The two [boundary conditions](../../../../boundary-condition.md) at unit radius then give $C+D=0$ and $2C+4D=1$. Consequently

$$
\boxed{\psi_{\mathrm{in}}(r,\theta)=\tfrac12(r^4-r^2)\cos2\theta,\qquad 0\leq r\leq1.}
$$

This extends smoothly through the origin: $r^2\cos2\theta=x^2-y^2$ and $r^4\cos2\theta=(x^2+y^2)(x^2-y^2)$ are [polynomials](../../../../polynomial-split.md). Its radial [derivative](../../../../derivative.md) at $r=1$ is $(2r^3-r)\cos2\theta=\cos2\theta$.

**Exterior.** The condition on the radial [derivative](../../../../derivative.md) at infinity excludes the $r^2$ and $r^4$ terms. A nonzero $B\cos2\theta$ is permitted, since the required decay concerns the radial [derivative](../../../../derivative.md). Now $A+B=0$ and $-2A=1$, giving

$$
\boxed{\psi_{\mathrm{out}}(r,\theta)=\tfrac12(1-r^{-2})\cos2\theta,\qquad r\geq1.}
$$

Indeed $\partial_r\psi_{\mathrm{out}}=r^{-3}\cos2\theta\to0$, and its value at unit radius is zero. These are particular interior and exterior solutions for the [biharmonic streamfunction](../../../../biharmonic-stream-function-for-planar-stokes-flow.md); no condition requiring $\psi$ itself to vanish at infinity was imposed.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [Paper 2](../../paper-2-split.md)
3. [2002](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
