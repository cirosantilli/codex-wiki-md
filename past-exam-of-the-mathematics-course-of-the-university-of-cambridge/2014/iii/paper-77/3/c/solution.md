<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a flat impermeable [free surface](../../../../../../free-surface.md) with zero tangential stress, the image of a parallel [stresslet](../../../../../../force-dipole-flow.md) is a [stresslet](../../../../../../force-dipole-flow.md) of the same strength and parallel orientation at the reflected point. Reflection makes the normal [velocity](../../../../../../velocity.md) odd and tangential [velocity](../../../../../../velocity.md) even across the plane, enforcing zero normal flow and zero tangential shear. This is the [free-surface image of a force dipole](../../../../../../free-surface-image-of-a-force-dipole.md); it is not the no-slip-wall image system.

The cell at $z=-h$ lies a distance $2h$ vertically below its image. Since $\mathbf e\cdot\mathbf r=0$ there, its induced vertical [velocity](../../../../../../velocity.md) is $S/(32\pi\mu h^2)$ towards the surface. There is no image-induced tangential [velocity](../../../../../../velocity.md), [vorticity](../../../../../../vorticity.md) or tangent-normal strain at this point, so a parallel orientation remains parallel in this idealization. Therefore the [finite-time free-surface approach of a point stresslet](../../../../../../finite-time-free-surface-approach-of-a-point-stresslet.md) is

$$
\boxed{\dot h=-\frac S{32\pi\mu h^2},\qquad
h(t)=\left(h_0^3-\frac{3S}{32\pi\mu}t\right)^{1/3},\qquad
t_* =\frac{32\pi\mu h_0^3}{3S}.}
$$

The trajectory combines its parallel self-propulsion with this normal drift. **Finite-time contact is the point-model prediction for $S>0$**, carried over from part (b). A puller with $S<0$ moves away instead. For a finite cell, the far-field approximation fails before $h$ reaches zero; surface deformation and near-contact physics can change the final encounter.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
