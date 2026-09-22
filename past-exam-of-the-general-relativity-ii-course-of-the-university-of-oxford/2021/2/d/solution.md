<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Continue with the active sign convention for the [linearized coordinate gauge transformation](../../../../linearized-coordinate-gauge-transformation.md). Choose local [functions](../../../../function-split.md) $A,B,C,F$ of $u$ by [integration](../../../../integral-split.md) so that

$$
A''=\frac c2,\qquad B''=\frac d2,\qquad C''=\frac e2,\qquad F'=-\frac f2.
$$

For example, for any fixed $u_0$ one may take

$$
A(u)=\frac12\int_{u_0}^u(u-s)c(s)\,ds,\quad
B(u)=\frac12\int_{u_0}^u(u-s)d(s)\,ds,\quad
C(u)=\frac12\int_{u_0}^u(u-s)e(s)\,ds,\quad
F(u)=-\frac12\int_{u_0}^u f(s)\,ds.
$$

A generator, specified as a [covector](../../../../covector.md) with components in the [null coordinates](../../../../null-coordinate.md) $(u,v,x,y)$, is

$$
\boxed{\chi=A\,dv+B\,dx+C\,dy+
\bigl(-A'v-B'x-C'y+F\bigr)\,du.}
$$

Indeed, with $\delta h_{AB}=\partial_A\chi_B+\partial_B\chi_A$, the mixed components cancel:

$$
\delta h_{uv}=A'-A'=0,\qquad
\delta h_{ux}=B'-B'=0,\qquad
\delta h_{uy}=C'-C'=0.
$$

All components without a $u$ index vanish as well, and

$$
\delta h_{uu}=-2A''v-2B''x-2C''y+2F'
=-cv-dx-ey-f.
$$

Since $n^\flat=du$, only the $uu$ component needs changing. Thus

$$
\boxed{\mathring h=\psi\,du^2,\qquad
\psi=a(u)(x^2-y^2)+b(u)xy.}
$$

**Yes, $\mathring h$ satisfies both equations (3).** Its [trace](../../../../matrix-trace.md) is zero, $\partial_v\psi=0$ gives zero [divergence](../../../../divergence.md), and the [harmonic quadratic plane-wave profile](../../../../harmonic-quadratic-plane-wave-profile.md) gives

$$
\partial^A\overline{\mathring h}_{AB}=2\partial_v\psi\,\delta_B{}^u=0,
\qquad
\Box\psi=4\partial_u\partial_v\psi+\partial_x^2\psi+\partial_y^2\psi=2a-2a=0.
$$

The two surviving [functions](../../../../function-split.md) encode the two [gravitational wave polarizations](../../../../gravitational-wave-polarization.md); constant and linear transverse terms have been removed by the explicit [linearized coordinate gauge transformation](../../../../linearized-coordinate-gauge-transformation.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the general relativity II course of the University of Oxford](../../../split.md)
5. [General relativity II course of the University of Oxford](../../../../general-relativity-ii-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
