<h1 id="section-e/15/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In SI units, the microscopic [Maxwell's equations](../../../../../maxwell-equations-split.md) for total charge density $\rho$ and current density $\mathbf J$ are

$$
\boxed{\boldsymbol\nabla\cdot\mathbf E=\frac\rho{\epsilon_0},\qquad \boldsymbol\nabla\cdot\mathbf B=0,\qquad \boldsymbol\nabla\times\mathbf E=-\frac{\partial\mathbf B}{\partial t},\qquad \boldsymbol\nabla\times\mathbf B=\mu_0\mathbf J+\mu_0\epsilon_0\frac{\partial\mathbf E}{\partial t}.}
$$

The first is [Gauss's law](../../../../../gauss-s-law.md): [electric charge](../../../../../electric-charge-split.md) sources [electric flux](../../../../../electric-flux.md). The second is [Gauss's law for magnetism](../../../../../gauss-s-law-for-magnetism.md), expressing the absence of magnetic monopole sources in this theory. [Faraday's law](../../../../../faraday-s-law-of-induction.md) relates changing [magnetic flux](../../../../../magnetic-flux.md) to circulating [electric field](../../../../../electric-field-split.md). The [Ampere-Maxwell law](../../../../../ampere-s-circuital-law.md) relates magnetic circulation to both material current and changing [electric flux](../../../../../electric-flux.md).

For fixed loops and surfaces, the integral versions are

$$
\oint_{\partial\Omega}\mathbf E\cdot d\mathbf A=\frac{Q_{\mathrm{enc}}}{\epsilon_0},\quad \oint_{\partial\Omega}\mathbf B\cdot d\mathbf A=0,
$$



$$
\oint_{\partial S}\mathbf E\cdot d\mathbf l=-\frac d{dt}\int_S\mathbf B\cdot d\mathbf A,\quad \oint_{\partial S}\mathbf B\cdot d\mathbf l=\mu_0I_S+\mu_0\epsilon_0\frac d{dt}\int_S\mathbf E\cdot d\mathbf A.
$$

Surface and loop orientations are related by the right-hand rule. These forms follow from the divergence theorem and Stokes' theorem. In material media, equivalent macroscopic equations can separate free and bound sources using $\mathbf D$ and $\mathbf H$ together with constitutive relations; the displayed forms use total sources.

The displacement-current term is essential for [charge conservation](../../../../../charge-conservation.md). Taking the divergence of the last differential equation and using [Gauss's law](../../../../../gauss-s-law.md) gives $\partial_t\rho+\boldsymbol\nabla\cdot\mathbf J=0$. It also makes magnetic circulation consistent for surfaces spanning the same loop through either a charging capacitor's wire or its dielectric gap.

In source-free vacuum the [curl](../../../../../curl.md) equations combine to give $\nabla^2\mathbf E=\mu_0\epsilon_0\partial_t^2\mathbf E$, with the same equation for $\mathbf B$. Thus

$$
\boxed{c=\frac1{\sqrt{\mu_0\epsilon_0}}.}
$$

A plane wave is transverse, with $\mathbf E$, $\mathbf B$ and propagation direction mutually perpendicular and $E=cB$. The fields transport [energy](../../../../../energy-split.md) with density $u=\epsilon_0E^2/2+B^2/(2\mu_0)$ and [Poynting vector](../../../../../poynting-vector.md) $\mathbf S=\mathbf E\times\mathbf B/\mu_0$. Together with the [Lorentz force law](../../../../../lorentz-force.md), the equations connect charges, currents, forces, induction and electromagnetic radiation.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [15](../../15.md)
3. [Section E](../../../section-e.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
