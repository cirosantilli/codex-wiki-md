<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a fixed fluid domain, consider an incompressible Newtonian [Stokes flow](../../../../../../stokes-flow-split.md) with prescribed [velocities](../../../../../../velocity.md) on its boundaries and prescribed far-field behaviour. Conservative body [forces](../../../../../../force.md), such as gravity, may be absorbed into the [pressure](../../../../../../pressure.md). Among all sufficiently regular divergence-free trial [velocity fields](../../../../../../velocity-field.md) with exactly those boundary [velocities](../../../../../../velocity.md) and far-field behaviour, the Stokes solution minimizes the [viscous dissipation](../../../../../../viscous-dissipation.md)

$$
\mathcal D[\mathbf u]=2\mu\int_{\mathcal D}e_{ij}(\mathbf u)e_{ij}(\mathbf u)\,dV,
\qquad e_{ij}=\tfrac12(\partial_i u_j+\partial_j u_i).
$$

To see this [Minimum-dissipation theorem for Stokes flow](../../../../../../minimum-dissipation-theorem-for-stokes-flow.md), write a trial field as $\mathbf v=\mathbf u+\mathbf w$, with $\nabla\cdot\mathbf w=0$ and homogeneous [velocity](../../../../../../velocity.md) boundary data. The [Newtonian fluid stress tensor](../../../../../../newtonian-fluid-stress-tensor.md) satisfies $\nabla\cdot\boldsymbol\sigma=0$, so integration by parts gives

$$
2\mu\int e(\mathbf u):e(\mathbf w)\,dV
=\int\boldsymbol\sigma:\nabla\mathbf w\,dV=0.
$$

Therefore

$$
\boxed{\mathcal D[\mathbf v]-\mathcal D[\mathbf u]
=2\mu\int e(\mathbf w):e(\mathbf w)\,dV\geq0.}
$$

Equality requires the difference to be a [rigid motion](../../../../../../rigid-transformation.md), eliminated by the fixed wall and far-field data. The theorem varies the [velocity field](../../../../../../velocity-field.md) in one fixed geometry; it does not minimize over particle positions. If a nonconservative body [force](../../../../../../force.md) is prescribed, the appropriate variational functional also includes its work, rather than being the dissipation alone.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
