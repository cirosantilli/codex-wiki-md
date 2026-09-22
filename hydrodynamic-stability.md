# Hydrodynamic stability

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hydrodynamic_stability)

Hydrodynamic stability studies whether small disturbances to a fluid base state decay, remain neutral, or grow. Linear normal modes reduce this question to eigenvalues or growth rates.

**Table of contents**

- [Global hydrodynamic mode](#global-hydrodynamic-mode)
- [Global hydrodynamic instability](#global-hydrodynamic-instability)
  - [Global modes of a quadratically confined Ginzburg-Landau equation](#global-modes-of-a-quadratically-confined-ginzburg-landau-equation)
- [Critical layer in a shear flow](#critical-layer-in-a-shear-flow)
  - [Neutral-mode critical-layer matching](#neutral-mode-critical-layer-matching)
    - [Neutral Rayleigh-mode dispersion correction](#neutral-rayleigh-mode-dispersion-correction)
  - [Prandtl critical layer at a stationary shear profile](#prandtl-critical-layer-at-a-stationary-shear-profile)
    - [High-wavenumber instability of a non-monotone Prandtl layer](#high-wavenumber-instability-of-a-non-monotone-prandtl-layer)
- [Critical level of a shear-flow wave](#critical-level-of-a-shear-flow-wave)
- [Baroclinic instability](#baroclinic-instability)
- [Three-layer long-wave shear-flow matching](#three-layer-long-wave-shear-flow-matching)
  - [Airy wall-layer matching determinant](#airy-wall-layer-matching-determinant)
- [Pressure equation for a shear-flow normal mode](#pressure-equation-for-a-shear-flow-normal-mode)
- [Adjoint linearized Navier-Stokes evolution](#adjoint-linearized-navier-stokes-evolution)
- [Kinetic-energy inner product](#kinetic-energy-inner-product)
- [Stability diagram of the linear complex Ginzburg-Landau equation](#stability-diagram-of-the-linear-complex-ginzburg-landau-equation)
- [Saddle growth rate along a ray](#saddle-growth-rate-along-a-ray)
- [Convective hydrodynamic instability](#convective-hydrodynamic-instability)
- [Absolute hydrodynamic instability](#absolute-hydrodynamic-instability)
  - [Anisotropic absolute-instability threshold for positive diffusion](#anisotropic-absolute-instability-threshold-for-positive-diffusion)
  - [Absolute frequency](#absolute-frequency)
    - [Absolute-frequency conservation in steady shear](#absolute-frequency-conservation-in-steady-shear)
    - [Absolute growth rate](#absolute-growth-rate)
    - [Absolute wavenumber](#absolute-wavenumber)
- [Orr-Sommerfeld equation](#orr-sommerfeld-equation)
  - [Squire's theorem](#squire-s-theorem)
    - [Squire transformation](#squire-transformation)
  - [Airy reduction of the Orr-Sommerfeld equation in constant shear](#airy-reduction-of-the-orr-sommerfeld-equation-in-constant-shear)
    - [Velocity reconstruction from the Orr-Sommerfeld vorticity](#velocity-reconstruction-from-the-orr-sommerfeld-vorticity)
  - [Squire equation](#squire-equation)
    - [Squire mode](#squire-mode)
      - [Dissipation identity for a homogeneous Squire mode](#dissipation-identity-for-a-homogeneous-squire-mode)
  - [Orr-Sommerfeld mode](#orr-sommerfeld-mode)
- [Inertial instability](#inertial-instability)
- [Rayleigh equation for inviscid shear flow](#rayleigh-equation-for-inviscid-shear-flow)
  - [Inviscid instability of a piecewise-linear mixing layer](#inviscid-instability-of-a-piecewise-linear-mixing-layer)
  - [Axisymmetric inviscid pipe stability equation](#axisymmetric-inviscid-pipe-stability-equation)
    - [Evanescent potential modes of inviscid Poiseuille flow](#evanescent-potential-modes-of-inviscid-poiseuille-flow)
  - [Inviscid instability of a triangular jet](#inviscid-instability-of-a-triangular-jet)
  - [Pressure matching at a piecewise-linear shear interface](#pressure-matching-at-a-piecewise-linear-shear-interface)
  - [Fjørtoft theorem](#fjortoft-theorem)
  - [Inviscid Couette continuous spectrum](#inviscid-couette-continuous-spectrum)
    - [Inviscid Couette initial-value Green function](#inviscid-couette-initial-value-green-function)
    - [Linear inviscid damping in unbounded Couette flow](#linear-inviscid-damping-in-unbounded-couette-flow)
    - [Vorticity-sheet eigenfunction of inviscid Couette flow](#vorticity-sheet-eigenfunction-of-inviscid-couette-flow)
  - [Vorticity-jump matching for an inviscid shear flow](#vorticity-jump-matching-for-an-inviscid-shear-flow)
  - [Inviscid parallel shear flow](#inviscid-parallel-shear-flow)
    - [Unbounded piecewise-linear shear layer](#unbounded-piecewise-linear-shear-layer)
    - [Three-layer stratified piecewise-linear shear flow](#three-layer-stratified-piecewise-linear-shear-flow)
      - [Quartic dispersion relation for a three-layer stratified shear flow](#quartic-dispersion-relation-for-a-three-layer-stratified-shear-flow)
      - [Unstable band of a three-layer stratified shear flow](#unstable-band-of-a-three-layer-stratified-shear-flow)
    - [Hazel model](#hazel-model)
      - [Neutral mode of the equal-width Hazel model](#neutral-mode-of-the-equal-width-hazel-model)
        - [Critical-layer regularity of a neutral Hazel mode](#critical-layer-regularity-of-a-neutral-hazel-mode)
    - [Bounded piecewise-linear shear layer](#bounded-piecewise-linear-shear-layer)
      - [Instability threshold for a bounded piecewise-linear shear layer](#instability-threshold-for-a-bounded-piecewise-linear-shear-layer)
  - [Rayleigh's inflection-point theorem](#rayleigh-s-inflection-point-theorem)
  - [Howard's semicircle theorem](#howard-s-semicircle-theorem)
    - [Weighted identity for Howard's semicircle theorem](#weighted-identity-for-howard-s-semicircle-theorem)
- [Counterpropagating wave instability](#counterpropagating-wave-instability)
  - [Counterpropagating wave resonance in a three-layer shear flow](#counterpropagating-wave-resonance-in-a-three-layer-shear-flow)
- [Transient growth from non-normal modes](#transient-growth-from-non-normal-modes)
  - [Orr mechanism](#orr-mechanism)
  - [Lift-up effect](#lift-up-effect)
- [Energy-stability threshold](#energy-stability-threshold)
- [Symmetric instability](#symmetric-instability)
- [Eady model](#eady-model)
  - [Eady model with parallel sloping boundaries](#eady-model-with-parallel-sloping-boundaries)
  - [Boundary pseudomomentum of a sloping Eady layer](#boundary-pseudomomentum-of-a-sloping-eady-layer)
  - [Finite-depth Eady dispersion relation](#finite-depth-eady-dispersion-relation)
  - [Semi-infinite Eady model](#semi-infinite-eady-model)
    - [Absence of exponential instability in the semi-infinite Eady model](#absence-of-exponential-instability-in-the-semi-infinite-eady-model)
    - [Semi-infinite Eady edge wave](#semi-infinite-eady-edge-wave)
      - [Dispersion relation of a semi-infinite Eady edge wave](#dispersion-relation-of-a-semi-infinite-eady-edge-wave)
        - [Steering height of a semi-infinite Eady edge wave](#steering-height-of-a-semi-infinite-eady-edge-wave)
      - [Decaying vertical structure of a semi-infinite Eady edge wave](#decaying-vertical-structure-of-a-semi-infinite-eady-edge-wave)
  - [Eady model with a sloping lower boundary](#eady-model-with-a-sloping-lower-boundary)
    - [Instability for negative slopes in the sloping-boundary Eady model](#instability-for-negative-slopes-in-the-sloping-boundary-eady-model)
  - [Eady instability](#eady-instability)
  - [Boundary Rossby wave](#boundary-rossby-wave)
    - [Eady edge wave](#eady-edge-wave)
      - [Forced Eady edge wave](#forced-eady-edge-wave)
      - [Sloping-boundary Eady edge wave](#sloping-boundary-eady-edge-wave)
    - [Quasi-geostrophic wave at a stratification interface](#quasi-geostrophic-wave-at-a-stratification-interface)
  - [Damped Eady-wave dispersion relation](#damped-eady-wave-dispersion-relation)
- [Dissipation-induced instability](#dissipation-induced-instability)
- [Rayleigh discriminant](#rayleigh-discriminant)
  - [Rayleigh's circulation criterion](#rayleigh-s-circulation-criterion)

## Global hydrodynamic mode

↑ **Parent:** [Hydrodynamic stability](hydrodynamic-stability.md)

A global hydrodynamic mode is a separated solution $a(x)e^{-i\omega t}$ satisfying the complete spatial [boundary conditions](differential-equation.md#boundary-condition) of a linearized flow problem. Its [eigenvalue](linear-operator-theory.md#eigenvalue) depends on the spatial domain and variable coefficients, rather than solely on a local [dispersion relation](wave-equation.md#dispersion-relation).

## Global hydrodynamic instability

↑ **Parent:** [Hydrodynamic stability](hydrodynamic-stability.md)

A spatially nonuniform system is globally unstable when a [normal mode](wave-equation.md#normal-mode) satisfying its global spatial [boundary conditions](differential-equation.md#boundary-condition) has positive temporal [growth rate](wave-equation.md#growth-rate). This differs from purely local temporal amplification or [convective wave-packet instability](wave-equation.md#convective-wave-packet-instability). A locally absolutely unstable region can be necessary without being sufficient for a growing global mode of finite spatial extent.

### Global modes of a quadratically confined Ginzburg-Landau equation

↑ **Parent:** [Global hydrodynamic instability](#global-hydrodynamic-instability)

For the whole-line [linear complex Ginzburg-Landau equation](partial-differential-equation.md#linear-complex-ginzburg-landau-equation) with real positive diffusion $\gamma$ and $\mu(x)=\mu_0-\nu\epsilon^2x^2$, removing drift and scaling $\xi=\sqrt\epsilon(\nu/\gamma)^{1/4}x$ gives the [Hermite differential equation](analysis.md#hermite-differential-equation). Decay at both infinities quantizes the spectral parameter to $2j+1$. The strongest mode is $j=0$, giving global instability iff $\mu_0>U^2/(4\gamma)+\epsilon\sqrt{\gamma\nu}$. The confinement correction vanishes in the slow-profile limit, recovering the homogeneous [absolute wave-packet instability](wave-equation.md#absolute-wave-packet-instability) threshold.

## Critical layer in a shear flow

↑ **Parent:** [Hydrodynamic stability](hydrodynamic-stability.md)

A critical layer is a region where the leading wave phase speed coincides with the local shear-flow [velocity](classical-mechanics.md#velocity) and an outer approximation degenerates. Small viscosity or other corrections must then be retained on a distinguished transverse scale. The width depends on the order of vanishing of $U-c_0$ and on the governing mode equation; simple-shear and stationary-profile layers have different balances.

### Neutral-mode critical-layer matching

↑ **Parent:** [Critical layer in a shear flow](#critical-layer-in-a-shear-flow)

For a monotone [inviscid parallel shear flow](#inviscid-parallel-shear-flow), let a regular neutral [Rayleigh equation for inviscid shear flow](#rayleigh-equation-for-inviscid-shear-flow) mode have $U(0)=c_0$, $U''(0)=0$, $d=U'(0)>0$, and $p=\phi_0(0)\ne0$. A perturbation $c=c_0+\varepsilon c_1$ with $\operatorname{Im}c_1>0$ resolves the singularity on the [inner variable](differential-equation.md#inner-variable) $\eta=y/\varepsilon$. The first outer correction has $\phi_1=a+\beta y\log|y|+b_\pm y+\cdots$, with $\beta=c_1U'''(0)p/d^2$. The inner particular solution contains $(d\eta-c_1)\log(d\eta-c_1)$. Its [complex logarithm](analysis.md#complex-logarithm) has argument tending to zero at positive infinity and to $-\pi$ at negative infinity, giving the displayed matching jump.

#### Neutral Rayleigh-mode dispersion correction

↑ **Parent:** [Neutral-mode critical-layer matching](#neutral-mode-critical-layer-matching)

Let $I=\int\phi_0^2dy$, $J=\operatorname{PV}\int U''\phi_0^2/(U-c_0)^2dy$, and $M=U'''(0)\phi_0(0)^2/U'(0)^2$. The [Wronskian](differential-equation.md#wronskian) identity for the first-order [Rayleigh equation for inviscid shear flow](#rayleigh-equation-for-inviscid-shear-flow), combined with [neutral-mode critical-layer matching](#neutral-mode-critical-layer-matching), gives $2k_0k_1I=-c_1(J+i\pi M)$. For real $k_1$, its imaginary part is $2k_0k_1I\pi M/(J^2+\pi^2M^2)$. The [Cauchy principal value](complex-analysis.md#cauchy-principal-value) is necessary when the outer forcing has a simple real pole.

### Prandtl critical layer at a stationary shear profile

↑ **Parent:** [Critical layer in a shear flow](#critical-layer-in-a-shear-flow)

For the [Prandtl normal-mode equation](viscous-fluid-flow.md#prandtl-normal-mode-equation) with viscosity scaled to one and a profile having a nondegenerate [stationary point](calculus-of-variations.md#stationary-point), $U-c_0\sim (y-y_c)^2/2$. A piecewise outer mode proportional to $U-c_0$ has a second-derivative jump. Balancing the advective and third-derivative terms smooths that jump over width $\alpha^{-1/4}$, with [velocity](classical-mechanics.md#velocity) amplitude $\alpha^{-1/2}$ and a phase-speed correction of the same order. Matching selects the [eigenvalue](linear-operator-theory.md#eigenvalue) through a third-order inner problem.

#### High-wavenumber instability of a non-monotone Prandtl layer

↑ **Parent:** [Prandtl critical layer at a stationary shear profile](#prandtl-critical-layer-at-a-stationary-shear-profile)

A [stationary point](calculus-of-variations.md#stationary-point) in a non-monotone [velocity profile](viscous-fluid-flow.md#velocity-profile) can support a [quarter-power critical layer](#prandtl-critical-layer-at-a-stationary-shear-profile) whose phase-speed correction has positive imaginary part. The resulting [normal mode](wave-equation.md#normal-mode) grows at a rate proportional to the square root of the [wavenumber](wave-equation.md#wavenumber). Such unbounded high-frequency amplification demonstrates [linear instability](algebra.md#linear-instability) of the frozen layer; nonlinear evolution and precise well-posedness consequences require separate analysis.

## Critical level of a shear-flow wave

↑ **Parent:** [Hydrodynamic stability](hydrodynamic-stability.md)

For a wave with zonal [phase velocity](wave-equation.md#phase-velocity) $c$ in a basic shear $U(z)$, a critical level is a height $z_c$ at which $U(z_c)=c$. The Doppler-shifted material frequency then vanishes. This means equality of the laboratory velocities; the $U$ and $-c$ terms cancel in the wave frame. It does not mean $U=-c$. A [semi-infinite Eady edge wave](#semi-infinite-eady-edge-wave) with zero interior [potential vorticity](geophysical-fluid-dynamics.md#potential-vorticity) anomaly can remain regular through its steering height.

## Baroclinic instability

↑ **Parent:** [Hydrodynamic stability](hydrodynamic-stability.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Baroclinic_instability)

[Baroclinic instability](#baroclinic-instability) converts [potential energy](classical-mechanics.md#potential-energy) of a stratified sheared basic flow into growing disturbances. In the [Eady model](#eady-model), coupled [Boundary Rossby waves](#boundary-rossby-wave) provide a useful mechanism: their induced velocities displace boundary [buoyancy](fluid-mechanics.md#buoyancy) anomalies, and suitable wavelengths permit phase locking. A single neutral boundary wave does not by itself imply exponential instability.

## Three-layer long-wave shear-flow matching

↑ **Parent:** [Hydrodynamic stability](hydrodynamic-stability.md)

A high-[Reynolds number](fluid-mechanics.md#reynolds-number) long-wave mode near a wall has a viscous layer of thickness $\delta=(\alpha R)^{-1/3}$, an order-one region following the base profile, and a pressure-decay region of thickness $1/\alpha$. The lower [Airy function](differential-equation.md#airy-function) solution fixes velocity displacement and [fluid pressure](fluid-mechanics.md#fluid-pressure). The middle [Rayleigh equation for inviscid shear flow](#rayleigh-equation-for-inviscid-shear-flow) transports these to the outer constant-velocity region. Matching its decaying pressure produces an [Airy wall-layer matching determinant](#airy-wall-layer-matching-determinant). For order-one amplitudes, constant leading middle pressure requires $\alpha^2\ll\delta$; the distinguished balance $\alpha\sim\delta$ gives $\alpha\sim R^{-1/4}$.

### Airy wall-layer matching determinant

↑ **Parent:** [Three-layer long-wave shear-flow matching](#three-layer-long-wave-shear-flow-matching)

With the [Airy displacement integrals](differential-equation.md#airy-displacement-integral), the lower pressure-to-velocity ratio is $-iq\operatorname{Ai}\prime(-qC)/I_0(C)$. The decaying upper mode gives that ratio as $\alpha/\delta$. Hence for $\alpha=kR^{-1/4}$ the [dispersion relation](wave-equation.md#dispersion-relation) is $k^{4/3}I_0(C)+iq\operatorname{Ai}\prime(-qC)=0$. Writing it without division remains meaningful if an individual moment vanishes. The wavespeed is $c=\delta C$ and a positive wavenumber grows temporally when $\operatorname{Im}C>0$.

## Pressure equation for a shear-flow normal mode

↑ **Parent:** [Hydrodynamic stability](hydrodynamic-stability.md)

For an incompressible parallel flow with base velocity $U(y)$ and perturbation proportional to $e^{i\alpha(x-ct)}$, divergence of the linearized momentum equations gives $p\prime\prime-\alpha^2p=-2i\alpha U\prime v$. At a [no-slip boundary condition](viscous-fluid-flow.md#no-slip-boundary-condition), streamwise momentum gives $p(0)=u\prime\prime(0)/(i\alpha R)$. The equation encodes how base shear generates perturbation [fluid pressure](fluid-mechanics.md#fluid-pressure).

## Adjoint linearized Navier-Stokes evolution

↑ **Parent:** [Hydrodynamic stability](hydrodynamic-stability.md)

Relative to the [kinetic-energy inner product](#kinetic-energy-inner-product), integration by parts reverses incompressible base transport, transposes the velocity-gradient coupling, and preserves viscous diffusion. With reverse time $\tau=-t$, the adjoint base state is evaluated at $-\tau$. The [Leray-Helmholtz projection](viscous-fluid-flow.md#leray-helmholtz-projection) or adjoint pressure enforces divergence-free adjoint velocity. The [curl of a cross product](calculus.md#curl-of-a-cross-product) and [vorticity cross-product identity](fluid-mechanics.md#vorticity-cross-product-identity) give the equivalent form $\partial_\tau v=\Omega\times v-\nabla\times(U\times v)-\nabla\pi+\mathrm{Re}^{-1}\Delta v$.

## Kinetic-energy inner product

↑ **Parent:** [Hydrodynamic stability](hydrodynamic-stability.md)

For a constant reference density, fluid perturbation [kinetic energy](classical-mechanics.md#kinetic-energy) is proportional to $\|u\|^2/2$ under the displayed $L^2$ [inner product](linear-algebra.md#inner-product). An [adjoint operator](hilbert-space.md#adjoint-operator) for perturbation evolution must be defined relative to this inner product, including [boundary conditions](differential-equation.md#boundary-condition) and the projection onto [incompressible flow](fluid-mechanics.md#incompressible-flow).

## Stability diagram of the linear complex Ginzburg-Landau equation

↑ **Parent:** [Hydrodynamic stability](hydrodynamic-stability.md)

For the [linear complex Ginzburg-Landau equation](partial-differential-equation.md#linear-complex-ginzburg-landau-equation) with real $U,c_d,\mu$ and positive real diffusion coefficient scaled to one, the maximum [temporal growth rate](wave-equation.md#growth-rate) is $\mu$ and the [absolute growth rate](#absolute-growth-rate) is $\mu-U^2/[4(1+c_d^2)]$. For $U>0$, $\mu<0$ is stable, $0<\mu<\mu_a$ has [convective hydrodynamic instability](#convective-hydrodynamic-instability), and $\mu>\mu_a$ has [absolute hydrodynamic instability](#absolute-hydrodynamic-instability). Both equality boundaries are marginal in exponential rate.

## Saddle growth rate along a ray

↑ **Parent:** [Hydrodynamic stability](hydrodynamic-stability.md)

On a ray $x/t=V$, a localized [wave packet](wave-equation.md#wave-packet) is governed by a physically selected [saddle point](analysis.md#saddle-point) satisfying $d\omega/dk=V$ in its analytic [dispersion relation](wave-equation.md#dispersion-relation). The exponent's real growth is $\operatorname{Im}(\omega_\star-Vk_\star)$. The fixed-frame case $V=0$ gives the [absolute growth rate](#absolute-growth-rate). This ray formulation makes the frame dependence of [convective hydrodynamic instability](#convective-hydrodynamic-instability) explicit.

## Convective hydrodynamic instability

↑ **Parent:** [Hydrodynamic stability](hydrodynamic-stability.md)

A [convective hydrodynamic instability](#convective-hydrodynamic-instability) amplifies an advected localized disturbance while its amplitude decays at any fixed position. The distinction from [absolute hydrodynamic instability](#absolute-hydrodynamic-instability) depends on the observation frame.

## Absolute hydrodynamic instability

↑ **Parent:** [Hydrodynamic stability](hydrodynamic-stability.md)

An [absolute hydrodynamic instability](#absolute-hydrodynamic-instability) makes the response to a localized impulse grow at a fixed spatial point in a specified frame. This differs from [convective hydrodynamic instability](#convective-hydrodynamic-instability), which amplifies a moving [wave packet](wave-equation.md#wave-packet) while its response decays at fixed positions. For analytic [dispersion relations](wave-equation.md#dispersion-relation), the relevant [absolute frequency](#absolute-frequency) is associated with an accessible zero-[group velocity](wave-equation.md#group-velocity) saddle, with the spatial-branch selection checked rather than assumed for an arbitrary dispersion relation.

### Anisotropic absolute-instability threshold for positive diffusion

↑ **Parent:** [Absolute hydrodynamic instability](#absolute-hydrodynamic-instability)

For $\eta_t+\boldsymbol c\cdot\nabla\eta=\mu\eta+\nabla\cdot(\Gamma\nabla\eta)$ with symmetric positive definite $\Gamma$, the [dispersion relation](wave-equation.md#dispersion-relation) is $\omega=\boldsymbol c\cdot\boldsymbol k+i(\mu-\boldsymbol k^T\Gamma\boldsymbol k)$. Its zero-[group velocity](wave-equation.md#group-velocity) saddle is $\boldsymbol k_0=-i\Gamma^{-1}\boldsymbol c/2$. The anisotropic [heat kernel](diffusion-equation.md#heat-kernel) has fixed-position exponential rate $\mu-\boldsymbol c^T\Gamma^{-1}\boldsymbol c/4$, so this accessible saddle gives the actual threshold. At fixed speed $q$, the threshold ranges from $q^2/(4d_{\max})$ to $q^2/(4d_{\min})$, where $d_{\min},d_{\max}$ are the [eigenvalues](linear-operator-theory.md#eigenvalue) of $\Gamma$. Absence of [absolute hydrodynamic instability](#absolute-hydrodynamic-instability) in every direction requires the upper bound $\mu\le q^2/(4d_{\max})$.

### Absolute frequency

↑ **Parent:** [Absolute hydrodynamic instability](#absolute-hydrodynamic-instability)

The [absolute frequency](#absolute-frequency) is the generally complex [angular frequency](classical-mechanics.md#angular-frequency) at the physically selected [absolute wavenumber](#absolute-wavenumber). Its [imaginary part](complex-analysis.md#imaginary-part) is the fixed-position exponential [growth rate](wave-equation.md#growth-rate) under the convention $e^{-i\omega t}$. Marginal zero exponential growth may still carry an algebraic prefactor.

#### Absolute-frequency conservation in steady shear

↑ **Parent:** [Absolute frequency](#absolute-frequency)

A time-independent ray Hamiltonian conserves the stationary-observer [absolute frequency](#absolute-frequency). A horizontally uniform background also conserves horizontal wavenumber. The [intrinsic frequency](gravity-wave.md#intrinsic-frequency) $\widehat\omega=\omega-kU(z)$ nevertheless changes when the ray moves through shear. These follow from the [Hamiltonian ray-tracing equations](continuum-mechanics.md#hamiltonian-ray-tracing-equations) and are essential to identifying a [critical level of an internal gravity wave](gravity-wave.md#critical-level-of-an-internal-gravity-wave).

#### Absolute growth rate

↑ **Parent:** [Absolute frequency](#absolute-frequency)

The absolute growth rate is the exponential [growth rate](wave-equation.md#growth-rate) of a localized impulse at a fixed position in the chosen observation frame. Under the convention $e^{i(kx-\omega t)}$, it is the [imaginary part](complex-analysis.md#imaginary-part) of the physically selected [absolute frequency](#absolute-frequency). Positive values give [absolute hydrodynamic instability](#absolute-hydrodynamic-instability); negative values can still coexist with [convective hydrodynamic instability](#convective-hydrodynamic-instability).

#### Absolute wavenumber

↑ **Parent:** [Absolute frequency](#absolute-frequency)

An [absolute wavenumber](#absolute-wavenumber) is a complex [wavenumber](wave-equation.md#wavenumber) at the selected zero-[group velocity](wave-equation.md#group-velocity) saddle of a [dispersion relation](wave-equation.md#dispersion-relation). For the [linear complex Ginzburg-Landau equation](partial-differential-equation.md#linear-complex-ginzburg-landau-equation), $k_0=-U/[2(c_d-i)]$; the positive real part of the diffusion coefficient makes the Gaussian saddle accessible from the real Fourier contour.

## Orr-Sommerfeld equation

↑ **Parent:** [Hydrodynamic stability](hydrodynamic-stability.md)

The Orr-Sommerfeld equation governs the wall-normal velocity of [normal mode](wave-equation.md#normal-mode) disturbances to an incompressible viscous parallel [shear flow](fluid-mechanics.md#shear-flow). Here $D=d/dy$, $\kappa^2=\alpha^2+\beta^2$, and $Re$ is the [Reynolds number](fluid-mechanics.md#reynolds-number). It follows by eliminating pressure from the linearized [Navier-Stokes equations](viscous-fluid-flow.md#navier-stokes-equation). At a rigid no-slip wall, $\widehat v=D\widehat v=0$. In the inviscid limit it reduces to the [Rayleigh equation for inviscid shear flow](#rayleigh-equation-for-inviscid-shear-flow).

<h3 id="squire-s-theorem">Squire's theorem</h3>

↑ **Parent:** [Orr-Sommerfeld equation](#orr-sommerfeld-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Squire's_theorem)

For temporal normal-mode stability of a viscous parallel shear flow, any unstable three-dimensional mode maps by the [Squire transformation](#squire-transformation) to an unstable two-dimensional mode at a no larger [Reynolds number](fluid-mechanics.md#reynolds-number). Hence the first temporal modal instability occurs among two-dimensional disturbances. The theorem does not exclude three-dimensional [transient growth](linear-operator-theory.md#transient-growth) or forced responses.

#### Squire transformation

↑ **Parent:** [Squire's theorem](#squire-s-theorem)

For positive streamwise [wavenumber](wave-equation.md#wavenumber) $k$, replace a three-dimensional [Orr-Sommerfeld equation](#orr-sommerfeld-equation) by a two-dimensional one with the displayed parameters. Both the transverse operator and the coefficient $1/(ikR)$ remain unchanged, preserving the eigenfunction and phase-speed [eigenvalue](linear-operator-theory.md#eigenvalue). This proves the modal comparison in [Squire's theorem](#squire-s-theorem).

### Airy reduction of the Orr-Sommerfeld equation in constant shear

↑ **Parent:** [Orr-Sommerfeld equation](#orr-sommerfeld-equation)

For nondimensional constant shear $U=y$ and streamwise wavenumber one, put $W=(D^2-1)\widehat v$. The [Orr-Sommerfeld equation](#orr-sommerfeld-equation) gives $W''=[1+iRe(y-c)]W$. The displayed substitution transforms it into the [Airy ordinary differential equation](differential-equation.md#airy-ordinary-differential-equation), because $(e^{i\pi/6})^3=i$. The scale $Re^{-1/3}$ balances shear advection against viscous diffusion.

#### Velocity reconstruction from the Orr-Sommerfeld vorticity

↑ **Parent:** [Airy reduction of the Orr-Sommerfeld equation in constant shear](#airy-reduction-of-the-orr-sommerfeld-equation-in-constant-shear)

The equation $(D^2-1)\widehat v=W$ is inverted by the displayed formula: differentiating twice produces the endpoint contribution $W(y)$, since $\sinh0=0$ and $(\sinh)'(0)=1$. If $W=a_1\operatorname{Ai}(Z)+a_2\operatorname{Bi}(Z)$, there are four independent constants $C_+,C_-,a_1,a_2$. This reconstructs the velocity from the [Airy reduction of the Orr-Sommerfeld equation in constant shear](#airy-reduction-of-the-orr-sommerfeld-equation-in-constant-shear); four no-slip and no-flux conditions determine the boundary eigenproblem.

### Squire equation

↑ **Parent:** [Orr-Sommerfeld equation](#orr-sommerfeld-equation)

The Squire equation governs wall-normal [vorticity](fluid-mechanics.md#vorticity) $\eta=\partial_zu-\partial_xw$ in the same [normal mode](wave-equation.md#normal-mode) convention as the [Orr-Sommerfeld equation](#orr-sommerfeld-equation). It follows by taking $\partial_z$ of the streamwise momentum equation minus $\partial_x$ of the spanwise momentum equation. At a rigid no-slip wall, $\widehat\eta=0$.

#### Squire mode

↑ **Parent:** [Squire equation](#squire-equation)

A Squire mode has zero wall-normal velocity and nonzero wall-normal [vorticity](fluid-mechanics.md#vorticity), satisfying the homogeneous [Squire equation](#squire-equation). For real base velocity, positive finite [Reynolds number](fluid-mechanics.md#reynolds-number), and zero boundary terms,

$$
\operatorname{Im}\omega=-\frac{\int(|\widehat\eta'|^2+\kappa^2|\widehat\eta|^2)\,dy}{Re\int|\widehat\eta|^2\,dy}<0
$$

for a nontrivial mode in a finite channel with no-slip walls. This follows by multiplying the homogeneous equation by $\overline\eta$, integrating by parts and taking the real part. Such modes are damped even when the coupled velocity-vorticity system can exhibit [transient growth from non-normal modes](#transient-growth-from-non-normal-modes).

##### Dissipation identity for a homogeneous Squire mode

↑ **Parent:** [Squire mode](#squire-mode)

For real base-flow velocity and positive [Reynolds number](fluid-mechanics.md#reynolds-number), multiply the homogeneous [Squire equation](#squire-equation) by the conjugate mode and integrate with zero endpoint values. Taking real parts gives the displayed negative temporal [growth rate](wave-equation.md#growth-rate). This proves decay of homogeneous Squire modes; the coupled shear-flow system can still be unstable or show [transient growth](linear-operator-theory.md#transient-growth) because wall-normal velocity can force the Squire variable.

### Orr-Sommerfeld mode

↑ **Parent:** [Orr-Sommerfeld equation](#orr-sommerfeld-equation)

An Orr-Sommerfeld mode has nonzero wall-normal velocity satisfying the [Orr-Sommerfeld equation](#orr-sommerfeld-equation). Its wall-normal vorticity satisfies the accompanying forced [Squire equation](#squire-equation). The triangular coupling separates the velocity eigenproblem from the vorticity forcing; the vorticity need not vanish in three dimensions.

## Inertial instability

↑ **Parent:** [Hydrodynamic stability](hydrodynamic-stability.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inertial_instability)

Inertial instability occurs when displaced fluid parcels amplify their displacement by conserving absolute momentum in a rotating flow. For a uniformly stratified basic state on an [f-plane](geophysical-fluid-dynamics.md#f-plane), a necessary condition is that the [Ertel potential vorticity](geophysical-fluid-dynamics.md#ertel-potential-vorticity) have the opposite sign to the [Coriolis parameter](geophysical-fluid-dynamics.md#coriolis-parameter).

## Rayleigh equation for inviscid shear flow

↑ **Parent:** [Hydrodynamic stability](hydrodynamic-stability.md)

For a parallel inviscid base flow $U(z)$ and disturbance streamfunction $\phi(z)e^{i\alpha(x-ct)}$, the Rayleigh equation is

$$
(U-c)(\phi''-\alpha^2\phi)-U''\phi=0.
$$

### Inviscid instability of a piecewise-linear mixing layer

↑ **Parent:** [Rayleigh equation for inviscid shear flow](#rayleigh-equation-for-inviscid-shear-flow)

For $U=-1$ below $z=-1$, $U=z$ between $z=-1$ and $z=1$, and $U=1$ above $z=1$, decaying [normal modes](wave-equation.md#normal-mode) solve $\phi''-k^2\phi=0$ in each region. [Pressure matching at a piecewise-linear shear interface](#pressure-matching-at-a-piecewise-linear-shear-interface) gives continuity of $\phi$ and $(U-c)\phi'-U'\phi$. The two corner conditions yield the displayed [dispersion relation](wave-equation.md#dispersion-relation). At $k=1/2$ the wave speeds are $c=\pm i/e$, so one mode grows exponentially with rate $1/(2e)$.

### Axisymmetric inviscid pipe stability equation

↑ **Parent:** [Rayleigh equation for inviscid shear flow](#rayleigh-equation-for-inviscid-shear-flow)

An axisymmetric [Stokes streamfunction](fluid-mechanics.md#stokes-streamfunction) disturbance $\phi(r)e^{ik(z-ct)}$ of an axial basic flow obeys the displayed [ordinary differential equation](differential-equation.md#ordinary-differential-equation). Regularity requires $\phi=O(r^2)$ at the axis, and an impermeable wall requires $\phi(a)=0$ for nonzero $k$. Multiplication by $\phi^*/r$ and [integration by parts](calculus.md#integration-by-parts) shows that a growing real-wavenumber mode requires $(U'/r)'$ to change sign; if it vanishes identically, the positive energy integral rules out such a mode. The condition concerns this cylindrical vorticity gradient rather than $U''$ alone.

#### Evanescent potential modes of inviscid Poiseuille flow

↑ **Parent:** [Axisymmetric inviscid pipe stability equation](#axisymmetric-inviscid-pipe-stability-equation)

When $U'/r$ is constant and $U\ne c$, the [axisymmetric inviscid pipe stability equation](#axisymmetric-inviscid-pipe-stability-equation) reduces to $\phi''-\phi'/r-k^2\phi=0$. Axis regularity selects $rI_1(kr)$ and impermeability gives $I_1(ka)=0$. These imaginary-wavenumber disturbances are spatially evanescent potential fields, not bounded whole-pipe temporal normal modes; their radial equation supplies no eigenvalue condition on $c$.

### Inviscid instability of a triangular jet

↑ **Parent:** [Rayleigh equation for inviscid shear flow](#rayleigh-equation-for-inviscid-shear-flow)

Decaying [normal modes](wave-equation.md#normal-mode) of this continuous piecewise-linear profile satisfy $\phi''-k^2\phi=0$ between the corners. [Pressure matching at a piecewise-linear shear interface](#pressure-matching-at-a-piecewise-linear-shear-interface) yields an odd [varicose mode of a planar jet](fluid-mechanics.md#varicose-mode-of-a-planar-jet) with real speed $c=(1-e^{-2k})/(2k)$ and an even [sinuous mode of a planar jet](fluid-mechanics.md#sinuous-mode-of-a-planar-jet) whose speeds satisfy

$$
2k^2c^2+k(1-2k-e^{-2k})c-[1-k-(1+k)e^{-2k}]=0.
$$

Its reduced [discriminant](polynomial.md#discriminant) factors as $(2k-3-e^{-2k}-4e^{-k})(2k-3-e^{-2k}+4e^{-k})$. The second factor is positive for $k>0$, while the first is strictly increasing and crosses zero once. Thus exactly the long-wave even branch is exponentially unstable, for $0<k<k_c$, where $2k_c-3-e^{-2k_c}-4e^{-k_c}=0$.

### Pressure matching at a piecewise-linear shear interface

↑ **Parent:** [Rayleigh equation for inviscid shear flow](#rayleigh-equation-for-inviscid-shear-flow)

For a [normal mode](wave-equation.md#normal-mode) of an inviscid parallel flow, the perturbation [pressure](thermodynamics.md#pressure) is $p=-(U-c)\phi'+U'\phi$. At an interface where $U$ is continuous but $U'$ jumps, continuity of normal velocity and [pressure](thermodynamics.md#pressure) gives continuity of $\phi$ and the displayed flux. Consequently $(U-c)[\phi']=[U']\phi$. A [sinuous mode of a planar jet](fluid-mechanics.md#sinuous-mode-of-a-planar-jet) may therefore have a cusp at a symmetric velocity-profile corner: even parity alone does not force its one-sided derivative to vanish.

<h3 id="fjortoft-theorem">Fjørtoft theorem</h3>

↑ **Parent:** [Rayleigh equation for inviscid shear flow](#rayleigh-equation-for-inviscid-shear-flow)

For a smooth inviscid parallel shear profile with an exponentially growing mode, let $U_s$ be its velocity at an inflection point. The real and imaginary parts of the integrated [Rayleigh equation for inviscid shear flow](#rayleigh-equation-for-inviscid-shear-flow) imply $\int U''(U-U_s)|\psi|^2/|U-c|^2=-\int(|\psi'|^2+k^2|\psi|^2)<0$. Consequently $U''(U-U_s)<0$ somewhere in the channel. This strengthens [Rayleigh's inflection-point theorem](#rayleigh-s-inflection-point-theorem) but is still only a necessary condition, not a sufficient instability criterion.

### Inviscid Couette continuous spectrum

↑ **Parent:** [Rayleigh equation for inviscid shear flow](#rayleigh-equation-for-inviscid-shear-flow)

For inviscid plane [Couette flow](viscous-fluid-flow.md#couette-flow) $U=z$ between impermeable walls at $z=\pm1$, the nonzero real streamwise [wavenumber](wave-equation.md#wavenumber) $\alpha$ gives no nontrivial smooth discrete vertical-velocity modes. Instead, the vorticity variable $q=(D^2-\alpha^2)w$ obeys $(\partial_t+i\alpha z)q=0$. Localized [vorticity sheets](fluid-mechanics.md#vortex-sheet) give [generalized eigenfunctions](linear-operator-theory.md#generalized-eigenfunction) with real frequencies $\omega_\xi=\alpha\xi$. Their closure forms a neutral [continuous spectrum](linear-operator-theory.md#continuous-spectrum).

#### Inviscid Couette initial-value Green function

↑ **Parent:** [Inviscid Couette continuous spectrum](#inviscid-couette-continuous-spectrum)

For constant shear $U=\lambda y$, the wall-normal Laplacian of velocity is advected with phase $e^{-i\alpha\lambda yt}$. Inverting $D^2-k^2$, $k^2=\alpha^2+\beta^2$, with its [Dirichlet Green function](analysis.md#dirichlet-green-function) gives the displayed initial-value solution. Impermeable inviscid walls impose zero normal velocity, not zero tangential velocity or no-slip wall vorticity.

#### Linear inviscid damping in unbounded Couette flow

↑ **Parent:** [Inviscid Couette continuous spectrum](#inviscid-couette-continuous-spectrum)

In unbounded [Couette flow](viscous-fluid-flow.md#couette-flow) with velocity $(y,0)$, linear [vorticity](fluid-mechanics.md#vorticity) is transported exactly as $\omega(x,y,t)=\omega_0(x-yt,y)$. For a nonzero streamwise [Fourier mode](fourier-analysis.md#fourier-mode) $\alpha$ and sufficiently localized smooth initial data, inversion by the [one-dimensional modified Helmholtz Green function](analysis.md#one-dimensional-modified-helmholtz-green-function) gives the displayed pointwise decay of the [streamfunction](fluid-mechanics.md#stream-function) and [velocity](classical-mechanics.md#velocity), although [vorticity](fluid-mechanics.md#vorticity) does not decay in magnitude. The mechanism is phase mixing: shearing produces increasingly rapid transverse oscillations, whose elliptic velocity reconstruction suppresses them. Smoothness and decay of the initial [streamfunction](fluid-mechanics.md#stream-function) without derivative control do not alone imply these algebraic rates.

#### Vorticity-sheet eigenfunction of inviscid Couette flow

↑ **Parent:** [Inviscid Couette continuous spectrum](#inviscid-couette-continuous-spectrum)

Let $G_a$ be the [Dirichlet Green function](analysis.md#dirichlet-green-function) of $D^2-a^2$ on $[-1,1]$, with $a=|\alpha|$:

$$
G_a(z,\xi)=-\frac{\sinh[a(z_<+1)]\sinh[a(1-z_>)]}{a\sinh(2a)}.
$$

It is continuous and has derivative jump one, so $(D^2-a^2)G_a=\delta(z-\xi)$. The [Dirac delta multiplication identity](distribution-theory.md#dirac-delta-multiplication-identity) gives $(z-\xi)\delta(z-\xi)=0$, proving it is a [generalized eigenfunction](linear-operator-theory.md#generalized-eigenfunction) of the [inviscid Couette continuous spectrum](#inviscid-couette-continuous-spectrum). Integrating $G_a(z,\xi)q_0(\xi)e^{-i\alpha\xi t}$ reconstructs the evolving vertical [velocity](classical-mechanics.md#velocity) from its initial vorticity.

### Vorticity-jump matching for an inviscid shear flow

↑ **Parent:** [Rayleigh equation for inviscid shear flow](#rayleigh-equation-for-inviscid-shear-flow)

Across a jump of $U'$ in a constant-density parallel flow with continuous $U$, the [normal mode](wave-equation.md#normal-mode) vertical velocity and pressure are continuous. The linearized momentum equation gives $\widehat p=\rho[(U-c)\widehat w'-U'\widehat w]/(ik)$, yielding the displayed conditions. Equivalently, away from $U=c$, $(U-c)[\widehat w']=[U']\widehat w$. Derivative continuity is generally incorrect when the background [vorticity](fluid-mechanics.md#vorticity) jumps. This is the constant-density, continuous-velocity specialization of [jump conditions for stratified inviscid shear flow](gravity-wave.md#jump-conditions-for-stratified-inviscid-shear-flow).

### Inviscid parallel shear flow

↑ **Parent:** [Rayleigh equation for inviscid shear flow](#rayleigh-equation-for-inviscid-shear-flow)

An inviscid parallel shear flow has base velocity $\mathbf u=U(y)\mathbf e_x$. Two-dimensional normal-mode perturbations satisfy the [Rayleigh equation for inviscid shear flow](#rayleigh-equation-for-inviscid-shear-flow).

#### Unbounded piecewise-linear shear layer

↑ **Parent:** [Inviscid parallel shear flow](#inviscid-parallel-shear-flow)

A uniform-density inviscid [shear flow](fluid-mechanics.md#shear-flow) with $U=U_0z/d$ for $|z|<d$ and $U=\pm U_0$ outside has two [vorticity](fluid-mechanics.md#vorticity) jumps but no walls. Decaying [normal modes](wave-equation.md#normal-mode) satisfy $w''-k^2w=0$ in each region. Continuity of $w$ and [pressure matching at a piecewise-linear shear interface](#pressure-matching-at-a-piecewise-linear-shear-interface) gives a two-by-two determinant whose diagonal entries are $1-2kd\pm2kd\,c/U_0$ and off-diagonal entries $e^{-2kd}$. Its vanishing gives the displayed [dispersion relation](wave-equation.md#dispersion-relation). The [Kelvin-Helmholtz instability](fluid-mechanics.md#kelvin-helmholtz-instability) band is $0<kd<\alpha_s$, where $2\alpha_s-1=e^{-2\alpha_s}$ has its unique positive root above $1/2$, approximately $0.63923227$. Short waves decouple the two edges and remain neutral; long waves approach the [vortex sheet](fluid-mechanics.md#vortex-sheet) instability with $c=\pm iU_0$.

#### Three-layer stratified piecewise-linear shear flow

↑ **Parent:** [Inviscid parallel shear flow](#inviscid-parallel-shear-flow)

This three-layer [shear flow](fluid-mechanics.md#shear-flow) has $U=\Delta Uz/h$ and density $\rho_0$ between $z=\pm h/2$. Above and below, the [velocity](classical-mechanics.md#velocity) is the corresponding constant $\pm\Delta U/2$, and the [mass density](fluid-mechanics.md#density) is $\rho_0\mp\Delta\rho/2$. The density drops and [vorticity](fluid-mechanics.md#vorticity) jumps coincide at both interfaces. Its [hydrodynamic stability](hydrodynamic-stability.md) involves coupled [gravity-vorticity interface waves](gravity-wave.md#gravity-vorticity-interface-wave), unlike a profile with uniform shear extending through all three layers.

##### Quartic dispersion relation for a three-layer stratified shear flow

↑ **Parent:** [Three-layer stratified piecewise-linear shear flow](#three-layer-stratified-piecewise-linear-shear-flow)

For the bounded-shear three-layer profile with density contrasts minus one, zero and plus one, the localized-mode matching determinant is $[a(1-c)^2-(1-c)-J][a(1+c)^2-(1+c)-J]-b^2(1-c^2)^2=0$, where $a=\alpha[1+\coth(2\alpha)]$ and $b=\alpha\operatorname{csch}(2\alpha)$. Dividing by $a^2-b^2=2\alpha a$ gives a quartic in $c$ and a quadratic in $c^2$. Its constant term is $\{[2\alpha-(1+J)]^2-e^{-4\alpha}(1+J)^2\}/(4\alpha^2)$, whose negative sign proves the [unstable band of a three-layer stratified shear flow](#unstable-band-of-a-three-layer-stratified-shear-flow).

##### Unstable band of a three-layer stratified shear flow

↑ **Parent:** [Three-layer stratified piecewise-linear shear flow](#three-layer-stratified-piecewise-linear-shear-flow)

For the [three-layer stratified piecewise-linear shear flow](#three-layer-stratified-piecewise-linear-shear-flow), set $\alpha=kh/2$. The [dispersion relation](wave-equation.md#dispersion-relation) is quadratic in squared nondimensional [phase velocity](wave-equation.md#phase-velocity). Its constant term is $[2\alpha-(1+J)(1+e^{-2\alpha})][2\alpha-(1+J)(1-e^{-2\alpha})]/(4\alpha^2)$. Throughout the displayed band this is negative, so one squared speed is negative and gives an exponentially growing [normal mode](wave-equation.md#normal-mode).

#### Hazel model

↑ **Parent:** [Inviscid parallel shear flow](#inviscid-parallel-shear-flow)

The [Hazel model](#hazel-model) is a smooth stratified [shear flow](fluid-mechanics.md#shear-flow) whose base [velocity](classical-mechanics.md#velocity) has a hyperbolic-tangent profile and whose squared [buoyancy frequency](gravity-wave.md#buoyancy-frequency) has a hyperbolic-secant-squared profile. The equal-width nondimensional example is $U=\tanh z$ and $N^2=J\operatorname{sech}^2z$. For $J\geq0$, its [gradient Richardson number](gravity-wave.md#gradient-richardson-number) is $J\cosh^2z$, with minimum $J$.

##### Neutral mode of the equal-width Hazel model

↑ **Parent:** [Hazel model](#hazel-model)

The zero-[phase velocity](wave-equation.md#phase-velocity) ansatz $w=(\operatorname{sech}z)^k(\tanh z)^{1-k}$ solves the [Taylor–Goldstein equation](gravity-wave.md#taylor-goldstein-equation) away from its [critical level of an internal gravity wave](gravity-wave.md#critical-level-of-an-internal-gravity-wave) exactly when $J=k(1-k)$. Let $y=\tanh z$ and $a=1-k$. Then $w'/w=a/y-y$ and $w''/w=a(a-1)/y^2-a-1+2y^2$, so the differential-equation residual divided by $w$ is $[J-k(1-k)](y^{-2}-1)$. The curve has maximum $1/4$ at $k=1/2$. The endpoint $k=0$ does not decay at infinity; fractional powers at the critical level require a branch and regularity qualification.

###### Critical-layer regularity of a neutral Hazel mode

↑ **Parent:** [Neutral mode of the equal-width Hazel model](#neutral-mode-of-the-equal-width-hazel-model)

For $0<k<1$, a [neutral mode of the equal-width Hazel model](#neutral-mode-of-the-equal-width-hazel-model) behaves as $w\sim z^{1-k}$ near $z=0$. Its [derivative](calculus.md#derivative) diverges as $z^{-k}$, so it is not a classical continuously differentiable mode across the [critical level of an internal gravity wave](gravity-wave.md#critical-level-of-an-internal-gravity-wave). The horizontal [velocity](classical-mechanics.md#velocity) is proportional to $w'/k$; its local [kinetic energy](classical-mechanics.md#kinetic-energy) is finite only for $k<1/2$, because $\int_0^\epsilon z^{-2k}\,dz$ converges precisely then. One possible neutral-mode convention is the boundary value from $U-c$ with $c_i\downarrow0$, which fixes the phase of the power on the negative-$z$ side. The [Miles–Howard theorem](gravity-wave.md#miles-howard-theorem) concerns growing modes with nonreal $c$ and does not rule out such singular neutral limits.

#### Bounded piecewise-linear shear layer

↑ **Parent:** [Inviscid parallel shear flow](#inviscid-parallel-shear-flow)

Let $\zeta=z/L\in[-1,1]$, $h=L_s/L\in(0,1)$, and normalize velocity by its maximum magnitude. The profile is $U=\zeta/h$ for $|\zeta|<h$ and $U=\operatorname{sgn}\zeta$ outside. Each region has exponential vertical-velocity modes; the two walls and [vorticity-jump matching for an inviscid shear flow](#vorticity-jump-matching-for-an-inviscid-shear-flow) determine their coupling. With $\alpha=kL$, $q=\alpha h$, $X=\tanh q$, $Y=\tanh[\alpha(1-h)]$, $H=q(1+XY)$ and $J=q(X+Y)$, elimination gives $c^2=(H-Y)(J-XY)/(HJ)$, with $c$ normalized by the velocity scale.

##### Instability threshold for a bounded piecewise-linear shear layer

↑ **Parent:** [Bounded piecewise-linear shear layer](#bounded-piecewise-linear-shear-layer)

The [bounded piecewise-linear shear layer](#bounded-piecewise-linear-shear-layer) has exponentially growing modes exactly when $h<1/2$. Its squared phase speed tends to $2h-1$ as $kL\to0$ and to $1$ as $kL\to\infty$. For $h<1/2$, sufficiently long nonzero waves are therefore unstable. Conversely $J-XY>0$, and for $h\ge1/2$, $q\ge\alpha(1-h)>Y$, so $H-Y>0$ for every positive wavenumber and $c^2>0$. This proves the threshold without assuming monotonicity of the dispersion curve.

<h3 id="rayleigh-s-inflection-point-theorem">Rayleigh's inflection-point theorem</h3>

↑ **Parent:** [Rayleigh equation for inviscid shear flow](#rayleigh-equation-for-inviscid-shear-flow)

An inviscid parallel shear flow can possess an exponentially growing normal mode only if $U''$ changes sign somewhere in the flow.

<h3 id="howard-s-semicircle-theorem">Howard's semicircle theorem</h3>

↑ **Parent:** [Rayleigh equation for inviscid shear flow](#rayleigh-equation-for-inviscid-shear-flow)

If an inviscid shear-flow mode has complex wave speed $c$ and $U_-\leq U\leq U_+$, then

$$
\left(\operatorname{Re}c-\frac{U_++U_-}{2}\right)^2
+(\operatorname{Im}c)^2
\leq\left(\frac{U_+-U_-}{2}\right)^2.
$$

<h4 id="weighted-identity-for-howard-s-semicircle-theorem">Weighted identity for Howard's semicircle theorem</h4>

↑ **Parent:** [Howard's semicircle theorem](#howard-s-semicircle-theorem)

For a nonreal regular [Rayleigh equation for inviscid shear flow](#rayleigh-equation-for-inviscid-shear-flow) mode vanishing at the walls, put $F=\widehat w/(U-c)$. The equation becomes $[(U-c)^2F']'-k^2(U-c)^2F=0$. Multiplication by $\overline F$ and [integration by parts](calculus.md#integration-by-parts) gives the displayed identity. With $Q=|F'|^2+k^2|F|^2$, its imaginary and real parts give $\int UQ=c_r\int Q$ and $\int U^2Q=|c|^2\int Q$. Since $(U-U_{\min})(U_{\max}-U)\ge0$, these imply [Howard's semicircle theorem](#howard-s-semicircle-theorem).

## Counterpropagating wave instability

↑ **Parent:** [Hydrodynamic stability](hydrodynamic-stability.md)

Waves travelling in opposite directions relative to their local background currents can share a laboratory [phase velocity](wave-equation.md#phase-velocity). Their interaction can then lock their phases and extract energy from the mean shear, producing growing disturbances. In a layered flow, the coupling is often exponentially weak when the interface separation exceeds the waves' decay length. A [dispersion relation for two density interfaces in uniform shear](gravity-wave.md#dispersion-relation-for-two-density-interfaces-in-uniform-shear) gives a simple explicit example.

### Counterpropagating wave resonance in a three-layer shear flow

↑ **Parent:** [Counterpropagating wave instability](#counterpropagating-wave-instability)

For stable density jumps in the [three-layer stratified piecewise-linear shear flow](#three-layer-stratified-piecewise-linear-shear-flow), the upper interface's intrinsically left-going [gravity-vorticity interface wave](gravity-wave.md#gravity-vorticity-interface-wave) and the lower interface's intrinsically right-going wave have opposite laboratory [phase velocities](wave-equation.md#phase-velocity). They coincide at zero when $1+J=2\alpha$. At large [wavenumber](wave-equation.md#wavenumber), interaction is of order $e^{-2\alpha}$ and the [unstable band of a three-layer stratified shear flow](#unstable-band-of-a-three-layer-stratified-shear-flow) has width $4\alpha e^{-2\alpha}+O(\alpha e^{-6\alpha})$ around this resonance.

## Transient growth from non-normal modes

↑ **Parent:** [Hydrodynamic stability](hydrodynamic-stability.md)

Individually decaying nonorthogonal modes can interfere constructively and produce temporary energy growth. This mechanism is absent for an orthogonal eigenbasis of a normal evolution operator.

### Orr mechanism

↑ **Parent:** [Transient growth from non-normal modes](#transient-growth-from-non-normal-modes)

The Orr mechanism amplifies a leading two-dimensional shear disturbance as the background flow swings its wavefronts toward alignment. Conserved perturbation [vorticity](fluid-mechanics.md#vorticity) implies velocity [amplitude](physics.md#wave-amplitude) proportional to the inverse [wavevector](continuum-mechanics.md#wavevector) magnitude. This produces algebraic or transient [energy](classical-mechanics.md#energy) amplification without an exponentially growing [normal mode](wave-equation.md#normal-mode). [Viscosity](fluid-mechanics.md#dynamic-viscosity) limits the benefit of choosing an initially tightly wound disturbance.

// Target: gravitational-instability-of-an-astrophysical-disk.bigb

### Lift-up effect

↑ **Parent:** [Transient growth from non-normal modes](#transient-growth-from-non-normal-modes)

A streamwise-independent cross-stream disturbance in an inviscid parallel shear flow has time-independent wall-normal velocity. It advects the base streamwise momentum, producing the displayed linear growth of streamwise velocity and quadratic growth of perturbation kinetic energy. This is algebraic amplification, not an exponentially unstable [normal mode](wave-equation.md#normal-mode); it exemplifies [transient growth from non-normal modes](#transient-growth-from-non-normal-modes).

## Energy-stability threshold

↑ **Parent:** [Hydrodynamic stability](hydrodynamic-stability.md)

The energy-stability threshold is the parameter value below which a positive perturbation energy decreases monotonically for every disturbance. It can be lower than the linear instability threshold when non-normal transient growth is possible.

## Symmetric instability

↑ **Parent:** [Hydrodynamic stability](hydrodynamic-stability.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Symmetric_instability)

Symmetric instability occurs in rotating stratified flow when perturbations aligned with the basic current can extract energy from vertical shear. It is excluded when the Ertel potential vorticity has the stable sign; for constant gradients this gives a condition relating stratification, rotation, and horizontal buoyancy gradient.

## Eady model

↑ **Parent:** [Hydrodynamic stability](hydrodynamic-stability.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Eady_model)

The Eady model describes quasi-geostrophic baroclinic instability in a uniformly stratified layer with constant vertical shear, zero interior potential-vorticity gradient, and two rigid horizontal boundaries.

### Eady model with parallel sloping boundaries

↑ **Parent:** [Eady model](#eady-model)

When both rigid boundaries of a constant-shear [Eady model](#eady-model) have the same small slope $\alpha$, define $a=N^2\alpha/(f_0\Lambda)-1$, $M=N|k|D/|f_0|$ and $C=c/(\Lambda D)$. Zero-interior-PV modes have vertical structure $A\cosh(Mz/D)+B\sinh(Mz/D)$. The [boundary conditions](differential-equation.md#boundary-condition) $(z/D-C)\widehat\psi_{z/D}+a\widehat\psi=0$ at both endpoints give the displayed [dispersion relation](wave-equation.md#dispersion-relation). For $a\ge0$ its square root is real and there is no exponential [baroclinic instability](#baroclinic-instability). The same-sign boundary-pseudomomentum criterion is necessary, not sufficient.

### Boundary pseudomomentum of a sloping Eady layer

↑ **Parent:** [Eady model](#eady-model)

In a constant-shear [Eady model](#eady-model) with slopes $\alpha$ and $\gamma$, set $A_0=\Lambda-N^2\alpha/f_0$ and $A_D=\Lambda-N^2\gamma/f_0$. The interior [potential vorticity](geophysical-fluid-dynamics.md#potential-vorticity) obeys $(\partial_t+\Lambda z\partial_x)q'=0$. In the zero-interior-PV subspace, integrating $\psi'_xq'$ by parts and using the two [buoyancy](fluid-mechanics.md#buoyancy) boundary equations proves conservation of the displayed boundary [quadratic form](linear-algebra.md#quadratic-form). Opposite signs of $A_0,A_D$ make it definite and exclude growing [normal modes](wave-equation.md#normal-mode). For arbitrary nonzero interior PV, its derivative is $(N^2/f_0^3)\int\psi'_xq'\,dV$ and need not vanish. The restriction to zero interior PV is automatic for a growing smooth mode with complex [phase speed](wave-equation.md#phase-speed).

### Finite-depth Eady dispersion relation

↑ **Parent:** [Eady model](#eady-model)

For constant shear $U=\Lambda z$ between impermeable horizontal walls at $0,D$, with constant [buoyancy frequency](gravity-wave.md#buoyancy-frequency) and no interior [potential-vorticity gradient](geophysical-fluid-dynamics.md#potential-vorticity-gradient), define $m=NK/|f_0|$. The boundary conditions yield

$$
\left(c-\frac{\Lambda D}{2}\right)^2=\frac{\Lambda^2}{m^2}\left[\frac{(mD)^2}{4}-(mD)\coth(mD)+1\right].
$$

The bracket is negative for $0<mD<2.399\ldots$, giving [baroclinic instability](#baroclinic-instability) for nonzero zonal wavenumber. For large separation the boundary waves decouple; the lower-wave speed tends to $\Lambda/m$, matching the [dispersion relation of a semi-infinite Eady edge wave](#dispersion-relation-of-a-semi-infinite-eady-edge-wave).

### Semi-infinite Eady model

↑ **Parent:** [Eady model](#eady-model)

A uniformly stratified [quasi-geostrophic approximation](geophysical-fluid-dynamics.md#quasi-geostrophic-approximation) fluid with constant vertical shear occupies $z>0$, has a flat rigid lower wall, and has decaying perturbations aloft. On an [f-plane](geophysical-fluid-dynamics.md#f-plane), the basic interior [potential vorticity](geophysical-fluid-dynamics.md#potential-vorticity) is constant. Its smooth edge-wave modes have zero interior anomaly and propagate along the lower-boundary [buoyancy](fluid-mechanics.md#buoyancy) gradient. The absence of an upper wall removes the pair of interacting edge waves that makes the finite-depth [Eady model](#eady-model) unstable.

#### Absence of exponential instability in the semi-infinite Eady model

↑ **Parent:** [Semi-infinite Eady model](#semi-infinite-eady-model)

A growing complex phase speed cannot equal the real basic velocity. The linear interior [potential-vorticity equation](geophysical-fluid-dynamics.md#potential-vorticity-evolution-equation) then forces zero anomaly everywhere, decay fixes one exponential, and the wall fixes the real speed $c=\Lambda/m$. Thus there is no growing smooth decaying edge-wave eigenmode. This excludes exponential normal-mode instability without claiming that every initial disturbance lacks transient amplification or a singular neutral component.

#### Semi-infinite Eady edge wave

↑ **Parent:** [Semi-infinite Eady model](#semi-infinite-eady-model)

A lower-boundary [Eady edge wave](#eady-edge-wave) in the [semi-infinite Eady model](#semi-infinite-eady-model) has a smooth exponentially decaying vertical structure and a real frequency. It is supported by the horizontal boundary [buoyancy](fluid-mechanics.md#buoyancy) gradient while its interior [potential vorticity](geophysical-fluid-dynamics.md#potential-vorticity) anomaly vanishes. Its speed equals the basic velocity at one penetration depth.

##### Dispersion relation of a semi-infinite Eady edge wave

↑ **Parent:** [Semi-infinite Eady edge wave](#semi-infinite-eady-edge-wave)

For basic shear $U(z)=\Lambda z$ with a resting lower boundary, the [rigid-boundary buoyancy condition for quasi-geostrophic waves](geophysical-fluid-dynamics.md#rigid-boundary-buoyancy-condition-for-quasi-geostrophic-waves) and the decaying vertical exponential give

$$
c=\frac\Lambda m,\qquad \omega=kc,\qquad m=NK/|f_0|.
$$

This is real. The edge wave propagates in the same laboratory direction as the basic flow above its resting lower wall. If the basic buoyancy is $M^2y+N^2z$, then $\Lambda=-M^2/f_0$.

###### Steering height of a semi-infinite Eady edge wave

↑ **Parent:** [Dispersion relation of a semi-infinite Eady edge wave](#dispersion-relation-of-a-semi-infinite-eady-edge-wave)

The [critical level](#critical-level-of-a-shear-flow-wave) of the regular edge wave $c=\Lambda/m$, $U=\Lambda z$, is $z_c=1/m$ for $\Lambda\ne0$. At that height $U=c$, so mean advection and the phase term oppose in the wave frame. A literal condition $U=-c$ instead gives the unphysical height $-1/m$ below the lower wall.

##### Decaying vertical structure of a semi-infinite Eady edge wave

↑ **Parent:** [Semi-infinite Eady edge wave](#semi-infinite-eady-edge-wave)

A smooth zero-interior-[potential vorticity](geophysical-fluid-dynamics.md#potential-vorticity) mode has

$$
\widehat\psi''-m^2\widehat\psi=0,\qquad m=NK/|f_0|,\qquad K=\sqrt{k^2+l^2}.
$$

Decay for $z\to\infty$ gives $\widehat\psi=C e^{-mz}$. Its penetration depth $1/m$ increases with horizontal wavelength and decreases with [buoyancy frequency](gravity-wave.md#buoyancy-frequency). Singular neutral interior sheets are a distinct continuous-spectrum class.

### Eady model with a sloping lower boundary

↑ **Parent:** [Eady model](#eady-model)

A gently sloping lower boundary modifies the lower [Boundary Rossby wave](#boundary-rossby-wave) of the [Eady model](#eady-model), while a horizontal upper boundary retains the usual upper wave. With $M=N|k|D/|f_0|$, $a=\alpha N^2/(f_0\Lambda)$ and $C=c/(\Lambda D)$, the two-boundary dispersion relation is

$$
C^2-\left(1-a\frac{\coth M}{M}\right)C+(1-a)\left(\frac{\coth M}{M}-\frac1{M^2}\right)=0.
$$

For $a>1$ both speeds are real for every nonzero wavenumber. For every $a<1$ there is a band of exponentially growing modes; this includes negative slopes. The case $a=1$ has no exponential instability but can have a defective neutral mode at the crossing of the two uncoupled speeds.

#### Instability for negative slopes in the sloping-boundary Eady model

↑ **Parent:** [Eady model with a sloping lower boundary](#eady-model-with-a-sloping-lower-boundary)

The discriminant of the [Eady model with a sloping lower boundary](#eady-model-with-a-sloping-lower-boundary) is

$$
\Delta=\left[1-(2-a)\frac{\coth M}{M}\right]^2-4(1-a)\frac{\operatorname{csch}^2M}{M^2}.
$$

For any $a<1$, choose the unique $M>0$ satisfying $M\tanh M=2-a$. Then $\Delta<0$, proving existence of an unstable band even when $a<0$. For large negative $a$, resonance occurs at large $M$ and the exponentially weak boundary-wave coupling makes the unstable band narrow.

### Eady instability

↑ **Parent:** [Eady model](#eady-model)

Eady instability arises when counterpropagating Rossby waves localized on the upper and lower boundaries phase-lock and amplify one another.

### Boundary Rossby wave

↑ **Parent:** [Eady model](#eady-model)

A boundary Rossby wave is supported by a [buoyancy perturbation](fluid-mechanics.md#buoyancy-perturbation) or potential-temperature anomaly on a rigid horizontal boundary. Its intrinsic propagation depends on the boundary orientation and basic buoyancy gradient; the upper and lower boundary waves of the [Eady model](#eady-model) propagate oppositely relative to their local background flows.

#### Eady edge wave

↑ **Parent:** [Boundary Rossby wave](#boundary-rossby-wave)

For a semi-infinite fluid above a rigid horizontal boundary, constant [buoyancy frequency](gravity-wave.md#buoyancy-frequency) $N$, and [thermal wind](geophysical-fluid-dynamics.md#thermal-wind) $U=\Lambda z$, a zero-interior-[potential vorticity](geophysical-fluid-dynamics.md#potential-vorticity) perturbation has vertical dependence $e^{-\mu z}$, where $\mu=NK/|f_0|$ and $K=(k^2+l^2)^{1/2}$. Material conservation of boundary buoyancy gives $c\phi'(0)+\Lambda\phi(0)=0$. Thus its [phase velocity](wave-equation.md#phase-velocity) relative to the boundary flow is $c=\Lambda/\mu$. The wave's time dependence resides in its boundary condition; the interior field follows by potential-vorticity inversion. [MIT's Eady-edge-wave notes](https://ocw.mit.edu/courses/12-803-quasi-balanced-circulations-in-oceans-and-atmospheres-fall-2009/d6bf75cb60b05018230aefa5c315584d_MIT12_803F09_lec12.pdf) develop this boundary-wave interpretation.

##### Forced Eady edge wave

↑ **Parent:** [Eady edge wave](#eady-edge-wave)

With uniform [thermal wind](geophysical-fluid-dynamics.md#thermal-wind) $U=\Lambda z$ above a plane boundary, write the zero-interior-[potential vorticity](geophysical-fluid-dynamics.md#potential-vorticity) response as $\psi'=\operatorname{Re}\{Ae^{-\mu z+i(kx+ly)}\}$, where $\mu=N\sqrt{k^2+l^2}/f$ and $f>0$. Boundary vertical [velocity](classical-mechanics.md#velocity) $\epsilon\cos(kx+ly-\omega_0t)$ gives $C=N^2\epsilon/(f\mu)$ and natural [angular frequency](classical-mechanics.md#angular-frequency) $\omega=\Lambda k/\mu$. An initially zero response has $A=C(e^{-i\omega_0t}-e^{-i\omega t})/[i(\omega-\omega_0)]$. Its continuous resonant limit is $Ct e^{-i\omega t}$: forcing in phase with the boundary mode supplies [energy](classical-mechanics.md#energy) every cycle, and linear undamped theory predicts secular growth.

##### Sloping-boundary Eady edge wave

↑ **Parent:** [Eady edge wave](#eady-edge-wave)

For a semi-infinite stratified fluid with [thermal wind](geophysical-fluid-dynamics.md#thermal-wind) $U=\Lambda z$ above a gently sloping boundary $z=\alpha y$, a zero-interior-[potential vorticity](geophysical-fluid-dynamics.md#potential-vorticity) perturbation decays as $e^{-\mu z}$, where $\mu=N|k|/|f_0|$. The boundary [buoyancy perturbation](fluid-mechanics.md#buoyancy-perturbation) obeys a single oscillatory equation with [phase velocity](wave-equation.md#phase-velocity) $c=(\Lambda-\alpha N^2/f_0)/\mu$. The topographic and thermal-wind contributions cancel when the boundary follows a background [isopycnal](fluid-mechanics.md#isopycnal).

#### Quasi-geostrophic wave at a stratification interface

↑ **Parent:** [Boundary Rossby wave](#boundary-rossby-wave)

Two vertically unbounded regions with [buoyancy frequencies](gravity-wave.md#buoyancy-frequency) $N_1,N_2$ and [thermal wind](geophysical-fluid-dynamics.md#thermal-wind) shears $\Lambda_1,\Lambda_2$ support a localized wave if pressure and normal velocity are continuous at their common material interface. With decays $\phi_1=Ae^{\mu_1z}$ below and $\phi_2=Ae^{-\mu_2z}$ above, $\mu_j=N_jK/|f_0|$, matching gives

$$
c-U_I=\frac{\Lambda_2/N_2^2-\Lambda_1/N_1^2}{\mu_1/N_1^2+\mu_2/N_2^2}.
$$

When $N_1/N_2\to\infty$ with bounded shear, the lower layer becomes effectively rigid and the upper-layer [Eady edge wave](#eady-edge-wave) speed $\Lambda_2/\mu_2$ is recovered.

### Damped Eady-wave dispersion relation

↑ **Parent:** [Eady model](#eady-model)

Adding linear damping to one boundary of the Eady model makes the two boundary-wave phase speeds complex and can destabilize modes that were neutral without damping.

## Dissipation-induced instability

↑ **Parent:** [Hydrodynamic stability](hydrodynamic-stability.md)

Dissipation-induced instability occurs when damping one component of a coupled system moves an eigenvalue into the growing half-plane. Selective damping can alter the phase relation that previously stabilized two interacting waves or oscillators.

## Rayleigh discriminant

↑ **Parent:** [Hydrodynamic stability](hydrodynamic-stability.md)

For inviscid axisymmetric disturbances to a rotating flow, the Rayleigh discriminant measures the radial gradient of squared specific angular momentum.

<h3 id="rayleigh-s-circulation-criterion">Rayleigh's circulation criterion</h3>

↑ **Parent:** [Rayleigh discriminant](#rayleigh-discriminant)

An inviscid rotating flow is centrifugally stable to axisymmetric disturbances when $(r^2\Omega)^2$ is nondecreasing with radius. An outward decrease permits centrifugal instability.

## ↑ Ancestors (4)

1. [Fluid mechanics](fluid-mechanics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-331.md#3/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-331.md#3/c/ii/solution)
- [Three-layer stratified piecewise-linear shear flow](#three-layer-stratified-piecewise-linear-shear-flow)
- [Vertical velocity](fluid-mechanics.md#vertical-velocity)
