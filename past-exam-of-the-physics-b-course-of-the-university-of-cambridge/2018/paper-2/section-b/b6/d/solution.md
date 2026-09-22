<h1 id="section-b/b6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The absence of magnetic monopoles is expressed by $\nabla\cdot\mathbf B=0$. In a regular simply connected region, a magnetic [vector](../../../../../../vector.md) potential may be introduced so that

$$
\boxed{\mathbf B=\nabla\times\mathbf A.}
$$

Its units are $\mathrm{T\,m}=\mathrm{Wb\,m^{-1}}$. It is not unique: adding a gradient leaves the [magnetic field](../../../../../../magnetic-field-split.md) unchanged because $\nabla\times\nabla\chi=0$. In time-dependent electromagnetism,

$$
\mathbf E=-\nabla\phi-\partial_t\mathbf A,
\qquad
\mathbf A\mapsto\mathbf A+\nabla\chi,\quad
\phi\mapsto\phi-\partial_t\chi
$$

is a [gauge transformation](../../../../../../gauge-transformation.md) preserving both physical fields. [Stokes theorem](../../../../../../stokes-theorem.md) gives $\oint_C\mathbf A\cdot d\boldsymbol\ell=\int_S\mathbf B\cdot d\mathbf S=\Phi_B$ for a contour bounding an appropriate surface.

For localized steady currents, choose the [Coulomb gauge](../../../../../../coulomb-gauge.md) $\nabla\cdot\mathbf A=0$. Substitution into [Ampère's law](../../../../../../ampere-s-circuital-law.md) and the curl-of-curl identity gives

$$
-\nabla^2\mathbf A=\mu_0\mathbf J,
\qquad
\mathbf A(\mathbf r)=\frac{\mu_0}{4\pi}\int\frac{\mathbf J(\mathbf r')}{|\mathbf r-\mathbf r'|}\,d^3r'.
$$

[Boundary conditions](../../../../../../boundary-condition.md) are needed in addition to the gauge choice. For a uniform [magnetic field](../../../../../../magnetic-field-split.md) one convenient choice is $\mathbf A=\tfrac12\mathbf B\times\mathbf r$. For a magnetic dipole, $\mathbf A=\mu_0\mathbf m\times\mathbf r/(4\pi r^3)$ outside its source. The magnetic [vector](../../../../../../vector.md) potential simplifies field calculations and appears directly in the [Lagrangian](../../../../../../lagrangian.md) of a charged particle, $L=\tfrac12m v^2+q\mathbf v\cdot\mathbf A-q\phi$. In multiply connected regions, a field-free region can retain nontrivial circulation of $\mathbf A$, relevant to the [Aharonov-Bohm effect](../../../../../../aharonov-bohm-effect.md); a local gauge argument cannot remove every global circulation.

## ↑ Ancestors (15)

1. [D](../d.md)
2. [B6](../../b6.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2018](../../../../split.md)
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
