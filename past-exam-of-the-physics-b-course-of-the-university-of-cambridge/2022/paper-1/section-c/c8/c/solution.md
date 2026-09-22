<h1 id="section-c/c8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [divergence](../../../../../../divergence.md) identity for a [cross product](../../../../../../cross-product.md), followed by [Faraday's law of induction](../../../../../../faraday-s-law-of-induction.md) and the [Ampère-Maxwell equation](../../../../../../ampere-s-circuital-law.md):

$$
\nabla\cdot(\mathbf E\times\mathbf H)
=\mathbf H\cdot(\nabla\times\mathbf E)-\mathbf E\cdot(\nabla\times\mathbf H),
$$



$$
\nabla\times\mathbf E=-\mu_0\frac{\partial\mathbf H}{\partial t},\qquad
\nabla\times\mathbf H=\mathbf J+\epsilon_0\frac{\partial\mathbf E}{\partial t}.
$$

With the [electromagnetic energy](../../../../../../electromagnetic-energy.md) density of part (b), these give

$$
\nabla\cdot\mathbf N
=-\mathbf E\cdot\mathbf J-\mu_0\mathbf H\cdot\partial_t\mathbf H-\epsilon_0\mathbf E\cdot\partial_t\mathbf E
=-\mathbf E\cdot\mathbf J-\frac{\partial U}{\partial t}.
$$

Integrate over a fixed volume $V$ and apply the [divergence theorem](../../../../../../divergence-theorem.md), choosing $d\mathbf S$ outward:

$$
\boxed{\oint_S\mathbf N\cdot d\mathbf S
=-\int_V\mathbf E\cdot\mathbf J\,dV-\frac d{dt}\int_VU\,dV.}
$$

This is [Poynting's theorem](../../../../../../poynting-theorem.md). The outward [electromagnetic energy](../../../../../../electromagnetic-energy.md) flux equals minus the [power](../../../../../../power.md) transferred to matter and minus the rate at which [electromagnetic energy](../../../../../../electromagnetic-energy.md) accumulates inside. For the dissipative [electrical conductor](../../../../../../electrical-conductor.md) in this question, the matter term is [Ohmic heating](../../../../../../joule-heating.md).

## ↑ Ancestors (15)

1. [C](../c.md)
2. [C8](../../c8.md)
3. [Section C](../../../section-c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2022](../../../../split.md)
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
