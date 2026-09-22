<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Given an admissible [velocity field](../../../../velocity-field.md), recover the [pressure gradient](../../../../pressure-gradient.md) from the [Stokes equation](../../../../stokes-equation.md), $\nabla p=\mu\nabla^2\mathbf v$, and integrate it, fixing the additive constant by matching to the bath [pressure](../../../../pressure-split.md) near the open ends. The [biharmonic equation](../../../../biharmonic-equation.md) ensures the compatibility of this integration. For a freely moving hinge, the laboratory [velocity field](../../../../velocity-field.md) also contains the unknown rigid translation and rotation. Solve the interior and exterior [Stokes flows](../../../../stokes-flow-split.md) with these wall [velocities](../../../../velocity.md), then impose zero total external [force](../../../../force-split.md) and [torque](../../../../torque.md) on the complete apparatus if its motor supplies only internal actuation. The pinned solution alone cannot determine that free motion.

At a fixed angle, the actuation [velocity](../../../../velocity.md) scale is $U\sim L|\dot\alpha|$. The [Stokes equation](../../../../stokes-equation.md) gives $\Delta p\sim\mu U/L\sim\mu|\dot\alpha|$. Integrating normal [traction](../../../../traction.md) over a plate of [length](../../../../length.md) $L$ gives a [force](../../../../force-split.md) per unit width of scale

$$
\boxed{F=\mu L\dot\alpha\,C(\alpha),}
$$

with a dimensionless signed coefficient depending on geometry and exterior matching. Normal [viscous stress](../../../../viscous-stress-tensor.md) has the same dimensional scale and is included in $C$. The [force](../../../../force-split.md) reverses when the actuation reverses. A narrow gap can make $|C|$ large.

More specifically, the corrected local [streamfunction](../../../../stream-function.md) gives, up to a reference [pressure](../../../../pressure-split.md),

$$
p=\mu\dot\alpha\,K(\alpha)\log(r/r_*)+\text{constant},\qquad
K(\alpha)=\frac{2\cos\alpha}{\sin\alpha-\alpha\cos\alpha}.
$$

Indeed, inserting $\mathbf v=(-\dot\alpha rG'/2,\dot\alpha rG)$ into the vector [Laplacian](../../../../laplacian.md) gives $p_r=-\mu\dot\alpha(G'''+4G')/(2r)=\mu\dot\alpha K/r$ and $p_\theta=0$. For $\alpha<\pi/2$, opening produces reduced [pressure](../../../../pressure-split.md) toward the hinge when matched at $r_*\sim L$. The logarithmic singularity is integrable: $\int_0^L\log(L/r)\,dr=L$, consistent with the stated [force](../../../../force-split.md) scale. A real hinge regularizes the singularity; the local formula is not a full end-matched solution.

The [scallop theorem](../../../../scallop-theorem.md) applies to a single periodically actuated hinge in a stationary [Newtonian fluid](../../../../newtonian-fluid.md) with negligible fluid and body [inertia](../../../../inertia.md). At each shape, [Linearity of Stokes flow](../../../../linearity-of-stokes-flow.md) makes its rigid [velocity](../../../../velocity.md) proportional to $\dot\alpha$. Closing retraces the sequence of shapes and reverses the corresponding motion, irrespective of different opening and closing rates. The hinge may move during each half-cycle, but

$$
\boxed{\text{net rigid displacement and rotation over a reciprocal cycle}=0.}
$$

A motor can generate instantaneous [forces](../../../../force-split.md) and consume [energy](../../../../energy-split.md) through [viscous dissipation](../../../../viscous-dissipation.md) without producing sustained swimming. Additional independently controlled shape changes, appreciable [inertia](../../../../inertia.md), or a fluid with memory would require a different analysis.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the fluids course of the University of Oxford](../../../split.md)
5. [Fluids course of the University of Oxford](../../../../fluids-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
