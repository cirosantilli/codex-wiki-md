<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Under spherical symmetry, the [continuity equation](../../../../continuity-equation.md) and [Darcy's law](../../../../darcy-law.md) give

$$
\frac1{r^2}\frac{d}{dr}(r^2q_r)=0,\qquad
q_r=-\frac{\Pi_1}{\eta}\frac{dp}{dr}.
$$

Hence $q_r=C/r^2$, and integrating the [pressure gradient](../../../../pressure-gradient.md) from infinity gives

$$
p(r)-p_0=\frac{\eta C}{\Pi_1r}.
$$

The [boundary condition](../../../../boundary-condition.md) at $r=a$ fixes $C=\Pi_1a\Delta p/\eta$. Therefore [spherical Darcy injection](../../../../spherical-darcy-injection.md) has

$$
\boxed{p(r)=p_0+\frac{a\Delta p}{r},\qquad
q_r(r)=\frac{\Pi_1a\Delta p}{\eta r^2},\qquad
Q=4\pi r^2q_r=\frac{4\pi\Pi_1a\Delta p}{\eta}.}
$$

Here $q_r$ is the superficial [Darcy velocity](../../../../darcy-velocity.md), not the pore [velocity](../../../../velocity.md) $q_r/\varphi$.

For the comparison, assume geometrically similar pore networks, equal [porosity](../../../../porosity.md), the same source radius and far boundary geometry, and equal pump efficiency. [Dimensional analysis](../../../../dimensional-analysis.md) then gives $\Pi_1=C_{\mathrm{geom}}d^2$ with the same dimensionless factor. Consequently

$$
\frac{\Pi_{1A}}{\Pi_{1B}}=4,\qquad
\frac{(\Pi_1/\eta)_A}{(\Pi_1/\eta)_B}=2.
$$

At a fixed desired [volumetric flow rate](../../../../volumetric-flow-rate.md), the required excess [pressure](../../../../pressure-split.md) and pumping [power](../../../../power.md) are

$$
\Delta p=\frac{\eta Q}{4\pi\Pi_1a},\qquad
\mathcal P=Q\Delta p=\frac{\eta Q^2}{4\pi\Pi_1a}.
$$

**Aquifer A requires half the pumping power** at equal throughput, or half the [energy](../../../../energy-split.md) to inject the same volume over the same time. This compares the excess [pressure-volume work](../../../../pressure-volume-work.md) dissipated by the [Darcy flow](../../../../darcy-flow.md); any different baseline compression or other plant costs need separate accounting.

The imposed comparison matters. At fixed $\Delta p$, A takes twice the [volumetric flow rate](../../../../volumetric-flow-rate.md) and twice the instantaneous [power](../../../../power.md), but the same excess [energy](../../../../energy-split.md) per injected volume. The pore spacing alone does not determine [permeability of a porous medium](../../../../permeability-of-a-porous-medium.md) if network geometry or [porosity](../../../../porosity.md) changes; without the geometric assumptions the preference cannot be inferred from $d$ alone.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the fluids course of the University of Oxford](../../../split.md)
5. [Fluids course of the University of Oxford](../../../../fluids-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
