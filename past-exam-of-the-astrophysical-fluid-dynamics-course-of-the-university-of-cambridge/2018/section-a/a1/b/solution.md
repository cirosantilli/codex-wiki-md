<h1 id="section-a/a1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the nonrelativistic moving-conductor Ohm law in the form

$$
\mathbf E=\frac{\mathbf j}{\sigma}-\mathbf u\times\mathbf B.
$$

The [Maxwell equations](../../../../../maxwell-equations-split.md) give [Faraday's law of induction](../../../../../faraday-s-law-of-induction.md), $\partial_t\mathbf B=-\nabla\times\mathbf E$. For a nonmagnetic conductor with constant permeability $\mu_0$, the quasistatic [Ampere-Maxwell law](../../../../../ampere-s-circuital-law.md) gives $\mathbf j\simeq(\nabla\times\mathbf B)/\mu_0$. This step neglects [displacement current](../../../../../displacement-current.md), requiring it to be small compared with conduction current; nonrelativistic velocity alone is not the complete justification.

For spatially uniform scalar [electrical conductivity](../../../../../electrical-conductivity.md) $\sigma$,

$$
\partial_t\mathbf B
=\nabla\times(\mathbf u\times\mathbf B)
-\frac{1}{\mu_0\sigma}\nabla\times(\nabla\times\mathbf B).
$$

Apply the identity $\nabla\times(\nabla\times\mathbf B)=\nabla(\nabla\cdot\mathbf B)-\nabla^2\mathbf B$ and [Gauss's law for magnetism](../../../../../gauss-s-law-for-magnetism.md), $\nabla\cdot\mathbf B=0$. The [resistive induction equation](../../../../../resistive-induction-equation.md) is

$$
\boxed{\frac{\partial\mathbf B}{\partial t}
\simeq\nabla\times(\mathbf u\times\mathbf B)
+\eta\nabla^2\mathbf B,\qquad
\eta=\frac1{\mu_0\sigma}.}
$$

The first term transports and deforms the [magnetic field](../../../../../magnetic-field-split.md) with the moving fluid; the second diffuses it. The [magnetic diffusivity](../../../../../magnetic-diffusivity.md) $\eta$ has units $\mathrm{m^2\,s^{-1}}$, so both terms have units tesla per second. No assumption of [incompressible flow](../../../../../incompressible-flow.md) was needed. If $\sigma$ varies spatially, the [conductivity-gradient term in magnetic induction](../../../../../conductivity-gradient-term-in-magnetic-induction.md), $-\nabla\eta\times(\nabla\times\mathbf B)$, must also be retained.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [A1](../../a1.md)
3. [Section A](../../../section-a.md)
4. [2018](../../../../2018-split.md)
5. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../../../split.md)
6. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../../../../astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
