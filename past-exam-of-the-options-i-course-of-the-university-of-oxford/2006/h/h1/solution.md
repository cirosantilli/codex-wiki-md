<h1 id="h/h1/solution">Solution</h1>

↑ **Parent:** [H1](../h1.md)

For a holonomic conservative system the [Lagrangian](../../../../lagrangian.md) is $L(q,\dot q,t)=T-V$, the difference between [kinetic energy](../../../../kinetic-energy.md) and [potential energy](../../../../potential-energy.md). The [Euler-Lagrange equations](../../../../euler-lagrange-equation.md) are

$$
\frac d{dt}\frac{\partial L}{\partial\dot q_j}-\frac{\partial L}{\partial q_j}=0,\qquad j=1,\ldots,n.
$$

If $\partial L/\partial q_j=0$, this gives $d p_j/dt=0$ for the [generalized momentum](../../../../generalized-momentum.md) $p_j=\partial L/\partial\dot q_j$. Such a coordinate is a [cyclic coordinate](../../../../cyclic-coordinate.md).

In [cylindrical coordinates](../../../../cylindrical-coordinate-system.md) the squared speed is $\dot r^2+r^2\dot\theta^2+\dot z^2$. The holonomic constraint $z=r^2/a$ gives $\dot z=2r\dot r/a$, while gravity has [potential energy](../../../../potential-energy.md) $V=mgz$. Therefore

$$
\boxed{L=\frac m2\left[\left(1+\frac{4r^2}{a^2}\right)\dot r^2+r^2\dot\theta^2\right]-\frac{mg r^2}{a}}.
$$

There is no explicit $\theta$ dependence, so $\theta$ is a [cyclic coordinate](../../../../cyclic-coordinate.md) and

$$
\boxed{p_\theta=mr^2\dot\theta=\text{constant}}.
$$

This is [angular momentum](../../../../angular-momentum.md) about the vertical symmetry axis. At $r=0$ the polar angle is singular, but the Cartesian [angular momentum](../../../../angular-momentum.md) $m(x\dot y-y\dot x)$ remains well defined and has the same conserved value.

## ↑ Ancestors (12)

1. [H1](../h1.md)
2. [H](../../h.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
