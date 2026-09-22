<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write horizontal components with a subscript $h$. The steady [ideal magnetohydrodynamic induction equation](../../../../../../ideal-magnetohydrodynamic-induction-equation.md) gives $\nabla\times(\mathbf u\times\mathbf B)=0$. Since $\partial_z=0$, its horizontal components imply

$$
\partial_x(\mathbf u\times\mathbf B)_z=\partial_y(\mathbf u\times\mathbf B)_z=0.
$$

Thus $(\mathbf u\times\mathbf B)_z=C$ is a spatial constant. A vanishing axial [electric field](../../../../../../electric-field.md), $E_z=-C=0$, is needed to infer horizontal alignment. It is satisfied, for example, if the constant electric field vanishes at a boundary or at infinity. With this additional condition and $\mathbf B_h\ne0$, define the [magnetohydrodynamic mass loading](../../../../../../magnetohydrodynamic-mass-loading.md) $k$ by $\rho\mathbf u_h=k\mathbf B_h$, and put $U=u_z-kB_z/\rho$. Then

$$
\boxed{\mathbf u=\frac{k\mathbf B}{\rho}+U\mathbf e_z}.
$$

The steady [continuity equation](../../../../../../continuity-equation.md) and the [solenoidal magnetic-field constraint](../../../../../../solenoidal-magnetic-field-constraint.md) give

$$
0=\nabla\cdot(\rho\mathbf u)=\nabla\cdot(k\mathbf B+\rho U\mathbf e_z)=\mathbf B\cdot\nabla k.
$$

Also $\mathbf u\times\mathbf B=U\mathbf e_z\times\mathbf B$. Using the vector identity for the curl of a cross product, together with $\partial_z\mathbf B=0$ and $\nabla\cdot\mathbf B=0$, its curl is $\mathbf e_z\mathbf B\cdot\nabla U$. Hence

$$
\boxed{\mathbf B\cdot\nabla k=\mathbf B\cdot\nabla U=0}.
$$

These are [steady planar ideal-MHD field-line invariants](../../../../../../steady-planar-ideal-mhd-field-line-invariants.md): both quantities are constant along a [magnetic field line](../../../../../../magnetic-field-line.md).

The zero-electric-field condition does not follow from the printed stationarity assumptions alone. Constant $\rho,p,s$, $\Phi=0$, $\mathbf u=u_0\mathbf e_x$ and $\mathbf B=B_0\mathbf e_y$, with $u_0B_0\ne0$, satisfy every displayed [ideal magnetohydrodynamics](../../../../../../ideal-magnetohydrodynamics.md) equation but have perpendicular horizontal velocity and magnetic field. Their $C=u_0B_0$ is nonzero, so no $k,U$ give the stated decomposition. **The field-line decomposition is valid on the $E_z=0$ branch; as an unrestricted implication, the first claim has this counterexample**. The subsequent calculations use that branch.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
