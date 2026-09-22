<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With $u=-t+z$ and $v=t+z$, the [Minkowski metric](../../../../minkowski-metric.md) and the specified [null vector](../../../../null-vector.md) become

$$
\eta=du\,dv+dx^2+dy^2,\qquad
\eta_{uv}=\eta_{vu}=\frac12,\qquad
n=2\partial_v,\qquad n^\flat=du.
$$

The [Minkowski wave operator in null coordinates](../../../../minkowski-wave-operator-in-null-coordinates.md) is $\Box=4\partial_u\partial_v+\partial_x^2+\partial_y^2$. All components of the original [metric perturbation](../../../../linearized-gravity-split.md) still depend only on $u$, since this coordinate change is linear. The result of part (a), differentiated once, reads

$$
2\tilde h''_{v\nu}=\frac12H''\delta_\nu{}^u.
$$

It follows that $\tilde h''_{vv}=\tilde h''_{vx}=\tilde h''_{vy}=0$ and $\tilde h''_{uv}=H''/4$. Taking the [trace](../../../../matrix-trace.md) gives

$$
H''=4\tilde h''_{uv}+\tilde h''_{xx}+\tilde h''_{yy},
\qquad \tilde h''_{xx}+\tilde h''_{yy}=0.
$$

Expanding the scalar $\phi=\tilde h''_{AB}x^Ax^B/2$ in these [null coordinates](../../../../null-coordinate.md) therefore yields

$$
\boxed{\phi=a(u)(x^2-y^2)+b(u)xy+c(u)v+d(u)x+e(u)y+f(u),}
$$

where the coefficients are explicitly

$$
\boxed{a=\frac12\tilde h''_{xx},\quad b=\tilde h''_{xy},\quad
c=\frac14uH'',\quad d=u\tilde h''_{ux},\quad
e=u\tilde h''_{uy},\quad f=\frac12u^2\tilde h''_{uu}.}
$$

The quadratic transverse term is a [harmonic quadratic plane-wave profile](../../../../harmonic-quadratic-plane-wave-profile.md). In particular $\partial_v\phi=c$, $\partial^\mu\overline{\hat h}_{\mu\nu}=2c\,n_\nu$ and $\Box\phi=4c'$, consistently reproducing the failure of wave gauge in part (b).

## ↑ Ancestors (12)

1. [C](../c.md)
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
