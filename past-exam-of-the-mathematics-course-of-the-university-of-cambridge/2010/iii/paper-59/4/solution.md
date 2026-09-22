<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [magnetorotational instability](../../../../../magnetorotational-instability.md) extracts energy from [differential rotation](../../../../../differential-rotation.md) through [magnetic tension](../../../../../magnetic-tension.md). It can destabilize a disk whose specific [angular momentum](../../../../../angular-momentum.md) increases outward, even though such a disk satisfies [Rayleigh's circulation criterion](../../../../../rayleigh-s-circulation-criterion.md). The distinction is that an unmagnetized displaced parcel approximately conserves its own [angular momentum](../../../../../angular-momentum.md), whereas a field line transfers [angular momentum](../../../../../angular-momentum.md) between parcels. If [angular velocity](../../../../../angular-velocity.md) decreases outward, an outward-displaced parcel lags its inner partner. Magnetic tension transfers [angular momentum](../../../../../angular-momentum.md) to the outer parcel and removes it from the inner one, making their radial separation increase. A sufficiently stiff magnetic connection suppresses the separation instead. The instability therefore requires a finite range of field-line-bending strengths.

Make this mechanism quantitative in the local [shearing sheet](../../../../../shearing-sheet.md) of a cylindrical rotation profile $\Omega(r)$. Put $q=-d\log\Omega/d\log r$, and take $0<q<2$ so the unmagnetized flow is stable. Its [radial epicyclic frequency](../../../../../radial-epicyclic-frequency.md) is $\kappa^2=2(2-q)\Omega^2$. Let the uniform field be vertical, $B_z\mathbf e_z$, with constant [mass density](../../../../../density.md), and use an axisymmetric horizontal disturbance proportional to $e^{st+ikz}$. Write $\mathbf h=\mathbf b/\sqrt{\mu_0\rho}$ and $\omega_A=kB_z/\sqrt{\mu_0\rho}$. The linearized [ideal magnetohydrodynamics](../../../../../ideal-magnetohydrodynamics.md) equations are

$$
\begin{aligned}
su_r-2\Omega u_\phi&=i\omega_Ah_r,&su_\phi+(2-q)\Omega u_r&=i\omega_Ah_\phi,\\
sh_r&=i\omega_Au_r,&sh_\phi&=-q\Omega h_r+i\omega_Au_\phi.
\end{aligned}
$$

The first pair contains [Coriolis acceleration](../../../../../coriolis-acceleration.md) and the epicyclic response; the last equation is the shear-winding of a radial field perturbation into an azimuthal one. Omitting that winding term would remove the driving mechanism.

Eliminating $h_r,h_\phi$ gives $(s^2+\omega_A^2)u_r=2\Omega s u_\phi$ and $s(s^2+\omega_A^2)u_\phi+\Omega[(2-q)s^2-q\omega_A^2]u_r=0$. Their determinant is the [ideal magnetorotational dispersion relation](../../../../../ideal-magnetorotational-dispersion-relation.md)

$$
\boxed{s^4+(2\omega_A^2+\kappa^2)s^2+\omega_A^2(\omega_A^2-2q\Omega^2)=0.}
$$

Its [discriminant](../../../../../discriminant.md) as a quadratic in $s^2$ is $\kappa^4+16\Omega^2\omega_A^2>0$. Since $2\omega_A^2+\kappa^2>0$, a positive $s^2$ exists precisely when its constant term is negative:

$$
\boxed{0<\omega_A^2<2q\Omega^2=-\frac{d\Omega^2}{d\log r}.}
$$

Thus [angular velocity](../../../../../angular-velocity.md), rather than specific [angular momentum](../../../../../angular-momentum.md), must decrease outward. A Keplerian disk has $q=3/2$, $\kappa^2=\Omega^2$ and is hydrodynamically stable, yet magnetic modes with $0<k^2v_A^2<3\Omega^2$ grow.

The growing root is $s^2=-\omega_A^2-\kappa^2/2+\tfrac12\sqrt{\kappa^4+16\Omega^2\omega_A^2}$. Differentiation with respect to $\omega_A^2$ gives the [maximum growth rate of ideal magnetorotational instability](../../../../../maximum-growth-rate-of-ideal-magnetorotational-instability.md):

$$
\boxed{s_{\max}=\frac{q\Omega}2,\qquad \omega_{A,\max}^2=\frac{q(4-q)}4\Omega^2.}
$$

For Keplerian shear these are $3\Omega/4$ and $15\Omega^2/16$. The ideal maximum is set by shear; reducing field strength reduces the fastest wavelength instead of reducing this maximum growth rate. This is why the exactly zero-field problem differs from a sequence of weak-field problems with progressively larger [wave number](../../../../../wavenumber.md). At fixed [wave number](../../../../../wavenumber.md), growth does tend to zero as the field vanishes. The wavelength must fit the actual disk, and diffusion eventually matters at sufficiently short scales.

The instability has the required angular-momentum-transfer sign. In a growing mode, $u_\phi/u_r=(s^2+\omega_A^2)/(2\Omega s)>0$. At the fastest mode this ratio is one, while induction gives $h_\phi=-h_r$ after allowing for their common Fourier phase. Thus the averaged [Reynolds stress](../../../../../reynolds-stress.md) minus [Maxwell stress tensor](../../../../../maxwell-stress-tensor.md), $\rho\langle u_ru_\phi-h_rh_\phi\rangle$, is positive: [angular momentum](../../../../../angular-momentum.md) moves outward. Its product with $q\Omega$ is the energy supplied by the background shear. These local mechanisms and coefficient conventions are also checked in [the primary MRI stability calculation](https://www.damtp.cam.ac.uk/user/gio10/dad14.pdf).

More general fields require separating field-line bending from field gradients and curvature. At leading local order, for a stationary compatible field in an [incompressible flow](../../../../../incompressible-flow.md) with axisymmetric wavevector $(k_r,0,k_z)$, the bending frequency is

$$
\omega_A=\frac{\mathbf k\cdot\mathbf B}{\sqrt{\mu_0\rho}},\qquad k^2=k_r^2+k_z^2.
$$

[Pressure](../../../../../pressure.md) elimination projects the radial force by $f=k_z^2/k^2$. The radial momentum equation becomes $su_r-2f\Omega u_\phi=i\omega_Ah_r$; the azimuthal and induction equations retain the form above. Eliminating the amplitudes gives the [oblique axisymmetric magnetorotational dispersion relation](../../../../../oblique-axisymmetric-magnetorotational-dispersion-relation.md)

$$
\boxed{\frac{k^2}{k_z^2}(s^2+\omega_A^2)^2+\kappa^2(s^2+\omega_A^2)-4\Omega^2\omega_A^2=0.}
$$

Here $k_z\ne0$. The unstable range is $0<\omega_A^2<-f\,d\Omega^2/d\log r$. The [poloidal magnetic field](../../../../../poloidal-magnetic-field.md) therefore determines whether an axisymmetric perturbation bends a field line. A locally uniform [toroidal magnetic field](../../../../../toroidal-magnetic-field.md) does not enter $\mathbf k\cdot\mathbf B$ for axisymmetry, and can contribute [magnetic pressure](../../../../../magnetic-pressure.md) that is projected out of this incompressible leading-order problem. Thus a toroidal component does not suppress the weak-field MRI merely by being present. Conversely a purely toroidal field has no ordinary axisymmetric local bending MRI in this approximation. This does not imply that every globally curved toroidal equilibrium is stable.

A steady general [poloidal magnetic field](../../../../../poloidal-magnetic-field.md) must also be compatible with the equilibrium rotation. The azimuthal [ideal magnetohydrodynamic induction equation](../../../../../ideal-magnetohydrodynamic-induction-equation.md) contains $\partial_tB_\phi=r\mathbf B_p\cdot\nabla\Omega$. A stationary axisymmetric equilibrium with no meridional flow consequently requires $\mathbf B_p\cdot\nabla\Omega=0$, [Ferraro's law of isorotation](../../../../../ferraro-s-law-of-isorotation.md). A radial field crossing cylindrical differential-rotation surfaces would otherwise wind secularly; it cannot simply be substituted into a stationary normal-mode calculation. Boundary conditions and the along-field eigenvalue problem replace a freely chosen local $k$ in nonuniform or bounded equilibria. Strong enough field-line tension can then stabilize all admissible wavelengths.

An explicit axisymmetric effect of nonuniform field strength and curvature is obtained with a purely toroidal field $B_\phi(r)\mathbf e_\phi$, constant [mass density](../../../../../density.md) and cylindrical rotation. A radial [fluid displacement](../../../../../lagrangian-displacement-fluid-mechanics.md) changes the field by

$$
b_\phi=\left(\frac{B_\phi}{r}-B_\phi'\right)\xi_r.
$$

This follows directly from $\mathbf b=\nabla\times(\boldsymbol\xi\times\mathbf B)$ and incompressibility. Its radial curvature force, after absorbing the magnetic-pressure perturbation, is $-2B_\phi b_\phi/(\mu_0\rho r)$. The axisymmetric azimuthal momentum equation is $su_\phi+(2\Omega+r\Omega')u_r=0$. Combining it with the radial force and then projecting out [pressure](../../../../../pressure.md) gives

$$
\boxed{\omega^2=\frac{k_z^2}{k^2}\mathcal D,\qquad \mathcal D=\kappa^2-\frac r{\mu_0\rho}\frac{d}{dr}\left(\frac{B_\phi}{r}\right)^2.}
$$

This is the local [Michael criterion for axisymmetric toroidal-field interchange](../../../../../michael-criterion-for-axisymmetric-toroidal-field-interchange.md). The new term can either stabilize or destabilize: for $B_\phi\propto r^p$, $\mathcal D=\kappa^2+2(1-p)v_{A\phi}^2/r^2$. A current-free $B_\phi\propto r^{-1}$ is stabilizing; $B_\phi\propto r$ leaves this axisymmetric interchange coefficient unchanged; a sufficiently steep increase with $p>1$ can destabilize even a centrifugally stable rotation law. That last instability can persist without differential rotation, so its energy source is the magnetic-current equilibrium rather than the ordinary MRI. Nonaxisymmetric current-driven modes are outside the requested essay scope.

For mixed poloidal and toroidal fields, the full induction perturbation contains $(\mathbf B\cdot\nabla)\boldsymbol\xi-(\boldsymbol\xi\cdot\nabla)\mathbf B-\mathbf B\nabla\cdot\boldsymbol\xi$, and the linear [Lorentz force](../../../../../lorentz-force.md) contains both $(\nabla\times\mathbf b)\times\mathbf B$ and $(\nabla\times\mathbf B)\times\mathbf b$. These terms explain why gradients and curvature cannot be replaced everywhere by a scalar $k^2v_A^2$: they can draw on equilibrium-current energy and couple the radial and vertical motions. Compressibility introduces additional [magnetic pressure](../../../../../magnetic-pressure.md) and magnetosonic responses; a strong toroidal field can alter the dispersion even though it disappeared from the leading incompressible weak-field result.

Finally, a vertically or radially stratified general field also supports part of the equilibrium weight through [magnetic pressure](../../../../../magnetic-pressure.md). A displaced flux tube carries its frozen-in mass-to-flux relation, so its [mass density](../../../../../density.md) at the surrounding total [pressure](../../../../../pressure.md) can differ from its new environment. This introduces [magnetic buoyancy instability](../../../../../magnetic-buoyancy-instability.md) and competition with ordinary [buoyancy](../../../../../buoyancy.md). Axisymmetric interchange displacements can access this energy without an azimuthal [wave number](../../../../../wavenumber.md), while poloidal tension resists variation along the field. Growth that survives when $d\Omega/dr=0$ must not be attributed to shear-driven MRI. The general-field stability problem therefore combines shear, field-line tension, current/curvature forces, compressibility, [buoyancy](../../../../../buoyancy.md) and boundary constraints; the uniform-field result isolates the basic angular-momentum feedback mechanism.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
