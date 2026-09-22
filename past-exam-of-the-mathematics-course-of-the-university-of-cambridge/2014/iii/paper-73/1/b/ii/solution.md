<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [minimum dissipation theorem](../../../../../../../minimum-dissipation-theorem-for-stokes-flow.md) fixes the boundary velocities and the far-field [velocity](../../../../../../../velocity.md): among admissible incompressible [velocity](../../../../../../../velocity.md) fields, the [Stokes flow](../../../../../../../stokes-flow-split.md) minimizes

$$
\mathcal D=2\mu\int\mathbf e:\mathbf e\,dV,
\qquad \mathbf e=\tfrac12(\nabla\mathbf u+\nabla\mathbf u^T).
$$

For a competitor $\mathbf u+\mathbf v$ with zero boundary data for $\mathbf v$, integration by parts eliminates the cross term and leaves $\mathcal D[\mathbf u+\mathbf v]-\mathcal D[\mathbf u]=2\mu\int\mathbf e(\mathbf v):\mathbf e(\mathbf v)\,dV\ge0$.

Extend the actual two-sphere [velocity](../../../../../../../velocity.md) rigidly through sphere 2. It is an admissible field in the one-sphere exterior, with the same translation and rotation of sphere 1. It is continuous across the filled boundary, incompressible, and adds zero strain dissipation inside. Applying the theorem to the exact isolated-sphere flow therefore gives

$$
\mathcal D_{\rm pair}\ge6\pi\mu a|\mathbf U_1|^2+8\pi\mu a^3|\boldsymbol\Omega_1|^2.
$$

With all applied couples and the second [force](../../../../../../../force.md) zero, the boundary-work identity is $\mathcal D_{\rm pair}=\mathbf F_1\cdot\mathbf U_1$. Thus $6\pi\mu a|\mathbf U_1|^2\le\mathbf F_1\cdot\mathbf U_1\le|\mathbf F_1||\mathbf U_1|$, which proves

$$
\boxed{\mathbf U_1\cdot\mathbf F_1\le\frac{|\mathbf F_1|^2}{6\pi\mu a}.}
$$

This [fixed-force comparison of minimum viscous dissipation](../../../../../../../fixed-force-comparison-of-minimum-viscous-dissipation.md) uses a comparison at fixed actual [velocity](../../../../../../../velocity.md) first; directly comparing different-force or different-velocity solutions would not justify the result.

If $\mathbf G_1\ne0$, the power is instead $\mathbf F_1\cdot\mathbf U_1+\mathbf G_1\cdot\boldsymbol\Omega_1$, so the preceding estimate no longer bounds the [force](../../../../../../../force.md) contribution alone. The two-sphere [hydrodynamic mobility matrix](../../../../../../../hydrodynamic-mobility-matrix.md) generally has a nonzero self translation-rotation coupling: the freely moving second sphere reflects the first sphere's torque field. In the planar geometry this coupling produces a [velocity](../../../../../../../velocity.md) perpendicular to $\mathbf R$; by choosing the sign and magnitude of the couple when the [force](../../../../../../../force.md) has a component in that direction, its contribution to $\mathbf F_1\cdot\mathbf U_1$ can exceed the isolated force-only value. **There is no universal force-only inequality with an additional applied couple.** Special geometries can eliminate the coupling, but do not restore a general theorem.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 73](../../../../paper-73-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
