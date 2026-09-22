<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For rotation about the [hydrodynamic centre of a two-sphere dumbbell](../../../../hydrodynamic-centre-of-a-two-sphere-dumbbell.md), the sphere centres have [velocities](../../../../velocity.md) $\mathbf v_i=\boldsymbol\Omega\times(\mathbf r_i-\mathbf r_c)$. Their resultant drag [force](../../../../force-split.md) in the [free-draining approximation](../../../../free-draining-approximation.md) is

$$
\mathbf F=-\sum_i\zeta_i\boldsymbol\Omega\times(\mathbf r_i-\mathbf r_c)
=-\boldsymbol\Omega\times\left(\sum_i\zeta_i\mathbf r_i-(\zeta_1+\zeta_2)\mathbf r_c\right)
=\boxed{\mathbf0.}
$$

Each sphere also experiences a spin drag [torque](../../../../torque.md), but its isolated rotation causes no net [force](../../../../force-split.md). Those spin contributions therefore do not alter the cancellation.

This illustrates [translation-rotation reciprocal coupling](../../../../translation-rotation-reciprocal-coupling.md). About any fixed origin, write the fluid's rigid-body [force](../../../../force-split.md) and [torque](../../../../torque.md) as

$$
\begin{pmatrix}\mathbf F\\\mathbf T\end{pmatrix}=-\begin{pmatrix}A&B\\B^T&C\end{pmatrix}\begin{pmatrix}\mathbf U\\\boldsymbol\Omega\end{pmatrix}.
$$

The transposed cross-blocks follow from the [Lorentz reciprocal theorem](../../../../lorentz-reciprocal-theorem-for-stokes-flow.md). If pure translation causes zero [torque](../../../../torque.md) about an origin for every $\mathbf U$, then $B^T=0$, hence pure rotation about that origin causes zero [force](../../../../force-split.md). This implication is general for linear [Stokes flow](../../../../stokes-flow-split.md); the existence and leading location of such an origin here use the two-sphere geometry and the approximation in part [c](../c.md).

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
