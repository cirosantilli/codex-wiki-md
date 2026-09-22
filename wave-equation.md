# Wave equation

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wave_equation)

The wave equation is a second-order [linear partial differential equation](partial-differential-equation.md#linear-partial-differential-equation) describing [waves](physics.md#wave) with [finite propagation speed](#finite-propagation-speed). In one spatial dimension its homogeneous, constant-coefficient form is

$$
u_{tt}=c^2u_{xx},\qquad c>0.
$$

Here $x$ is position, $t$ is time, $u(x,t)$ is the disturbance, and subscripts denote [partial derivatives](calculus.md#partial-derivative). For a [wave equation on a string](#wave-equation-on-a-string), $u$ is transverse displacement; in [linear acoustics](linear-acoustics.md), it can be a pressure perturbation. In several spatial dimensions, $u_{xx}$ becomes the [Laplacian](calculus.md#laplacian) $\Delta u$. The same mathematical structure connects vibrating strings and [acoustic waves](fluid-mechanics.md#acoustic-wave), although their physical assumptions and [wave speeds](#wave-speed) differ. [MIT, Wave Propagation, Chapter 1](https://ocw.mit.edu/courses/2-062j-wave-propagation-spring-2017/2f9f71f7f386b36c9c42f48c03aecfe6_MIT2_062J_S17_Chap1.pdf)

For the whole-line [Cauchy problem](partial-differential-equation.md#cauchy-problem), prescribe both displacement $u(x,0)=f(x)$ and [velocity](classical-mechanics.md#velocity) $u_t(x,0)=g(x)$. A [classical solution](partial-differential-equation.md#classical-solution) has continuous [partial derivatives](calculus.md#partial-derivative) through order two; $f\in C^2(\mathbb R)$ and $g\in C^1(\mathbb R)$ suffice for [D'Alembert's formula](#d-alembert-s-formula) to produce one. A finite string additionally needs [boundary conditions](differential-equation.md#boundary-condition). These statements concern the unforced model with constant $c$; [damping](#damping), spatially varying coefficients and nonlinear terms change the solution formula.

A [travelling wave](analysis.md#travelling-wave) $F(x-ct)$ carries its entire profile to the right at [wave speed](#wave-speed) $c$; $G(x+ct)$ travels left. Their sum is again a solution by the [superposition principle](vector-space.md#superposition-principle). A [standing wave](physics.md#standing-wave) instead has a fixed [mode shape](#mode-shape) whose size and sign oscillate: in $\sin(kx)\cos(ckt)$, each [node of a standing wave](#node-physics) stays stationary. The distinction is especially clear in the pulse and string diagrams below. For this ideal model, the [dispersion relation](#dispersion-relation) is $\omega^2=c^2k^2$: each propagation branch is [nondispersive](#nondispersive-wave), so a localized profile translates without spreading. This makes the equation a useful reference against which to understand [wave dispersion](#wave-dispersion) and [damping](#damping).

The appealing combination is local interaction with global predictability: neighbouring displacements determine [acceleration](classical-mechanics.md#acceleration) through $u_{xx}$, yet [D'Alembert's formula](#d-alembert-s-formula) explicitly identifies exactly which initial locations can influence a later observation. [Finite propagation speed](#finite-propagation-speed) turns that observation into a [domain of dependence](partial-differential-equation.md#domain-of-dependence), rather than requiring knowledge of the entire initial string.

**Table of contents**

- [Regular time-harmonic spherical wave](#regular-time-harmonic-spherical-wave)
- [Retarded acoustic Green function](#retarded-acoustic-green-function)
- [All-time boundedness of a wave equation with a reaction term](#all-time-boundedness-of-a-wave-equation-with-a-reaction-term)
- [Vector field method for wave equations](#vector-field-method-for-wave-equations)
  - [Commuted wave energy](#commuted-wave-energy)
  - [Klainerman-Sobolev inequality](#klainerman-sobolev-inequality)
  - [Commutation vector field for the wave equation](#commutation-vector-field-for-the-wave-equation)
    - [Scaling vector field](#scaling-vector-field)
    - [Lorentz boost vector field](#lorentz-boost-vector-field)
    - [Spatial rotation vector field](#spatial-rotation-vector-field)
    - [Spacetime translation vector field](#spacetime-translation-vector-field)
- [Wave energy](#wave-energy)
- [Reflected-step solution of the wave equation](#reflected-step-solution-of-the-wave-equation)
- [Wave speed](#wave-speed)
  - [Acoustic time-of-flight speed measurement](#acoustic-time-of-flight-speed-measurement)
    - [Timing calibration for acoustic speed measurements](#timing-calibration-for-acoustic-speed-measurements)
    - [Microphone](#microphone)
    - [Sampling rate](#sampling-rate)
  - [Slowness](#slowness)
- [Kirchhoff formula](#kirchhoff-formula)
  - [Method of descent for the wave equation](#method-of-descent-for-the-wave-equation)
  - [Strong Huygens principle](#strong-huygens-principle)
- [Finite propagation speed](#finite-propagation-speed)
  - [Causal cone for the constant-speed wave equation](#causal-cone-for-the-constant-speed-wave-equation)
  - [Support widening for the wave equation](#support-widening-for-the-wave-equation)
  - [Weak Huygens principle](#weak-huygens-principle)
  - [Shrinking cone energy argument](#shrinking-cone-energy-argument)
  - [Characteristic diamond for speed one minus y squared](#characteristic-diamond-for-speed-one-minus-y-squared)
- [Radiation field](#radiation-field)
  - [Scattering map](#scattering-map)
- [One-dimensional wave equation](#one-dimensional-wave-equation)
  - [Characteristic line for the one-dimensional wave equation](#characteristic-line-for-the-one-dimensional-wave-equation)
  - [Countertravelling decomposition of the one-dimensional wave equation](#countertravelling-decomposition-of-the-one-dimensional-wave-equation)
- [d'Alembert operator](#d-alembert-operator)
- [Semilinear wave equation](#semilinear-wave-equation)
  - [Wave map](#wave-map)
    - [Small data global regularity for wave maps](#small-data-global-regularity-for-wave-maps)
    - [Global regularity for one-dimensional wave maps](#global-regularity-for-one-dimensional-wave-maps)
    - [Stationary wave map](#stationary-wave-map)
    - [Wave map energy](#wave-map-energy)
      - [Wave map energy and criticality](#wave-map-energy-and-criticality)
    - [Wave map Cauchy data](#wave-map-cauchy-data)
  - [Null form for wave equations](#null-form-for-wave-equations)
    - [Classical null condition for wave equations](#classical-null-condition-for-wave-equations)
  - [Focusing semilinear wave equation](#focusing-semilinear-wave-equation)
    - [Localized ordinary differential equation blowup for a wave equation](#localized-ordinary-differential-equation-blowup-for-a-wave-equation)
  - [Smooth continuation criterion for semilinear wave equations](#smooth-continuation-criterion-for-semilinear-wave-equations)
  - [Almost global existence for wave equations](#almost-global-existence-for-wave-equations)
  - [Defocusing semilinear wave equation](#defocusing-semilinear-wave-equation)
    - [H2 bound for the defocusing cubic wave equation](#h2-bound-for-the-defocusing-cubic-wave-equation)
    - [Morawetz identity for the defocusing wave equation](#morawetz-identity-for-the-defocusing-wave-equation)
      - [Distributional bilaplacian of the radial coordinate in three dimensions](#distributional-bilaplacian-of-the-radial-coordinate-in-three-dimensions)
      - [Morawetz estimate for the defocusing wave equation](#morawetz-estimate-for-the-defocusing-wave-equation)
    - [Radial reduction of the three-dimensional wave equation](#radial-reduction-of-the-three-dimensional-wave-equation)
      - [Outgoing shell source estimate for a radial wave](#outgoing-shell-source-estimate-for-a-radial-wave)
      - [Outgoing-energy identity for a radial defocusing wave](#outgoing-energy-identity-for-a-radial-defocusing-wave)
  - [Local weak solution by contraction for a semilinear wave equation](#local-weak-solution-by-contraction-for-a-semilinear-wave-equation)
- [Elastic wave](#elastic-wave)
  - [Characteristic crossing in a boundary-generated elastic simple wave](#characteristic-crossing-in-a-boundary-generated-elastic-simple-wave)
  - [Elastic slowness surface](#elastic-slowness-surface)
    - [Vertical slowness sextic of an anisotropic solid](#vertical-slowness-sextic-of-an-anisotropic-solid)
    - [Elastic wave surface](#elastic-wave-surface)
      - [Slowness curvature and wave-surface cusps](#slowness-curvature-and-wave-surface-cusps)
    - [Elastic energy velocity](#elastic-energy-velocity)
      - [Elastic mode classification by vertical energy flux](#elastic-mode-classification-by-vertical-energy-flux)
        - [Free-surface anisotropic reflection amplitudes](#free-surface-anisotropic-reflection-amplitudes)
  - [Elastodynamic Green tensor](#elastodynamic-green-tensor)
    - [Far-field P and S radiation from a point force](#far-field-p-and-s-radiation-from-a-point-force)
    - [Elastodynamic surface-jump representation](#elastodynamic-surface-jump-representation)
    - [Point-moment elastodynamic displacement](#point-moment-elastodynamic-displacement)
  - [Seismic moment tensor](#seismic-moment-tensor)
    - [Explosion radiation in an isotropic elastic solid](#explosion-radiation-in-an-isotropic-elastic-solid)
    - [Double-couple fault source](#double-couple-fault-source)
      - [Double-couple radiation pattern](#double-couple-radiation-pattern)
    - [Tensile-crack seismic source](#tensile-crack-seismic-source)
      - [Tensile-crack radiation pattern](#tensile-crack-radiation-pattern)
  - [Energy uniqueness for traction-driven elasticity](#energy-uniqueness-for-traction-driven-elasticity)
    - [Elastic energy uniqueness with restoring boundary springs](#elastic-energy-uniqueness-with-restoring-boundary-springs)
  - [Seismic impedance](#seismic-impedance)
    - [Seismic layer transfer matrix](#seismic-layer-transfer-matrix)
      - [Periodic seismic multilayer stop band](#periodic-seismic-multilayer-stop-band)
    - [Flux-normalized elastic characteristic amplitudes](#flux-normalized-elastic-characteristic-amplitudes)
      - [Zero-frequency scattering through an elastic layer](#zero-frequency-scattering-through-an-elastic-layer)
  - [Love wave](#love-wave)
    - [Anisotropic Love-wave dispersion](#anisotropic-love-wave-dispersion)
    - [Rigid-base approximation to Love waves](#rigid-base-approximation-to-love-waves)
      - [Group-velocity minimum of a high-contrast Love wave](#group-velocity-minimum-of-a-high-contrast-love-wave)
    - [Love-wave cutoff frequencies](#love-wave-cutoff-frequencies)
    - [Love-wave interface reflection phase](#love-wave-interface-reflection-phase)
    - [Strict cutoff of the second Love-wave mode](#strict-cutoff-of-the-second-love-wave-mode)
  - [Rayleigh wave](#rayleigh-wave)
  - [Rigid elastic waveguide mode](#rigid-elastic-waveguide-mode)
    - [Ray asymptotics of a clamped elastic waveguide mode](#ray-asymptotics-of-a-clamped-elastic-waveguide-mode)
  - [Helmholtz separation of elastic waves](#helmholtz-separation-of-elastic-waves)
    - [P-SV displacement potentials](#p-sv-displacement-potentials)
  - [P wave](#p-wave)
    - [P-wavefront discontinuity transport](#p-wavefront-discontinuity-transport)
      - [Transmitted jump at a collimating solid-fluid interface](#transmitted-jump-at-a-collimating-solid-fluid-interface)
      - [Ray-tube conservation for a P-wave jump](#ray-tube-conservation-for-a-p-wave-jump)
    - [Reflection of a P-wave from a rigid plane](#reflection-of-a-p-wave-from-a-rigid-plane)
    - [Longitudinal polarization](#longitudinal-polarization)
  - [S wave](#s-wave)
    - [Transverse polarization](#transverse-polarization)
    - [SV-wave](#sv-wave)
    - [SH-wave](#sh-wave)
      - [SH ray-tube amplitude transport](#sh-ray-tube-amplitude-transport)
        - [Refraction of a cylindrical SH wavefront](#refraction-of-a-cylindrical-sh-wavefront)
      - [SH line-source near-field singularity](#sh-line-source-near-field-singularity)
      - [Guided SH modes between rigid and free planes](#guided-sh-modes-between-rigid-and-free-planes)
  - [Elastic-interface boundary conditions](#elastic-interface-boundary-conditions)
    - [P-SV mode conversion at a solid interface](#p-sv-mode-conversion-at-a-solid-interface)
    - [Snell law for elastic waves](#snell-law-for-elastic-waves)
  - [Acoustic reflection and transmission at an interface](#acoustic-reflection-and-transmission-at-an-interface)
    - [Lossless acoustic membrane scattering](#lossless-acoustic-membrane-scattering)
    - [Equal displacement-amplitude condition at an acoustic interface](#equal-displacement-amplitude-condition-at-an-acoustic-interface)
- [Damping](#damping)
  - [Critical damping](#critical-damping)
  - [Viscous damping](#viscous-damping)
    - [Damping ratio](#damping-ratio)
    - [Oscillator energy dissipation](#oscillator-energy-dissipation)
  - [Underdamping](#underdamping)
  - [Overdamping](#overdamping)
  - [Damping measurement from free decay](#damping-measurement-from-free-decay)
    - [Air track](#air-track)
    - [Ultrasonic motion sensor](#ultrasonic-motion-sensor)
    - [Logarithmic decrement](#logarithmic-decrement)
  - [Eddy-current damping](#eddy-current-damping)
- [Wave equation on a string](#wave-equation-on-a-string)
  - [Impulsively struck fixed-end string](#impulsively-struck-fixed-end-string)
  - [Modal energy of a localized velocity impulse on a string](#modal-energy-of-a-localized-velocity-impulse-on-a-string)
  - [Periodic reflection for a fixed-end string](#periodic-reflection-for-a-fixed-end-string)
  - [Linearly damped string](#linearly-damped-string)
    - [Velocity-impulse Green function for a damped string](#velocity-impulse-green-function-for-a-damped-string)
    - [Separated solution of the damped string equation](#separated-solution-of-the-damped-string-equation)
    - [Energy dissipation identity for a linearly damped string](#energy-dissipation-identity-for-a-linearly-damped-string)
- [Normal mode](#normal-mode)
  - [Mode shape](#mode-shape)
  - [Countability of elastic eigenfrequencies](#countability-of-elastic-eigenfrequencies)
  - [Eigenfrequency](#eigenfrequency)
  - [Modal energy distribution](#modal-energy-distribution)
  - [Normal-mode energy exchange](#normal-mode-energy-exchange)
  - [Node (physics)](#node-physics)
  - [Antinode](#antinode)
- [Fourier transform method for the wave equation](#fourier-transform-method-for-the-wave-equation)
  - [Low-frequency decomposition of the wave propagator](#low-frequency-decomposition-of-the-wave-propagator)
  - [Entire wave cosine multiplier](#entire-wave-cosine-multiplier)
- [D'Alembert's formula](#d-alembert-s-formula)
  - [Rectangular pulse splitting under the wave equation](#rectangular-pulse-splitting-under-the-wave-equation)
  - [D'Alembert formula with initial velocity](#d-alembert-formula-with-initial-velocity)
    - [Central zero region for odd compactly supported initial velocity](#central-zero-region-for-odd-compactly-supported-initial-velocity)
- [Wavenumber](#wavenumber)
  - [Spectroscopic wavenumber](#spectroscopic-wavenumber)
  - [Spatial sampling of a wave](#spatial-sampling-of-a-wave)
  - [Wavelength](#wavelength)
    - [Acoustic wavelength measurement](#acoustic-wavelength-measurement)
      - [Oscilloscope](#oscilloscope)
      - [Propagation of uncertainty](#propagation-of-uncertainty)
    - [Local wavelength](#local-wavelength)
- [Dispersion relation](#dispersion-relation)
  - [Spatial root of a dispersion relation](#spatial-root-of-a-dispersion-relation)
  - [Spatiotemporal wave-packet stability](#spatiotemporal-wave-packet-stability)
    - [Modulational instability](#modulational-instability)
      - [Benjamin-Feir instability](#benjamin-feir-instability)
      - [Focusing nonlinear Schrodinger modulation dispersion](#focusing-nonlinear-schrodinger-modulation-dispersion)
    - [Briggs-Bers criterion](#briggs-bers-criterion)
      - [Bounded temporal growth condition for cubic dispersion](#bounded-temporal-growth-condition-for-cubic-dispersion)
      - [Quartic impulse-response Laplace resolvent](#quartic-impulse-response-laplace-resolvent)
        - [Physical-sheet growth rate of a quartic impulse response](#physical-sheet-growth-rate-of-a-quartic-impulse-response)
      - [Spatial pinch point](#spatial-pinch-point)
        - [False complex saddle in dissipative cubic dispersion](#false-complex-saddle-in-dissipative-cubic-dispersion)
        - [False spatial saddle in quartic dispersion](#false-spatial-saddle-in-quartic-dispersion)
    - [Convective wave-packet instability](#convective-wave-packet-instability)
    - [Absolute wave-packet instability](#absolute-wave-packet-instability)
    - [Finite maximum temporal growth rate](#finite-maximum-temporal-growth-rate)
  - [Wave dispersion](#wave-dispersion)
    - [Nondispersive wave](#nondispersive-wave)
  - [Dispersion diagram](#dispersion-diagram)
  - [Ray tracing](#ray-tracing)
    - [Travel time](#travel-time)
    - [Elastic ray](#elastic-ray)
      - [Spherical elastic ray invariant](#spherical-elastic-ray-invariant)
        - [Herglotz–Wiechert inversion](#herglotz-wiechert-inversion)
          - [Hidden turning-ray zone from nonmonotone spherical slowness](#hidden-turning-ray-zone-from-nonmonotone-spherical-slowness)
        - [Core-reflected travel time](#core-reflected-travel-time)
      - [Hyperbolic interface collimation of P-waves](#hyperbolic-interface-collimation-of-p-waves)
    - [Hamiltonian ray equations for a local dispersion relation](#hamiltonian-ray-equations-for-a-local-dispersion-relation)
      - [Simple turning point of a variable-speed wave](#simple-turning-point-of-a-variable-speed-wave)
        - [Airy scaling at a variable-speed wave turning point](#airy-scaling-at-a-variable-speed-wave-turning-point)
          - [Decaying Airy continuation and ray reflection](#decaying-airy-continuation-and-ray-reflection)
          - [Turning-point enhancement of wave amplitude](#turning-point-enhancement-of-wave-amplitude)
    - [Stationary square-root-dispersion wake](#stationary-square-root-dispersion-wake)
  - [Growth rate](#growth-rate)
  - [Phase velocity and group velocity](#phase-velocity-and-group-velocity)
    - [Klein-Gordon packet velocities](#klein-gordon-packet-velocities)
    - [Phase-group orthogonality for degree-zero dispersion](#phase-group-orthogonality-for-degree-zero-dispersion)
    - [Phase velocity](#phase-velocity)
      - [Horizontal phase velocity](#horizontal-phase-velocity)
      - [Phase speed](#phase-speed)
    - [Group velocity](#group-velocity)
    - [Front velocity](#front-velocity)
    - [Information velocity](#information-velocity)
    - [Crest and trough](#crest-and-trough)
      - [Wave crest](#wave-crest)
      - [Wave trough](#wave-trough)
    - [Wave packet](#wave-packet)
      - [Envelope (waves)](#envelope-waves)
      - [Carrier wave](#carrier-wave)
      - [Gaussian envelope in a Klein-Gordon medium](#gaussian-envelope-in-a-klein-gordon-medium)
    - [Ninth-order dispersive advection equation](#ninth-order-dispersive-advection-equation)
- [Klein-Gordon equation](#klein-gordon-equation)
  - [Exponential initial-velocity tail for the Klein-Gordon equation](#exponential-initial-velocity-tail-for-the-klein-gordon-equation)
  - [Stationary-phase asymptotic of a Klein-Gordon wave along a subluminal ray](#stationary-phase-asymptotic-of-a-klein-gordon-wave-along-a-subluminal-ray)
    - [Upward zero crossings of an oscillatory stationary-phase tail](#upward-zero-crossings-of-an-oscillatory-stationary-phase-tail)

## Regular time-harmonic spherical wave

↑ **Parent:** [Wave equation](wave-equation.md)

For a [spherically symmetric function](calculus.md#spherically-symmetric-function), $v=ru$ reduces the radial [wave equation](wave-equation.md) to $v_{tt}=c^2v_{rr}$. A time-harmonic separated solution has radial numerator $C\sin(kr)+D\cos(kr)$, with $k=\omega/c$. Finiteness at the origin excludes $D$, and the prescribed finite origin value fixes $C$. This is a standing combination of incoming and outgoing waves. A purely outgoing point-source wave instead has a $1/r$ singularity and must be specified by its source strength, not by a finite value at the origin.

## Retarded acoustic Green function

↑ **Parent:** [Wave equation](wave-equation.md)

This is the causal three-dimensional fundamental solution of $\partial_t^2-c_0^2\nabla^2$. It concentrates on the outgoing sound cone and gives the retarded convolution of acoustic sources.

## All-time boundedness of a wave equation with a reaction term

↑ **Parent:** [Wave equation](wave-equation.md)

For $u_{tt}=\Delta u+\alpha u$ with a homogeneous [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition), let $\lambda_1>0$ be the first [Dirichlet Laplacian eigenvalue](partial-differential-equation.md#dirichlet-laplacian-eigenvalue). On a bounded one-dimensional interval, finite-energy displacement remains bounded for all time and all initial data exactly when $\alpha<\lambda_1$. The conserved energy $\tfrac12(\|u_t\|_2^2+\|\nabla u\|_2^2-\alpha\|u\|_2^2)$ controls the gradient and, by the [Poincaré inequality](sobolev-space.md#poincare-inequality) and one-dimensional integration, the maximum [norm](functional-analysis.md#norm). At equality a mode can grow linearly; above it a mode can grow exponentially. Bounded oscillations need not have a long-time limit.

## Vector field method for wave equations

↑ **Parent:** [Wave equation](wave-equation.md)

The vector field method commutes a [wave equation](wave-equation.md) with spacetime symmetry generators, estimates the resulting [commuted wave energies](#commuted-wave-energy), and converts weighted [L2 norms](real-analysis.md#l2-norm) to pointwise decay using a [Klainerman-Sobolev inequality](#klainerman-sobolev-inequality). The [commutation vector fields for the wave equation](#commutation-vector-field-for-the-wave-equation) include translations, rotations, [Lorentz boost vector fields](#lorentz-boost-vector-field) and the [scaling vector field](#scaling-vector-field). It is useful for [almost global existence for wave equations](#almost-global-existence-for-wave-equations) and for small-data global existence under the [classical null condition for wave equations](#classical-null-condition-for-wave-equations).

### Commuted wave energy

↑ **Parent:** [Vector field method for wave equations](#vector-field-method-for-wave-equations)

A commuted wave energy controls derivatives of a solution after applying the [commutation vector fields for the wave equation](#commutation-vector-field-for-the-wave-equation). A convenient equivalent norm is $A_m(t)=\sum_{|I|\leq m}\|\partial Z^Iu(t)\|_2$. The [wave energy estimate](partial-differential-equation.md#wave-energy-estimate) controls its growth through commuted sources, while the [Klainerman-Sobolev inequality](#klainerman-sobolev-inequality) gives pointwise decay for low-order derivatives.

### Klainerman-Sobolev inequality

↑ **Parent:** [Vector field method for wave equations](#vector-field-method-for-wave-equations)

In three spatial dimensions, with $Z$ the eleven translations, spatial rotations, boosts and scaling [commutation vector fields for the wave equation](#commutation-vector-field-for-the-wave-equation), a sufficiently decaying [smooth function](analysis.md#smooth-function) satisfies $|u(t,x)|\leq C(1+t+|x|)^{-1}(1+|t-|x||)^{-1/2}\sum_{|I|\leq2}\|Z^Iu(t)\|_2$. This weighted [Sobolev inequality](sobolev-space.md#sobolev-inequality) converts control of [commuted wave energy](#commuted-wave-energy) into decay. It holds independently of any [wave equation](wave-equation.md) satisfied by $u$.

### Commutation vector field for the wave equation

↑ **Parent:** [Vector field method for wave equations](#vector-field-method-for-wave-equations)

A first-order [vector field](calculus.md#vector-field) $Z$ is a commutation field for the flat [wave equation](wave-equation.md) when $[\Box,Z]$ is zero or a controlled multiple of $\Box$. Translations, spatial rotations and [Lorentz boost vector fields](#lorentz-boost-vector-field) commute with $\Box$; the [scaling vector field](#scaling-vector-field) satisfies $[\Box,S]=2\Box$. Repeated commutation preserves the differential order of a [semilinear wave equation](#semilinear-wave-equation).

#### Scaling vector field

↑ **Parent:** [Commutation vector field for the wave equation](#commutation-vector-field-for-the-wave-equation)

The [vector field](calculus.md#vector-field) $S=t\partial_t+x\cdot\nabla$ generates simultaneous spacetime dilation. For the flat [d'Alembert operator](#d-alembert-operator), $[\Box,S]=2\Box$. Consequently it commutes with the homogeneous [wave equation](wave-equation.md) at the level of its solution set, although its operator [commutator](lie-algebra.md#commutator) is nonzero.

#### Lorentz boost vector field

↑ **Parent:** [Commutation vector field for the wave equation](#commutation-vector-field-for-the-wave-equation)

For [Minkowski spacetime](special-relativity.md#minkowski-spacetime) with unit light speed, $L_i=t\partial_i+x_i\partial_t$ generates a [Lorentz boost](special-relativity.md#lorentz-boost). It commutes with the [d'Alembert operator](#d-alembert-operator) and controls derivatives transverse to time slices in the [vector field method for wave equations](#vector-field-method-for-wave-equations).

#### Spatial rotation vector field

↑ **Parent:** [Commutation vector field for the wave equation](#commutation-vector-field-for-the-wave-equation)

The [vector field](calculus.md#vector-field) $\Omega_{ij}=x_i\partial_j-x_j\partial_i$ is an infinitesimal spatial rotation. It commutes with the flat [d'Alembert operator](#d-alembert-operator) and supplies angular derivatives in the [Klainerman-Sobolev inequality](#klainerman-sobolev-inequality).

#### Spacetime translation vector field

↑ **Parent:** [Commutation vector field for the wave equation](#commutation-vector-field-for-the-wave-equation)

The [vector fields](calculus.md#vector-field) $\partial_t$ and $\partial_i$ generate time and space translations and commute with the flat [d'Alembert operator](#d-alembert-operator). They form the unweighted part of the [commutation vector fields for the wave equation](#commutation-vector-field-for-the-wave-equation).

## Wave energy

↑ **Parent:** [Wave equation](wave-equation.md)

For a real scalar [wave equation](wave-equation.md), the kinetic and gradient [energy](classical-mechanics.md#energy) is $E_{\mathrm{lin}}(t)=\frac12\int(|u_t|^2+|\nabla u|^2)\,dx$. A potential term is added for a [semilinear wave equation](#semilinear-wave-equation) $u_{tt}-\Delta u+V^{\prime}(u)=0$, giving the conserved [wave energy](#wave-energy) $E=E_{\mathrm{lin}}+\int V(u)\,dx$.

## Reflected-step solution of the wave equation

↑ **Parent:** [Wave equation](wave-equation.md)

For $y_{tt}=c^2y_{xx}$ on $0<x<L$, initially at rest with zero displacement, apply $y(0,t)=a$ for $t>0$ and keep $y(L,t)=0$. A [geometric series](real-analysis.md#geometric-series) in the [Laplace transform](analysis.md#laplace-transform) gives

$$
y(x,t)=a\sum_{m\geq0}\left[H\!\left(t-\frac{2mL+x}{c}\right)-H\!\left(t-\frac{(2m+2)L-x}{c}\right)\right].
$$

Here $H$ is the [Heaviside step function](analysis.md#heaviside-step-function), $L,c>0$, and only finitely many terms contribute at any finite time. The second step in each pair is a sign-reversed reflection from the fixed endpoint. The formula solves the [wave equation](wave-equation.md) classically away from the fronts and distributionally across them; the midpoint is a square wave of period $2L/c$.

## Wave speed

↑ **Parent:** [Wave equation](wave-equation.md)

For the homogeneous [one-dimensional wave equation](#one-dimensional-wave-equation) $u_{tt}=c^2u_{xx}$ with constant $c>0$, [wave speed](#wave-speed) means the speed at which a [travelling wave](analysis.md#travelling-wave) profile translates. In $F(x-ct)$, a feature initially at $x=s$ follows $x=s+ct$, giving signed [velocity](classical-mechanics.md#velocity) $+c$; in $G(x+ct)$ it follows $x=s-ct$, giving signed [velocity](classical-mechanics.md#velocity) $-c$. The [characteristic lines for the one-dimensional wave equation](#characteristic-line-for-the-one-dimensional-wave-equation) therefore have slopes $dx/dt=\pm c$. The speed of either profile is $c$, even though the [displacement](classical-mechanics.md#displacement) at a fixed point can change sign or pass through zero.[The 1-D Wave Equation](physics-bibliography.md#18-303-linear-partial-differential-equations-fall-2006-by-matthew-j-hancock/the-1-d-wave-equation)

The same $c$ bounds the [causal cone for the constant-speed wave equation](#causal-cone-for-the-constant-speed-wave-equation). For a [wave equation on a string](#wave-equation-on-a-string), $c=\sqrt{T/\mu}$ depends on [tension](classical-mechanics.md#tension) and [linear mass density](fluid-mechanics.md#linear-mass-density); for small [acoustic waves](fluid-mechanics.md#acoustic-wave) in stationary uniform air it is the [speed of sound](compressible-flow.md#speed-of-sound). This interpretation assumes the stated ideal [wave equation](wave-equation.md). In media with [wave dispersion](#wave-dispersion), [phase velocity](#phase-velocity), [group velocity](#group-velocity) and the earliest signal arrival have different meanings: a measured [wave crest](#wave-crest) speed need not be the speed of a [wave envelope](#envelope-waves), and neither alone establishes a [causal cone for the constant-speed wave equation](#causal-cone-for-the-constant-speed-wave-equation).

### Acoustic time-of-flight speed measurement

↑ **Parent:** [Wave speed](#wave-speed)

The experiment in [A time of flight method to measure the speed of sound using a stereo sound card by Carlos C. Carvalho and others](physics-bibliography.md#a-time-of-flight-method-to-measure-the-speed-of-sound-using-a-stereo-sound-card-by-carlos-c-carvalho-and-others) makes [wave speed](#wave-speed) visible as a delay. Two powered [microphones](#microphone) feed separate channels of one stereo line input. A clap beyond one end of their common axis reaches the nearer [microphone](#microphone) first. The displayed [signals](electrical-engineering.md#signal) show two separated onsets when enlarged; count their sample separation $N$ to obtain $\Delta t=N/f_s$ and infer [speed of sound](compressible-flow.md#speed-of-sound) $c=d/\Delta t$ from the measured [microphone](#microphone) spacing $d$. The reported [sampling rate](#sampling-rate) is $44100\,\mathrm{s^{-1}}$. Repeating at different spacings gives a distance-versus-delay plot whose slope estimates [speed of sound](compressible-flow.md#speed-of-sound); dependence on distance helps identify acoustic travel rather than a fixed electronic delay. These are the paper's apparatus and observed readout, not measurements made for this article.[A time of flight method to measure the speed of sound using a stereo sound card by Carlos C. Carvalho and others](physics-bibliography.md#a-time-of-flight-method-to-measure-the-speed-of-sound-using-a-stereo-sound-card-by-carlos-c-carvalho-and-others)

A controlled implementation also needs [timing calibration for acoustic speed measurements](#timing-calibration-for-acoustic-speed-measurements). Put the [microphones](#microphone) side by side to estimate the channel-delay offset $\tau_0$, swap channels to check its sign, and check the acquisition clock against an independent timing reference. Measure spacings between consistent points on the [microphones](#microphone), keep the source outside their span and on their axis, and fit $\Delta t=d/c+\tau_0$ by [linear regression](linear-regression.md) rather than forcing a zero intercept. Repeat pulses and compare the same onset criterion before reflections arrive. These are proposed calibration and control checks, not additional procedures claimed for the paper.

One sample corresponds to $1/f_s\simeq22.7\,\mathrm{\mu s}$ for the reported [sampling rate](#sampling-rate), so a delay of only a few samples has large relative [measurement error](probability-and-statistics.md#measurement-error). Background [measurement noise](probability-and-statistics.md#measurement-noise), different [microphone](#microphone) responses and threshold choice can move the apparent onset; reflections can supply a later competing pulse. Record [temperature](thermodynamics.md#temperature), keep air motion small, and compare several spacings. The result estimates [speed of sound](compressible-flow.md#speed-of-sound) under those conditions; it cannot prove an exactly zero precursor below the instrument's sensitivity or establish [finite propagation speed](#finite-propagation-speed) for every real medium. Both new diagrams in these sections show explicitly synthetic ideal [wave equation](wave-equation.md) solutions.[A time of flight method to measure the speed of sound using a stereo sound card by Carlos C. Carvalho and others](physics-bibliography.md#a-time-of-flight-method-to-measure-the-speed-of-sound-using-a-stereo-sound-card-by-carlos-c-carvalho-and-others)

#### Timing calibration for acoustic speed measurements

↑ **Parent:** [Acoustic time-of-flight speed measurement](#acoustic-time-of-flight-speed-measurement)

[Timing calibration for acoustic speed measurements](#timing-calibration-for-acoustic-speed-measurements) separates travel delay from the offset $\tau_0$ between acquisition channels and checks the clock defining the [sampling rate](#sampling-rate). A constant offset changes the intercept of a delay-versus-distance [linear regression](linear-regression.md); a clock-scale error changes the inferred [speed of sound](compressible-flow.md#speed-of-sound) itself.

#### Microphone

↑ **Parent:** [Acoustic time-of-flight speed measurement](#acoustic-time-of-flight-speed-measurement)

A microphone is an [acoustic transducer](physics.md#acoustic-transducer) that converts an [acoustic wave](fluid-mechanics.md#acoustic-wave) into an electrical [signal](electrical-engineering.md#signal). In an [acoustic time-of-flight speed measurement](#acoustic-time-of-flight-speed-measurement), its response affects which recorded feature is identified as arrival.

#### Sampling rate

↑ **Parent:** [Acoustic time-of-flight speed measurement](#acoustic-time-of-flight-speed-measurement)

The sampling rate is the number of recorded samples per unit [time](classical-mechanics.md#time-in-physics). A sample-index difference $N$ represents a delay $N/f_s$ when the acquisition clock is correctly calibrated.

### Slowness

↑ **Parent:** [Wave speed](#wave-speed)

[Slowness](#slowness) is the reciprocal of [phase velocity](#phase-velocity), measured in time per distance. A [plane wave](quantum-mechanics.md#plane-wave) with [wavevector](continuum-mechanics.md#wavevector) $\mathbf k$ and [angular frequency](classical-mechanics.md#angular-frequency) $\omega$ has vector [slowness](#slowness) $\mathbf p=\mathbf k/\omega$. Its direction is the [wavefront](optics.md#wavefront) normal, which need not be the [group velocity](#group-velocity) direction in an [anisotropic](continuum-mechanics.md#anisotropy) medium.

## Kirchhoff formula

↑ **Parent:** [Wave equation](wave-equation.md)

In three spatial dimensions, the solution with initial position $u_0$ and velocity $u_1$ is

$$
u(t,x)=\partial_t\bigl(tM_tu_0(x)\bigr)+tM_tu_1(x),
$$

where $M_t$ is the spherical mean.

### Method of descent for the wave equation

↑ **Parent:** [Kirchhoff formula](#kirchhoff-formula)

Extend lower-dimensional data independently of an extra coordinate and apply the higher-dimensional [wave equation](wave-equation.md) solution. Projecting a three-dimensional sphere to the planar disk yields the [kernel](linear-algebra.md#kernel-of-a-linear-map) $[2\pi\sqrt{t^2-r^2}]^{-1}$ for the two-dimensional solution with zero initial displacement. This [method of descent for the wave equation](#method-of-descent-for-the-wave-equation) explains why three-dimensional wave propagation can depend on a sphere while two-dimensional propagation depends on its interior.

### Strong Huygens principle

↑ **Parent:** [Kirchhoff formula](#kirchhoff-formula)

The strong Huygens principle says that the three-dimensional wave solution at $(t,x)$ depends only on initial data on the sphere $|y-x|=|t|$. A compactly supported disturbance therefore leaves no tail in the interior of its light cone.

## Finite propagation speed

↑ **Parent:** [Wave equation](wave-equation.md)

For the unforced, constant-$c$ [one-dimensional wave equation](#one-dimensional-wave-equation), [finite propagation speed](#finite-propagation-speed) says that changing [Cauchy data](partial-differential-equation.md#cauchy-data) outside $[x_*-ct_*,x_*+ct_*]$ cannot change the solution at $(x_*,t_*)$, where $c>0$ and $t_*\geq0$. This interval is the initial-data [domain of dependence](partial-differential-equation.md#domain-of-dependence). Its endpoints are found by following the two [characteristic lines for the one-dimensional wave equation](#characteristic-line-for-the-one-dimensional-wave-equation) backwards from the observation. [D'Alembert's formula](#d-alembert-s-formula) makes the dependence sharper: initial [displacement](classical-mechanics.md#displacement) is sampled at the endpoints, while initial [velocity](classical-mechanics.md#velocity) is integrated over the entire interval.[5 Wave Equation in R](physics-bibliography.md#math-220a-partial-differential-equations-of-applied-mathematics/5-wave-equation-in-r)

<a id="image-synthetic-constant-speed-spacetime-geometry-backward-dependence-and-widening-support"></a>
![](wave-equation-characteristic-causal-cones.png)

**[Figure 1](#image-synthetic-constant-speed-spacetime-geometry-backward-dependence-and-widening-support). Synthetic constant-speed spacetime geometry: backward dependence and widening support**.

For the synthetic choice $c=1$, $(x_*,t_*)=(0.5,1.5)$ has initial-data [domain of dependence](partial-differential-equation.md#domain-of-dependence) $[-1,2]$. A change confined near $x=3$ is irrelevant to that observation, however large it is. If both [Cauchy data](partial-differential-equation.md#cauchy-data) vanish outside $[-a,a]$, their [compact support](function.md#compact-support) can influence only $[-a-ct,a+ct]$ at $t\geq0$. Thus an observer at $x>a$ sees exactly zero [displacement](classical-mechanics.md#displacement) for $0\leq t<(x-a)/c$. There is no nonzero precursor beyond this [causal cone for the constant-speed wave equation](#causal-cone-for-the-constant-speed-wave-equation) in the ideal model. This is an exact statement about the [partial differential equation](partial-differential-equation.md), stronger than an experimental failure to detect a small [signal](electrical-engineering.md#signal).

[Support widening for the wave equation](#support-widening-for-the-wave-equation) is a bound on possible influence, not a claim that every point inside the expanding interval moves. A [bump function](analysis.md#bump-function) released with zero initial [velocity](classical-mechanics.md#velocity) splits into two separated [travelling waves](analysis.md#travelling-wave); the middle can become empty. An initial kick can instead leave an interior tail, as in the [D'Alembert formula with initial velocity](#d-alembert-formula-with-initial-velocity). Consequently [finite propagation speed](#finite-propagation-speed) does not imply the [Strong Huygens principle](#strong-huygens-principle). A finite string needs [boundary conditions](differential-equation.md#boundary-condition), and the whole-line formula applies locally only until its backward [causal cone for the constant-speed wave equation](#causal-cone-for-the-constant-speed-wave-equation) encounters an endpoint.

### Causal cone for the constant-speed wave equation

↑ **Parent:** [Finite propagation speed](#finite-propagation-speed)

For $c>0$, the backward causal cone at $(x_*,t_*)$ is

$$
\mathcal C^-_c(x_*,t_*)=\{(x,t):0\leq t\leq t_*,\ |x-x_*|\leq c(t_*-t)\}.
$$

Its boundaries are [characteristic lines for the one-dimensional wave equation](#characteristic-line-for-the-one-dimensional-wave-equation); its base on $t=0$ is the initial-data [domain of dependence](partial-differential-equation.md#domain-of-dependence). The forward cone from $(s,0)$ is $t\geq0$, $|x-s|\leq ct$. Here the cone is set by the model's [wave speed](#wave-speed), which may be acoustic or a string [wave speed](#wave-speed); it does not assert propagation at the [speed of light](special-relativity.md#speed-of-light).

### Support widening for the wave equation

↑ **Parent:** [Finite propagation speed](#finite-propagation-speed)

For whole-line [Cauchy data](partial-differential-equation.md#cauchy-data) with [support](function.md#support) contained in $[-a,a]$, the displayed inclusion holds at $t\geq0$. A short check uses [D'Alembert's formula](#d-alembert-s-formula): if $x>a+ct$, both sampled endpoints and the whole [interval](real-analysis.md#interval-mathematics) of [integration](calculus.md#integral) lie to the right of $a$, so all contributions vanish; the argument for $x<-a-ct$ is identical. The inclusion can be strict, and a nonzero response at the first permitted arrival is not guaranteed.

### Weak Huygens principle

↑ **Parent:** [Finite propagation speed](#finite-propagation-speed)

The [weak Huygens principle](#weak-huygens-principle) is the domain-of-dependence statement that initial data outside a backward light cone cannot influence its tip. It permits an interior tail and is weaker than the [Strong Huygens principle](#strong-huygens-principle). For $u_{tt}-\Delta u+V(x)u=0$ with $V\ge0$, integrating the local [energy](classical-mechanics.md#energy) over shrinking balls proves this statement: the boundary contribution is $u_t\partial_\nu u-\tfrac12(u_t^2+|\nabla u|^2+Vu^2)\le0$.

### Shrinking cone energy argument

↑ **Parent:** [Finite propagation speed](#finite-propagation-speed)

For the homogeneous speed-one [wave equation](wave-equation.md), integrate its [wave energy](#wave-energy) density over $B(x_*,T-t)$. The moving boundary contributes $-e$, while the usual flux contributes $u_t\partial_nu$. Their sum is $-\frac12(u_t-\partial_nu)^2-\frac12|\nabla_{\mathrm{tan}}u|^2\leq0$. Zero [Cauchy data](partial-differential-equation.md#cauchy-data) in the initial ball therefore force zero solution in its backward [light cone](special-relativity.md#light-cone).

### Characteristic diamond for speed one minus y squared

↑ **Parent:** [Finite propagation speed](#finite-propagation-speed)

For [Cauchy data](partial-differential-equation.md#cauchy-data) prescribed on $x=0$ over $|y|<a<1$, put $S=\operatorname{artanh}a$. The maximal region determined solely by those data is

$$
\left\{(x,y):|x|+|\operatorname{artanh}y|<S\right\}.
$$

In the [travel-time coordinate for a one-dimensional variable-speed wave equation](partial-differential-equation.md#travel-time-coordinate-for-a-one-dimensional-variable-speed-wave-equation) $(x,s)$ this is the ordinary characteristic diamond $|x|+|s|<S$, as follows from [finite propagation speed](#finite-propagation-speed).

## Radiation field

↑ **Parent:** [Wave equation](wave-equation.md)

A radiation field is the rescaled limit of a wave along null infinity. For a three-dimensional wave, the outgoing field is the limit of $ru(t,r\omega)$ with $t-r$ fixed, while the incoming field fixes $t+r$.

### Scattering map

↑ **Parent:** [Radiation field](#radiation-field)

A scattering map sends incoming asymptotic data to outgoing asymptotic data for the same solution.

## One-dimensional wave equation

↑ **Parent:** [Wave equation](wave-equation.md)

On the whole line, the homogeneous one-dimensional [wave equation](wave-equation.md) with constant [wave speed](#wave-speed) $c>0$ is

$$
u_{tt}-c^2u_{xx}=0,\qquad u(x,0)=f(x),\qquad u_t(x,0)=g(x).
$$

Here $u$ is [displacement](classical-mechanics.md#displacement) in the string interpretation; $f$ is initial [displacement](classical-mechanics.md#displacement) and $g$ is initial [velocity](classical-mechanics.md#velocity). Its two directions of travel give

$$
u(x,t)=F(x-ct)+G(x+ct)=\frac{f(x-ct)+f(x+ct)}2+\frac1{2c}\int_{x-ct}^{x+ct}g(s)\,ds.
$$

This is [D'Alembert's formula](#d-alembert-s-formula), including both [Cauchy data](partial-differential-equation.md#cauchy-data). The [countertravelling decomposition of the one-dimensional wave equation](#countertravelling-decomposition-of-the-one-dimensional-wave-equation) identifies $F(x-ct)$ as the right-moving [travelling wave](analysis.md#travelling-wave) and $G(x+ct)$ as the left-moving [travelling wave](analysis.md#travelling-wave). Their sum is permitted by the [superposition principle](vector-space.md#superposition-principle). For $f\in C^2$ and $g\in C^1$, it is a [classical solution](partial-differential-equation.md#classical-solution). More generally, [travelling waves](analysis.md#travelling-wave) with profiles $F$ and $G$ that are [locally integrable functions](distribution-theory.md#locally-integrable-function) solve the equation as [distributions](distribution-theory.md#distribution-mathematical-analysis), with derivatives interpreted distributionally.[The 1-D Wave Equation](physics-bibliography.md#18-303-linear-partial-differential-equations-fall-2006-by-matthew-j-hancock/the-1-d-wave-equation)

<a id="image-synthetic-pulse-solutions-release-from-rest-splits-a-profile-while-matched-initial-velocity-launches-it-rightward"></a>
![](wave-equation-countertravelling-pulse-components.png)

**[Figure 2](#image-synthetic-pulse-solutions-release-from-rest-splits-a-profile-while-matched-initial-velocity-launches-it-rightward). Synthetic pulse solutions: release from rest splits a profile, while matched initial velocity launches it rightward**.

The synthetic diagram uses the smooth [bump function](analysis.md#bump-function) $b$ defined in [D'Alembert's formula](#d-alembert-s-formula), with $f(x)=b(x)$ and $c=1$. Releasing this [displacement](classical-mechanics.md#displacement) from rest, $g=0$, gives $F=G=f/2$. Each emerging [travelling wave](analysis.md#travelling-wave) has half the original peak. Launching the identical initial [displacement](classical-mechanics.md#displacement) solely to the right instead requires $g=-cf'$ and gives $F=f$, $G=0$. At $t=1.5$, the released profiles have peaks $1/2$ at $x=\pm1.5$, while the launched profile has peak $1$ at $x=1.5$. These are calculated model values. A purely left-moving launch requires $g=cf'$. The initial [velocity](classical-mechanics.md#velocity) therefore selects the balance of directions; the initial shape alone does not.

### Characteristic line for the one-dimensional wave equation

↑ **Parent:** [One-dimensional wave equation](#one-dimensional-wave-equation)

These [characteristic curves](partial-differential-equation.md#characteristic-curve) are straight when [wave speed](#wave-speed) $c$ is constant. A right-moving component is constant on $x-ct=s$, and a left-moving component on $x+ct=s$. The full [superposition](vector-space.md#superposition-principle) generally is not constant on either family, because the other component can vary along it. Their backwards intersections with the initial line select the endpoints used in [D'Alembert's formula](#d-alembert-s-formula).

### Countertravelling decomposition of the one-dimensional wave equation

↑ **Parent:** [One-dimensional wave equation](#one-dimensional-wave-equation)

Let $H$ be any [antiderivative](calculus.md#antiderivative) of the initial [velocity](classical-mechanics.md#velocity), $H'=g$. One choice of profiles is

$$
F(s)=\frac{f(s)}2-\frac{H(s)}{2c},\qquad G(s)=\frac{f(s)}2+\frac{H(s)}{2c}.
$$

Opposite additive constants in $F$ and $G$ cancel, so the [displacement](classical-mechanics.md#displacement) is independent of the chosen [antiderivative](calculus.md#antiderivative). Even for [compact support](function.md#compact-support) of $g$, these separate profiles can approach nonzero constants; cancellation in their sum is essential to [support widening for the wave equation](#support-widening-for-the-wave-equation).

For a short derivation, the [characteristic coordinates](partial-differential-equation.md#characteristic-coordinate) $\xi=x-ct$, $\eta=x+ct$ give $u_{tt}-c^2u_{xx}=-4c^2u_{\xi\eta}$ by the [chain rule](calculus.md#chain-rule). Thus $u=F(\xi)+G(\eta)$, and the [Cauchy data](partial-differential-equation.md#cauchy-data) imply $F+G=f$ and $-cF'+cG'=g$, giving the profiles above.

<h2 id="d-alembert-operator">d'Alembert operator</h2>

↑ **Parent:** [Wave equation](wave-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/d'Alembert_operator)

The d'Alembert operator is the Lorentzian wave operator $\Box=\eta^{\mu\nu}\partial_\mu\partial_\nu$ in flat spacetime, or $\Box=\nabla^\mu\nabla_\mu$ on scalar fields in curved spacetime.

## Semilinear wave equation

↑ **Parent:** [Wave equation](wave-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Semilinear_wave_equation)

A semilinear wave equation has the form

$$
u_{tt}-\Delta u=F(u,\nabla u),
$$

so its highest-order part is linear while the forcing may depend nonlinearly on the solution and its lower derivatives.

### Wave map

↑ **Parent:** [Semilinear wave equation](#semilinear-wave-equation)

A wave map is a [harmonic map](differential-geometry.md#harmonic-map) with Lorentzian domain: a critical point of the action obtained by contracting the pullback target metric with the domain [Lorentzian metric](general-relativity.md#lorentzian-metric). For target [sphere](geometry-and-topology.md#sphere) $S^2$ in Euclidean space and $\Box=-\partial_t^2+\Delta$, its extrinsic equation is $\Box\phi=\phi(|\phi_t|^2-|\nabla\phi|^2)$, subject to $|\phi|=1$. The derivative contractions are [null forms for wave equations](#null-form-for-wave-equations). [Wave map Cauchy data](#wave-map-cauchy-data) must include a tangent initial velocity.

#### Small data global regularity for wave maps

↑ **Parent:** [Wave map](#wave-map)

Smooth compatible data sufficiently small in high weighted [Sobolev norms](sobolev-space.md#sobolev-norm) relative to a constant map produce global smooth [wave maps](#wave-map) in three and four spatial dimensions. In four dimensions, derivative decay $(1+t)^{-3/2}$ is time-integrable and closes [commuted wave energy](#commuted-wave-energy) estimates. In three dimensions the weaker $(1+t)^{-1}$ decay requires the cancellation of [null forms for wave equations](#null-form-for-wave-equations), exploited by the [vector field method for wave equations](#vector-field-method-for-wave-equations). These classical localized-data statements do not assert global regularity from small supercritical energy alone.

#### Global regularity for one-dimensional wave maps

↑ **Parent:** [Wave map](#wave-map)

For smooth localized compatible [wave map Cauchy data](#wave-map-cauchy-data) and compact Riemannian target, one-dimensional [wave maps](#wave-map) stay smooth globally. In null coordinates, the equation is $D_v\phi_u=D_u\phi_v=0$. Compatibility of the target metric with the [covariant derivative](general-relativity.md#covariant-derivative) makes $|\phi_u|^2$ independent of $v$ and $|\phi_v|^2$ independent of $u$. These transported derivative bounds and higher [energy estimates](partial-differential-equation.md#energy-estimate) prevent finite-time breakdown.

#### Stationary wave map

↑ **Parent:** [Wave map](#wave-map)

A time-independent [wave map](#wave-map) is a [harmonic map](differential-geometry.md#harmonic-map) of its spatial domain into the target. For target $S^2$, its equation is $\Delta Q+|\nabla Q|^2Q=0$. In two dimensions inverse [stereographic projection](complex-analysis.md#stereographic-projection) gives a smooth nonconstant example of finite [wave map energy](#wave-map-energy) $4\pi$.

#### Wave map energy

↑ **Parent:** [Wave map](#wave-map)

The conserved [energy](classical-mechanics.md#energy) of a [wave map](#wave-map) from Minkowski spacetime to a Riemannian target is $E=\frac12\int(|\phi_t|^2+|\nabla\phi|^2)\,dx$, with norms measured in the target metric. Contraction of the [wave map](#wave-map) equation with the velocity and [integration by parts](calculus.md#integration-by-parts) gives conservation.

##### Wave map energy and criticality

↑ **Parent:** [Wave map energy](#wave-map-energy)

Under $\phi_\lambda(t,x)=\phi(t/\lambda,x/\lambda)$, the conserved [wave map energy](#wave-map-energy) scales as $\lambda^{n-2}E$. Energy is subcritical for $n=1$, critical for $n=2$, and supercritical for $n\geq3$. The critical derivative index of the [homogeneous Sobolev space](sobolev-space.md#homogeneous-sobolev-space) is $s_c=n/2$. Small energy alone is not an appropriate general small-data regularity hypothesis in supercritical dimensions.

#### Wave map Cauchy data

↑ **Parent:** [Wave map](#wave-map)

Initial position $\phi_0$ for a [wave map](#wave-map) takes values in the target, and initial velocity $\phi_1$ belongs to its [tangent space](differential-geometry.md#tangent-space) at $\phi_0(x)$. For $S^2$ this means $|\phi_0|=1$ and $\phi_0\cdot\phi_1=0$. Localized data agree with a constant map and zero velocity outside a compact set; the map itself need not be a compactly supported ambient function.

### Null form for wave equations

↑ **Parent:** [Semilinear wave equation](#semilinear-wave-equation)

A quadratic derivative expression is a null form when its symbol vanishes on parallel [null covectors](general-relativity.md#null-covector). The Lorentz contraction $Q_0(f,g)=-f_tg_t+\nabla f\cdot\nabla g$ is the basic example. Its cancellation suppresses interactions of derivatives pointing along the same light ray. It is the algebraic structure behind the [classical null condition for wave equations](#classical-null-condition-for-wave-equations).

#### Classical null condition for wave equations

↑ **Parent:** [Null form for wave equations](#null-form-for-wave-equations)

For a quadratic derivative source $A^{\alpha\beta}\partial_\alpha u\partial_\beta u$, the classical null condition is $A^{\alpha\beta}\ell_\alpha\ell_\beta=0$ whenever $-\ell_0^2+|\ell_{\mathrm{sp}}|^2=0$. It removes the leading interaction of parallel lightlike derivatives. In three dimensions this structure gives global smooth solutions for sufficiently small, localized data through the [vector field method for wave equations](#vector-field-method-for-wave-equations). This PDE condition is distinct from the [null condition](special-relativity.md#null-condition) asserting that a single vector is lightlike.

### Focusing semilinear wave equation

↑ **Parent:** [Semilinear wave equation](#semilinear-wave-equation)

The focusing power [wave equation](wave-equation.md) is $u_{tt}-\Delta u=u|u|^{p-1}$. Its conserved [energy](classical-mechanics.md#energy) has the negative potential term $-|u|^{p+1}/(p+1)$ and is not positive definite. [Localized ordinary differential equation blowup for a wave equation](#localized-ordinary-differential-equation-blowup-for-a-wave-equation) produces smooth compactly supported data with finite maximal lifespan for suitable focusing powers.

#### Localized ordinary differential equation blowup for a wave equation

↑ **Parent:** [Focusing semilinear wave equation](#focusing-semilinear-wave-equation)

A spatially constant blowup profile for a [wave equation](wave-equation.md) solves an [ordinary differential equation](differential-equation.md#ordinary-differential-equation). Choose smooth compactly supported initial data which agree with the profile on a ball larger than its blowup time times the [wave speed](#wave-speed). [Finite propagation speed](#finite-propagation-speed) preserves agreement in an interior [light cone](special-relativity.md#light-cone), forcing finite-time breakdown of the localized solution. For $u_{tt}-\Delta u=u^3$, the profile $u(t)=\sqrt2/(1-t)$ is one example.

### Smooth continuation criterion for semilinear wave equations

↑ **Parent:** [Semilinear wave equation](#semilinear-wave-equation)

For a smooth [semilinear wave equation](#semilinear-wave-equation) whose nonlinearity is a smooth function of the solution and its first derivatives, local [Sobolev space](sobolev-space.md) theory gives a continuation criterion: a finite maximal existence time requires divergence of a sufficiently high solution norm. A bounded base norm $H^{s+1}\times H^s$, with $s>n/2$, allows restarting local existence. Higher regularity persists by differentiated [energy estimates](partial-differential-equation.md#energy-estimate). Precise norms can be weakened for particular nonlinearities.

### Almost global existence for wave equations

↑ **Parent:** [Semilinear wave equation](#semilinear-wave-equation)

Almost global existence means a lifespan which grows exponentially in the inverse size of small initial data, typically $T_\varepsilon\geq\exp(c/\varepsilon)-1$ for derivative-quadratic [semilinear wave equations](#semilinear-wave-equation) in three dimensions. [Commuted wave energy](#commuted-wave-energy) and the [Klainerman-Sobolev inequality](#klainerman-sobolev-inequality) lead to a logarithmic accumulation $\varepsilon\log(1+T)$ in a [bootstrap argument](partial-differential-equation.md#bootstrap-argument). This implies existence up to every fixed inverse power $\varepsilon^{-N}$ when the data are small enough depending on $N$.

### Defocusing semilinear wave equation

↑ **Parent:** [Semilinear wave equation](#semilinear-wave-equation)

The defocusing power-type wave equation has the conserved nonnegative energy

$$
E(u)=\int\left(\frac{|u_t|^2+|\nabla u|^2}{2}+\frac{|u|^{p+1}}{p+1}\right)dx.
$$

#### H2 bound for the defocusing cubic wave equation

↑ **Parent:** [Defocusing semilinear wave equation](#defocusing-semilinear-wave-equation)

For $u_{tt}-\Delta u+u^3=0$ in three spatial dimensions, conserved positive [wave energy](#wave-energy) $E$ controls $\|\nabla u\|_2$. The [Sobolev inequality](sobolev-space.md#sobolev-inequality) gives $\|u^2\nabla u\|_2\lesssim\|\nabla u\|_2^2\|D^2u\|_2\lesssim E\|D^2u\|_2$. Differentiated [wave energy estimates](partial-differential-equation.md#wave-energy-estimate) and the [Gronwall inequality](probability-and-statistics.md#gronwall-inequality) then give $\|u(t)\|_{\dot H^2}+\|u_t(t)\|_{\dot H^1}\leq C D e^{C E t}$, where $D$ bounds the corresponding initial [Sobolev norms](sobolev-space.md#sobolev-norm).

#### Morawetz identity for the defocusing wave equation

↑ **Parent:** [Defocusing semilinear wave equation](#defocusing-semilinear-wave-equation)

Multiplying a defocusing wave equation by $\nabla\psi\cdot\nabla u+(\Delta\psi)u/2$ and integrating by parts gives a weighted spacetime identity. For a radial solution and radial weight, its coercive terms are

$$
\psi''|\nabla u|^2-\frac14(\Delta^2\psi)u^2
+\frac{p-1}{2(p+1)}(\Delta\psi)|u|^{p+1}.
$$

##### Distributional bilaplacian of the radial coordinate in three dimensions

↑ **Parent:** [Morawetz identity for the defocusing wave equation](#morawetz-identity-for-the-defocusing-wave-equation)

In three dimensions, $\Delta|x|=2/|x|$ away from the origin and $-\Delta(1/|x|)=4\pi\delta_0$. Hence $-\Delta^2|x|=8\pi\delta_0$ as a distribution.

##### Morawetz estimate for the defocusing wave equation

↑ **Parent:** [Morawetz identity for the defocusing wave equation](#morawetz-identity-for-the-defocusing-wave-equation)

For a finite-energy defocusing power-wave solution in three dimensions,

$$
\int_0^\infty\int_{\mathbb R^3}\frac{|u(t,x)|^{p+1}}{|x|}\,dx\,dt
\lesssim E(u(0)).
$$

Hardy's inequality bounds the Morawetz action by the conserved energy.

#### Radial reduction of the three-dimensional wave equation

↑ **Parent:** [Defocusing semilinear wave equation](#defocusing-semilinear-wave-equation)

For a radial function $u(t,r)$ in three dimensions, setting $w=ru$ removes the radial first derivative because $r\Delta u=w_{rr}$. The defocusing power equation becomes

$$
w_{tt}-w_{rr}+r^{1-p}|w|^{p-1}w=0
$$

on the half-line.

##### Outgoing shell source estimate for a radial wave

↑ **Parent:** [Radial reduction of the three-dimensional wave equation](#radial-reduction-of-the-three-dimensional-wave-equation)

In three dimensions set $w=ru$ for a [radial function](partial-differential-equation.md#radial-function) satisfying $\Box u=F$. If the source has [support](function.md#support) in $s\leq r\leq s+1$ and $|F(s,r)|\leq(1+s)^{-2}$, the [Duhamel principle](diffusion-equation.md#duhamel-s-principle) bounds its contribution to $w(t,t+a)$ by $\frac12\log(1+t)$ for $1/2\leq a\leq1$. Its backward characteristic interval meets the source in a set of length at most one, and $r|F|\leq(1+s)^{-1}$. Division by $r\simeq1+t$ gives $|u|\lesssim\log(2+t)/(1+t)$ for compactly supported initial data.

##### Outgoing-energy identity for a radial defocusing wave

↑ **Parent:** [Radial reduction of the three-dimensional wave equation](#radial-reduction-of-the-three-dimensional-wave-equation)

For $q=w_t+w_r$ and a radial weight $\psi$,

$$
\frac d{dt}\int_0^\infty\psi\left(\frac12q^2+\frac{|w|^{p+1}}{(p+1)r^{p-1}}\right)dr
=-\frac12\int_0^\infty\psi'q^2dr
+\frac1{p+1}\int_0^\infty\frac{|w|^{p+1}}{r^{p-1}}
\left(\psi'-(p-1)\frac\psi r\right)dr.
$$

### Local weak solution by contraction for a semilinear wave equation

↑ **Parent:** [Semilinear wave equation](#semilinear-wave-equation)

Suppose the inhomogeneous linear wave equation has an energy estimate in a Banach solution space $X_T$, and its nonlinearity obeys

$$
\|F(w)\|_{L^2((0,T)\times U)}\leq C\sqrt T\,\|w\|_{X_T}^2,
$$

together with the corresponding locally Lipschitz estimate. For a sufficiently large closed ball and sufficiently small $T$, the map that solves the linear equation with source $F(w)$ is a contraction. The [contraction mapping theorem](analysis.md#contraction-mapping-theorem) then gives a local [weak solution](partial-differential-equation.md#weak-solution).

## Elastic wave

↑ **Parent:** [Wave equation](wave-equation.md)

An elastic wave propagates a disturbance through an elastic solid. Small displacements in [linear elasticity](continuum-mechanics.md#linear-elasticity) satisfy a vector [wave equation](wave-equation.md) governed by [mass density](fluid-mechanics.md#density) and the two [Lamé parameters](continuum-mechanics.md#lame-parameter).

### Characteristic crossing in a boundary-generated elastic simple wave

↑ **Parent:** [Elastic wave](#elastic-wave)

In a right-going [simple wave](compressible-flow.md#simple-wave), the state emitted at boundary time $s$ travels along $X=c_b(s)(t-s)$. The mapping from emission time to position first becomes singular when $\dot c_b(t-s)-c_b=0$, giving the displayed shock time and position $X=c_b^2/\dot c_b$. A smooth increase of [traction](continuum-mechanics.md#traction) produces steepening only if it increases the propagation speed. This describes the first gradient singularity; continuation as a [shock wave](partial-differential-equation.md#shock-wave) needs admissible jump conditions.

### Elastic slowness surface

↑ **Parent:** [Elastic wave](#elastic-wave)

For homogeneous stable [linear elasticity](continuum-mechanics.md#linear-elasticity), the three positive [eigenvalues](linear-operator-theory.md#eigenvalue) of the [acoustic tensor](continuum-mechanics.md#acoustic-tensor) give three [phase velocities](#phase-velocity) for each [wavefront](optics.md#wavefront) normal. Plotting the corresponding three vectors $\mathbf p=\mathbf n/v$ gives the three sheets of the elastic [slowness surface](#elastic-slowness-surface). Sheets can meet at degeneracies. The [elastic-wave energy flux](continuum-mechanics.md#elastic-wave-energy-flux) is normal to each regular sheet: differentiating its [eigenvalue](linear-operator-theory.md#eigenvalue) equation along a sheet tangent $d\mathbf p$ gives $c_{ijkl}a_i a_k p_l\,dp_j=0$.

#### Vertical slowness sextic of an anisotropic solid

↑ **Parent:** [Elastic slowness surface](#elastic-slowness-surface)

Fix horizontal [slowness](#slowness) $p_\alpha$ and define $T_{ip}=c_{i3p3}$, $R_{ip}=c_{i3p\alpha}p_\alpha$ and $Q_{ip}=c_{i\alpha p\beta}p_\alpha p_\beta$. Under [strong ellipticity in elasticity](continuum-mechanics.md#strong-ellipticity-in-elasticity), $T$ is positive definite, so the vertical-slowness determinant has degree six with real coefficients. Real roots are intersections of a vertical line with the [elastic slowness surface](#elastic-slowness-surface); complex-conjugate pairs give [evanescent waves](continuum-mechanics.md#evanescent-wave).

#### Elastic wave surface

↑ **Parent:** [Elastic slowness surface](#elastic-slowness-surface)

The unit-time elastic [wave surface](#elastic-wave-surface) is the locus of [group velocities](#group-velocity) on the three branches of a homogeneous [elastic wave](#elastic-wave). At time $t$, its scaled sheets describe the propagating [wavefronts](optics.md#wavefront) from an impulsive point source when that source excites the corresponding modes. Homogeneity of the [dispersion relation](#dispersion-relation) gives $\mathbf p\cdot\mathbf g=1$, so each regular sheet is the envelope of planes $\mathbf p\cdot\mathbf x=1$. It is generally different from the radial reciprocal of the [elastic slowness surface](#elastic-slowness-surface).

##### Slowness curvature and wave-surface cusps

↑ **Parent:** [Elastic wave surface](#elastic-wave-surface)

In a symmetry-plane cross-section, write $\mathbf p=r(\theta)\mathbf n(\theta)$, $v=1/r$, and $\mathbf t=\mathbf n\prime$. The [elastic wave surface](#elastic-wave-surface) is $\mathbf g=v\mathbf n+v\prime\mathbf t$. Its derivative vanishes when $v+v\prime\prime=(r^2+2r\prime^2-r r\prime\prime)/r^3=0$, exactly an [inflection point](topology.md#inflection-point) of the regular [slowness surface](#elastic-slowness-surface). At a simple zero the second and third derivatives of $\mathbf g$ are linearly independent, giving an ordinary [cusp](algebraic-geometry.md#cusp-algebraic-geometry). Smooth nonconvex [slowness surface](#elastic-slowness-surface) sheets can therefore generate cusped [wavefronts](optics.md#wavefront).

#### Elastic energy velocity

↑ **Parent:** [Elastic slowness surface](#elastic-slowness-surface)

For a real branch polarization $\mathbf a$ and complex displacement amplitude $U$, the cycle averages are $\langle F_j\rangle=\omega|U|^2c_{ijkl}a_i a_k k_l/2$ and $\langle W\rangle=\rho\omega^2|U|^2|\mathbf a|^2/2$. Differentiating the [acoustic tensor](continuum-mechanics.md#acoustic-tensor) [eigenvalue](linear-operator-theory.md#eigenvalue) equation with respect to $k_j$ gives their ratio as the [group velocity](#group-velocity). This identifies the [energy flux](physics.md#energy-flux) direction with the normal to the [elastic slowness surface](#elastic-slowness-surface) in a lossless nondispersive elastic medium.

##### Elastic mode classification by vertical energy flux

↑ **Parent:** [Elastic energy velocity](#elastic-energy-velocity)

For a mode $u=a e^{i\omega(p_\alpha x_\alpha+qx_3-t)}$ with $x_3$ positive downwards, the reduced [traction](continuum-mechanics.md#traction) is $(Tq+R)a$. Its mean vertical [acoustic energy flux](continuum-mechanics.md#acoustic-energy-flux) is the displayed expression. Propagating modes are downgoing for positive flux and upgoing for negative flux; phase-slowness sign need not agree in [anisotropy](continuum-mechanics.md#anisotropy). Depth-decaying evanescent modes have $\operatorname{Im}q>0$. At grazing or repeated roots use limiting radiation modes.

###### Free-surface anisotropic reflection amplitudes

↑ **Parent:** [Elastic mode classification by vertical energy flux](#elastic-mode-classification-by-vertical-energy-flux)

Select the three downgoing or depth-decaying elastic modes for a solid below a plane free surface. For each mode use its reduced [traction](continuum-mechanics.md#traction) column $b=(Tq+R)a$. Zero total boundary [traction](continuum-mechanics.md#traction) gives $BA=-b_0$ for an incident mode of reduced traction $b_0$. Invertibility gives the displayed amplitudes. A singular matrix instead permits an outgoing homogeneous surface mode, so a radiation-limit or solvability analysis is necessary.

### Elastodynamic Green tensor

↑ **Parent:** [Elastic wave](#elastic-wave)

The causal [Green function](analysis.md#green-s-function) for isotropic [linear elasticity](continuum-mechanics.md#linear-elasticity) is tensor-valued: column $k$ is the displacement caused by a point impulsive [body force](fluid-mechanics.md#body-force) in direction $k$. Its radiative terms are longitudinal [P waves](#p-wave) at $t=R/\alpha$ and transverse [S waves](#s-wave) at $t=R/\beta$, proportional to $R^{-1}$. A term supported between the arrivals carries the intermediate/near-field response. Convolution in time and space constructs the displacement for a general source.

#### Far-field P and S radiation from a point force

↑ **Parent:** [Elastodynamic Green tensor](#elastodynamic-green-tensor)

In a homogeneous [isotropic](continuum-mechanics.md#isotropy) solid, the far-field [P wave](#p-wave) is the radial projection of the force and the [S wave](#s-wave) is its transverse projection. For a unit force axis $d$, the magnitudes are $|\cos\theta|$ and $\sin\theta$. The approximation requires distance large compared with both reduced wavelengths; angular nodes can still be controlled by a smaller near-field contribution.

#### Elastodynamic surface-jump representation

↑ **Parent:** [Elastodynamic Green tensor](#elastodynamic-green-tensor)

Choose a surface normal $\mathbf n$ from its minus to its plus side and jumps $[u]=u^+-u^-$, $[t]=(\sigma^+-\sigma^-)\mathbf n$. The equivalent force density is $-[t]$ and the dipole density is $M_{jk}=c_{jk\ell m}[u_\ell]n_m$. This follows by applying the elastic wave operator to a piecewise smooth [displacement field](continuum-mechanics.md#displacement-field-mechanics): its distributional source is $-[t_i]\delta_\Sigma-\partial_j(c_{ijkl}[u_k]n_l\delta_\Sigma)$. [Integration by parts](calculus.md#integration-by-parts) against the [elastodynamic Green tensor](#elastodynamic-green-tensor) gives the displayed signs. At a material interface the dipole term is interpreted through the continuous reciprocal Green [traction](continuum-mechanics.md#traction), rather than an undefined product of a discontinuous stiffness with a surface delta.

#### Point-moment elastodynamic displacement

↑ **Parent:** [Elastodynamic Green tensor](#elastodynamic-green-tensor)

Integrating the equivalent dipole [body force](fluid-mechanics.md#body-force) against the [elastodynamic Green tensor](#elastodynamic-green-tensor) by parts gives the displayed time convolution. For a fixed [seismic moment tensor](#seismic-moment-tensor) shape $M_{kj}=K_{kj}V(t)$, its $R^{-1}$ terms are $[\mathbf e(\mathbf e\cdot K\mathbf e)\dot V(t-R/\alpha)/\alpha^3+(K\mathbf e-\mathbf e(\mathbf e\cdot K\mathbf e))\dot V(t-R/\beta)/\beta^3]/(4\pi\rho R)$. Derivatives of the angular projectors and the retarded near-field integral additionally produce $R^{-2}$ and $R^{-4}$ coefficients, yielding the final static field after the source stops.

### Seismic moment tensor

↑ **Parent:** [Elastic wave](#elastic-wave)

A localized zero-resultant [seismic moment tensor](#seismic-moment-tensor) represents the leading force-dipole part of an [elastic wave](#elastic-wave) source through the displayed equivalent [body force](fluid-mechanics.md#body-force). For a prescribed displacement jump $b_i$ across a surface with normal $n_j$, its moment density is $c_{ijkl}b_kn_l$, where $c$ is the [elastic stiffness tensor](continuum-mechanics.md#elastic-stiffness-tensor). Spatial integration gives the point-source moment when the source is small compared with the wavelengths.

#### Explosion radiation in an isotropic elastic solid

↑ **Parent:** [Seismic moment tensor](#seismic-moment-tensor)

An isotropic point moment is a dilatational gradient source. Its radial projection gives direction-independent [P wave](#p-wave) radiation, whereas its transverse projection vanishes. Thus it produces no far-field [S wave](#s-wave) in a homogeneous [isotropic](continuum-mechanics.md#isotropy) solid; conversion at an interface can change that conclusion.

#### Double-couple fault source

↑ **Parent:** [Seismic moment tensor](#seismic-moment-tensor)

Tangential fault slip $\mathbf b$ in an [isotropic](continuum-mechanics.md#isotropy) elastic material has the displayed moment density. It is symmetric and trace-free, with [eigenvalues](linear-operator-theory.md#eigenvalue) $\mu|b|,-\mu|b|,0$. The two off-diagonal force dipoles form equal couples with opposite [torques](classical-mechanics.md#torque), producing zero resultant force and [torque](classical-mechanics.md#torque). For a uniform patch of area $A$, the scalar seismic moment is $M_0=\mu A|b|$. [Traction](continuum-mechanics.md#traction) continuity removes the single-force layer in the [elastodynamic surface-jump representation](#elastodynamic-surface-jump-representation).

##### Double-couple radiation pattern

↑ **Parent:** [Double-couple fault source](#double-couple-fault-source)

For the [seismic moment tensor](#seismic-moment-tensor) $M=e_1e_2^{\mathsf T}+e_2e_1^{\mathsf T}$, source differentiation of the outgoing [elastodynamic Green tensor](#elastodynamic-green-tensor) gives $A_P=n^{\mathsf T}Mn$ and $\boldsymbol A_S=(I-nn^{\mathsf T})Mn$. In the $x_1x_2$ plane the signed radial [P wave](#p-wave) and tangential [S wave](#s-wave) factors are $\sin2\phi$ and $\cos2\phi$. The full [S wave](#s-wave) magnitude squared is $n_1^2+n_2^2-4n_1^2n_2^2$.

#### Tensile-crack seismic source

↑ **Parent:** [Seismic moment tensor](#seismic-moment-tensor)

A small planar crack of area $S$ opening normally by $d(t)$ has volume change $V=Sd$ and the displayed [seismic moment tensor](#seismic-moment-tensor). Its principal dipoles are $\lambda V,\lambda V,(\lambda+2\mu)V$: two act in the crack plane and the largest acts normally for positive opening and ordinary positive Lamé parameters. The definition follows by contracting the isotropic [elastic stiffness tensor](continuum-mechanics.md#elastic-stiffness-tensor) with two copies of the crack normal.

##### Tensile-crack radiation pattern

↑ **Parent:** [Tensile-crack seismic source](#tensile-crack-seismic-source)

For a planar [tensile-crack seismic source](#tensile-crack-seismic-source), $\theta$ is measured from its normal. The [P wave](#p-wave) displacement is radial with the first displayed amplitude. The [S wave](#s-wave) displacement is tangential in the plane containing the observation direction and crack normal, with four alternating signed lobes and nodes at the poles and equator. Both radiative fields depend on the opening rate and vanish once opening stops; the static [displacement field](continuum-mechanics.md#displacement-field-mechanics) depends on the final opening.

### Energy uniqueness for traction-driven elasticity

↑ **Parent:** [Elastic wave](#elastic-wave)

The difference of two solutions with the same [body force](fluid-mechanics.md#body-force), boundary [traction](continuum-mechanics.md#traction) and initial data satisfies a homogeneous elastic equation with zero boundary [work](classical-mechanics.md#work). Multiplication by its [velocity](classical-mechanics.md#velocity) and [integration by parts](calculus.md#integration-by-parts) conserve the displayed positive [energy](classical-mechanics.md#energy). Zero initial [energy](classical-mechanics.md#energy) forces zero [velocity](classical-mechanics.md#velocity) for all times, and zero initial [displacement field](continuum-mechanics.md#displacement-field-mechanics) then forces zero [displacement field](continuum-mechanics.md#displacement-field-mechanics). Rigid zero-strain motions do not cause nonuniqueness after initial data are fixed. This assumes positive [mass density](fluid-mechanics.md#density), stable real elastic moduli and sufficient regularity for the [energy](classical-mechanics.md#energy) identity.

#### Elastic energy uniqueness with restoring boundary springs

↑ **Parent:** [Energy uniqueness for traction-driven elasticity](#energy-uniqueness-for-traction-driven-elasticity)

For a time-independent symmetric negative semidefinite boundary matrix $k$, the difference of two [linear elasticity](continuum-mechanics.md#linear-elasticity) solutions with the same data has [traction](continuum-mechanics.md#traction) $kw$. Integration by parts conserves the displayed nonnegative [energy](classical-mechanics.md#energy). Zero initial data force zero velocity and then zero displacement. The matrix $-k$ is the stiffness of boundary springs to a prescribed support; null directions are traction-free.

### Seismic impedance

↑ **Parent:** [Elastic wave](#elastic-wave)

For a one-dimensional shear [elastic wave](#elastic-wave), the [seismic impedance](#seismic-impedance) is the magnitude of the ratio of [stress](continuum-mechanics.md#stress) to particle [velocity](classical-mechanics.md#velocity) in a progressive wave. With the positive coordinate aligned with [elastic wave](#elastic-wave) propagation and tension-positive [stress](continuum-mechanics.md#stress), $\sigma=-Zv$ for the forward wave and $\sigma=Zv$ for the backward wave. Its instantaneous [elastic-wave energy flux](continuum-mechanics.md#elastic-wave-energy-flux) is $-v\sigma$.

#### Seismic layer transfer matrix

↑ **Parent:** [Seismic impedance](#seismic-impedance)

At normal incidence, a uniform lossless [elastic wave](#elastic-wave) layer of thickness $h_j$, speed $c_j$ and [seismic impedance](#seismic-impedance) $q_j=\rho_jc_j$ has [wave phase](physics.md#phase-waves) thickness $\delta_j=\omega h_j/c_j$. With phasors proportional to $e^{-i\omega t}$, particle [velocity](classical-mechanics.md#velocity) $V$ and compressive [traction](continuum-mechanics.md#traction) $P=-T$, the displayed [matrix](vector-space.md#matrix) maps $(V,P)$ from the top to the bottom. It has [determinant](linear-algebra.md#determinant) one. Multiplying these [matrices](vector-space.md#matrix) in physical order accounts for all coherent multiple reflections. Continuity of $V,P$ connects adjacent layers without another propagation factor.

##### Periodic seismic multilayer stop band

↑ **Parent:** [Seismic layer transfer matrix](#seismic-layer-transfer-matrix)

The two-layer cell [seismic layer transfer matrix](#seismic-layer-transfer-matrix) has reciprocal [eigenvalues](linear-operator-theory.md#eigenvalue) because its [determinant](linear-algebra.md#determinant) is one. Writing them as $e^{\pm iKd}$ gives the displayed half-trace relation. At a real [frequency](physics.md#frequency), an absolute half-trace exceeding one forces an exponentially growing/decaying pair instead of propagating cell modes. A long finite stack then suppresses transmission in this stop band, without dissipating [energy](classical-mechanics.md#energy): the missing transmitted flux is reflected. Quarter-wave layers of unequal [seismic impedance](#seismic-impedance) give half-trace $-\tfrac12(q_1/q_2+q_2/q_1)<-1$.

#### Flux-normalized elastic characteristic amplitudes

↑ **Parent:** [Seismic impedance](#seismic-impedance)

These characteristic [wave amplitudes](physics.md#wave-amplitude) split a one-dimensional [elastic wave](#elastic-wave) into forward and backward components. Their instantaneous net [elastic-wave energy flux](continuum-mechanics.md#elastic-wave-energy-flux) is $\phi_+^2-\phi_-^2$. For real-part harmonic phasors the mean flux is $(|\phi_+|^2-|\phi_-|^2)/2$. In a static graded medium with real positive [seismic impedance](#seismic-impedance), put $g=(\log Z)'/2$; then $\partial_x\phi_\pm\pm\beta^{-1}\partial_t\phi_\pm=g\phi_\mp$. [Seismic impedance](#seismic-impedance) [gradients](calculus.md#gradient) couple the two directions while preserving net flux.

##### Zero-frequency scattering through an elastic layer

↑ **Parent:** [Flux-normalized elastic characteristic amplitudes](#flux-normalized-elastic-characteristic-amplitudes)

At zero [frequency](physics.md#frequency) the graded-layer transfer equation integrates to $\exp[L\begin{pmatrix}0&1\\1&0\end{pmatrix}]$, where $L=\tfrac12\log(Z_b/Z_a)$. Eliminating the outgoing [wave amplitude](physics.md#wave-amplitude) at the left endpoint gives the displayed incoming-to-outgoing [scattering matrix](quantum-mechanics.md#s-matrix). It is real [orthogonal](linear-algebra.md#orthogonal-vectors), so it preserves total incoming and outgoing flux. It coincides with continuity of [velocity](classical-mechanics.md#velocity) and [traction](continuum-mechanics.md#traction) at a sharp [seismic impedance](#seismic-impedance) interface; the profile between the endpoints enters at nonzero [frequency](physics.md#frequency).

### Love wave

↑ **Parent:** [Elastic wave](#elastic-wave)

A Love wave is a horizontally polarized shear wave trapped in a slower elastic surface layer above a faster elastic half-space. Zero shear traction at the free surface, displacement continuity and traction continuity at the interface produce its dispersion relation. A trapped mode has phase speed between the two shear speeds and decays exponentially into the half-space.

#### Anisotropic Love-wave dispersion

↑ **Parent:** [Love wave](#love-wave)

For an aligned anisotropic surface layer, $q^2=(\omega^2-\beta_x'^2k^2)/\beta_z'^2$, while the isotropic substrate has $\kappa^2=k^2-\omega^2/\beta^2$. Zero top [traction](continuum-mechanics.md#traction) and welded displacement/traction continuity give the displayed [dispersion relation](#dispersion-relation). The horizontal speed sets the limiting [phase velocity](#phase-velocity); the vertical speed sets rigid-base cutoff frequencies. The effective contrast for the high-contrast transition is $\rho'\beta_x'\beta_z'/(\rho\beta^2)$.

#### Rigid-base approximation to Love waves

↑ **Parent:** [Love wave](#love-wave)

A free top and rigid base impose transverse [wavenumbers](#wavenumber) $(n+1/2)\pi/h$ on [guided SH modes between rigid and free planes](#guided-sh-modes-between-rigid-and-free-planes). Their [phase velocity](#phase-velocity) and [group velocity](#group-velocity) are $c=\beta'/\sqrt{1-\omega_n^2/\omega^2}$ and $U=\beta'\sqrt{1-\omega_n^2/\omega^2}$ for $\omega>\omega_n$. A real [Love wave](#love-wave) replaces the rigid base by an evanescent elastic load; the approximation becomes reliable sufficiently above the corresponding strong-dispersion transition, not at the actual mode cutoff.

##### Group-velocity minimum of a high-contrast Love wave

↑ **Parent:** [Rigid-base approximation to Love waves](#rigid-base-approximation-to-love-waves)

With $\epsilon=\beta'/\beta\ll1$, $\eta=\mu'/\mu=O(\epsilon^2)$ and a fixed mode index, put $y=qh$, $W=\omega h/\beta'$ and $K=kh$. The exact [Love wave](#love-wave) branch has $W=y\sqrt{1+\eta^2\tan^2y}/\sqrt{1-\epsilon^2}$ and $K=y\sqrt{\epsilon^2+\eta^2\tan^2y}/\sqrt{1-\epsilon^2}$. Its minimum [group velocity](#group-velocity) occurs near $y=(n+1/2)\pi$, with transition width $W-(n+1/2)\pi$ of order $(\eta^2(n+1/2)\pi)^{1/3}$. Well above that width, the [rigid-base approximation to Love waves](#rigid-base-approximation-to-love-waves) captures both velocities. Density ratios and the mode index must be controlled in this estimate.

#### Love-wave cutoff frequencies

↑ **Parent:** [Love wave](#love-wave)

For a slow uniform layer over a faster half-space, the nth [Love wave](#love-wave) branch reaches the half-space shear [wave speed](#wave-speed) at the displayed threshold. Its half-space decay exponent then vanishes, so the threshold is a limiting nonlocalized state, not a trapped finite-energy mode. The fundamental has zero threshold and exists at every positive [frequency](physics.md#frequency); overtones require [frequency](physics.md#frequency) strictly above their positive threshold. At high [frequency](physics.md#frequency) each fixed branch approaches the layer shear [wave speed](#wave-speed) from above.

#### Love-wave interface reflection phase

↑ **Parent:** [Love wave](#love-wave)

For a slower surface layer supporting propagating [SH-waves](#sh-wave) with vertical [wavenumber](#wavenumber) $q>0$ above an [evanescent](continuum-mechanics.md#evanescent-wave) half-space with decay exponent $p>0$, continuity of [displacement field](continuum-mechanics.md#displacement-field-mechanics) and [traction](continuum-mechanics.md#traction) gives the displayed [reflection coefficient](partial-differential-equation.md#reflection-coefficient) for a downward incident [displacement field](continuum-mechanics.md#displacement-field-mechanics) wave. Its modulus is one and its [wave phase](physics.md#phase-waves) is $-2\arctan(\mu p/(\mu_0q))$. A traction-free top reflects [displacement field](continuum-mechanics.md#displacement-field-mechanics) with coefficient $+1$. The round-trip condition $R_he^{2iqh}=1$ then gives $\tan(qh)=\mu p/(\mu_0q)$, equivalent to direct [Love wave](#love-wave) mode matching.

#### Strict cutoff of the second Love-wave mode

↑ **Parent:** [Love wave](#love-wave)

For a slow elastic layer above a faster half-space, put $q=\sqrt{c^2/\bar c_s^2-1}$ and $q_{\max}=\sqrt{c_s^2/\bar c_s^2-1}$. The positive branches of $\tan(khq)$ intersect the positive strictly decreasing traction ratio once whenever their left endpoint $m\pi$ is strictly below $khq_{\max}$. The fundamental exists for every positive $kh$; the second requires the displayed strict inequality. At equality $c=c_s$ and the half-space decay exponent vanishes, so that endpoint is a cutoff, not a trapped mode satisfying decay at minus infinity.

### Rayleigh wave

↑ **Parent:** [Elastic wave](#elastic-wave)

A [Rayleigh wave](#rayleigh-wave) propagates along a stress-free boundary of an isotropic elastic half-space and decays into its interior. It combines an evanescent longitudinal wave with an evanescent vertically polarized shear wave. If its speed is $0<c<c_S<c_P$, the decay factors are $\alpha=\sqrt{1-c^2/c_P^2}$ and $\beta=\sqrt{1-c^2/c_S^2}$. Vanishing shear and normal traction gives the displayed determinant condition.

### Rigid elastic waveguide mode

↑ **Parent:** [Elastic wave](#elastic-wave)

In a homogeneous elastic layer $-H<z<H$ with rigid boundaries, in-plane propagating modes mix P- and SV-waves. For phase speed $c>c_P>c_S$, one even-horizontal, odd-vertical family obeys

$$
a\tan(akH)=-\frac{\tan(bkH)}b,
\qquad
a=\sqrt{\frac{c^2}{c_P^2}-1},
\quad
b=\sqrt{\frac{c^2}{c_S^2}-1}.
$$

#### Ray asymptotics of a clamped elastic waveguide mode

↑ **Parent:** [Rigid elastic waveguide mode](#rigid-elastic-waveguide-mode)

A [shear-horizontal wave](continuum-mechanics.md#shear-horizontal-wave) mode has $\omega_n(k)=c_s\sqrt{k^2+(n\pi/h)^2}$. At $x=Vt$ with $0<|V|<c_s$, a nondegenerate stationary Fourier phase gives generic $t^{-1/2}$ decay. Faster rays have no [stationary point](calculus-of-variations.md#stationary-point); compactly supported data give eventual zero by [finite propagation speed](#finite-propagation-speed).

### Helmholtz separation of elastic waves

↑ **Parent:** [Elastic wave](#elastic-wave)

Divergence of the elastic equation isolates dilatational motion, while curl isolates rotational motion, producing P and S wave equations with different speeds.

#### P-SV displacement potentials

↑ **Parent:** [Helmholtz separation of elastic waves](#helmholtz-separation-of-elastic-waves)

In a uniform isotropic material, these scalar [P-SV displacement potentials](#p-sv-displacement-potentials) separate longitudinal [P waves](#p-wave) from vertically polarized [SV-waves](#sv-wave) in an $x,z$ plane. They satisfy $\phi_{tt}=\alpha^2\Delta\phi$ and $\psi_{tt}=\beta^2\Delta\psi$, with compressional and shear speeds $\alpha,\beta$. Reversing the sign convention for $\psi$ changes its polarization column but not the physical [P-SV directional impedance matrix](continuum-mechanics.md#p-sv-directional-impedance-matrix) or the separate modal [energy](classical-mechanics.md#energy) fluxes.

### P wave

↑ **Parent:** [Elastic wave](#elastic-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/P_wave)

A P-wave is longitudinal, carries nonzero dilatation, and has speed $c_P=\sqrt{(\lambda+2\mu)/\rho}$ in an isotropic solid.

#### P-wavefront discontinuity transport

↑ **Parent:** [P wave](#p-wave)

Let $t=T(\mathbf x)$ be a smooth [wavefront](optics.md#wavefront) and suppose the first jump in time [derivatives](calculus.md#derivative) of [displacement field](continuum-mechanics.md#displacement-field-mechanics) is $[\partial_t^k\mathbf u]=a^{[k]}\mathbf n$, with $k\geq2$. Substitution of $\mathbf u=a^{[k]}\mathbf n(t-T)_+^k/k!+\cdots$ into the elastic equation first gives the [eikonal equation](continuum-mechanics.md#eikonal-equation) $|\nabla T|=1/\alpha$ and longitudinal polarization $\mathbf n=\alpha\nabla T$. Projecting the next-order compatibility condition onto $\mathbf n$ gives $2\rho\alpha\mathbf n\cdot\nabla a^{[k]}+a^{[k]}\nabla\cdot(\rho\alpha\mathbf n)=0$, hence the displayed conservation law. Coefficients and [wavefront](optics.md#wavefront) must be sufficiently differentiable for this classical transport equation; its local form fails at a [caustic](optics.md#wave-caustic).

##### Transmitted jump at a collimating solid-fluid interface

↑ **Parent:** [P-wavefront discontinuity transport](#p-wavefront-discontinuity-transport)

The spherical source potential $f(t-r/\alpha)/r$ gives leading longitudinal [displacement field](continuum-mechanics.md#displacement-field-mechanics) $-f'(t-r/\alpha)/(\alpha r)$. Apply the local [solid-fluid P-wave transmission coefficient](continuum-mechanics.md#solid-fluid-p-wave-transmission-coefficient) to its potential at a smooth interface. In [hyperbolic interface collimation of P-waves](#hyperbolic-interface-collimation-of-p-waves), transmitted rays are parallel, so [ray-tube conservation for a P-wave jump](#ray-tube-conservation-for-a-p-wave-jump) makes the leading coefficient constant along each vertical ray. This yields the displayed jump for the first nonzero [derivative](calculus.md#derivative) discontinuity of the waveform. Smooth transverse [derivatives](calculus.md#derivative) multiply $f$ rather than $f'$ and are one order more regular. The construction presupposes the indicated one-sided [derivative](calculus.md#derivative) jump exists; a source smooth to every order may have no jump.

##### Ray-tube conservation for a P-wave jump

↑ **Parent:** [P-wavefront discontinuity transport](#p-wavefront-discontinuity-transport)

A tube of neighboring [elastic rays](#elastic-ray) follows the [wavefront](optics.md#wavefront) normal. If $J$ is its infinitesimal transverse area, its expansion is $d\log J/ds=\nabla\cdot\mathbf n$ along arclength. The [P-wavefront discontinuity transport](#p-wavefront-discontinuity-transport) law therefore gives the displayed conserved flux. Geometrical spreading, [mass density](fluid-mechanics.md#density) and [wave speed](#wave-speed) determine the leading jump [wave amplitude](physics.md#wave-amplitude) together; the rule is valid before the ray tube reaches a [caustic](optics.md#wave-caustic).

#### Reflection of a P-wave from a rigid plane

↑ **Parent:** [P wave](#p-wave)

For a stable isotropic solid in $y<0$, use $u_x=\phi_x+\psi_y$, $u_y=\phi_y-\psi_x$. An incident [P wave](#p-wave) with [frequency](physics.md#frequency) $\omega$, tangential [wavenumber](#wavenumber) $\kappa$ and upward normal [wavenumber](#wavenumber) $a$ reflects into a P potential $Ae^{i(\kappa x-ay-\omega t)}$ and an SV potential $Be^{i(\kappa x-by-\omega t)}$, where $b^2=\omega^2/c_s^2-\kappa^2$. Vanishing of both displacements at the rigid plane gives $\kappa(1+A)-bB=0$, $a(1-A)-\kappa B=0$. Hence $A=(ab-\kappa^2)/(ab+\kappa^2)$ and $B=2a\kappa/(ab+\kappa^2)$. Because $c_p>c_s$ and $\kappa^2\leq\omega^2/c_p^2$, $b^2>0$ and the converted [S wave](#s-wave) propagates rather than being evanescent.

#### Longitudinal polarization

↑ **Parent:** [P wave](#p-wave)

In a longitudinal plane wave, displacement is parallel to the wavevector and the curl vanishes.

### S wave

↑ **Parent:** [Elastic wave](#elastic-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/S_wave)

An S-wave is transverse, carries rotation without dilatation, and has speed $c_S=\sqrt{\mu/\rho}$.

#### Transverse polarization

↑ **Parent:** [S wave](#s-wave)

In a transverse plane wave, displacement is perpendicular to the wavevector and its divergence vanishes.

#### SV-wave

↑ **Parent:** [S wave](#s-wave)

An SV-wave is polarized in the vertical plane containing its wavevector and perpendicular to that wavevector.

#### SH-wave

↑ **Parent:** [S wave](#s-wave)

An SH-wave is polarized horizontally and perpendicular to the vertical propagation plane.

##### SH ray-tube amplitude transport

↑ **Parent:** [SH-wave](#sh-wave)

For a leading [wavefront](optics.md#wavefront) singularity or discontinuity in a smooth isotropic [shear-horizontal wave](continuum-mechanics.md#shear-horizontal-wave) field, the ray transport equation conserves the displayed quantity along a tube of [elastic rays](#elastic-ray). Here $J$ is transverse tube width in two dimensions and area in three. Cylindrical spreading has $J\propto r$, so the leading [wave amplitude](physics.md#wave-amplitude) is proportional to $r^{-1/2}$. This rule excludes the immediate source neighborhood and [caustics](optics.md#wave-caustic).

###### Refraction of a cylindrical SH wavefront

↑ **Parent:** [SH ray-tube amplitude transport](#sh-ray-tube-amplitude-transport)

Place a line source a distance $h$ above a plane welded interface and put $q_j=(\beta_j^{-2}-p^2)^{1/2}$, $t_1=h/(\beta_1^2q_1)$ and $r_1=h/(\beta_1q_1)$. The transmitted [elastic ray](#elastic-ray) is $x=hp/q_1+\beta_2^2p(t-t_1)$, $z=\beta_2^2q_2(t-t_1)$. [Elastic-interface boundary conditions](#elastic-interface-boundary-conditions) give $T_{\rm SH}=2\mu_1q_1/(\mu_1q_1+\mu_2q_2)$. Differentiating the ray positions across neighboring values of $p$ and applying [SH ray-tube amplitude transport](#sh-ray-tube-amplitude-transport) gives the displayed leading amplitude. Both $q_j$ must be positive; critical and evanescent incidence require different asymptotics.

##### SH line-source near-field singularity

↑ **Parent:** [SH-wave](#sh-wave)

Integrating the [shear-horizontal wave](continuum-mechanics.md#shear-horizontal-wave) equation with force $F(t)\delta^{(2)}(\mathbf x)$ over a shrinking circle gives $2\pi\mu r\partial_ru\to-F(t)$. Thus the local [displacement field](continuum-mechanics.md#displacement-field-mechanics) has the displayed logarithmic singularity. This is a fixed-time near-source limit, distinct from the wavefront limit underlying [SH ray-tube amplitude transport](#sh-ray-tube-amplitude-transport).

##### Guided SH modes between rigid and free planes

↑ **Parent:** [SH-wave](#sh-wave)

For a layer $0<z<h$ with rigid lower boundary and traction-free upper boundary, an SH mode  
$u_y=Y(z)e^{i(\kappa x-\omega t)}$ has

$$
Y(z)=\sin(q_nz),\qquad
q_n=\frac{(2n+1)\pi}{2h},
$$

and dispersion

$$
\omega^2=c_s^2(\kappa^2+q_n^2).
$$

Its cutoff is $\omega_n=c_sq_n$, its phase speed is $\omega/\kappa$, and its group speed is $c_s^2\kappa/\omega$.

### Elastic-interface boundary conditions

↑ **Parent:** [Elastic wave](#elastic-wave)

At a perfectly bonded interface, all displacement and traction components are continuous.

#### P-SV mode conversion at a solid interface

↑ **Parent:** [Elastic-interface boundary conditions](#elastic-interface-boundary-conditions)

An obliquely incident in-plane P-wave generally produces reflected and transmitted P and SV waves; SH polarization decouples.

#### Snell law for elastic waves

↑ **Parent:** [Elastic-interface boundary conditions](#elastic-interface-boundary-conditions)

Phase matching fixes a common frequency and tangential wavenumber for every incident, reflected, and transmitted elastic mode.

### Acoustic reflection and transmission at an interface

↑ **Parent:** [Elastic wave](#elastic-wave)

For two inviscid media, continuity of normal displacement and normal stress determines the reflected and transmitted longitudinal amplitudes.

#### Lossless acoustic membrane scattering

↑ **Parent:** [Acoustic reflection and transmission at an interface](#acoustic-reflection-and-transmission-at-an-interface)

Equal normal velocities and the membrane tension-mass balance determine complex pressure amplitudes. With identical fluids on both sides the reflected and transmitted squared amplitudes sum to one, expressing conserved mean energy flux.

#### Equal displacement-amplitude condition at an acoustic interface

↑ **Parent:** [Acoustic reflection and transmission at an interface](#acoustic-reflection-and-transmission-at-an-interface)

Equating the absolute reflected and transmitted displacement amplitudes, then using acoustic Snell's law, gives an algebraic condition on incidence angle and the two moduli-over-speed impedances.

## Damping

↑ **Parent:** [Wave equation](wave-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Damping)

Damping dissipates the [energy](classical-mechanics.md#energy) of an [oscillation](physics.md#oscillation), reducing its [amplitude](physics.md#wave-amplitude). A [linearly damped string](#linearly-damped-string) applies this mechanism to each [normal mode](#normal-mode).

Why can stronger [damping](#damping) make a return to [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system) slower? A weak brake lets a [spring](continuum-mechanics.md#spring) exchange [potential energy](classical-mechanics.md#potential-energy) with [kinetic energy](classical-mechanics.md#kinetic-energy) many times; a very strong brake makes the final motion creep. [Critical damping](#critical-damping) marks the boundary between these behaviours. The distinction depends on the [force](classical-mechanics.md#force) law: the classification below concerns a single [damped harmonic oscillator](analysis.md#damped-harmonic-oscillator) with [viscous damping](#viscous-damping), rather than every mechanism that removes [energy](classical-mechanics.md#energy).

Let $x(t)$ be [displacement](classical-mechanics.md#displacement) from [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system), $m>0$ the moving [mass](classical-mechanics.md#mass), $k>0$ the [spring constant](continuum-mechanics.md#spring-constant), and $b\geq0$ the constant coefficient of [viscous damping](#viscous-damping). With no driving [force](classical-mechanics.md#force), [Newton's second law](classical-mechanics.md#newton-s-second-law) gives

$$
m\ddot x+b\dot x+kx=0,\qquad x(0)=x_0,\quad \dot x(0)=v_0.
$$

The two [initial conditions](differential-equation.md#initial-condition) specify [displacement](classical-mechanics.md#displacement) and [velocity](classical-mechanics.md#velocity). Define the undamped [eigenfrequency](#eigenfrequency) as an [angular frequency](classical-mechanics.md#angular-frequency) $\omega_0=\sqrt{k/m}$ and the [damping ratio](#damping-ratio) as $\zeta=b/(2\sqrt{mk})$. The [ordinary differential equation](differential-equation.md#ordinary-differential-equation) becomes $\ddot x+2\zeta\omega_0\dot x+\omega_0^2x=0$. A constant weight in a vertical [spring](continuum-mechanics.md#spring) merely shifts [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system); it is already absorbed in the definition of $x$.[§15.5, equations 15.23–15.26 and the force discussion preceding 15.23](physics-bibliography.md#university-physics-volume-1-by-william-moebs-and-others/15-5-damped-oscillations)

For example, the ideal parameters $m=1\,\mathrm{kg}$ and $k=4\,\mathrm{N\,m^{-1}}$ give $\omega_0=2\,\mathrm{s^{-1}}$ and [critical damping](#critical-damping) at $b=4\,\mathrm{kg\,s^{-1}}$. Values $b=1,4,8\,\mathrm{kg\,s^{-1}}$ give [damping ratios](#damping-ratio) $0.25,1,2$, respectively. These are model choices, not measured values. For release from rest with $x_0>0$, set $X=x/x_0$ and $\tau=\omega_0t$; then $X''+2\zeta X'+X=0$, where primes now denote [derivatives](calculus.md#derivative) with respect to $\tau$.

<a id="image-ideal-viscous-oscillator-responses-release-from-rest-in-three-damping-regimes-and-the-effect-of-initial-velocity-at-critical-damping"></a>
![](damped-oscillator-initial-value-responses.png)

**[Figure 3](#image-ideal-viscous-oscillator-responses-release-from-rest-in-three-damping-regimes-and-the-effect-of-initial-velocity-at-critical-damping). Ideal viscous oscillator responses: release from rest in three damping regimes, and the effect of initial velocity at critical damping**.

The left panel uses identical [initial conditions](differential-equation.md#initial-condition) $X(0)=1$, $X'(0)=0$. [Underdamping](#underdamping) produces repeated crossings of [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system); [critical damping](#critical-damping) and [overdamping](#overdamping) give positive decreasing responses. The right panel keeps [critical damping](#critical-damping) but changes initial [velocity](classical-mechanics.md#velocity): $X'(0)=-2$ gives one crossing, although there is no [oscillation](physics.md#oscillation). Both panels are exact model predictions.

### Critical damping

↑ **Parent:** [Damping](#damping)

[Critical damping](#critical-damping) is the repeated-root case of the [viscous damping](#viscous-damping) model: its two [characteristic roots](differential-equation.md#characteristic-root-of-a-constant-coefficient-differential-equation) coincide at $r=-\omega_0$. The solution with arbitrary [initial conditions](differential-equation.md#initial-condition) is

$$
x(t)=\bigl[x_0+(v_0+\omega_0x_0)t\bigr]e^{-\omega_0t}.
$$

The extra factor $t$ is essential: one [exponential function](calculus.md#exponential-function) alone cannot fit arbitrary initial [displacement](classical-mechanics.md#displacement) and [velocity](classical-mechanics.md#velocity) when the [characteristic equation](differential-equation.md#characteristic-equation-of-a-constant-coefficient-differential-equation) has a double [polynomial root](polynomial.md#root-of-a-polynomial). Substitution, or taking the limit of the [underdamped](#underdamping) formula as its [angular frequency](classical-mechanics.md#angular-frequency) tends to zero, gives the displayed expression.

The precise fastest-return statement is this: hold $m$, $k$, $x_0>0$ and $v_0=0$ fixed, and compare all $\zeta\geq1$. Every response decreases positively toward [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system); the [critically damped](#critical-damping) response

$$
x_{\mathrm c}(t)=x_0(1+\omega_0t)e^{-\omega_0t}
$$

is smaller than every [overdamped](#overdamping) response at each $t>0$. It therefore reaches and stays within any specified band $|x|\leq\epsilon x_0$, $0<\epsilon<1$, sooner than those responses. Exact arrival at rest takes infinite [time](classical-mechanics.md#time-in-physics). This is a comparison among nonoscillatory regimes for these particular [initial conditions](differential-equation.md#initial-condition), not a universal minimum of every possible settling-time criterion.

One short comparison argument uses $q=\partial X/\partial\zeta$. Its [initial conditions](differential-equation.md#initial-condition) are zero and $q''+2\zeta q'+q=-2X'$. For release from rest, $X'<0$ at $\tau>0$; the [causal Green function of a damped oscillator](analysis.md#causal-green-function-of-a-damped-oscillator) is positive at positive [time](classical-mechanics.md#time-in-physics) for $\zeta\geq1$. Its [convolution](fourier-analysis.md#convolution) with $-2X'$ gives $q>0$: increasing [damping](#damping) beyond the critical value increases the remaining [displacement](classical-mechanics.md#displacement).

There is no repeated [oscillation](physics.md#oscillation) at [critical damping](#critical-damping), but there can be overshoot once. For $x_0>0$, the factor in square brackets crosses zero precisely when $v_0<-\omega_0x_0$, at

$$
t_*=-\frac{x_0}{v_0+\omega_0x_0}>0.
$$

For example, $v_0=-2\omega_0x_0$ gives $x=x_0(1-\omega_0t)e^{-\omega_0t}$, crossing [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system) at $t=1/\omega_0$ as shown above. An [overdamped](#overdamping) response can also cross once for suitable [initial conditions](differential-equation.md#initial-condition). Conversely, specially chosen [initial conditions](differential-equation.md#initial-condition) can remove its slow [exponential decay](analysis.md#exponential-decay) entirely. Thus the generic slow-root argument must not be applied to a response whose slow-root coefficient is zero.

### Viscous damping

↑ **Parent:** [Damping](#damping)

[Viscous damping](#viscous-damping) means a [force](classical-mechanics.md#force) proportional to, and opposite to, [velocity](classical-mechanics.md#velocity): $F_{\mathrm d}=-b\dot x$ with $b\geq0$. Its coefficient has units $\mathrm{kg\,s^{-1}}$, equivalently $\mathrm{N\,s\,m^{-1}}$. The name describes a [force](classical-mechanics.md#force) law; [eddy-current damping](#eddy-current-damping) can approximate the same law without a viscous fluid. Constant $m$, $b$ and $k$ produce a [linear ordinary differential equation](differential-equation.md#linear-ordinary-differential-equation), allowing [superposition](vector-space.md#superposition-principle) of responses. [Kinetic friction](classical-mechanics.md#kinetic-friction) with approximately constant magnitude and [quadratic drag](fluid-mechanics.md#quadratic-drag) obey different laws, so their decay need not have the [exponential decay](analysis.md#exponential-decay) or critical threshold derived here.

#### Damping ratio

↑ **Parent:** [Viscous damping](#viscous-damping)

The [damping ratio](#damping-ratio) is the dimensionless ratio $b/b_{\mathrm{crit}}$. Substituting the [exponential function](calculus.md#exponential-function) $x=e^{rt}$ into the [viscous damping](#viscous-damping) model gives the [characteristic equation](differential-equation.md#characteristic-equation-of-a-constant-coefficient-differential-equation) and its [characteristic roots](differential-equation.md#characteristic-root-of-a-constant-coefficient-differential-equation):

$$
mr^2+br+k=0,\qquad r_\pm=-\zeta\omega_0\pm\omega_0\sqrt{\zeta^2-1}.
$$

For $0<\zeta<1$, [underdamping](#underdamping) gives a pair of [complex conjugate](complex-analysis.md#complex-conjugate) roots with negative [real part](complex-analysis.md#real-part). For $\zeta=1$, [critical damping](#critical-damping) gives the repeated negative real root. For $\zeta>1$, [overdamping](#overdamping) gives two distinct negative real roots. At $\zeta=0$ the roots are purely imaginary and the [harmonic oscillator](classical-mechanics.md#simple-harmonic-motion) is undamped; this boundary case has no [energy](classical-mechanics.md#energy) loss. With $m,k>0$, negative $b$ would inject [energy](classical-mechanics.md#energy) and lies outside the dissipative model.

<a id="image-characteristic-roots-of-an-ideal-viscous-oscillator-and-their-dimensionless-decay-rates-as-the-damping-ratio-varies"></a>
![](damped-oscillator-characteristic-root-paths.png)

**[Figure 4](#image-characteristic-roots-of-an-ideal-viscous-oscillator-and-their-dimensionless-decay-rates-as-the-damping-ratio-varies). Characteristic roots of an ideal viscous oscillator and their dimensionless decay rates as the damping ratio varies**.

The left panel locates $r/\omega_0$ in the [complex plane](complex-analysis.md#complex-plane); the [imaginary part](complex-analysis.md#imaginary-part) gives the damped [angular frequency](classical-mechanics.md#angular-frequency), while the negative [real part](complex-analysis.md#real-part) gives the [exponential decay](analysis.md#exponential-decay) rate. The right panel shows the positive rates $-\operatorname{Re}(r_\pm)/\omega_0$. Beyond [critical damping](#critical-damping), one root moves toward zero, explaining slow late motion for generic [initial conditions](differential-equation.md#initial-condition). The repeated-root solution also has a [polynomial](polynomial.md) prefactor, so these rates alone do not describe its complete response.

#### Oscillator energy dissipation

↑ **Parent:** [Viscous damping](#viscous-damping)

For the [damped harmonic oscillator](analysis.md#damped-harmonic-oscillator), the [mechanical energy](classical-mechanics.md#mechanical-energy) is the sum of [kinetic energy](classical-mechanics.md#kinetic-energy) and [spring](continuum-mechanics.md#spring) [potential energy](classical-mechanics.md#potential-energy):

$$
E=\frac12m\dot x^2+\frac12kx^2,\qquad
\frac{dE}{dt}=\dot x(m\ddot x+kx)=-b\dot x^2\leq0.
$$

Thus $b\dot x^2$ is the [power](classical-mechanics.md#power) transferred out of the oscillator's [mechanical energy](classical-mechanics.md#mechanical-energy). For $b>0$, the rate vanishes instantaneously at a turning point, despite nonzero stored [potential energy](classical-mechanics.md#potential-energy); it is not a constant loss per unit [time](classical-mechanics.md#time-in-physics). In [eddy-current damping](#eddy-current-damping) the loss becomes [Joule heating](electromagnetism.md#joule-heating). [Damped Harmonic Oscillation](physics-bibliography.md#oscillations-and-waves-by-richard-fitzpatrick/damped-harmonic-oscillation)

For an [underdamped](#underdamping) response, advancing one [oscillation period](classical-mechanics.md#period-of-an-oscillation) multiplies both [displacement](classical-mechanics.md#displacement) and [velocity](classical-mechanics.md#velocity) by $e^{-\zeta\omega_0T_{\mathrm d}}$, so $E(t+T_{\mathrm d})=e^{-2\zeta\omega_0T_{\mathrm d}}E(t)$. This exact cycle relation does not imply that instantaneous [energy](classical-mechanics.md#energy) is a pure [exponential function](calculus.md#exponential-function) throughout each cycle.

### Underdamping

↑ **Parent:** [Damping](#damping)

For $0<\zeta<1$, define the damped [angular frequency](classical-mechanics.md#angular-frequency) $\omega_{\mathrm d}=\omega_0\sqrt{1-\zeta^2}$. The [initial value problem](differential-equation.md#initial-value-problem) has solution

$$
x(t)=e^{-\zeta\omega_0t}\left[x_0\cos(\omega_{\mathrm d}t)+\frac{v_0+\zeta\omega_0x_0}{\omega_{\mathrm d}}\sin(\omega_{\mathrm d}t)\right].
$$

Every nonzero [underdamped](#underdamping) response crosses [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system) repeatedly. Its [oscillation period](classical-mechanics.md#period-of-an-oscillation) is $T_{\mathrm d}=2\pi/\omega_{\mathrm d}$, not $2\pi/\omega_0$. The [amplitude](physics.md#wave-amplitude) envelope decays as $e^{-\zeta\omega_0t}$, but the actual [displacement](classical-mechanics.md#displacement) also changes sign. The envelope coefficient need not equal $|x_0|$: initial [velocity](classical-mechanics.md#velocity) fixes the [oscillation phase](physics.md#phase-waves) as well as that coefficient.

### Overdamping

↑ **Parent:** [Damping](#damping)

For $\zeta>1$, let $r_+>r_-$ be the real [characteristic roots](differential-equation.md#characteristic-root-of-a-constant-coefficient-differential-equation). The response with the specified [initial conditions](differential-equation.md#initial-condition) is

$$
x(t)=C_+e^{r_+t}+C_-e^{r_-t},\qquad
C_+=\frac{v_0-r_-x_0}{r_+-r_-},\quad C_-=\frac{r_+x_0-v_0}{r_+-r_-}.
$$

The generic late response is governed by $r_+$, the root nearer zero. For very large [damping ratio](#damping-ratio), $r_+\sim-\omega_0/(2\zeta)=-k/b$: an increasingly strong brake delays the return to [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system). This approximation comes from balancing the [spring](continuum-mechanics.md#spring) and [viscous damping](#viscous-damping) terms after the fast transient. Choosing $v_0=r_-x_0$ makes $C_+=0$ and leaves only the faster root; that exception requires different initial [velocities](classical-mechanics.md#velocity) as $b$ varies.

### Damping measurement from free decay

↑ **Parent:** [Damping](#damping)

An experimentally useful question is whether the disappearing [oscillation](physics.md#oscillation) follows [viscous damping](#viscous-damping), and whether increasing the brake changes $b$ rather than $m$ or $k$. A published teaching protocol uses a cart on an [air track](#air-track), attached between two [springs](continuum-mechanics.md#spring), with ceramic magnets providing [eddy-current damping](#eddy-current-damping) and an [ultrasonic motion sensor](#ultrasonic-motion-sensor) recording [position](classical-mechanics.md#position) against [time](classical-mechanics.md#time-in-physics). Replace the magnets with equal [masses](classical-mechanics.md#mass) in the baseline trial so the moving [mass](classical-mechanics.md#mass) stays fixed. Obtain each [spring constant](continuum-mechanics.md#spring-constant) from the slope of applied [force](classical-mechanics.md#force) versus extension, then use $k=k_1+k_2$. Time many baseline cycles to check $\omega_0\simeq\sqrt{k/m}$. Compare one-magnet and two-magnet free decays; the protocol calls for a fit of the full trace including its offset. [Driven Harmonic Oscillator](physics-bibliography.md#driven-harmonic-oscillator)

The following additional controls make the inference testable. Level the [air track](#air-track) and hold its air supply fixed. Check the [ultrasonic motion sensor](#ultrasonic-motion-sensor) at several stationary flag positions against a ruler, including the full planned travel range; record the offset and scale correction. Check elapsed acquisition [time](classical-mechanics.md#time-in-physics) against an independent clock, and choose a [sampling rate](#sampling-rate) that resolves many samples within the shortest expected [oscillation period](classical-mechanics.md#period-of-an-oscillation). Record the resting [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system) before and after each run. Release the cart from a small measured [displacement](classical-mechanics.md#displacement) with minimal initial [velocity](classical-mechanics.md#velocity), with the driving apparatus inactive. Repeat at several release sizes and magnet settings while keeping the [springs](continuum-mechanics.md#spring) and total [mass](classical-mechanics.md#mass) unchanged. These are proposed calibration and repeatability checks, not reported measurements from the source.

For [underdamping](#underdamping), fit the recorded [position](classical-mechanics.md#position) to $y(t)=y_{\mathrm{eq}}+Ae^{-\alpha t}\cos(\omega_{\mathrm d}t+\phi)$ by [nonlinear regression](statistical-modelling.md#nonlinear-regression). The readout to inspect is a sequence of alternating extrema about $y_{\mathrm{eq}}$ with shrinking [amplitudes](physics.md#wave-amplitude), and the deviations of the fitted curve from the recorded points. The model predicts

$$
\alpha=\frac{b}{2m}=\zeta\omega_0,\qquad
\alpha^2+\omega_{\mathrm d}^2=\frac{k}{m}.
$$

Compare the right-hand side, determined independently from [mass](classical-mechanics.md#mass) and [spring constants](continuum-mechanics.md#spring-constant), with the fitted left-hand side. A good fit supports a constant-coefficient single [normal mode](#normal-mode) over the observed range; it does not establish a universal microscopic [force](classical-mechanics.md#force) law. The published protocol denotes the decay rate by $b$ and the [velocity](classical-mechanics.md#velocity)-proportional coefficient by $c$; here they are $\alpha$ and $b$, respectively.

At [critical damping](#critical-damping) or [overdamping](#overdamping), fit the corresponding nonoscillatory response including its offset and both [initial conditions](differential-equation.md#initial-condition), rather than forcing a damped cosine onto the data. Adjusting the brake can explore the transition, but the cited protocol does not establish that its one-magnet or two-magnet settings attain [critical damping](#critical-damping). A near-critical trace over a short interval can be hard to distinguish from neighbouring [damping ratios](#damping-ratio).

Important limitations are finite sensor range, missed or reflected [acoustic wave](fluid-mechanics.md#acoustic-wave) pulses, [measurement noise](probability-and-statistics.md#measurement-noise) near [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system), nonzero release [velocity](classical-mechanics.md#velocity), and position-dependent magnetic braking. Changing the release size tests for [quadratic drag](fluid-mechanics.md#quadratic-drag) or nonlinear [spring](continuum-mechanics.md#spring) response; inspecting deviations near turning points can expose [kinetic friction](classical-mechanics.md#kinetic-friction). Slow drift of the offset can imitate a long [overdamped](#overdamping) tail. Report uncertainties in fitted rates and independently measured $m,k$; absence of a visible crossing only bounds the behaviour within the instrument's sensitivity and recording interval. No numerical experimental results are asserted here.

#### Air track

↑ **Parent:** [Damping measurement from free decay](#damping-measurement-from-free-decay)

An [air track](#air-track) supports a cart on a cushion of air to reduce contact [friction](classical-mechanics.md#friction). It provides a nearly one-dimensional platform for a [damped harmonic oscillator](analysis.md#damped-harmonic-oscillator); residual [drag](fluid-mechanics.md#drag-physics) remains part of the baseline [damping](#damping).

#### Ultrasonic motion sensor

↑ **Parent:** [Damping measurement from free decay](#damping-measurement-from-free-decay)

An [ultrasonic motion sensor](#ultrasonic-motion-sensor) estimates distance from the return delay of an [acoustic wave](fluid-mechanics.md#acoustic-wave) pulse reflected by a target. The teaching setup places a flat flag on the cart facing the detector above the [air track](#air-track), and specifies a minimum range of about $0.3\,\mathrm m$ for its detector. That apparatus-specific limit should not be assumed for every sensor model. [Motion Sensor Setup](physics-bibliography.md#motion-sensor-setup)

#### Logarithmic decrement

↑ **Parent:** [Damping measurement from free decay](#damping-measurement-from-free-decay)

For [underdamping](#underdamping), let $x_n,x_{n+1}$ be successive same-sign extrema of [displacement](classical-mechanics.md#displacement) relative to [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system), one full [oscillation period](classical-mechanics.md#period-of-an-oscillation) apart. The [logarithmic decrement](#logarithmic-decrement) is

$$
\delta=\ln\frac{|x_n|}{|x_{n+1}|}=\alpha T_{\mathrm d}
=\frac{2\pi\zeta}{\sqrt{1-\zeta^2}},\qquad
\zeta=\frac{\delta}{\sqrt{4\pi^2+\delta^2}}.
$$

Comparing extrema $N$ full cycles apart instead gives $\delta=N^{-1}\ln(|x_n|/|x_{n+N}|)$. Adjacent extrema of opposite sign are only half a cycle apart and give half this decrement. This distinction matters when inferring a [damping ratio](#damping-ratio). Near [critical damping](#critical-damping), a full second same-sign extremum may be too small to resolve above [measurement noise](probability-and-statistics.md#measurement-noise); a full-trace fit with uncertainty is then more informative than a peak ratio.

### Eddy-current damping

↑ **Parent:** [Damping](#damping)

[Eddy-current damping](#eddy-current-damping) is [electromagnetic damping](physics.md#electromagnetic-damping) in which motion of an [electrical conductor](electromagnetism.md#electrical-conductor) through a [magnetic field](electromagnetism.md#magnetic-field) induces circulating [electric currents](electromagnetism.md#electric-current), producing an opposing [force](classical-mechanics.md#force) and [Joule heating](electromagnetism.md#joule-heating). In the cart experiment it approximates [viscous damping](#viscous-damping) over the fitted range; spatial variation of the [magnetic field](electromagnetism.md#magnetic-field) or changes in [velocity](classical-mechanics.md#velocity) can limit that approximation.

## Wave equation on a string

↑ **Parent:** [Wave equation](wave-equation.md)

An ideal uniform, flexible string under constant [tension](classical-mechanics.md#tension) $T>0$ has transverse displacement $y(x,t)$ satisfying

$$
\mu y_{tt}=Ty_{xx},\qquad c=\sqrt{\frac{T}{\mu}},
$$

where $\mu>0$ is [linear mass density](fluid-mechanics.md#linear-mass-density), meaning mass per unit length of the straight reference string. The approximation assumes small slope $|y_x|\ll1$, transverse motion, negligible bending stiffness, negligible [damping](#damping), and no distributed external force. Constant [tension](classical-mechanics.md#tension) and uniform [linear mass density](fluid-mechanics.md#linear-mass-density) make $c$ constant. Some texts use $\rho$ for this same [linear mass density](fluid-mechanics.md#linear-mass-density), giving $c=\sqrt{T/\rho}$; here $\rho$ must have units $\mathrm{kg\,m^{-1}}$, rather than units of volume [mass density](fluid-mechanics.md#density). [5 Wave Equation in R](physics-bibliography.md#math-220a-partial-differential-equations-of-applied-mathematics/5-wave-equation-in-r)

The units provide a useful check: $T/\mu$ has units $(\mathrm{kg\,m\,s^{-2}})/(\mathrm{kg\,m^{-1}})=\mathrm{m^2\,s^{-2}}$. For $T=100\,\mathrm N$ and $\mu=0.010\,\mathrm{kg\,m^{-1}}$, the [wave speed](#wave-speed) is $100\,\mathrm{m\,s^{-1}}$, so a pulse crosses a one-metre string in $0.010\,\mathrm s$. Quadrupling [tension](classical-mechanics.md#tension) doubles [wave speed](#wave-speed); quadrupling [linear mass density](fluid-mechanics.md#linear-mass-density) halves it. These square-root laws explain how material and loading set the time scale of the vibration.

For a length-$L$ string with fixed endpoints, the homogeneous [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition) are $y(0,t)=y(L,t)=0$. Its nonzero [normal modes](#normal-mode) have

$$
\phi_n(x)=\sin\frac{n\pi x}{L},\qquad
\omega_n=\frac{cn\pi}{L},\qquad
\nu_n=\frac{\omega_n}{2\pi}=\frac{cn}{2L},\qquad n=1,2,\ldots.
$$

Thus $cn\pi/L$ is an [angular frequency](classical-mechanics.md#angular-frequency), in radians per second, whereas $cn/(2L)$ is the [frequency](physics.md#frequency) in hertz. The [wavelength](#wavelength) is $2L/n$, and each [node of a standing wave](#node-physics) lies at $x=jL/n$ for some $j=0,\ldots,n$. For the numerical string above with $L=1\,\mathrm m$, the first three [frequencies](physics.md#frequency) are $50$, $100$ and $150\,\mathrm{Hz}$, with [angular frequencies](classical-mechanics.md#angular-frequency) $100\pi$, $200\pi$ and $300\pi\,\mathrm{s^{-1}}$. [Richard Fitzpatrick, Normal Modes of Uniform String](https://farside.ph.utexas.edu/teaching/315/Waveshtml/node28.html)

<a id="image-first-three-fixed-end-string-modes-showing-opposite-extrema-and-stationary-nodes"></a>
![](string-standing-modes.png)

**[Figure 5](#image-first-three-fixed-end-string-modes-showing-opposite-extrema-and-stationary-nodes). First three fixed-end string modes, showing opposite extrema and stationary nodes**.

Each [normal mode](#normal-mode) is a [standing wave](physics.md#standing-wave), but it also has a [travelling wave](analysis.md#travelling-wave) description:

$$
\sin(kx)\cos(ckt)=\frac12\sin(k(x-ct))+\frac12\sin(k(x+ct)).
$$

At a fixed endpoint an incident displacement pulse reflects with reversed sign, allowing incident and reflected displacements to cancel at the endpoint. [Periodic reflection for a fixed-end string](#periodic-reflection-for-a-fixed-end-string) implements both endpoints through odd, $2L$-periodic extensions of the initial data. This is the bridge between moving pulses and the stationary [Fourier sine basis](fourier-series.md#fourier-sine-basis). [MIT, Wave Propagation, Section 2.4](https://ocw.mit.edu/courses/2-062j-wave-propagation-spring-2017/9e6f7f49eea8381d72965b469e1a3fdf_MIT2_062J_S17_Chap2.pdf)

A short derivation comes from [Newton's second law](classical-mechanics.md#newton-s-second-law). The transverse force on a small segment is approximately $T[y_x(x+\delta x,t)-y_x(x,t)]$, and its mass is $\mu\delta x$. Dividing the force balance by $\delta x$ and taking the limit gives $\mu y_{tt}=Ty_{xx}$. [Separation of variables](partial-differential-equation.md#separation-of-variables) then gives $\phi''+k^2\phi=0$; the fixed-end [boundary conditions](differential-equation.md#boundary-condition) select $k=n\pi/L$, while the temporal equation is a [harmonic oscillator equation](classical-mechanics.md#simple-harmonic-motion) with $\omega=ck$.

### Impulsively struck fixed-end string

↑ **Parent:** [Wave equation on a string](#wave-equation-on-a-string)

For $0<\xi<l$, the [wave equation](wave-equation.md) $y_{tt}=c^2y_{xx}$ with zero endpoint displacement, zero initial displacement and initial velocity $\delta(x-\xi)$ has the [distributional weak solution](partial-differential-equation.md#weak-solution)

$$
y(x,t)=\frac{2}{\pi c}\sum_{n\ge1}\frac{\sin(n\pi\xi/l)\sin(n\pi x/l)\sin(n\pi ct/l)}{n}.
$$

Expand the [Dirac delta](distribution-theory.md#dirac-delta-function) in the [Fourier sine basis](fourier-series.md#fourier-sine-basis) and solve each modal [ordinary differential equation](differential-equation.md#ordinary-differential-equation). Equivalently take the odd, $2l$-periodic extension $v$ of the initial velocity and use $y=(2c)^{-1}\int_{x-ct}^{x+ct}v(s)\,ds$. The image impulses enforce the fixed endpoints. At jump fronts the [Fourier series](fourier-series.md) selects the midpoint of the two one-sided values.

### Modal energy of a localized velocity impulse on a string

↑ **Parent:** [Wave equation on a string](#wave-equation-on-a-string)

A fixed-end string of length $L$ initially straight receives velocity $v$ on an interval of width $a$ centred at $l$, and zero elsewhere. Its sine-mode velocity coefficient is $g_n=4v\sin(n\pi l/L)\sin(n\pi a/(2L))/(n\pi)$. For linear density $\rho$, orthogonality gives mode energy $E_n=\rho Lg_n^2/4$ and total energy $E=\rho av^2/2$. Their ratio is the displayed formula. Zeros in either sine factor suppress a [normal mode](#normal-mode) completely.

### Periodic reflection for a fixed-end string

↑ **Parent:** [Wave equation on a string](#wave-equation-on-a-string)

Zero values at both endpoints of a length-$L$ string allow the [D'Alembert formula](#d-alembert-s-formula) to be written with opposite travelling waves and a $2L$-periodic profile. This represents reflection with sign reversal at each fixed endpoint. For positive-time boundary conditions, periodicity concerns the arguments visited by the string solution; unused profile values can be defined by periodic extension.

### Linearly damped string

↑ **Parent:** [Wave equation on a string](#wave-equation-on-a-string)

With fixed endpoints, $y_{tt}-y_{xx}+y_t=0$ separates into sine modes whose amplitudes satisfy

$$
T_n''+T_n'+n^2\pi^2T_n=0.
$$

#### Velocity-impulse Green function for a damped string

↑ **Parent:** [Linearly damped string](#linearly-damped-string)

For $y_{tt}+2ky_t=c^2y_{xx}$ with fixed endpoints, initial displacement zero and initial velocity a [Dirac delta](distribution-theory.md#dirac-delta-function) at $a\in(0,l)$, the [Fourier sine series](fourier-series.md#fourier-sine-series) coefficient of that velocity is $2\sin(n\pi a/l)/l$. Each coefficient evolves by $T_n''+2kT_n'+(n\pi c/l)^2T_n=0$. Here $\omega_n^2=(n\pi c/l)^2-k^2$. At [critical damping](#critical-damping), replace $\sin(\omega_nt)/\omega_n$ by $t$; for an overdamped mode replace it by $\sinh(\sqrt{k^2-(n\pi c/l)^2}\,t)/\sqrt{k^2-(n\pi c/l)^2}$. The initial conditions hold in the sense of [distributions](distribution-theory.md#distribution-mathematical-analysis).

#### Separated solution of the damped string equation

↑ **Parent:** [Linearly damped string](#linearly-damped-string)

For initial sine coefficient $a_n$ and zero initial velocity, put $\omega_n^2=n^2\pi^2-1/4$. The modal amplitude is

$$
T_n(t)=a_ne^{-t/2}
\left(\cos(\omega_nt)+\frac{\sin(\omega_nt)}{2\omega_n}\right).
$$

#### Energy dissipation identity for a linearly damped string

↑ **Parent:** [Linearly damped string](#linearly-damped-string)

For fixed endpoints and

$$
E(t)=\frac12\int_0^1(y_t^2+y_x^2)\,dx,
$$

integration by parts and the damped wave equation give

$$
E'(t)=-\int_0^1y_t^2\,dx\leq0.
$$

## Normal mode

↑ **Parent:** [Wave equation](wave-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Normal_mode)

A normal mode, also called an [eigenmode](#normal-mode), is a pattern of free [oscillation](physics.md#oscillation) in a linear system whose relative displacements stay fixed while a single temporal factor changes their size and sign. For an undamped stable vibrational mode,

$$
u(x,t)=\phi(x)q(t),\qquad q(t)=A\cos(\omega t+\varphi).
$$

Here $\phi$ is the [mode shape](#mode-shape), $A$ sets the [amplitude](physics.md#wave-amplitude), $\omega$ is the [eigenfrequency](#eigenfrequency) expressed as an [angular frequency](classical-mechanics.md#angular-frequency), and $\varphi$ is the [oscillation phase](physics.md#phase-waves). Every snapshot is a [scalar multiple](vector-space.md#scalar-multiple) of the same [mode shape](#mode-shape); neighbouring regions may move in opposite directions. [Normal modes of a double pendulum](classical-mechanics.md#normal-modes-of-a-double-pendulum) show that [normal modes](#normal-mode) also describe coupled discrete systems, beyond strings. Their shapes are [eigenvectors](linear-operator-theory.md#eigenvector), rather than spatial [eigenfunctions](linear-operator-theory.md#eigenfunction). [Feynman, Leighton and Sands, The Feynman Lectures on Physics, Volume I, Chapter 49](https://www.feynmanlectures.caltech.edu/I_49.html)

For the ideal [wave equation on a string](#wave-equation-on-a-string), take a uniform string of length $L$ with constant [tension](classical-mechanics.md#tension) $\tau$ and [linear mass density](fluid-mechanics.md#linear-mass-density) $\mu$. Assume small transverse slope, negligible bending stiffness, no [damping](#damping), and fixed endpoints. Its [wave speed](#wave-speed) is $c=\sqrt{\tau/\mu}$, and the nonzero [normal modes](#normal-mode) are

$$
u_n(x,t)=A\sin\left(\frac{n\pi x}{L}\right)\cos(\omega_nt+\varphi),\qquad \omega_n=\frac{n\pi c}{L},\qquad f_n=\frac{\omega_n}{2\pi}=\frac{nc}{2L},\qquad n=1,2,3,\ldots.
$$

The [angular frequency](classical-mechanics.md#angular-frequency) $\omega_n$ is in radians per second; the [frequency](physics.md#frequency) $f_n$ is in hertz. The [wavelength](#wavelength) is $2L/n$. The [mode shape](#mode-shape) has $n$ loops separated by [nodes of a standing wave](#node-physics), including both fixed endpoints. [OpenStax, University Physics Volume 1, Section 16.6](https://openstax.org/books/university-physics-volume-1/pages/16-6-standing-waves-and-resonance)

As a worked example, choose $L=1\,\mathrm m$, $\tau=1\,\mathrm N$, and $\mu=1\,\mathrm{kg\,m^{-1}}$. Then $c=1\,\mathrm{m\,s^{-1}}$ and $f_1=0.5\,\mathrm{Hz}$, $f_2=1\,\mathrm{Hz}$, $f_3=1.5\,\mathrm{Hz}$. Their [oscillation periods](classical-mechanics.md#period-of-an-oscillation) are $T_1=2\,\mathrm s$, $T_2=1\,\mathrm s$, and $T_3=2/3\,\mathrm s$. These are deliberately simple model parameters, rather than measurements of a musical instrument. The plot divides [displacement](classical-mechanics.md#displacement) by $A$ so that the three [mode shapes](#mode-shape) can be compared, and uses each mode's own [oscillation period](classical-mechanics.md#period-of-an-oscillation) for its snapshots.

<a id="image-first-three-ideal-fixed-string-normal-modes-at-fractions-of-their-own-periods-black-dots-mark-permanent-nodes"></a>
![](standing-string-normal-modes.png)

**[Figure 6](#image-first-three-ideal-fixed-string-normal-modes-at-fractions-of-their-own-periods-black-dots-mark-permanent-nodes). First three ideal fixed-string normal modes at fractions of their own periods; black dots mark permanent nodes**.

For $\varphi=0$, at $t=T_n/4$ every point has zero [displacement](classical-mechanics.md#displacement), but most points have nonzero [velocity](classical-mechanics.md#velocity). Only zeros of the [mode shape](#mode-shape) are permanent [nodes of a standing wave](#node-physics). At $t=T_n/2$ the original [mode shape](#mode-shape) has reversed sign, and at $t=T_n$ it returns. The synchronized conversion between [kinetic energy](classical-mechanics.md#kinetic-energy) and [potential energy](classical-mechanics.md#potential-energy) is shown in [normal-mode energy exchange](#normal-mode-energy-exchange).

The short derivation uses [separation of variables](partial-differential-equation.md#separation-of-variables): substituting $u=\phi q$ into the [wave equation](wave-equation.md) gives $\phi''+k^2\phi=0$ and $q''+c^2k^2q=0$. The fixed-end [boundary conditions](differential-equation.md#boundary-condition) remove the cosine spatial term and require $\sin(kL)=0$, hence $k=n\pi/L$ and $\omega_n=ck$. Different geometries and [boundary conditions](differential-equation.md#boundary-condition) give different [eigenfunctions](linear-operator-theory.md#eigenfunction); a sine [mode shape](#mode-shape) is a property of this uniform fixed string, not a universal form of an [eigenmode](#normal-mode).

The usefulness is that a complicated vibration becomes a collection of [harmonic oscillators](classical-mechanics.md#simple-harmonic-motion). For sufficiently regular fixed-end initial data, the [Fourier sine series](fourier-series.md#fourier-sine-series) gives

$$
u(x,t)=\sum_{n=1}^{\infty}\sin\left(\frac{n\pi x}{L}\right)\left[a_n\cos(\omega_nt)+b_n\sin(\omega_nt)\right].
$$

The initial [displacement](classical-mechanics.md#displacement) and [velocity](classical-mechanics.md#velocity) determine $a_n$ and $b_n$. This is the [superposition principle](vector-space.md#superposition-principle) in a [Fourier sine basis](fourier-series.md#fourier-sine-basis), and [modal energy distribution](#modal-energy-distribution) measures how strongly each [normal mode](#normal-mode) is excited. The striking simplification is that each component keeps its identity while their sum can continually change shape. [Feynman, Leighton and Sands, The Feynman Lectures on Physics, Volume I, Section 50-2](https://www.feynmanlectures.caltech.edu/I_50.html)

These independent [normal modes](#normal-mode) belong to the linear model. At larger slopes, changing [tension](classical-mechanics.md#tension) introduces nonlinear effects and can couple the modes. A [linearly damped string](#linearly-damped-string) still admits a [Fourier sine basis](fourier-series.md#fourier-sine-basis), but its temporal factors decay and need not oscillate; its [energy dissipation identity for a linearly damped string](#energy-dissipation-identity-for-a-linearly-damped-string) replaces [conservation of energy](physics.md#conservation-of-energy). More general [damping](#damping) need not leave undamped [mode shapes](#mode-shape) independent.

### Mode shape

↑ **Parent:** [Normal mode](#normal-mode)

The mode shape is the fixed spatial [eigenfunction](linear-operator-theory.md#eigenfunction) multiplying the temporal factor of a [normal mode](#normal-mode). It is determined by the governing [differential equation](differential-equation.md) and [boundary conditions](differential-equation.md#boundary-condition), and may be normalized by a chosen amplitude or energy convention.

### Countability of elastic eigenfrequencies

↑ **Parent:** [Normal mode](#normal-mode)

Distinct squared traction-free [eigenfrequencies](#eigenfrequency) in a bounded lossless elastic body have [eigenfunctions](linear-operator-theory.md#eigenfunction) [orthogonal](linear-algebra.md#orthogonal-vectors) in $L^2(\mathcal D,\rho\,dV)^3$, by the [Betti identity for elastodynamic fields](continuum-mechanics.md#betti-identity-for-elastodynamic-fields). Normalize one field from each [eigenspace](linear-operator-theory.md#eigenspace). This is an [orthonormal set](linear-algebra.md#orthonormal-set) in a [separable Hilbert space](hilbert-space.md#separable-hilbert-space), so it is countable: disjoint balls of radius less than $1/\sqrt2$ around its unit vectors must contain distinct points of a countable dense set. Positive and negative [frequency](physics.md#frequency) partners add at most a factor of two. This argument proves countability without requiring a separate compact-resolvent proof.

### Eigenfrequency

↑ **Parent:** [Normal mode](#normal-mode)

An eigenfrequency is the natural [frequency](physics.md#frequency) associated with a free [normal mode](#normal-mode). Always specify whether it means the [angular frequency](classical-mechanics.md#angular-frequency) $\omega$ or the [frequency](physics.md#frequency) $f=\omega/(2\pi)$ in hertz. For a uniform fixed-end [wave equation on a string](#wave-equation-on-a-string), $\omega_n=n\pi\sqrt{\tau/\mu}/L$ and $f_n=n\sqrt{\tau/\mu}/(2L)$; the [amplitude](physics.md#wave-amplitude) does not change either within the linear model. In a [generalized eigenvalue problem for small oscillations](classical-mechanics.md#generalized-eigenvalue-problem-for-small-oscillations), the [eigenvalue](linear-operator-theory.md#eigenvalue) is $\omega^2$, rather than $\omega$ itself.

For a first-order system $\dot z=iAz$, a real [eigenvalue](linear-operator-theory.md#eigenvalue) $\lambda$ of $A$ instead gives a signed eigenfrequency in $e^{i\lambda t}$. A positive imaginary part of $\lambda$ gives exponential decay with this sign convention. Thus a complex damped eigenfrequency encodes both [oscillation](physics.md#oscillation) and decay; it is not just the number of cycles per second.

### Modal energy distribution

↑ **Parent:** [Normal mode](#normal-mode)

[Orthogonality](linear-algebra.md#orthogonal-vectors) separates total quadratic [wave energy](#wave-energy) into a sum of independent modal energies.

### Normal-mode energy exchange

↑ **Parent:** [Normal mode](#normal-mode)

For the undamped first [normal mode](#normal-mode) of a fixed string, start at maximum [displacement](classical-mechanics.md#displacement) with $u(x,t)=A\sin(\pi x/L)\cos(\omega_1t)$. In the small-slope [wave equation on a string](#wave-equation-on-a-string), its [kinetic energy](classical-mechanics.md#kinetic-energy) and excess [potential energy](classical-mechanics.md#potential-energy) are

$$
\mathrm{KE}(t)=\frac{\mu}{2}\int_0^L u_t^2\,dx,\qquad \mathrm{PE}(t)=\frac{\tau}{2}\int_0^L u_x^2\,dx.
$$

The [potential energy](classical-mechanics.md#potential-energy) comes from the extra length under [tension](classical-mechanics.md#tension): $\sqrt{1+u_x^2}-1\simeq u_x^2/2$. It depends on slope, so a [node of a standing wave](#node-physics) need not have zero local [potential energy](classical-mechanics.md#potential-energy) density. These are physical [energies](classical-mechanics.md#energy), with the mass and [tension](classical-mechanics.md#tension) factors restored to the normalized [wave energy](#wave-energy). [Richard Fitzpatrick, Oscillations and Waves, Energy Conservation, equations 6.24-6.29](https://farside.ph.utexas.edu/teaching/315/Waveshtml/node43.html)

Integrating $\sin^2(\pi x/L)$ and $\cos^2(\pi x/L)$ over the string gives $L/2$ in both cases. Using $\mu\omega_1^2=\tau\pi^2/L^2$ yields

$$
E=\frac{\tau A^2\pi^2}{4L},\qquad \mathrm{KE}(t)=E\sin^2(\omega_1t),\qquad \mathrm{PE}(t)=E\cos^2(\omega_1t),\qquad \mathrm{KE}+\mathrm{PE}=E.
$$

For the model $\mu=1\,\mathrm{kg\,m^{-1}}$, $\tau=1\,\mathrm N$, $L=1\,\mathrm m$, and $A=0.010\,\mathrm m$, the [angular frequency](classical-mechanics.md#angular-frequency) is $\omega_1=\pi\,\mathrm{rad\,s^{-1}}$, the [frequency](physics.md#frequency) is $0.5\,\mathrm{Hz}$, and $E\simeq2.4674\times10^{-4}\,\mathrm J$. The maximum slope $A\pi/L\simeq0.0314$ is small. At $t=0$ all the [energy](classical-mechanics.md#energy) is [potential energy](classical-mechanics.md#potential-energy); at $t=T_1/4=0.5\,\mathrm s$ the string is straight and all the [energy](classical-mechanics.md#energy) is [kinetic energy](classical-mechanics.md#kinetic-energy). At $t=T_1/2=1\,\mathrm s$ the [displacement](classical-mechanics.md#displacement) is reversed and all the [energy](classical-mechanics.md#energy) is again [potential energy](classical-mechanics.md#potential-energy). The energy curves repeat twice during one [displacement](classical-mechanics.md#displacement) cycle, while [conservation of energy](physics.md#conservation-of-energy) keeps their sum constant.

<a id="image-first-mode-displacement-in-metres-and-kinetic-and-potential-energies-divided-by-the-conserved-total-energy"></a>
![](normal-mode-energy-exchange.png)

**[Figure 7](#image-first-mode-displacement-in-metres-and-kinetic-and-potential-energies-divided-by-the-conserved-total-energy). First-mode displacement in metres and kinetic and potential energies divided by the conserved total energy**.

### Node (physics)

↑ **Parent:** [Normal mode](#normal-mode)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Node_(physics))

A node of an ideal [standing wave](physics.md#standing-wave) is a position whose oscillation [amplitude](physics.md#wave-amplitude) is zero: its [displacement](classical-mechanics.md#displacement) stays zero for all time. For a nontrivial [normal mode](#normal-mode) $u(x,t)=\phi(x)q(t)$, this means $\phi(x)=0$. A momentary zero caused by $q(t)=0$ does not make every position a node. In more dimensions the zeros of a [mode shape](#mode-shape) can form curves or surfaces.

For the $n$th [normal mode](#normal-mode) of a uniform fixed-end [wave equation on a string](#wave-equation-on-a-string), the [nodes of a standing wave](#node-physics) are

$$
x_j=\frac{jL}{n},\qquad j=0,1,\ldots,n.
$$

There are $n+1$ [nodes of a standing wave](#node-physics) including the two endpoints, and $n-1$ interior ones. For $n=3$ and $L=1\,\mathrm m$, they lie at $0$, $1/3$, $2/3$, and $1\,\mathrm m$. Each remains stationary through every snapshot in the [normal mode](#normal-mode) diagram; an [antinode](#antinode) instead marks a maximum oscillation [amplitude](physics.md#wave-amplitude). [OpenStax, University Physics Volume 1, Section 16.6](https://openstax.org/books/university-physics-volume-1/pages/16-6-standing-waves-and-resonance)

### Antinode

↑ **Parent:** [Normal mode](#normal-mode)

An antinode is a position of maximum oscillation [amplitude](physics.md#wave-amplitude) in a [standing wave](physics.md#standing-wave). For $u_n=A\sin(n\pi x/L)\cos(\omega_nt+\varphi)$, the [antinodes](#antinode) occur at

$$
x_j=\frac{(2j+1)L}{2n},\qquad j=0,1,\ldots,n-1,
$$

where the [amplitude](physics.md#wave-amplitude) is $|A|$. They sit halfway between consecutive [nodes of a standing wave](#node-physics). For the first [normal mode](#normal-mode), the sole [antinode](#antinode) is $x=L/2$. It reaches zero [displacement](classical-mechanics.md#displacement) at a quarter [oscillation period](classical-mechanics.md#period-of-an-oscillation) while moving fastest, which illustrates why an [antinode](#antinode) is defined by oscillation [amplitude](physics.md#wave-amplitude) rather than instantaneous height.

## Fourier transform method for the wave equation

↑ **Parent:** [Wave equation](wave-equation.md)

Fourier transformation in space turns $u_{tt}=c^2u_{xx}$ into the independent oscillators $\widehat u_{tt}+c^2k^2\widehat u=0$.

### Low-frequency decomposition of the wave propagator

↑ **Parent:** [Fourier transform method for the wave equation](#fourier-transform-method-for-the-wave-equation)

For zero initial displacement and unit delta initial velocity, the spatial [Fourier transform](analysis.md#fourier-transform) of the [wave equation](wave-equation.md) gives the displayed multiplier. A compact [cutoff function](distribution-theory.md#cutoff-function) around zero frequency produces an ordinary smooth function after inversion. The remaining sine splits into two [oscillatory integrals](distribution-theory.md#oscillatory-integral) with phases $x\cdot\xi\pm ct|\xi|$ and symbols proportional to $(1-\chi)/|\xi|$ of order $-1$. Their stationary directions lie on $|x|=c|t|$, proving a light-cone bound for [singular support](distribution-theory.md#singular-support). This does not claim vanishing of smooth tails inside the cone.

### Entire wave cosine multiplier

↑ **Parent:** [Fourier transform method for the wave equation](#fourier-transform-method-for-the-wave-equation)

For real wave speed $c$ and $t\ge0$, define the complex-frequency cosine through the entire series $C_t(z)=\sum_{j\ge0}(-1)^j(ct)^{2j}(z\cdot z)^j/(2j)!$. The expression is independent of the square-root branch even though the square root itself need not be entire. Writing $z=a+ib$ gives $|\operatorname{Im}\sqrt{z\cdot z}|\le|b|$, and hence $|C_t(z)|\le e^{|c|t|\operatorname{Im}z|}$. The [Paley–Wiener–Schwartz theorem](distribution-theory.md#paley-wiener-schwartz-theorem) therefore makes its inverse [Fourier transform](analysis.md#fourier-transform) a [distribution](distribution-theory.md#distribution-mathematical-analysis) supported in the radius-$|c|t$ ball. Multiplication by $C_t$ evolves initial displacement with zero initial velocity in the [wave equation](wave-equation.md), giving [finite propagation speed](#finite-propagation-speed) for compactly supported initial [distributions](distribution-theory.md#distribution-mathematical-analysis).

<h2 id="d-alembert-s-formula">D'Alembert's formula</h2>

↑ **Parent:** [Wave equation](wave-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/D'Alembert's_formula)

For constant [wave speed](#wave-speed) $c>0$, the whole-line [Cauchy problem](partial-differential-equation.md#cauchy-problem)

$$
u_{tt}=c^2u_{xx},\qquad u(x,0)=f(x),\qquad u_t(x,0)=g(x)
$$

has the unique [classical solution](partial-differential-equation.md#classical-solution), for $f\in C^2(\mathbb R)$ and $g\in C^1(\mathbb R)$,

$$
u(x,t)=\frac{f(x-ct)+f(x+ct)}2+\frac1{2c}\int_{x-ct}^{x+ct}g(s)\,ds.
$$

The first term evolves displacement released from rest; the second evolves initial [velocity](classical-mechanics.md#velocity). The factor $1/(2c)$ converts an integral of [velocity](classical-mechanics.md#velocity) over distance into displacement. On a finite string the formula applies before the backward [characteristic curves](partial-differential-equation.md#characteristic-curve) reach an endpoint, or globally after an extension that enforces the [boundary conditions](differential-equation.md#boundary-condition). [5 Wave Equation in R](physics-bibliography.md#math-220a-partial-differential-equations-of-applied-mathematics/5-wave-equation-in-r)

For a completely smooth example, choose a [bump function](analysis.md#bump-function) with [compact support](function.md#compact-support):

$$
b(z)=\begin{cases}\exp\!\left(1-\frac1{1-z^2}\right),&|z|<1,\\0,&|z|\geq1,\end{cases}
\qquad f(x)=A b(x/a),\qquad g(x)=0,
$$

where $a>0$ sets the half-width and $A$ sets the initial peak. Then

$$
u(x,t)=\frac A2 b\!\left(\frac{x-ct}{a}\right)+\frac A2 b\!\left(\frac{x+ct}{a}\right).
$$

At $t=0$ the two copies coincide, recovering peak $A$. At $t=a/(2c)$, $u(0,t)=A e^{-1/3}\simeq0.716531A$. At $t=3a/(2c)$ the pulses are separated, centred at $x=\pm3a/2$, each of width $2a$ and peak $A/2$. Zero initial [velocity](classical-mechanics.md#velocity) forces equal left and right contributions; a purely right-moving initial profile instead requires $g=-cf'$. Thus “released from rest” and “launched to the right” describe different [Cauchy data](partial-differential-equation.md#cauchy-data).

<a id="image-a-smooth-pulse-released-from-rest-splits-in-two-while-backward-characteristics-select-a-causal-interval"></a>
![](wave-pulse-propagation.png)

**[Figure 8](#image-a-smooth-pulse-released-from-rest-splits-in-two-while-backward-characteristics-select-a-causal-interval). A smooth pulse released from rest splits in two, while backward characteristics select a causal interval**.

The [domain of dependence](partial-differential-equation.md#domain-of-dependence) of $(x_*,t_*)$, for $t_*\geq0$, is contained in $[x_*-ct_*,x_*+ct_*]$ on the initial line. More precisely, displacement contributes only through the two endpoints, while initial [velocity](classical-mechanics.md#velocity) contributes throughout the interval. With $c=1$, $x_*=0.5$ and $t_*=1.5$, that interval is $[-1,2]$. Changing either initial datum outside it cannot change $u(0.5,1.5)$. If both initial data vanish outside $[-a,a]$, the solution vanishes outside $[-a-ct,a+ct]$: this is [finite propagation speed](#finite-propagation-speed). The expanding interval bounds possible influence; it need not be filled by nonzero displacement, as the separated bumps demonstrate.

Historically, d'Alembert studied the vibrating-string problem in “Recherches sur la courbe que forme une corde tendue mise en vibration”, in the Berlin Academy's volume for the year 1747, pages 214–219. The memoir introduces the differential equation and integrates it through two arbitrary one-variable functions. The original geometric problem makes the formula's enduring appeal clear: arbitrary initial shapes can be handled without first decomposing them into [normal modes](#normal-mode). [D'Alembert, vibrating-string memoir, Academy year 1747](https://webusers.imj-prg.fr/~david.aubin/cours/Textes/Dalembert-HAB-1747-cordes-vibrantes.pdf)

For a brief derivation, use [characteristic coordinates](partial-differential-equation.md#characteristic-coordinate) $\xi=x-ct$ and $\eta=x+ct$. The [chain rule](calculus.md#chain-rule) gives $u_{tt}-c^2u_{xx}=-4c^2u_{\xi\eta}$, so $u=F(\xi)+G(\eta)$. The initial conditions yield $F+G=f$ and $-cF'+cG'=g$. Integrating these relations gives the displayed formula; the arbitrary integration constants cancel in their sum.

### Rectangular pulse splitting under the wave equation

↑ **Parent:** [D'Alembert's formula](#d-alembert-s-formula)

A rectangular initial displacement with zero initial velocity splits into two equal half-height copies moving in opposite directions. The [D'Alembert formula](#d-alembert-s-formula) reads $u(x,t)=[u_0(x+ct)+u_0(x-ct)]/2$. Overlap adds the heights; separated copies each retain the original width. For discontinuous fronts the formula defines a [weak solution](partial-differential-equation.md#weak-solution) of the [wave equation](wave-equation.md).

<h3 id="d-alembert-formula-with-initial-velocity">D'Alembert formula with initial velocity</h3>

↑ **Parent:** [D'Alembert's formula](#d-alembert-s-formula)

For the [wave equation](wave-equation.md) $u_{tt}=c^2u_{xx}$ with zero initial displacement and initial [velocity](classical-mechanics.md#velocity) $g$, [D'Alembert's formula](#d-alembert-s-formula) becomes

$$
u(x,t)=\frac1{2c}\int_{x-ct}^{x+ct}g(s)\,ds.
$$

For $c=1$ this is the original speed-one form $u(t,x)=\tfrac12\int_{x-t}^{x+t}f(s)\,ds$ when the initial [velocity](classical-mechanics.md#velocity) is named $f$. The integral records the total initial kick inside the [domain of dependence](partial-differential-equation.md#domain-of-dependence).

For a computed example, set $g(x)=V$ on $[-a,a]$ and zero elsewhere, with $V>0$. This discontinuous datum gives a [weak solution](partial-differential-equation.md#weak-solution):

$$
u(x,t)=\frac{V}{2c}\,\operatorname{length}\bigl([x-ct,x+ct]\cap[-a,a]\bigr),\qquad t\geq0.
$$

At the centre, $u(0,t)=V\min(t,a/c)$. For $a=1\,\mathrm m$, $c=2\,\mathrm{m\,s^{-1}}$ and $V=0.4\,\mathrm{m\,s^{-1}}$, this is $0.1\,\mathrm m$ at $t=0.25\,\mathrm s$ and $0.2\,\mathrm m$ at $t=1\,\mathrm s$. Once $ct>a$, a central plateau $u=Va/c$ occupies $|x|\leq ct-a$. In contrast, [central zero region for odd compactly supported initial velocity](#central-zero-region-for-odd-compactly-supported-initial-velocity) follows when the full integral of $g$ vanishes. [Finite propagation speed](#finite-propagation-speed) permits an interior tail; it does not imply the [Strong Huygens principle](#strong-huygens-principle).

#### Central zero region for odd compactly supported initial velocity

↑ **Parent:** [D'Alembert formula with initial velocity](#d-alembert-formula-with-initial-velocity)

If $u(x,0)=0$, $u_t(x,0)=g(x)$, and the odd function $g$ is supported on $[-a,a]$, then

$$
u(x,t)=0
\qquad\text{whenever }t>a\text{ and }|x|\leq t-a.
$$

The interval $[x-t,x+t]$ then contains the entire support, whose integral vanishes by oddness.

## Wavenumber

↑ **Parent:** [Wave equation](wave-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wavenumber)

A [wavenumber](#wavenumber) measures how rapidly a [wave phase](physics.md#phase-waves) changes with distance. Two conventions coexist: angular [wavenumber](#wavenumber) counts [radians](geometry-and-topology.md#radian) per unit length, while ordinary [spatial frequency](fourier-analysis.md#spatial-frequency) counts cycles per unit length. For a [monochromatic wave](physics.md#monochromatic-wave) with [wavelength](#wavelength) $\lambda>0$,

$$
K=\frac{2\pi}{\lambda},\qquad \nu_x=\frac1\lambda,\qquad K=2\pi\nu_x.
$$

Here $K\geq0$ is the magnitude of the angular [wavenumber](#wavenumber). The symbol $k$ can instead denote a signed one-dimensional angular [wavenumber](#wavenumber): a factor $e^{ikx}$ has [wavelength](#wavelength) $2\pi/|k|$ for real $k\ne0$. Both conventions have dimensions of inverse length; writing $\mathrm{rad\,m^{-1}}$ or “cycles per metre” exposes the convention. A quoted value in $\mathrm{m^{-1}}$ alone does not resolve the factor of $2\pi$. [Spectroscopic wavenumber](#spectroscopic-wavenumber) usually uses the cycles-per-length convention.[section 16.2, equations 16.2–16.5: angular convention and sinusoidal wave phase](physics-bibliography.md#university-physics-volume-1-by-william-moebs-and-others)

For a real [monochromatic](ramsey-theory.md#monochromatic-set) [plane wave](quantum-mechanics.md#plane-wave), fix the convention

$$
u(\mathbf x,t)=A\cos\phi(\mathbf x,t),\qquad \phi=\mathbf k\cdot\mathbf x-\omega t+\phi_0,\qquad K=|\mathbf k|.
$$

The [wavevector](continuum-mechanics.md#wavevector) $\mathbf k$ supplies both the spatial [wave phase](physics.md#phase-waves) slope and the normal to the [wavefronts](optics.md#wavefront); its [dot product](linear-algebra.md#dot-product) with position makes the [wave phase](physics.md#phase-waves) constant on parallel planes. The [angular frequency](classical-mechanics.md#angular-frequency) is $\omega=2\pi f$, with $f>0$ the ordinary [frequency](physics.md#frequency). Moving a distance $\lambda$ along $\mathbf k$ changes the [wave phase](physics.md#phase-waves) by $2\pi$. Holding a [wave crest](#wave-crest)'s [wave phase](physics.md#phase-waves) fixed gives its [phase velocity](#phase-velocity) $\omega\mathbf k/K^2$ and [phase speed](#phase-speed)

$$
v_p=\frac{\omega}{K}=f\lambda.
$$

In one dimension the signed [phase velocity](#phase-velocity) is $\omega/k$. This identifies a moving pattern; it does not identify the motion of the medium's particles or a [wave packet](#wave-packet)'s [group velocity](#group-velocity).

For the synthetic [plane wave](quantum-mechanics.md#plane-wave) below, choose $\lambda=0.40\,\mathrm m$ and $f=5\,\mathrm{Hz}$. Then $K=5\pi\,\mathrm{rad\,m^{-1}}$, $\nu_x=2.5$ cycles per metre, $\omega=10\pi\,\mathrm{rad\,s^{-1}}$, and $v_p=2\,\mathrm{m\,s^{-1}}$. The [wave crests](#wave-crest) are $0.40\,\mathrm m$ apart at one instant; after a quarter [oscillation period](classical-mechanics.md#period-of-an-oscillation), each has advanced $0.10\,\mathrm m$. The lower panel retains whole turns of [wave phase](physics.md#phase-waves), making its slope visible instead of reducing it modulo $2\pi$.

<a id="image-synthetic-plane-wave-snapshots-crest-spacing-phase-slope-and-a-quarter-period-advance"></a>
![](wavenumber-phase-crest-distance.png)

**[Figure 9](#image-synthetic-plane-wave-snapshots-crest-spacing-phase-slope-and-a-quarter-period-advance). Synthetic plane-wave snapshots: crest spacing, phase slope, and a quarter-period advance**.

### Spectroscopic wavenumber

↑ **Parent:** [Wavenumber](#wavenumber)

A [spectroscopic wavenumber](#spectroscopic-wavenumber) commonly means the reciprocal of the vacuum [wavelength](#wavelength) $\lambda_0$ of [electromagnetic radiation](electromagnetism.md#electromagnetic-radiation), often in $\mathrm{cm^{-1}}$. It is an ordinary [spatial frequency](fourier-analysis.md#spatial-frequency), so the vacuum angular [wavenumber](#wavenumber) is $K_0=2\pi\tilde\nu$. Specify vacuum or in-medium [wavelength](#wavelength): the same [frequency](physics.md#frequency) can have different [wavelengths](#wavelength) in different media. IUPAC's “wavenumber in medium” entry defines the in-medium reciprocal $1/\lambda$ and notes that unqualified spectroscopic usage often means the vacuum reciprocal.[wavenumber in medium](physics-bibliography.md#wavenumber-in-medium)

For example, a vacuum [wavelength](#wavelength) of $500\,\mathrm{nm}=5\times10^{-5}\,\mathrm{cm}$ corresponds to $\tilde\nu=20000\,\mathrm{cm^{-1}}=2\times10^6\,\mathrm{m^{-1}}$. Multiplication by $2\pi$ gives $K_0=4\pi\times10^6\,\mathrm{rad\,m^{-1}}$. Converting centimetres to metres and converting cycles to [radians](geometry-and-topology.md#radian) are separate operations.

### Spatial sampling of a wave

↑ **Parent:** [Wavenumber](#wavenumber)

In [spatial sampling of a wave](#spatial-sampling-of-a-wave), a detector records a [wave](physics.md#wave) at positions $x_n=np$ separated by pitch $p>0$. Angular [wavenumbers](#wavenumber) differing by $2\pi m/p$, with [integers](number-theory.md#integer) $m$, give identical samples of a complex [Fourier mode](fourier-analysis.md#fourier-mode):

$$
e^{i(k+2\pi m/p)np}=e^{iknp}.
$$

This is spatial [aliasing](fourier-analysis.md#aliasing). To distinguish arbitrary [sinusoids](geometry-and-topology.md#sinusoid) within a prescribed band, require $|k|<\pi/p$, equivalently $|\nu_x|<1/(2p)$, the [Nyquist spatial frequency](fourier-analysis.md#nyquist-spatial-frequency). Thus $p<\lambda_{\min}/2$ for the shortest allowed [wavelength](#wavelength). At equality a [sine](geometry-and-topology.md#sine) can vanish at every sample, so phase information can be lost. The [Nyquist–Shannon sampling theorem](fourier-analysis.md#nyquist-shannon-sampling-theorem) states the precise reconstruction conditions for a [bandlimited function](analysis.md#bandlimited-function); a finite scan introduces further limitations.

The synthetic two-tone snapshot is

$$
\frac{u(x)}A=\cos(2\pi\nu_1x)+\frac12\cos(2\pi\nu_2x),\qquad \nu_1=2\,\mathrm{m^{-1}},\quad \nu_2=8\,\mathrm{m^{-1}},
$$

where both $\nu_j$ count cycles per metre. The component [wavelengths](#wavelength) are $0.50\,\mathrm m$ and $0.125\,\mathrm m$. With $p=0.05\,\mathrm m$, both lie below the [Nyquist spatial frequency](fourier-analysis.md#nyquist-spatial-frequency) of $10$ cycles per metre. With $p=0.10\,\mathrm m$, the $8$-cycle component aliases to the $2$-cycle component: at every $x_n=n/10$, $\cos(2\pi\cdot8x_n)=\cos(2\pi\cdot2x_n)$. The sampled sum is therefore indistinguishable from $1.5\cos(4\pi x)$, although the continuous curves differ between samples. Drawing lines between sample points cannot resolve this ambiguity.

<a id="image-synthetic-two-tone-spatial-waveform-fine-samples-distinguish-the-components-coarse-samples-hide-the-shorter-wavelength"></a>
![](two-tone-spatial-sampling.png)

**[Figure 10](#image-synthetic-two-tone-spatial-waveform-fine-samples-distinguish-the-components-coarse-samples-hide-the-shorter-wavelength). Synthetic two-tone spatial waveform: fine samples distinguish the components, coarse samples hide the shorter wavelength**.

### Wavelength

↑ **Parent:** [Wavenumber](#wavenumber)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wavelength)

The [wavelength](#wavelength) $\lambda$ is the spatial [period](mathematics.md#period-of-a-function) of a [monochromatic wave](physics.md#monochromatic-wave), measured at a fixed time along the [wavevector](continuum-mechanics.md#wavevector). For a [plane wave](quantum-mechanics.md#plane-wave) with a [sinusoid](geometry-and-topology.md#sinusoid) as its profile, it is the distance between consecutive [wave crests](#wave-crest), or between any consecutive points with the same [wave phase](physics.md#phase-waves) modulo $2\pi$:

$$
\lambda=\frac{2\pi}{|\mathbf k|}=\frac{v_p}{f}.
$$

Here $\mathbf k$ uses angular [wavenumber](#wavenumber), $f$ is ordinary [frequency](physics.md#frequency), and $v_p$ is [phase speed](#phase-speed). A distance between arbitrary zero crossings need not be a [wavelength](#wavelength): consecutive zeros of a [sinusoid](geometry-and-topology.md#sinusoid) are only $\lambda/2$ apart, with opposite slopes. In a [standing wave](physics.md#standing-wave), consecutive [nodes of a standing wave](#node-physics) are also $\lambda/2$ apart; $\lambda$ refers to the constituent [travelling waves](analysis.md#travelling-wave), even though the [nodes of a standing wave](#node-physics) do not travel.

Across a stationary interface between stationary linear media, the incident, reflected and transmitted [monochromatic waves](physics.md#monochromatic-wave) have the same [frequency](physics.md#frequency). The [boundary conditions](differential-equation.md#boundary-condition) must hold at every time: terms oscillating with different [angular frequencies](classical-mechanics.md#angular-frequency) cannot cancel throughout the entire time record. Each medium's [dispersion relation](#dispersion-relation) then determines its own angular [wavenumber](#wavenumber) and [wavelength](#wavelength), so

$$
f_1=f_2,\qquad \frac{\lambda_2}{\lambda_1}=\frac{v_{p,2}}{v_{p,1}}.
$$

For [electromagnetic radiation](electromagnetism.md#electromagnetic-radiation) in a transparent medium with [refractive index](electromagnetism.md#refractive-index) $n$, $v_p=c_0/n$ and $\lambda=\lambda_0/n$, where $c_0$ is the vacuum [speed of light](special-relativity.md#speed-of-light). A synthetic example with $\lambda_0=600\,\mathrm{nm}$ and $n=1.5$ gives $\lambda=400\,\mathrm{nm}$ at the same [frequency](physics.md#frequency). This conservation argument assumes time-independent linear material response and a stationary interface in the chosen frame. A moving interface can produce a [Doppler effect](physics.md#doppler-effect); time-dependent or nonlinear response can change or generate [frequencies](physics.md#frequency).[27.1 The Wave Aspect of Light: Interference](physics-bibliography.md#college-physics-by-paul-peter-urone-and-others/27-1-the-wave-aspect-of-light-interference)

A broad [frequency spectrum](fourier-analysis.md#frequency-spectrum) generally supplies many component [wavelengths](#wavelength), rather than one [wavelength](#wavelength) for an entire pulse. Even two tones have both their individual [wavelengths](#wavelength) and a different overall repetition distance: the $2$- and $8$-cycle-per-metre sum in [spatial sampling of a wave](#spatial-sampling-of-a-wave) repeats after $0.50\,\mathrm m$, but contains the finer $0.125\,\mathrm m$ structure. A narrow [wave packet](#wave-packet) can have an approximate carrier [wavelength](#wavelength); the [wave envelope](#envelope-waves) propagates approximately at [group velocity](#group-velocity), determined by the slope of the [dispersion relation](#dispersion-relation). Substituting that [group velocity](#group-velocity) into $\lambda=v_p/f$ generally gives the wrong carrier [wavelength](#wavelength). Where the medium varies slowly, [local wavelength](#local-wavelength) gives a more useful description.

#### Acoustic wavelength measurement

↑ **Parent:** [Wavelength](#wavelength)

An [acoustic wavelength measurement](#acoustic-wavelength-measurement) makes an invisible spatial pattern readable with a ruler. The authored guide [Interesting and inexpensive experiments for high school physics by Joe Wolfe](physics-bibliography.md#interesting-and-inexpensive-experiments-for-high-school-physics-by-joe-wolfe) places a loudspeaker near a pipe's open end, drives it with an oscillator, and slides a [microphone](#microphone) attached to a metre rule through the pipe. An [oscilloscope](#oscilloscope) or computer displays the [microphone](#microphone) [signal](electrical-engineering.md#signal). Its oscillation [amplitude](physics.md#wave-amplitude) rises and falls with position; adjacent minima locate [pressure](thermodynamics.md#pressure) [nodes of a standing wave](#node-physics) a distance $d=\lambda/2$ apart. A cap gives a [pressure](thermodynamics.md#pressure) [antinode](#antinode) at the closed end; an open end has a [pressure](thermodynamics.md#pressure) node just outside it. These are [pressure](thermodynamics.md#pressure) patterns, distinct from [displacement](classical-mechanics.md#displacement) patterns. The guide advises [wavelengths](#wavelength) longer than the pipe diameter, sufficient pipe length to locate both a node and an [antinode](#antinode), and [frequency spectrum](fourier-analysis.md#frequency-spectrum) analysis to distinguish the intended tone from other sounds.[pp. 10–11, Standing waves. Reflection and transmission. Speed of sound; apparatus, microphone scan, and pressure-node distinction](physics-bibliography.md#interesting-and-inexpensive-experiments-for-high-school-physics-by-joe-wolfe)

The inference follows from [superposition](vector-space.md#superposition-principle) of two oppositely directed [acoustic plane waves](physics.md#acoustic-plane-wave). In an ideal uniform, lossless pipe, taking equal [pressure](thermodynamics.md#pressure) [amplitudes](physics.md#wave-amplitude) $P$ and a rigid cap at $x=0$ gives

$$
p'(x,t)=P\cos(kx-\omega t)+P\cos(kx+\omega t)=2P\cos(kx)\cos(\omega t).
$$

The time-varying [pressure](thermodynamics.md#pressure) perturbation $p'$ has local oscillation [amplitude](physics.md#wave-amplitude) $2|P\cos(kx)|$. Its zeros are separated by $\pi/|k|=\lambda/2$. Unequal incident and reflected [amplitudes](physics.md#wave-amplitude) leave nonzero minima, but their spacing remains $\lambda/2$ in this ideal model. A [microphone](#microphone) detects that [pressure](thermodynamics.md#pressure) variation through a changing electrical [signal](electrical-engineering.md#signal), rather than watching a [wave crest](#wave-crest) move. Record the tone's [frequency](physics.md#frequency) too, then infer [phase speed](#phase-speed) $v_p=2fd$.

For proposed controls, keep the drive [frequency](physics.md#frequency) and [amplitude](physics.md#wave-amplitude) fixed during a scan, verify the [frequency](physics.md#frequency) on the recorded [signal](electrical-engineering.md#signal), and repeat the scan in both directions. Fit several minimum positions $x_j=a+jd$ using [linear regression](linear-regression.md) to reduce dependence on one pair of positions. Check the ruler scale and use one consistent reference point on the [microphone](#microphone). Compare with the source switched off to locate background [measurement noise](probability-and-statistics.md#measurement-noise); use [frequency spectrum](fourier-analysis.md#frequency-spectrum) analysis to check for additional tones, and reduce drive if the trace ceases to resemble a [sinusoid](geometry-and-topology.md#sinusoid). Record air [temperature](thermodynamics.md#temperature) and avoid strong air motion. These are suggested controls, not additional procedures or observations attributed to the guide.

The pipe must support approximately [plane waves](quantum-mechanics.md#plane-wave) over the measured region: transverse structure at shorter [wavelengths](#wavelength), the [microphone](#microphone)'s finite size, and disturbance by the ruler can compromise the interpretation. Weak reflection gives shallow minima, while [damping](#damping) and other reflections can shift the extrema of the simple two-wave model. Measure interior spacings rather than assuming the first minimum is exactly at the pipe lip. A short scan may not include enough minima to estimate $d$ reliably, and drift during sequential scanning can imitate spatial variation.

For an explicitly hypothetical calculation, $f=1000\,\mathrm{Hz}$ and $d=0.1715\,\mathrm m$ give $\lambda=0.3430\,\mathrm m$, $K\simeq18.3183\,\mathrm{rad\,m^{-1}}$, and $v_p=343.0\,\mathrm{m\,s^{-1}}$. No such measurements are claimed here. If independent small [measurement errors](probability-and-statistics.md#measurement-error) in $f$ and fitted $d$ have [standard deviations](variance.md#standard-deviation) $\sigma_f$ and $\sigma_d$, first-order [error propagation](#propagation-of-uncertainty) gives $\sigma_{v_p}/v_p\simeq\sqrt{(\sigma_f/f)^2+(\sigma_d/d)^2}$. A systematic scale error or changing air conditions requires separate assessment.

##### Oscilloscope

↑ **Parent:** [Acoustic wavelength measurement](#acoustic-wavelength-measurement)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Oscilloscope)

An [oscilloscope](#oscilloscope) displays an electrical [signal](electrical-engineering.md#signal) versus time. In an [acoustic wavelength measurement](#acoustic-wavelength-measurement), the [microphone](#microphone) trace supplies the tone's [frequency](physics.md#frequency) and oscillation [amplitude](physics.md#wave-amplitude) as the detector changes position.

##### Propagation of uncertainty

↑ **Parent:** [Acoustic wavelength measurement](#acoustic-wavelength-measurement)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Propagation_of_uncertainty)

[Propagation of uncertainty](#propagation-of-uncertainty) estimates how [measurement errors](probability-and-statistics.md#measurement-error) in inputs affect a calculated result. For small input errors with [covariance matrix](variance.md#covariance-matrix) $\Sigma$, linearizing a differentiable [function](function.md) $g$ gives the displayed approximation for its [variance](variance.md). For independent errors in a product $g=2fd$, the squared relative [standard deviations](variance.md#standard-deviation) add. Correlated errors need the covariance terms; systematic offsets require separate assessment.

#### Local wavelength

↑ **Parent:** [Wavelength](#wavelength)

For a locally oscillatory [wave](physics.md#wave) written $u(\mathbf x,t)=A(\mathbf x,t)\cos\phi(\mathbf x,t)$, the local [wavevector](continuum-mechanics.md#wavevector) is $\mathbf k_{\mathrm{loc}}=\nabla\phi$, where $\nabla$ is the spatial [gradient](calculus.md#gradient). The [local wavelength](#local-wavelength) $2\pi/|\mathbf k_{\mathrm{loc}}|$ measures local [wave phase](physics.md#phase-waves) spacing normal to the [wavefront](optics.md#wavefront). Interpreting it as a crest separation requires the [amplitude](physics.md#wave-amplitude) and local [wavevector](continuum-mechanics.md#wavevector) to vary little over one [wavelength](#wavelength), as in the [WKB approximation](analysis.md#wkb-approximation). Along a unit direction $\mathbf e$ the corresponding local repeat distance is $2\pi/|\mathbf k_{\mathrm{loc}}\cdot\mathbf e|$, if that [dot product](linear-algebra.md#dot-product) is nonzero; oblique sampling measures this projected spacing.

A real snapshot alone does not uniquely specify $A$ and $\phi$: their meaning requires a chosen oscillatory component or physical approximation. Strong [interference](optics.md#interference-wave-propagation), zeros of [amplitude](physics.md#wave-amplitude), and rapidly changing media can defeat a single-carrier description. If $\nabla\phi=0$, the local reciprocal formula gives no finite [wavelength](#wavelength); it does not establish an exact global spatial [period](mathematics.md#period-of-a-function).

## Dispersion relation

↑ **Parent:** [Wave equation](wave-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dispersion_relation)

A [dispersion relation](#dispersion-relation) specifies which [angular frequencies](classical-mechanics.md#angular-frequency) and [wavevectors](continuum-mechanics.md#wavevector) a linear wave model admits. Fix the [plane wave](quantum-mechanics.md#plane-wave) convention

$$
u(\mathbf x,t)=\operatorname{Re}\!\left\{a e^{i(\mathbf k\cdot\mathbf x-\omega t)}\right\},\qquad D(\omega,\mathbf k)=0.
$$

Here $a$ is a constant [complex amplitude](physics.md#complex-amplitude), $\mathbf k$ is the [wavevector](continuum-mechanics.md#wavevector), and $\omega$ is the [angular frequency](classical-mechanics.md#angular-frequency). Substitution into a constant-coefficient [linear partial differential equation](partial-differential-equation.md#linear-partial-differential-equation) replaces $\partial_t$ by $-i\omega$ and $\nabla$ by $i\mathbf k$, turning the wave problem into an algebraic condition. A system can have several roots; $\omega=\omega(\mathbf k)$ means one chosen branch, rather than a promise that the full [dispersion relation](#dispersion-relation) is single-valued. For real $\mathbf k$, $\operatorname{Im}\omega>0$ means temporal growth in this convention, while $\operatorname{Im}\omega<0$ means [damping](#damping). The real-branch discussion of [phase velocity](#phase-velocity) and [group velocity](#group-velocity) below assumes negligible loss.

For the one-dimensional [wave equation](wave-equation.md) $u_{tt}=c^2u_{xx}$, the [dispersion relation](#dispersion-relation) is $\omega^2=c^2k^2$. The branch $\omega=ck$ carries right-moving [travelling waves](analysis.md#travelling-wave) for $c>0$; both its [phase velocity](#phase-velocity) and [group velocity](#group-velocity) are $c$. One may instead use the positive-[angular frequency](classical-mechanics.md#angular-frequency) branch $\omega=c|k|$, with right-moving components at $k>0$ and left-moving components at $k<0$. A real wave pairs each $(k,\omega)$ with $(-k,-\omega)$; that conjugate pair represents the same travelling pattern. Branch and sign choices therefore matter when interpreting a [dispersion diagram](#dispersion-diagram).

A particularly tangible [dispersive](#wave-dispersion) example is a small-amplitude [surface gravity wave](fluid-mechanics.md#surface-gravity-wave) on still water of uniform depth $h$. Neglect [surface tension](fluid-mechanics.md#surface-tension) and [viscosity](fluid-mechanics.md#dynamic-viscosity), assume [incompressible flow](fluid-mechanics.md#incompressible-flow) and [irrotational flow](fluid-mechanics.md#irrotational-flow), and impose a flat impermeable bottom. With $k>0$ and positive [angular frequency](classical-mechanics.md#angular-frequency),

$$
\omega^2=gk\tanh(kh),\qquad g>0.
$$

Here $g$ is [gravitational acceleration](classical-mechanics.md#gravitational-acceleration) and $\tanh$ is the [hyperbolic tangent](calculus.md#hyperbolic-tangent). Deep water means $kh\gg1$: $\omega\simeq\sqrt{gk}$ and longer [wavelengths](#wavelength) have larger [phase speed](#phase-speed). Shallow water means $kh\ll1$: $\omega\simeq\sqrt{gh}\,k$, an approximately [nondispersive wave](#nondispersive-wave). Thus depth relative to [wavelength](#wavelength), rather than depth alone, determines whether crests and [wave packets](#wave-packet) travel together.[equation 3.2](physics-bibliography.md#free-surface-water-waves-13-012-hydrodynamics-for-ocean-engineers-reading-5-by-a-h-techet)

The [dispersion diagram](#dispersion-diagram) below also includes the ideal deep-water [capillary wave](fluid-mechanics.md#capillary-wave) limit $\omega=\sqrt{\gamma/\rho}\,k^{3/2}$, where $\gamma$ is [surface tension](fluid-mechanics.md#surface-tension) and $\rho$ is [mass density](fluid-mechanics.md#density). This limit requires the [surface tension](fluid-mechanics.md#surface-tension) restoring term to dominate [gravity](physics.md#gravity); it reverses the trend of the [surface gravity wave](fluid-mechanics.md#surface-gravity-wave), giving larger [phase speed](#phase-speed) at shorter [wavelength](#wavelength). The combined [gravity-capillary wave](fluid-mechanics.md#gravity-capillary-wave) has $\omega^2=gk+(\gamma/\rho)k^3$.[equation 9.7](physics-bibliography.md#pulse-propagation-by-richard-fitzpatrick)

<a id="image-analytical-dispersion-diagrams-origin-to-point-slope-gives-phase-velocity-tangent-slope-gives-group-velocity"></a>
![](phase-group-dispersion-slopes.png)

**[Figure 11](#image-analytical-dispersion-diagrams-origin-to-point-slope-gives-phase-velocity-tangent-slope-gives-group-velocity). Analytical dispersion diagrams: origin-to-point slope gives phase velocity, tangent slope gives group velocity**.

The curves use dimensionless normalizations chosen separately for each model; they are analytical diagrams, not experimental data. Their beauty is that a single [dispersion relation](#dispersion-relation) encodes several observable behaviours: its value gives the [angular frequency](classical-mechanics.md#angular-frequency), its origin-to-point slope gives the one-dimensional [phase velocity](#phase-velocity), its tangent slope gives the [group velocity](#group-velocity), and variation of that tangent slope predicts distortion of a [wave packet](#wave-packet). A straight line through the origin describes a [nondispersive wave](#nondispersive-wave); an affine branch $\omega=ck+b$ with $b\ne0$ has constant [group velocity](#group-velocity) but [phase velocity](#phase-velocity) $c+b/k$, so those properties must be distinguished.

### Spatial root of a dispersion relation

↑ **Parent:** [Dispersion relation](#dispersion-relation)

For fixed complex frequency $\omega$, a spatial root is a complex [wavenumber](#wavenumber) $k$ satisfying the [dispersion relation](#dispersion-relation). Analytic continuation of these branches from a causal temporal contour is essential in the [Briggs-Bers criterion](#briggs-bers-criterion); their collision alone does not decide whether a [spatial pinch point](#spatial-pinch-point) occurs.

### Spatiotemporal wave-packet stability

↑ **Parent:** [Dispersion relation](#dispersion-relation)

The response to a localized perturbation must be followed in space as well as time. Growth at a fixed position is [absolute wave-packet instability](#absolute-wave-packet-instability); growth transported away while the original position decays is [convective wave-packet instability](#convective-wave-packet-instability). The [Briggs-Bers criterion](#briggs-bers-criterion) evaluates the relevant complex spatial branches of a [dispersion relation](#dispersion-relation), while a real-wavenumber temporal mode test alone does not generally distinguish those behaviors.

#### Modulational instability

↑ **Parent:** [Spatiotemporal wave-packet stability](#spatiotemporal-wave-packet-stability)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Modulational_instability)

Modulational instability is growth of long-wavelength [perturbations](analysis.md#perturbation) of a uniform or periodic wave due to coupling between its modulation and nonlinear dynamics. In the [focusing nonlinear Schrodinger equation](integrable-systems.md#focusing-nonlinear-schrodinger-equation), the amplitude and phase perturbations can have imaginary modulation frequencies even though the unperturbed wave is an exact solution.

##### Benjamin-Feir instability

↑ **Parent:** [Modulational instability](#modulational-instability)

For the [complex Ginzburg–Landau equation](partial-differential-equation.md#complex-ginzburg-landau-equation) $A_t=A+(1+ic_1)A_{xx}-(1+ic_3)|A|^2A$, the uniform oscillation has a neutral [phase](physics.md#phase-waves) mode whose [growth rate](#growth-rate) is $\lambda=-(1+c_1c_3)k^2+O(k^4)$. Negative [phase](physics.md#phase-waves) diffusion therefore causes a long-wavelength [modulational instability](#modulational-instability). The [Benjamin-Feir stability condition](partial-differential-equation.md#benjamin-feir-stability-condition) is the complementary positive-diffusion condition. On a finite domain an unstable wavenumber must actually be allowed by the boundary conditions.

##### Focusing nonlinear Schrodinger modulation dispersion

↑ **Parent:** [Modulational instability](#modulational-instability)

For $-iA_t+\chi A_{xx}-\mu A+\delta A|A|^2=0$ with positive coefficients, linearize around $A=\sqrt{\mu/\delta}$ using real amplitude and phase perturbations. Their two-by-two [dispersion relation](#dispersion-relation) gives the displayed equation. The [modulational instability](#modulational-instability) band is $0<K^2<2\mu/\chi$, with maximum [growth rate](#growth-rate) $\mu$ at $K^2=\mu/\chi$.

#### Briggs-Bers criterion

↑ **Parent:** [Spatiotemporal wave-packet stability](#spatiotemporal-wave-packet-stability)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Briggs–Bers_criterion)

A criterion for [absolute wave-packet instability](#absolute-wave-packet-instability) based on analytic continuation of the spatial roots of a [dispersion relation](#dispersion-relation). Start the temporal inversion contour above the spectrum, then lower it while deforming the spatial contour. A [spatial pinch point](#spatial-pinch-point) occurs when branches originating in opposite spatial half-planes obstruct that deformation. A double root $D=D_k=0$ is only an algebraic candidate. The opposite-half-plane condition is stated in the primary study [https://doi.org/10.1017/jfm.2016.195,](https://doi.org/10.1017/jfm.2016.195,) section 4.2.

##### Bounded temporal growth condition for cubic dispersion

↑ **Parent:** [Briggs-Bers criterion](#briggs-bers-criterion)

For $\omega(k)=i\alpha k^2-\beta k^3-i\gamma$, real-wavenumber growth is $\operatorname{Re}\alpha\,k^2-\operatorname{Im}\beta\,k^3-\operatorname{Re}\gamma$. A nonzero cubic coefficient is unbounded above on one side; after it vanishes, a positive quadratic coefficient is unbounded above on both sides. The displayed conditions are therefore necessary and sufficient for a finite temporal upper bound, which is then $-\operatorname{Re}\gamma$. The bound permits the initial causal temporal contour required by the [Briggs-Bers criterion](#briggs-bers-criterion).

##### Quartic impulse-response Laplace resolvent

↑ **Parent:** [Briggs-Bers criterion](#briggs-bers-criterion)

For the whole-line equation $A_t+a_1A_{xx}+a_2A_{xxxx}+a_3A=0$ with $\operatorname{Re}a_2>0$, the [dispersion relation](#dispersion-relation) is $s=a_1k^2-a_2k^4-a_3$. The temporal [Laplace transform](analysis.md#laplace-transform) of the impulse response at zero is the real-k integral of $[s+a_3-a_1k^2+a_2k^4]^{-1}/(2\pi)$. Factor the denominator as $a_2(k^2+\kappa_1^2)(k^2+\kappa_2^2)$ with $\operatorname{Re}\kappa_j>0$ for large $\operatorname{Re}s$. Partial fractions give the displayed resolvent. Square-root sheets are chosen by continuation from this causal large-s region; choosing roots independently can introduce false [spatial pinch points](#spatial-pinch-point).

###### Physical-sheet growth rate of a quartic impulse response

↑ **Parent:** [Quartic impulse-response Laplace resolvent](#quartic-impulse-response-laplace-resolvent)

Put $z=a_1/\sqrt{a_2}$ using the root with positive real part. The additional resolvent singularity at $s+a_3=z^2/4$ lies on the physical square-root sheet only when $\operatorname{Re}z>0$; otherwise the apparent saddle is on the other sheet. The singularity at $s=-a_3$ remains, including a quartic degeneracy when $a_1=0$. The rightmost physical singularity determines the exponential fixed-position growth rate. Compare it with the temporal maximum $-\operatorname{Re}a_3+\max(\operatorname{Re}a_1,0)^2/(4\operatorname{Re}a_2)$ to distinguish [absolute wave-packet instability](#absolute-wave-packet-instability) from [convective wave-packet instability](#convective-wave-packet-instability). Equality cases require their algebraic prefactors.

##### Spatial pinch point

↑ **Parent:** [Briggs-Bers criterion](#briggs-bers-criterion)

A collision of spatial branches which pinches the spatial inversion contour as the temporal contour is lowered from above all singularities. The branches must originate on opposite sides of the spatial contour. A collision of two upper-half-plane branches or two lower-half-plane branches can solve the double-root equations without causing [absolute wave-packet instability](#absolute-wave-packet-instability).

###### False complex saddle in dissipative cubic dispersion

↑ **Parent:** [Spatial pinch point](#spatial-pinch-point)

For these constants, every real-wavenumber [growth rate](#growth-rate) is $-k^2-1/10<0$. The real-contour impulse integral decays with envelope $e^{-t/10}t^{-1/2}$ at fixed position. Yet the stationary candidate $k=-2i/3$ has $\operatorname{Im}\omega=4/27-1/10>0$. It cannot be a contributing [spatial pinch point](#spatial-pinch-point); otherwise it would contradict the real-contour growth bound. This explicit example shows why solving the algebraic saddle equations is insufficient for [absolute wave-packet instability](#absolute-wave-packet-instability).

###### False spatial saddle in quartic dispersion

↑ **Parent:** [Spatial pinch point](#spatial-pinch-point)

The real dispersion above is temporally stable for every real $k$, but its analytic continuation has stationary points at $k=\pm i$ with $\omega=i/2$. Writing $\omega=i\Omega$ gives $k^2=-1\pm\sqrt{1/2-\Omega}$; as $\Omega$ decreases to $1/2$, both branches at $+i$ approach from the upper half-plane and both at $-i$ from the lower. These are not [spatial pinch points](#spatial-pinch-point). This provides a concrete counterexample to treating growing algebraic double roots as sufficient for [absolute wave-packet instability](#absolute-wave-packet-instability).

#### Convective wave-packet instability

↑ **Parent:** [Spatiotemporal wave-packet stability](#spatiotemporal-wave-packet-stability)

A localized disturbance grows along some moving rays but decays at its original fixed location. This wave-packet meaning differs from buoyancy-driven stellar convection and is therefore given a distinct canonical title. Changing the observation frame can change the absolute/convective classification. The [Briggs-Bers criterion](#briggs-bers-criterion) uses the laboratory-frame impulse response to distinguish this case from [absolute wave-packet instability](#absolute-wave-packet-instability).

#### Absolute wave-packet instability

↑ **Parent:** [Spatiotemporal wave-packet stability](#spatiotemporal-wave-packet-stability)

A localized perturbation has positive asymptotic exponential growth at a fixed observation point in the chosen reference frame. The relevant [spatial pinch point](#spatial-pinch-point) of the [Briggs-Bers criterion](#briggs-bers-criterion) has positive imaginary [frequency](physics.md#frequency). Merely finding a growing temporal mode or a formal complex saddle is not sufficient; the saddle must contribute to the localized impulse response.

#### Finite maximum temporal growth rate

↑ **Parent:** [Spatiotemporal wave-packet stability](#spatiotemporal-wave-packet-stability)

With normal modes $e^{ikx-i\omega t}$, a finite upper bound on $\operatorname{Im}\omega$ allows the inverse temporal [Laplace transform](analysis.md#laplace-transform) contour to start above all temporal singularities. An unbounded growth rate at high real [wavenumber](#wavenumber) prevents the standard causal [Green function](analysis.md#green-s-function) construction used in the [Briggs-Bers criterion](#briggs-bers-criterion). For $\operatorname{Im}\omega=\alpha k^2-\beta k^4-\gamma$ with nonzero real $\beta$, the bound holds exactly when $\beta>0$.

### Wave dispersion

↑ **Parent:** [Dispersion relation](#dispersion-relation)

Wave dispersion means that [phase velocity](#phase-velocity) depends on [wavenumber](#wavenumber) or, equivalently, [wavelength](#wavelength). [Wave packets](#wave-packet) generally travel with [group velocity](#group-velocity), which need not equal [phase velocity](#phase-velocity). The [linear rotating shallow-water dispersion relation](geophysical-fluid-dynamics.md#linear-rotating-shallow-water-dispersion-relation) $\omega^2=f^2+c^2k^2$ has faster long-wave phase motion but slower long-[wave packet](#wave-packet) motion when $f\ne0$.

#### Nondispersive wave

↑ **Parent:** [Wave dispersion](#wave-dispersion)

A nondispersive wave has constant [phase velocity](#phase-velocity) on a propagation branch. For $\omega=ck$, its [group velocity](#group-velocity) is also $c$. A [frequency](physics.md#frequency) relation with a nonzero offset, such as $\omega=ck+b$, has constant [group velocity](#group-velocity) but a [phase velocity](#phase-velocity) $c+b/k$ depending on [wavenumber](#wavenumber); constant [group velocity](#group-velocity) alone is therefore not sufficient for nondispersion.

### Dispersion diagram

↑ **Parent:** [Dispersion relation](#dispersion-relation)

A dispersion diagram plots the branches of a [dispersion relation](#dispersion-relation), usually with [wavenumber](#wavenumber) on the horizontal axis and [angular frequency](classical-mechanics.md#angular-frequency) on the vertical axis. Its slopes, intersections, and gaps display [group velocities](#group-velocity), mode conversion, and forbidden frequency ranges.

### Ray tracing

↑ **Parent:** [Dispersion relation](#dispersion-relation)

Ray tracing follows the paths along which a slowly modulated wave packet propagates. For a local dispersion relation $\omega=\Omega(\mathbf k;\mathbf x,t)$, the ray velocity is the [group velocity](#group-velocity) $\nabla_{\mathbf k}\Omega$.

#### Travel time

↑ **Parent:** [Ray tracing](#ray-tracing)

A wave's travel time along a [elastic ray](#elastic-ray) is the integral of local [slowness](#slowness) against [arc length](riemannian-geometry.md#arc-length). Its variation with source and receiver position describes the arrival branches, including transmitted and reflected paths. Different paths can have different travel times between the same endpoints.

#### Elastic ray

↑ **Parent:** [Ray tracing](#ray-tracing)

In a smooth isotropic medium, an [elastic ray](#elastic-ray) is the path followed by a local [wavefront](optics.md#wavefront) normal, with the appropriate P or S [wave speed](#wave-speed) $c$. Arclength $s$ gives the displayed trajectory and travel-time equations. Its neighboring ray paths determine geometrical spreading, while the [eikonal equation](continuum-mechanics.md#eikonal-equation) determines the normals. A [caustic](optics.md#wave-caustic) occurs where the neighboring paths focus and the elementary ray [wave amplitude](physics.md#wave-amplitude) description ceases to be uniform.

##### Spherical elastic ray invariant

↑ **Parent:** [Elastic ray](#elastic-ray)

For an [isotropic](continuum-mechanics.md#isotropy) radial [wave speed](#wave-speed) $\alpha(r)$, the [elastic ray](#elastic-ray) equations imply conservation of $\mathbf x\times\mathbf y$, where $\mathbf y$ is the [slowness](#slowness) vector. Indeed, its derivative is $\alpha\mathbf y\times\mathbf y+\mathbf x\times\nabla(1/\alpha)=0$. Thus each nonradial [elastic ray](#elastic-ray) lies in a fixed plane through the centre and $p=|\mathbf x\times\mathbf y|$ is constant. The angle $i$ is measured from the radial direction; tangential [slowness](#slowness) continuity preserves $p$ across spherical interfaces.

<h6 id="herglotz-wiechert-inversion">Herglotz–Wiechert inversion</h6>

↑ **Parent:** [Spherical elastic ray invariant](#spherical-elastic-ray-invariant)

For a spherically symmetric speed with strictly increasing $\eta(r)=r/v(r)$, a turning ray of parameter $p$ has $\Delta(p)=2p\int_p^{\eta_a}(d\log r/d\eta)(\eta^2-p^2)^{-1/2}\,d\eta$. Integrate this against $(p^2-\mu^2)^{-1/2}$ and interchange the triangular integration region. The inner kernel integral is $\pi/2$, giving the displayed radius and then $v(r(\mu))=r(\mu)/\mu$. Complete turning-ray branch data are required.

###### Hidden turning-ray zone from nonmonotone spherical slowness

↑ **Parent:** [Herglotz–Wiechert inversion](#herglotz-wiechert-inversion)

Where $\eta=r/v$ decreases outwards, it increases as a surface ray travels inward, so no surface ray turns inside that interval. Penetrating rays may traverse it and turn deeper. The radius is then not a single-valued function of $\eta$, and angular ray data constrain combined branch contributions rather than the single function inverted by [Herglotz–Wiechert inversion](#herglotz-wiechert-inversion). Additional structural or observational information is needed to locate the hidden profile.

###### Core-reflected travel time

↑ **Parent:** [Spherical elastic ray invariant](#spherical-elastic-ray-invariant)

In a constant-speed spherical shell with outer radius $R$ and inner radius $a$, a symmetric single reflection from the inner boundary has the displayed [travel time](#travel-time). The boundary lies on the angular bisector of source and receiver. The branch exists only for $0\leq\Delta\leq2\arccos(a/R)$, since the incident line must remain in the shell. At the endpoint it joins the mantle-only chord branch with the same slope $a/c$. Continuing the formula beyond that endpoint would make the line intersect the inner boundary before its supposed reflection point.

##### Hyperbolic interface collimation of P-waves

↑ **Parent:** [Elastic ray](#elastic-ray)

A solid-to-fluid interface can turn spherical source [P waves](#p-wave) into parallel vertical rays if its height $Z(R)$ satisfies the displayed travel-time identity, with $r=\sqrt{R^2+Z^2}$. The positive branch through $Z(0)=z_0$ is a hyperboloid when $\alpha>\alpha_f$. Differentiating the travel-time identity enforces [Snell law for elastic and acoustic waves](continuum-mechanics.md#snell-law-for-elastic-and-acoustic-waves). Travel time above the interface is then $z_0/\alpha+(z-z_0)/\alpha_f$, independent of cylindrical radius. The leading [wavefront](optics.md#wavefront) is planar although its [wave amplitude](physics.md#wave-amplitude) need not be uniform across that plane.

#### Hamiltonian ray equations for a local dispersion relation

↑ **Parent:** [Ray tracing](#ray-tracing)

A local [dispersion relation](#dispersion-relation) $\omega=\Omega(\mathbf k;\mathbf X,T)$ yields

$$
\frac{d\mathbf X}{dT}=\nabla_{\mathbf k}\Omega,\quad\frac{d\mathbf k}{dT}=-\nabla_{\mathbf X}\Omega\big|_{\mathbf k},\quad\frac{d\omega}{dT}=\Omega_T\big|_{\mathbf k}.
$$

The spatial and temporal derivatives on the right hold the [wavevector](continuum-mechanics.md#wavevector) fixed. Translation symmetries conserve the corresponding wavevector components, while time independence conserves frequency.

##### Simple turning point of a variable-speed wave

↑ **Parent:** [Hamiltonian ray equations for a local dispersion relation](#hamiltonian-ray-equations-for-a-local-dispersion-relation)

A simple turning point for a stratified [wavespeed](#wave-speed) occurs at $c(Y_s)=\omega/k$, where $Q=\omega^2/c^2-k^2$ has a nonzero derivative. If $c_Y(Y_s)>0$, write $q=-Q'(Y_s)>0$; then $\ell\sim[q(Y_s-Y)]^{1/2}$ below it. The vertical [group velocity](#group-velocity) vanishes and the [stationary wave amplitude in a stratified wavespeed](optics.md#stationary-wave-amplitude-in-a-stratified-wavespeed) diverges as $(Y_s-Y)^{-1/4}$.

###### Airy scaling at a variable-speed wave turning point

↑ **Parent:** [Simple turning point of a variable-speed wave](#simple-turning-point-of-a-variable-speed-wave)

In $\varepsilon^2\Psi''+2\varepsilon^2(c'/c)\Psi'+Q(Y)\Psi=0$, with $Q\sim-q(Y-Y_s)$ and $q>0$, set $Y-Y_s=(\varepsilon^2/q)^{1/3}\eta$. The leading equation is $\Psi_{\eta\eta}-\eta\Psi=0$, the [Airy ordinary differential equation](differential-equation.md#airy-ordinary-differential-equation). The first derivative and nonlinear coefficient corrections are smaller by $O(\varepsilon^{2/3})$.

###### Decaying Airy continuation and ray reflection

↑ **Parent:** [Airy scaling at a variable-speed wave turning point](#airy-scaling-at-a-variable-speed-wave-turning-point)

The local inner solution is a combination of [Airy functions](differential-equation.md#airy-function) $\operatorname{Ai},\operatorname{Bi}$. Decay in the forbidden region removes $\operatorname{Bi}$. The remaining [Airy turning-point connection formula](analysis.md#airy-turning-point-connection-formula) is oscillatory on the allowed side and represents an incident/reflected pair, not a single upward branch. Without the forbidden-side condition the local differential equation alone leaves both coefficients free.

###### Turning-point enhancement of wave amplitude

↑ **Parent:** [Airy scaling at a variable-speed wave turning point](#airy-scaling-at-a-variable-speed-wave-turning-point)

A simple ray turning point has outer [amplitude](physics.md#wave-amplitude) proportional to $|Y-Y_s|^{-1/4}$. At the [Airy scaling at a variable-speed wave turning point](#airy-scaling-at-a-variable-speed-wave-turning-point), $|Y-Y_s|=O(\varepsilon^{2/3})$, this gives an inner wavefield of size $O(\varepsilon^{-1/6})$ when the incident action normalization is order one. The enhancement is finite for nonzero $\varepsilon$ and is resolved by the [Airy function](differential-equation.md#airy-function).

#### Stationary square-root-dispersion wake

↑ **Parent:** [Ray tracing](#ray-tracing)

For the zero-frequency dispersion relation

$$
\Omega=\alpha|\mathbf k|^{1/2}-Vk_1,
$$

write $\mathbf k=\kappa(\cos\phi,\sin\phi)$. Then

$$
\kappa=\frac{\alpha^2}{V^2\cos^2\phi},
\qquad
\tan\psi=-\frac{\tan\phi}{1+2\tan^2\phi},
$$

where $\psi$ is the direction of the [group velocity](#group-velocity). Maximizing the angular slope gives a downstream wake wedge of semi-angle

$$
\tan^{-1}(2^{-3/2}).
$$

### Growth rate

↑ **Parent:** [Dispersion relation](#dispersion-relation)

For a normal mode proportional to $e^{\sigma t}$, the real part $\operatorname{Re}\sigma$ is its exponential growth rate. A positive growth rate signals linear instability.

### Phase velocity and group velocity

↑ **Parent:** [Dispersion relation](#dispersion-relation)

For a dispersion relation $\omega(k)$, the phase velocity is $c_p=\omega/k$ and the group velocity is $c_g=d\omega/dk$. For the Klein-Gordon relation at $k>0$,

$$
c_p=c\frac{\sqrt{k^2+A^2}}{k}>c,
\qquad
c_g=c\frac{k}{\sqrt{k^2+A^2}}<c,
\qquad
c_pc_g=c^2.
$$

#### Klein-Gordon packet velocities

↑ **Parent:** [Phase velocity and group velocity](#phase-velocity-and-group-velocity)

A useful stipulated dispersive medium obeys the [Klein-Gordon equation](#klein-gordon-equation) $u_{tt}-c^2u_{xx}+\omega_0^2u=0$, with $c>0$ and $\omega_0>0$. Its positive-[angular frequency](classical-mechanics.md#angular-frequency) [dispersion relation](#dispersion-relation) is

$$
\omega(k)=\sqrt{\omega_0^2+c^2k^2},\qquad
v_p=\frac{\omega(k)}{k},\qquad
v_g=\omega'(k)=\frac{c^2k}{\omega(k)}.
$$

Here $\omega_0$ is the gap at zero [wavenumber](#wavenumber), not the central [angular frequency](classical-mechanics.md#angular-frequency) $\omega_c=\omega(k_0)$ of a [wave packet](#wave-packet); the parameter in the preceding formula is $A=\omega_0/c$. For $k>0$, the [phase velocity](#phase-velocity) satisfies $v_p>c$, the [group velocity](#group-velocity) satisfies $0<v_g<c$, and $v_pv_g=c^2$. In this stipulated medium $c$ is the limiting propagation speed of the model; it need not mean the vacuum [speed of light](special-relativity.md#speed-of-light). The same square-root [dispersion relation](#dispersion-relation) appears in [waveguide phase and group velocities](electromagnetism.md#waveguide-phase-and-group-velocities), with a [waveguide cutoff frequency](electromagnetism.md#waveguide-cutoff-frequency) playing the role of $\omega_0$.[equation 9.6 and equations 9.10–9.12: square-root dispersion and local group velocity](physics-bibliography.md#pulse-propagation-by-richard-fitzpatrick)

For the original dimensionless choice $c=\omega_0=k_0=1$, a [carrier wave](#carrier-wave) has [phase velocity](#phase-velocity) $v_p=\sqrt2$, while a narrow [wave packet](#wave-packet) has leading [group velocity](#group-velocity) $v_g=1/\sqrt2$. After time $t=8$, the carrier's zero-[wave phase](physics.md#phase-waves) reference has moved to $x=8\sqrt2\simeq11.31$, whereas the leading [wave envelope](#envelope-waves) centre is at $x=8/\sqrt2\simeq5.66$. A carrier [wave crest](#wave-crest) therefore moves through the [wave envelope](#envelope-waves); it does not carry an identifiable piece of the envelope with it.

<a id="image-stipulated-klein-gordon-medium-secant-phase-velocity-tangent-group-velocity-and-front-speed"></a>
![](klein-gordon-dispersion-and-velocity-scales.png)

**[Figure 12](#image-stipulated-klein-gordon-medium-secant-phase-velocity-tangent-group-velocity-and-front-speed). Stipulated Klein-Gordon medium: secant phase velocity, tangent group velocity and front speed**.

The origin-to-curve secant on the [dispersion diagram](#dispersion-diagram) gives [phase velocity](#phase-velocity), while its local tangent gives [group velocity](#group-velocity). As $k\to0^+$, $v_p\to\infty$ and $v_g\to0$; at $k=0$ the [phase velocity](#phase-velocity) itself is undefined. As $k\to\infty$, both approach $c$, from opposite sides. On the same positive-[angular frequency](classical-mechanics.md#angular-frequency) branch with $k<0$, both signed velocities are negative and their product remains $c^2$. These conventions distinguish direction from [phase speed](#phase-speed). Reversing both $k$ and $\omega$ represents the same real [plane wave](quantum-mechanics.md#plane-wave); changing just one sign changes its direction.

For an original finite-bandwidth check, take equal-amplitude [plane waves](quantum-mechanics.md#plane-wave) at $k_1=0.8$ and $k_2=1.2$, still with $c=\omega_0=1$. The exact two-tone [wave envelope](#envelope-waves) speed is

$$
v_{\rm beat}=\frac{\sqrt{1+1.2^2}-\sqrt{1+0.8^2}}{1.2-0.8}\simeq0.703563,
$$

while its [carrier wave](#carrier-wave) has [phase velocity](#phase-velocity) $(\sqrt{1+0.8^2}+\sqrt{1+1.2^2})/2\simeq1.421337$. Their product is exactly $1$: rationalizing the difference gives $v_{\rm beat}=2/(\omega_1+\omega_2)$. Nevertheless $v_{\rm beat}\ne\omega'(1)$; the derivative describes the limit of vanishing separation, not an arbitrary pair of tones. The two-tone [wave envelope](#envelope-waves) repeats indefinitely, so it has no isolated first arrival and cannot measure [front velocity](#front-velocity).

#### Phase-group orthogonality for degree-zero dispersion

↑ **Parent:** [Phase velocity and group velocity](#phase-velocity-and-group-velocity)

If a differentiable [dispersion relation](#dispersion-relation) $\omega(\mathbf k)$ is homogeneous of degree zero at nonzero $\mathbf k$, the [Euler homogeneous function theorem](real-analysis.md#euler-theorem-for-homogeneous-functions) gives $\mathbf k\cdot\nabla_{\mathbf k}\omega=0$. Therefore [phase velocity](#phase-velocity) $\omega\mathbf k/k^2$ is orthogonal to [group velocity](#group-velocity) $\nabla_{\mathbf k}\omega$. The result applies exactly to limiting [inertial waves](geophysical-fluid-dynamics.md#inertial-wave); finite compressibility can alter the dispersion.

#### Phase velocity

↑ **Parent:** [Phase velocity and group velocity](#phase-velocity-and-group-velocity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Phase_velocity)

The [phase velocity](#phase-velocity) is the motion of a constant-[wave phase](physics.md#phase-waves) surface. For a one-dimensional [plane wave](quantum-mechanics.md#plane-wave) $u=a\cos(kx-\omega t+\phi_0)$ with real $k\ne0$ and real $\omega$, fixing $kx-\omega t+\phi_0$ gives

$$
k\frac{dx}{dt}-\omega=0,\qquad c_p=\frac{\omega}{k}.
$$

Each [wave crest](#wave-crest) of this monochromatic [travelling wave](analysis.md#travelling-wave) advances at that signed [phase velocity](#phase-velocity). Its magnitude is the [phase speed](#phase-speed) $|c_p|=\lambda/T$, where $\lambda=2\pi/|k|$ is the [wavelength](#wavelength) and $T=2\pi/|\omega|$ is the temporal [period](mathematics.md#period-of-a-function) when $\omega\ne0$. Choosing $\omega>0$ makes positive $k$ mean rightward [phase velocity](#phase-velocity) and negative $k$ mean leftward [phase velocity](#phase-velocity). Reversing both signs leaves the real [plane wave](quantum-mechanics.md#plane-wave) and its [phase velocity](#phase-velocity) unchanged. At $k=0$ there are no spatial crests to track, so $\omega/k$ is undefined; a finite limit as $k\to0$ is a limiting [phase speed](#phase-speed), not the speed of a spatially uniform oscillation.

In several dimensions, a [plane wave](quantum-mechanics.md#plane-wave) has [wave phase](physics.md#phase-waves) $\mathbf k\cdot\mathbf x-\omega t+\phi_0$. Constant-[wave phase](physics.md#phase-waves) planes obey $\mathbf k\cdot\mathbf v=\omega$. Their normal [phase velocity](#phase-velocity) is

$$
\mathbf c_p=\frac{\omega\mathbf k}{|\mathbf k|^2}\qquad(\mathbf k\ne0).
$$

Tangential motion within a plane does not move that [wavefront](optics.md#wavefront), which is why the normal direction fixes the vector convention. In an [anisotropic](continuum-mechanics.md#anisotropy) medium the [group velocity](#group-velocity) need not point along this [wavevector](continuum-mechanics.md#wavevector). Likewise the [horizontal phase velocity](#horizontal-phase-velocity) of a tilted [wavefront](optics.md#wavefront) is its crossing speed along a horizontal line, rather than a component of the normal [phase velocity](#phase-velocity).

For the [nondispersive wave](#nondispersive-wave) branch $\omega=ck$, a [wave crest](#wave-crest) and a [wave envelope](#envelope-waves) both move at $c$. For deep-water [surface gravity waves](fluid-mechanics.md#surface-gravity-wave), $\omega=\sqrt{gk}$ gives $c_p=\sqrt{g/k}$ and [group velocity](#group-velocity) $c_g=c_p/2$. With the illustrative choices $g=9.81\,\mathrm{m\,s^{-2}}$ and $\lambda=1\,\mathrm m$, the model predicts $c_p\simeq1.25\,\mathrm{m\,s^{-1}}$ and $c_g\simeq0.625\,\mathrm{m\,s^{-1}}$. These are calculated values for negligible [surface tension](fluid-mechanics.md#surface-tension) and sufficiently large $kh$, not measurements. A [wave crest](#wave-crest) moves forward through the [wave packet](#wave-packet), so timing a crest does not time the packet's journey.

There is a direct laboratory meaning to this distinction. MIT's 2005 surface-wave lab uses a long water tank, a controllable hydraulic paddle, and an absorbing beach. Resistance probes convert submerged length into voltage; calibration converts their readouts into [free surface](fluid-mechanics.md#free-surface) elevation versus time. Two probes a known distance apart, backed by a ruler and stopwatch, let students time a [wave crest](#wave-crest) and separately time a feature of the [wave packet](#wave-packet). The lab records depth and varies [frequency](physics.md#frequency) and [wave amplitude](physics.md#wave-amplitude).[Surface Waves Kinematics (MIT 2.016 Hydrodynamics) by Massachusetts Institute of Technology, 2.016 course staff](physics-bibliography.md#surface-waves-kinematics-mit-2-016-hydrodynamics-by-massachusetts-institute-of-technology-2-016-course-staff)

For a clean measurement of [phase velocity](#phase-velocity), fit the periodic portion of both records or follow one identifiable [wave crest](#wave-crest). A phase difference is only known modulo $2\pi$: probe spacing below half the shortest relevant [wavelength](#wavelength), or continuity while sweeping [frequency](physics.md#frequency), avoids assigning the wrong whole-cycle delay. Then compare the timed [phase velocity](#phase-velocity) with $\lambda/T$. Tracking pepper grains instead measures fluid-particle motion, which has a different meaning from either [phase velocity](#phase-velocity) or [group velocity](#group-velocity).

The [Klein-Gordon packet velocities](#klein-gordon-packet-velocities) example makes the distinction especially sharp: its [phase velocity](#phase-velocity) exceeds $c$, yet its narrow [wave envelope](#envelope-waves) moves below $c$. A [carrier wave](#carrier-wave) labels successive oscillations; its speed alone does not establish [information velocity](#information-velocity). The [front velocity](#front-velocity) depends on the full causal model, including [angular frequencies](classical-mechanics.md#angular-frequency) far outside the carrier's narrow range.

##### Horizontal phase velocity

↑ **Parent:** [Phase velocity](#phase-velocity)

For phase $kx+mz-\omega t$ with $k\ne0$, hold $z$ fixed: a contour of constant [wave phase](physics.md#phase-waves) advances in $x$ at $\omega/k$. This is the speed at which a tilted [wavefront](optics.md#wavefront) crosses a horizontal line. It differs from the horizontal component of the vector [phase velocity](#phase-velocity), $\omega k/(k^2+m^2)$, which is defined along the [wavevector](continuum-mechanics.md#wavevector).

##### Phase speed

↑ **Parent:** [Phase velocity](#phase-velocity)

The magnitude of the [phase velocity](#phase-velocity) of a real-frequency plane [Fourier mode](fourier-analysis.md#fourier-mode) is $|\omega|/|\mathbf k|$. In an anisotropic medium it depends on the direction of the [wave vector](continuum-mechanics.md#wavevector) and need not equal the [group velocity](#group-velocity) magnitude.

#### Group velocity

↑ **Parent:** [Phase velocity and group velocity](#phase-velocity-and-group-velocity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Group_velocity)

The [group velocity](#group-velocity) of a differentiable, real [dispersion relation](#dispersion-relation) branch is

$$
\mathbf c_g=\nabla_{\mathbf k}\omega(\mathbf k_0),\qquad c_g=\frac{d\omega}{dk}(k_0)\ \text{in one dimension}.
$$

It describes the leading translation of a narrow-band [wave packet](#wave-packet) centred on [wavevector](continuum-mechanics.md#wavevector) $\mathbf k_0$, assuming a linear model, a locally uniform medium and negligible loss. Narrow-band means that the appreciably excited [wavevectors](continuum-mechanics.md#wavevector) occupy a small neighbourhood on which one smooth branch can be linearized. Write its complex wavefield as

$$
\psi(\mathbf x,t)=\int a(\mathbf q)e^{i[(\mathbf k_0+\mathbf q)\cdot\mathbf x-\omega(\mathbf k_0+\mathbf q)t]}\,d\mathbf q.
$$

The [Taylor expansion](calculus.md#taylor-expansion) $\omega(\mathbf k_0+\mathbf q)\simeq\omega_0+\mathbf c_g\cdot\mathbf q$ gives

$$
\psi(\mathbf x,t)\simeq e^{i(\mathbf k_0\cdot\mathbf x-\omega_0t)}A(\mathbf x-\mathbf c_gt),\qquad A(\mathbf y)=\int a(\mathbf q)e^{i\mathbf q\cdot\mathbf y}\,d\mathbf q.
$$

Thus the rapid [wave phase](physics.md#phase-waves) follows the [phase velocity](#phase-velocity), while the slowly varying [wave envelope](#envelope-waves) follows the [group velocity](#group-velocity). This [Fourier analysis](fourier-analysis.md) argument is an outline of the approximation, rather than a statement that every [wave packet](#wave-packet) translates rigidly forever. In one dimension a useful short-time condition is $|\omega''(k_0)|t(\Delta k)^2\ll1$, where $\Delta k$ is the characteristic spectral width; neglected higher derivatives must also remain small. Curvature of the [dispersion relation](#dispersion-relation) eventually changes the [wave envelope](#envelope-waves).[equations 9.9–9.16](physics-bibliography.md#pulse-propagation-by-richard-fitzpatrick)

Two nearby [plane waves](quantum-mechanics.md#plane-wave) make the derivative visible without an integral. For equal [wave amplitudes](physics.md#wave-amplitude) $a$, define $\bar k=(k_1+k_2)/2$, $\bar\omega=(\omega_1+\omega_2)/2$, $\Delta k=k_2-k_1$ and $\Delta\omega=\omega_2-\omega_1$. The [superposition principle](vector-space.md#superposition-principle) gives the exact identity

$$
a\cos(k_1x-\omega_1t)+a\cos(k_2x-\omega_2t)=2a\cos\!\left(\frac{\Delta k\,x-\Delta\omega\,t}{2}\right)\cos(\bar kx-\bar\omega t).
$$

The periodic [wave envelope](#envelope-waves) has speed $\Delta\omega/\Delta k$, approaching [group velocity](#group-velocity) as the two [wavenumbers](#wavenumber) coalesce, while the carrier [wave phase](physics.md#phase-waves) has speed $\bar\omega/\bar k$. Two tones alone form an infinite beat train, not a localized [wave packet](#wave-packet). The figure shows an exact two-tone [surface gravity wave](fluid-mechanics.md#surface-gravity-wave) model with dimensionless $\omega=\sqrt{k}$: $k_1=0.9$, $k_2=1.1$. Its carrier [phase velocity](#phase-velocity) is approximately $0.99875$, its finite-difference envelope velocity approximately $0.50063$, and $\omega'(1)=0.5$ is the limiting [group velocity](#group-velocity). The marked carrier phase line need not coincide exactly with a maximum of the full modulated wave.

<a id="image-exact-analytical-two-tone-gravity-wave-model-carrier-phase-advances-through-a-slower-periodic-envelope"></a>
![](phase-group-dispersion-beats.png)

**[Figure 13](#image-exact-analytical-two-tone-gravity-wave-model-carrier-phase-advances-through-a-slower-periodic-envelope). Exact analytical two-tone gravity-wave model: carrier phase advances through a slower periodic envelope**.

The deep-water [surface gravity wave](fluid-mechanics.md#surface-gravity-wave) therefore has $c_g=c_p/2$, whereas the deep-water [capillary wave](fluid-mechanics.md#capillary-wave) limit has $c_g=3c_p/2$: crests can drift either forward or backward relative to a [wave envelope](#envelope-waves). For finite-depth [surface gravity waves](fluid-mechanics.md#surface-gravity-wave), differentiating the [dispersion relation](#dispersion-relation) gives

$$
c_g=\frac{c_p}{2}\left(1+\frac{2kh}{\sinh(2kh)}\right),\qquad k>0.
$$

Here $\sinh$ is the [hyperbolic sine](calculus.md#hyperbolic-sine). The shallow-water limit has $c_g\simeq c_p\simeq\sqrt{gh}$; the deep-water limit has $c_g\simeq c_p/2$.[equations 6.8–6.11](physics-bibliography.md#free-surface-water-waves-13-012-hydrodynamics-for-ocean-engineers-reading-5-by-a-h-techet)

In the wave tank, produce a finite train with a smooth turn-on and turn-off and time the same [wave envelope](#envelope-waves) feature at two probes separated by distance $L$; its transit estimate is $L/\Delta t$. Independently follow [wave crests](#wave-crest) through that train. Techet's 2003 lab asks students to observe a deep-water train's foremost crest disappearing as the group moves forward, and to compare deep- and shallow-water cases. The interpretation is that a [wave crest](#wave-crest) overtakes the slower [wave envelope](#envelope-waves), dwindling at its front while other crests become visible at its rear. This is a qualitative expected observation in the teaching protocol, not a published set of measured curves.[Waves, phase speed, and group speed (13.012 Hydrodynamics for Ocean Engineers, Laboratory 1) by A. H. Techet](physics-bibliography.md#waves-phase-speed-and-group-speed-13-012-hydrodynamics-for-ocean-engineers-laboratory-1-by-a-h-techet)

A useful controlled version keeps the paddle [wave amplitude](physics.md#wave-amplitude) small, records $h$ and $\lambda$, and checks both $ka\ll1$ and $a/h\ll1$. Compare runs with $kh\gg1$ and $kh\ll1$, rather than assuming every ripple tank is shallow relative to every [wavelength](#wavelength). Increase train duration at fixed central [frequency](physics.md#frequency) to narrow its spectrum, and check that the envelope transit estimate stabilizes. Calibrate both probes, sample fast enough to resolve the carrier, and compare records before reflected waves return; an absorbing beach reduces this contamination. A current changes laboratory velocities, large [wave amplitudes](physics.md#wave-amplitude) introduce nonlinear effects, and very short [wavelengths](#wavelength) require [surface tension](fluid-mechanics.md#surface-tension). Strong [damping](#damping) or noticeable reshaping makes the chosen threshold or peak an unreliable marker of simple [group velocity](#group-velocity). These are proposed controls and model limits, not claims that the cited lab measured every correction.

Three velocities should consequently be kept separate. The [group velocity](#group-velocity) predicts narrow-band [wave envelope](#envelope-waves) motion. An energy-transport velocity is [energy flux](physics.md#energy-flux) divided by [energy density](statistical-physics.md#energy-density), using the appropriate time average; it agrees with [group velocity](#group-velocity) in standard lossless linear wave models when all stored [energy](classical-mechanics.md#energy) is included.[Mathematical Methods in Nanophotonics, MIT 18.369, Spring 2016 — lectures 18–19 by Steven G. Johnson](physics-bibliography.md#mathematical-methods-in-nanophotonics-mit-18-369-spring-2016-lectures-18-19-by-steven-g-johnson) A signal-front velocity concerns the earliest response to a new disturbance and requires a causal model over its full spectrum. A strictly band-limited [wave packet](#wave-packet) has no sharply bounded onset, and a mathematical two-tone envelope cannot test front arrival. In strongly absorbing or broadband propagation, a single [group velocity](#group-velocity) need not describe the observed peak, energy transport, or first detectable response. A complex $\omega$ or $k$ also prevents interpreting its derivative as an ordinary real transport velocity without further analysis.

In particular, an unusually large or negative [group velocity](#group-velocity) from pulse reshaping does not establish superluminal information transmission. For the causal dielectric model analysed by Fitzpatrick, the field ahead of the front vanishes for $t<x/c$, even when its [phase velocity](#phase-velocity) exceeds the vacuum [speed of light](special-relativity.md#speed-of-light) $c$. That result concerns the electromagnetic model's [causality](special-relativity.md#causality); the ideal water-wave diagrams above contain no relativistic signal-front claim.[equations 871–873](physics-bibliography.md#wave-front-propagation-by-richard-fitzpatrick)

Finally, zero [wavenumber](#wavenumber) requires care: the positive-frequency [wave equation](wave-equation.md) branch $c|k|$ is not differentiable at $k=0$, so it has no unique [group velocity](#group-velocity) there, although its one-sided values are $\pm c$. A smooth gapped branch such as the [Klein-Gordon equation](#klein-gordon-equation) instead has $\omega'(0)=0$ despite undefined [phase velocity](#phase-velocity) at $k=0$. The same signed branch must be used in both derivatives and ratios; a negative [group velocity](#group-velocity) means an envelope moving in the negative coordinate direction, not a negative elapsed time. The practical value of [group velocity](#group-velocity) is precisely this translation between a local slope on a [dispersion diagram](#dispersion-diagram) and a measurable packet transit, with its assumptions made explicit.

The [Gaussian envelope in a Klein-Gordon medium](#gaussian-envelope-in-a-klein-gordon-medium) supplies a quantitative next step: the first [derivative](calculus.md#derivative) translates the [wave envelope](#envelope-waves), the second [derivative](calculus.md#derivative) spreads it, and higher [derivatives](calculus.md#derivative) limit that approximation. At finite spectral width, a peak's measured speed need not equal the [group velocity](#group-velocity) at the central [wavenumber](#wavenumber). Neither a peak nor a fixed fraction of its height generally identifies [front velocity](#front-velocity).

#### Front velocity

↑ **Parent:** [Phase velocity and group velocity](#phase-velocity-and-group-velocity)

The [front velocity](#front-velocity) is the propagation speed of the earliest boundary of a newly introduced disturbance's [support](function.md#support). It asks when an initially unaffected observer can first respond, whereas [group velocity](#group-velocity) asks how a narrow [wave envelope](#envelope-waves) translates. A detector threshold defines a practical arrival time, but can miss arbitrarily small earlier responses; a packet peak is another distinct timing convention. In a causal dielectric model, a high-[angular frequency](classical-mechanics.md#angular-frequency) contour argument gives exactly zero field for $t<x/c$, even when [phase velocity](#phase-velocity) exceeds $c$. This is a statement about that model's [relativistic causality](special-relativity.md#relativistic-causality), not a universal identification of [group velocity](#group-velocity) with [front velocity](#front-velocity).[equations 871–873 and the paragraph following equation 887: zero field ahead of the causal front](physics-bibliography.md#wave-front-propagation-by-richard-fitzpatrick)

For the stipulated [Klein-Gordon equation](#klein-gordon-equation) with compactly supported real [Cauchy data](partial-differential-equation.md#cauchy-data), [front velocity](#front-velocity) is bounded by $c$, and $c$ is the model's maximal speed of influence. A short [energy method](numerical-analysis.md#energy-method) outline uses

$$
e=\frac12\left(u_t^2+c^2u_x^2+\omega_0^2u^2\right),\qquad
J=-c^2u_tu_x,\qquad
\partial_te+\partial_xJ=0,\qquad |J|\le ce.
$$

Integration outside an expanding interval shows that zero initial [energy](classical-mechanics.md#energy) there remains zero. Thus initial [support](function.md#support) in $[-a,a]$ cannot influence $x>a$ before $t=(x-a)/c$. The positive [energy density](statistical-physics.md#energy-density) includes the restoring term $\omega_0^2u^2/2$: this adds oscillation behind the front without extending its [domain of dependence](partial-differential-equation.md#domain-of-dependence). A particular disturbance may fail to excite the leading boundary, so the maximal speed is not a promise of a detectable response for every source.

A [Gaussian function](calculus.md#gaussian-function) is nonzero arbitrarily far away, so the [Gaussian envelope in a Klein-Gordon medium](#gaussian-envelope-in-a-klein-gordon-medium) has no sharp initial [support](function.md#support) boundary. Its small distant tails are already in the initial data. Likewise, keeping only a narrow interval of the [frequency spectrum](fourier-analysis.md#frequency-spectrum) cannot reproduce an exact abrupt onset. Cutting off a Gaussian tail changes its [Fourier transform](analysis.md#fourier-transform) and the accompanying initial [velocity](classical-mechanics.md#velocity); it is a different initial-value problem. The [exponential initial-velocity tail for the Klein-Gordon equation](#exponential-initial-velocity-tail-for-the-klein-gordon-equation) is another concrete example of a pre-existing tail outside the main disturbance.

The water-tank measurement in [phase velocity](#phase-velocity) records [free surface](fluid-mechanics.md#free-surface) elevation with calibrated resistance probes and uses a ruler and stopwatch for an independent check. The inspected protocol calls the front or back of a group a timing feature. That visible edge establishes an envelope transit estimate, not the first nonzero disturbance in the sense of [front velocity](#front-velocity).[p. 1, Equipment; p. 2, task 2; p. 3, tasks 5–6: apparatus, calibration and group-feature timing](physics-bibliography.md#surface-waves-kinematics-mit-2-016-hydrodynamics-by-massachusetts-institute-of-technology-2-016-course-staff) A proposed additional control would repeat the transit fit at several detection thresholds and train durations, using matched probe calibration and the same [sampling rate](#sampling-rate). Dependence on the threshold diagnoses [wave envelope](#envelope-waves) reshaping or limited sensitivity; records should be compared before reflections return. Such a test could expose limitations of a [group velocity](#group-velocity) estimate, but would not establish an exact causal front or validate the stipulated [Klein-Gordon equation](#klein-gordon-equation) for water waves.

#### Information velocity

↑ **Parent:** [Phase velocity and group velocity](#phase-velocity-and-group-velocity)

An [information velocity](#information-velocity) must specify what counts as a newly distinguishable message and how it is detected. In a causal model, receivers cannot distinguish two otherwise identical preparations before their difference can arrive. [Front velocity](#front-velocity) therefore bounds the arrival of genuinely new changes when the model has a finite [domain of dependence](partial-differential-equation.md#domain-of-dependence). [Group velocity](#group-velocity) can estimate the delay of a weakly distorted narrow [wave packet](#wave-packet), but it is not a universal speed of information: [damping](#damping), amplification and reshaping can move the peak without advancing the first possible response. A Gaussian peak shift alone does not test [relativistic causality](special-relativity.md#relativistic-causality).[equations 871–873 and discussion after equation 887: earliest response versus phase propagation](physics-bibliography.md#wave-front-propagation-by-richard-fitzpatrick)

#### Crest and trough

↑ **Parent:** [Phase velocity and group velocity](#phase-velocity-and-group-velocity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Crest_and_trough)

The [wave crest](#wave-crest) and [wave trough](#wave-trough) are respectively the highest and lowest displacements in a [wave](physics.md#wave).

##### Wave crest

↑ **Parent:** [Crest and trough](#crest-and-trough)

A wave crest is a [local maximum](analysis.md#local-maximum) of the wave's displacement. In a monochromatic travelling [wave](physics.md#wave) it lies at a fixed phase and propagates at the [phase velocity](#phase-velocity).

##### Wave trough

↑ **Parent:** [Crest and trough](#crest-and-trough)

A wave trough is a [local minimum](analysis.md#local-minimum) of the wave's displacement.

#### Wave packet

↑ **Parent:** [Phase velocity and group velocity](#phase-velocity-and-group-velocity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wave_packet)

A [wave packet](#wave-packet) is a localized [superposition](vector-space.md#superposition-principle) of [Fourier modes](fourier-analysis.md#fourier-mode). In a narrow packet, nearby [wavenumbers](#wavenumber) interfere to produce a slowly varying [wave envelope](#envelope-waves) around a rapid [carrier wave](#carrier-wave). Its leading translation is governed by [group velocity](#group-velocity); the carrier's [wave phase](physics.md#phase-waves) follows [phase velocity](#phase-velocity). Localized does not necessarily mean [compact support](function.md#compact-support): a [Gaussian function](calculus.md#gaussian-function) decays rapidly but extends over the whole line. The [Gaussian envelope in a Klein-Gordon medium](#gaussian-envelope-in-a-klein-gordon-medium) gives an original example with both translation and spreading.

##### Envelope (waves)

↑ **Parent:** [Wave packet](#wave-packet)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Envelope_(waves))

A [wave envelope](#envelope-waves) is a slowly varying [wave amplitude](physics.md#wave-amplitude) multiplying a rapidly oscillating [carrier wave](#carrier-wave). For a complex wavefield $\psi=A(x,t)e^{i(k_0x-\omega_ct)}$, its nonnegative amplitude envelope is $|A|=|\psi|$; the complex $A$ can also encode a slowly varying [wave phase](physics.md#phase-waves). This choice distinguishes the amplitude envelope from a signed modulation factor, such as the cosine factor in a two-tone [superposition](vector-space.md#superposition-principle). A slowly varying [wave envelope](#envelope-waves) is useful when the carrier's [wavelength](#wavelength) and [period](mathematics.md#period-of-a-function) are short compared with its variation scales. Strong overlap between distinct packets or a broad [frequency spectrum](fourier-analysis.md#frequency-spectrum) can spoil a unique carrier-envelope interpretation.

##### Carrier wave

↑ **Parent:** [Wave packet](#wave-packet)

A [carrier wave](#carrier-wave) is the rapid reference oscillation in a modulated [wave](physics.md#wave). In the narrow-packet representation $\psi=A(x,t)e^{i(k_0x-\omega_ct)}$, choose $k_0$ near the centre of the [frequency spectrum](fourier-analysis.md#frequency-spectrum) and $\omega_c=\omega(k_0)$ on its [dispersion relation](#dispersion-relation). Its constant-[wave phase](physics.md#phase-waves) reference moves at [phase velocity](#phase-velocity) $\omega_c/k_0$. This reference need not coincide with a [local maximum](analysis.md#local-maximum) of the complete real wavefield when the [wave envelope](#envelope-waves) varies. Moving the reference $k_0$ shifts some slow [wave phase](physics.md#phase-waves) into $A$ without changing $\psi$.

##### Gaussian envelope in a Klein-Gordon medium

↑ **Parent:** [Wave packet](#wave-packet)

For the stipulated [Klein-Gordon packet velocities](#klein-gordon-packet-velocities), take the original normalized spectral amplitude

$$
a(k)=\frac{1}{\sqrt{2\pi}\sigma}\exp\!\left[-\frac{(k-k_0)^2}{2\sigma^2}\right],\qquad
\psi(x,t)=\int_{\mathbb R}a(k)e^{i[kx-\omega(k)t]}\,dk,
$$

with $k_0>0$ and $0<\sigma\ll k_0$. Here $\sigma$ is the width of the spectral amplitude, not the [standard deviation](variance.md#standard-deviation) of its squared magnitude. Initially $\psi(x,0)=e^{-\sigma^2x^2/2}e^{ik_0x}$, a [Gaussian function](calculus.md#gaussian-function) multiplying a [carrier wave](#carrier-wave). Taking $u=\operatorname{Re}\psi$ gives a real solution of the [Klein-Gordon equation](#klein-gordon-equation) with the corresponding initial [velocity](classical-mechanics.md#velocity). The tiny negative-$k$ tail is retained in this exact integral; the statement that it is mainly right-going is a narrow-spectrum approximation, not a claim of strictly positive [wavenumbers](#wavenumber).

<a id="image-original-klein-gordon-packet-evolution-exact-spectral-integral-slower-envelope-and-carrier-phase-reference"></a>
![](klein-gordon-gaussian-carrier-envelope-evolution.png)

**[Figure 14](#image-original-klein-gordon-packet-evolution-exact-spectral-integral-slower-envelope-and-carrier-phase-reference). Original Klein-Gordon packet evolution: exact spectral integral, slower envelope and carrier phase reference**.

The dimensionless figure uses $c=\omega_0=k_0=1$ and $\sigma=0.18$ at $t=0,4,8$. Blue curves are $\operatorname{Re}\psi$, orange bounds are $\pm|\psi|$, and the marked [carrier wave](#carrier-wave) reference is $x=v_pt$; it need not be a crest of the full wavefield. The dashed envelope-centre reference $x=v_gt$ is a leading approximation. These are calculated curves, not experimental records. The exact [dispersion relation](#dispersion-relation) makes the packet slightly asymmetric; a quadratic approximation predicts symmetric broadening about $v_gt$.

The first-order [Taylor expansion](calculus.md#taylor-expansion) translates the initial [wave envelope](#envelope-waves) without changing its shape. Retaining curvature instead gives

$$
\omega(k)\simeq\omega_c+v_gq+\frac12\beta q^2,\qquad q=k-k_0,\qquad
\beta=\omega''(k_0)=\frac{c^2\omega_0^2}{\omega_c^3}>0.
$$

The distinction between translation and curvature-driven spreading is the same one exposed by the Gaussian pulse calculation in [Pulse Propagation by Richard Fitzpatrick](physics-bibliography.md#pulse-propagation-by-richard-fitzpatrick) (equations 9.8–9.18). Its first-order approximation is not an assertion that a dispersive packet keeps its shape indefinitely.

Evaluating the quadratic [Gaussian integral](calculus.md#gaussian-integral) gives the original approximation

$$
\psi_2(x,t)=\frac{e^{i(k_0x-\omega_ct)}}{\sqrt{1+i\beta t\sigma^2}}
\exp\!\left[-\frac{\sigma^2(x-v_gt)^2}{2(1+i\beta t\sigma^2)}\right],
$$

and hence

$$
|\psi_2(x,t)|=(1+\beta^2t^2\sigma^4)^{-1/4}
\exp\!\left[-\frac{(x-v_gt)^2}{2L(t)^2}\right],\qquad
L(t)=\frac{\sqrt{1+\beta^2t^2\sigma^4}}{\sigma}.
$$

Here $L$ is the amplitude width: the [standard deviation](variance.md#standard-deviation) of the normalized intensity $|\psi_2|^2$ is $L/\sqrt2$. The peak falls as the packet widens, while $\int|\psi_2|^2dx$ stays constant. This conserved integral is not the complete physical [wave energy](#wave-energy) of the [Klein-Gordon equation](#klein-gordon-equation).

Rigid translation requires $|\beta|t\sigma^2\ll1$. The quadratic approximation can allow that quantity to be order one, but still requires the accumulated neglected cubic [wave phase](physics.md#phase-waves) to be small over the appreciable spectrum, for example $(t/6)\sup_{|q|\le3\sigma}|\omega'''(k_0+q)|(3\sigma)^3\ll1$. This sufficient check controls only the stated three-width spectral window; the Gaussian tails must also be negligible at the required accuracy. Higher [derivatives](calculus.md#derivative) or very long times require returning to the exact spectral integral. The width $L(t)$ is therefore a controlled local approximation; it neither predicts [front velocity](#front-velocity) nor establishes a universal identity between [group velocity](#group-velocity) and [information velocity](#information-velocity).

#### Ninth-order dispersive advection equation

↑ **Parent:** [Phase velocity and group velocity](#phase-velocity-and-group-velocity)

For

$$
\phi_t+U\phi_x+\frac19\phi_{xxxxxxxxx}=0,
$$

the dispersion relation is $\omega=Uk+k^9/9$, so $c_p=U+k^8/9$ and $c_g=U+k^8$.

## Klein-Gordon equation

↑ **Parent:** [Wave equation](wave-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Klein–Gordon_equation)

The one-dimensional Klein-Gordon equation

$$
\phi_{tt}-c^2\phi_{xx}+A^2c^2\phi=0
$$

has positive-frequency dispersion relation $\omega(k)=c\sqrt{k^2+A^2}$.

### Exponential initial-velocity tail for the Klein-Gordon equation

↑ **Parent:** [Klein-Gordon equation](#klein-gordon-equation)

For $u_{tt}=u_{xx}-u$ with $u(x,0)=0$ and $u_t(x,0)=e^{-|x|}$, the solution outside $|x|\leq t$ is exactly $te^{-|x|}$. On the positive half-line, $te^{-x}$ satisfies both the equation and initial data; the [finite propagation speed](#finite-propagation-speed) limits dependence at $x>t$ to positive initial points. Uniqueness on this [domain of dependence](partial-differential-equation.md#domain-of-dependence) proves the formula there, and reflection gives the negative half-line. The exterior tail is nonzero because the initial velocity is not compactly supported.

### Stationary-phase asymptotic of a Klein-Gordon wave along a subluminal ray

↑ **Parent:** [Klein-Gordon equation](#klein-gordon-equation)

For zero initial velocity and Fourier amplitude $a(k)$, observation along $x=Vt$ with $0\leq V<c$ selects the two stationary wavenumbers $\pm k_0$, where

$$
k_0=\frac{AV}{\sqrt{c^2-V^2}}.
$$

Writing $s=\sqrt{c^2-V^2}$, the leading oscillation has angular frequency $As$ and amplitude proportional to $t^{-1/2}$.

#### Upward zero crossings of an oscillatory stationary-phase tail

↑ **Parent:** [Stationary-phase asymptotic of a Klein-Gordon wave along a subluminal ray](#stationary-phase-asymptotic-of-a-klein-gordon-wave-along-a-subluminal-ray)

If the leading asymptotic is $Ct^{-1/2}\cos(\Omega t+\gamma)$ with $C>0$, its upward zero crossings satisfy

$$
\Omega t+\gamma=\frac{3\pi}{2}+2\pi n
$$

to leading order.

## ↑ Ancestors (5)

1. [Partial differential equation](partial-differential-equation.md)
2. [Analysis](analysis.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (118)

- [Acoustic dipole](linear-acoustics.md#acoustic-dipole)
- [Acoustic monopole](linear-acoustics.md#acoustic-monopole)
- [Acoustic multipole source](linear-acoustics.md#acoustic-multipole-source)
- [Acoustic time-of-flight speed measurement](#acoustic-time-of-flight-speed-measurement)
- [Commutation vector field for the wave equation](#commutation-vector-field-for-the-wave-equation)
- [D'Alembert formula with initial velocity](#d-alembert-formula-with-initial-velocity)
- [Dispersion relation](#dispersion-relation)
- [Eikonal equation for a variable-speed wave](optics.md#eikonal-equation-for-a-variable-speed-wave)
- [Elastic wave](#elastic-wave)
- [Electromagnetic wave](electromagnetism.md#electromagnetic-wave)
- [Entire wave cosine multiplier](#entire-wave-cosine-multiplier)
- [Finite propagation in porous-medium diffusion](diffusion-equation.md#finite-propagation-in-porous-medium-diffusion)
- [Focusing semilinear wave equation](#focusing-semilinear-wave-equation)
- [Group velocity](#group-velocity)
- [Harmonic reduction of the vacuum Einstein equations](numerical-relativity.md#harmonic-reduction-of-the-vacuum-einstein-equations)
- [Hydrostatic response to a localized horizontal force](geophysical-fluid-dynamics.md#hydrostatic-response-to-a-localized-horizontal-force)
- [Impulsively struck fixed-end string](#impulsively-struck-fixed-end-string)
- [Infinite propagation speed](diffusion-equation.md#infinite-propagation-speed)
- [Initial displacement](differential-equation.md#initial-displacement)
- [Initial velocity](differential-equation.md#initial-velocity)
- [Klainerman-Sobolev inequality](#klainerman-sobolev-inequality)
- [Lighthill acoustic analogy](linear-acoustics.md#lighthill-acoustic-analogy)
- [Local wave energy estimate](partial-differential-equation.md#local-wave-energy-estimate)
- [Localized ordinary differential equation blowup for a wave equation](#localized-ordinary-differential-equation-blowup-for-a-wave-equation)
- [Low-frequency decomposition of the wave propagator](#low-frequency-decomposition-of-the-wave-propagator)
- [Mass-injection term in the acoustic analogy](linear-acoustics.md#mass-injection-term-in-the-acoustic-analogy)
- [Method of descent for the wave equation](#method-of-descent-for-the-wave-equation)
- [Nambu–Goto equations of motion](string-theory.md#nambu-goto-equations-of-motion)
- [Normal mode](#normal-mode)
- [One-dimensional wave equation](#one-dimensional-wave-equation)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-59.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-66.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-3.md#2a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-67.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-3.md#12d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-3.md#12d/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-4.md#2d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-1.md#17b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-49.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-4.md#5h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-54.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-54.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-4.md#30a/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-4.md#30a/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4.md#5b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2.md#30a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-4.md#30c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-52.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-2.md#8c/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-1.md#38a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-2.md#38a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-1.md#35b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-44.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-74.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1.md#39b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-51.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-68.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-4.md#5c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-52.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-70.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-2.md#6b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-4.md#14b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-5.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-67.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-75.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4.md#29e/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-10.md#1/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-10.md#1/2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-10.md#1/3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-10.md#1/4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-10.md#2/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-43.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-52.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-2.md#16a/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-3.md#15b/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4.md#14a/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-336.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-2.md#8c/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-1.md#14b/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-105.md#1/1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-311.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-1.md#39c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-105.md#4/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-306.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-306.md#1/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-309.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1.md#40b/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1.md#40b/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2.md#13e/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-2.md#6a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-1.md#13c/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-1.md#40c/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-327.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ia/paper-2.md#11f/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3.md#14a/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3.md#32e/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-105.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-306.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-336.md#1/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-105.md#3/c/solution)
- [Plane-wave string mode frequency](string-theory.md#plane-wave-string-mode-frequency)
- [Rectangular pulse splitting under the wave equation](#rectangular-pulse-splitting-under-the-wave-equation)
- [Reflected-step solution of the wave equation](#reflected-step-solution-of-the-wave-equation)
- [Regular time-harmonic spherical wave](#regular-time-harmonic-spherical-wave)
- [Scalar equation of Brans-Dicke theory](general-relativity.md#scalar-equation-of-brans-dicke-theory)
- [Scaling vector field](#scaling-vector-field)
- [Shrinking cone energy argument](#shrinking-cone-energy-argument)
- [Straight rotating string with one fixed endpoint](string-theory.md#straight-rotating-string-with-one-fixed-endpoint)
- [String sigma model in an isotropic plane wave](string-theory.md#string-sigma-model-in-an-isotropic-plane-wave)
- [Travel-time coordinate for a one-dimensional variable-speed wave equation](partial-differential-equation.md#travel-time-coordinate-for-a-one-dimensional-variable-speed-wave-equation)
- [Vector field method for wave equations](#vector-field-method-for-wave-equations)
- [Wave-action transport for a variable-speed wave](optics.md#wave-action-transport-for-a-variable-speed-wave)
- [Wave energy](#wave-energy)
- [Wave energy estimate](partial-differential-equation.md#wave-energy-estimate)
- [Wave speed](#wave-speed)
- [Winding-supported circular string](string-theory.md#winding-supported-circular-string)
