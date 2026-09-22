# Paper 49

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper49.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper49.pdf)

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

↑ **Parent:** [Paper 49](paper-49.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Let $p$ be [kinematic pressure](../../../thermodynamics.md#kinematic-pressure), with the resting hydrostatic part subtracted, and let $\sigma$ be the [buoyancy perturbation](../../../fluid-mechanics.md#buoyancy-perturbation) about background buoyancy $N^2z$. The nonrotating inviscid [Boussinesq equations](../../../geophysical-fluid-dynamics.md#boussinesq-equations), with no buoyancy diffusion, are

$$
\frac{Du}{Dt}=-p_x,\qquad
\frac{Dw}{Dt}=-p_z+\sigma,\qquad
u_x+w_z=0,\qquad
\frac{D\sigma}{Dt}+N^2w=0,
\qquad \frac D{Dt}=\partial_t+u\partial_x+w\partial_z.
$$

Here the third equation is [mass conservation](../../../continuum-mechanics.md#mass-conservation) for [incompressible flow](../../../fluid-mechanics.md#incompressible-flow), and the last expresses [buoyancy](../../../fluid-mechanics.md#buoyancy) conservation following a parcel. Linearization about rest removes the products of disturbances. For a [plane internal gravity wave](../../../gravity-wave.md#plane-internal-gravity-wave) proportional to $e^{i(kx+mz-\omega t)}$, the resulting [Linearized Boussinesq equations](../../../geophysical-fluid-dynamics.md#linearized-boussinesq-equations) become

$$
-i\omega\widehat u=-ik\widehat p,\qquad
-i\omega\widehat w=-im\widehat p+\widehat\sigma,\qquad
k\widehat u+m\widehat w=0,\qquad
-i\omega\widehat\sigma+N^2\widehat w=0.
$$

With $K=(k^2+m^2)^{1/2}$ and $k\ne0$, the first and third equations give $\widehat p=-m\omega\widehat w/k^2$. Substitution in vertical momentum and buoyancy gives the [dispersion relation](../../../wave-equation.md#dispersion-relation)

$$
\boxed{\omega^2=\frac{N^2k^2}{k^2+m^2}.}
$$

Since the [velocity](../../../classical-mechanics.md#velocity) is the time [derivative](../../../calculus.md#derivative) of the [displacement field](../../../continuum-mechanics.md#displacement-field-mechanics), $\widehat{\boldsymbol u}=-i\omega\widehat{\boldsymbol\xi}$. Thus the complete [buoyancy polarization of a plane internal gravity wave](../../../gravity-wave.md#buoyancy-polarization-of-a-plane-internal-gravity-wave) is

$$
\boxed{
\widehat w=\frac{i\omega}{N^2}\widehat\sigma,\quad
\widehat u=-\frac{im\omega}{kN^2}\widehat\sigma,\quad
\widehat\zeta=-\frac{\widehat\sigma}{N^2},\quad
\widehat\xi=\frac{m\widehat\sigma}{kN^2},\quad
\widehat p=-\frac{im}{K^2}\widehat\sigma.}
$$

Both [velocity](../../../classical-mechanics.md#velocity) and [displacement](../../../classical-mechanics.md#displacement) are perpendicular to the [wavevector](../../../continuum-mechanics.md#wavevector); [pressure](../../../thermodynamics.md#pressure) and [velocity](../../../classical-mechanics.md#velocity) are in [quadrature](../../../physics.md#phase-quadrature) with [buoyancy](../../../fluid-mechanics.md#buoyancy) and [displacement](../../../classical-mechanics.md#displacement).

For upward/rightward [phase velocity](../../../wave-equation.md#phase-velocity), choose $k,m>0$ and $\omega=Nk/K$. Differentiating this [dispersion relation](../../../wave-equation.md#dispersion-relation) gives the [group velocity](../../../wave-equation.md#group-velocity), while the vector [phase velocity](../../../wave-equation.md#phase-velocity) points along the [wavevector](../../../continuum-mechanics.md#wavevector):

$$
\boxed{\mathbf c_g=\left(\frac{Nm^2}{K^3},-\frac{Nkm}{K^3}\right),\qquad
\mathbf c_p=\frac{Nk}{K^3}(k,m).}
$$

Their [dot product](../../../linear-algebra.md#dot-product) is zero and $\mathbf c_p+\mathbf c_g=(N/K,0)$. Draw $\mathbf c_g$ from the tip of $\mathbf c_p$: the [right-triangle geometry of internal-wave velocities](../../../gravity-wave.md#right-triangle-geometry-of-internal-wave-velocities) has horizontal hypotenuse $N/K$. This hypotenuse is distinct from the [horizontal phase velocity](../../../wave-equation.md#horizontal-phase-velocity) $\omega/k$.

At an instant with real [complex amplitude](../../../physics.md#complex-amplitude) $\widehat\sigma=A$, write $\phi=kx+mz-\omega t$. The spatial fields are

$$
\sigma=A\cos\phi,\quad
(\xi,\zeta)=\frac A{N^2}(m/k,-1)\cos\phi,\quad
(u,w)=\frac{\omega A}{N^2}(m/k,-1)\sin\phi,\quad
p=\frac{mA}{K^2}\sin\phi.
$$

The [constant-phase lines of an internal gravity wave](../../../gravity-wave.md#constant-phase-line-of-an-internal-gravity-wave) slope down to the right, with $dz/dx=-k/m$. [Buoyancy](../../../fluid-mechanics.md#buoyancy) maxima lie a quarter [wavelength](../../../wave-equation.md#wavelength) from [pressure](../../../thermodynamics.md#pressure) maxima; the oscillating [displacement](../../../classical-mechanics.md#displacement) and [velocity](../../../classical-mechanics.md#velocity) run along the phase lines. The [group velocity](../../../wave-equation.md#group-velocity) points down and right along them, despite upward/rightward motion of the [wave phase](../../../physics.md#phase-waves).

<a id="1/image-internal-wave-buoyancy-displacement-pressure-and-velocity-fields-with-downward-energy-propagation-and-the-phase-group-velocity-right-triangle"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-49-internal-wave.png)

**[Figure 1](#1/image-internal-wave-buoyancy-displacement-pressure-and-velocity-fields-with-downward-energy-propagation-and-the-phase-group-velocity-right-triangle). Internal-wave buoyancy, displacement, pressure and velocity fields, with downward energy propagation and the phase/group-velocity right triangle**.

Let $P=\overline{\xi_xu+\zeta_xw}$, using horizontal averaging over a [wavelength](../../../wave-equation.md#wavelength). This is the [displacement pseudomomentum of an internal gravity wave](../../../gravity-wave.md#displacement-pseudomomentum-of-an-internal-gravity-wave), whose sign convention is opposite to $k\overline E/\omega$. For complex coefficients, $\overline{ab}=\tfrac12\operatorname{Re}(\widehat a\widehat b^*)$. The above [wave polarization](../../../physics.md#polarization-waves) consequently gives

$$
P=-\frac{\omega K^2|\widehat\sigma|^2}{2kN^4},\qquad
\overline{\zeta_xp}=\frac{km|\widehat\sigma|^2}{2N^2K^2}.
$$

Since $c_{gz}=-\omega m/K^2$, these obey $\overline{\zeta_xp}=c_{gz}P$. With weak [kinematic viscosity](../../../fluid-mechanics.md#kinematic-viscosity), each leading monochromatic [velocity](../../../classical-mechanics.md#velocity) component satisfies $\nabla^2u=-K^2u$, $\nabla^2w=-K^2w$. The dissipative term is therefore $-\nu K^2P$, so the supplied averaged balance reduces to

$$
P_t+\partial_z(c_{gz}P)=-\nu K^2P.
$$

For constant $k,m,N$ and a steady wave envelope, $c_{gz}P_z=-\nu K^2P$. As $P$ is proportional to squared [wave amplitude](../../../physics.md#wave-amplitude), [viscous attenuation of an internal gravity wave](../../../gravity-wave.md#viscous-attenuation-of-an-internal-gravity-wave) gives

$$
\boxed{|\widehat\sigma(z)|=|\widehat\sigma(z_s)|
\exp\left[-\frac{\nu K^2(z-z_s)}{2c_{gz}}\right].}
$$

Here $c_{gz}<0$, so amplitude decreases below a source at $z_s$: **the source is above the receiving level**. The same conclusion follows directly because downward [group velocity](../../../wave-equation.md#group-velocity) carries [energy](../../../classical-mechanics.md#energy) from the source downward. Upward [phase velocity](../../../wave-equation.md#phase-velocity) does not locate the source.

For a slowly varying mean [shear flow](../../../fluid-mechanics.md#shear-flow) $U(z)$, the local [intrinsic frequency](../../../gravity-wave.md#intrinsic-frequency) is $\widehat\omega=\omega-kU(z)$. A local [WKB approximation](../../../analysis.md#wkb-approximation) uses $\widehat\omega^2=N^2k^2/(k^2+m(z)^2)$, with varying vertical [wavenumber](../../../wave-equation.md#wavenumber) and [group velocity](../../../wave-equation.md#group-velocity). The appropriate transported quantity is [wave action](../../../geophysical-fluid-dynamics.md#wave-action-fluid-dynamics), or horizontal [wave pseudomomentum](../../../geophysical-fluid-dynamics.md#wave-pseudomomentum) $kE/\widehat\omega$; its vertical flux has viscous loss, and the changing polarization factors must be retained. In particular, $P/|\widehat\sigma|^2$ is no longer constant.

Near a [critical level of an internal gravity wave](../../../gravity-wave.md#critical-level-of-an-internal-gravity-wave), $\widehat\omega\to0$, so $|m|\sim N|k|/|\widehat\omega|$ and $|c_{gz}|\sim\widehat\omega^2/(N|k|)$. The damping per vertical distance, of order $\nu K^2/|c_{gz}|$, grows rapidly. The waves are strongly attenuated over a narrow altitude range and transfer momentum to the mean flow there or before reaching the critical level. The inviscid [WKB approximation](../../../analysis.md#wkb-approximation) eventually fails; [viscosity](../../../fluid-mechanics.md#dynamic-viscosity) and possibly [internal-wave breaking](../../../gravity-wave.md#internal-wave-breaking) regulate the small scales.

## 2

↑ **Parent:** [Paper 49](paper-49.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Let $h$ be layer thickness and $g$ gravitational acceleration. The unforced [shallow water equations](../../../physics.md#shallow-water-equations) on the equatorial [beta plane](../../../geophysical-fluid-dynamics.md#beta-plane) are

$$
u_t+uu_x+vu_y-\beta yv=-gh_x,\qquad
v_t+uv_x+vv_y+\beta yu=-gh_y,\qquad
h_t+(hu)_x+(hv)_y=0.
$$

Linearize about $u=v=0$, $h=h_0$. Put $c_0=\sqrt{gh_0}$ and $L=\sqrt{c_0/\beta}$, and scale $(x,y)=L(X,Y)$, $t=(L/c_0)T$, $(u,v)=c_0(U,V)$ and $h=h_0(1+\eta)$. Dropping capitals, the [linearized shallow water equations](../../../physics.md#linearized-shallow-water-equations) become

$$
u_t-yv=-\eta_x,\qquad
v_t+yu=-\eta_y,\qquad
\eta_t+u_x+v_y=0.
$$

The choice $\beta L^2/c_0=1$ makes both the wave speed and the coefficient of the dimensionless [Coriolis parameter](../../../geophysical-fluid-dynamics.md#coriolis-parameter) equal to one.

Take [Fourier modes](../../../fourier-analysis.md#fourier-mode) $\{u(y),v(y),\eta(y)\}e^{i(kx-\omega t)}$ that decay as $y\to\pm\infty$. Their equations are

$$
\omega u-k\eta=iyv,\qquad
\omega\eta-ku=-iv',\qquad
-i\omega v+yu=-\eta'.
$$

For $v=0$ and nonzero $k$, the first two require $\omega^2=k^2$. The root $\omega=k$ gives $u=\eta$, and meridional balance becomes $u'=-yu$. Hence the [equatorial Kelvin wave](../../../geophysical-fluid-dynamics.md#equatorial-kelvin-wave) is

$$
\boxed{\omega=k,\qquad v=0,\qquad u=\eta=C e^{-y^2/2}.}
$$

It travels eastward at speed $c_0$ in dimensional units. The other sign gives $\eta=-u$ and $u'=yu$, so $u\propto e^{y^2/2}$ is not trapped.

For $v\ne0$, $\omega\ne0$ and $\omega^2\ne k^2$, inversion of the first two equations gives the [equatorial wave velocity polarization](../../../geophysical-fluid-dynamics.md#equatorial-wave-velocity-polarization)

$$
u=\frac{i(\omega yv-kv')}{\omega^2-k^2},\qquad
\eta=\frac{i(kyv-\omega v')}{\omega^2-k^2}.
$$

Substitute in the remaining momentum equation. Multiplication by $(\omega^2-k^2)/i$ leaves

$$
-\omega(\omega^2-k^2)v+\omega y^2v+kv-\omega v''=0,
$$

so

$$
v''+(\lambda-y^2)v=0,\qquad
\lambda=\omega^2-k^2-\frac k\omega.
$$

Writing $v=e^{-y^2/2}H(y)$ yields $H''-2yH'+(\lambda-1)H=0$, the [Hermite differential equation](../../../analysis.md#hermite-differential-equation). The trapped solutions have the [Hermite oscillator quantization](../../../analysis.md#hermite-oscillator-quantization) $\lambda=2n+1$ and $H=H_n$.

For completeness, quantization follows without assuming that every acceptable solution is a [polynomial](../../../polynomial.md). On decaying smooth functions, define $a=d/dy+y$, $a^\dagger=-d/dy+y$ and $\mathcal H=-d^2/dy^2+y^2=a^\dagger a+1$. [Integration by parts](../../../calculus.md#integration-by-parts) gives $\lambda\ge1$ and $\|av\|^2=(\lambda-1)\|v\|^2$. If $av\ne0$, it is an [eigenfunction](../../../linear-operator-theory.md#eigenfunction) of $\mathcal H$ with [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\lambda-2$. Repeated lowering must terminate: otherwise it eventually produces an [eigenvalue](../../../linear-operator-theory.md#eigenvalue) below one. At termination $av=0$, so the terminal [eigenfunction](../../../linear-operator-theory.md#eigenfunction) is $e^{-y^2/2}$ and has [eigenvalue](../../../linear-operator-theory.md#eigenvalue) one. Repeated raising gives $H_n(y)e^{-y^2/2}$ and $\lambda=2n+1$; uniqueness of a decaying solution at one end of this second-order equation fixes each mode up to scale.

Thus, away from the exceptional quotients, all fields are determined by

$$
\boxed{
v=C H_n(y)e^{-y^2/2},\qquad
\omega^2-k^2-\frac k\omega=2n+1,\qquad n=0,1,2,\ldots.}
$$

Insert this $v$ and its [derivative](../../../calculus.md#derivative) in the polarization formulae to obtain $u$ and $\eta$. For $n\ge1$, the cubic $\omega^3-(k^2+2n+1)\omega-k=0$ supplies the low-frequency [equatorial Rossby wave](../../../geophysical-fluid-dynamics.md#equatorial-rossby-wave) and two [equatorial inertia--gravity wave](../../../geophysical-fluid-dynamics.md#equatorial-inertia-gravity-wave) branches. Their meridional structures are Gaussian-weighted [Hermite polynomials](../../../numerical-analysis.md#hermite-polynomial).

For $n=0$, multiplication by $\omega$ factorizes the [equatorial shallow-water dispersion relation](../../../geophysical-fluid-dynamics.md#equatorial-shallow-water-dispersion-relation) as

$$
(\omega+k)(\omega^2-k\omega-1)=0.
$$

The physically admissible quadratic gives the [mixed Rossby-gravity wave](../../../geophysical-fluid-dynamics.md#rossby-gravity-waves), equivalently the [Yanai wave](../../../geophysical-fluid-dynamics.md#rossby-gravity-waves):

$$
\boxed{\omega-k-\frac1\omega=0,\qquad
v=C e^{-y^2/2},\qquad u=\eta=i\omega yv.}
$$

These fields satisfy all three original equations directly and decay at both infinities, including where the quotient formulae are singular.

To test the other factor, set $\omega=-k\ne0$. The original equations give $u+\eta=-iyv/k$ and $v'=-yv$. Put $\delta=u-\eta$; meridional momentum then gives

$$
\delta'-y\delta=i(2k-k^{-1})v,\qquad
(e^{-y^2/2}\delta)'=i(2k-k^{-1})C e^{-y^2}.
$$

Decay of $u,\eta$ at both infinities requires the integral of the right side to vanish. Hence $C=0$ unless $k^2=1/2$. Ordinarily the extra factor supplies no trapped mode. At the [exceptional root of the mixed Rossby-gravity mode](../../../geophysical-fluid-dynamics.md#exceptional-root-of-the-mixed-rossby-gravity-mode), $k^2=1/2$, it coincides with the quadratic root and gives the same physical fields, not an additional branch. This distinction avoids discarding a regular physical mode at the crossing.

These arguments concern nonzero wave [angular frequency](../../../classical-mechanics.md#angular-frequency). At $k=0$, the oscillatory nonzero-$v$ modes have $\omega=\pm\sqrt{2n+1}$, while zero-frequency $v=0$ geostrophic states must be considered in the original equations rather than in expressions divided by $\omega$.

## 3

↑ **Parent:** [Paper 49](paper-49.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The basic [quasi-geostrophic streamfunction](../../../geophysical-fluid-dynamics.md#quasi-geostrophic-streamfunction) $\bar\psi=-\Lambda yz$ gives $\bar u=\Lambda z$, $\bar v=0$ and constant [quasi-geostrophic potential vorticity](../../../geophysical-fluid-dynamics.md#three-dimensional-quasi-geostrophic-potential-vorticity) $\bar Q=f$. Define

$$
q'=\nabla_h^2\psi'+\frac{f^2}{N^2}\psi'_{zz}.
$$

Because the background has no [potential-vorticity gradient](../../../geophysical-fluid-dynamics.md#potential-vorticity-gradient), the linear [potential-vorticity equation](../../../geophysical-fluid-dynamics.md#potential-vorticity-evolution-equation) is simply

$$
(\partial_t+\Lambda z\partial_x)q'=0.
$$

Its [characteristics](../../../algebra.md#characteristic-of-a-field) have constant $y,z,x-\Lambda zt$, so the general solution is $q'=\mathcal F(y,z,x-\Lambda zt)$. In particular, $q'=F(y,z)G(x-\Lambda zt)$ is the requested arbitrary separated family; one product is not the most general initial field.

Linearizing the vertical [velocity](../../../classical-mechanics.md#velocity) requires retaining advection of $\bar\psi_z=-\Lambda y$ by $v'=\psi'_x$. Therefore

$$
w'=-\frac f{N^2}\left[(\partial_t+\Lambda z\partial_x)\psi'_z-\Lambda\psi'_x\right].
$$

The impermeable boundary at $z=0$ imposes

$$
\boxed{\partial_t\psi'_z-\Lambda\psi'_x=0\quad(z=0).}
$$

This is conservation of boundary [buoyancy](../../../fluid-mechanics.md#buoyancy), not merely a condition that $\psi'_z$ vanish.

For zero interior [potential vorticity](../../../geophysical-fluid-dynamics.md#potential-vorticity), write $\psi'=\operatorname{Re}\{\phi(z,t)e^{i(kx+ly)}\}$. With $K_h=\sqrt{k^2+l^2}>0$, [stratified quasi-geostrophic inversion](../../../geophysical-fluid-dynamics.md#stratified-quasi-geostrophic-inversion) gives

$$
\phi_{zz}-\frac{N^2K_h^2}{f^2}\phi=0.
$$

The decaying solution is

$$
\boxed{\phi=A(t)e^{-\mu z},\qquad\mu=\frac{N K_h}{f}.}
$$

No time dependence has been assumed to obtain this vertical structure. Applying the boundary condition gives $-\mu\dot A-i\Lambda kA=0$, hence

$$
\boxed{A=A_0e^{-i\omega t},\qquad
\omega=\frac{\Lambda k}{\mu}=\frac{f\Lambda k}{N\sqrt{k^2+l^2}}.}
$$

Thus the [Eady edge wave](../../../hydrodynamic-stability.md#eady-edge-wave) travels eastward with [horizontal phase velocity](../../../wave-equation.md#horizontal-phase-velocity) $\omega/k=\Lambda/\mu$ for $k\ne0$.

The propagation mechanism can be made explicit using boundary parcels. [Thermal wind](../../../geophysical-fluid-dynamics.md#thermal-wind) gives the background [buoyancy gradient](../../../fluid-mechanics.md#buoyancy-gradient) $\bar b_y=f\bar\psi_{zy}=-f\Lambda$. A small meridional parcel [displacement](../../../classical-mechanics.md#displacement) $d$ produces boundary [buoyancy perturbation](../../../fluid-mechanics.md#buoyancy-perturbation) $b'=-d\bar b_y=f\Lambda d$. Meanwhile the decaying [potential-vorticity inversion](../../../geophysical-fluid-dynamics.md#potential-vorticity-inversion) gives $b'=f\psi'_z=-f\mu\psi'$ at the boundary. Consequently $\psi'=-\Lambda d/\mu$ there, and the parcel equation $d_t=v'=\psi'_x$ becomes

$$
d_t+\frac\Lambda\mu d_x=0.
$$

A displaced buoyancy contour therefore induces a [velocity field](../../../fluid-mechanics.md#velocity-field) that advances that displacement eastward. No interior [potential-vorticity gradient](../../../geophysical-fluid-dynamics.md#potential-vorticity-gradient) is needed because the boundary buoyancy supplies the invertibility data.

[Vortex stretching](../../../physics.md#vortex-stretching) is what sets the induced flow's vertical reach. In the interior, the zero-[potential vorticity](../../../geophysical-fluid-dynamics.md#potential-vorticity) condition requires

$$
\underbrace{\nabla_h^2\psi'}_{\text{relative vorticity}}=-K_h^2\psi',\qquad
\underbrace{\frac{f^2}{N^2}\psi'_{zz}}_{\text{stretching}}=+K_h^2\psi'.
$$

Boundary [isopycnal displacement](../../../geophysical-fluid-dynamics.md#isopycnal-displacement) decreases with height as $e^{-\mu z}$, so fluid columns are stretched or compressed over depth $\mu^{-1}=f/(NK_h)$. Conservation of [potential vorticity](../../../geophysical-fluid-dynamics.md#potential-vorticity) makes this stretching balance the [relative vorticity](../../../fluid-mechanics.md#relative-vorticity). The resulting inversion factor $b'=-f\mu\psi'$ gives the propagation speed: stronger [density stratification](../../../gravity-wave.md#density-stratification) reduces penetration and speed, while larger $f$ increases them. Zero interior [potential vorticity](../../../geophysical-fluid-dynamics.md#potential-vorticity) therefore does not imply zero interior flow.

For imposed boundary vertical [velocity](../../../classical-mechanics.md#velocity), retain the same decaying structure and write

$$
w'(0)=\operatorname{Re}\{\epsilon e^{i(kx+ly-\omega_0t)}\}.
$$

The boundary relation becomes the [forced Eady edge wave](../../../hydrodynamic-stability.md#forced-eady-edge-wave) equation

$$
\dot A+i\omega A=C e^{-i\omega_0t},\qquad C=\frac{N^2\epsilon}{f\mu}.
$$

The [integrating factor](../../../differential-equation.md#integrating-factor) $e^{i\omega t}$ gives, for $\omega_0\ne\omega$,

$$
\boxed{A(t)=B e^{-i\omega t}+\frac{C}{i(\omega-\omega_0)}e^{-i\omega_0t},\qquad
\psi'=\operatorname{Re}\{A(t)e^{-\mu z+i(kx+ly)}\}.}
$$

The arbitrary homogeneous coefficient $B$ sets the initial disturbance. With $A(0)=0$, this is $A=C(e^{-i\omega_0t}-e^{-i\omega t})/[i(\omega-\omega_0)]$.

At [resonance](../../../dynamical-systems.md#resonance), $\omega_0=\omega$, integration instead yields

$$
\boxed{A(t)=(B+Ct)e^{-i\omega t}.}
$$

An initially undisturbed fluid has $\psi'=Ct e^{-\mu z}\cos(kx+ly-\omega t)$. The imposed pumping reinforces the same boundary [normal mode](../../../wave-equation.md#normal-mode) every cycle, with no dissipative loss, so the linear amplitude grows secularly. The divergence describes [resonance](../../../dynamical-systems.md#resonance) of the undamped linear model; sufficiently large [wave amplitude](../../../physics.md#wave-amplitude) invalidates the assumed small-disturbance approximation.

## 4

↑ **Parent:** [Paper 49](paper-49.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

[Potential-vorticity inversion](../../../geophysical-fluid-dynamics.md#potential-vorticity-inversion) is the diagnostic recovery of the flow from its advected vortical scalar, using the balance relation and specified [boundary conditions](../../../differential-equation.md#boundary-condition). Its usefulness is a separation of tasks: transport the scalar by the current [velocity](../../../classical-mechanics.md#velocity), invert to find the new [velocity](../../../classical-mechanics.md#velocity), and repeat. The inverse is spatially nonlocal even though the transport law is local. The four models differ chiefly in the operator being inverted and the information needed at boundaries.

In [two-dimensional vortex dynamics](../../../fluid-mechanics.md#two-dimensional-vortex-dynamics), planar [incompressibility](../../../fluid-mechanics.md#incompressible-flow) permits $\boldsymbol u=(-\psi_y,\psi_x)$, and vertical [vorticity](../../../fluid-mechanics.md#vorticity) is $\zeta=\nabla^2\psi$. The [curl](../../../calculus.md#curl) of inviscid momentum gives

$$
\zeta_t+J(\psi,\zeta)=0,\qquad
J(\psi,\zeta)=\psi_x\zeta_y-\psi_y\zeta_x.
$$

There is no [vortex stretching](../../../physics.md#vortex-stretching) in strictly planar motion, so [vorticity](../../../fluid-mechanics.md#vorticity) is materially conserved. The [two-dimensional potential-vorticity inversion](../../../geophysical-fluid-dynamics.md#two-dimensional-potential-vorticity-inversion) is the [Poisson equation](../../../partial-differential-equation.md#poisson-equation) $\nabla^2\psi=\zeta$. On the plane, with suitable integrability and far-field behavior, its [Green's function](../../../analysis.md#green-s-function) is $(2\pi)^{-1}\log|\boldsymbol x-\boldsymbol x'|$, giving

$$
\psi(\boldsymbol x)=\frac1{2\pi}\int\zeta(\boldsymbol x')\log|\boldsymbol x-\boldsymbol x'|\,d^2x'+\psi_h(\boldsymbol x).
$$

Differentiation gives the [planar Biot-Savart kernel](../../../fluid-mechanics.md#planar-vorticity-velocity-kernel). Here $\psi_h$ is a [harmonic function](../../../partial-differential-equation.md#harmonic-function) fixed by boundary, circulation and far-field data. A rigid impermeable wall is a streamline, so $\psi$ is constant on it; constants or circulations around distinct holes require specification. The [vorticity](../../../fluid-mechanics.md#vorticity) alone cannot distinguish two flows differing by a permitted harmonic contribution, such as a uniform current on an unbounded plane. A constant added to $\psi$ has no physical effect.

In [nonrotating layerwise-two-dimensional vortex dynamics](../../../fluid-mechanics.md#nonrotating-layerwise-two-dimensional-vortex-dynamics), strong stable [density stratification](../../../gravity-wave.md#density-stratification) constrains motion to almost horizontal layers. In the ideal independent-layer limit, vertical [velocity](../../../classical-mechanics.md#velocity) vanishes at leading order, $(u,v)=(-\psi_y,\psi_x)$ and

$$
\zeta_t+J(\psi,\zeta)=0,\qquad\nabla_h^2\psi=\zeta
$$

hold separately at each fixed $z$. Height is a parameter: the horizontal inverse [Laplacian](../../../calculus.md#laplacian) contains no vertical [derivative](../../../calculus.md#derivative). With background buoyancy $N^2z$, the leading [Ertel potential vorticity](../../../geophysical-fluid-dynamics.md#ertel-potential-vorticity) is $Q=\boldsymbol\omega\cdot\nabla b\simeq N^2\zeta$, so the materially advected normalized scalar is $Q/N^2\simeq\zeta$. The same horizontal [Poisson equation](../../../partial-differential-equation.md#poisson-equation) is inverted layer by layer, using each layer's boundary data. This is an asymptotic constrained model, not arbitrary three-dimensional Euler motion with vertical [velocity](../../../classical-mechanics.md#velocity) set to zero: its validity requires small [Froude number](../../../reduced-gravity.md#froude-number) and controlled vertical scales. At finite [buoyancy frequency](../../../gravity-wave.md#buoyancy-frequency), the weak vertical motion and tilted [isopycnals](../../../fluid-mechanics.md#isopycnal) restore coupling. The inversion may be independent by layer while the reconstructed fields vary with height. The horizontal [Euler equations for an inviscid fluid](../../../fluid-mechanics.md#euler-equations-for-an-inviscid-fluid) determine the [pressure gradient](../../../fluid-mechanics.md#pressure-gradient), while [hydrostatic balance](../../../fluid-mechanics.md#hydrostatic-balance) relates its vertical [derivative](../../../calculus.md#derivative) to [buoyancy](../../../fluid-mechanics.md#buoyancy).

In [shallow-water quasi-geostrophic inversion](../../../geophysical-fluid-dynamics.md#shallow-water-quasi-geostrophic-inversion), begin with the exact [shallow-water potential vorticity](../../../geophysical-fluid-dynamics.md#shallow-water-potential-vorticity) $(f+\zeta)/h$. Linearizing its anomaly about depth $H$ gives, after multiplying by $H$, $\zeta-f_0\eta/H$. For small [Rossby number](../../../geophysical-fluid-dynamics.md#rossby-number), [geostrophic balance](../../../physics.md#geostrophic-balance) gives $\psi=g\eta/f_0$, while $\zeta=\nabla_h^2\psi$. Keeping the [beta plane](../../../geophysical-fluid-dynamics.md#beta-plane) background gradient gives

$$
q=\nabla_h^2\psi-\frac{\psi}{L_D^2}+\beta y,\qquad
L_D=\frac{\sqrt{gH}}{|f_0|},\qquad
q_t+J(\psi,q)=0.
$$

Thus $q-\beta y$ is inverted with the [modified Helmholtz equation](../../../partial-differential-equation.md#modified-helmholtz-equation) $(\nabla_h^2-L_D^{-2})\psi=q-\beta y$, under the specified boundary and far-field conditions. The [velocity](../../../classical-mechanics.md#velocity) follows from $\psi$ and surface elevation from $\eta=f_0\psi/g$. A horizontal [Fourier mode](../../../fourier-analysis.md#fourier-mode) of the anomaly satisfies

$$
\widehat\psi=-\frac{\widehat{q-\beta y}}{|\boldsymbol k_h|^2+L_D^{-2}}.
$$

The [Rossby deformation radius](../../../physics.md#rossby-deformation-radius) therefore limits the reach of the balanced response. Layer stretching, represented by $-\psi/L_D^2$, is absent from ordinary planar [vorticity](../../../fluid-mechanics.md#vorticity) inversion. Unlike the pure [Poisson equation](../../../partial-differential-equation.md#poisson-equation), the finite-deformation operator also responds to the constant part of $\psi$, which specifies mean elevation rather than an arbitrary streamfunction offset. Specified bottom topography adds a known source to $q$; it is subtracted along with the background before inversion.

In [stratified quasi-geostrophic inversion](../../../geophysical-fluid-dynamics.md#stratified-quasi-geostrophic-inversion), continuously varying vertical displacement replaces the shallow layer's single stretching term. For positive $N^2(z)$ and constant nonzero $f_0$, the [three-dimensional quasi-geostrophic potential vorticity](../../../geophysical-fluid-dynamics.md#three-dimensional-quasi-geostrophic-potential-vorticity) is

$$
q=\nabla_h^2\psi+\partial_z\left(\frac{f_0^2}{N^2}\psi_z\right)+\beta y,
\qquad q_t+J(\psi,q)=0.
$$

[Geostrophic balance](../../../physics.md#geostrophic-balance) and [hydrostatic balance](../../../fluid-mechanics.md#hydrostatic-balance) give [velocity](../../../classical-mechanics.md#velocity) $(-\psi_y,\psi_x)$ and [buoyancy perturbation](../../../fluid-mechanics.md#buoyancy-perturbation) $b=f_0\psi_z$. Invert the anisotropic [elliptic boundary value problem](../../../elliptic-boundary-value-problem.md) using interior $q$, prescribed top and bottom [buoyancy](../../../fluid-mechanics.md#buoyancy) as [Neumann boundary conditions](../../../differential-equation.md#neumann-boundary-condition), and the lateral, far-field and global-flow data. Boundary [buoyancy](../../../fluid-mechanics.md#buoyancy) evolves by its own material conservation when the boundary is impermeable. It cannot be discarded: the [Eady edge wave](../../../hydrodynamic-stability.md#eady-edge-wave) in the preceding solution has zero interior [potential vorticity](../../../geophysical-fluid-dynamics.md#potential-vorticity) anomaly but nonzero boundary buoyancy and a nonzero induced flow.

For constant $N,f_0$, the [stretched coordinates for quasi-geostrophic inversion](../../../geophysical-fluid-dynamics.md#stretched-coordinates-for-quasi-geostrophic-inversion) $Z=Nz/|f_0|$ turn the inversion operator into the three-dimensional [Laplacian](../../../calculus.md#laplacian). Its infinite-space [Green's function](../../../analysis.md#green-s-function) is $-1/(4\pi|\boldsymbol X-\boldsymbol X'|)$ in $(x,y,Z)$ coordinates. Hence a horizontal disturbance of scale $L$ communicates vertically over scale $|f_0|L/N$, explicitly coupling layers. In a bounded domain with homogeneous difference data, multiplying the difference of two inversions by its [streamfunction](../../../fluid-mechanics.md#stream-function) and applying [integration by parts](../../../calculus.md#integration-by-parts) gives

$$
\int\left(|\nabla_h\delta\psi|^2+\frac{f_0^2}{N^2}|\delta\psi_z|^2\right)dV=0.
$$

This proves uniqueness up to a constant when the relevant boundary terms vanish; a mean or pressure reference fixes the remaining constant. Compatible boundary fluxes are needed for a purely [Neumann boundary-value problem](../../../differential-equation.md#neumann-boundary-value-problem).

Across all four models, inversion provides the induced flow, while scalar transport supplies time evolution. The independent horizontal inverse in the first two models becomes a finite-deformation inverse in shallow water and a vertically coupled elliptic inverse in continuous stratification. The principle applies within the stated balance or constrained model. In the unrestricted [Boussinesq equations](../../../geophysical-fluid-dynamics.md#boussinesq-equations) or [shallow water equations](../../../physics.md#shallow-water-equations), [gravity waves](../../../gravity-wave.md) and divergent motion can share the same [potential vorticity](../../../geophysical-fluid-dynamics.md#potential-vorticity), so the vortical scalar alone does not reconstruct every possible flow.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
