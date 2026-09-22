<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the same [stream function](../../../../stream-function.md) convention and denote differentiation with respect to the [dimensionless variable](../../../../dimensionless-variable.md) $\eta=y/\delta$ by a prime. The proposed [similarity solution](../../../../similarity-solution.md) gives

$$
u=Ax f'(\eta),\qquad v=-A\delta f(\eta).
$$

Its [continuity equation](../../../../continuity-equation.md) holds identically. Substitution in the tangential [Prandtl boundary-layer equation](../../../../prandtl-boundary-layer-equation.md) gives

$$
A^2x\bigl((f')^2-ff''\bigr)
=\frac{\nu Ax}{\delta^2}f'''+A^2x.
$$

Choose the constant scale $\delta=\sqrt{\nu/A}$. The [Hiemenz flow](../../../../hiemenz-flow.md) equation and its [boundary conditions](../../../../boundary-condition.md) are

$$
\boxed{f'''+ff''-(f')^2=-1,\qquad
f(0)=0,\quad f'(0)=0,\quad f'(\infty)=1.}
$$

The first two conditions impose the [no-penetration boundary condition](../../../../no-penetration-boundary-condition.md) and [no-slip boundary condition](../../../../no-slip-boundary-condition.md). The last matches the tangential outer [velocity](../../../../velocity.md). One also has $f''\to0$ and $f(\eta)/\eta\to1$. It is too strong to impose $f-\eta\to0$: the [displacement thickness](../../../../displacement-thickness.md) generally permits a constant offset, $f\sim\eta-B$.

The normal [Navier-Stokes equation](../../../../navier-stokes-equation.md) makes the approximation in part (c) explicit. With this [similarity solution](../../../../similarity-solution.md), it gives

$$
p_y=-\rho g-\rho A^2\delta\bigl(ff'+f''\bigr).
$$

At the wall this differs from $(p_\infty)_y=-\rho g$ by $-\rho A^2\delta f''(0)$. This is a concrete next-order counterexample to interpreting the printed normal [pressure gradient](../../../../pressure-gradient.md) equality exactly; the tangential [Hiemenz flow](../../../../hiemenz-flow.md) equation remains valid at its stated order.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the fluids course of the University of Oxford](../../../split.md)
5. [Fluids course of the University of Oxford](../../../../fluids-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
