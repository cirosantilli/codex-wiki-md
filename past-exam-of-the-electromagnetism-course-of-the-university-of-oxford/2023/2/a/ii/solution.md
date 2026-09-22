<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Allow time dependence while keeping the [constitutive relations](../../../../../constitutive-relations.md) linear, isotropic, nondispersive, and independent of time. The [Maxwell equations in matter](../../../../../maxwell-equations-in-matter.md) give

$$
\nabla\times\mathbf E=-\partial_t\mathbf B,\qquad
\nabla\times\mathbf H=\mathbf J_f+\partial_t\mathbf D.
$$

For the [Poynting vector](../../../../../poynting-vector.md) $\boldsymbol{\mathcal P}=\mathbf E\times\mathbf H$, the [divergence](../../../../../divergence.md) identity yields

$$
\begin{aligned}
\nabla\cdot\boldsymbol{\mathcal P}
&=\mathbf H\cdot(\nabla\times\mathbf E)-\mathbf E\cdot(\nabla\times\mathbf H)\\
&=-\frac1\mu\mathbf B\cdot\partial_t\mathbf B
-\epsilon\mathbf E\cdot\partial_t\mathbf E-\mathbf E\cdot\mathbf J_f.
\end{aligned}
$$

The first two terms are exact time [derivatives](../../../../../derivative.md). Taking the zero-field [energy density](../../../../../energy-density.md) as zero gives the [electromagnetic energy density](../../../../../electromagnetic-energy-density.md)

$$
\boxed{\mathcal E=\frac12\epsilon|\mathbf E|^2+\frac1{2\mu}|\mathbf B|^2
=\frac12(\mathbf E\cdot\mathbf D+\mathbf B\cdot\mathbf H).}
$$

Consequently the [Poynting theorem](../../../../../poynting-theorem.md) is the [continuity equation](../../../../../continuity-equation.md)

$$
\boxed{\partial_t\mathcal E+\nabla\cdot\boldsymbol{\mathcal P}=-\mathbf J_f\cdot\mathbf E.}
$$

In integral form,

$$
\frac d{dt}\int_W\mathcal E\,d^3r+
\oint_{\partial W}\boldsymbol{\mathcal P}\cdot\mathbf n\,dS
=-\int_W\mathbf J_f\cdot\mathbf E\,d^3r.
$$

The left side is the rate of increase of stored [electromagnetic energy](../../../../../electromagnetic-energy.md) plus outward [Poynting flux](../../../../../poynting-flux.md). The right side accounts for work delivered to the free [electric current](../../../../../electric-current.md); in an Ohmic medium $\mathbf J_f\cdot\mathbf E$ is the local rate of [Joule heating](../../../../../joule-heating.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the electromagnetism course of the University of Oxford](../../../../split.md)
6. [Electromagnetism course of the University of Oxford](../../../../../electromagnetism-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
