<h1 id="section-a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The first argument mixes a material [fluid element](../../../../fluid-element.md) with a fixed spatial volume. For a [material volume element](../../../../material-volume-element.md) following the fluid, its volume is generally time dependent:

$$
\frac D{Dt}\delta V=(\nabla\cdot\mathbf u)\delta V.
$$

Therefore the [material derivative](../../../../material-derivative.md) cannot be taken outside the product with $\delta V$ as in the proposed cancellation. Instead, [mass conservation](../../../../mass-conservation.md) states

$$
\frac D{Dt}(\rho\delta V)=0,\qquad
\frac{D\rho}{Dt}=-\rho\nabla\cdot\mathbf u.
$$

The [momentum balance for a material fluid element](../../../../momentum-balance-for-a-material-fluid-element.md), using [Newton's second law](../../../../newton-s-second-law.md), is consequently

$$
\frac D{Dt}(\rho\delta V\,\mathbf u)
=(\rho\delta V)\frac{D\mathbf u}{Dt}
=-\nabla p\,\delta V,
\qquad
\boxed{\rho\frac{D\mathbf u}{Dt}=-\nabla p.}
$$

For a fixed [control volume](../../../../control-volume.md), fluid crosses its boundary and carries [momentum](../../../../momentum-split.md); a [momentum flux](../../../../momentum-flux.md) term must be included. Its local conservative form is $\partial_t(\rho\mathbf u)+\nabla\cdot(\rho\mathbf u\otimes\mathbf u)=-\nabla p$, equivalent to the displayed [Euler equations](../../../../euler-equations-for-an-inviscid-fluid-split.md) after using the [continuity equation](../../../../continuity-equation.md). The erroneous equation omits the term $\rho\mathbf u\nabla\cdot\mathbf u$ needed to convert a material derivative of momentum density into this conservative form.

For the second task, take a homogeneous fluid with constant [mass density](../../../../density.md) $\rho$, prescribed gravitational [acceleration](../../../../acceleration.md) $\mathbf g$, [incompressible flow](../../../../incompressible-flow.md) and [inviscid flow](../../../../inviscid-flow.md). Its equations are

$$
\frac{D\mathbf u}{Dt}=-\nabla\left(\frac p\rho\right)+\mathbf g,\qquad\nabla\cdot\mathbf u=0.
$$

Under the replacement $\rho\mapsto\widetilde\rho=C\rho$, the same [velocity](../../../../velocity.md) solves these equations if $p\mapsto\widetilde p=Cp$, up to a spatially constant pressure offset. This is [density scaling invariance of incompressible Euler flow](../../../../density-scaling-invariance-of-incompressible-euler-flow.md):

$$
\boxed{\text{The velocity field alone cannot determine the uniform fluid density.}}
$$

The comparison assumes the same geometry and compatible velocity or gravitational [free surface](../../../../free-surface.md) conditions; an independently specified nonuniform boundary [pressure](../../../../pressure-split.md) would supply additional information. The [gravitational field](../../../../gravitational-field.md) is taken as prescribed. If the fluid's own [self-gravity](../../../../self-gravity.md) must be included, its field changes with [mass density](../../../../density.md), so the invariance need not hold. A single freely moving particle's density-independent gravitational acceleration does not justify neglecting that distinction.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Section A](../../section-a.md)
3. [2021](../../../2021-split.md)
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
