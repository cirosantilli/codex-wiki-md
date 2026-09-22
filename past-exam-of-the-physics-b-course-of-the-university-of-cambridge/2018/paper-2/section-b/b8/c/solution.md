<h1 id="section-b/b8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In [Lagrangian](../../../../../../lagrangian.md) mechanics, [generalized coordinates](../../../../../../generalized-coordinate.md) $q_i$ describe the independent configurations allowed by the [constraints](../../../../../../constraint-mechanics.md). For particles with ordinary conservative [forces](../../../../../../force-split.md) in an [inertial frame](../../../../../../inertial-frame.md), use $L=T-V$, with [kinetic energy](../../../../../../kinetic-energy.md) $T$ and [potential energy](../../../../../../potential-energy.md) $V$. [Holonomic constraints](../../../../../../holonomic-constraint.md) can often be built into the coordinates, avoiding explicit [constraint](../../../../../../constraint-mechanics.md) [forces](../../../../../../force-split.md).

The [principle of stationary action](../../../../../../principle-of-stationary-action.md) makes the [action](../../../../../../action.md) $\mathcal S=\int_{t_1}^{t_2}L(q,\dot q,t)\,dt$ stationary for variations vanishing at the endpoints. Integrating the [velocity](../../../../../../velocity.md) variation by parts gives

$$
\delta\mathcal S=\int_{t_1}^{t_2}\sum_i
\left(\frac{\partial L}{\partial q_i}-\frac{d}{dt}\frac{\partial L}{\partial\dot q_i}\right)\delta q_i\,dt.
$$

Since each independent variation is arbitrary, the [Euler-Lagrange equations](../../../../../../euler-lagrange-equation.md) are

$$
\boxed{\frac{d}{dt}\frac{\partial L}{\partial\dot q_i}-\frac{\partial L}{\partial q_i}=0.}
$$

If nonconservative [generalized forces](../../../../../../generalized-forces.md) are present, their components appear on the right. The formalism is invariant under suitable coordinate changes and adding a total time [derivative](../../../../../../derivative.md) to $L$ leaves the fixed-endpoint equations unchanged.

The [generalized momentum](../../../../../../generalized-momentum.md) is $p_i=\partial L/\partial\dot q_i$. If $q_i$ is cyclic, $\partial L/\partial q_i=0$ and $p_i$ is conserved. If $L$ has no explicit time dependence, the conserved [energy](../../../../../../energy-split.md) function is

$$
E_L=\sum_i\dot q_i\frac{\partial L}{\partial\dot q_i}-L.
$$

For a [kinetic energy](../../../../../../kinetic-energy.md) quadratic in [velocities](../../../../../../velocity.md) and a velocity-independent [potential energy](../../../../../../potential-energy.md), this equals $T+V$. This connects [symmetry](../../../../../../symmetry-physics.md) to [conservation laws](../../../../../../conservation-law.md).

For example, a [simple pendulum](../../../../../../simple-pendulum-split.md) of [mass](../../../../../../mass.md) $m$ and length $\ell$ has

$$
L=\frac12m\ell^2\dot\theta^2-mg\ell(1-\cos\theta),
\qquad \ddot\theta+\frac{g}{\ell}\sin\theta=0.
$$

Its [tension](../../../../../../tension.md) does not appear because the fixed-length [constraint](../../../../../../constraint-mechanics.md) is already imposed. Expanding for small $\theta$ gives [simple harmonic motion](../../../../../../simple-harmonic-motion.md) with $\omega=\sqrt{g/\ell}$. More generally, expansion of $T$ and $V$ to quadratic order about a [stable equilibrium](../../../../../../stable-equilibrium.md) leads directly to the normal-mode [eigenvalue](../../../../../../eigenvalue.md) problem.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [B8](../../b8.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
