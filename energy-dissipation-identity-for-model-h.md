# Energy dissipation identity for Model H

↑ **Parent:** [Model H dynamics](model-h-dynamics.md)

For constant positive [order-parameter mobility](order-parameter-mobility.md) $M$, [dynamic viscosity](dynamic-viscosity.md) $\eta$ and [mass density](density.md) $\rho$, deterministic [Model H dynamics](model-h-dynamics.md) dissipates the sum of composition [free energy](thermodynamic-free-energy.md) and kinetic energy:

$$
\frac{d}{dt}\left[F+\frac\rho2\int|\mathbf v|^2\right]=-\int[M|\nabla\mu|^2+\eta|\nabla\mathbf v|^2]\le0.
$$

Assume smooth fields and periodic or closed, no-work boundaries. Using the [chemical potential of a composition field](chemical-potential-of-a-composition-field.md), [integration by parts](integration-by-parts.md) and [incompressible flow](incompressible-flow.md) gives $\dot F=\int\phi\mathbf v\cdot\nabla\mu-M\int|\nabla\mu|^2$. Dotting the momentum equation with velocity gives $\dot E_{\rm kin}=-\int\phi\mathbf v\cdot\nabla\mu-\eta\int|\nabla\mathbf v|^2$. [Pressure](pressure.md) and convective work vanish under the boundary assumptions; the two capillary transfer terms cancel. This proves both the sign of the [Korteweg force](korteweg-force.md) and its reversible exchange of energy with the composition field.

## ↑ Ancestors (9)

1. [Model H dynamics](model-h-dynamics.md)
2. [Binary fluid mixture](binary-fluid-mixture.md)
3. [Compositional order parameter](compositional-order-parameter.md)
4. [Order parameter](order-parameter.md)
5. [Critical phenomenon](critical-phenomenon-split.md)
6. [Statistical physics](statistical-physics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-344/2/a/solution.md)
