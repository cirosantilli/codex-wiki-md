<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take an [isothermal](../../../../isothermal-process.md) [hydrostatic](../../../../hydrostatic-equilibrium.md) reference atmosphere, $\rho_0(z)=\rho_s e^{-z/H}$, and [linearize](../../../../linearization.md) about rest. The horizontal acceleration and pressure-gradient force retain the equatorial [Coriolis parameter](../../../../coriolis-parameter.md) $f\simeq\beta y$, with $\beta=2\Omega/a$. The [traditional approximation](../../../../traditional-approximation-geophysical-fluid-dynamics.md) retains only its vertical component. Quadratic perturbation advection is neglected. The vertical acceleration is balanced by perturbation [buoyancy](../../../../buoyancy.md) and [pressure gradient](../../../../gradient.md) after removing the reference [hydrostatic balance](../../../../hydrostatic-equilibrium.md).

The continuity constraint is the [anelastic approximation](../../../../anelastic-approximation.md), $\nabla\cdot(\rho_0\mathbf u)=0$, giving $u_x+v_y+w_z-w/H=0$. It retains stratification-driven expansion while filtering acoustic [density](../../../../density.md) fluctuations. It is therefore not the full compressible continuity equation. Adiabatic displacement in a stably stratified background gives $b_t+N^2w=0$, with $N$ the [Brunt–Väisälä frequency](../../../../buoyancy-frequency.md); upward displacement develops restoring negative [buoyancy](../../../../buoyancy.md).

**[Pressure](../../../../pressure-split.md) convention matters.** With the entropy-buoyancy equation just described, a consistent reduced-pressure form writes the [pressure](../../../../pressure-split.md) acceleration as $-\nabla\Phi$, where $\Phi=p'/\rho_0$. Its vertical term is $-\partial_z(p'/\rho_0)$, not simply $-\rho_0^{-1}p'_z$. The original source explicitly specifies variable $\rho_0(z)$ but prints the latter. Those differ by $p'/(\rho_0H)$, so the two cannot silently be equated. Parts [b](../b.md) and [c](../c.md) display the consequence and then solve the explicitly corrected reduced-pressure model that yields the requested wave equation. This is a mathematical inconsistency in the printed set, not missing source material.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
