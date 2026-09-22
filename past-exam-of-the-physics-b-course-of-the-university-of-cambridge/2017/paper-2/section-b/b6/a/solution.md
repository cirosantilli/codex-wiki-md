<h1 id="section-b/b6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Maxwell's [displacement current](../../../../../../displacement-current.md) is the electric-field contribution needed to make [Ampère's law](../../../../../../ampere-s-circuital-law.md) consistent with [charge conservation](../../../../../../charge-conservation.md). In macroscopic form,

$$
\boxed{\nabla\times\mathbf H=\mathbf J_f+\frac{\partial\mathbf D}{\partial t}.}
$$

The [displacement current](../../../../../../displacement-current.md) density $\mathbf J_d=\partial_t\mathbf D$ has units $\mathrm{A\,m^{-2}}$. Since $\mathbf D=\epsilon_0\mathbf E+\mathbf P$, it contains the [vacuum](../../../../../../vacuum.md) field term and, in matter, the polarization-current contribution. It need not represent [free charge](../../../../../../free-charge.md) moving through a material.

Taking the [divergence](../../../../../../divergence.md) gives $0=\nabla\cdot\mathbf J_f+\partial_t(\nabla\cdot\mathbf D)$. [Gauss's law](../../../../../../gauss-s-law.md), $\nabla\cdot\mathbf D=\rho_f$, then yields the [continuity equation](../../../../../../continuity-equation.md) $\partial_t\rho_f+\nabla\cdot\mathbf J_f=0$. Without the [displacement](../../../../../../displacement.md) term, Ampère's original law would incorrectly require every current distribution to be divergence-free even while charge accumulates.

A charging parallel-plate [capacitor](../../../../../../capacitor.md) makes this concrete. Ignoring fringing, $D=Q/A$, so the [displacement current](../../../../../../displacement-current.md) across its [dielectric](../../../../../../dielectric.md) gap is $I_d=A\partial_tD=dQ/dt$, equal to the conduction [electric current](../../../../../../electric-current.md) in its wire. The [integral](../../../../../../integral-split.md) law

$$
\oint\mathbf H\cdot d\boldsymbol\ell
=\int_S\mathbf J_f\cdot d\mathbf S+\frac{d}{dt}\int_S\mathbf D\cdot d\mathbf S
$$

therefore gives the same answer whether the spanning surface cuts the wire or passes through the gap. Together with [Faraday's law](../../../../../../faraday-s-law-of-induction.md), this field term also permits self-consistent [electromagnetic waves](../../../../../../electromagnetic-wave-split.md) in [vacuum](../../../../../../vacuum.md), with [speed](../../../../../../speed.md) $c=1/\sqrt{\mu_0\epsilon_0}$.

## ↑ Ancestors (15)

1. [A](../a.md)
2. [B6](../../b6.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
