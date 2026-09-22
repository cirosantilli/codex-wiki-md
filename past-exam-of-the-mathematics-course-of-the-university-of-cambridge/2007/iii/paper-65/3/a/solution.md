<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use a steady [axisymmetric flow](../../../../../../axisymmetric-flow.md) governed by [ideal magnetohydrodynamics](../../../../../../ideal-magnetohydrodynamics.md) and take the [Newtonian gravitational potential](../../../../../../newtonian-gravitational-potential.md) to be axisymmetric. Work locally on connected regular [magnetic flux](../../../../../../magnetic-flux.md) surfaces with nonzero poloidal flow. As usual for a wind without an imposed toroidal loop voltage, $E_\phi=0$; regularity on an included rotation axis guarantees this condition. It is needed to exclude steady cross-field flow in an annular domain.

Since $\nabla\phi=\mathbf e_\phi/R$, the [poloidal magnetic flux function](../../../../../../poloidal-magnetic-flux-function.md) gives

$$
\mathbf B_p=\frac1R\nabla\psi\times\mathbf e_\phi,
\qquad B_R=-\frac1R\partial_z\psi,\qquad
B_z=\frac1R\partial_R\psi,\qquad
\mathbf B_p\cdot\nabla\psi=0.
$$

The [poloidal magnetic field](../../../../../../poloidal-magnetic-field.md) is divergence-free. The zero toroidal [electric field](../../../../../../electric-field.md), with $\mathbf E=-\mathbf u\times\mathbf B$, gives $\mathbf u_p\parallel\mathbf B_p$. Define $k$ by $\rho\mathbf u_p=k\mathbf B_p$. Steady [mass conservation](../../../../../../mass-conservation.md) then gives

$$
0=\nabla\cdot(\rho\mathbf u_p)=\nabla\cdot(k\mathbf B_p)=\mathbf B_p\cdot\nabla k.
$$

Thus $k=k(\psi)$ is the [magnetohydrodynamic mass loading](../../../../../../magnetohydrodynamic-mass-loading.md), the [mass flux](../../../../../../mass-flux.md) per unit poloidal [magnetic flux](../../../../../../magnetic-flux.md). Subtracting $(k/\rho)\mathbf B$ from the full [velocity](../../../../../../velocity.md) leaves only an azimuthal component. The [cross product](../../../../../../cross-product.md) is

$$
\mathbf u\times\mathbf B
=\left(u_\phi-\frac{kB_\phi}{\rho}\right)\frac{\nabla\psi}{R}
\equiv\omega\nabla\psi.
$$

The steady [ideal magnetohydrodynamic induction equation](../../../../../../ideal-magnetohydrodynamic-induction-equation.md) requires $0=\nabla\times(\omega\nabla\psi)=\nabla\omega\times\nabla\psi$. Consequently the [field-line angular velocity](../../../../../../field-line-angular-velocity.md) is $\omega=\omega(\psi)$ and

$$
\boxed{\mathbf u=\frac{k(\psi)\mathbf B}{\rho}+R\omega(\psi)\mathbf e_\phi}.
$$

Neither gas [pressure](../../../../../../pressure.md) nor axisymmetric gravity exerts an azimuthal [torque](../../../../../../torque.md). Multiplying the azimuthal momentum equation by $R$ combines the cylindrical curvature terms into angular-momentum transport:

$$
\rho\mathbf u_p\cdot\nabla(Ru_\phi)
=\frac1{\mu_0}\mathbf B_p\cdot\nabla(RB_\phi).
$$

Insert $\rho\mathbf u_p=k\mathbf B_p$ and use $\mathbf B_p\cdot\nabla k=0$. It follows that

$$
\mathbf B_p\cdot\nabla\left[R\left(u_\phi-\frac{B_\phi}{\mu_0k}\right)\right]=0,
$$

so the [magnetohydrodynamic angular-momentum invariant](../../../../../../magnetohydrodynamic-angular-momentum-invariant.md) is

$$
\boxed{u_\phi-\frac{B_\phi}{\mu_0k(\psi)}=\frac{\ell(\psi)}R}.
$$

The two terms account respectively for matter and [Maxwell stress tensor](../../../../../../maxwell-stress-tensor.md) transport of [angular momentum](../../../../../../angular-momentum.md).

Finally, subtracting $\gamma$ times the logarithmic [mass density](../../../../../../density.md) equation from the logarithmic [pressure](../../../../../../pressure.md) equation gives $D\ln(p/\rho^\gamma)/Dt=0$. The [specific entropy](../../../../../../specific-entropy.md) of a fixed-composition [ideal gas](../../../../../../ideal-gas.md) is a function of $p/\rho^\gamma$. Steadiness and [axisymmetry](../../../../../../axisymmetric-vector-field.md) reduce its advection to $\mathbf u_p\cdot\nabla s=0$. Hence

$$
\boxed{s=s(\psi),\qquad p=K(\psi)\rho^\gamma}.
$$

These flux-label functions are local on connected regular surfaces; disconnected components with the same numerical label need not share constants without an additional matching condition.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
