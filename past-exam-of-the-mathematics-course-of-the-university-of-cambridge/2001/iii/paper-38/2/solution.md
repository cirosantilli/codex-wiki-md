<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The wind integrals require a steady [axisymmetric magnetohydrodynamic wind](../../../../../axisymmetric-magnetohydrodynamic-wind.md) in [ideal magnetohydrodynamics](../../../../../ideal-magnetohydrodynamics.md), with no viscous azimuthal [torque](../../../../../torque.md) or imposed toroidal loop voltage. Axisymmetry by itself is insufficient. Assume smooth connected [poloidal flux surfaces](../../../../../axisymmetric-magnetic-flux-surface.md) with nonzero [poloidal magnetic field](../../../../../poloidal-magnetic-field.md); functions of the flux label below are understood on each such branch. In [cylindrical coordinates](../../../../../cylindrical-coordinate-system.md), the given [poloidal magnetic flux function](../../../../../poloidal-magnetic-flux-function.md) obeys

$$
\mathbf B_p=\frac1s\nabla\chi\times\widehat{\boldsymbol\phi},\qquad
\mathbf B_p\cdot\nabla\chi=0,\qquad
\widehat{\boldsymbol\phi}\times\mathbf B_p=\frac1s\nabla\chi.
$$

For a steady ideal wind, the [electric field](../../../../../electric-field.md) is $\mathbf E=-\mathbf u\times\mathbf B$ and $\nabla\times\mathbf E=0$. Its toroidal component satisfies $\partial_zE_\phi=0$ and $\partial_s(sE_\phi)=0$, so $E_\phi=C/s$. Regularity at the axis, or equivalently the absence of an imposed loop voltage in an annular domain, gives $C=0$. Thus $(\mathbf u_p\times\mathbf B_p)_\phi=0$ and $\mathbf u_p=f\mathbf B_p$. The [continuity equation](../../../../../continuity-equation.md) and $\nabla\cdot\mathbf B_p=0$ now yield

$$
0=\nabla\cdot(\rho\mathbf u_p)=\mathbf B_p\cdot\nabla(\rho f),\qquad
\rho f=\kappa(\chi).
$$

Consequently $\kappa$ is the [magnetohydrodynamic mass loading](../../../../../magnetohydrodynamic-mass-loading.md). Including the [toroidal magnetic field](../../../../../toroidal-magnetic-field.md), rewrite the full [velocity](../../../../../velocity.md) as

$$
\mathbf u=\frac{\kappa}{\rho}\mathbf B+s\omega\widehat{\boldsymbol\phi},\qquad
\omega=\Omega-\frac{\kappa B_\phi}{\rho s}.
$$

Since $\mathbf u\times\mathbf B=\omega\nabla\chi$, steady ideal induction gives $0=\nabla\omega\times\nabla\chi$. Hence $\omega=\omega(\chi)$, establishing

$$
\boxed{\mathbf u=\rho^{-1}\kappa(\chi)\mathbf B+s\omega(\chi)\widehat{\boldsymbol\phi}.}
$$

The invariant $\omega$ is the [field-line angular velocity of an axisymmetric wind](../../../../../field-line-angular-velocity-of-an-axisymmetric-wind.md), not generally the fluid's [angular velocity](../../../../../angular-velocity.md) $\Omega$. When an ideal magnetic surface is anchored to a rigidly rotating star, $\omega$ equals the stellar [angular velocity](../../../../../angular-velocity.md). With no poloidal outflow this reduces to [Ferraro's law of isorotation](../../../../../ferraro-s-law-of-isorotation.md).

To calculate the magnetic [torque](../../../../../torque.md), use the azimuthal momentum equation. Axisymmetric [pressure](../../../../../pressure.md) and [Newtonian gravity](../../../../../gravitational-acceleration.md) have no azimuthal components; the magnetic pressure has none either. The azimuthal acceleration and magnetic tension contain the curvature terms characteristic of [cylindrical coordinates](../../../../../cylindrical-coordinate-system.md):

$$
\rho\left(\mathbf u_p\cdot\nabla u_\phi+\frac{u_su_\phi}{s}\right)
=\frac1{\mu_0}\left(\mathbf B_p\cdot\nabla B_\phi+\frac{B_sB_\phi}{s}\right).
$$

Multiplication by $s$ gives the [Maxwell torque conservation in an axisymmetric wind](../../../../../maxwell-torque-conservation-in-an-axisymmetric-wind.md) equation

