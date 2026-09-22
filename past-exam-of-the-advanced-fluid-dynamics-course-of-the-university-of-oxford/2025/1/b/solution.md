<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $E_B=\int_VB^2/(2\mu_0)\,dV$ be the total [magnetic energy](../../../../magnetic-energy.md). Multiply the curl form of the [resistive induction equation](../../../../resistive-induction-equation.md) by $\mathbf B/\mu_0$ and integrate over the fixed volume. The identity

$$
\int_V\mathbf B\cdot\nabla\times\mathbf C\,dV=\int_V\mathbf C\cdot\nabla\times\mathbf B\,dV+\int_{\partial V}\mathbf n\cdot(\mathbf C\times\mathbf B)\,dS
$$

follows from the [divergence theorem](../../../../divergence-theorem.md). The stated zero boundary fields remove its surface term. Applying it to the motional and resistive contributions yields the [magnetic energy balance in resistive magnetohydrodynamics](../../../../magnetic-energy-balance-in-resistive-magnetohydrodynamics.md):

$$
\boxed{\dot E_B=\int_V(\mathbf u\times\mathbf B)\cdot\mathbf J\,dV-\frac\eta{\mu_0^2}\int_V|\nabla\times\mathbf B|^2\,dV
=-\int_V\mathbf u\cdot(\mathbf J\times\mathbf B)\,dV-\eta\int_VJ^2\,dV.}
$$

The first term is the negative of the mechanical power delivered to the fluid by the [Lorentz force density](../../../../lorentz-force-density.md). It transfers [energy](../../../../energy-split.md) between fluid motion and the [magnetic field](../../../../magnetic-field-split.md), with either sign. The second is the nonpositive magnetic contribution to [Joule heating](../../../../joule-heating.md). A nonzero positive [electrical resistivity](../../../../electrical-resistivity.md) therefore dissipates [magnetic energy](../../../../magnetic-energy.md) at rate $\eta\int_VJ^2\,dV$; it does not force the total [magnetic energy](../../../../magnetic-energy.md) to decrease when fluid motion supplies a larger positive power.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
