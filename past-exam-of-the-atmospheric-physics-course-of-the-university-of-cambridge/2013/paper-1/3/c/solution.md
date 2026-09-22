<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For [dry atmospheric Ertel potential vorticity](../../../../../dry-atmospheric-ertel-potential-vorticity.md), use [absolute vorticity](../../../../../absolute-vorticity.md) $\boldsymbol\omega_a=\nabla\times\mathbf u+2\boldsymbol\Omega$ and [potential temperature](../../../../../potential-temperature.md) $\theta=T(p_0/p)^{R_d/c_p}$:

$$
\boxed{q_E=\frac{\boldsymbol\omega_a\cdot\nabla\theta}{\rho},\qquad
\frac{Dq_E}{Dt}=0.}
$$

The conservation statement is [Ertel's theorem](../../../../../ertel-s-theorem.md) for smooth, inviscid, adiabatic flow with conservative body forces and a thermodynamic equation of state $p=p(\rho,\theta)$. Stretching of $\boldsymbol\omega_a/\rho$ cancels deformation of $\nabla\theta$ in their material derivative; the remaining baroclinic triple product vanishes because $\nabla p$ lies in the span of $\nabla\rho,\nabla\theta$. The atmospheric form includes $1/\rho$; the commonly used [Boussinesq approximation](../../../../../boussinesq-approximation.md) version has a different normalization.

In a predominantly vertical stratification, $q_E\simeq(f+\zeta)\,\partial_z\theta/\rho$. Thus rotation and stratification jointly label air masses. Material conservation explains how parcels deform and stretch while preserving a useful scalar, supports [Rossby waves](../../../../../rossby-wave.md), and helps diagnose sharp fronts, jets and stratospheric intrusions.

Under an appropriate balance model, [potential-vorticity inversion](../../../../../potential-vorticity-inversion.md) recovers associated wind and temperature fields from a PV distribution together with stratification and boundary data. **PV alone does not specify every component of an arbitrary atmospheric flow.** [Potential-vorticity generation by heating and friction](../../../../../potential-vorticity-generation-by-heating-and-friction.md) limits conservative parcel reasoning near strong heating, surface stress or mixing.[PartII§12, equationII.17, physical PDF pp.150–152: dry atmospheric PV and qualified invertibility](../../../../../fundamentals-of-atmosphere-ocean-dynamics-by-michael-edgeworth-mcintyre.md)

## ↑ Ancestors (14)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the atmospheric physics course of the University of Cambridge](../../../../split.md)
6. [Atmospheric Physics course of the University of Cambridge](../../../../../atmospheric-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
