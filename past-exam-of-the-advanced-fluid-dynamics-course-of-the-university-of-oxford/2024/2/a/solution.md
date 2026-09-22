<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Using the given linear momentum balance, multiply by the [velocity](../../../../velocity.md) and integrate over the fixed volume:

$$
\frac{d}{dt}\int_V\frac12\rho u_iu_i\,dV=\int_Vu_i\partial_j\sigma_{ij}\,dV
=\int_{\partial V}u_i\sigma_{ij}n_j\,dS-\int_V\sigma_{ij}\partial_j u_i\,dV.
$$

This is [integration by parts](../../../../integration-by-parts.md) component by component, or the [divergence theorem](../../../../divergence-theorem.md). The first term is boundary [stress](../../../../stress.md) power. With component-first [velocity gradient](../../../../velocity-gradient.md) $K_{ij}=\partial_j u_i$, the second is the [double contraction](../../../../double-contraction.md) $\Phi=\sigma:K$.

For a [Newtonian fluid](../../../../newtonian-fluid.md), $\sigma=-pI+2\mu e$, where $e=(K+K^T)/2$ is the [rate-of-strain tensor](../../../../strain-rate-tensor.md) and $\mu\ge0$ is [dynamic viscosity](../../../../dynamic-viscosity-split.md). [Incompressibility](../../../../incompressible-flow.md) removes the pressure contribution, and the [symmetric tensor](../../../../symmetric-tensor.md) $e$ is orthogonal to the antisymmetric part of $K$. Therefore

$$
\boxed{\Phi=2\mu e:e=2\mu\sum_{ij}e_{ij}^2\ge0.}
$$

The displayed energy identity follows for the stated linear balance. A full advective momentum equation in a fixed control volume would also contribute an advective [kinetic energy](../../../../kinetic-energy.md) flux. The nonnegativity statement here is for a purely Newtonian viscous stress; a [viscoelastic](../../../../viscoelasticity.md) stress can exchange stored [free energy](../../../../thermodynamic-free-energy.md) with the flow.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
