<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Away from the axis, [cylindrical coordinates](../../../../../cylindrical-coordinate-system.md) put the field in the [line vortex](../../../../../line-vortex.md) form

$$
\mathbf v=\frac{\kappa}{2\pi\rho}\mathbf e_\phi.
$$

The only potentially nonzero component of its [curl](../../../../../curl.md) is

$$
(\nabla\times\mathbf v)_z=\frac1\rho\frac{\partial}{\partial\rho}(\rho v_\phi)=\frac1\rho\frac{\partial}{\partial\rho}\frac\kappa{2\pi}=0.
$$

The other components vanish because there is no axial dependence and no radial or axial velocity. Thus **the [curl](../../../../../curl.md) is zero for $\rho>0$**; the field is singular on the axis, so a classical [curl](../../../../../curl.md) there is not defined.

For a spanning surface avoiding that axis, the smoothness hypotheses of [Stokes theorem](../../../../../stokes-theorem.md) hold and give $\oint_C\mathbf v\cdot d\mathbf r=0$. If the enclosed planar region contains the axis, the singularity prevents applying that theorem directly. Excise a small disk about the origin. The resulting annulus has zero [curl](../../../../../curl.md), so its outer [circulation](../../../../../circulation-physics.md) equals the counterclockwise circulation on the small circle:

$$
\boxed{\oint_C\mathbf v\cdot d\mathbf r=\int_0^{2\pi}\frac{\kappa}{2\pi\rho}\rho\,d\phi=\kappa.}
$$

This sign assumes positive, counterclockwise orientation. Clockwise orientation gives $-\kappa$; more generally the value is $\kappa$ times the [winding number](../../../../../winding-number.md) about the origin. A curve through the origin is excluded because its integral is singular. In the [distribution](../../../../../distribution-mathematical-analysis.md) interpretation the missing [vorticity](../../../../../vorticity-split.md) is concentrated on the axis as $\kappa\delta(x)\delta(y)\mathbf e_z$, explaining the nonzero circulation despite zero classical [curl](../../../../../curl.md) away from it.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
