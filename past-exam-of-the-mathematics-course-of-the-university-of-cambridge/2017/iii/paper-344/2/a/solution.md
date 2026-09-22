<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The field $\phi$ is a [compositional order parameter](../../../../../../compositional-order-parameter.md) in a [binary fluid mixture](../../../../../../binary-fluid-mixture.md). Its spatial integral is conserved in a closed sample, so advection and diffusion enter a [continuity equation](../../../../../../continuity-equation.md); the [material derivative](../../../../../../material-derivative.md) follows the incompressible fluid. The diffusive current $\mathbf J=-M\nabla\mu$, with positive [order-parameter mobility](../../../../../../order-parameter-mobility.md) $M$, moves material down the [chemical potential](../../../../../../chemical-potential.md) [gradient](../../../../../../gradient.md). The [chemical potential of a composition field](../../../../../../chemical-potential-of-a-composition-field.md) is the [functional derivative](../../../../../../functional-derivative.md) of the symmetric quartic [Landau free energy](../../../../../../landau-free-energy.md)

$$
F=\int\left[\frac a2\phi^2+\frac b4\phi^4+\frac\kappa2|\nabla\phi|^2\right]d\mathbf r,
$$

so $\mu=a\phi+b\phi^3-\kappa\nabla^2\phi$. Positive $b,\kappa$ stabilize large amplitudes and penalize sharp interfaces; $a<0$ permits phase separation.

The momentum equation is the [Navier-Stokes equation](../../../../../../navier-stokes-equation.md) with [dynamic viscosity](../../../../../../dynamic-viscosity.md) $\eta$, constant [mass density](../../../../../../density.md) $\rho$, and the [Korteweg force](../../../../../../korteweg-force.md) $-\phi\nabla\mu$ arising from composition stresses. The [pressure](../../../../../../pressure.md) enforces [incompressible flow](../../../../../../incompressible-flow.md), $\nabla\cdot\mathbf v=0$, and can absorb pure [gradient](../../../../../../gradient.md) contributions to that thermodynamic force. For example, $-\phi\nabla\mu=\mu\nabla\phi-\nabla(\phi\mu)$ gives an equivalent force after redefining the [pressure](../../../../../../pressure.md). These equations constitute deterministic [Model H dynamics](../../../../../../model-h-dynamics.md).

Their dissipative signs can be checked by the [energy dissipation identity for Model H](../../../../../../energy-dissipation-identity-for-model-h.md). Under periodic or no-flux, no-work [boundary conditions](../../../../../../boundary-condition.md), composition advection and capillary work cancel between $F$ and the kinetic energy, giving

$$
\boxed{\frac{d}{dt}\left[F+\frac\rho2\int|\mathbf v|^2\,d\mathbf r\right]=-\int\left[M|\nabla\mu|^2+\eta|\nabla\mathbf v|^2\right]d\mathbf r\le0.}
$$

Thus diffusion and viscosity dissipate energy, while the reversible advective coupling transfers it between composition and motion. Thermal noises are omitted at this deterministic hydrodynamic level.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
