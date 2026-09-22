<h1 id="section-b/b6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Lagrangian mechanics](../../../../../../lagrangian-mechanics-split.md) expresses dynamics through [generalized coordinates](../../../../../../generalized-coordinate.md) $q_i$ that respect the constraints. For a system with conservative, velocity-independent [forces](../../../../../../force-split.md) and standard [kinetic energy](../../../../../../kinetic-energy.md), the [Lagrangian](../../../../../../lagrangian.md) is $L=T-V$. Its equations follow from the [principle of stationary action](../../../../../../principle-of-stationary-action.md):

$$
\mathcal S[q]=\int_{t_1}^{t_2}L(q,\dot q,t)\,dt,\qquad \delta\mathcal S=0
$$

for variations that vanish at the endpoints. Varying the [integral](../../../../../../integral-split.md) and integrating the $\delta\dot q_i$ term by parts gives

$$
\delta\mathcal S=\int_{t_1}^{t_2}\sum_i\left[\frac{\partial L}{\partial q_i}-\frac d{dt}\frac{\partial L}{\partial\dot q_i}\right]\delta q_i\,dt.
$$

Independent variations therefore yield the [Euler-Lagrange equations](../../../../../../euler-lagrange-equation.md):

$$
\boxed{\frac d{dt}\frac{\partial L}{\partial\dot q_i}-\frac{\partial L}{\partial q_i}=0.}
$$

Additional nonconservative [generalized forces](../../../../../../generalized-forces.md) appear on the right-hand side as $Q_i$. The [action](../../../../../../action.md) is stationary, not necessarily a minimum. For ideal [holonomic constraints](../../../../../../holonomic-constraint.md), using suitable [generalized coordinates](../../../../../../generalized-coordinate.md) removes the need to solve explicitly for constraint [forces](../../../../../../force-split.md).

The [conjugate momentum](../../../../../../canonical-momentum.md) is $p_i=\partial L/\partial\dot q_i$. If a coordinate is cyclic, $\partial L/\partial q_i=0$ and its [conjugate momentum](../../../../../../canonical-momentum.md) is conserved. If $L$ has no explicit time dependence, the [energy](../../../../../../energy-split.md) function

$$
E=\sum_i\dot q_ip_i-L
$$

is conserved. It equals $T+V$ for the usual quadratic [kinetic energy](../../../../../../kinetic-energy.md) with time-independent geometry, but that identification is not universal for every [Lagrangian](../../../../../../lagrangian.md) or constraint.

For example, a [simple pendulum](../../../../../../simple-pendulum-split.md) with angle $\theta$, length $\ell$ and bob mass $m$ has

$$
L=\frac12m\ell^2\dot\theta^2+mg\ell\cos\theta,
\qquad \ddot\theta+\frac g\ell\sin\theta=0.
$$

The [tension](../../../../../../tension.md) does no [virtual work](../../../../../../virtual-work.md) in the allowed angular displacement and never needs to be calculated to obtain the angular equation. The method scales naturally to coupled systems and coordinates with complicated geometry.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [B6](../../b6.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2021](../../../../split.md)
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
