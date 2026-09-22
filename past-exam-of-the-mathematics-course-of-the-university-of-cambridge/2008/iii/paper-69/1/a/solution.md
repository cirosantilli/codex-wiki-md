<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For an axisymmetric [magnetic field](../../../../../../magnetic-field.md), the solenoidal condition becomes $\partial_R(RB_R)+\partial_z(RB_z)=0$. Locally introduce a [poloidal magnetic flux function](../../../../../../poloidal-magnetic-flux-function.md) $\Psi$ by

$$
\boxed{B_R=-\frac1R\partial_z\Psi,\qquad B_z=\frac1R\partial_R\Psi,\qquad
\mathbf B_p=\nabla\Psi\times\nabla\phi.}
$$

The divergence condition is exactly the integrability condition for these two derivatives. The additive constant in $\Psi$ fixes the reference flux. For a field regular on the axis choose $\Psi(0,z,t)=0$. Then the [magnetic flux](../../../../../../magnetic-flux.md) through a horizontal disk of radius $R$ is $2\pi\Psi(R,z,t)$, and the flux between two such surfaces is $2\pi\Delta\Psi$.

Since $\mathbf B_p\cdot\nabla\Psi=0$ and $\partial_\phi\Psi=0$, the level surfaces of $\Psi$ contain the complete [magnetic field](../../../../../../magnetic-field.md), including its [toroidal magnetic field](../../../../../../toroidal-magnetic-field.md) component. Thus regular levels are [poloidal flux surfaces](../../../../../../axisymmetric-magnetic-flux-surface.md). Their meridional contours trace the projected field lines. The representation is local on regular regions; disconnected flux surfaces with the same label need not share additional physical data.

The azimuthal component of $\mathbf u\times\mathbf B$ is $u_zB_R-u_RB_z=-\mathbf u_p\cdot\nabla\Psi/R$. The [ideal magnetohydrodynamic induction equation](../../../../../../ideal-magnetohydrodynamic-induction-equation.md), equivalently Faraday's law with $\mathbf E=-\mathbf u\times\mathbf B$, gives $\Psi_t=R(\mathbf u\times\mathbf B)_\phi$ up to a time-dependent reference constant. Fixing that reference gives the [material advection of an axisymmetric magnetic flux function](../../../../../../material-advection-of-an-axisymmetric-magnetic-flux-function.md):

$$
\boxed{\partial_t\Psi+\mathbf u_p\cdot\nabla\Psi=0,\qquad D\Psi/Dt=0.}
$$

Axisymmetry removes the azimuthal contribution to the [material derivative](../../../../../../material-derivative.md). This is [magnetic flux freezing](../../../../../../magnetic-flux-freezing.md) expressed using one scalar flux label.

The azimuthal component itself is generally not an advected scalar. Including the cylindrical basis-vector derivatives in the induction equation gives

$$
\frac{DB_\phi}{Dt}=R\mathbf B_p\cdot\nabla\left(\frac{u_\phi}{R}\right)
 +\frac{u_R}{R}B_\phi-B_\phi\nabla\cdot\mathbf u.
$$

Using [mass conservation](../../../../../../mass-conservation.md), $D\rho/Dt=-\rho\nabla\cdot\mathbf u$, and $DR/Dt=u_R$, this becomes the [toroidal magnetic-field winding equation](../../../../../../toroidal-magnetic-field-winding-equation.md):

$$
\boxed{\frac D{Dt}\left(\frac{B_\phi}{\rho R}\right)
=\frac{\mathbf B_p}{\rho}\cdot\nabla\Omega,\qquad \Omega=u_\phi/R.}
$$

Thus $B_\phi/(\rho R)$ is conserved following the flow if the [angular velocity](../../../../../../angular-velocity.md) is constant along the [poloidal magnetic field](../../../../../../poloidal-magnetic-field.md), including the case of no rotation. Otherwise differential rotation winds poloidal field into toroidal field.

There is also an explicit flux-conservation form,

$$
\partial_tB_\phi+\partial_R(u_RB_\phi-u_\phi B_R)
+\partial_z(u_zB_\phi-u_\phi B_z)=0.
$$

Integrating this over a meridional region converts its change of toroidal flux to boundary terms. Hence such a flux is conserved when the indicated boundary transport vanishes. More generally [magnetic flux freezing](../../../../../../magnetic-flux-freezing.md) conserves flux through every material surface, but a meridional coordinate surface need not remain material when the fluid rotates. **Toroidal flux conservation therefore does not imply that $B_\phi$ itself is materially constant.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
