<h1 id="11a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\phi_1,\phi_2$ be two solutions with the same [Neumann boundary condition](../../../../../../neumann-boundary-condition.md), and set $u=\phi_1-\phi_2$. Then

$$
\nabla^2u-m^2u=0\quad\hbox{in }V,
\qquad
\frac{\partial u}{\partial n}=0\quad\hbox{on }S.
$$

Multiplying by $u$ and applying [Green's first identity](../../../../../../green-s-first-identity.md) gives

$$
\int_V\left(|\nabla u|^2+m^2u^2\right)dV
=\int_Su\frac{\partial u}{\partial n}\,dS
=0.
$$

The integrand is nonnegative. If $m>0$, both terms can vanish only when $u=0$, so the solution of the [modified Helmholtz equation](../../../../../../modified-helmholtz-equation.md) is unique.

If $m=0$, the identity only forces $\nabla u=0$. On a connected region, $u$ may be any constant. Thus solutions of the [Laplace equation](../../../../../../laplace-equation.md) with prescribed normal derivative are unique only up to an additive constant, so

$$
\boxed{\text{uniqueness fails when }m=0}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [11A](../../11a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
