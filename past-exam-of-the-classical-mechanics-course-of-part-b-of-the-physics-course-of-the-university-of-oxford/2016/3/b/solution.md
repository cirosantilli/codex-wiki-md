<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $n$ degrees of freedom, [phase space](../../../../phase-space.md) is the $2n$-dimensional space of [canonical coordinates](../../../../canonical-variables.md) $(q_1,\ldots,q_n,p_1,\ldots,p_n)$. Initial data at one point determine a [trajectory](../../../../trajectory.md) under the [Hamilton equations](../../../../hamilton-s-equations.md).

[Liouville's theorem](../../../../liouville-theorem.md) in [Hamiltonian](../../../../hamiltonian.md) mechanics states that this flow preserves the canonical volume element $d\Gamma=\prod_i dq_i\,dp_i$. Its [divergence](../../../../divergence.md) is

$$
\nabla_{q,p}\cdot(\dot q,\dot p)
=\sum_i\left(\frac{\partial^2H}{\partial q_i\partial p_i}-\frac{\partial^2H}{\partial p_i\partial q_i}\right)=0.
$$

If $J(t)$ is the [Jacobian determinant](../../../../jacobian-determinant.md) of the flow from initial data, the determinant evolution formula gives $\dot J=J\nabla\cdot(\dot q,\dot p)=0$. Since $J(0)=1$, it remains one, proving preservation of every advected phase volume. The proof also applies to smooth explicitly time-dependent Hamiltonians.

For an ensemble density $\rho(q,p,t)$, probability conservation and the same vanishing [divergence](../../../../divergence.md) give

$$
\boxed{\partial_t\rho+\sum_i\left(\dot q_i\partial_{q_i}\rho+\dot p_i\partial_{p_i}\rho\right)=0,
\quad\text{or}\quad \partial_t\rho+\{\rho,H\}=0.}
$$

Thus the fine-grained density is constant along the [Hamiltonian](../../../../hamiltonian.md) [trajectories](../../../../trajectory.md), although the ensemble may shear, stretch and develop fine structure. This is not a claim that coordinate-space volume or every lower-dimensional projection is conserved.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the classical mechanics course of Part B of the physics course of the University of Oxford](../../../split.md)
5. [Classical mechanics course of Part B of the physics course of the University of Oxford](../../../../classical-mechanics-course-of-part-b-of-the-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
