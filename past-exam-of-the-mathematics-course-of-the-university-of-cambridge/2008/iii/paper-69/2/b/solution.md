<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Steady axisymmetric [mass conservation](../../../../../../mass-conservation.md) is $\nabla\cdot(\rho\mathbf u_p)=0$, permitting the [axisymmetric hydrodynamic mass flux function](../../../../../../axisymmetric-hydrodynamic-mass-flux-function.md) representation

$$
u_R=-\frac{\psi_z}{\rho R},\qquad u_z=\frac{\psi_R}{\rho R},\qquad
\mathbf u_p\cdot\nabla\psi=0.
$$

Thus stream surfaces are regular level surfaces of $\psi$. Adiabaticity gives $\mathbf u\cdot\nabla s=0$, and axisymmetry removes the azimuthal derivative, so the [specific entropy](../../../../../../specific-entropy.md) is constant along their meridional streamlines. The azimuthal [Euler equations for an inviscid fluid](../../../../../../euler-equations-for-an-inviscid-fluid.md) has no [pressure](../../../../../../pressure.md) or gravitational torque:

$$
\mathbf u_p\cdot\nabla u_\phi+u_Ru_\phi/R=0
\quad\Longrightarrow\quad
\mathbf u_p\cdot\nabla(Ru_\phi)=0.
$$

The conserved [specific angular momentum](../../../../../../specific-angular-momentum.md) is $\ell=Ru_\phi$. Taking the scalar product of the steady [Crocco form of the unsteady Euler equation](../../../../../../crocco-form-of-the-unsteady-euler-equation.md) with $\mathbf u$ also gives

$$
\mathbf u\cdot\nabla\varepsilon=T\mathbf u\cdot\nabla s=0,\qquad
\varepsilon=u^2/2+\Phi+w.
$$

Consequently, on each connected regular family of stream surfaces,

$$
\boxed{s=s(\psi),\qquad \ell=\ell(\psi),\qquad
\varepsilon=\varepsilon(\psi).}
$$

These functions express entropy, angular momentum and the [Bernoulli function](../../../../../../bernoulli-function.md) carried by a [stellar wind](../../../../../../stellar-wind.md). Stagnation regions and disconnected branches with identical flux labels require their own matching information; the argument establishes the functions locally where the poloidal flow is nonzero.

To derive the [hydrodynamic transfield equation for an axisymmetric wind](../../../../../../hydrodynamic-transfield-equation-for-an-axisymmetric-wind.md), decompose the [vorticity](../../../../../../vorticity.md). The poloidal part comes from the toroidal [velocity](../../../../../../velocity.md):

$$
\boldsymbol\omega_p=\nabla(Ru_\phi)\times\nabla\phi
=\ell'(\psi)\nabla\psi\times\nabla\phi=\rho\ell'\mathbf u_p.
$$

The azimuthal part comes from the poloidal [velocity](../../../../../../velocity.md):

$$
\begin{aligned}
\omega_\phi&=\partial_z u_R-\partial_Ru_z\\
&=-\partial_z\left(\frac{\psi_z}{\rho R}\right)
 -\partial_R\left(\frac{\psi_R}{\rho R}\right)
=-R\nabla\cdot\left(\frac{\nabla\psi}{\rho R^2}\right).
\end{aligned}
$$

The final divergence is the full axisymmetric cylindrical divergence, including its radial $1/R$ factor.

Since $\mathbf u_p=\nabla\psi\times\mathbf e_\phi/(\rho R)$, the meridional part of $\boldsymbol\omega\times\mathbf u$ is

$$
\boldsymbol\omega_p\times u_\phi\mathbf e_\phi
+\omega_\phi\mathbf e_\phi\times\mathbf u_p
=\left(-\frac{\ell\ell'}{R^2}+\frac{\omega_\phi}{\rho R}\right)\nabla\psi.
$$

The remaining steady [Euler equations for an inviscid fluid](../../../../../../euler-equations-for-an-inviscid-fluid.md) is therefore

$$
\left(-\frac{\ell\ell'}{R^2}+\frac{\omega_\phi}{\rho R}\right)\nabla\psi
=(Ts'-\varepsilon')\nabla\psi.
$$

Canceling $\nabla\psi$ on a regular stream surface and inserting $\omega_\phi$ gives

$$
\boxed{\frac1\rho\nabla\cdot\left(\frac{\nabla\psi}{\rho R^2}\right)
=\frac{d\varepsilon}{d\psi}-T\frac{ds}{d\psi}
-\frac{\ell}{R^2}\frac{d\ell}{d\psi}.}
$$

The sign of the angular-momentum term follows from $\mathbf u_p\times\mathbf e_\phi=-\nabla\psi/(\rho R)$. To determine the wind, this transverse force equation is supplemented by its [Bernoulli function](../../../../../../bernoulli-function.md) relation

$$
\varepsilon(\psi)=\frac{|\nabla\psi|^2}{2\rho^2R^2}
+\frac{\ell(\psi)^2}{2R^2}+\Phi+w(\rho,s(\psi)),
$$

and the [equation of state](../../../../../../equation-of-state.md), with the [gravitational potential](../../../../../../newtonian-potential-of-a-point-mass.md) supplied externally or by the [Poisson equation](../../../../../../poisson-equation.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
