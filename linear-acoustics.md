# Linear acoustics

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_acoustics)

Linear acoustics describes small pressure, density, and velocity perturbations about a uniform quiescent compressible fluid.

**Table of contents**

- [Stationary vorticity mode in linear acoustics](#stationary-vorticity-mode-in-linear-acoustics)
- [Rayleigh integral for baffled acoustic radiation](#rayleigh-integral-for-baffled-acoustic-radiation)
- [Acoustic far field](#acoustic-far-field)
  - [Acoustic directivity](#acoustic-directivity)
- [Moving-surface retarded Jacobian](#moving-surface-retarded-jacobian)
- [Stratified acoustic pressure equation](#stratified-acoustic-pressure-equation)
- [Acoustic density perturbation](#acoustic-density-perturbation)
- [Acoustic compact-source approximation](#acoustic-compact-source-approximation)
- [Acoustic multipole source](#acoustic-multipole-source)
  - [Acoustic quadrupole](#acoustic-quadrupole)
    - [Compact rotating two-blade loading source](#compact-rotating-two-blade-loading-source)
    - [Compact acoustic quadrupole Mach-number scaling](#compact-acoustic-quadrupole-mach-number-scaling)
      - [Two-dimensional compact quadrupole scaling](#two-dimensional-compact-quadrupole-scaling)
  - [Acoustic dipole](#acoustic-dipole)
    - [Acoustic dipole Mach-number scaling](#acoustic-dipole-mach-number-scaling)
  - [Acoustic monopole](#acoustic-monopole)
    - [Rotating acoustic point source](#rotating-acoustic-point-source)
- [Lighthill acoustic analogy](#lighthill-acoustic-analogy)
  - [Mass-injection term in the acoustic analogy](#mass-injection-term-in-the-acoustic-analogy)
  - [Far-field acoustic force and stress moments](#far-field-acoustic-force-and-stress-moments)
  - [Distributional acoustic analogy across a moving interface](#distributional-acoustic-analogy-across-a-moving-interface)
    - [Ffowcs Williams-Hawkings equation](#ffowcs-williams-hawkings-equation)
      - [Fixed-body retarded acoustic loading formula](#fixed-body-retarded-acoustic-loading-formula)
      - [Acoustic loading noise](#acoustic-loading-noise)
        - [Small-body loading-noise threshold](#small-body-loading-noise-threshold)
      - [Acoustic thickness noise](#acoustic-thickness-noise)
        - [Compact radiation moments of a pulsating spherical bubble](#compact-radiation-moments-of-a-pulsating-spherical-bubble)
        - [Translating-sphere acoustic thickness dipole](#translating-sphere-acoustic-thickness-dipole)
  - [Lighthill stress tensor](#lighthill-stress-tensor)
    - [Surface sources of a discontinuous Lighthill stress tensor](#surface-sources-of-a-discontinuous-lighthill-stress-tensor)
- [Linear homentropic acoustic equations](#linear-homentropic-acoustic-equations)
  - [Acoustic pressure wave equation](#acoustic-pressure-wave-equation)
    - [Outgoing acoustic square-root branch](#outgoing-acoustic-square-root-branch)
- [Homentropic pressure perturbation](#homentropic-pressure-perturbation)
- [Acoustic velocity potential](#acoustic-velocity-potential)
  - [Outgoing acoustic field of a pulsating sphere](#outgoing-acoustic-field-of-a-pulsating-sphere)
    - [Mean acoustic power of a pulsating sphere](#mean-acoustic-power-of-a-pulsating-sphere)
    - [Surface acoustic energy-to-flux ratio of a pulsating sphere](#surface-acoustic-energy-to-flux-ratio-of-a-pulsating-sphere)
  - [Pressure-forced standing acoustic wave in a spherical annulus](#pressure-forced-standing-acoustic-wave-in-a-spherical-annulus)
    - [Radial acoustic resonance in a spherical annulus](#radial-acoustic-resonance-in-a-spherical-annulus)
  - [Spherically symmetric vibration of a gas-filled elastic shell](#spherically-symmetric-vibration-of-a-gas-filled-elastic-shell)
- [Acoustic energy conservation](#acoustic-energy-conservation)
  - [Near-field energy imbalance in a spherical acoustic wave](#near-field-energy-imbalance-in-a-spherical-acoustic-wave)
  - [Acoustic energy density](#acoustic-energy-density)
- [Evanescent acoustic surface wave](#evanescent-acoustic-surface-wave)
  - [Acoustic wave on a tensioned massive membrane](#acoustic-wave-on-a-tensioned-massive-membrane)
    - [Elastic-sheet tension](#elastic-sheet-tension)
    - [Point-force radiation from a fluid-loaded sheet](#point-force-radiation-from-a-fluid-loaded-sheet)
      - [One-sided fluid-loaded membrane radiation](#one-sided-fluid-loaded-membrane-radiation)
    - [Tensioned-sheet acoustic impedance](#tensioned-sheet-acoustic-impedance)
      - [Reflection pole of a fluid-loaded membrane](#reflection-pole-of-a-fluid-loaded-membrane)
    - [Fluid-loaded membrane edge scattering](#fluid-loaded-membrane-edge-scattering)
      - [Plane-wave forcing of a pinned elastic half-sheet](#plane-wave-forcing-of-a-pinned-elastic-half-sheet)
      - [Incoming-pole cancellation at a pinned membrane edge](#incoming-pole-cancellation-at-a-pinned-membrane-edge)
  - [Spring-supported acoustic membrane wave](#spring-supported-acoustic-membrane-wave)
    - [Acoustic membrane dispersion asymptotics](#acoustic-membrane-dispersion-asymptotics)
  - [Added mass of an evanescent fluid layer](#added-mass-of-an-evanescent-fluid-layer)
- [Time average of harmonic power](#time-average-of-harmonic-power)
  - [Reactive acoustic energy flux](#reactive-acoustic-energy-flux)

## Stationary vorticity mode in linear acoustics

↑ **Parent:** [Linear acoustics](linear-acoustics.md)

Linearizing inviscid barotropic flow about uniform rest gives $\partial_t(\nabla\times u)=0$, not automatically $\nabla\times u=0$. Irrotational [linear acoustics](linear-acoustics.md) therefore requires zero initial [vorticity](fluid-mechanics.md#vorticity) or restriction to the longitudinal acoustic mode. A time-independent divergence-free field, with zero pressure and density perturbations, is a nonacoustic solution of the linearized equations.

## Rayleigh integral for baffled acoustic radiation

↑ **Parent:** [Linear acoustics](linear-acoustics.md)

An aperture in a rigid plane with prescribed harmonic normal displacement $f(x')e^{i\omega t}$ radiates into a half-space. Superposing [acoustic monopoles](#acoustic-monopole), each doubled by its same-sign rigid-wall image, gives the stated integral, where $R$ is the distance from aperture element to observer. In the [acoustic far field](#acoustic-far-field), expanding $R$ to first order across the aperture identifies the angular radiation amplitude with the aperture's [Fourier transform](analysis.md#fourier-transform).

## Acoustic far field

↑ **Parent:** [Linear acoustics](linear-acoustics.md)

The acoustic far field is the radiation region where the observer is many reduced wavelengths from the source and far compared with its geometric extent. Three-dimensional outgoing [acoustic density perturbations](#acoustic-density-perturbation) spread as $R^{-1}$; two-dimensional harmonic fields spread as $R^{-1/2}$. The condition is independent of the [acoustic compact-source approximation](#acoustic-compact-source-approximation) $k_0\ell\ll1$. Differentiating a retarded phase produces the radiating part of a [Green function](analysis.md#green-s-function) integral; derivatives of the spreading factor produce near-field terms.

### Acoustic directivity

↑ **Parent:** [Acoustic far field](#acoustic-far-field)

Acoustic directivity describes the angular dependence of radiation in the [acoustic far field](#acoustic-far-field). For a time-harmonic source in $d$ spatial dimensions, separating the geometric spreading and oscillatory phase leaves a complex amplitude pattern $\mathcal D$. The angular intensity pattern is proportional to $|\mathcal D|^2$. Directivity can be normalized by a reference direction or total radiated power; a stated convention is needed when comparing absolute directivity factors.

## Moving-surface retarded Jacobian

↑ **Parent:** [Linear acoustics](linear-acoustics.md)

For a source surface parameterized by $y(p,q,\tau)$, the [retarded time](electromagnetism.md#retarded-time) equation is $t=\tau+|x-y(p,q,\tau)|/c_0$. Integrating a [Dirac delta distribution](distribution-theory.md#dirac-delta-function) enforcing that equation produces the reciprocal [derivative](calculus.md#derivative) $|1-M_r|^{-1}$ at each simple root. For subsonic motion there is a unique retarded root. Multiple roots require summation; a zero [derivative](calculus.md#derivative) is outside the simple-root rule. This factor is the moving-source counterpart of a delta change-of-variable Jacobian.

## Stratified acoustic pressure equation

↑ **Parent:** [Linear acoustics](linear-acoustics.md)

For adiabatic perturbations of a static perfect gas, pressure obeys

$$
c_0^{-2}p'_{tt}-a^{-1}\nabla\cdot(a\nabla p')=0,\qquad a=p_0^{1/\gamma}/\rho_0.
$$

The stationary balance is $\nabla(p_0+\chi)=0$. Density and entropy need not be spatially uniform. Expanding the divergence exposes the gradient terms that distinguish this equation from the homogeneous [acoustic pressure wave equation](#acoustic-pressure-wave-equation). Its divergence form yields [weighted acoustic Green-function reciprocity](physics.md#weighted-acoustic-green-function-reciprocity).

## Acoustic density perturbation

↑ **Parent:** [Linear acoustics](linear-acoustics.md)

An acoustic density perturbation is the deviation of fluid [mass density](fluid-mechanics.md#density) from its quiescent reference value. In a homogeneous isentropic linear acoustic field, its corresponding [pressure](thermodynamics.md#pressure) perturbation is $p'=c_0^2\rho'$. Nonlinear and entropy-dependent departures from this relation enter the [Lighthill stress tensor](#lighthill-stress-tensor).

## Acoustic compact-source approximation

↑ **Parent:** [Linear acoustics](linear-acoustics.md)

An acoustic source is compact when its size is much smaller than the acoustic wavelength. The propagation delay across the source can then be neglected in leading source integrals. This condition is distinct from the radiation-region requirement $k_0r\gg1$.

## Acoustic multipole source

↑ **Parent:** [Linear acoustics](linear-acoustics.md)

Acoustic sources may be organized by the number of spatial derivatives in their effective [wave equation](wave-equation.md) forcing. A direct scalar source is an [acoustic monopole](#acoustic-monopole), a divergence of a force density an [acoustic dipole](#acoustic-dipole), and a double divergence of a stress tensor an [acoustic quadrupole](#acoustic-quadrupole).

### Acoustic quadrupole

↑ **Parent:** [Acoustic multipole source](#acoustic-multipole-source)

An acoustic quadrupole has forcing $\partial_i\partial_jT_{ij}$. The [acoustic compact-source approximation](#acoustic-compact-source-approximation) reduces its leading far-field density to $n_in_j\ddot S_{ij}/(4\pi c_0^4r)$ in three dimensions, with $S_{ij}=\int T_{ij}d^3y$ evaluated at retarded time.

#### Compact rotating two-blade loading source

↑ **Parent:** [Acoustic quadrupole](#acoustic-quadrupole)

Two diametrically opposite rotating blades with equal tangential loads have zero total rotating [force](classical-mechanics.md#force). Their leading compact [acoustic dipoles](#acoustic-dipole) cancel, but their retarded positions and [moving-surface retarded Jacobians](#moving-surface-retarded-jacobian) leave an [acoustic quadrupole](#acoustic-quadrupole). For line load $2Fr/a^2$ and angular speed $\Omega$, the first radiating density is $2F\Omega^2a\sin^2\theta\sin(2\Omega\tau_0)/(3\pi c_0^4R)$. The twofold geometry gives frequency $2\Omega$, while projection into the rotor plane gives the amplitude directivity $\sin^2\theta$.

#### Compact acoustic quadrupole Mach-number scaling

↑ **Parent:** [Acoustic quadrupole](#acoustic-quadrupole)

For a low-[Mach number](compressible-flow.md#mach-number) source with stress $O(\rho_0U^2)$ and advective time $\ell/U$, the three-dimensional compact [acoustic quadrupole](#acoustic-quadrupole) has density amplitude $O(\rho_0M^4\ell/r)$, where $M=U/c_0$. The power depends on these source-time and stress hypotheses, not only on the quadrupole label.

##### Two-dimensional compact quadrupole scaling

↑ **Parent:** [Compact acoustic quadrupole Mach-number scaling](#compact-acoustic-quadrupole-mach-number-scaling)

In two dimensions, the outgoing harmonic [Helmholtz equation](partial-differential-equation.md#helmholtz-equation) kernel has magnitude proportional to $(k_0r)^{-1/2}$. Combining this spreading with the compact [acoustic quadrupole](#acoustic-quadrupole) source and $k_0\ell=O(M)$ changes the density-amplitude [Mach number](compressible-flow.md#mach-number) power to $7/2$ when geometric range is separated.

### Acoustic dipole

↑ **Parent:** [Acoustic multipole source](#acoustic-multipole-source)

An acoustic dipole represents an applied force density. A surface force defect contributes $-\partial_i(L_i\delta_s)$ to the density [wave equation](wave-equation.md).

#### Acoustic dipole Mach-number scaling

↑ **Parent:** [Acoustic dipole](#acoustic-dipole)

For a small body of size $l$ in flow of speed $u$, force of order $\rho_0u^2l^2$ varying on time $l/u$ produces an [acoustic dipole](#acoustic-dipole) density amplitude of the displayed order, where $M=u/c_0$ is the [Mach number](compressible-flow.md#mach-number). Its sound power scales as $\rho_0u^6l^2/c_0^3$. The corresponding [compact acoustic quadrupole Mach-number scaling](#compact-acoustic-quadrupole-mach-number-scaling) has density amplitude of order $(l/r)M^4$ and power $\rho_0u^8l^2/c_0^5$.

### Acoustic monopole

↑ **Parent:** [Acoustic multipole source](#acoustic-multipole-source)

An acoustic monopole represents unsteady mass or volume injection. A moving-interface mass-flux defect contributes $\partial_t(Q\delta_s)$ to the density [wave equation](wave-equation.md).

#### Rotating acoustic point source

↑ **Parent:** [Acoustic monopole](#acoustic-monopole)

A point source moving at angular speed $\Omega$ on a circle of radius $a$ has observer-direction [Mach number](compressible-flow.md#mach-number) $m=\Omega a\sin\iota/c_0$. In the far field its retarded phase satisfies $\Theta+\theta-\pi/2=\Omega(t-r/c_0)+m\sin\Theta$. For $m<1$ there is one retarded root, and a constant source strength gives $\rho'=q\dot\Theta/(4\pi c_0^2\Omega r)$. For $m>1$, multiple retarded roots can occur; their contributions require $|1-m\cos\Theta|$ and a sum over roots. Coalescing roots produce a [caustic](optics.md#wave-caustic) in the ideal point-source model.

## Lighthill acoustic analogy

↑ **Parent:** [Linear acoustics](linear-acoustics.md)

The Lighthill acoustic analogy rewrites fluid mass and momentum conservation as a constant-speed [wave equation](wave-equation.md) driven by a nonlinear [Lighthill stress tensor](#lighthill-stress-tensor). It is an exact rearrangement before making source approximations. The outgoing field can be constructed with a [retarded acoustic Green function](wave-equation.md#retarded-acoustic-green-function).

### Mass-injection term in the acoustic analogy

↑ **Parent:** [Lighthill acoustic analogy](#lighthill-acoustic-analogy)

If the [continuity equation](physics.md#continuity-equation) has mass source $M$ and the conservative momentum equation has momentum source $S_i$, elimination of momentum gives the displayed [wave equation](wave-equation.md). With no imposed momentum source, its extra term is $\partial_tM$. A compact source of total mass rate $\mathcal M=\int M\,dV$ radiates the [acoustic monopole](#acoustic-monopole) $\rho'_M=\dot{\mathcal M}(t-r/c_0)/(4\pi c_0^2r)$. The momentum source supplies an additional [acoustic dipole](#acoustic-dipole); specifying mass injection alone does not fix that dipole.

### Far-field acoustic force and stress moments

↑ **Parent:** [Lighthill acoustic analogy](#lighthill-acoustic-analogy)

For compact [Lighthill stress tensor](#lighthill-stress-tensor) and applied-force distributions, define $S_{ij}=\int T_{ij}\,d^3y$ and $F_i=\int f_i\,d^3y$. Differentiating the [retarded acoustic Green function](wave-equation.md#retarded-acoustic-green-function) at far distance gives the displayed leading radiation field, evaluated at $t-r/c_0$. Source compactness requires its size to be small compared with the acoustic wavelength, not merely with the observer distance.

### Distributional acoustic analogy across a moving interface

↑ **Parent:** [Lighthill acoustic analogy](#lighthill-acoustic-analogy)

Mass and momentum flux defects at a moving interface add surface [acoustic monopole](#acoustic-monopole) and [acoustic dipole](#acoustic-dipole) terms to [Lighthill acoustic analogy](#lighthill-acoustic-analogy). For a physical conservative fluid [shock wave](partial-differential-equation.md#shock-wave), the [Rankine-Hugoniot conditions](partial-differential-equation.md#rankine-hugoniot-conditions) set both defects to zero; the shock still affects distributional derivatives of the [Lighthill stress tensor](#lighthill-stress-tensor). A discontinuity alone is not independent mass or force injection.

#### Ffowcs Williams-Hawkings equation

↑ **Parent:** [Distributional acoustic analogy across a moving interface](#distributional-acoustic-analogy-across-a-moving-interface)

The [Lighthill acoustic analogy](#lighthill-acoustic-analogy) for a moving body has a volume [acoustic quadrupole](#acoustic-quadrupole), a surface [acoustic monopole](#acoustic-monopole) from [acoustic thickness noise](#acoustic-thickness-noise), and a surface [acoustic dipole](#acoustic-dipole) from [acoustic loading noise](#acoustic-loading-noise). For an impermeable moving surface, with outward normal $n$, normal surface speed $v_n$, and fluid and body [normal velocities](classical-mechanics.md#normal-velocity) equal, the surface [mass](classical-mechanics.md#mass) coefficient is $\rho_0v_n$ and the surface loading is the [force](classical-mechanics.md#force) exerted on the fluid. Schematically, the density-source equation is

$$
(\partial_t^2-c_0^2\nabla^2)\rho'=\partial_i\partial_j(T_{ij}H(f))+\partial_t(Q\delta_s)-\partial_i(L_i\delta_s),
\quad \delta_s=\delta(f)|\nabla f|.
$$

The density perturbation is understood with the chosen interior extension. Permeable-surface versions have additional [mass](classical-mechanics.md#mass) and momentum flux terms. Source approximations must distinguish local thickness radiation from cancellation of its compact net-volume contribution.

##### Fixed-body retarded acoustic loading formula

↑ **Parent:** [Ffowcs Williams-Hawkings equation](#ffowcs-williams-hawkings-equation)

For a fixed impermeable object, the [Ffowcs Williams-Hawkings equation](#ffowcs-williams-hawkings-equation) has a volume [acoustic quadrupole](#acoustic-quadrupole) and a surface [acoustic dipole](#acoustic-dipole), with no mass-injection term. If $F$ is the total force exerted on the fluid and $Q=\int T\,dV$ the integrated [Lighthill stress tensor](#lighthill-stress-tensor), the [acoustic compact-source approximation](#acoustic-compact-source-approximation) in the [acoustic far field](#acoustic-far-field) gives the displayed pressure at retarded time. A force convention directed onto the body reverses the loading sign. The [retarded acoustic Green function](wave-equation.md#retarded-acoustic-green-function) carries $1/c_0^2$ when the wave operator is $\partial_t^2-c_0^2\Delta$.

##### Acoustic loading noise

↑ **Parent:** [Ffowcs Williams-Hawkings equation](#ffowcs-williams-hawkings-equation)

Loading noise is the [acoustic dipole](#acoustic-dipole) radiation of the [force](classical-mechanics.md#force) exerted by a body on its surrounding fluid. For a compact, slowly moving source, the radiating [acoustic density perturbation](#acoustic-density-perturbation) is $n\cdot\dot{\mathcal F}(t-R/c_0)/(4\pi c_0^3R)$, where $\mathcal F$ is the total [force](classical-mechanics.md#force). If this total is constant, finite source-delay corrections can still create higher [acoustic multipole sources](#acoustic-multipole-source).

###### Small-body loading-noise threshold

↑ **Parent:** [Acoustic loading noise](#acoustic-loading-noise)

For a nonseparating small body in a smooth nearly inviscid eddy of speed $U$ and length $\ell$, the fluctuating resultant is an [added mass](physics.md#added-mass) or pressure-gradient force $F\sim\rho_0a^3U^2/\ell$. A uniform pressure integrates to zero over a closed surface. With time $\ell/U$, its [acoustic dipole](#acoustic-dipole) power divided by the eddy's [acoustic quadrupole](#acoustic-quadrupole) power is $(a/\ell)^6/M^2$, where $M=U/c_0$ is the [Mach number](compressible-flow.md#mach-number). Equal powers therefore give the displayed threshold. An area-scaled separated drag force with the same eddy time instead gives $a/\ell\sim\sqrt M$; a body-scale time gives a different criterion. The threshold depends on the specified loading and time models.

##### Acoustic thickness noise

↑ **Parent:** [Ffowcs Williams-Hawkings equation](#ffowcs-williams-hawkings-equation)

Thickness noise is the sound generated by displacement of fluid by a moving impermeable body, represented by the surface [acoustic monopole](#acoustic-monopole) term. For a [rigid body](classical-mechanics.md#rigid-body-dynamics), $\int_Sv_n\,dS=d\mathcal V/dt=0$, so its leading [acoustic compact-source approximation](#acoustic-compact-source-approximation) has no net-volume monopole. Its local source need not vanish: a moving finite-volume body can radiate through higher spatial moments. A thin-body or negligible-volume approximation is needed when all such radiation is to be omitted.

###### Compact radiation moments of a pulsating spherical bubble

↑ **Parent:** [Acoustic thickness noise](#acoustic-thickness-noise)

In the incompressible near field of a spherical bubble, $u_r=a^2\dot a/s^2$. Its volume-flux [acoustic monopole](#acoustic-monopole) is the displayed term at [retarded time](electromagnetism.md#retarded-time). The integrated surface pressure [force](classical-mechanics.md#force) vanishes by spherical symmetry, while the [Lighthill stress tensor](#lighthill-stress-tensor) approximation $\rho_0u_iu_j$ has moment $S_{ij}=4\pi\rho_0a^3\dot a^2\delta_{ij}/3$. Its leading compact [acoustic quadrupole](#acoustic-quadrupole) contribution is $\rho_0(a^3\dot a^2)''/(3c_0^4r)$. For small fractional radius oscillation $\delta$ and compactness parameter $\alpha=\omega a_0/c_0$, its size relative to the leading monopole is $O(\delta\alpha^2)$.

###### Translating-sphere acoustic thickness dipole

↑ **Parent:** [Acoustic thickness noise](#acoustic-thickness-noise)

For a small rigid sphere translating with [velocity](classical-mechanics.md#velocity) $\mathbf V(t)$, the integrated thickness source $\rho_0\int\mathbf V\cdot\mathbf n_s\,dS$ vanishes. The first spatial moment is instead $\rho_0\int y_j\mathbf V\cdot\mathbf n_s\,dS=\rho_0\mathcal V V_j$, where $\mathcal V$ is the sphere volume. Expanding the [retarded time](electromagnetism.md#retarded-time) across the compact source gives the displayed first nonzero thickness field. It is an [acoustic dipole](#acoustic-dipole), at the same order as [acoustic loading noise](#acoustic-loading-noise) for a translating sphere. The [added mass of a sphere](physics.md#added-mass-of-a-sphere) supplies half this volume-mass coefficient through the loading term; their sum is $3\rho_0\mathcal V\mathbf n\cdot\ddot{\mathbf V}/(8\pi c_0^3r)$.

### Lighthill stress tensor

↑ **Parent:** [Lighthill acoustic analogy](#lighthill-acoustic-analogy)

This tensor contains convective momentum flux, departure from the reference linear pressure-density relation, and viscous stress. Its double divergence is an [acoustic quadrupole](#acoustic-quadrupole) distribution in [Lighthill acoustic analogy](#lighthill-acoustic-analogy).

#### Surface sources of a discontinuous Lighthill stress tensor

↑ **Parent:** [Lighthill stress tensor](#lighthill-stress-tensor)

Write a piecewise smooth [Lighthill stress tensor](#lighthill-stress-tensor) as $T_{ij}=T^-_{ij}+D_{ij}H(S)$, where $D_{ij}=T^+_{ij}-T^-_{ij}$ and the regular level surface $S=0$ is a [shock wave](partial-differential-equation.md#shock-wave). The [distributional derivative of the Heaviside step function](distribution-theory.md#distributional-derivative-of-the-heaviside-step-function) gives

$$
\partial_i\partial_jT_{ij}=H(S)\partial_i\partial_jT^+_{ij}+H(-S)\partial_i\partial_jT^-_{ij}+(D_{ij,i}S_j+D_{ij,j}S_i+D_{ij}S_{ij})\delta(S)+D_{ij}S_iS_j\delta'(S).
$$

Here repeated indices are summed, $S_i=\partial_iS$ and $S_{ij}=\partial_i\partial_jS$. Keep the coefficients as smooth extensions before multiplying distributions: prematurely replacing the coefficient of $\delta'(S)$ by its surface trace can lose a $\delta(S)$ contribution. The extra [surface delta distributions](distribution-theory.md#surface-delta-distribution) and their derivatives are supported entirely on the discontinuity.

## Linear homentropic acoustic equations

↑ **Parent:** [Linear acoustics](linear-acoustics.md)

For perturbations $(\rho',p',\mathbf u)$ about a uniform fluid of density $\rho_0$, the linearized [continuity equation](physics.md#continuity-equation), [momentum equation](fluid-mechanics.md#euler-equations-for-an-inviscid-fluid), and [homentropic pressure perturbation](#homentropic-pressure-perturbation) relation are

$$
\rho'_t+\rho_0\nabla\mathbin\cdot\mathbf u=0,
\qquad
\rho_0\mathbf u_t=-\nabla p',
\qquad
p'=c_0^2\rho'.
$$

For [irrotational flow](fluid-mechanics.md#irrotational-flow) $\mathbf u=\nabla\phi$, they imply $p'=-\rho_0\phi_t$ and $\phi_{tt}=c_0^2\nabla^2\phi$.

### Acoustic pressure wave equation

↑ **Parent:** [Linear homentropic acoustic equations](#linear-homentropic-acoustic-equations)

Eliminating the velocity and density perturbations from the [linear homentropic acoustic equations](#linear-homentropic-acoustic-equations) gives

$$
\frac{\partial^2p'}{\partial t^2}=c_0^2\nabla^2p'.
$$

#### Outgoing acoustic square-root branch

↑ **Parent:** [Acoustic pressure wave equation](#acoustic-pressure-wave-equation)

For harmonic convention $e^{i\omega t-ikx}$, choose $\operatorname{Re}\gamma>0$ by continuation from $\operatorname{Im}\omega<0$ and impose vertical factors $e^{-\gamma y}$ above the interface and $e^{\gamma y}$ below it. At positive real frequency, $\gamma=i\sqrt{k_0^2-k^2}$ for propagating Fourier components and is positive real for evanescent components. This analytic prescription fixes the radiation branch and how the Fourier contour passes poles.

## Homentropic pressure perturbation

↑ **Parent:** [Linear acoustics](linear-acoustics.md)

For a homentropic reference state, first-order pressure and density perturbations satisfy $p'=c_0^2\rho'$, where $c_0$ is the sound speed.

## Acoustic velocity potential

↑ **Parent:** [Linear acoustics](linear-acoustics.md)

For irrotational linear acoustic flow, $\mathbf u=\nabla\phi$, $p'=-\rho_0\phi_t$, and $\phi$ obeys the wave equation.

### Outgoing acoustic field of a pulsating sphere

↑ **Parent:** [Acoustic velocity potential](#acoustic-velocity-potential)

For $R(t)=a+\operatorname{Re}(\epsilon e^{i\omega t})$, put $k=\omega/c_0$. To first order in $\epsilon/a$, the exterior outgoing velocity-potential amplitude is

$$
\widehat\phi(r)
=-\frac{i\omega\epsilon a^2}{1+ika}
\frac{e^{-ik(r-a)}}r.
$$

It satisfies $\widehat u_r(a)=\widehat\phi'(a)=i\omega\epsilon$.

#### Mean acoustic power of a pulsating sphere

↑ **Parent:** [Outgoing acoustic field of a pulsating sphere](#outgoing-acoustic-field-of-a-pulsating-sphere)

The mean power radiated by the pulsating sphere is

$$
\overline P
=2\pi a^2\rho_0\omega^2\epsilon^2c_0
\frac{\omega^2a^2}{c_0^2+\omega^2a^2}.
$$

#### Surface acoustic energy-to-flux ratio of a pulsating sphere

↑ **Parent:** [Outgoing acoustic field of a pulsating sphere](#outgoing-acoustic-field-of-a-pulsating-sphere)

At $r=a$,

$$
\frac{c_0\langle K+W\rangle}{|\langle I_r\rangle|}
=1+\frac{c_0^2}{2\omega^2a^2}.
$$

For $\omega a/c_0\gg1$, kinetic and compressional energies are equal and the field is locally radiative. For $\omega a/c_0\ll1$, reactive kinetic energy dominates and the mean radiated flux is small.

### Pressure-forced standing acoustic wave in a spherical annulus

↑ **Parent:** [Acoustic velocity potential](#acoustic-velocity-potential)

For $R<r<2R$, a rigid inner sphere and harmonic pressure

$$
p'(2R,t)=\varepsilon p_0\cos\omega t
$$

produce a standing radial field. With $k=\omega/c_0$ and $\alpha=kR$,

$$
\phi(r,t)
=-\frac{2R\varepsilon p_0}{\rho_0\omega r}
\frac{\cos k(r-R)+(kR)^{-1}\sin k(r-R)}
{\cos\alpha+\alpha^{-1}\sin\alpha}
\sin\omega t.
$$

The pressure and radial velocity are in temporal quadrature, so the period-averaged [acoustic intensity](#acoustic-energy-conservation) vanishes.

#### Radial acoustic resonance in a spherical annulus

↑ **Parent:** [Pressure-forced standing acoustic wave in a spherical annulus](#pressure-forced-standing-acoustic-wave-in-a-spherical-annulus)

The ideal pressure-forced response becomes resonant when

$$
\cos\alpha+\frac{\sin\alpha}{\alpha}=0,
$$

equivalently $\tan\alpha=-\alpha$. Damping regularizes the divergent linear response and introduces a nonzero phase lag and mean supplied power.

### Spherically symmetric vibration of a gas-filled elastic shell

↑ **Parent:** [Acoustic velocity potential](#acoustic-velocity-potential)

Let a thin spherical shell have equilibrium radius $a_0$, mass $m$ per unit area, and radial restoring stiffness $\kappa$ per unit area. If it encloses gas of density $\rho_0$ and sound speed $c_0$, its spherically symmetric normal-mode frequencies obey

$$
\boxed{\theta^2\left(1+\frac\alpha{\theta\cot\theta-1}\right)
=\frac{\kappa a_0^2}{mc_0^2},
\qquad
\theta=\frac{\omega a_0}{c_0},
\quad
\alpha=\frac{\rho_0a_0}{m}.}
$$

The fraction is the frequency-dependent acoustic added mass of the enclosed gas.

## Acoustic energy conservation

↑ **Parent:** [Linear acoustics](linear-acoustics.md)

Linear acoustic fields obey

$$
\frac{\partial}{\partial t}(K+W)+\nabla\cdot\mathbf I=0,
$$

where

$$
K=\frac12\rho_0|\mathbf u|^2,
\qquad
W=\frac{p'^2}{2\rho_0c_0^2},
\qquad
\mathbf I=p'\mathbf u.
$$

### Near-field energy imbalance in a spherical acoustic wave

↑ **Parent:** [Acoustic energy conservation](#acoustic-energy-conservation)

For outgoing [velocity potential](fluid-mechanics.md#velocity-potential) $\phi=F(r-ct)/r$, the radial velocity is $F'/r-F/r^2$ and the pressure perturbation is $\rho_0cF'/r$. The [acoustic energy density](#acoustic-energy-density) separates into kinetic density $\rho_0(F'/r-F/r^2)^2/2$ and compressional density $\rho_0(F'/r)^2/2$. They are generally unequal near the source but agree at leading far-field order. The additional $r^{-2}$ velocity term is the spherical near field.

### Acoustic energy density

↑ **Parent:** [Acoustic energy conservation](#acoustic-energy-conservation)

For a linear acoustic perturbation of a uniform fluid,

$$
E=\frac12\rho_0|\mathbf u|^2
+\frac{p'^2}{2\rho_0c_0^2}
$$

is the sum of kinetic and compressional energy densities. Together with the [acoustic energy flux](continuum-mechanics.md#acoustic-energy-flux) $\mathbf I=p'\mathbf u$, it satisfies $E_t+\nabla\mathbin\cdot\mathbf I=0$.

## Evanescent acoustic surface wave

↑ **Parent:** [Linear acoustics](linear-acoustics.md)

A surface wave with phase speed below the bulk sound speed decays normally as $e^{-\alpha z}$, where $\alpha=k\sqrt{1-c^2/c_0^2}$.

### Acoustic wave on a tensioned massive membrane

↑ **Parent:** [Evanescent acoustic surface wave](#evanescent-acoustic-surface-wave)

A membrane of mass per area $m$ and tension $T$ separating two identical acoustic half-spaces has evanescent modes with

$$
\left(m+\frac{2\rho_0}{\sqrt{k^2-\omega^2/c_0^2}}\right)\omega^2=Tk^2.
$$

The second term is the [added mass of an evanescent fluid layer](#added-mass-of-an-evanescent-fluid-layer) contributed by both sides. Hence the phase speed is below the vacuum membrane speed $\sqrt{T/m}$, and for $k\to0$ it obeys $c\sim\sqrt{Tk/(2\rho_0)}\to0$. Pressure and normal velocity are in quadrature, so the mean normal [acoustic energy flux](continuum-mechanics.md#acoustic-energy-flux) vanishes.

#### Elastic-sheet tension

↑ **Parent:** [Acoustic wave on a tensioned massive membrane](#acoustic-wave-on-a-tensioned-massive-membrane)

The in-plane tensile [force](classical-mechanics.md#force) per unit transverse length in a thin elastic sheet produces the linear transverse restoring [force](classical-mechanics.md#force) $T\eta_{xx}$ per unit area. A spatially uniform displacement has zero curvature and hence no [elastic-sheet tension](#elastic-sheet-tension) [force](classical-mechanics.md#force). This explains why infinite [elastic-sheet tension](#elastic-sheet-tension) blocks fixed nonzero-wavenumber [acoustic membrane waves](#acoustic-wave-on-a-tensioned-massive-membrane) but does not make the uniform mode rigid. The sheet's inertia, by contrast, acts also on uniform oscillations.

#### Point-force radiation from a fluid-loaded sheet

↑ **Parent:** [Acoustic wave on a tensioned massive membrane](#acoustic-wave-on-a-tensioned-massive-membrane)

A harmonic line [force](classical-mechanics.md#force) localized at one point of a two-dimensional sheet gives $\widehat\eta=F/D$ and $\Delta=\gamma D$ in the [Fourier transform](analysis.md#fourier-transform). The outgoing upper [pressure](thermodynamics.md#pressure) is the displayed amplitude. Dividing by $c_0^2$ converts it to [acoustic density perturbation](#acoustic-density-perturbation). The [method of steepest descent](analysis.md#method-of-steepest-descent) gives cylindrical sound from the [saddle point](analysis.md#saddle-point), while crossed zeros of the [dispersion relation](wave-equation.md#dispersion-relation) give guided or leaky modal residues. Retaining $k_0=\omega/c_0$ is essential for dimensionally consistent spreading and prefactors.

##### One-sided fluid-loaded membrane radiation

↑ **Parent:** [Point-force radiation from a fluid-loaded sheet](#point-force-radiation-from-a-fluid-loaded-sheet)

For one acoustic half-space and vacuum on the other side, a harmonic point [force](classical-mechanics.md#force) gives displacement amplitude $F\gamma/D$ and fluid [acoustic velocity potential](#acoustic-velocity-potential) amplitude $i\omega F e^{-\gamma y}/D$. For time dependence $e^{-i\omega t}$, the [outgoing acoustic square-root branch](#outgoing-acoustic-square-root-branch) has $\gamma>0$ for $|k|>k_0$ and $\gamma=-i\sqrt{k_0^2-k^2}$ for $|k|<k_0$. The causal limit $\omega\mapsto\omega+i0$ places the positive guided-mode pole above the inversion contour and the negative pole below. The [saddle point](analysis.md#saddle-point) generates cylindrical radiation, whereas guided residues decay normally to the membrane.

#### Tensioned-sheet acoustic impedance

↑ **Parent:** [Acoustic wave on a tensioned massive membrane](#acoustic-wave-on-a-tensioned-massive-membrane)

A sheet of [mass](classical-mechanics.md#mass) per area $m$ and [elastic-sheet tension](#elastic-sheet-tension) $T$ backed by an identical outgoing fluid half-space presents the stated [surface acoustic impedance](continuum-mechanics.md#surface-acoustic-impedance) to the other half-space, using upward sheet [velocity](classical-mechanics.md#velocity) $i\omega\eta=-V$. The fluid term is its [normal acoustic impedance](continuum-mechanics.md#normal-acoustic-impedance); the remaining term is structural. Infinite [elastic-sheet tension](#elastic-sheet-tension) suppresses every fixed nonzero spatial wavenumber, but not $k=0$, whereas infinite [mass](classical-mechanics.md#mass) suppresses even spatially uniform motion. A massless untensioned sheet between identical fluids is transparent.

##### Reflection pole of a fluid-loaded membrane

↑ **Parent:** [Tensioned-sheet acoustic impedance](#tensioned-sheet-acoustic-impedance)

A free [acoustic membrane wave](#acoustic-wave-on-a-tensioned-massive-membrane) is a zero of the outgoing [dispersion relation](wave-equation.md#dispersion-relation) $D$. At this zero, the impedance seen from one side equals the negative of that side's outgoing [normal acoustic impedance](continuum-mechanics.md#normal-acoustic-impedance). Thus the continued by [analytic continuation](complex-analysis.md#analytic-continuation) [reflection coefficient](partial-differential-equation.md#reflection-coefficient) has a pole. A real guided mode is evanescent normal to the sheet; a complex root can describe a leaky mode. The pole describes nontrivial homogeneous motion with no incoming wave, rather than unbounded passive reflection at an ordinary real incidence angle.

#### Fluid-loaded membrane edge scattering

↑ **Parent:** [Acoustic wave on a tensioned massive membrane](#acoustic-wave-on-a-tensioned-massive-membrane)

A pinned semi-infinite membrane scatters an incoming guided mode into reflected guided modes and outgoing sound. For unit incident displacement the scattered endpoint value is $-1$. Its [Half-range Fourier transform](analysis.md#half-range-fourier-transform) therefore has nonzero endpoint terms even though the total displacement vanishes. The [Wiener-Hopf equation](differential-equation.md#wiener-hopf-equation) kernel is $2/(m\omega^2-Tk^2)+\gamma/(\rho_0\omega^2)$ with the outgoing branch $\gamma^2=k^2-\omega^2/c_0^2$.

##### Plane-wave forcing of a pinned elastic half-sheet

↑ **Parent:** [Fluid-loaded membrane edge scattering](#fluid-loaded-membrane-edge-scattering)

For identical unit-density, unit-sound-speed fluids above and below a sheet on $x<0$, use time $e^{i\omega t}$ and transform $\int e^{ikx}\phi\,dx$. The [outgoing acoustic square-root branch](#outgoing-acoustic-square-root-branch) obeys $\gamma^2=k^2-\omega^2$. If $J$ is the pressure jump upper minus lower, $s=\eta'(0)$ and $d^+$ the right [Half-range Fourier transform](analysis.md#half-range-fourier-transform) of the scattered normal derivative, the [Wiener-Hopf equation](differential-equation.md#wiener-hopf-equation) is

$$
KJ+d^+=\frac{\omega\sin\theta_0}{k+\omega\cos\theta_0}+\frac{T\omega^2s}{m\omega^2-Tk^2}.
$$

The total displacement is pinned, so its transformed second derivative is $s-k^2\eta^-$. The bare-sheet pole $b=\omega\sqrt{m/T}$ in reconstructed displacement must cancel: $J(b)=Ts$. This is an [incoming-pole cancellation at a pinned membrane edge](#incoming-pole-cancellation-at-a-pinned-membrane-edge) condition, distinct from the outgoing coupled-mode pole at the zero of $K$.

##### Incoming-pole cancellation at a pinned membrane edge

↑ **Parent:** [Fluid-loaded membrane edge scattering](#fluid-loaded-membrane-edge-scattering)

Reconstructing the left scattered displacement in [fluid-loaded membrane edge scattering](#fluid-loaded-membrane-edge-scattering) divides by $m\omega^2-Tk^2$. The pole at the lower bare-membrane wavenumber $b=\omega\sqrt{m/T}$ must cancel to preserve outgoing half-plane analyticity. This gives a linear condition determining the otherwise unknown endpoint slope $A$. The prescribed incident pole in the total field is a different singularity.

### Spring-supported acoustic membrane wave

↑ **Parent:** [Evanescent acoustic surface wave](#evanescent-acoustic-surface-wave)

For a massless spring-supported membrane adjoining a fluid half-space, kinematic and pressure balance give the dispersion relation $As^4+s^2-1=0$ with $s=c/c_0$.

#### Acoustic membrane dispersion asymptotics

↑ **Parent:** [Spring-supported acoustic membrane wave](#spring-supported-acoustic-membrane-wave)

For $As^4+s^2-1=0$, the physical speed approaches $c_0(1-A/2)$ as $A$ tends to zero and scales as $c_0A^{-1/4}$ as $A$ tends to infinity.

### Added mass of an evanescent fluid layer

↑ **Parent:** [Evanescent acoustic surface wave](#evanescent-acoustic-surface-wave)

A disturbance decaying over depth $1/k$ accelerates fluid mass of order $\rho_0/k$ per unit area, giving a frequency-dependent added inertia.

## Time average of harmonic power

↑ **Parent:** [Linear acoustics](linear-acoustics.md)

For real harmonic fields with complex amplitudes $\widehat p$ and $\widehat u$, their period-averaged product is $\operatorname{Re}(\widehat p\widehat u^*)/2$.

### Reactive acoustic energy flux

↑ **Parent:** [Time average of harmonic power](#time-average-of-harmonic-power)

When pressure and velocity are in quadrature, their instantaneous energy flux oscillates but its period average vanishes.

## ↑ Ancestors (4)

1. [Fluid mechanics](fluid-mechanics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-70.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1.md#40c/a/solution)
- [Stationary vorticity mode in linear acoustics](#stationary-vorticity-mode-in-linear-acoustics)
