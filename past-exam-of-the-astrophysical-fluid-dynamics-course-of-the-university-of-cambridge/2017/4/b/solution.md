<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The surface must be a **material surface $S(t)$**, moving with the fluid; its boundary moves with it as well. The stated [barotropic vorticity transport](../../../../barotropic-vorticity-transport.md) law, with $\boldsymbol\omega=\boldsymbol\nabla\times\mathbf v$, gives $\boldsymbol\nabla\cdot\boldsymbol\omega=0$. Expanding its curl therefore yields

$$
\frac{D\boldsymbol\omega}{Dt}
=(\boldsymbol\omega\cdot\boldsymbol\nabla)\mathbf v
-\boldsymbol\omega(\boldsymbol\nabla\cdot\mathbf v).
$$

A material tangent vector $\mathbf t$ obeys $D\mathbf t/Dt=(\boldsymbol\nabla\mathbf v)\mathbf t$. Apply the [product rule](../../../../product-rule.md) to the [cross product](../../../../cross-product.md) of two such tangents to obtain [material surface element evolution](../../../../material-surface-element-evolution.md):

$$
\frac{D(d\mathbf S)}{Dt}
=\left[(\boldsymbol\nabla\cdot\mathbf v)I-(\boldsymbol\nabla\mathbf v)^{\mathsf T}\right]d\mathbf S.
$$

Here $(\boldsymbol\nabla\mathbf v)_{ij}=\partial_jv_i$. The stretching and area-change terms cancel exactly in the transported flux element:

$$
\begin{aligned}
\frac D{Dt}(\boldsymbol\omega\cdot d\mathbf S)
&=\big[(\boldsymbol\omega\cdot\boldsymbol\nabla)\mathbf v
-\boldsymbol\omega\boldsymbol\nabla\cdot\mathbf v\big]\cdot d\mathbf S\\
&\quad+\boldsymbol\omega\cdot
\big[(\boldsymbol\nabla\cdot\mathbf v)I-(\boldsymbol\nabla\mathbf v)^{\mathsf T}\big]d\mathbf S
=0.
\end{aligned}
$$

Integrate over the fixed particle labels parameterizing the material surface. This proves the [conservation of vorticity flux through a material surface](../../../../conservation-of-vorticity-flux-through-a-material-surface.md):

$$
\boxed{\frac d{dt}\int_{S(t)}\boldsymbol\omega\cdot d\mathbf S=0.}
$$

The conserved flux is also the [circulation](../../../../circulation-physics.md) $\oint_{\partial S(t)}\mathbf v\cdot d\boldsymbol\ell$ by the [Stokes theorem](../../../../stokes-theorem.md), so this agrees with [Kelvin's circulation theorem](../../../../kelvin-s-circulation-theorem.md). The assumptions are smooth inviscid barotropic flow and conservative body forces. A fixed open surface generally exchanges vorticity flux with its surroundings and does not satisfy this conservation statement; compressibility by itself does not invalidate the material-surface result.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [2017](../../../2017-split.md)
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
