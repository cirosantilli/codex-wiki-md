<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the real [magnetic field](../../../../../../magnetic-field.md) $\boldsymbol{\mathcal B}$ in the coupled equations; its leading periodic approximation will be $\operatorname{Re}(\mathbf B e^{i\omega t})$. In the conducting [incompressible flow](../../../../../../incompressible-flow.md), the [magnetohydrodynamic momentum equation](../../../../../../magnetohydrodynamic-momentum-equation.md), [resistive induction equation](../../../../../../resistive-induction-equation.md) and [solenoidal magnetic-field constraint](../../../../../../solenoidal-magnetic-field-constraint.md) are

$$
\begin{aligned}
\rho[\partial_t\mathbf u+(\mathbf u\cdot\nabla)\mathbf u]&=-\nabla p+\rho\nu\nabla^2\mathbf u+\mathbf j\times\boldsymbol{\mathcal B},\\
\partial_t\boldsymbol{\mathcal B}&=\nabla\times(\mathbf u\times\boldsymbol{\mathcal B})+\eta\nabla^2\boldsymbol{\mathcal B},\\
\nabla\cdot\mathbf u&=0,\qquad\nabla\cdot\boldsymbol{\mathcal B}=0,\qquad\mathbf j=\mu_0^{-1}\nabla\times\boldsymbol{\mathcal B}.
\end{aligned}
$$

Here $p$ is [pressure](../../../../../../pressure.md), $\mathbf j$ is [electric current density](../../../../../../current-density.md), and $\eta$ and $\nu$ are [magnetic diffusivity](../../../../../../magnetic-diffusivity.md) and [kinematic viscosity](../../../../../../kinematic-viscosity.md). The [moving-conductor Ohm law](../../../../../../moving-conductor-ohm-law.md) gives $\mathbf E=-\mathbf u\times\boldsymbol{\mathcal B}+\eta\nabla\times\boldsymbol{\mathcal B}$.

In the insulating exterior, neglecting [displacement current](../../../../../../displacement-current.md), the [magnetic field](../../../../../../magnetic-field.md) is [curl](../../../../../../curl.md)-free away from the wire and [solenoidal](../../../../../../solenoidal-vector-field.md). The imposed [electric current density](../../../../../../current-density.md) supplies

$$
\nabla\times\boldsymbol{\mathcal B}_{\rm ext}=\mu_0J\cos(\omega t)\delta(x)\delta(y+b)\mathbf e_z,
\qquad \nabla\cdot\boldsymbol{\mathcal B}_{\rm ext}=0.
$$

The exterior [electric field](../../../../../../electric-field.md) also satisfies [Faraday's law](../../../../../../faraday-s-law-of-induction.md). At the rigid wall, impose the [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md) $\mathbf u=0$. At finite conductivity, the [interface conditions for electromagnetic fields](../../../../../../interface-conditions-for-electromagnetic-fields.md) give continuous normal [magnetic field](../../../../../../magnetic-field.md), continuous tangential [magnetic field](../../../../../../magnetic-field.md) for equal permeability and no prescribed singular surface current, and continuous tangential [electric field](../../../../../../electric-field.md). The normal [electric current density](../../../../../../current-density.md) is zero at an insulating wall; it is automatic for the present two-dimensional fields with current only along $z$. The induced fields decay far from the wire and wall, and initial conditions, or selection of the periodic state after transients, complete the specification. In the limiting [perfect conductor](../../../../../../perfect-conductor.md) approximation a surface current can emerge, permitting a tangential-field jump.

The fully coupled solution need not remain monochromatic: a harmonic [magnetic field](../../../../../../magnetic-field.md) produces both a mean and a twice-frequency [Lorentz force density](../../../../../../lorentz-force-density.md), and the resulting [velocity](../../../../../../velocity.md) can generate further harmonics. The following parts consistently use the leading magnetic response with fluid motion neglected.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
