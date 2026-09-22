# Paper 38

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper38.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper38.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 38](paper-38.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Work with the complex representation and take its real part to obtain the physical [magnetic field](../../../electromagnetism.md#magnetic-field). For constant [magnetic diffusivity](../../../astrophysical-fluid-dynamics.md#magnetic-diffusivity) and the prescribed circular [velocity](../../../classical-mechanics.md#velocity) $\mathbf u=s\Omega(s)\widehat{\boldsymbol\phi}$, the [resistive induction equation](../../../astrophysical-fluid-dynamics.md#resistive-induction-equation) and $\mathbf B=\nabla\times(A\widehat{\mathbf z})$ give

$$
B_s=\frac1s\partial_\phi A,\qquad B_\phi=-\partial_s A,\qquad
\partial_tA+\Omega\partial_\phi A=\eta\left(\partial_s^2A+\frac1s\partial_sA+\frac1{s^2}\partial_\phi^2A\right).
$$

To see the last equation directly, $\mathbf u\times\mathbf B=-s\Omega B_s\widehat{\mathbf z}=-\Omega A_\phi\widehat{\mathbf z}$. Taking its [curl](../../../calculus.md#curl) reproduces the induction equation if $A_t=-\Omega A_\phi+\eta\nabla^2A$, up to a time-dependent additive constant removable by the [gauge transformation](../../../electromagnetism.md#gauge-transformation). This is the scalar form of advection and [magnetic diffusion](../../../astrophysical-fluid-dynamics.md#magnetic-diffusion) in [cylindrical coordinates](../../../calculus.md#cylindrical-coordinate-system).

Put $\psi=\phi-\Omega(s)t$. The [material derivative](../../../continuum-mechanics.md#material-derivative) of $ae^{i\psi}$ is $a_t e^{i\psi}$, because $\psi_t+\Omega\psi_\phi=0$. A radial [derivative](../../../calculus.md#derivative) instead acts on both amplitude and phase:

$$
\partial_sA=(a_s-it\Omega'a)e^{i\psi},\qquad
\partial_s^2A=(a_{ss}-2it\Omega'a_s-it\Omega''a-t^2(\Omega')^2a)e^{i\psi}.
$$

Also $A_{\phi\phi}=-ae^{i\psi}$. Substitution gives the [shearing-coordinate magnetic flux equation](../../../astrophysical-fluid-dynamics.md#shearing-coordinate-magnetic-flux-equation), here for azimuthal mode number one:

$$
\boxed{a_t=\eta\left[a_{ss}+\frac{a_s}{s}-\frac a{s^2}-(\Omega')^2t^2a-2it\Omega'a_s-\frac{it\Omega'}s a-it\Omega''a\right].}
$$

Writing it with $a_t$ on the left is important when considering zero [magnetic diffusivity](../../../astrophysical-fluid-dynamics.md#magnetic-diffusivity): one must not literally divide by $\eta=0$. **In the ideal limit, $a_t=0$**, so $A(s,\phi,t)=A(s,\phi-\Omega(s)t,0)$. This is [magnetic flux freezing](../../../astrophysical-fluid-dynamics.md#magnetic-flux-freezing): the scalar flux pattern is carried with each rotating fluid ring. It does not make the [magnetic field](../../../electromagnetism.md#magnetic-field) stationary. Indeed,

$$
B_s=\frac{ia(s,0)}s e^{i\psi},\qquad B_\phi=[-a_s(s,0)+it\Omega'a(s,0)]e^{i\psi},
$$

so [differential rotation](../../../astrophysical-fluid-dynamics.md#differential-rotation) winds the field and can make its azimuthal component grow linearly in time. Rigid rotation, for which $\Omega'=0$, only rotates the pattern.

For the specified interior [angular velocity](../../../classical-mechanics.md#angular-velocity), $\Omega'=-\Omega_0/d$ and $\Omega''=0$ away from the circulation edge. Let $T=\Omega_0t$, $x=s/d$ and $\mathrm{Rm}=\Omega_0d^2/\eta$. The amplitude equation becomes

$$
\partial_Ta=\frac1{\mathrm{Rm}}\left[a_{xx}+\frac{a_x}{x}-\frac a{x^2}-T^2a+2iTa_x+\frac{iT}{x}a\right].
$$

For a smooth initial amplitude on the cell scale, at $x$ bounded away from zero and the edge, the $-T^2a$ term dominates when $T\gg1$. Its accumulated damping is order one at $T=O(\mathrm{Rm}^{1/3})$, whereas the integrated terms proportional to $T$ are only $O(\mathrm{Rm}^{-1/3})$ and the terms independent of $T$ are $O(\mathrm{Rm}^{-2/3})$. The resulting [cubic-time resistive damping in a differentially rotating cell](../../../astrophysical-fluid-dynamics.md#cubic-time-resistive-damping-in-a-differentially-rotating-cell) is

$$
a(s,t)\simeq a(s,0)\exp\left[-\frac{\eta\Omega_0^2t^3}{3d^2}\right],\qquad
\boxed{\tau_c=\left(\frac{3d^2}{\eta\Omega_0^2}\right)^{1/3},\quad\Omega_0\tau_c=(3\mathrm{Rm})^{1/3}.}
$$

The [magnetic field](../../../electromagnetism.md#magnetic-field) has this leading [exponential decay](../../../analysis.md#exponential-decay) envelope. Its components also contain the algebraic winding factor visible in $B_\phi$, so the claim concerns the cubic exponent, not an exact amplitude with no prefactor. Equivalently the radial [wavenumber](../../../wave-equation.md#wavenumber) grows as $|k_s|\simeq|\Omega'|t$ and the integrated resistive damping is $\int_0^t\eta k_s^2dt=\eta(\Omega')^2t^3/3$.

This is [phase mixing in magnetic flux expulsion](../../../astrophysical-fluid-dynamics.md#phase-mixing-in-magnetic-flux-expulsion). The circulation creates ever finer gradients, allowing weak [magnetic diffusion](../../../astrophysical-fluid-dynamics.md#magnetic-diffusion) to act much sooner than its unsheared time $t_\eta=d^2/\eta$:

$$
\Omega_0^{-1}\ll\tau_c\ll t_\eta,\qquad \frac{\tau_c}{t_\eta}=3^{1/3}\mathrm{Rm}^{-2/3}.
$$

**Rapid winding followed by resistive smoothing expels the imposed field from the cell interior.** The maintained exterior [magnetic field](../../../electromagnetism.md#magnetic-field) is redistributed into a circulation-edge [boundary layer](../../../continuum-mechanics.md#boundary-layer). The result is an interior high-[magnetic Reynolds number](../../../astrophysical-fluid-dynamics.md#magnetic-reynolds-number) transient, not a uniform assertion at the axis and the nonsmooth edge, nor the exact $t\to\infty$ solution with a continuously imposed far field. The diffusion length at $\tau_c$ is $\sqrt{\eta\tau_c}/d=3^{1/6}\mathrm{Rm}^{-1/3}$, identifying where a local bulk approximation can fail. The linear profile also needs smoothing at a regular rotation axis and at $s=d$ if used as a fully smooth global flow.

In photospheric [magnetoconvection](../../../astrophysical-fluid-dynamics.md#magnetoconvection), circulating and diverging [convection](../../../fluid-mechanics.md#convection) transports weak [magnetic flux](../../../electromagnetism.md#magnetic-flux) towards converging downflow regions. [Solar granulation](../../../stellar-astrophysics.md#solar-granulation) concentrates field in [intergranular lanes](../../../stellar-astrophysics.md#intergranular-lane), while larger-scale [supergranulation](../../../stellar-astrophysics.md#supergranulation) helps form the [solar magnetic network](../../../stellar-astrophysics.md#solar-magnetic-network). [Flux expulsion](../../../astrophysical-fluid-dynamics.md#flux-expulsion) explains why a highly conducting [photosphere](../../../stellar-structure.md#photosphere) can have relatively weak field in cell interiors and intermittent concentrations at their edges: high [electrical conductivity](../../../electromagnetism.md#electrical-conductivity) delays diffusion on the original scale, but does not prevent diffusion on the fine scales created by advection. A long-lived circulation must last long enough for the expulsion time; rapidly changing cells need not reach this idealized state. Once the field becomes strong, the [Lorentz force](../../../electromagnetism.md#lorentz-force) modifies the [convection](../../../fluid-mechanics.md#convection), so this prescribed-flow calculation alone neither determines the final field strength nor describes strong-field [sunspots](../../../stellar-astrophysics.md#sunspot).

## 2

↑ **Parent:** [Paper 38](paper-38.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The wind integrals require a steady [axisymmetric magnetohydrodynamic wind](../../../astrophysical-fluid-dynamics.md#axisymmetric-magnetohydrodynamic-wind) in [ideal magnetohydrodynamics](../../../astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamics), with no viscous azimuthal [torque](../../../classical-mechanics.md#torque) or imposed toroidal loop voltage. Axisymmetry by itself is insufficient. Assume smooth connected [poloidal flux surfaces](../../../astrophysical-fluid-dynamics.md#axisymmetric-magnetic-flux-surface) with nonzero [poloidal magnetic field](../../../astrophysical-fluid-dynamics.md#poloidal-magnetic-field); functions of the flux label below are understood on each such branch. In [cylindrical coordinates](../../../calculus.md#cylindrical-coordinate-system), the given [poloidal magnetic flux function](../../../astrophysical-fluid-dynamics.md#poloidal-magnetic-flux-function) obeys

$$
\mathbf B_p=\frac1s\nabla\chi\times\widehat{\boldsymbol\phi},\qquad
\mathbf B_p\cdot\nabla\chi=0,\qquad
\widehat{\boldsymbol\phi}\times\mathbf B_p=\frac1s\nabla\chi.
$$

For a steady ideal wind, the [electric field](../../../electromagnetism.md#electric-field) is $\mathbf E=-\mathbf u\times\mathbf B$ and $\nabla\times\mathbf E=0$. Its toroidal component satisfies $\partial_zE_\phi=0$ and $\partial_s(sE_\phi)=0$, so $E_\phi=C/s$. Regularity at the axis, or equivalently the absence of an imposed loop voltage in an annular domain, gives $C=0$. Thus $(\mathbf u_p\times\mathbf B_p)_\phi=0$ and $\mathbf u_p=f\mathbf B_p$. The [continuity equation](../../../physics.md#continuity-equation) and $\nabla\cdot\mathbf B_p=0$ now yield

$$
0=\nabla\cdot(\rho\mathbf u_p)=\mathbf B_p\cdot\nabla(\rho f),\qquad
\rho f=\kappa(\chi).
$$

Consequently $\kappa$ is the [magnetohydrodynamic mass loading](../../../astrophysical-fluid-dynamics.md#magnetohydrodynamic-mass-loading). Including the [toroidal magnetic field](../../../astrophysical-fluid-dynamics.md#toroidal-magnetic-field), rewrite the full [velocity](../../../classical-mechanics.md#velocity) as

$$
\mathbf u=\frac{\kappa}{\rho}\mathbf B+s\omega\widehat{\boldsymbol\phi},\qquad
\omega=\Omega-\frac{\kappa B_\phi}{\rho s}.
$$

Since $\mathbf u\times\mathbf B=\omega\nabla\chi$, steady ideal induction gives $0=\nabla\omega\times\nabla\chi$. Hence $\omega=\omega(\chi)$, establishing

$$
\boxed{\mathbf u=\rho^{-1}\kappa(\chi)\mathbf B+s\omega(\chi)\widehat{\boldsymbol\phi}.}
$$

The invariant $\omega$ is the [field-line angular velocity of an axisymmetric wind](../../../astrophysical-fluid-dynamics.md#field-line-angular-velocity-of-an-axisymmetric-wind), not generally the fluid's [angular velocity](../../../classical-mechanics.md#angular-velocity) $\Omega$. When an ideal magnetic surface is anchored to a rigidly rotating star, $\omega$ equals the stellar [angular velocity](../../../classical-mechanics.md#angular-velocity). With no poloidal outflow this reduces to [Ferraro's law of isorotation](../../../astrophysical-fluid-dynamics.md#ferraro-s-law-of-isorotation).

To calculate the magnetic [torque](../../../classical-mechanics.md#torque), use the azimuthal momentum equation. Axisymmetric [pressure](../../../thermodynamics.md#pressure) and [Newtonian gravity](../../../classical-mechanics.md#gravitational-acceleration) have no azimuthal components; the magnetic pressure has none either. The azimuthal acceleration and magnetic tension contain the curvature terms characteristic of [cylindrical coordinates](../../../calculus.md#cylindrical-coordinate-system):

$$
\rho\left(\mathbf u_p\cdot\nabla u_\phi+\frac{u_su_\phi}{s}\right)
=\frac1{\mu_0}\left(\mathbf B_p\cdot\nabla B_\phi+\frac{B_sB_\phi}{s}\right).
$$

Multiplication by $s$ gives the [Maxwell torque conservation in an axisymmetric wind](../../../astrophysical-fluid-dynamics.md#maxwell-torque-conservation-in-an-axisymmetric-wind) equation

$$
\rho\mathbf u_p\cdot\nabla(su_\phi)=\frac1{\mu_0}\mathbf B_p\cdot\nabla(sB_\phi).
$$

Using $u_\phi=s\Omega$, $\rho\mathbf u_p=\kappa\mathbf B_p$ and $\mathbf B_p\cdot\nabla\kappa=0$ proves

$$
\mathbf B_p\cdot\nabla\left(\kappa s^2\Omega-\frac{sB_\phi}{\mu_0}\right)=0,\qquad
\boxed{\ell(\chi)=\kappa s^2\Omega-\frac{sB_\phi}{\mu_0}.}
$$

This is the total [angular momentum](../../../classical-mechanics.md#angular-momentum) transport per unit poloidal [magnetic flux](../../../electromagnetism.md#magnetic-flux). The first term is the material contribution and the second is the contribution of the [Maxwell stress tensor](../../../electromagnetism.md#maxwell-stress-tensor). The specific [magnetohydrodynamic angular-momentum invariant](../../../astrophysical-fluid-dynamics.md#magnetohydrodynamic-angular-momentum-invariant) is $L=\ell/\kappa$ when $\kappa\ne0$; its normalization differs from the paper's $\ell$.

Define the poloidal [Alfvén Mach number](../../../astrophysical-fluid-dynamics.md#alfven-mach-number) by

$$
M_A^2=\frac{|\mathbf u_p|^2}{|\mathbf B_p|^2/(\mu_0\rho)}=\frac{\mu_0\kappa^2}{\rho}.
$$

Substituting $\Omega=\omega+\kappa B_\phi/(\rho s)$ into $\ell$ gives

$$
\ell=\kappa s^2\omega+\frac{sB_\phi}{\mu_0}(M_A^2-1).
$$

At a smooth crossing of the [Alfvén surface](../../../astrophysical-fluid-dynamics.md#alfven-surface), $M_A^2=1$ and the [toroidal magnetic field](../../../astrophysical-fluid-dynamics.md#toroidal-magnetic-field) is finite. The [Alfvén-surface regularity condition for an axisymmetric wind](../../../astrophysical-fluid-dynamics.md#alfven-surface-regularity-condition-for-an-axisymmetric-wind) is therefore

$$
\boxed{\ell=\kappa s_A^2\omega,\qquad L=s_A^2\omega.}
$$

One can also expose the apparent singularity explicitly:

$$
B_\phi=\frac{\mu_0\kappa}{s}\frac{L-s^2\omega}{M_A^2-1},\qquad
\Omega=\frac{M_A^2 L/s^2-\omega}{M_A^2-1}.
$$

Finite passage through the [Alfvén surface](../../../astrophysical-fluid-dynamics.md#alfven-surface) requires the numerator to vanish with the denominator. Equality of the numerator zeros is necessary; a globally smooth wind must also satisfy its other dynamical critical conditions. Here $s_A$ is the cylindrical distance from the rotation axis, not automatically the spherical [Alfvén radius](../../../astrophysical-fluid-dynamics.md#alfven-radius).

For a tube carrying outward mass flux $d\dot M=\kappa\mathbf B_p\cdot d\mathbf S$, the outward [angular momentum](../../../classical-mechanics.md#angular-momentum) flux is

$$
d\dot J_{\rm out}=\left(\rho\mathbf u_p s u_\phi-\frac{\mathbf B_p sB_\phi}{\mu_0}\right)\cdot d\mathbf S
=L\,d\dot M=\omega s_A^2\,d\dot M.
$$

Thus the stellar [torque](../../../classical-mechanics.md#torque) is $\dot J_\star=-\int\omega s_A^2\,d\dot M$, with the integral over the escaping wind. **Magnetic stresses give each mass element an effective angular-momentum lever arm equal to the cylindrical Alfvén crossing radius.** In a strongly sub-Alfvénic region the fluid approximately corotates with the magnetic surface; beyond that region it can carry the accumulated [angular momentum](../../../classical-mechanics.md#angular-momentum) away. For an outward field and positive $\omega$, a super-Alfvénic expanding tube with $s>s_A$ has $B_\phi<0$, so the magnetic stress transports positive [angular momentum](../../../classical-mechanics.md#angular-momentum) outwards. If $s_A$ greatly exceeds the stellar surface lever arm, a modest mass-loss rate can cause substantial [wind-driven magnetic braking of a solar-type star](../../../stellar-astrophysics.md#wind-driven-magnetic-braking-of-a-solar-type-star). An unmagnetized outflow would instead carry approximately the material [angular momentum](../../../classical-mechanics.md#angular-momentum) fixed at its launch radius.

## 3

↑ **Parent:** [Paper 38](paper-38.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Take the historical scope to be the state of [solar dynamo](../../../stellar-astrophysics.md#solar-dynamo) theory around 2001. A successful explanation must account for organized patterns, not merely the existence of a [magnetic field](../../../electromagnetism.md#magnetic-field). For the [Sun](../../../stellar-astrophysics.md#sun), the main constraints are the roughly eleven-year [sunspot](../../../stellar-astrophysics.md#sunspot) cycle and twenty-two-year magnetic [solar cycle](../../../stellar-astrophysics.md#solar-cycle); opposite leading polarities in the two hemispheres and reversal between successive cycles according to [Hale's polarity law](../../../stellar-astrophysics.md#hale-s-polarity-law); the equatorward drift of the activity belts in the [solar butterfly diagram](../../../stellar-astrophysics.md#solar-butterfly-diagram); the systematic bipolar-region tilt of [Joy's law](../../../stellar-astrophysics.md#joy-s-law); and reversal of the large-scale polar field near activity maximum. The field is intermittent, with strong [sunspots](../../../stellar-astrophysics.md#sunspot) coexisting with weaker surface [magnetic flux](../../../electromagnetism.md#magnetic-flux), and cycle amplitudes vary, including extended [solar grand minima](../../../stellar-astrophysics.md#solar-grand-minimum) such as the [Maunder minimum](../../../stellar-astrophysics.md#maunder-minimum). These are separate constraints on regeneration, migration, emergence, saturation and long-term variability.

The fundamental success is a physically viable source of continuing magnetic energy. In a highly conducting star the [resistive induction equation](../../../astrophysical-fluid-dynamics.md#resistive-induction-equation) permits stretching and folding to transfer kinetic energy into [magnetic energy](../../../electromagnetism.md#magnetic-energy); [magnetic diffusion](../../../astrophysical-fluid-dynamics.md#magnetic-diffusion) allows changes of topology and opposes amplification. A [kinematic magnetic dynamo](../../../astrophysical-fluid-dynamics.md#kinematic-magnetic-dynamo) can have growing solutions even though the velocity is prescribed, demonstrating the regenerative mechanism. The [Cowling anti-dynamo theorem](../../../astrophysical-fluid-dynamics.md#cowling-anti-dynamo-theorem) rules out a self-sustaining entirely axisymmetric magnetic configuration; an approximately axisymmetric large-scale field can nevertheless be maintained by nonaxisymmetric [convection](../../../fluid-mechanics.md#convection) and its correlations. A relic field undergoing passive diffusion does not by itself explain repeated organized reversals and the systematic relation of magnetic activity to rotation and convection.

A tractable description is a [mean-field dynamo](../../../astrophysical-fluid-dynamics.md#mean-field-dynamo). Split velocity and field into means and fluctuations. Averaging the induction equation gives

$$
\partial_t\overline{\mathbf B}=\nabla\times\left(\overline{\mathbf U}\times\overline{\mathbf B}+\boldsymbol{\mathcal E}-\eta\nabla\times\overline{\mathbf B}\right),\qquad
\boldsymbol{\mathcal E}=\langle\mathbf u'\times\mathbf b'\rangle.
$$

The [mean-field electromotive force](../../../astrophysical-fluid-dynamics.md#mean-field-electromotive-force) is where unresolved correlations enter. A simple local isotropic closure is $\boldsymbol{\mathcal E}=\alpha\overline{\mathbf B}-\eta_t\nabla\times\overline{\mathbf B}$. The [alpha effect](../../../astrophysical-fluid-dynamics.md#alpha-effect) couples the [toroidal magnetic field](../../../astrophysical-fluid-dynamics.md#toroidal-magnetic-field) back to a [poloidal magnetic field](../../../astrophysical-fluid-dynamics.md#poloidal-magnetic-field), while the [Omega effect](../../../astrophysical-fluid-dynamics.md#omega-effect) produces a [toroidal magnetic field](../../../astrophysical-fluid-dynamics.md#toroidal-magnetic-field) from [differential rotation](../../../astrophysical-fluid-dynamics.md#differential-rotation):

$$
(\partial_t\overline B_\phi)_{\Omega}=s\overline{\mathbf B}_p\cdot\nabla\Omega.
$$

In the short-correlation, locally isotropic version of [first-order smoothing](../../../astrophysical-fluid-dynamics.md#first-order-smoothing-approximation), $\alpha\simeq-\tau\langle\mathbf u'\cdot\nabla\times\mathbf u'\rangle/3$ and $\eta_t\simeq\tau\langle|\mathbf u'|^2\rangle/3$. Rotation and stratification can produce [kinetic helicity](../../../fluid-mechanics.md#hydrodynamical-helicity) with opposite signs in the two hemispheres, allowing a hemispherically organized [alpha effect](../../../astrophysical-fluid-dynamics.md#alpha-effect). These formulae explain a possible mechanism, but their controlled assumptions are not automatically satisfied by stellar [turbulence](../../../turbulence.md) at very large [magnetic Reynolds number](../../../astrophysical-fluid-dynamics.md#magnetic-reynolds-number).

An [alpha-Omega dynamo](../../../astrophysical-fluid-dynamics.md#alpha-omega-dynamo) naturally supports oscillation and migration rather than just monotone amplification. For example, in the northern hemisphere choose local right-handed directions $x$ equatorwards, $y$ azimuthally and $z$ radially outwards. With $U_y=Sz$ and poloidal potential $A\widehat{\mathbf y}$, the local equations are

$$
A_t=\alpha B+\eta_T A_{xx},\qquad B_t=S A_x+\eta_T B_{xx},\qquad\eta_T=\eta+\eta_t.
$$

For $e^{pt+ikx}$ the [local alpha-Omega dynamo wave dispersion](../../../astrophysical-fluid-dynamics.md#local-alpha-omega-dynamo-wave-dispersion) is

$$
(p+\eta_Tk^2)^2=i\alpha Sk,\qquad
\operatorname{Re}p=-\eta_Tk^2+\sqrt{|\alpha Sk|/2}.
$$

The growing [Parker dynamo wave](../../../astrophysical-fluid-dynamics.md#parker-dynamo-wave) has phase velocity $-\operatorname{Im}p/k$, equatorward for $\alpha S<0$. Thus a migration direction, an excitation threshold and a finite oscillation period arise from the feedback between the [alpha effect](../../../astrophysical-fluid-dynamics.md#alpha-effect) and shear, rather than being independently imposed. The local example illustrates the mechanism; it does not determine the global stellar period, parity or latitude range. [Dipole and quadrupole parity in a mean-field dynamo](../../../astrophysical-fluid-dynamics.md#dipole-and-quadrupole-parity-in-a-mean-field-dynamo) depend on the spatial coefficients, coupling between hemispheres and boundary conditions.

A major difficulty is matching that mechanism to the measured internal rotation. [Helioseismology](../../../astrophysical-fluid-dynamics.md#helioseismology) constrains [differential rotation](../../../astrophysical-fluid-dynamics.md#differential-rotation) and the [tachocline](../../../stellar-astrophysics.md#tachocline), giving a plausible strong-shear region near the base of the convection zone. At low northern latitudes a positive radial shear combined with the usual positive convective $\alpha$ would give poleward propagation in the simple local wave model, rather than the equatorward [solar butterfly diagram](../../../stellar-astrophysics.md#solar-butterfly-diagram). A different sign or location of the [alpha effect](../../../astrophysical-fluid-dynamics.md#alpha-effect), an [interface solar dynamo](../../../stellar-astrophysics.md#interface-solar-dynamo), and magnetic transport must therefore be examined rather than assuming that any [alpha-Omega dynamo](../../../astrophysical-fluid-dynamics.md#alpha-omega-dynamo) predicts the observed migration. The stable region below the convection zone may store strong toroidal [magnetic flux](../../../electromagnetism.md#magnetic-flux); [magnetic buoyancy](../../../fluid-mechanics.md#magnetic-buoyancy) can then produce rising tubes and bipolar active regions. Flux-tube emergence also has to account for their low latitudes and [Joy's law](../../../stellar-astrophysics.md#joy-s-law) tilts, not simply for a large interior field.

The [Babcock-Leighton mechanism](../../../stellar-astrophysics.md#babcock-leighton-mechanism) supplies a more directly observable route to regeneration. Tilted bipolar regions disperse; cancellation of opposite polarities and poleward transport of surviving flux alter the polar [poloidal magnetic field](../../../astrophysical-fluid-dynamics.md#poloidal-magnetic-field). [Differential rotation](../../../astrophysical-fluid-dynamics.md#differential-rotation) subsequently winds that field into a [toroidal magnetic field](../../../astrophysical-fluid-dynamics.md#toroidal-magnetic-field). A [flux-transport solar dynamo](../../../stellar-astrophysics.md#flux-transport-solar-dynamo) combines this surface source with [meridional circulation in a star](../../../stellar-structure.md#meridional-circulation-in-a-star) and [turbulent magnetic diffusivity](../../../astrophysical-fluid-dynamics.md#turbulent-magnetic-diffusivity). Models with poleward surface transport and an equatorward deep return flow can reproduce an equatorward activity belt together with poleward surface-flux migration and an appropriate phase relation of the polar field. This was already an explicit model construction in the [1999 flux-transport calculation](https://www.researchgate.net/publication/230948034_A_Babcock-Leighton_Flux_Transport_Dynamo_with_Solar-like_Differential_Rotation). Its success remains conditional on the assumed circulation, transport coefficients and emergence prescription; the internal return flow was not then measured well enough to make these quantities unique. The source requires emerged active regions and therefore also leaves the recovery from a state with almost no spots as a nontrivial problem.

Saturation is another limitation of kinematic models. Exponential growth cannot persist indefinitely: the [Lorentz force](../../../electromagnetism.md#lorentz-force) alters the shear and [convection](../../../fluid-mechanics.md#convection), and changes the correlations that generate the [alpha effect](../../../astrophysical-fluid-dynamics.md#alpha-effect). Algebraic [dynamo quenching](../../../astrophysical-fluid-dynamics.md#dynamo-quenching) can produce bounded cycles but fitting a quenching coefficient is not a first-principles amplitude prediction. Near conservation of [magnetic helicity](../../../electromagnetism.md#magnetic-helicity) in a highly conducting fluid adds constraints on the growth and saturation of a large-scale field; boundaries and helicity transport matter. [Magnetic buoyancy](../../../fluid-mechanics.md#magnetic-buoyancy), intermittency and the interaction of mean and fluctuating fields likewise make a local isotropic closure incomplete. Fluctuating regeneration and flow, or nonlinear interactions, can produce cycle irregularity and [solar grand minima](../../../stellar-astrophysics.md#solar-grand-minimum), but reproducing one irregular time series does not establish a unique explanation of the [Maunder minimum](../../../stellar-astrophysics.md#maunder-minimum).

Other solar-type stars provide an important independent test. Long-term [chromosphere](../../../stellar-astrophysics.md#chromosphere) observations already showed both cyclic and irregular activity, with rapidly rotating young stars tending to be more active and older slower rotators more often showing smooth cycles; see the original [stellar activity survey](https://www.researchgate.net/publication/259950104_Chromospheric_variations_in_main-sequence_stars_II). These qualitative trends support a rotational-convective origin and [stellar rotation-activity feedback](../../../stellar-astrophysics.md#stellar-rotation-activity-feedback) through [wind-driven magnetic braking of a solar-type star](../../../stellar-astrophysics.md#wind-driven-magnetic-braking-of-a-solar-type-star). The relevant control need not be rotation alone: the [stellar activity Rossby number](../../../geophysical-fluid-dynamics.md#stellar-activity-rossby-number), comparing rotation and the convection time, expresses why stellar structure matters. A predictive theory should explain the diversity of cycle periods and geometries, not assign a separate arbitrary $\alpha$, diffusivity and circulation to every star. Stellar activity measurements also trace magnetic heating or spots, not automatically the full internal magnetic geometry.

**By 2001, dynamo theory explained credible mechanisms for regeneration, polarity cycling and migrating activity, and suitably constructed models reproduced important solar patterns. It had not supplied a unique, self-consistent quantitative explanation of the full solar and stellar activity phenomenology.** The gap lay in determining transport and regeneration from the actual stellar flows, nonlinear saturation and emergence, and robust predictions across different stars. Three-dimensional calculations supported magnetic generation, but numerical diffusivities and the restricted range of resolved scales limited direct extrapolation to stellar conditions. Agreement of a prescribed-coefficient [mean-field dynamo](../../../astrophysical-fluid-dynamics.md#mean-field-dynamo) with selected observations is meaningful evidence of feasibility, not a demonstration that its detailed mechanism or parameters have been uniquely established.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
