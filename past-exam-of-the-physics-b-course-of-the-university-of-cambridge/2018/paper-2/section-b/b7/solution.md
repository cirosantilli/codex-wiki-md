<h1 id="section-b/b7/solution">Solution</h1>

↑ **Parent:** [B7](../b7.md)

**From molecular dipoles to macroscopic fields.** A [dielectric](../../../../../dielectric.md) contains charges which remain bound to its atoms or [molecules](../../../../../molecule-split.md). An applied [electric field](../../../../../electric-field-split.md) displaces positive and negative charge centres and can orient permanent [electric dipoles](../../../../../electric-dipole.md). The [electric polarization](../../../../../polarization-density.md) $\mathbf P$ is [electric dipole moment](../../../../../electric-dipole-moment.md) per unit [volume](../../../../../volume-thermodynamics.md), in $\mathrm{C\,m^{-2}}$. Its associated [bound charge](../../../../../bound-charge.md) is

$$
\rho_b=-\nabla\cdot\mathbf P,\qquad \sigma_b=\mathbf P\cdot\widehat{\mathbf n}
$$

at the boundary of the polarized material, where $\widehat{\mathbf n}$ points outward. A uniform [electric polarization](../../../../../polarization-density.md) has no [volume](../../../../../volume-thermodynamics.md) [bound charge](../../../../../bound-charge.md), but generally has surface [bound charge](../../../../../bound-charge.md). The [electric field](../../../../../electric-field-split.md) remains the [force](../../../../../force-split.md) per unit test charge; it includes the fields of both free and bound charges.

Introducing the [electric displacement field](../../../../../electric-displacement-field.md) $\mathbf D=\epsilon_0\mathbf E+\mathbf P$ packages the free-charge source separately:

$$
\nabla\cdot\mathbf E=\frac{\rho_f+\rho_b}{\epsilon_0},\qquad
\nabla\cdot\mathbf D=\rho_f,\qquad \nabla\times\mathbf E=0.
$$

For a homogeneous linear isotropic [dielectric](../../../../../dielectric.md),

$$
\mathbf P=\epsilon_0\chi_e\mathbf E,\qquad
\mathbf D=\epsilon\mathbf E,\qquad \epsilon=\epsilon_0(1+\chi_e)=\epsilon_0\epsilon_r.
$$

The [electric susceptibility](../../../../../electric-susceptibility.md) $\chi_e$ is dimensionless; the [permittivity](../../../../../permittivity-split.md) $\epsilon$ has units $\mathrm{F\,m^{-1}}$. This is a constitutive approximation. An anisotropic [dielectric](../../../../../dielectric.md) requires a [permittivity tensor](../../../../../permittivity-tensor.md), while a nonlinear [dielectric](../../../../../dielectric.md) need not have [electric polarization](../../../../../polarization-density.md) proportional to [electric field](../../../../../electric-field-split.md). The field in these equations is the macroscopic field, not necessarily the [local field](../../../../../local-field.md) at an individual [molecule](../../../../../molecule-split.md).

