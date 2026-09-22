<h1 id="section-a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

This is [magnetic flux freezing](../../../../magnetic-flux-freezing.md) in [ideal magnetohydrodynamics](../../../../ideal-magnetohydrodynamics-split.md). In addition to the supplied [ideal magnetohydrodynamic induction equation](../../../../ideal-magnetohydrodynamic-induction-equation.md), a physical [magnetic field](../../../../magnetic-field-split.md) obeys [Gauss's law for magnetism](../../../../gauss-s-law-for-magnetism.md), $\nabla\cdot\mathbf B=0$.

Parameterize the [material surface](../../../../material-surface.md) by two particle labels $a,b$, so $d\mathbf S=(\partial_a\mathbf x\times\partial_b\mathbf x)\,da\,db$ and $D\mathbf x/Dt=\mathbf u$. Differentiating these tangents gives the [material surface element evolution](../../../../material-surface-element-evolution.md) law

$$
\frac D{Dt}d\mathbf S=
\left[(\nabla\cdot\mathbf u)\mathsf I-(\nabla\mathbf u)^{\mathsf T}\right]d\mathbf S,
$$

where $(\nabla\mathbf u)_{ij}=\partial_j u_i$. Thus the [material magnetic-flux transport theorem](../../../../material-magnetic-flux-transport-theorem.md) is

$$
\frac D{Dt}\int_{S(t)}\mathbf B\cdot d\mathbf S
=\int_{S(t)}\left[\frac{D\mathbf B}{Dt}
+\mathbf B(\nabla\cdot\mathbf u)-(\mathbf B\cdot\nabla)\mathbf u\right]\cdot d\mathbf S.
$$

Expand the [curl](../../../../curl.md) in the [ideal magnetohydrodynamic induction equation](../../../../ideal-magnetohydrodynamic-induction-equation.md):

$$
\partial_t\mathbf B=(\mathbf B\cdot\nabla)\mathbf u-(\mathbf u\cdot\nabla)\mathbf B
-\mathbf B(\nabla\cdot\mathbf u)+\mathbf u(\nabla\cdot\mathbf B).
$$

Since $D/Dt=\partial_t+\mathbf u\cdot\nabla$ is the [material derivative](../../../../material-derivative.md), the first three terms cancel the corresponding terms in the surface transport formula. The remaining integrand is $\mathbf u\,\nabla\cdot\mathbf B=0$. Therefore

$$
\boxed{\frac D{Dt}\int_{S(t)}\mathbf B\cdot d\mathbf S=0.}
$$

No [incompressible flow](../../../../incompressible-flow.md) assumption is needed: the changing [surface](../../../../topological-surface-split.md) area cancels the compression term. This proof assumes smooth [velocity](../../../../velocity.md) and [magnetic field](../../../../magnetic-field-split.md) and a surface carried with the fluid; the [ideal magnetohydrodynamic induction equation](../../../../ideal-magnetohydrodynamic-induction-equation.md) by itself, for an arbitrary non-solenoidal [vector field](../../../../vector-field.md), would leave the final divergence term.

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Section A](../../section-a.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../../split.md)
5. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../../../astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
