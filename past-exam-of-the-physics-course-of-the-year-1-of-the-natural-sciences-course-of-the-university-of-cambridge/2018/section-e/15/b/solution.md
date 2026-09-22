<h1 id="section-e/15/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [conservative vector field](../../../../../conservative-vector-field.md) has path-independent [work](../../../../../work.md): the integral $\int_A^B\mathbf F\cdot d\mathbf r$ depends only on its endpoints. Equivalently, the [line integral](../../../../../line-integral.md) around every closed path in its domain vanishes. One can then define a single-valued [potential energy](../../../../../potential-energy.md) $U$ by

$$
U(B)-U(A)=-\int_A^B\mathbf F\cdot d\mathbf r,
\qquad
\boxed{\mathbf F=-\nabla U,\qquad W_{A\to B}=U(A)-U(B).}
$$

The arbitrary additive constant in $U$ has no effect on the [force](../../../../../force-split.md). A useful zero is often chosen at infinity for a localized attractive interaction.

A differentiable [conservative force](../../../../../conservative-force.md) has $\nabla\times\mathbf F=0$ because the [curl](../../../../../curl.md) of a [gradient](../../../../../gradient.md) vanishes. Conversely, a smooth curl-free field on a [simply connected](../../../../../simply-connected-space.md) domain admits a global scalar potential. The domain condition matters: on the punctured plane, $\mathbf F=(C/r)\widehat{\boldsymbol\theta}$ has zero [curl](../../../../../curl.md) away from the missing origin but closed-loop work $2\pi C$ around it. It is not globally conservative there. The existence of a local potential does not establish a single-valued potential throughout a domain with holes.

The [work-energy theorem](../../../../../work-energy-theorem.md) gives $\Delta T=W$ for [kinetic energy](../../../../../kinetic-energy.md) $T$. If all forces are conservative and $U$ has no explicit time dependence, then

$$
\Delta T=-\Delta U,\qquad
\boxed{T+U=\text{constant}.}
$$

This is [conservation of mechanical energy](../../../../../conservation-of-mechanical-energy.md). In one dimension, an [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) occurs at $dU/dx=0$; a local minimum with $U''>0$ is stable, while a maximum with $U''<0$ is unstable. Expanding about a minimum gives $U\simeq U_0+U''(x_0)(x-x_0)^2/2$, producing [simple harmonic motion](../../../../../simple-harmonic-motion.md) with $\omega^2=U''(x_0)/m$.

Examples include the [spring](../../../../../spring.md) force $F_x=-kx$ with $U=kx^2/2$, the near-surface gravitational [force](../../../../../force-split.md) $-mg\widehat{\mathbf z}$ with $U=mgz$, and the central [Newtonian gravitational field](../../../../../newtonian-gravitational-field.md) with $U=-GMm/r$. An electrostatic [force](../../../../../force-split.md) on a fixed [electric charge](../../../../../electric-charge-split.md) $q$ has $U=q\Phi$, where $\Phi$ is the [electric potential](../../../../../electric-potential.md).

Sliding [friction](../../../../../friction.md) provides a contrasting physical test: traversing a closed path still dissipates [mechanical energy](../../../../../mechanical-energy.md), since the frictional force opposes the local motion on both outward and return legs. Its work depends on path length and cannot be represented by a position-only $U$. Total [energy](../../../../../energy-split.md) can remain conserved when the resulting internal energy is included. Also, even if $\mathbf F=-\nabla U(\mathbf r,t)$ at each instant, explicit time dependence gives $d(T+U)/dt=\partial U/\partial t$; a static conservative-field argument alone does not guarantee constant mechanical energy in that situation.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [15](../../15.md)
3. [Section E](../../../section-e.md)
4. [2018](../../../../2018-split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
