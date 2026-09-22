# Paper 59

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper59.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper59.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 59](paper-59.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Take the equilibrium [mass density](../../../fluid-mechanics.md#density) to be constant and absorb any conservative equilibrium force into the [pressure](../../../thermodynamics.md#pressure). The linearized [ideal magnetohydrodynamic induction equation](../../../astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamic-induction-equation), using the [solenoidal vector field](../../../calculus.md#solenoidal-vector-field) conditions, is

$$
\partial_t\mathbf b=(\mathbf B\cdot\nabla)\mathbf u-(\mathbf u\cdot\nabla)\mathbf B.
$$

For $\mathbf B=Jr\mathbf e_\phi$, differentiation of the cylindrical basis is important. Acting on a vector whose cylindrical components have azimuthal dependence $e^{im\phi}$ gives $(\mathbf B\cdot\nabla)\mathbf u=imJ\mathbf u+J\mathbf e_z\times\mathbf u$. Also $(\mathbf u\cdot\nabla)\mathbf B=J\mathbf e_z\times\mathbf u$. These basis contributions cancel in induction, giving **$i\omega\mathbf b=imJ\mathbf u$**.

The perturbation of the [Lorentz force](../../../electromagnetism.md#lorentz-force) is

$$
(\nabla\times\mathbf b)\times\mathbf B+(\nabla\times\mathbf B)\times\mathbf b=(\mathbf B\cdot\nabla)\mathbf b+(\mathbf b\cdot\nabla)\mathbf B-\nabla(\mathbf B\cdot\mathbf b).
$$

Both of the first two terms now contribute a basis-rotation term. With $\widetilde p=p_1/\rho+\mathbf B\cdot\mathbf b/(\mu_0\rho)$, the linearized [ideal magnetohydrodynamic momentum equation](../../../astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamic-momentum-equation) is therefore

$$
\boxed{i\omega\mathbf u=-\nabla\widetilde p+\frac1{\mu_0\rho}(imJ\mathbf b+2J\mathbf e_z\times\mathbf b),\qquad i\omega\mathbf b=imJ\mathbf u.}
$$

The magnetic part of $\widetilde p$ is the perturbation of [magnetic pressure](../../../astrophysical-fluid-dynamics.md#magnetic-pressure), not an extra restoring force to retain after projecting out [pressure](../../../thermodynamics.md#pressure).

Put $D=\omega^2-m^2\widetilde J^2$, where $\widetilde J=J/\sqrt{\mu_0\rho}$. For $mJ\ne0$, substitute $\mathbf u=\omega\mathbf b/(mJ)$ into the momentum equation and multiply by $mJ$. Taking a curl removes the modified [pressure](../../../thermodynamics.md#pressure). Since

$$
\nabla\times(\mathbf e_z\times\mathbf b)=\mathbf e_z\nabla\cdot\mathbf b-\partial_z\mathbf b=-ik\mathbf b,
$$

we obtain the [uniform-current toroidal-field curl reduction](../../../astrophysical-fluid-dynamics.md#uniform-current-toroidal-field-curl-reduction)

$$
D\nabla\times\mathbf b=-2mk\widetilde J^2\mathbf b.
$$

A second curl, using $\nabla\times\nabla\times\mathbf b=-\nabla^2\mathbf b$, gives

$$
\boxed{\nabla^2\mathbf b=-\frac{4m^2k^2\widetilde J^4}{(\omega^2-m^2\widetilde J^2)^2}\mathbf b.}
$$

The divided expression assumes $D\ne0$. If $mkJ\ne0$, the undivided curl equation shows that $D=0$ would force $\mathbf b=0$, so this restriction loses no such magnetic mode. The $k=0$ degenerate limit can instead be taken in the undivided equations; it has no growing branch of the kind considered below. Axisymmetric $m=0$ disturbances are likewise excluded by the [velocity](../../../classical-mechanics.md#velocity) elimination, and induction gives no nonzero-frequency magnetic disturbance in this particular equilibrium.

For a vector Laplacian eigenmode with $\alpha^2+k^2>0$, elimination gives

$$
D^2=\frac{4m^2k^2\widetilde J^4}{\alpha^2+k^2},\qquad \boxed{\omega^2_\pm=\widetilde J^2\left(m^2\pm\frac{2|mk|}{\sqrt{\alpha^2+k^2}}\right).}
$$

Thus **both squared frequencies are real**. The lower branch satisfies $\omega_-^2\geq\widetilde J^2(|m|^2-2|m|)$, so it is positive for $|m|>2$. For $|m|=2$ it is positive when $\alpha\ne0$, but the printed strict-positivity statement needs an endpoint qualification: **$|m|=2$, $\alpha=0$ permits a neutral mode unless boundary conditions exclude it**.

This is a genuine counterexample to the unqualified endpoint, not merely a loose algebraic bound. The [neutral quadrupolar perturbation of a uniform-current toroidal field](../../../astrophysical-fluid-dynamics.md#neutral-quadrupolar-perturbation-of-a-uniform-current-toroidal-field)

$$
\mathbf b=Cr(\mathbf e_r+i\mathbf e_\phi)e^{2i\phi+ikz},\qquad \mathbf u=0,\qquad \widetilde p=0,\qquad \omega=0
$$

is regular at the axis, is solenoidal, and has $\nabla\times\mathbf b=k\mathbf b$, hence $\nabla^2\mathbf b=-k^2\mathbf b$. Also $\mathbf e_z\times\mathbf b=-i\mathbf b$, so the non-gradient part of the linearized [Lorentz force](../../../electromagnetism.md#lorentz-force) vanishes for $m=2$. The gas-pressure perturbation $p_1=-\mathbf B\cdot\mathbf b/\mu_0$ cancels its [magnetic pressure](../../../astrophysical-fluid-dynamics.md#magnetic-pressure) gradient, as required by $\widetilde p=0$. Taking its real part gives a real disturbance. Decay at radial infinity or an appropriate homogeneous radial boundary condition would exclude it, restoring strict positivity for the allowed eigenmodes; no such condition is printed.

For $|m|=1$ the lower branch is unstable precisely when

$$
\boxed{m=\pm1,\qquad k\ne0,\qquad \alpha^2<3k^2.}
$$

At equality it is marginal. With the time convention $e^{i\omega t}$, the growing member has $\omega=-is$ and

$$
s=|\widetilde J|\sqrt{\frac{2|k|}{\sqrt{\alpha^2+k^2}}-1}.
$$

The other branch remains oscillatory. Actual admissibility of a chosen $\alpha$ depends on the radial domain and its [boundary conditions](../../../differential-equation.md#boundary-condition).

## 2

↑ **Parent:** [Paper 59](paper-59.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Write the inward radial [velocity](../../../classical-mechanics.md#velocity) as $u_R=-v(R)$, with $v>0$. Steady spherical [mass conservation](../../../continuum-mechanics.md#mass-conservation) and the radial [Euler equations for an inviscid fluid](../../../fluid-mechanics.md#euler-equations-for-an-inviscid-fluid) give

$$
\boxed{\dot M=4\pi R^2\rho v=\text{constant}>0,\qquad vv'=-\frac1\rho p'-\Phi'.}
$$

For a [barotropic fluid](../../../fluid-mechanics.md#barotropic-fluid), define the [sound speed](../../../compressible-flow.md#speed-of-sound) $c_s^2=dp/d\rho>0$ and the [barotropic enthalpy function](../../../fluid-mechanics.md#barotropic-enthalpy-function) by $dh=dp/\rho$. Choosing $\Phi(\infty)=0$, integration gives the [Bernoulli equation](../../../fluid-mechanics.md#bernoulli-equation)

$$
\frac{v^2}{2}+h(\rho)+\Phi=h(\rho_\infty),\qquad p(\rho_\infty)=p_0.
$$

The continuity equation gives $\rho'/\rho=-2/R-v'/v$. Eliminating [mass density](../../../fluid-mechanics.md#density) from the momentum equation produces the [barotropic spherical accretion equation](../../../fluid-mechanics.md#barotropic-spherical-accretion-equation)

$$
\boxed{\left(v-\frac{c_s^2}{v}\right)v'=\frac{2c_s^2}{R}-\Phi'.}
$$

The [sonic point](../../../compressible-flow.md#sonic-point) is where the inward [Mach number](../../../compressible-flow.md#mach-number) $v/c_s$ equals one. A smooth solution cannot cross the vanishing coefficient on the left with a nonzero right-hand side, so a regular sonic radius must obey

$$
v_s=c_{s,s},\qquad c_{s,s}^2=\frac{R_s\Phi'(R_s)}2.
$$

Conversely a continuous flow that is subsonic at infinity and supersonic inward must cross unit [Mach number](../../../compressible-flow.md#mach-number); smooth passage selects a simultaneous zero of the two sides, hence a regular [sonic point](../../../compressible-flow.md#sonic-point). The associated critical accretion branch, rather than an arbitrary subsonic solution with smaller flux, is selected by these outer and inner requirements.

For the [polytropic equation of state](../../../astrophysical-fluid-dynamics.md#polytropic-equation-of-state), set $\Gamma=1+1/m$ to distinguish its exponent from any separately specified perturbation exponent. Assume $K>0$ and first take the usual positive index $m>0$. Then

$$
c_s^2=\Gamma K\rho^{1/m},\qquad h=mc_s^2,\qquad \rho_\infty=(p_0/K)^{m/(m+1)},\qquad c_\infty^2=\Gamma p_0/\rho_\infty.
$$

For the attractive mixed potential, assume $\lambda,\mu>0$. The sonic condition and [Bernoulli equation](../../../fluid-mechanics.md#bernoulli-equation) give

$$
c_{s,s}^2=\frac\lambda{R_s^2}+\frac\mu{2R_s},\qquad (m+\tfrac12)c_{s,s}^2-\frac\lambda{R_s^2}-\frac\mu{R_s}=mc_\infty^2.
$$

Hence [polytropic accretion in a mixed inverse-power potential](../../../fluid-mechanics.md#polytropic-accretion-in-a-mixed-inverse-power-potential) reduces to

$$
mc_\infty^2R_s^2-\frac{2m-3}{4}\mu R_s-\frac{2m-1}{2}\lambda=0.
$$

For $0<m\leq1/2$ all nonzero coefficients in the left side are nonnegative for $R_s>0$, with at least one strictly positive: there is no finite positive root. For $m>1/2$ the constant term is negative and the leading coefficient positive, giving exactly one positive root. Define $B=(2m-3)\mu/4$ and $C=(2m-1)\lambda/2$. Then

$$
\boxed{m>\tfrac12\quad(1<\Gamma<3),\qquad R_s=\frac{B+\sqrt{B^2+4mc_\infty^2C}}{2mc_\infty^2}.}
$$

This is the finite-radius transonic range for the two positive attractive terms.

The critical point has real distinct crossing slopes. To check this rather than just solve the sonic equalities, put $U=\lambda/R_s^2$, $V=\mu/(2R_s)$ and $x=R_sv_s'/v_s$. Differentiating the [barotropic spherical accretion equation](../../../fluid-mechanics.md#barotropic-spherical-accretion-equation) at its simultaneous zero gives

$$
(2m+1)x^2+4x+4+2m-m\frac{6U+4V}{U+V}=0.
$$

Its [discriminant](../../../polynomial.md#discriminant) is $8m[2(2m-1)U+(2m-3)V]/(U+V)$. The sonic [Bernoulli equation](../../../fluid-mechanics.md#bernoulli-equation) says $(2m-1)U+(2m-3)V=2mc_\infty^2$, so this [discriminant](../../../polynomial.md#discriminant) is strictly positive for $m>1/2$. The accretion crossing is the slope for which $d\log(v/c_s)/d\log R<0$, namely the smaller root. The two slopes have opposite signs of this Mach-number derivative. This is the regular transonic saddle, not a singular vertical tangent.

The corresponding [mass accretion rate](../../../astrophysics.md#mass-accretion-rate) follows without an additional arbitrary [mass density](../../../fluid-mechanics.md#density) normalization:

$$
\rho_s=\rho_\infty\left(\frac{c_{s,s}^2}{c_\infty^2}\right)^m,\qquad \boxed{\dot M=4\pi R_s^2\rho_\infty c_{s,s}\left(\frac{c_{s,s}^2}{c_\infty^2}\right)^m.}
$$

One may equivalently replace $\rho_s$ by $[c_{s,s}^2/(\Gamma K)]^m$. With a nonzero $\lambda$ term, inner free fall has $v\sim\sqrt{2\lambda}/R$ and continuity gives $\rho\propto R^{-1}$. Thus $v^2/c_s^2\propto R^{-2+1/m}$ increases without bound precisely in the positive-index range $m>1/2$, consistent with the required inner supersonic branch.

The assumptions on the parameters matter. If $\lambda=0$ and $\mu>0$, the finite sonic radius instead requires $m>3/2$, the usual [Bondi accretion](../../../astrophysics.md#bondi-accretion) range; $m=3/2$ is the zero-radius limiting critical case. If $\mu=0$ and $\lambda>0$, the condition remains $m>1/2$. With arbitrary signs of $\lambda,\mu$, one must use the quadratic and retain only positive roots with $c_{s,s}^2>0$ and real admissible crossing slopes; attraction was not explicitly given as a sign condition in the source.

If positive polytropic index was not intended as an implicit physical convention, there is a further mathematical range. For $K>0$, positive compressibility also permits $m<-1$, giving $0<\Gamma<1$. Both potential terms attractive then give a positive sonic root as well:

$$
R_s=\frac{B-\sqrt{B^2+4mc_\infty^2C}}{2mc_\infty^2}>0.
$$

The same [mass accretion rate](../../../astrophysics.md#mass-accretion-rate) formula applies; its crossing-slope [discriminant](../../../polynomial.md#discriminant) is positive. The range $-1<m<0$ has $c_s^2<0$ and no physical acoustic sonic point, $m=-1$ has constant [pressure](../../../thermodynamics.md#pressure) and zero [sound speed](../../../compressible-flow.md#speed-of-sound), and $m=0$ does not define the printed equation of state. Thus the usual answer $m>1/2$ assumes $m>0$ and positive attractive coefficients; these conventions should not be confused with additional printed restrictions.

## 3

↑ **Parent:** [Paper 59](paper-59.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Assume a nonrotating, nonmagnetic equilibrium, inviscid adiabatic perturbations, and no dissipation. Let $g=\phi'(R)>0$, so [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) is $p'=-\rho g$. Use $\boldsymbol\xi e^{i\omega t}$ for the [fluid displacement](../../../fluid-mechanics.md#lagrangian-displacement-fluid-mechanics). To avoid a source ambiguity, write [Eulerian fluid perturbations](../../../fluid-mechanics.md#eulerian-fluid-perturbation) as $p_1,\rho_1,\phi_1$, and use $\Delta$ for quantities following the displaced material element, as in [Eulerian and Lagrangian fluid perturbations](../../../fluid-mechanics.md#eulerian-and-lagrangian-fluid-perturbations). They are related by $\Delta p=p_1+\xi_Rp'$ and similarly for [mass density](../../../fluid-mechanics.md#density) and potential.

The printed identity needs two corrections: its compression denominator must be **$\gamma p$, not $\gamma\rho$**, and the [pressure](../../../thermodynamics.md#pressure) and potential appearing in this form of the identity must be **[Eulerian fluid perturbations](../../../fluid-mechanics.md#eulerian-fluid-perturbation)**. The printed denominator has the wrong dimensions for an [energy density](../../../statistical-physics.md#energy-density). The claimed Lagrangian interpretation does not produce the displayed buoyancy-compression split; the following derivation specifies the consistent version.

Linearized [mass conservation](../../../continuum-mechanics.md#mass-conservation), the adiabatic relation, and the [Poisson equation](../../../partial-differential-equation.md#poisson-equation) give

$$
\boxed{\rho_1=-\nabla\cdot(\rho\boldsymbol\xi),\qquad \Delta p=-\gamma p\nabla\cdot\boldsymbol\xi,\qquad \nabla^2\phi_1=4\pi G\rho_1.}
$$

Consequently $p_1=-\gamma p\nabla\cdot\boldsymbol\xi-\xi_Rp'$. Linearizing the [Euler equations for an inviscid fluid](../../../fluid-mechanics.md#euler-equations-for-an-inviscid-fluid) about the static star gives the [linear adiabatic stellar oscillation equations](../../../astrophysical-fluid-dynamics.md#linear-adiabatic-stellar-oscillation-equations)

$$
-\omega^2\rho\boldsymbol\xi=-\nabla p_1-\rho_1\nabla\phi-\rho\nabla\phi_1.
$$

Require regularity at the center, a vanishing Lagrangian surface [pressure](../../../thermodynamics.md#pressure), and the usual matching to a decaying exterior gravitational potential. Because $p$ and $\rho$ vanish at the surface, the [pressure](../../../thermodynamics.md#pressure) boundary term vanishes for regular displacements; compactly supported trials also suffice below. The perturbed [Newtonian gravitational potential](../../../classical-mechanics.md#newtonian-gravitational-potential) solves Laplace's equation outside the star and must be included there when its field energy is computed.

Multiply the momentum equation by $-\boldsymbol\xi^*$ and integrate. The [pressure](../../../thermodynamics.md#pressure) term is $-\int_Vp_1\nabla\cdot\boldsymbol\xi^*\,dV$. Let $d=\nabla\cdot\boldsymbol\xi$. The adiabatic relation and [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) imply

$$
d=\frac{\rho g\xi_R-p_1}{\gamma p},\qquad \rho_1=\frac{\rho p_1}{\gamma p}-\left(\frac{\rho^2g}{\gamma p}+\rho'\right)\xi_R.
$$

The [pressure](../../../thermodynamics.md#pressure) and equilibrium-gravity terms then combine pointwise as

$$
-p_1d^*+g\rho_1\xi_R^*=\frac{|p_1|^2}{\gamma p}-\left(\frac{\rho^2g^2}{\gamma p}+g\rho'\right)|\xi_R|^2=\frac{|p_1|^2}{\gamma p}+\rho N^2|\xi_R|^2,
$$

where $N^2=g[(1/\gamma)p'/p-\rho'/\rho]$ is the [stellar buoyancy frequency](../../../gravity-wave.md#stellar-buoyancy-frequency). The potentially troublesome cross terms cancel exactly.

For the perturbed [self-gravity](../../../classical-mechanics.md#self-gravity) term, integration by parts gives

$$
\int_V\rho\boldsymbol\xi^*\cdot\nabla\phi_1\,dV=\int_V\rho_1^*\phi_1\,dV=\frac1{4\pi G}\int_{\mathbb R^3}\phi_1\nabla^2\phi_1^*\,dV=-\frac1{4\pi G}\int_{\mathbb R^3}|\nabla\phi_1|^2\,dV.
$$

Thus the corrected [stellar displacement energy identity](../../../astrophysical-fluid-dynamics.md#stellar-displacement-energy-identity) is

$$
\boxed{\omega^2\int_V\rho|\boldsymbol\xi|^2\,dV=-\frac1{4\pi G}\int_{\mathbb R^3}|\nabla\phi_1|^2\,dV+\int_V\left(\frac{|p_1|^2}{\gamma p}+\rho N^2|\xi_R|^2\right)dV.}
$$

The right side is a real [quadratic form](../../../linear-algebra.md#quadratic-form). With these conservative [boundary conditions](../../../differential-equation.md#boundary-condition), the force operator is a [self-adjoint operator](../../../linear-operator-theory.md#self-adjoint-operator). Its [Rayleigh quotient](../../../linear-operator-theory.md#rayleigh-quotient) characterizes squared mode frequencies, and a negative admissible trial quotient proves an unstable spectral component; it does not require the trial displacement itself to be an exact [eigenfunction](../../../linear-operator-theory.md#eigenfunction).

For a generic compressive disturbance of scale $\ell$ in a region with slowly varying equilibrium coefficients, estimate $\rho_1\sim\rho\xi/\ell$, $p_1\sim\gamma p\xi/\ell$ and $\phi_1\sim4\pi G\rho_1\ell^2$. The [self-gravity](../../../classical-mechanics.md#self-gravity) and compression energy densities have orders

$$
|E_g|/V\sim4\pi G\rho^2\xi^2,\qquad E_p/V\sim\rho c_s^2\xi^2/\ell^2,\qquad \frac{|E_g|}{E_p}\sim\frac{4\pi G\rho\ell^2}{c_s^2},
$$

with [adiabatic sound speed](../../../compressible-flow.md#adiabatic-sound-speed) $c_s^2=\gamma p/\rho$. Under the plausible stellar estimate $c_s^2\sim G\bar\rho a^2$, global modes can have comparable gravity and [pressure](../../../thermodynamics.md#pressure) contributions, while their ratio for small-scale compressive modes is of order $(\rho/\bar\rho)(\ell/a)^2$. Thus perturbations with $\ell\ll c_s/\sqrt{4\pi G\rho}$ admit the [Cowling approximation](../../../astrophysical-fluid-dynamics.md#cowling-approximation). This estimate compares two nonzero compressive terms; it cannot alone justify neglecting gravity for a trial deliberately chosen to have $p_1=0$.

For an explicit convective trial, choose $c<d<e<b$ and a nonzero smooth bump

$$
f(R)=\begin{cases}\varepsilon\exp\!\left[-\dfrac{(e-d)^2}{(R-d)(e-R)}\right],&d<R<e,\\0,&\text{otherwise.}\end{cases}
$$

Let $Y$ be a normalized [spherical harmonic](../../../analysis.md#spherical-harmonic) of degree $\ell\geq1$, let $L=\ell(\ell+1)$, and let $\nabla_\Omega$ be the unit-sphere gradient. The [pressure-free localized stellar convective trial](../../../astrophysical-fluid-dynamics.md#pressure-free-localized-stellar-convective-trial) is

$$
\boxed{\boldsymbol\xi=fY\mathbf e_R+h\nabla_\Omega Y,\qquad h=\frac R L\left[\frac{(R^2f)'}{R^2}-\frac{\rho g}{\gamma p}f\right].}
$$

It is supported away from the center and surface, so it satisfies every needed mechanical boundary condition. Since $\Delta_\Omega Y=-LY$,

$$
\nabla\cdot\boldsymbol\xi=\left[\frac{(R^2f)'}{R^2}-\frac LRh\right]Y=\frac{\rho g}{\gamma p}fY.
$$

Therefore $p_1=-\gamma p\nabla\cdot\boldsymbol\xi+\rho g\xi_R=0$ exactly. Its [buoyancy](../../../fluid-mechanics.md#buoyancy) energy is $\int_d^e\rho N^2R^2|f|^2dR<0$, whereas its kinetic norm $\int_d^e\rho R^2(|f|^2+L|h|^2)dR$ is positive. In the [Cowling approximation](../../../astrophysical-fluid-dynamics.md#cowling-approximation) this gives a negative [Rayleigh quotient](../../../linear-operator-theory.md#rayleigh-quotient), and hence **$N^2<0$ in an interior shell implies convective instability**. Retaining perturbed [self-gravity](../../../classical-mechanics.md#self-gravity) only adds a nonpositive term, so the same trial proves instability in the full conservative problem too.

There is also a quantitative small-scale check for this very trial. Its [mass density](../../../fluid-mechanics.md#density) amplitude is $\rho_1=(\rho N^2/g)fY$, independent of $\ell$. Write $\rho_1=s(R)Y$ and $\phi_1=F(R)Y$. The radial [Poisson equation](../../../partial-differential-equation.md#poisson-equation) gives

$$
A=\int_0^\infty\left(R^2|F'|^2+L|F|^2\right)dR=-4\pi G\int_0^\infty R^2F^*s\,dR.
$$

By the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality), $A\leq4\pi G(\int R^4|s|^2dR)^{1/2}(A/L)^{1/2}$, and so the [angular-degree bound on perturbed stellar self-gravity](../../../astrophysical-fluid-dynamics.md#angular-degree-bound-on-perturbed-stellar-self-gravity) is

$$
|E_g|=\frac A{4\pi G}\leq\frac{4\pi G}{\ell(\ell+1)}\int_d^eR^4|s|^2dR.
$$

It tends to zero with horizontal scale $R/\ell$, while the strictly negative [buoyancy](../../../fluid-mechanics.md#buoyancy) integral is fixed. This justifies the small-scale neglect of gravity even though the trial's compression term vanishes.

## 4

↑ **Parent:** [Paper 59](paper-59.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [magnetorotational instability](../../../astrophysics.md#magnetorotational-instability) extracts energy from [differential rotation](../../../astrophysical-fluid-dynamics.md#differential-rotation) through [magnetic tension](../../../astrophysical-fluid-dynamics.md#magnetic-tension). It can destabilize a disk whose specific [angular momentum](../../../classical-mechanics.md#angular-momentum) increases outward, even though such a disk satisfies [Rayleigh's circulation criterion](../../../hydrodynamic-stability.md#rayleigh-s-circulation-criterion). The distinction is that an unmagnetized displaced parcel approximately conserves its own [angular momentum](../../../classical-mechanics.md#angular-momentum), whereas a field line transfers [angular momentum](../../../classical-mechanics.md#angular-momentum) between parcels. If [angular velocity](../../../classical-mechanics.md#angular-velocity) decreases outward, an outward-displaced parcel lags its inner partner. Magnetic tension transfers [angular momentum](../../../classical-mechanics.md#angular-momentum) to the outer parcel and removes it from the inner one, making their radial separation increase. A sufficiently stiff magnetic connection suppresses the separation instead. The instability therefore requires a finite range of field-line-bending strengths.

Make this mechanism quantitative in the local [shearing sheet](../../../gravitational-instability-of-an-astrophysical-disk.md#shearing-sheet) of a cylindrical rotation profile $\Omega(r)$. Put $q=-d\log\Omega/d\log r$, and take $0<q<2$ so the unmagnetized flow is stable. Its [radial epicyclic frequency](../../../astrophysics.md#radial-epicyclic-frequency) is $\kappa^2=2(2-q)\Omega^2$. Let the uniform field be vertical, $B_z\mathbf e_z$, with constant [mass density](../../../fluid-mechanics.md#density), and use an axisymmetric horizontal disturbance proportional to $e^{st+ikz}$. Write $\mathbf h=\mathbf b/\sqrt{\mu_0\rho}$ and $\omega_A=kB_z/\sqrt{\mu_0\rho}$. The linearized [ideal magnetohydrodynamics](../../../astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamics) equations are

$$
\begin{aligned}
su_r-2\Omega u_\phi&=i\omega_Ah_r,&su_\phi+(2-q)\Omega u_r&=i\omega_Ah_\phi,\\
sh_r&=i\omega_Au_r,&sh_\phi&=-q\Omega h_r+i\omega_Au_\phi.
\end{aligned}
$$

The first pair contains [Coriolis acceleration](../../../physics.md#coriolis-acceleration) and the epicyclic response; the last equation is the shear-winding of a radial field perturbation into an azimuthal one. Omitting that winding term would remove the driving mechanism.

Eliminating $h_r,h_\phi$ gives $(s^2+\omega_A^2)u_r=2\Omega s u_\phi$ and $s(s^2+\omega_A^2)u_\phi+\Omega[(2-q)s^2-q\omega_A^2]u_r=0$. Their determinant is the [ideal magnetorotational dispersion relation](../../../astrophysics.md#ideal-magnetorotational-dispersion-relation)

$$
\boxed{s^4+(2\omega_A^2+\kappa^2)s^2+\omega_A^2(\omega_A^2-2q\Omega^2)=0.}
$$

Its [discriminant](../../../polynomial.md#discriminant) as a quadratic in $s^2$ is $\kappa^4+16\Omega^2\omega_A^2>0$. Since $2\omega_A^2+\kappa^2>0$, a positive $s^2$ exists precisely when its constant term is negative:

$$
\boxed{0<\omega_A^2<2q\Omega^2=-\frac{d\Omega^2}{d\log r}.}
$$

Thus [angular velocity](../../../classical-mechanics.md#angular-velocity), rather than specific [angular momentum](../../../classical-mechanics.md#angular-momentum), must decrease outward. A Keplerian disk has $q=3/2$, $\kappa^2=\Omega^2$ and is hydrodynamically stable, yet magnetic modes with $0<k^2v_A^2<3\Omega^2$ grow.

The growing root is $s^2=-\omega_A^2-\kappa^2/2+\tfrac12\sqrt{\kappa^4+16\Omega^2\omega_A^2}$. Differentiation with respect to $\omega_A^2$ gives the [maximum growth rate of ideal magnetorotational instability](../../../astrophysics.md#maximum-growth-rate-of-ideal-magnetorotational-instability):

$$
\boxed{s_{\max}=\frac{q\Omega}2,\qquad \omega_{A,\max}^2=\frac{q(4-q)}4\Omega^2.}
$$

For Keplerian shear these are $3\Omega/4$ and $15\Omega^2/16$. The ideal maximum is set by shear; reducing field strength reduces the fastest wavelength instead of reducing this maximum growth rate. This is why the exactly zero-field problem differs from a sequence of weak-field problems with progressively larger [wave number](../../../wave-equation.md#wavenumber). At fixed [wave number](../../../wave-equation.md#wavenumber), growth does tend to zero as the field vanishes. The wavelength must fit the actual disk, and diffusion eventually matters at sufficiently short scales.

The instability has the required angular-momentum-transfer sign. In a growing mode, $u_\phi/u_r=(s^2+\omega_A^2)/(2\Omega s)>0$. At the fastest mode this ratio is one, while induction gives $h_\phi=-h_r$ after allowing for their common Fourier phase. Thus the averaged [Reynolds stress](../../../turbulence.md#reynolds-stress) minus [Maxwell stress tensor](../../../electromagnetism.md#maxwell-stress-tensor), $\rho\langle u_ru_\phi-h_rh_\phi\rangle$, is positive: [angular momentum](../../../classical-mechanics.md#angular-momentum) moves outward. Its product with $q\Omega$ is the energy supplied by the background shear. These local mechanisms and coefficient conventions are also checked in [the primary MRI stability calculation](https://www.damtp.cam.ac.uk/user/gio10/dad14.pdf).

More general fields require separating field-line bending from field gradients and curvature. At leading local order, for a stationary compatible field in an [incompressible flow](../../../fluid-mechanics.md#incompressible-flow) with axisymmetric wavevector $(k_r,0,k_z)$, the bending frequency is

$$
\omega_A=\frac{\mathbf k\cdot\mathbf B}{\sqrt{\mu_0\rho}},\qquad k^2=k_r^2+k_z^2.
$$

[Pressure](../../../thermodynamics.md#pressure) elimination projects the radial force by $f=k_z^2/k^2$. The radial momentum equation becomes $su_r-2f\Omega u_\phi=i\omega_Ah_r$; the azimuthal and induction equations retain the form above. Eliminating the amplitudes gives the [oblique axisymmetric magnetorotational dispersion relation](../../../astrophysics.md#oblique-axisymmetric-magnetorotational-dispersion-relation)

$$
\boxed{\frac{k^2}{k_z^2}(s^2+\omega_A^2)^2+\kappa^2(s^2+\omega_A^2)-4\Omega^2\omega_A^2=0.}
$$

Here $k_z\ne0$. The unstable range is $0<\omega_A^2<-f\,d\Omega^2/d\log r$. The [poloidal magnetic field](../../../astrophysical-fluid-dynamics.md#poloidal-magnetic-field) therefore determines whether an axisymmetric perturbation bends a field line. A locally uniform [toroidal magnetic field](../../../astrophysical-fluid-dynamics.md#toroidal-magnetic-field) does not enter $\mathbf k\cdot\mathbf B$ for axisymmetry, and can contribute [magnetic pressure](../../../astrophysical-fluid-dynamics.md#magnetic-pressure) that is projected out of this incompressible leading-order problem. Thus a toroidal component does not suppress the weak-field MRI merely by being present. Conversely a purely toroidal field has no ordinary axisymmetric local bending MRI in this approximation. This does not imply that every globally curved toroidal equilibrium is stable.

A steady general [poloidal magnetic field](../../../astrophysical-fluid-dynamics.md#poloidal-magnetic-field) must also be compatible with the equilibrium rotation. The azimuthal [ideal magnetohydrodynamic induction equation](../../../astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamic-induction-equation) contains $\partial_tB_\phi=r\mathbf B_p\cdot\nabla\Omega$. A stationary axisymmetric equilibrium with no meridional flow consequently requires $\mathbf B_p\cdot\nabla\Omega=0$, [Ferraro's law of isorotation](../../../astrophysical-fluid-dynamics.md#ferraro-s-law-of-isorotation). A radial field crossing cylindrical differential-rotation surfaces would otherwise wind secularly; it cannot simply be substituted into a stationary normal-mode calculation. Boundary conditions and the along-field eigenvalue problem replace a freely chosen local $k$ in nonuniform or bounded equilibria. Strong enough field-line tension can then stabilize all admissible wavelengths.

An explicit axisymmetric effect of nonuniform field strength and curvature is obtained with a purely toroidal field $B_\phi(r)\mathbf e_\phi$, constant [mass density](../../../fluid-mechanics.md#density) and cylindrical rotation. A radial [fluid displacement](../../../fluid-mechanics.md#lagrangian-displacement-fluid-mechanics) changes the field by

$$
b_\phi=\left(\frac{B_\phi}{r}-B_\phi'\right)\xi_r.
$$

This follows directly from $\mathbf b=\nabla\times(\boldsymbol\xi\times\mathbf B)$ and incompressibility. Its radial curvature force, after absorbing the magnetic-pressure perturbation, is $-2B_\phi b_\phi/(\mu_0\rho r)$. The axisymmetric azimuthal momentum equation is $su_\phi+(2\Omega+r\Omega')u_r=0$. Combining it with the radial force and then projecting out [pressure](../../../thermodynamics.md#pressure) gives

$$
\boxed{\omega^2=\frac{k_z^2}{k^2}\mathcal D,\qquad \mathcal D=\kappa^2-\frac r{\mu_0\rho}\frac{d}{dr}\left(\frac{B_\phi}{r}\right)^2.}
$$

This is the local [Michael criterion for axisymmetric toroidal-field interchange](../../../astrophysical-fluid-dynamics.md#michael-criterion-for-axisymmetric-toroidal-field-interchange). The new term can either stabilize or destabilize: for $B_\phi\propto r^p$, $\mathcal D=\kappa^2+2(1-p)v_{A\phi}^2/r^2$. A current-free $B_\phi\propto r^{-1}$ is stabilizing; $B_\phi\propto r$ leaves this axisymmetric interchange coefficient unchanged; a sufficiently steep increase with $p>1$ can destabilize even a centrifugally stable rotation law. That last instability can persist without differential rotation, so its energy source is the magnetic-current equilibrium rather than the ordinary MRI. Nonaxisymmetric current-driven modes are outside the requested essay scope.

For mixed poloidal and toroidal fields, the full induction perturbation contains $(\mathbf B\cdot\nabla)\boldsymbol\xi-(\boldsymbol\xi\cdot\nabla)\mathbf B-\mathbf B\nabla\cdot\boldsymbol\xi$, and the linear [Lorentz force](../../../electromagnetism.md#lorentz-force) contains both $(\nabla\times\mathbf b)\times\mathbf B$ and $(\nabla\times\mathbf B)\times\mathbf b$. These terms explain why gradients and curvature cannot be replaced everywhere by a scalar $k^2v_A^2$: they can draw on equilibrium-current energy and couple the radial and vertical motions. Compressibility introduces additional [magnetic pressure](../../../astrophysical-fluid-dynamics.md#magnetic-pressure) and magnetosonic responses; a strong toroidal field can alter the dispersion even though it disappeared from the leading incompressible weak-field result.

Finally, a vertically or radially stratified general field also supports part of the equilibrium weight through [magnetic pressure](../../../astrophysical-fluid-dynamics.md#magnetic-pressure). A displaced flux tube carries its frozen-in mass-to-flux relation, so its [mass density](../../../fluid-mechanics.md#density) at the surrounding total [pressure](../../../thermodynamics.md#pressure) can differ from its new environment. This introduces [magnetic buoyancy instability](../../../astrophysical-fluid-dynamics.md#magnetic-buoyancy-instability) and competition with ordinary [buoyancy](../../../fluid-mechanics.md#buoyancy). Axisymmetric interchange displacements can access this energy without an azimuthal [wave number](../../../wave-equation.md#wavenumber), while poloidal tension resists variation along the field. Growth that survives when $d\Omega/dr=0$ must not be attributed to shear-driven MRI. The general-field stability problem therefore combines shear, field-line tension, current/curvature forces, compressibility, [buoyancy](../../../fluid-mechanics.md#buoyancy) and boundary constraints; the uniform-field result isolates the basic angular-momentum feedback mechanism.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
