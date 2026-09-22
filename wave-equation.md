# Wave equation

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wave_equation)

The wave equation models finite-speed propagation and second-order oscillation.

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
  - [Slowness](#slowness)
- [Kirchhoff formula](#kirchhoff-formula)
  - [Method of descent for the wave equation](#method-of-descent-for-the-wave-equation)
  - [Strong Huygens principle](#strong-huygens-principle)
- [Finite propagation speed](#finite-propagation-speed)
  - [Weak Huygens principle](#weak-huygens-principle)
  - [Shrinking cone energy argument](#shrinking-cone-energy-argument)
  - [Characteristic diamond for speed one minus y squared](#characteristic-diamond-for-speed-one-minus-y-squared)
- [Radiation field](#radiation-field)
  - [Scattering map](#scattering-map)
- [One-dimensional wave equation](#one-dimensional-wave-equation)
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
  - [Node (physics)](#node-physics)
- [Fourier transform method for the wave equation](#fourier-transform-method-for-the-wave-equation)
  - [Low-frequency decomposition of the wave propagator](#low-frequency-decomposition-of-the-wave-propagator)
  - [Entire wave cosine multiplier](#entire-wave-cosine-multiplier)
- [D'Alembert's formula](#d-alembert-s-formula)
  - [Rectangular pulse splitting under the wave equation](#rectangular-pulse-splitting-under-the-wave-equation)
  - [D'Alembert formula with initial velocity](#d-alembert-formula-with-initial-velocity)
    - [Central zero region for odd compactly supported initial velocity](#central-zero-region-for-odd-compactly-supported-initial-velocity)
- [Wavenumber](#wavenumber)
  - [Wavelength](#wavelength)
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
    - [Phase-group orthogonality for degree-zero dispersion](#phase-group-orthogonality-for-degree-zero-dispersion)
    - [Phase velocity](#phase-velocity)
      - [Horizontal phase velocity](#horizontal-phase-velocity)
      - [Phase speed](#phase-speed)
    - [Group velocity](#group-velocity)
    - [Crest and trough](#crest-and-trough)
      - [Wave crest](#wave-crest)
      - [Wave trough](#wave-trough)
    - [Wave packet](#wave-packet)
      - [Envelope (waves)](#envelope-waves)
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

The wave speed $c$ is the propagation speed in a wave equation such as $u_{tt}=c^2\nabla^2u$.

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

Finite propagation speed means that data outside the backward light cone of a spacetime point cannot affect the solution at that point.

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

The one-dimensional wave equation has left-moving and right-moving travelling-wave solutions. Their superposition is described by the [D'Alembert formula](#d-alembert-s-formula) and remains valid distributionally for [locally integrable profiles](distribution-theory.md#locally-integrable-function).

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

### Critical damping

↑ **Parent:** [Damping](#damping)

Critical damping occurs when a second-order mode has a repeated real characteristic root. It returns to equilibrium without oscillating and as quickly as possible among nonoscillatory regimes.

## Wave equation on a string

↑ **Parent:** [Wave equation](wave-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wave_equation_on_a_string)

A stretched uniform string obeys y\_tt=c^2 y\_xx with wave speed equal to the square root of tension over density.

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

A normal mode oscillates at one frequency with a fixed spatial eigenfunction.

### Mode shape

↑ **Parent:** [Normal mode](#normal-mode)

The mode shape is the fixed spatial [eigenfunction](linear-operator-theory.md#eigenfunction) multiplying the temporal factor of a [normal mode](#normal-mode). It is determined by the governing [differential equation](differential-equation.md) and [boundary conditions](differential-equation.md#boundary-condition), and may be normalized by a chosen amplitude or energy convention.

### Countability of elastic eigenfrequencies

↑ **Parent:** [Normal mode](#normal-mode)

Distinct squared traction-free [eigenfrequencies](#eigenfrequency) in a bounded lossless elastic body have [eigenfunctions](linear-operator-theory.md#eigenfunction) [orthogonal](linear-algebra.md#orthogonal-vectors) in $L^2(\mathcal D,\rho\,dV)^3$, by the [Betti identity for elastodynamic fields](continuum-mechanics.md#betti-identity-for-elastodynamic-fields). Normalize one field from each [eigenspace](linear-operator-theory.md#eigenspace). This is an [orthonormal set](linear-algebra.md#orthonormal-set) in a [separable Hilbert space](hilbert-space.md#separable-hilbert-space), so it is countable: disjoint balls of radius less than $1/\sqrt2$ around its unit vectors must contain distinct points of a countable dense set. Positive and negative [frequency](physics.md#frequency) partners add at most a factor of two. This argument proves countability without requiring a separate compact-resolvent proof.

### Eigenfrequency

↑ **Parent:** [Normal mode](#normal-mode)

The temporal frequency of a [normal mode](#normal-mode). In $\dot z=iAz$, a real [eigenvalue](linear-operator-theory.md#eigenvalue) of $A$ is a signed eigenfrequency; its positive imaginary part after damping gives exponential decay in $e^{i\lambda t}$.

### Modal energy distribution

↑ **Parent:** [Normal mode](#normal-mode)

[Orthogonality](linear-algebra.md#orthogonal-vectors) separates total quadratic [wave energy](#wave-energy) into a sum of independent modal energies.

### Node (physics)

↑ **Parent:** [Normal mode](#normal-mode)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Node_(physics))

A node is a point where a [standing wave](physics.md#standing-wave) has minimum [amplitude](physics.md#wave-amplitude). For an ideal standing [normal mode](#normal-mode), its [eigenfunction](linear-operator-theory.md#eigenfunction) vanishes there at all times.

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

The Cauchy problem $u_{tt}=c^2u_{xx}$ has

$$
u(x,t)=\frac{f(x-ct)+f(x+ct)}2+\frac1{2c}\int_{x-ct}^{x+ct}g(y)dy.
$$

### Rectangular pulse splitting under the wave equation

↑ **Parent:** [D'Alembert's formula](#d-alembert-s-formula)

A rectangular initial displacement with zero initial velocity splits into two equal half-height copies moving in opposite directions. The [D'Alembert formula](#d-alembert-s-formula) reads $u(x,t)=[u_0(x+ct)+u_0(x-ct)]/2$. Overlap adds the heights; separated copies each retain the original width. For discontinuous fronts the formula defines a [weak solution](partial-differential-equation.md#weak-solution) of the [wave equation](wave-equation.md).

<h3 id="d-alembert-formula-with-initial-velocity">D'Alembert formula with initial velocity</h3>

↑ **Parent:** [D'Alembert's formula](#d-alembert-s-formula)

For $u_{tt}-u_{xx}=0$ with $u(0,x)=0$ and $u_t(0,x)=f(x)$,

$$
u(t,x)=\frac12\int_{x-t}^{x+t}f(y)\,dy.
$$

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

The wavenumber is the spatial angular frequency of a monochromatic wave. A factor $e^{ikx}$ has wavelength $2\pi/|k|$.

### Wavelength

↑ **Parent:** [Wavenumber](#wavenumber)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wavelength)

The wavelength is the spatial period of a monochromatic wave. For angular [wavenumber](#wavenumber) $k$, it is $\lambda=2\pi/|k|$.

## Dispersion relation

↑ **Parent:** [Wave equation](wave-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dispersion_relation)

A dispersion relation gives angular frequency $\omega$ as a function of wavenumber $k$ for monochromatic waves admitted by a linear wave equation.

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

#### Phase-group orthogonality for degree-zero dispersion

↑ **Parent:** [Phase velocity and group velocity](#phase-velocity-and-group-velocity)

If a differentiable [dispersion relation](#dispersion-relation) $\omega(\mathbf k)$ is homogeneous of degree zero at nonzero $\mathbf k$, the [Euler homogeneous function theorem](real-analysis.md#euler-theorem-for-homogeneous-functions) gives $\mathbf k\cdot\nabla_{\mathbf k}\omega=0$. Therefore [phase velocity](#phase-velocity) $\omega\mathbf k/k^2$ is orthogonal to [group velocity](#group-velocity) $\nabla_{\mathbf k}\omega$. The result applies exactly to limiting [inertial waves](geophysical-fluid-dynamics.md#inertial-wave); finite compressibility can alter the dispersion.

#### Phase velocity

↑ **Parent:** [Phase velocity and group velocity](#phase-velocity-and-group-velocity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Phase_velocity)

Phase velocity is the velocity of a surface of constant phase. For a one-dimensional monochromatic wave it is $c_p=\omega/k$.

##### Horizontal phase velocity

↑ **Parent:** [Phase velocity](#phase-velocity)

For phase $kx+mz-\omega t$ with $k\ne0$, hold $z$ fixed: a contour of constant [wave phase](physics.md#phase-waves) advances in $x$ at $\omega/k$. This is the speed at which a tilted [wavefront](optics.md#wavefront) crosses a horizontal line. It differs from the horizontal component of the vector [phase velocity](#phase-velocity), $\omega k/(k^2+m^2)$, which is defined along the [wavevector](continuum-mechanics.md#wavevector).

##### Phase speed

↑ **Parent:** [Phase velocity](#phase-velocity)

The magnitude of the [phase velocity](#phase-velocity) of a real-frequency plane [Fourier mode](fourier-analysis.md#fourier-mode) is $|\omega|/|\mathbf k|$. In an anisotropic medium it depends on the direction of the [wave vector](continuum-mechanics.md#wavevector) and need not equal the [group velocity](#group-velocity) magnitude.

#### Group velocity

↑ **Parent:** [Phase velocity and group velocity](#phase-velocity-and-group-velocity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Group_velocity)

Group velocity is the gradient of angular frequency with respect to wavevector, $\mathbf c_g=\nabla_{\mathbf k}\omega$. It gives the leading propagation velocity of a narrow wave packet.

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

A wave packet is a localized superposition of nearby wavenumbers. Its envelope propagates at the [group velocity](#phase-velocity-and-group-velocity) to leading order.

##### Envelope (waves)

↑ **Parent:** [Wave packet](#wave-packet)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Envelope_(waves))

A wave envelope is a slowly varying amplitude multiplying a rapidly oscillating carrier wave. Its variation describes localization, modulation, growth, or attenuation of the carrier.

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

## ← Incoming links (110)

- [Acoustic dipole](linear-acoustics.md#acoustic-dipole)
- [Acoustic monopole](linear-acoustics.md#acoustic-monopole)
- [Acoustic multipole source](linear-acoustics.md#acoustic-multipole-source)
- [Commutation vector field for the wave equation](#commutation-vector-field-for-the-wave-equation)
- [Eikonal equation for a variable-speed wave](optics.md#eikonal-equation-for-a-variable-speed-wave)
- [Elastic wave](#elastic-wave)
- [Entire wave cosine multiplier](#entire-wave-cosine-multiplier)
- [Finite propagation in porous-medium diffusion](diffusion-equation.md#finite-propagation-in-porous-medium-diffusion)
- [Focusing semilinear wave equation](#focusing-semilinear-wave-equation)
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
- [Winding-supported circular string](string-theory.md#winding-supported-circular-string)
