<h1 id="10/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For independent [generalized coordinates](../../../../generalized-coordinate.md) $q_i$, their [generalized velocities](../../../../generalized-velocity.md) $\dot q_i$ and a [Lagrangian](../../../../lagrangian.md) $L(q,\dot q,t)$, the [Euler-Lagrange equations](../../../../euler-lagrange-equation.md) are

$$
\boxed{\frac{d}{dt}\left(\frac{\partial L}{\partial\dot q_i}\right)
-\frac{\partial L}{\partial q_i}=0.}
$$

Here the partial [derivatives](../../../../derivative.md) treat $q_i,\dot q_i,t$ as independent arguments, whereas $d/dt$ follows the motion. For a conservative mechanical system, choose coordinates satisfying the [mechanical constraints](../../../../constraint-mechanics.md), express the [kinetic energy](../../../../kinetic-energy.md) $T$ and [potential energy](../../../../potential-energy.md) $V$ in those coordinates, set $L=T-V$, and evaluate these equations to obtain the [equations of motion](../../../../equation-of-motion.md). If nonconservative [generalized forces](../../../../generalized-forces.md) $Q_i$ are present, they appear on the right-hand side.

A [cyclic coordinate](../../../../cyclic-coordinate.md) is absent explicitly from $L$: $\partial L/\partial q_i=0$, even though $L$ may depend on $\dot q_i$. Its [canonical momentum](../../../../canonical-momentum.md) is consequently conserved,

$$
p_i=\frac{\partial L}{\partial\dot q_i},\qquad\boxed{\dot p_i=0.}
$$

This does not require $\dot q_i=0$ or even that $\dot q_i$ be constant; the relation between [canonical momentum](../../../../canonical-momentum.md) and [generalized velocity](../../../../generalized-velocity.md) depends on the [Lagrangian](../../../../lagrangian.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [10](../../10.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the physics 1 paper of the University of Oxford](../../../split.md)
5. [Physics 1 paper of the University of Oxford](../../../../physics-1-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
