<h1 id="section-b/b7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because the [magnetic field](../../../../../../magnetic-field-split.md) obeys $\nabla\cdot\mathbf B=0$, it can be represented locally as the [curl](../../../../../../curl.md) of a [magnetic vector potential](../../../../../../magnetic-vector-potential.md):

$$
\boxed{\mathbf B=\nabla\times\mathbf A.}
$$

This automatically enforces the absence of magnetic monopoles. It is also a global representation throughout ordinary all-space problems without monopole singularities. It is not unique: the [gauge transformation](../../../../../../gauge-transformation.md)

$$
\mathbf A\longmapsto\mathbf A+\nabla\chi
$$

leaves $\mathbf B$ unchanged because the [curl](../../../../../../curl.md) of a [gradient](../../../../../../gradient.md) vanishes. In a time-dependent problem,

$$
\mathbf E=-\nabla\phi-\frac{\partial\mathbf A}{\partial t},\qquad
\phi\longmapsto\phi-\frac{\partial\chi}{\partial t}
$$

makes the same transformation leave both physical fields unchanged and automatically satisfies [Faraday's law](../../../../../../faraday-s-law-of-induction.md).

In vacuum [magnetostatics](../../../../../../magnetostatics.md), choose the [Coulomb gauge](../../../../../../coulomb-gauge.md) $\nabla\cdot\mathbf A=0$. Substitution into [Ampère's law](../../../../../../ampere-s-circuital-law.md) and the identity $\nabla\times(\nabla\times\mathbf A)=\nabla(\nabla\cdot\mathbf A)-\nabla^2\mathbf A$ gives

$$
\nabla^2\mathbf A=-\mu_0\mathbf J,\qquad
\mathbf A(\mathbf r)=\frac{\mu_0}{4\pi}\int\frac{\mathbf J(\mathbf r')}{|\mathbf r-\mathbf r'|}\,d^3r'
$$

for a localized steady [electric current density](../../../../../../current-density.md) and a potential vanishing at infinity. Taking the [curl](../../../../../../curl.md) recovers the [Biot-Savart law](../../../../../../biot-savart-law.md). The [magnetic vector potential](../../../../../../magnetic-vector-potential.md) converts a constrained [vector](../../../../../../vector.md) field problem into componentwise [Poisson equations](../../../../../../poisson-s-equation.md) once a gauge is chosen.

For a uniform [magnetic field](../../../../../../magnetic-field-split.md), $\mathbf A=\tfrac12\mathbf B\times\mathbf r$ is a convenient choice. For a localized [magnetic dipole moment](../../../../../../magnetic-dipole-moment.md) $\mathbf m$, the leading far-field potential is

$$
\mathbf A(\mathbf r)=\frac{\mu_0}{4\pi}\frac{\mathbf m\times\mathbf r}{r^3}.
$$

Another useful relation is [Stokes theorem](../../../../../../stokes-theorem.md), which relates a closed-path [integral](../../../../../../integral-split.md) to the [magnetic flux](../../../../../../magnetic-flux.md) through a spanning surface:

$$
\oint_{\partial S}\mathbf A\cdot d\boldsymbol\ell=\int_S\mathbf B\cdot d\mathbf S.
$$

The units of $\mathbf A$ are $\mathrm{T\,m}$, equivalently $\mathrm{Wb\,m^{-1}}$.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [B7](../../b7.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
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