$$
\rho\mathbf u_p\cdot\nabla(su_\phi)=\frac1{\mu_0}\mathbf B_p\cdot\nabla(sB_\phi).
$$

Using $u_\phi=s\Omega$, $\rho\mathbf u_p=\kappa\mathbf B_p$ and $\mathbf B_p\cdot\nabla\kappa=0$ proves

$$
\mathbf B_p\cdot\nabla\left(\kappa s^2\Omega-\frac{sB_\phi}{\mu_0}\right)=0,\qquad
\boxed{\ell(\chi)=\kappa s^2\Omega-\frac{sB_\phi}{\mu_0}.}
$$

This is the total [angular momentum](../../../../../angular-momentum.md) transport per unit poloidal [magnetic flux](../../../../../magnetic-flux.md). The first term is the material contribution and the second is the contribution of the [Maxwell stress tensor](../../../../../maxwell-stress-tensor.md). The specific [magnetohydrodynamic angular-momentum invariant](../../../../../magnetohydrodynamic-angular-momentum-invariant.md) is $L=\ell/\kappa$ when $\kappa\ne0$; its normalization differs from the paper's $\ell$.

Define the poloidal [Alfvén Mach number](../../../../../alfven-mach-number.md) by

$$
M_A^2=\frac{|\mathbf u_p|^2}{|\mathbf B_p|^2/(\mu_0\rho)}=\frac{\mu_0\kappa^2}{\rho}.
$$

Substituting $\Omega=\omega+\kappa B_\phi/(\rho s)$ into $\ell$ gives

$$
\ell=\kappa s^2\omega+\frac{sB_\phi}{\mu_0}(M_A^2-1).
$$

At a smooth crossing of the [Alfvén surface](../../../../../alfven-surface.md), $M_A^2=1$ and the [toroidal magnetic field](../../../../../toroidal-magnetic-field.md) is finite. The [Alfvén-surface regularity condition for an axisymmetric wind](../../../../../alfven-surface-regularity-condition-for-an-axisymmetric-wind.md) is therefore

$$
\boxed{\ell=\kappa s_A^2\omega,\qquad L=s_A^2\omega.}
$$

One can also expose the apparent singularity explicitly:

$$
B_\phi=\frac{\mu_0\kappa}{s}\frac{L-s^2\omega}{M_A^2-1},\qquad
\Omega=\frac{M_A^2 L/s^2-\omega}{M_A^2-1}.
$$

Finite passage through the [Alfvén surface](../../../../../alfven-surface.md) requires the numerator to vanish with the denominator. Equality of the numerator zeros is necessary; a globally smooth wind must also satisfy its other dynamical critical conditions. Here $s_A$ is the cylindrical distance from the rotation axis, not automatically the spherical [Alfvén radius](../../../../../alfven-radius.md).

For a tube carrying outward mass flux $d\dot M=\kappa\mathbf B_p\cdot d\mathbf S$, the outward [angular momentum](../../../../../angular-momentum.md) flux is

$$
d\dot J_{\rm out}=\left(\rho\mathbf u_p s u_\phi-\frac{\mathbf B_p sB_\phi}{\mu_0}\right)\cdot d\mathbf S
=L\,d\dot M=\omega s_A^2\,d\dot M.
$$

Thus the stellar [torque](../../../../../torque.md) is $\dot J_\star=-\int\omega s_A^2\,d\dot M$, with the integral over the escaping wind. **Magnetic stresses give each mass element an effective angular-momentum lever arm equal to the cylindrical Alfvén crossing radius.** In a strongly sub-Alfvénic region the fluid approximately corotates with the magnetic surface; beyond that region it can carry the accumulated [angular momentum](../../../../../angular-momentum.md) away. For an outward field and positive $\omega$, a super-Alfvénic expanding tube with $s>s_A$ has $B_\phi<0$, so the magnetic stress transports positive [angular momentum](../../../../../angular-momentum.md) outwards. If $s_A$ greatly exceeds the stellar surface lever arm, a modest mass-loss rate can cause substantial [wind-driven magnetic braking of a solar-type star](../../../../../wind-driven-magnetic-braking-of-a-solar-type-star.md). An unmagnetized outflow would instead carry approximately the material [angular momentum](../../../../../angular-momentum.md) fixed at its launch radius.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