**Interfaces.** Let $\widehat{\mathbf n}$ point from medium 1 into medium 2. Integrating [Gauss's law](../../../../../gauss-s-law.md) over a thin pillbox, and the electrostatic [curl](../../../../../curl.md) equation around a thin loop, gives the [electrostatic interface boundary conditions](../../../../../electrostatic-interface-boundary-conditions.md)

$$
\boxed{\widehat{\mathbf n}\cdot(\mathbf D_2-\mathbf D_1)=\sigma_f,
\qquad \widehat{\mathbf n}\times(\mathbf E_2-\mathbf E_1)=0.}
$$

Thus normal electric [displacement](../../../../../displacement.md) is continuous when there is no free surface charge, whereas tangential [electric field](../../../../../electric-field-split.md) is continuous even if the [permittivity](../../../../../permittivity-split.md) changes. Normal [electric field](../../../../../electric-field-split.md) generally jumps because the interface carries [bound charge](../../../../../bound-charge.md). The electric potential is continuous for an ordinary interface without an ideal dipole sheet. These conditions, together with [Laplace's equation](../../../../../laplace-equation.md) in each homogeneous charge-free region, determine the field.

**[Energy](../../../../../energy-split.md) and electrical sources.** Reversibly assembling [free charge](../../../../../free-charge.md) requires incremental [work](../../../../../work.md) $\delta W=\int\mathbf E\cdot\delta\mathbf D\,dV$. For a linear [dielectric](../../../../../dielectric.md) whose response can be reversibly integrated from zero field, the [electrostatic energy](../../../../../electrostatic-energy.md) is

$$
\boxed{W=\frac12\int\mathbf E\cdot\mathbf D\,dV.}
$$

This includes the material polarization response, rather than simply using $\epsilon_0E^2/2$ everywhere. In a [capacitor](../../../../../capacitor.md), $W=Q^2/(2C)=CV^2/2$. Inserting a [dielectric](../../../../../dielectric.md) increases [capacitance](../../../../../capacitance.md). At fixed charge the stored [energy](../../../../../energy-split.md) decreases. At fixed voltage the stored field [energy](../../../../../energy-split.md) increases, but the voltage source supplies $V\,dQ$; the appropriate mechanical [energy](../../../../../energy-split.md) including that source changes by $-V^2dC/2$. Both cases predict attraction of [dielectric](../../../../../dielectric.md) into the [capacitor](../../../../../capacitor.md). A [force](../../../../../force-split.md) calculation must state which electrical quantity is fixed. A lossy or hysteretic [dielectric](../../../../../dielectric.md) also dissipates [energy](../../../../../energy-split.md), so the reversible quadratic expression does not describe its full history.

**Shape and depolarization.** Suppose the [dielectric](../../../../../dielectric.md) is surrounded by [vacuum](../../../../../vacuum.md) and the distant imposed [electric field](../../../../../electric-field-split.md) is $\mathbf E_0$. Bound surface charge produces a [depolarization field](../../../../../depolarization-field.md). For a uniformly polarized [ellipsoid](../../../../../ellipsoid.md), along a [principal axis](../../../../../principal-axis.md),

$$
E_{\rm in}=E_0-\frac{N_dP}{\epsilon_0},\qquad
P=\epsilon_0(\epsilon_r-1)E_{\rm in},
\qquad
\boxed{E_{\rm in}=\frac{E_0}{1+N_d(\epsilon_r-1)}.}
$$

Here $N_d$ is the [depolarization factor of a dielectric ellipsoid](../../../../../depolarization-factor-of-a-dielectric-ellipsoid.md). This self-consistent field explains why the same material responds differently in different shapes.

An infinite slab with [electric field](../../../../../electric-field-split.md) normal to its faces has $N_d=1$, giving $E_{\rm in}=E_0/\epsilon_r$; its opposite surface bound charges reduce the internal field. For [electric field](../../../../../electric-field-split.md) parallel to the faces, $N_d=0$, giving $E_{\rm in}=E_0$. End effects are neglected.

A very long circular rod in an axial [electric field](../../../../../electric-field-split.md) has negligible depolarization away from its ends, so $E_{\rm in}\simeq E_0$. In a transverse [electric field](../../../../../electric-field-split.md) the infinite-cylinder solution has $N_d=1/2$, giving $E_{\rm in}=2E_0/(\epsilon_r+1)$. To see the latter directly, take the applied field along $x$. The interior and exterior electric potentials can be written $\phi_{\rm in}=-B r\cos\theta$ and $\phi_{\rm out}=-E_0r\cos\theta+A\cos\theta/r$. Continuity of potential and normal electric [displacement](../../../../../displacement.md) at $r=a$ gives $B=2E_0/(\epsilon_r+1)$.

For a [sphere](../../../../../sphere.md) of radius $a$, $N_d=1/3$ and

$$
\boxed{\mathbf E_{\rm in}=\frac{3}{\epsilon_r+2}\mathbf E_0,
\qquad \mathbf p=4\pi\epsilon_0a^3\frac{\epsilon_r-1}{\epsilon_r+2}\mathbf E_0.}
$$

For example, write $\phi_{\rm in}=-B r\cos\theta$ and $\phi_{\rm out}=-E_0r\cos\theta+C\cos\theta/r^2$. Continuity of potential gives $B=E_0-C/a^3$, and continuity of normal electric [displacement](../../../../../displacement.md) gives $\epsilon B=\epsilon_0(E_0+2C/a^3)$. Solving yields $B=3E_0/(\epsilon_r+2)$ and $C=a^3E_0(\epsilon_r-1)/(\epsilon_r+2)$. The $1/r^2$ potential is that of the [electric dipole moment](../../../../../electric-dipole-moment.md) above. For $\epsilon_r=1$ all these induced effects vanish; as $\epsilon_r$ becomes very large the normal-field [sphere](../../../../../sphere.md) and slab approach the corresponding conductor field exclusion. The ideal infinitely long rod in an exactly axial imposed field has a different, singular end-free limit.

## ↑ Ancestors (14)

1. [B7](../b7.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2018](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
