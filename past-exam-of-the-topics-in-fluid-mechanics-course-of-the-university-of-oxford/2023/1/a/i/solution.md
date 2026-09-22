<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take $z$ positive away from the wall into the liquid, and write $p_a$ for [atmospheric pressure](../../../../../atmospheric-pressure.md). For a constant-[mass density](../../../../../density.md) [Newtonian fluid](../../../../../newtonian-fluid.md), the two-dimensional [Navier-Stokes equation](../../../../../navier-stokes-equation.md) and [continuity equation](../../../../../continuity-equation.md) are

$$
\begin{aligned}
u_x+w_z&=0,\\
\rho(u_t+uu_x+wu_z)&=-p_x+\mu(u_{xx}+u_{zz})+\rho g\sin\alpha,\\
\rho(w_t+uw_x+ww_z)&=-p_z+\mu(w_{xx}+w_{zz})-\rho g\cos\alpha.
\end{aligned}
$$

The stationary wall imposes the [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) and [no-penetration boundary condition](../../../../../no-penetration-boundary-condition.md), $u=w=0$ at $z=0$. For a flat [free surface](../../../../../free-surface.md) with negligible air [shear stress](../../../../../shear-stress.md), the [stress boundary condition](../../../../../stress-boundary-condition.md) is $u_z=0$, $p=p_a$ at $z=h_0$; the [kinematic boundary condition](../../../../../kinematic-boundary-condition.md) is $w=0$ there.

For [steady flow](../../../../../steady-flow.md) independent of $x$, these equations give $w=0$, $\mu u_{zz}=-\rho g\sin\alpha$ and $p_z=-\rho g\cos\alpha$. Two [integrations](../../../../../integral-split.md) and the [boundary conditions](../../../../../boundary-condition.md) give the [uniform gravity-driven Newtonian film](../../../../../uniform-gravity-driven-newtonian-film.md):

$$
\boxed{\bar u=\frac{\rho g\sin\alpha}{2\mu}(2h_0z-z^2),\qquad
\bar w=0,\qquad \bar p=p_a+\rho g\cos\alpha(h_0-z).}
$$

Its surface [velocity](../../../../../velocity.md) is $U_0=\rho gh_0^2\sin\alpha/(2\mu)$, while its mean [velocity](../../../../../velocity.md) is $2U_0/3$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the topics in fluid mechanics course of the University of Oxford](../../../../split.md)
6. [Topics in fluid mechanics course of the University of Oxford](../../../../../topics-in-fluid-mechanics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
