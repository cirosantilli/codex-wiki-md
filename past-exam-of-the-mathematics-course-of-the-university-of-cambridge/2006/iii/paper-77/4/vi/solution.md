<h1 id="4/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

[Potential-vorticity conservation](../../../../../../potential-vorticity-conservation.md) makes the evolving PV distribution a set of parcel-carried labels. In the ideal model it can be rearranged into filaments and complicated geometry, but it is not created or destroyed by advection. Apparent homogenization, such as that assumed for the shallow-water experiment, describes a coarse-grained mixed distribution rather than pointwise destruction of materially conserved PV.

Within a balanced regime, [potential-vorticity inversion](../../../../../../potential-vorticity-inversion.md) turns those labels and the boundary data into a [velocity](../../../../../../velocity.md) field. This makes understanding a flow a coupled geometric problem: determine how PV is rearranged, invert the resulting distribution, and use the recovered [velocity](../../../../../../velocity.md) to find the next rearrangement. Inversion is nonlocal, so a compact PV anomaly influences fluid well outside its support, as the spherical example explicitly demonstrates.

The [quasi-geostrophic potential-vorticity equation](../../../../../../quasi-geostrophic-potential-vorticity-equation.md) has only one time derivative:

$$
\partial_tQ+J(\psi,Q)=0,\qquad
J(\psi,Q)=\psi_xQ_y-\psi_yQ_x,\qquad\nabla_*^2\psi=Q-f.
$$

**An initial PV field and the inversion data determine the balanced evolution; an independent initial acceleration is not needed.** [Pressure](../../../../../../pressure.md), [buoyancy](../../../../../../buoyancy.md) and the leading [velocity](../../../../../../velocity.md) are diagnosed from that field at each instant. This reduced initial-data requirement reflects the removal of freely oscillating inertia-gravity waves, which in the full fluid equations require additional initial information. The principles are consequently powerful for slow large-scale flow, but do not recover every unbalanced motion or remove the need to state [boundary conditions](../../../../../../boundary-condition.md) and the balance approximation.

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [4](../../4.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
