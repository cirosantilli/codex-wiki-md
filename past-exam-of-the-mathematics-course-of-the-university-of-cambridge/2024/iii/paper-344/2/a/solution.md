<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The thermodynamic [order parameter](../../../../../../order-parameter.md) is the conserved scalar composition difference $\phi$ of the [binary fluid mixture](../../../../../../binary-fluid-mixture.md). The momentum density $\rho\mathbf v$ is an additional conserved [hydrodynamic mode](../../../../../../hydrodynamic-mode.md); it is not a symmetry-breaking order parameter, but it must be retained because momentum relaxes only through spatial transport.

Composition conservation gives a continuity equation,

$$
(\partial_t+\mathbf v\mathbin\cdot\nabla)\phi=-\nabla\mathbin\cdot\mathbf J.
$$

The current $\mathbf J=-M\nabla\mu$ is the leading isotropic, dissipative constitutive law: it drives material down gradients of the [chemical potential](../../../../../../chemical-potential.md). For the [Landau-Ginzburg theory](../../../../../../landau-ginzburg-theory.md)

$$
F[\phi]=\int d^3\mathbf r
\left(\frac a2\phi^2+\frac b4\phi^4+\frac\kappa2|\nabla\phi|^2\right),
$$

the [functional derivative](../../../../../../functional-derivative.md) is

$$
\mu=\frac{\delta F}{\delta\phi}
=a\phi+b\phi^3-\kappa\nabla^2\phi.
$$

These statements give the advective [Cahn--Hilliard equation](../../../../../../cahn-hilliard-equation.md).

Constant mass density and [incompressible flow](../../../../../../incompressible-flow.md) require $\nabla\mathbin\cdot\mathbf v=0$. Momentum conservation gives the [Navier-Stokes equation](../../../../../../navier-stokes-equation.md): material acceleration equals the sum of the Newtonian viscous force $\eta\nabla^2\mathbf v$, the pressure force $-\nabla P$, and the [Korteweg force](../../../../../../korteweg-force.md) $-\phi\nabla\mu$. The pressure is the [Lagrange multiplier](../../../../../../lagrange-multiplier.md) enforcing incompressibility. Together these equations are [Model H dynamics](../../../../../../model-h-dynamics.md); isothermality removes the need for a separate energy equation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
