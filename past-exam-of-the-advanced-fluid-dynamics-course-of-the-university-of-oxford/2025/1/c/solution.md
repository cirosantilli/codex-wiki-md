<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose a [magnetic vector potential](../../../../magnetic-vector-potential.md) with $\mathbf B=\nabla\times\mathbf A$. The [resistive induction equation](../../../../resistive-induction-equation.md) permits the evolution equation

$$
\partial_t\mathbf A=\mathbf u\times\mathbf B-\eta_m\nabla\times\mathbf B-\nabla\phi.
$$

A [gauge transformation](../../../../gauge-transformation.md) changes $H=\int_V\mathbf A\cdot\mathbf B\,dV$ by a surface integral of the normal [magnetic field](../../../../magnetic-field-split.md), which is zero here. Thus the integrated [magnetic helicity](../../../../magnetic-helicity.md) has [gauge invariance](../../../../gauge-invariance.md) under the stated boundary conditions.

Differentiate both factors in $H$. Use the stated vanishing-boundary assumption to remove the helicity surface flux; this can be implemented in the usual closed-boundary gauge $\mathbf n\times\mathbf A=0$, or by extending the localized field and integrating over all space with sufficient decay. The curl [integration by parts](../../../../integration-by-parts.md) identity then gives

$$
\dot H=\int_V\partial_t\mathbf A\cdot\mathbf B\,dV+\int_V\mathbf A\cdot\nabla\times\partial_t\mathbf A\,dV
=2\int_V\partial_t\mathbf A\cdot\mathbf B\,dV.
$$

The motional term is zero pointwise because $(\mathbf u\times\mathbf B)\cdot\mathbf B=0$. The scalar-potential term integrates to zero by $\nabla\cdot\mathbf B=0$ and the boundary condition. The [resistive magnetic-helicity balance](../../../../resistive-magnetic-helicity-balance.md) is therefore

$$
\boxed{\dot H=-\frac{2\eta}{\mu_0}\int_V\mathbf B\cdot(\nabla\times\mathbf B)\,dV.}
$$

Unlike the resistive [magnetic energy](../../../../magnetic-energy.md) contribution, this signed [integral](../../../../integral-split.md) need not have a fixed sign.

## ↑ Ancestors (12)

1. [C](../c.md)
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
