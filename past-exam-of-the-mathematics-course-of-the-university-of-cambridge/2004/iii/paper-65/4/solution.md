<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

In the rapidly rotating [magnetohydrodynamics](../../../../../magnetohydrodynamics.md) of a conducting core, the [magnetostrophic balance](../../../../../magnetostrophic-balance.md) neglects inertia and, initially, viscosity:

$$
2\rho\Omega\hat z\times u=-\nabla p+f_b+J\times B,\qquad \nabla\cdot u=0,\qquad J=\mu_0^{-1}\nabla\times B.
$$

Take a spherical or suitable axisymmetric impenetrable container, with gravity/buoyancy having no azimuthal component and no applied mechanical torque. Small [Rossby number](../../../../../rossby-number.md) is the slow-motion assumption. It does not imply that an arbitrary magnetic field is compatible with the balance.

Use cylindrical coordinates $(s,\phi,z)$ and integrate the azimuthal momentum equation over the fluid portion $C_s$ of a cylinder. The pressure term integrates to zero because it is a periodic $\phi$ derivative. The Coriolis contribution is proportional to the radial flux $\int_{C_s}u_s\,s\,d\phi dz$. By incompressibility and impermeability it is zero: closing the cylinder with the container's caps and applying the [divergence theorem](../../../../../divergence-theorem.md) produces no net flux. There is no azimuthal buoyancy term. Consequently

$$
\boxed{\int_{C_s}(J\times B)_\phi\,d\phi dz=0\quad\text{on every geostrophic cylinder}.}
$$

This is [Taylor's condition](../../../../../taylor-constraint.md). Equivalently define the torque per radial thickness by $\mathcal T(s)=s^2\int_{C_s}(J\times B)_\phi d\phi dz$; it must vanish. In a shell, cylinders split by the inner boundary require the corresponding connected-region conditions. These compatibility conditions concern rotating-fluid torque, distinct from force-free magnetic relaxation in a plasma. Their primary origin is [Taylor's rotating-fluid analysis](https://mhd.ens.fr/IHP09/Jackson/Biblio/taylor_63.pdf).

A [magnetostrophic Taylor state](../../../../../magnetostrophic-taylor-state.md) allows construction of the flow's ageostrophic part. Taking the curl gives

$$
-2\rho\Omega\partial_z u=\nabla\times(f_b+J\times B).
$$

Integrate along rotation-axis lines and impose impermeability, then use incompressibility and periodicity to reconstruct a particular solution $u_a$. In a sphere the boundary geometry supplies the independent endpoint conditions; a cylinder with parallel planar end normals has additional degeneracies. The homogeneous momentum equation admits any differential cylindrical rotation $u_g=s\omega(s)\hat\phi$. Its Coriolis force is a radial pressure gradient, so momentum balance alone cannot determine $\omega$.

The additional equation is dynamic preservation of the constraint. Let

$$
\mathcal D_B[C](s)=\frac{s^2}{\mu_0}\int_{C_s}\left[(\nabla\times C)\times B+(\nabla\times B)\times C\right]_\phi d\phi dz.
$$

This is the first variation of the cylindrical Lorentz torque. The [resistive induction equation](../../../../../resistive-induction-equation.md) supplies $\dot B=\nabla\times(u\times B)+\eta\nabla^2B$. Define $C_a=\nabla\times(u_a\times B)+\eta\nabla^2B$ and $L_B[\omega]=\nabla\times(s\omega\hat\phi\times B)$. Then the [geostrophic flow preserving the Taylor constraint](../../../../../geostrophic-flow-preserving-the-taylor-constraint.md) solves

$$
\boxed{\mathcal D_B[L_B[\omega]]=-\mathcal D_B[C_a].}
$$

For a given field this is linear in $\omega$; it prescribes the cylindrical rotation needed to keep the field on the Taylor-state manifold. The magnetic boundary conditions must also be imposed on $\dot B$. Boundary terms cannot generally be discarded for insulating exteriors; their role in a correct construction is described in [Hardy and collaborators' primary analysis](https://arxiv.org/abs/1806.06612).

For example, when magnetic surface torque vanishes, as for compatible $B\cdot n=0$ conditions, the [Maxwell stress tensor](../../../../../maxwell-stress-tensor.md) gives

$$
\mathcal T(s)=\frac1{\mu_0}\partial_s\left[s^2\int_{C_s}B_sB_\phi d\phi dz\right].
$$

Cylindrical rotation induces component changes $\dot B_s=-\omega\partial_\phi B_s$ and $\dot B_\phi=sB_s\omega'-\omega\partial_\phi B_\phi$. Their product variation integrates to $s\omega'\int B_s^2d\phi dz$, since the azimuthal derivative integrates to zero. Thus the geostrophic part of the preservation equation reduces to

$$
\frac1{\mu_0}\partial_s\left[s^3\left(\int_{C_s}B_s^2d\phi dz\right)\omega'\right]=-\mathcal D_B[C_a].
$$

Regularity and compatible boundary conditions fix the nontrivial integration freedom; total [angular momentum](../../../../../angular-momentum.md) fixes the solid-body rotation null mode. If $B_s$ vanishes on an entire cylinder, the magnetic coupling coefficient degenerates and generic uniqueness must not be asserted. The simplified expression is conditional on the surface-torque assumption, rather than a general replacement for the boundary-compatible operator equation.

With small positive viscosity the momentum equation adds $\rho\nu\nabla^2u$. Its cylinder integral becomes the [viscous regularization of the Taylor constraint](../../../../../viscous-regularization-of-the-taylor-constraint.md)

$$
\boxed{\mathcal T_L(s)+\mathcal T_\nu(s)=0.}
$$

Magnetic torque need no longer vanish exactly; it can be transmitted by viscous stress. Bulk viscosity is order $E=\nu/(2\Omega L^2)$ at fixed velocity. For ordinary no-slip rotating boundaries, thin [Ekman layers](../../../../../ekman-layer.md) have thickness of order $L\sqrt E$ and shear stress of order $\rho\Omega LU\sqrt E$, larger than the bulk order-$E$ correction. Boundary pumping and this friction help select the otherwise undetermined [geostrophic flow](../../../../../geostrophic-flow.md). In the inviscid interior only impermeability is imposed; no-slip matching is supplied by the thin layer, so simply imposing all viscous boundary conditions on the zero-viscosity equations is incorrect.

For bounded velocities, the viscous torque tends to zero as $E\to0$, recovering the leading Taylor condition. A prescribed order-one uncompensated magnetic torque would instead require a velocity growing like $E^{-1/2}$ under Ekman friction, or $E^{-1}$ under bulk friction alone. Such growth eventually invalidates the assumed small Rossby number: the limit is singular, not a regular guarantee that every imposed magnetic field has an inviscid solution. With stress-free boundaries the leading no-slip friction is absent, and bulk stresses, magnetic boundary conditions and angular-momentum normalization require their own treatment. Retaining inertia permits torque-driven torsional motion rather than an exact magnetostrophic constraint. Thus zero viscosity gives a magnetic compatibility condition and an induction-based selection of cylindrical rotation, while small viscosity replaces it by a torque balance whose bounded solutions approach compatible Taylor states.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 65](../../paper-65-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
