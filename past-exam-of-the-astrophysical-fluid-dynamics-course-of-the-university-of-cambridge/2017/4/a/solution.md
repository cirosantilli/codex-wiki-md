<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume an inviscid [barotropic fluid](../../../../barotropic-fluid.md) acted on by a conservative body force $-\boldsymbol\nabla\psi$. Define its [barotropic enthalpy function](../../../../barotropic-enthalpy-function.md) by

$$
H(\rho)=\int^{\rho}\frac{p'(s)}s\,ds,\qquad
\boldsymbol\nabla H=\frac{\boldsymbol\nabla p}{\rho}.
$$

The [Euler equations for an inviscid fluid](../../../../euler-equations-for-an-inviscid-fluid-split.md) are then $\partial_t\mathbf v+(\mathbf v\cdot\boldsymbol\nabla)\mathbf v=-\boldsymbol\nabla(H+\psi)$. Using the [vorticity](../../../../vorticity-split.md) $\boldsymbol\omega=\boldsymbol\nabla\times\mathbf v$ and the vector identity

$$
(\mathbf v\cdot\boldsymbol\nabla)\mathbf v
=\boldsymbol\nabla(v^2/2)-\mathbf v\times\boldsymbol\omega
$$

gives $\partial_t\mathbf v+\boldsymbol\nabla B=\mathbf v\times\boldsymbol\omega$, where $B=v^2/2+H+\psi$.

For **steady flow**, dotting this equation with $\mathbf v$ yields $\mathbf v\cdot\boldsymbol\nabla B=0$. Thus [Bernoulli's equation](../../../../bernoulli-equation.md) is

$$
\boxed{\frac{v^2}{2}+\int^{\rho}\frac{p'(s)}s\,ds+\psi
=\text{constant along each streamline}.}
$$

The constant need not agree between different [streamlines](../../../../streamline.md). If the flow is also [irrotational](../../../../irrotational-vector-field.md), the vector equation gives $\boldsymbol\nabla B=0$, so one common constant applies throughout a connected flow region.

For an [isentropic process](../../../../isentropic-process.md) with $p=K\rho^\gamma$, $H=\gamma p/[(\gamma-1)\rho]$ up to an additive constant, equal to the thermodynamic [specific enthalpy](../../../../specific-enthalpy.md). For an externally maintained isothermal gas, $H=a^2\ln(\rho/\rho_{\rm ref})$; this [pressure](../../../../pressure-split.md) potential is not the constant thermodynamic enthalpy of a fixed-temperature ideal gas.

If steady flow is not assumed, a useful additional case is unsteady [potential flow](../../../../potential-flow.md) $\mathbf v=\boldsymbol\nabla\phi$. The same vector equation integrates spatially to

$$
\boxed{\partial_t\phi+\frac{v^2}{2}+H+\psi=C(t).}
$$

General unsteady barotropic flow does not possess the steady streamline constant without further conditions.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../../split.md)
5. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../../../astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
