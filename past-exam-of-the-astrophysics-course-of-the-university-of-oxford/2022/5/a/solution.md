<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $n(\mathbf x)=\int f\,d^3v$ and $\overline A=n^{-1}\int Af\,d^3v$. Assume the [one-particle distribution function](../../../../one-particle-distribution-function.md) and its weighted tails decay enough that all required [velocity](../../../../velocity.md) integrals converge and boundary terms at infinite [velocity](../../../../velocity.md) vanish. Multiply the steady [Collisionless Boltzmann equation](../../../../collisionless-boltzmann-equation.md) by $v_j$ and integrate over [velocity](../../../../velocity.md). In [Cartesian coordinates](../../../../cartesian-coordinate-system.md), spatial differentiation commutes with this integration, while [integration by parts](../../../../integration-by-parts.md) gives

$$
\int v_j\frac{\partial f}{\partial v_i}d^3v=-\delta_{ij}n.
$$

Consequently the three force-balance equations are

$$
\boxed{\sum_{i=1}^3\frac{\partial}{\partial x_i}\left(n\overline{v_iv_j}\right)=-n\frac{\partial\Phi}{\partial x_j},\qquad j=1,2,3.}
$$

Explicitly the $x$ component is $\partial_x(n\overline{v_x^2})+\partial_y(n\overline{v_xv_y})+\partial_z(n\overline{v_xv_z})=-n\Phi_x$, with cyclic counterparts for $y,z$. For equal stellar [masses](../../../../mass.md), multiplying by the common [mass](../../../../mass.md) replaces $n$ by the [mass density](../../../../density.md) $\rho$; for multiple stellar [masses](../../../../mass.md), use a mass-weighted [one-particle distribution function](../../../../one-particle-distribution-function.md) or derive a separate equation for each tracer population.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the astrophysics course of the University of Oxford](../../../split.md)
5. [Astrophysics course of the University of Oxford](../../../../astrophysics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
