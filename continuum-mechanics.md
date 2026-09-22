# Continuum mechanics

↑ **Parent:** [Branches of physics](physics.md#branches-of-physics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Continuum_mechanics)

**Table of contents**

- [Anisotropy](#anisotropy)
- [Isotropy](#isotropy)
- [Composite material](#composite-material)
  - [Elastic laminate](#elastic-laminate)
  - [Effective elastic energy](#effective-elastic-energy)
    - [Phase polarization comparison bound](#phase-polarization-comparison-bound)
    - [Reuss elastic approximation](#reuss-elastic-approximation)
    - [Voigt elastic approximation](#voigt-elastic-approximation)
    - [Hill-Mandel energy identity](#hill-mandel-energy-identity)
  - [Volume fraction](#volume-fraction)
  - [Two-point phase correlation function](#two-point-phase-correlation-function)
  - [Effective conductivity](#effective-conductivity)
    - [Self-consistent conductivity approximation](#self-consistent-conductivity-approximation)
    - [Hashin-Shtrikman conductivity variational principle](#hashin-shtrikman-conductivity-variational-principle)
      - [Two-dimensional isotropic polycrystal conductivity](#two-dimensional-isotropic-polycrystal-conductivity)
      - [Hashin-Shtrikman bounds for conductivity](#hashin-shtrikman-bounds-for-conductivity)
    - [Voigt bound](#voigt-bound)
    - [Laminate conductivity](#laminate-conductivity)
    - [Conductivity homogenization](#conductivity-homogenization)
      - [Polarization field of a conductivity inclusion](#polarization-field-of-a-conductivity-inclusion)
        - [Exciting field of a conductivity inclusion](#exciting-field-of-a-conductivity-inclusion)
        - [Spherical conductivity inclusion](#spherical-conductivity-inclusion)
          - [Dilute spherical-inclusion conductivity](#dilute-spherical-inclusion-conductivity)
            - [Maxwell approximation for conductivity](#maxwell-approximation-for-conductivity)
            - [Dipole interaction correction to effective conductivity](#dipole-interaction-correction-to-effective-conductivity)
      - [Periodic conductivity cell problem](#periodic-conductivity-cell-problem)
        - [Two-scale expansion for periodic conductivity](#two-scale-expansion-for-periodic-conductivity)
          - [Boundary corrector in periodic homogenization](#boundary-corrector-in-periodic-homogenization)
- [Plasticity (physics)](#plasticity-physics)
  - [Von Mises yield criterion](#von-mises-yield-criterion)
  - [Associated flow rule](#associated-flow-rule)
  - [Perfect plasticity](#perfect-plasticity)
    - [Antiplane perfect plasticity](#antiplane-perfect-plasticity)
      - [Centred antiplane plastic fan](#centred-antiplane-plastic-fan)
    - [Slip-line field theory](#slip-line-field-theory)
      - [Hencky stress relations](#hencky-stress-relations)
        - [Centred slip-line fan at a traction-free V-notch](#centred-slip-line-fan-at-a-traction-free-v-notch)
      - [Geiringer velocity relations](#geiringer-velocity-relations)
      - [Stress characteristics for an anisotropic yield curve](#stress-characteristics-for-an-anisotropic-yield-curve)
      - [Slip line](#slip-line)
- [Continuum thermodynamics](#continuum-thermodynamics)
  - [Reference-configuration jump balances](#reference-configuration-jump-balances)
  - [Thermoelasticity](#thermoelasticity)
    - [Thermoelasticity with a temperature-dependent constraint](#thermoelasticity-with-a-temperature-dependent-constraint)
      - [Linear thermoelasticity with prescribed thermal volume](#linear-thermoelasticity-with-prescribed-thermal-volume)
  - [Clausius-Duhem inequality](#clausius-duhem-inequality)
    - [Coleman-Noll procedure](#coleman-noll-procedure)
    - [Lagrangian entropy inequality](#lagrangian-entropy-inequality)
  - [Lagrangian internal energy balance](#lagrangian-internal-energy-balance)
  - [Internal variable](#internal-variable)
    - [Dissipation potential](#dissipation-potential)
      - [Exponential memory from tensor relaxation](#exponential-memory-from-tensor-relaxation)
    - [Thermodynamic force conjugate to an internal variable](#thermodynamic-force-conjugate-to-an-internal-variable)
- [Deformation (mechanics)](#deformation-mechanics)
  - [Finite strain theory](#finite-strain-theory)
    - [Spectral strain measure](#spectral-strain-measure)
      - [Biot strain tensor](#biot-strain-tensor)
    - [Inverse right Cauchy-Green strain](#inverse-right-cauchy-green-strain)
    - [Green-Lagrange strain tensor](#green-lagrange-strain-tensor)
    - [Plane strain](#plane-strain)
    - [Simple shear](#simple-shear)
    - [Stretch tensor](#stretch-tensor)
      - [Principal stretch](#principal-stretch)
      - [Right stretch tensor](#right-stretch-tensor)
      - [Left stretch tensor](#left-stretch-tensor)
    - [Deformation gradient](#deformation-gradient)
      - [Nanson's formula](#nanson-s-formula)
      - [Multiplicative decomposition of the deformation gradient](#multiplicative-decomposition-of-the-deformation-gradient)
      - [Polar decomposition in continuum mechanics](#polar-decomposition-in-continuum-mechanics)
      - [Right Cauchy-Green deformation tensor](#right-cauchy-green-deformation-tensor)
      - [Left Cauchy-Green deformation tensor](#left-cauchy-green-deformation-tensor)
  - [Deformation map](#deformation-map)
    - [Current configuration](#current-configuration)
    - [Reference configuration](#reference-configuration)
- [Constitutive equation](#constitutive-equation)
  - [Material frame indifference](#material-frame-indifference)
    - [Objective second-rank tensor](#objective-second-rank-tensor)
  - [Stress](#stress)
    - [Work-conjugate stress and strain](#work-conjugate-stress-and-strain)
      - [Symmetric Biot stress](#symmetric-biot-stress)
    - [Mandel stress tensor](#mandel-stress-tensor)
    - [Kirchhoff stress tensor](#kirchhoff-stress-tensor)
    - [Piola-Kirchhoff stress tensors](#piola-kirchhoff-stress-tensors)
      - [Second Piola-Kirchhoff stress tensor](#second-piola-kirchhoff-stress-tensor)
      - [First Piola-Kirchhoff stress tensor](#first-piola-kirchhoff-stress-tensor)
        - [Nominal stress tensor](#nominal-stress-tensor)
    - [Cauchy stress tensor](#cauchy-stress-tensor)
      - [Normal stress](#normal-stress)
      - [Principal stress](#principal-stress)
    - [Deviatoric stress](#deviatoric-stress)
    - [Traction](#traction)
      - [Hydrodynamic torque](#hydrodynamic-torque)
  - [Strain](#strain)
    - [Infinitesimal strain tensor](#infinitesimal-strain-tensor)
- [Velocity gradient](#velocity-gradient)
  - [Velocity divergence](#velocity-divergence)
- [Mass conservation](#mass-conservation)
- [Material derivative](#material-derivative)
  - [Reynolds transport theorem](#reynolds-transport-theorem)
  - [Convective acceleration](#convective-acceleration)
  - [Material acceleration](#material-acceleration)
  - [Eulerian coordinate](#eulerian-coordinate)
  - [Lagrangian coordinate](#lagrangian-coordinate)
  - [Eulerian time average](#eulerian-time-average)
  - [Lagrangian trajectory](#lagrangian-trajectory)
    - [Fluid element](#fluid-element)
    - [Stokes drift](#stokes-drift)
      - [Cross-wave Stokes drift](#cross-wave-stokes-drift)
      - [Initial and mean parcel labels in a surface wave](#initial-and-mean-parcel-labels-in-a-surface-wave)
- [Rayleigh-Taylor instability](#rayleigh-taylor-instability)
  - [Orthogonal-field magnetic Rayleigh-Taylor dispersion relation](#orthogonal-field-magnetic-rayleigh-taylor-dispersion-relation)
    - [Localization condition for the fastest orthogonal-field interface mode](#localization-condition-for-the-fastest-orthogonal-field-interface-mode)
  - [Viscous overturn of a dense crust](#viscous-overturn-of-a-dense-crust)
  - [Finite-depth Rayleigh-Taylor dispersion relation](#finite-depth-rayleigh-taylor-dispersion-relation)
    - [Thin-layer Rayleigh-Taylor growth asymptotics](#thin-layer-rayleigh-taylor-growth-asymptotics)
- [Boundary layer](#boundary-layer)
  - [Laminar plane jet from a line force](#laminar-plane-jet-from-a-line-force)
  - [Laminar skin-friction scaling along a slender swimmer](#laminar-skin-friction-scaling-along-a-slender-swimmer)
  - [Conical sink boundary layer](#conical-sink-boundary-layer)
  - [Similarity profile of an axisymmetric radial viscous free jet](#similarity-profile-of-an-axisymmetric-radial-viscous-free-jet)
  - [Plane laminar jet](#plane-laminar-jet)
    - [Bickley jet](#bickley-jet)
  - [Boundary-layer equation](#boundary-layer-equation)
  - [Turbulent boundary layer](#turbulent-boundary-layer)
    - [Viscous sublayer](#viscous-sublayer)
    - [Monin-Obukhov similarity theory](#monin-obukhov-similarity-theory)
      - [Near-neutral log-linear surface-layer profiles](#near-neutral-log-linear-surface-layer-profiles)
      - [Very stable surface-layer similarity](#very-stable-surface-layer-similarity)
      - [Monin-Obukhov length](#monin-obukhov-length)
    - [Law of the wall](#law-of-the-wall)
      - [Von Kármán constant](#von-karman-constant)
      - [Roughness length](#roughness-length)
  - [Thermal boundary layer](#thermal-boundary-layer)
    - [Boundary-layer renewal model](#boundary-layer-renewal-model)
  - [Boundary-layer scaling](#boundary-layer-scaling)
  - [Two-dimensional boundary-layer equations](#two-dimensional-boundary-layer-equations)
    - [Boundary layer over a linearly stretching sheet](#boundary-layer-over-a-linearly-stretching-sheet)
  - [Flow separation](#flow-separation)
- [Falkner-Skan equation](#falkner-skan-equation)
- [Acoustic energy flux](#acoustic-energy-flux)
  - [Spectral acoustic flux](#spectral-acoustic-flux)
  - [Transmitted velocity potential from a piston through an acoustic interface](#transmitted-velocity-potential-from-a-piston-through-an-acoustic-interface)
- [Burgers vortex](#burgers-vortex)
  - [Burgers vortex sheet](#burgers-vortex-sheet)
  - [Excess dissipation of a Burgers vortex](#excess-dissipation-of-a-burgers-vortex)
  - [Unsteady Burgers-vortex core radius](#unsteady-burgers-vortex-core-radius)
- [Granular material](#granular-material)
  - [Angle of repose](#angle-of-repose)
- [Elasticity (physics)](#elasticity-physics)
  - [Elastic deformation](#elastic-deformation)
  - [Perfectly bonded elastic interface](#perfectly-bonded-elastic-interface)
  - [Static elastic equilibrium](#static-elastic-equilibrium)
  - [Elastic beam](#elastic-beam)
  - [Dead loading](#dead-loading)
  - [Magnetostriction](#magnetostriction)
    - [Isotropic linear magnetostriction vanishes](#isotropic-linear-magnetostriction-vanishes)
  - [Betti identity for elastodynamic fields](#betti-identity-for-elastodynamic-fields)
  - [Shear modulus](#shear-modulus)
  - [Finite elasticity](#finite-elasticity)
    - [Inflation and extension of an incompressible tube](#inflation-and-extension-of-an-incompressible-tube)
    - [Constrained second-variation stability in elasticity](#constrained-second-variation-stability-in-elasticity)
    - [Torque and axial force of a twisted incompressible cylinder](#torque-and-axial-force-of-a-twisted-incompressible-cylinder)
      - [Nominal end traction of a twisted neo-Hookean cylinder](#nominal-end-traction-of-a-twisted-neo-hookean-cylinder)
    - [Twist and inflation of an incompressible tube](#twist-and-inflation-of-an-incompressible-tube)
      - [Neo-Hookean tube pressure under twist and inflation](#neo-hookean-tube-pressure-under-twist-and-inflation)
    - [Inextensible fibre constraint](#inextensible-fibre-constraint)
      - [Two-family inextensible-fibre pure stretch](#two-family-inextensible-fibre-pure-stretch)
      - [Incompressible inextensible-fibre plane strain](#incompressible-inextensible-fibre-plane-strain)
        - [Triangular equilibrium construction for inextensible-fibre plane strain](#triangular-equilibrium-construction-for-inextensible-fibre-plane-strain)
    - [Hyperelastic material](#hyperelastic-material)
      - [Compatibility condition for pure nonlinear transverse waves](#compatibility-condition-for-pure-nonlinear-transverse-waves)
        - [Compatible nonlinear shear energy](#compatible-nonlinear-shear-energy)
      - [Saint Venant–Kirchhoff hyperelastic energy](#saint-venant-kirchhoff-hyperelastic-energy)
      - [Lamé parameters from hyperelastic energy Hessian](#lame-parameters-from-hyperelastic-energy-hessian)
      - [Inflation pressure of a thin incompressible elastic balloon](#inflation-pressure-of-a-thin-incompressible-elastic-balloon)
      - [Incremental elastic moduli](#incremental-elastic-moduli)
        - [Elastic normal-mode energy identity](#elastic-normal-mode-energy-identity)
        - [Strong ellipticity in elasticity](#strong-ellipticity-in-elasticity)
        - [Acoustic tensor](#acoustic-tensor)
      - [Constraint reaction in hyperelastic stress](#constraint-reaction-in-hyperelastic-stress)
        - [Equibiaxial nominal tension of an incompressible sheet](#equibiaxial-nominal-tension-of-an-incompressible-sheet)
      - [Mooney-Rivlin solid](#mooney-rivlin-solid)
      - [Neo-Hookean solid](#neo-hookean-solid)
        - [Homogeneous tensile bifurcation of a neo-Hookean cube](#homogeneous-tensile-bifurcation-of-a-neo-hookean-cube)
      - [Strain energy density](#strain-energy-density)
        - [Nonnegative isotropic elastic strain energy](#nonnegative-isotropic-elastic-strain-energy)
    - [Material isotropy](#material-isotropy)
      - [Coaxiality of isotropic elastic stress](#coaxiality-of-isotropic-elastic-stress)
        - [Equivariance of isotropic principal stresses](#equivariance-of-isotropic-principal-stresses)
        - [Universal simple-shear normal-stress identity](#universal-simple-shear-normal-stress-identity)
  - [Elastic filament](#elastic-filament)
    - [Filament torsional stiffness](#filament-torsional-stiffness)
    - [Intrinsic curvature of an elastic filament](#intrinsic-curvature-of-an-elastic-filament)
      - [Free-end curvature boundary layer](#free-end-curvature-boundary-layer)
      - [Force-extension of an intrinsically curved filament](#force-extension-of-an-intrinsically-curved-filament)
        - [Smooth-curvature high-force extension law](#smooth-curvature-high-force-extension-law)
      - [Quenched intrinsic curvature](#quenched-intrinsic-curvature)
    - [Spatially varying tension in filament bending](#spatially-varying-tension-in-filament-bending)
    - [Thermal covariance of an elastic filament](#thermal-covariance-of-an-elastic-filament)
      - [Rigid-motion-projected thermal covariance of a free filament](#rigid-motion-projected-thermal-covariance-of-a-free-filament)
        - [Curvature-noise representation of a free filament](#curvature-noise-representation-of-a-free-filament)
        - [Free-filament variance with fixed translation and tilt](#free-filament-variance-with-fixed-translation-and-tilt)
      - [Zero-energy filament mode](#zero-energy-filament-mode)
    - [Clamped--clamped bending mode](#clamped-clamped-bending-mode)
    - [Self-adjoint endpoint conditions for filament bending](#self-adjoint-endpoint-conditions-for-filament-bending)
      - [Free-end bending boundary conditions](#free-end-bending-boundary-conditions)
        - [Free-free bending spectrum](#free-free-bending-spectrum)
          - [Stable characteristic equation for free-free bending modes](#stable-characteristic-equation-for-free-free-bending-modes)
    - [Tip-force compliance of a cantilever](#tip-force-compliance-of-a-cantilever)
  - [Elastic energy](#elastic-energy)
    - [Minimum potential energy principle in elasticity](#minimum-potential-energy-principle-in-elasticity)
  - [Linear elasticity](#linear-elasticity)
    - [Mean stress and strain boundary identities](#mean-stress-and-strain-boundary-identities)
      - [Equilibrium contraction of a self-gravitating elastic sphere](#equilibrium-contraction-of-a-self-gravitating-elastic-sphere)
    - [Elastic strain Green operator](#elastic-strain-green-operator)
      - [Isotropic elastic strain Green kernel](#isotropic-elastic-strain-green-kernel)
        - [Constant-shear bulk-modulus inclusion](#constant-shear-bulk-modulus-inclusion)
      - [Directional elastic strain Green operator](#directional-elastic-strain-green-operator)
      - [Elastic polarization](#elastic-polarization)
    - [Bulk modulus](#bulk-modulus)
    - [Antiplane shear](#antiplane-shear)
      - [Steadily moving antiplane shear](#steadily-moving-antiplane-shear)
      - [Complex stress potential for antiplane shear](#complex-stress-potential-for-antiplane-shear)
        - [Hilbert problem for an antiplane crack](#hilbert-problem-for-an-antiplane-crack)
          - [Cauchy solution for a steadily moving semi-infinite antiplane crack](#cauchy-solution-for-a-steadily-moving-semi-infinite-antiplane-crack)
            - [Homogeneous stress-intensity field of a semi-infinite antiplane crack](#homogeneous-stress-intensity-field-of-a-semi-infinite-antiplane-crack)
          - [Antiplane ligament Cauchy solution](#antiplane-ligament-cauchy-solution)
          - [Finite antiplane crack Cauchy solution](#finite-antiplane-crack-cauchy-solution)
    - [Elastic stiffness tensor](#elastic-stiffness-tensor)
      - [Independent elastic stiffness counts](#independent-elastic-stiffness-counts)
        - [Twofold elastic symmetry](#twofold-elastic-symmetry)
    - [Bending moment](#bending-moment)
    - [Elastic membrane](#elastic-membrane)
    - [Euler-Bernoulli beam equation](#euler-bernoulli-beam-equation)
      - [Schrodinger factorization of the elastic beam equation](#schrodinger-factorization-of-the-elastic-beam-equation)
    - [Second moment of area](#second-moment-of-area)
    - [Poisson's ratio](#poisson-s-ratio)
    - [Young's modulus](#young-s-modulus)
    - [Fracture toughness](#fracture-toughness)
    - [Hooke's law](#hooke-s-law)
      - [Spring](#spring)
    - [Elastic plate](#elastic-plate)
      - [Line-forced fluid-loaded bending plate](#line-forced-fluid-loaded-bending-plate)
      - [Flexural wave](#flexural-wave)
        - [Flexural-gravity wave](#flexural-gravity-wave)
          - [Minimum phase speed of a flexural-gravity wave](#minimum-phase-speed-of-a-flexural-gravity-wave)
          - [Dispersion relation of a floating elastic plate](#dispersion-relation-of-a-floating-elastic-plate)
          - [Group-velocity minimum of a flexural-gravity wave](#group-velocity-minimum-of-a-flexural-gravity-wave)
      - [Viscous peeling of an elastic plate](#viscous-peeling-of-an-elastic-plate)
      - [Axisymmetric clamped-plate deflection](#axisymmetric-clamped-plate-deflection)
      - [Bending stiffness](#bending-stiffness)
    - [Nondegenerate one-dimensional elastic material](#nondegenerate-one-dimensional-elastic-material)
    - [Displacement field (mechanics)](#displacement-field-mechanics)
      - [Lagrangian fluid displacement](#lagrangian-fluid-displacement)
      - [Displacement gradient tensor](#displacement-gradient-tensor)
    - [Lamé parameter](#lame-parameter)
      - [Poisson solid](#poisson-solid)
    - [Isotropic linear-elastic energy density](#isotropic-linear-elastic-energy-density)
    - [Navier-Cauchy equation](#navier-cauchy-equation)
      - [Uniform extension of a one-dimensional elastic body](#uniform-extension-of-a-one-dimensional-elastic-body)
    - [Elastic wave in an isotropic solid](#elastic-wave-in-an-isotropic-solid)
      - [Shear-horizontal wave](#shear-horizontal-wave)
        - [SH input impedance](#sh-input-impedance)
          - [SH impedance Riccati equation](#sh-impedance-riccati-equation)
            - [Uniform-layer SH impedance update](#uniform-layer-sh-impedance-update)
              - [Reflection from a layered SH impedance](#reflection-from-a-layered-sh-impedance)
            - [Complex-frequency SH flux monotonicity](#complex-frequency-sh-flux-monotonicity)
        - [Causal vertical wavenumber branch](#causal-vertical-wavenumber-branch)
        - [Guided shear-horizontal mode](#guided-shear-horizontal-mode)
      - [Mode conversion at a planar elastic interface](#mode-conversion-at-a-planar-elastic-interface)
        - [Solid-fluid P-wave transmission coefficient](#solid-fluid-p-wave-transmission-coefficient)
        - [Snell law for elastic and acoustic waves](#snell-law-for-elastic-and-acoustic-waves)
      - [Acoustic impedance](#acoustic-impedance)
        - [Normal acoustic impedance](#normal-acoustic-impedance)
          - [Surface acoustic impedance](#surface-acoustic-impedance)
            - [Passive acoustic impedance](#passive-acoustic-impedance)
        - [Acoustic transmission through a uniform layer](#acoustic-transmission-through-a-uniform-layer)
          - [Coherent acoustic layer above a rough reflector](#coherent-acoustic-layer-above-a-rough-reflector)
        - [Displacement reflection from an interface between two inviscid elastic liquids](#displacement-reflection-from-an-interface-between-two-inviscid-elastic-liquids)
  - [Elastic-wave energy flux](#elastic-wave-energy-flux)
    - [P-SV directional impedance matrix](#p-sv-directional-impedance-matrix)
      - [P-SV characteristic reconstruction](#p-sv-characteristic-reconstruction)
    - [Reflection of an SV-wave from a rigid plane](#reflection-of-an-sv-wave-from-a-rigid-plane)
      - [Evanescent reflected P-wave at a rigid plane](#evanescent-reflected-p-wave-at-a-rigid-plane)
        - [Unit-modulus SV reflection with evanescent P conversion](#unit-modulus-sv-reflection-with-evanescent-p-conversion)
      - [Rigid boundary condition for an elastic wave](#rigid-boundary-condition-for-an-elastic-wave)
    - [Wavevector](#wavevector)
      - [Hamiltonian ray-tracing equations](#hamiltonian-ray-tracing-equations)
        - [WKB method](#wkb-method)
          - [Eikonal equation](#eikonal-equation)
        - [Total derivative along a ray](#total-derivative-along-a-ray)
    - [Evanescent wave](#evanescent-wave)
- [Cauchy momentum equation](#cauchy-momentum-equation)
- [Falkner-Skan boundary layer](#falkner-skan-boundary-layer)
- [Sound intensity](#sound-intensity)

## Anisotropy

↑ **Parent:** [Continuum mechanics](continuum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Anisotropy)

Anisotropy is directional dependence of a material response. A [thermal conductivity tensor](thermodynamics.md#thermal-conductivity-tensor) with unequal principal conductivities is an example. Layered arrangements can produce [anisotropic](#anisotropy) [effective conductivity](#effective-conductivity) even from [isotropic](#isotropy) phases.

## Isotropy

↑ **Parent:** [Continuum mechanics](continuum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Isotropy)

Isotropy is invariance under rotations, so no spatial direction is preferred. For a three-dimensional second-rank conductivity [tensor](linear-algebra.md#tensor), invariance under every rotation forces $a=a_sI$. Isotropy of each constituent does not imply isotropy of an arranged composite microstructure. [Statistical isotropy](probability-and-statistics.md#statistical-isotropy) concerns the rotational invariance of its probability law.

## Composite material

↑ **Parent:** [Continuum mechanics](continuum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Composite_material)

A composite material contains distinct constituent phases arranged in a microstructure. Its macroscopic response depends on both phase properties and geometry, not just volume fractions. Anisotropic effective conductivity can arise even when every constituent has isotropic thermal conductivity.

### Elastic laminate

↑ **Parent:** [Composite material](#composite-material)

An [elastic laminate](#elastic-laminate) has planar perfectly bonded layers with a common normal. Its piecewise constant [strains](#strain) differ by $\operatorname{sym}(a\otimes n)$, while its normal [traction](#traction) is common to every layer. For positive [elastic stiffness tensors](#elastic-stiffness-tensor), these conditions and the mean [strain](#strain) uniquely determine the layer [strains](#strain): the difference of two solutions has zero mean and zero total elastic work, and positivity forces it to vanish.

### Effective elastic energy

↑ **Parent:** [Composite material](#composite-material)

The [effective elastic energy](#effective-elastic-energy) is the minimum averaged [strain energy density](#strain-energy-density) under prescribed affine boundary [displacement](classical-mechanics.md#displacement). For differentiable stable elastic response without [body force](fluid-mechanics.md#body-force), varying the prescribed mean [strain](#strain) gives $DW^{\mathrm{eff}}(E)=\langle\sigma\rangle$. The result follows by [integration by parts](calculus.md#integration-by-parts), because the interior variation with zero boundary data does no work against an equilibrated [stress tensor](#cauchy-stress-tensor).

#### Phase polarization comparison bound

↑ **Parent:** [Effective elastic energy](#effective-elastic-energy)

Take a positive comparison [elastic stiffness tensor](#elastic-stiffness-tensor) $C^0$, excess energies $F_r(e)=W_r(e)-e:C^0e/2$, and a phasewise constant [elastic polarization](#elastic-polarization). The [lower conjugate](convex-optimization.md#lower-conjugate) inequality majorizes the local energy by a quadratic-plus-linear function. Minimizing that function over compatible [strains](#strain) gives the displayed bound, where $A_{rs}=\int\int(\chi_r-c_r)\Gamma(\chi_s-c_s)$. Stationarity in $\tau^r$ gives $c_re^r+\sum_sA_{rs}\tau^s=c_rE$, with $e^r=DF_{r*}(\tau^r)$. Without this stationarity, dual [strains](#strain) must not be identified with the comparison solution's phase means.

#### Reuss elastic approximation

↑ **Parent:** [Effective elastic energy](#effective-elastic-energy)

The [Reuss elastic approximation](#reuss-elastic-approximation) assumes uniform [stress](#stress). The local [strain](#strain) is the derivative of the [convex conjugate](convex-optimization.md#convex-conjugate) $W^*(S,x)$; its mean is $D\langle W^*\rangle(S)$. Under invertible differentiable duality, this mean determines $S=DW_R(E)$. For positive [linear elasticity](#linear-elasticity), $C_R=\langle C^{-1}\rangle^{-1}$. Uniform [stress](#stress) is generally not accompanied by a compatible local [displacement field](#displacement-field-mechanics), so this approximation is distinguished from an exact heterogeneous solution.

#### Voigt elastic approximation

↑ **Parent:** [Effective elastic energy](#effective-elastic-energy)

The [Voigt elastic approximation](#voigt-elastic-approximation) assumes uniform [strain](#strain). Differentiating its averaged [strain energy density](#strain-energy-density) gives the averaged local [stress](#stress). For [linear elasticity](#linear-elasticity) the predicted [elastic stiffness tensor](#elastic-stiffness-tensor) is $C_V=\langle C\rangle$. The uniform [strain](#strain) is an admissible affine [displacement](classical-mechanics.md#displacement) trial field, so this gives an upper [elastic energy](#elastic-energy) bound for convex local energy.

#### Hill-Mandel energy identity

↑ **Parent:** [Effective elastic energy](#effective-elastic-energy)

For symmetric [stress](#stress) in [static elastic equilibrium](#static-elastic-equilibrium) without [body force](fluid-mechanics.md#body-force), write $E=\langle\varepsilon\rangle$ and $S=\langle\sigma\rangle$. The difference between microscopic and macroscopic work is $|\Omega|^{-1}\int_{\partial\Omega}(\sigma-S)n\cdot(u-Ex)$. It vanishes for affine boundary [displacement](classical-mechanics.md#displacement), uniform boundary [traction](#traction), or matching periodic [displacement](classical-mechanics.md#displacement) fluctuations and opposite [tractions](#traction) on paired faces.

### Volume fraction

↑ **Parent:** [Composite material](#composite-material)

The [volume fraction](#volume-fraction) of a constituent is its occupied volume divided by total sample volume. Fractions sum to one for a partition into phases. In a statistically homogeneous medium the phase fraction also equals the probability that a typical point lies in that phase, under the appropriate spatial or ensemble averaging assumptions.

### Two-point phase correlation function

↑ **Parent:** [Composite material](#composite-material)

The indicator correlation gives the probability of specified phases at two points. Statistical homogeneity makes it depend on separation; isotropy makes it depend only on its length. In particular $p_{11}(0)=p_1$, so the connected correlation at zero separation is $p_1-p_1^2=p_1p_2$.

### Effective conductivity

↑ **Parent:** [Composite material](#composite-material)

Effective conductivity describes the averaged response of a microscopic conductivity field to a macroscopic temperature or electric-potential gradient. Here the positive conductivity flux is $a\nabla u$; physical heat flux has the opposite sign. For periodic media it is computed by cell correctors, and can be a tensor even for isotropic constituents.

#### Self-consistent conductivity approximation

↑ **Parent:** [Effective conductivity](#effective-conductivity)

A [self-consistent conductivity approximation](#self-consistent-conductivity-approximation) sets the homogeneous comparison [effective conductivity](#effective-conductivity) equal to the predicted response. For a uniformly oriented two-dimensional polycrystal with principal conductivities $a,b>0$, the comparison formula gives $C_{\mathrm{SC}}^2=ab$, so its positive solution is $\sqrt{ab}$. This is an approximation defined by a fixed-point closure; exactness requires additional geometric or statistical hypotheses.

#### Hashin-Shtrikman conductivity variational principle

↑ **Parent:** [Effective conductivity](#effective-conductivity)

For a scalar reference $b$, choose a trial polarization $q$ and solve $b\Delta v+\nabla\cdot q=0$ with zero Dirichlet data. The trial functional is

$$
\mathcal F_b(q)=b|\Omega||\lambda|^2+2\lambda\cdot\int_\Omega q+\int_\Omega q\cdot\nabla v-\int_\Omega q\cdot(a-bI)^{-1}q.
$$

A reference above all phase conductivities gives $J(u)\le\mathcal F_b(q)$; one below all of them gives $J(u)\ge\mathcal F_b(q)$. If the reference equals a phase conductivity, admissible polarization vanishes in that phase and the inverse is taken only on the contrast subspace.

##### Two-dimensional isotropic polycrystal conductivity

↑ **Parent:** [Hashin-Shtrikman conductivity variational principle](#hashin-shtrikman-conductivity-variational-principle)

For uniformly distributed rotations of a two-dimensional conductivity [tensor](linear-algebra.md#tensor) with positive principal values $a\le b$, the [Hashin-Shtrikman conductivity variational principle](#hashin-shtrikman-conductivity-variational-principle) with isotropic comparison $cI$ yields $H(c)I$. Averaging a rotated diagonal [tensor](linear-algebra.md#tensor) replaces it by half its trace times the identity. Since $H'(c)=(a-b)^2/(a+b+2c)^2$, the admissible comparison endpoints give $a(a+3b)/(3a+b)\le C_{\mathrm{eff}}\le b(3a+b)/(a+3b)$ within the statistically isotropic polycrystal model.

##### Hashin-Shtrikman bounds for conductivity

↑ **Parent:** [Hashin-Shtrikman conductivity variational principle](#hashin-shtrikman-conductivity-variational-principle)

These are the optimal volume-fraction bounds for three-dimensional statistically isotropic two-phase conductivity with $0<a_1<a_2$. Constant phase polarization trial fields reduce the variational principle to a scalar quadratic optimization. The upper trial functional is minimized; the lower one is maximized.

#### Voigt bound

↑ **Parent:** [Effective conductivity](#effective-conductivity)

An affine trial temperature in the minimum-energy principle gives the upper tensor bound by the volume-averaged local conductivity. For an isotropic two-phase composite, $a^*\le p_1a_1+p_2a_2$. The same uniform-field variational idea supplies the familiar corresponding elastic upper bound.

#### Laminate conductivity

↑ **Parent:** [Effective conductivity](#effective-conductivity)

For isotropic phases with planar interfaces normal to $n$, normal conductivity is the weighted harmonic mean $a_H=(\sum p_i/a_i)^{-1}$ and tangential conductivity is the weighted arithmetic mean $a_A=\sum p_i a_i$. Continuity of normal flux and tangential temperature gradient gives the two averages directly.

#### Conductivity homogenization

↑ **Parent:** [Effective conductivity](#effective-conductivity)

Conductivity homogenization replaces rapidly varying positive coefficients in a divergence-form elliptic equation by a macroscopic effective conductivity. Periodic media admit cell problems; statistically homogeneous media can instead be described by ensemble averages. The small-scale assumptions and boundary regime must be specified.

##### Polarization field of a conductivity inclusion

↑ **Parent:** [Conductivity homogenization](#conductivity-homogenization)

Relative to a uniform reference conductivity $a_0$, this polarization is the excess positive conductivity flux. The equation becomes $a_0\Delta u+\nabla\cdot P=0$. For a prescribed mean gradient $E$, averaging gives $a^*E=a_0E+\langle P\rangle$. This sign convention differs from the physical heat-flux sign.

###### Exciting field of a conductivity inclusion

↑ **Parent:** [Polarization field of a conductivity inclusion](#polarization-field-of-a-conductivity-inclusion)

The exciting field excludes an inclusion's own singular dipole field. Other inclusions and periodic images supply the regular correction at its centre $y$. The angular mean of a self-dipole gradient on a concentric sphere vanishes, while the mean-value property recovers the regular field at the centre. Consequently a spherical average can recover the exciting field, even though the total pointwise field is not constant on that sphere.

###### Spherical conductivity inclusion

↑ **Parent:** [Polarization field of a conductivity inclusion](#polarization-field-of-a-conductivity-inclusion)

A sphere of conductivity $a_1$ in a host $a_0$ under a uniform incident gradient $E$ has interior gradient $3a_0E/(a_1+2a_0)$. Outside a sphere of radius $R$, its potential correction is $-R^3(a_1-a_0)(E\cdot x)/[(a_1+2a_0)|x|^3]$. Its polarization is $\beta E$ inside and zero outside. Temperature and normal-flux continuity determine these coefficients.

###### Dilute spherical-inclusion conductivity

↑ **Parent:** [Spherical conductivity inclusion](#spherical-conductivity-inclusion)

Well-separated shrinking spheres respond independently at leading order, so their polarization contributions add according to volume fraction. Clusters kept at fixed relative internal separation can have a different leading response; the dilute limit alone does not guarantee independent-sphere polarizability.

###### Maxwell approximation for conductivity

↑ **Parent:** [Dilute spherical-inclusion conductivity](#dilute-spherical-inclusion-conductivity)

Matching the far dipole of a spherical composite with the sum of isolated spherical-inclusion dipoles gives this approximation. Its dilute expansion is $a_0+p\beta+p^2\beta^2/(3a_0)+O(p^3)$. The rational expression is a useful closure, not the exact conductivity of every spherical-inclusion microstructure.

###### Dipole interaction correction to effective conductivity

↑ **Parent:** [Dilute spherical-inclusion conductivity](#dilute-spherical-inclusion-conductivity)

If the first exciting-field correction at inclusion $i$ is $-\beta\Lambda_iE/p_i$, its revised polarization is $\beta\chi_i(E-\beta\Lambda_iE/p_i)$. Averaging weights it by $p_i$ and gives the displayed second-reflection approximation. Further dipole reflections and finite-size multipoles are neglected.

##### Periodic conductivity cell problem

↑ **Parent:** [Conductivity homogenization](#conductivity-homogenization)

The periodic zero-mean corrector $w_j$ adjusts a unit imposed gradient so microscopic flux is divergence-free. For bounded uniformly elliptic coefficients, the weak problem has a unique solution modulo constants. The averaged flux is $a^*e_j=\langle a(e_j+\nabla w_j)\rangle$. For symmetric coefficients this also gives a symmetric positive-definite effective tensor.

###### Two-scale expansion for periodic conductivity

↑ **Parent:** [Periodic conductivity cell problem](#periodic-conductivity-cell-problem)

A periodic expansion with $y=x/\epsilon$ separates the macroscopic variable from the cell variable. Its leading cell equation forces $u_0$ to be independent of $y$, the next equation gives $u_1=w_j(y)\partial_{x_j}u_0$, and averaging the order-one flux equation yields the homogenized divergence equation. Bulk correctors generally require boundary-layer adjustments at a physical Dirichlet boundary.

###### Boundary corrector in periodic homogenization

↑ **Parent:** [Two-scale expansion for periodic conductivity](#two-scale-expansion-for-periodic-conductivity)

A bulk cell expansion generally leaves an oscillatory Dirichlet mismatch. A boundary corrector can solve the homogeneous oscillatory conductivity equation with boundary data cancelling that mismatch. It restores the prescribed physical boundary trace while leaving the leading bulk cell formula unchanged. Estimates depend on boundary regularity and on the coefficient assumptions.

## Plasticity (physics)

↑ **Parent:** [Continuum mechanics](continuum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Plasticity_(physics))

### Von Mises yield criterion

↑ **Parent:** [Plasticity (physics)](#plasticity-physics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Von_Mises_yield_criterion)

The [Von Mises yield criterion](#von-mises-yield-criterion) depends only on the second invariant of [deviatoric stress](#deviatoric-stress). With shear yield stress $k$, its surface is $\sigma':\sigma'=2k^2$; the uniaxial yield stress is $\sqrt3k$. An [associated flow rule](#associated-flow-rule) gives plastic strain rate proportional to $\sigma'$, up to a positive normalization of the plastic multiplier.

### Associated flow rule

↑ **Parent:** [Plasticity (physics)](#plasticity-physics)

Plastic strain rate is normal to the [yield surface](rheology.md#yield-surface) in the work-conjugate stress variables. With symmetric [stress](#stress) variations, the pairing is $D:\delta\sigma$; in two dimensions its off-diagonal contribution is $2D_{12}\delta\sigma_{12}$. This factor is essential when changing to reduced stress coordinates.

### Perfect plasticity

↑ **Parent:** [Plasticity (physics)](#plasticity-physics)

A perfectly plastic material has a [yield surface](rheology.md#yield-surface) that does not change with accumulated plastic deformation. This removes hardening while retaining the distinction between elastic and plastic loading.

#### Antiplane perfect plasticity

↑ **Parent:** [Perfect plasticity](#perfect-plasticity)

In [antiplane perfect plasticity](#antiplane-perfect-plasticity), [velocity](classical-mechanics.md#velocity) $w=v_3$ and shear [stresses](#stress) $a=\sigma_{13},b=\sigma_{23}$ depend only on $x_1,x_2$. [Force balance](classical-mechanics.md#force-balance) is $a_{,1}+b_{,2}=0$, the fixed [yield surface](rheology.md#yield-surface) is $f(a,b)=k$, and the [associated flow rule](#associated-flow-rule) is $\nabla w=2\dot\lambda(f_a,f_b)$ with $\dot\lambda\geq0$. Differentiating the yield equation in each coordinate and combining it with equilibrium shows that $a,b,w$ are constant along [characteristic curves](partial-differential-equation.md#characteristic-curve) tangent to $(-f_b,f_a)$. For example $-f_ba_{,1}+f_aa_{,2}=f_bb_{,2}+f_aa_{,2}=0$. Nonzero regular yield gradient is needed for a characteristic direction.

##### Centred antiplane plastic fan

↑ **Parent:** [Antiplane perfect plasticity](#antiplane-perfect-plasticity)

A centred fan consists of straight [characteristic curves](partial-differential-equation.md#characteristic-curve) emanating from one point. [Stress](#stress) and antiplane [velocity](classical-mechanics.md#velocity) are constant on each ray and depend on the polar angle $\phi$. The radial tangent condition is $(\cos\phi,\sin\phi)\parallel(-f_b,f_a)$, so $f_a\cos\phi+f_b\sin\phi=0$. A boundary ray carrying a traction-free crack-face [stress](#stress) $b=0$ has slope $\tan\phi_b=-f_a/f_b$, interpreted as vertical when $f_b=0$. For the elliptic yield condition $a^2/A^2+b^2/B^2=1$, a forward fan has $a=-A^2\sin\phi/H$, $b=B^2\cos\phi/H$, $H=(A^2\sin^2\phi+B^2\cos^2\phi)^{1/2}$. The boundary rays are vertical; the adjacent rear regions have constant [stresses](#stress) $(\mp A,0)$. [Velocity](classical-mechanics.md#velocity) is a function of angle whose magnitude requires further loading data.

#### Slip-line field theory

↑ **Parent:** [Perfect plasticity](#perfect-plasticity)

##### Hencky stress relations

↑ **Parent:** [Slip-line field theory](#slip-line-field-theory)

In [plane strain](#plane-strain) [perfect plasticity](#perfect-plasticity) with $\sigma_{11}=-p+k\sin2\phi$, $\sigma_{22}=-p-k\sin2\phi$ and $\sigma_{12}=-k\cos2\phi$, equilibrium gives

$$
\nabla p=2k\begin{pmatrix}\cos2\phi&\sin2\phi\\\sin2\phi&-\cos2\phi\end{pmatrix}\nabla\phi.
$$

The [slip line](#slip-line) tangent directions $(\cos\phi,\sin\phi)$ and $(-\sin\phi,\cos\phi)$ are eigenvectors with eigenvalues $+1,-1$. Taking directional derivatives proves the two [Hencky stress relations](#hencky-stress-relations). These sign choices must be changed consistently if the shear-stress convention changes.

###### Centred slip-line fan at a traction-free V-notch

↑ **Parent:** [Hencky stress relations](#hencky-stress-relations)

For a symmetric reentrant notch opening towards negative $x_1$, let its semi-angle be $0\leq\gamma\leq\pi/2$. On the upper free face, tensile tangential stress selects $p=-k$, $\phi=\pi/4-\gamma$. The adjacent centred fan has radial $\beta$ lines and circular $\alpha$ lines: $\phi=\vartheta-\pi/2$, $p=-k+2k[\vartheta-(3\pi/4-\gamma)]$, for $\pi/4\leq\vartheta\leq3\pi/4-\gamma$. It joins a constant stress region containing the forward axis, where $\phi=-\pi/4$ and $p=-k(1+\pi-2\gamma)$. Therefore $\sigma_{22}=k(2+\pi-2\gamma)$ in that fully plastic notch-tip region. This is a local stress field, not a claim that an arbitrary specimen is plastically yielded everywhere.

##### Geiringer velocity relations

↑ **Parent:** [Slip-line field theory](#slip-line-field-theory)

For an [associated flow rule](#associated-flow-rule) in the reduced plane-strain yield coordinates, the [rate-of-strain tensor](viscous-fluid-flow.md#strain-rate-tensor) has zero extension along both [slip line](#slip-line) directions. Write velocity as $u e_\alpha+v e_\beta$, with the local orthonormal axes turning through angle $\phi$. Differentiating along an $\alpha$ curve gives longitudinal extension $du-v\,d\phi$; along a $\beta$ curve it gives $dv+u\,d\phi$. Setting these extensions to zero proves the relations for the corresponding anisotropic [yield surface](rheology.md#yield-surface) parameterization.

##### Stress characteristics for an anisotropic yield curve

↑ **Parent:** [Slip-line field theory](#slip-line-field-theory)

Parameterize a fixed [yield surface](rheology.md#yield-surface) by stress-space [arc length](riemannian-geometry.md#arc-length) $l$ with $\xi_{,l}=-\cos2\phi$ and $\tau_{,l}=-\sin2\phi$. For mean normal stress $\sigma$, [force balance](classical-mechanics.md#force-balance) gives $\nabla\sigma=M\nabla l$, where $M=\begin{pmatrix}\cos2\phi&\sin2\phi\\\sin2\phi&-\cos2\phi\end{pmatrix}$. Its eigenvectors along angles $\phi$ and $\phi+\pi/2$ have [eigenvalues](linear-operator-theory.md#eigenvalue) $+1$ and $-1$, proving the displayed [slip line](#slip-line) invariants.

##### Slip line

↑ **Parent:** [Slip-line field theory](#slip-line-field-theory)

A slip line is a characteristic curve of a yielded plane-strain plastic equilibrium system. The two orthogonal families carry stress and velocity compatibility relations. Their directions need not agree with principal stress directions.

## Continuum thermodynamics

↑ **Parent:** [Continuum mechanics](continuum-mechanics.md)

### Reference-configuration jump balances

↑ **Parent:** [Continuum thermodynamics](#continuum-thermodynamics)

Let an interface move at signed speed $c$ in a reference unit normal direction $n$, and set $[a]=a^+-a^-$ with $n$ pointing from minus to plus. For continuous reference density and no surface sources, distributional [momentum conservation](classical-mechanics.md#momentum-conservation), [conservation of energy](physics.md#conservation-of-energy) and the [Lagrangian entropy inequality](#lagrangian-entropy-inequality) give

$$
\rho_0 c[v_i]+n_I[P_{Ii}]=0,\qquad
\rho_0 c[u+|v|^2/2]+n_I[P_{Ii}v_i-q_I^0]=0,
$$



$$
-\rho_0 c[\eta]+n_I[q_I^0/\theta]\geq0.
$$

For a level-set interface $\phi=0$, $\phi_t=-c|\nabla\phi|$, the singular part of $\partial_t a$ is $-c[a]\delta_S$ and that of $\operatorname{Div}b$ is $n\cdot[b]\delta_S$, proving these formulas. Using $V=-c$ reverses the speed terms. Density jumps require jumps of the complete conserved densities.

### Thermoelasticity

↑ **Parent:** [Continuum thermodynamics](#continuum-thermodynamics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thermoelasticity)

[Thermoelasticity](#thermoelasticity) couples [elasticity](#elasticity-physics) and [temperature](thermodynamics.md#temperature) through a specific [Helmholtz free energy](thermodynamics.md#helmholtz-free-energy) $\psi(F,\theta)$. Without constraints its reversible laws are $P_{Ii}=\rho_0\psi_{,F_{iI}}$ and $\eta=-\psi_{,\theta}$. Mixed derivatives give the same coupling tensor in the thermal stress response and the strain dependence of [specific entropy](thermodynamics.md#specific-entropy), with opposite signs.

#### Thermoelasticity with a temperature-dependent constraint

↑ **Parent:** [Thermoelasticity](#thermoelasticity)

The admissible rates obey $\phi_{,F}:\dot F=h'(\theta)\dot\theta$. A reaction multiplier $q$ in the reversible [nominal stress tensor](#nominal-stress-tensor) therefore has an accompanying [specific entropy](thermodynamics.md#specific-entropy) contribution:

$$
P_{Ii}=\rho_0\psi_{,F_{iI}}+q\phi_{,F_{iI}},\qquad\eta=-\psi_{,\theta}+\frac{q}{\rho_0}h'(\theta).
$$

Their reaction contributions cancel in the [Clausius-Duhem inequality](#clausius-duhem-inequality) on admissible rates. Omitting the entropy term would generally violate the constraint's power balance.

##### Linear thermoelasticity with prescribed thermal volume

↑ **Parent:** [Thermoelasticity with a temperature-dependent constraint](#thermoelasticity-with-a-temperature-dependent-constraint)

Linearize $\det F=h(\theta)$ at $F=I$, $\theta=\theta_0$, $h(\theta_0)=1$, and zero reaction. With displacement gradient $H$ and temperature increment $\vartheta$, one has $\operatorname{tr}H=h'(\theta_0)\vartheta$ and

$$
\sigma_{ji}=C_{jilk}H_{kl}+\beta_{ji}\vartheta+q\delta_{ji},\qquad\rho_0(\eta-\eta_0)=C_e\vartheta-\beta_{ji}H_{ij}+qh'(\theta_0),
$$

where $C_{jilk}=\rho_0\psi_{,F_{ij}F_{kl}}$, $\beta_{ji}=\rho_0\psi_{,F_{ij}\theta}$ and $C_e=-\rho_0\psi_{,\theta\theta}$ at the reference state. The temperature factor converts this entropy coefficient to a volumetric [heat capacity](thermodynamics.md#heat-capacity): $\theta_0C_e$. Strictly constant volume is the case $h'=0$.

### Clausius-Duhem inequality

↑ **Parent:** [Continuum thermodynamics](#continuum-thermodynamics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Clausius–Duhem_inequality)

#### Coleman-Noll procedure

↑ **Parent:** [Clausius-Duhem inequality](#clausius-duhem-inequality)

Requiring the [Clausius-Duhem inequality](#clausius-duhem-inequality) for independent reversible mechanical and thermal variations constrains a [constitutive equation](#constitutive-equation). For $U(F,\eta,\xi)$ it gives $P_{Ii}=\rho_0U_{,F_{iI}}$ and $\theta=U_{,\eta}$. Combining the [Lagrangian internal energy balance](#lagrangian-internal-energy-balance) with the [Lagrangian entropy inequality](#lagrangian-entropy-inequality) leaves $f_r\dot\xi_r-q_I\theta_{,I}/\theta\ge0$. The independence assumptions are part of the constitutive argument.

#### Lagrangian entropy inequality

↑ **Parent:** [Clausius-Duhem inequality](#clausius-duhem-inequality)

The local [entropy](thermodynamics.md#entropy) balance has nonnegative production, with heat supply $\rho_0r/\theta$ and [thermodynamic entropy flux](thermodynamics.md#thermodynamic-entropy-flux) $q/\theta$ at positive [temperature](thermodynamics.md#temperature) $\theta$. Its integral version holds on every material reference subvolume.

### Lagrangian internal energy balance

↑ **Parent:** [Continuum thermodynamics](#continuum-thermodynamics)

For the material-first [nominal stress tensor](#nominal-stress-tensor), the displayed local [conservation of energy](physics.md#conservation-of-energy) law balances mechanical work, heat supply and outgoing [heat flux](thermodynamics.md#heat-flux-density). Integrating over a fixed reference material volume and using the [divergence theorem](calculus.md#divergence-theorem) gives its integral form. The full total-energy balance includes [kinetic energy](classical-mechanics.md#kinetic-energy) and external mechanical work; [momentum conservation](classical-mechanics.md#momentum-conservation) reduces it to this internal-energy balance.

### Internal variable

↑ **Parent:** [Continuum thermodynamics](#continuum-thermodynamics)

An internal variable records a material state beyond its instantaneous [deformation gradient](#deformation-gradient) and [temperature](thermodynamics.md#temperature), such as a relaxing microstructural state. A [constitutive equation](#constitutive-equation) specifies its evolution and its contribution to the [free energy](thermodynamics.md#thermodynamic-free-energy).

#### Dissipation potential

↑ **Parent:** [Internal variable](#internal-variable)

A force-dependent potential specifies internal-variable rates by differentiation. Convexity with a minimum at zero force can ensure nonnegative force-rate dissipation. The name alone does not ensure the [Clausius-Duhem inequality](#clausius-duhem-inequality) for an arbitrary potential.

##### Exponential memory from tensor relaxation

↑ **Parent:** [Dissipation potential](#dissipation-potential)

The [dissipation potential](#dissipation-potential) $\Omega=\alpha\|Q\|^{n+1}/(n+1)-\operatorname{tr}(AQ)/\tau$, with the [Frobenius norm](compact-operator.md#frobenius-norm), gives $\dot A+A/\tau=\alpha\|Q\|^{n-1}Q^T$. An [integrating factor](differential-equation.md#integrating-factor) proves the displayed memory formula. For $n>0$, its nonlinear driving term is defined continuously as zero at $Q=0$. Mechanical dissipation is $\operatorname{tr}(Q\dot A)=\alpha\|Q\|^{n+1}-\operatorname{tr}(AQ)/\tau$, which must be nonnegative on thermodynamically admissible histories.

#### Thermodynamic force conjugate to an internal variable

↑ **Parent:** [Internal variable](#internal-variable)

The derivative of [internal energy](thermodynamics.md#internal-energy) at fixed [deformation gradient](#deformation-gradient) and [entropy](thermodynamics.md#entropy), or of specific [Helmholtz free energy](thermodynamics.md#helmholtz-free-energy) at fixed [temperature](thermodynamics.md#temperature), defines this force. Its product with the internal-variable rate contributes mechanical dissipation to the [Clausius-Duhem inequality](#clausius-duhem-inequality).

## Deformation (mechanics)

↑ **Parent:** [Continuum mechanics](continuum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Deformation_(mechanics))

### Finite strain theory

↑ **Parent:** [Deformation (mechanics)](#deformation-mechanics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finite_strain_theory)

#### Spectral strain measure

↑ **Parent:** [Finite strain theory](#finite-strain-theory)

For a [right stretch tensor](#right-stretch-tensor) $U=\sum_a\lambda_a n_a\otimes n_a$, define $E^f=f(U)=\sum_a f(\lambda_a)n_a\otimes n_a$. A standard normalized choice has $f\in C^1(0,\infty)$, $f(1)=0$, $f'(1)=1$ and $f$ strictly increasing; requiring $f'>0$ gives a nonsingular stretch-to-strain parameterization. This [strain](#strain) vanishes exactly for a rigid rotation, is independent of superposed spatial rotations, and agrees to first order with the infinitesimal symmetric displacement gradient. Indeed $F=I+H$ gives $U=I+(H+H^T)/2+O(\|H\|^2)$, and Taylor expansion of $f$ proves the last statement.

##### Biot strain tensor

↑ **Parent:** [Spectral strain measure](#spectral-strain-measure)

The [Biot strain tensor](#biot-strain-tensor) uses $f(\lambda)=\lambda-1$, so $E^{(1)}=U-I$. Its principal values are extension ratios minus one. It is a [spectral strain measure](#spectral-strain-measure), since $f(1)=0$, $f'(1)=1$ and $f'>0$. Its reference-volume work conjugate is the [symmetric Biot stress](#symmetric-biot-stress).

#### Inverse right Cauchy-Green strain

↑ **Parent:** [Finite strain theory](#finite-strain-theory)

For $C=F^TF$, differentiation of $C^{-1}$ gives $\dot E^{(-2)}=F^{-1}DF^{-T}$. Its reference-power conjugate is $T^{(-2)}=F^T\tau F$. In a convected coordinate basis $g_I=Fe_I$, these are the covariant components of the [Kirchhoff stress tensor](#kirchhoff-stress-tensor). The [second Piola-Kirchhoff stress tensor](#second-piola-kirchhoff-stress-tensor) instead gives its contravariant components, since $\tau=T^{(2)}_{IJ}g_I\otimes g_J$.

#### Green-Lagrange strain tensor

↑ **Parent:** [Finite strain theory](#finite-strain-theory)

With the [right Cauchy-Green deformation tensor](#right-cauchy-green-deformation-tensor) $C=F^TF$, the [Green-Lagrange strain tensor](#green-lagrange-strain-tensor) measures the change in the material metric. Since $\dot E^{(2)}=F^TDF$, its [work-conjugate stress and strain](#work-conjugate-stress-and-strain) partner is the [second Piola-Kirchhoff stress tensor](#second-piola-kirchhoff-stress-tensor) $F^{-1}\tau F^{-T}$. The formula follows by cycling factors in $T:\dot E^{(2)}$, not by identifying nominal and symmetric material stress.

#### Plane strain

↑ **Parent:** [Finite strain theory](#finite-strain-theory)

In plane strain, the [deformation map](#deformation-map) has $x_1=x_1(X_1,X_2)$, $x_2=x_2(X_1,X_2)$ and $x_3=X_3$. The out-of-plane stretch is one and out-of-plane shear vanishes. This kinematic condition need not make the out-of-plane [stress](#stress) vanish.

#### Simple shear

↑ **Parent:** [Finite strain theory](#finite-strain-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simple_shear)

Simple shear displaces one coordinate direction in proportion to a transverse coordinate while preserving volume. Its [deformation gradient](#deformation-gradient) has a single off-diagonal component $\gamma$. [Simple shear flow](viscous-fluid-flow.md#simple-shear-flow) describes the corresponding velocity field rather than the finite deformation.

#### Stretch tensor

↑ **Parent:** [Finite strain theory](#finite-strain-theory)

##### Principal stretch

↑ **Parent:** [Stretch tensor](#stretch-tensor)

The principal stretches are the [eigenvalues](linear-operator-theory.md#eigenvalue) of a [stretch tensor](#stretch-tensor), or equivalently the [singular values](linear-algebra.md#singular-value) of the [deformation gradient](#deformation-gradient). They measure local length ratios along the principal reference directions.

##### Right stretch tensor

↑ **Parent:** [Stretch tensor](#stretch-tensor)

##### Left stretch tensor

↑ **Parent:** [Stretch tensor](#stretch-tensor)

#### Deformation gradient

↑ **Parent:** [Finite strain theory](#finite-strain-theory)

The [Jacobian matrix](calculus.md#jacobian-matrix) of a [deformation map](#deformation-map) carries an infinitesimal reference line element to its current image. Its [determinant](linear-algebra.md#determinant) $J=\det F$ is the local volume ratio. An orientation-preserving deformation has $J>0$, and [incompressibility](fluid-mechanics.md#incompressible-flow) imposes $J=1$.

<h5 id="nanson-s-formula">Nanson's formula</h5>

↑ **Parent:** [Deformation gradient](#deformation-gradient)

For an orientation-preserving [deformation gradient](#deformation-gradient) $F$, oriented area transforms by its cofactor matrix: $(Fa)\times(Fb)=(\det F)F^{-T}(a\times b)$. Taking the [dot product](linear-algebra.md#dot-product) with $Fc$ proves this from the determinant identity for the scalar triple product. Applying it to tangent vectors of a surface proves [Nanson's formula](#nanson-s-formula). Equating current and reference [tractions](#traction) then gives the material-first [nominal stress tensor](#nominal-stress-tensor) $P=JF^{-1}\sigma$ for symmetric [Cauchy stress tensor](#cauchy-stress-tensor) $\sigma$.

##### Multiplicative decomposition of the deformation gradient

↑ **Parent:** [Deformation gradient](#deformation-gradient)

The factor $A$ can encode an internal relaxed configuration, while $F_*=FA^{-1}$ determines the instantaneous elastic energy. Differentiating $F_*$ at fixed $F$ or fixed $A$ produces the corresponding [nominal stress tensor](#nominal-stress-tensor) and [thermodynamic force conjugate to an internal variable](#thermodynamic-force-conjugate-to-an-internal-variable). This is a kinematic decomposition, not an assertion that each factor separately derives from a global [deformation map](#deformation-map).

##### Polar decomposition in continuum mechanics

↑ **Parent:** [Deformation gradient](#deformation-gradient)

For an orientation-preserving invertible [deformation gradient](#deformation-gradient), the [polar decomposition of an invertible real matrix](linear-algebra.md#polar-decomposition-of-an-invertible-real-matrix) separates a rotation $R$ from the [right stretch tensor](#right-stretch-tensor) $U$ or the [left stretch tensor](#left-stretch-tensor) $V$. The rotation is shared by the two factorizations, with $V=RUR^T$.

##### Right Cauchy-Green deformation tensor

↑ **Parent:** [Deformation gradient](#deformation-gradient)

The right Cauchy-Green tensor measures stretch on the [reference configuration](#reference-configuration). Its [eigenvalues](linear-operator-theory.md#eigenvalue) are the same squared [principal stretches](#principal-stretch) as those of the [left Cauchy-Green deformation tensor](#left-cauchy-green-deformation-tensor), but its [eigenvectors](linear-operator-theory.md#eigenvector) are reference directions.

##### Left Cauchy-Green deformation tensor

↑ **Parent:** [Deformation gradient](#deformation-gradient)

The left Cauchy-Green tensor measures stretch on the [current configuration](#current-configuration). It is a [positive-definite symmetric matrix](linear-algebra.md#symmetric-positive-definite-matrix) for an invertible [deformation gradient](#deformation-gradient), with [eigenvalues](linear-operator-theory.md#eigenvalue) equal to the squares of the [principal stretches](#principal-stretch).

### Deformation map

↑ **Parent:** [Deformation (mechanics)](#deformation-mechanics)

A deformation map sends each particle's [reference configuration](#reference-configuration) position to its [current configuration](#current-configuration) position. Its spatial derivative with respect to the [Lagrangian coordinates](#lagrangian-coordinate) is the [deformation gradient](#deformation-gradient).

#### Current configuration

↑ **Parent:** [Deformation map](#deformation-map)

#### Reference configuration

↑ **Parent:** [Deformation map](#deformation-map)

## Constitutive equation

↑ **Parent:** [Continuum mechanics](continuum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Constitutive_equation)

A constitutive equation relates continuum fields such as [stress](#stress), [strain](#strain), and the [rate-of-strain tensor](viscous-fluid-flow.md#strain-rate-tensor) to characterize a material beyond universal balance laws.

### Material frame indifference

↑ **Parent:** [Constitutive equation](#constitutive-equation)

A [constitutive equation](#constitutive-equation) is frame indifferent when a superposed rigid spatial rotation changes its outputs by their tensor transformation rules. For an elastic [Cauchy stress tensor](#cauchy-stress-tensor), this requires $\sigma(QF)=Q\sigma(F)Q^T$. It differs from [material isotropy](#material-isotropy), which rotates reference material directions.

#### Objective second-rank tensor

↑ **Parent:** [Material frame indifference](#material-frame-indifference)

An objective spatial second-rank [tensor](linear-algebra.md#tensor) transforms by the displayed rule under every rigid observer change $x^*=c(t)+Q(t)x$. This permits time-dependent rotations, not merely constant rotations. [Cauchy stress tensor](#cauchy-stress-tensor) is objective because contact traction and surface normal both rotate by Q. The symmetric [rate-of-strain tensor](viscous-fluid-flow.md#strain-rate-tensor) is objective because the additional observer spin in the [velocity gradient](#velocity-gradient) is antisymmetric.

### Stress

↑ **Parent:** [Constitutive equation](#constitutive-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stress)

Stress is force transmitted per unit area inside a continuum. The Cauchy stress tensor maps a surface normal to the traction acting across that surface.

#### Work-conjugate stress and strain

↑ **Parent:** [Stress](#stress)

A [stress](#stress) measure $T$ is work-conjugate to a [strain](#strain) measure $E$ when their contraction gives the mechanical power per specified volume for every admissible deformation rate. The reference-volume power is $P_{Ii}\dot F_{iI}=\tau:D$, with [Kirchhoff stress tensor](#kirchhoff-stress-tensor) $\tau$ and [rate-of-strain tensor](viscous-fluid-flow.md#strain-rate-tensor) $D$. A strain constraint can leave the conjugate stress undetermined by a reaction component that does no admissible work; uniqueness should therefore not be assumed on a restricted set of rates.

##### Symmetric Biot stress

↑ **Parent:** [Work-conjugate stress and strain](#work-conjugate-stress-and-strain)

Use the material-first [nominal stress](#nominal-stress-tensor) $P_{Ii}$ and $F=RU$. The [symmetric Biot stress](#symmetric-biot-stress) conjugate to the [Biot strain tensor](#biot-strain-tensor) is $T^{(1)}=\operatorname{sym}(PR)$. To prove it, set $M=P^T$ and differentiate $F=RU$. Conservation of [angular momentum](classical-mechanics.md#angular-momentum) makes $MF^T$ symmetric, so the contraction of $R^TM$ with $R^T\dot R\,U$ is zero: it is a contraction of a symmetric [tensor](linear-algebra.md#tensor) with a skew [tensor](linear-algebra.md#tensor) after cyclically moving $U$. Thus $M:\dot F=\operatorname{sym}(R^TM):\dot U=T^{(1)}:\dot E^{(1)}$. No assumption that $PR$ itself is symmetric is needed.

#### Mandel stress tensor

↑ **Parent:** [Stress](#stress)

With the [right Cauchy-Green deformation tensor](#right-cauchy-green-deformation-tensor) $C=F^TF$ and the [second Piola-Kirchhoff stress tensor](#second-piola-kirchhoff-stress-tensor) $S$, this mixed material stress is generally nonsymmetric. In the material-first [nominal stress tensor](#nominal-stress-tensor) convention, $PF=SC=M^T$. Thus replacing $PF^{-T}$ by $PF$ changes the stress measure. The relation follows from $\mathcal P=FS$, without any assumption of [material isotropy](#material-isotropy).

#### Kirchhoff stress tensor

↑ **Parent:** [Stress](#stress)

The Kirchhoff tensor is the [Cauchy stress tensor](#cauchy-stress-tensor) multiplied by the local volume ratio. Its [stress](#stress) power is per reference volume. Pushing forward the [second Piola-Kirchhoff stress tensor](#second-piola-kirchhoff-stress-tensor) gives the displayed formula.

#### Piola-Kirchhoff stress tensors

↑ **Parent:** [Stress](#stress)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Piola–Kirchhoff_stress_tensors)

These [stress](#stress) measures refer force or area to the [reference configuration](#reference-configuration). Different index-order conventions distinguish a [first Piola-Kirchhoff stress tensor](#first-piola-kirchhoff-stress-tensor) from its transposed [nominal stress tensor](#nominal-stress-tensor). The [second Piola-Kirchhoff stress tensor](#second-piola-kirchhoff-stress-tensor) has two material indices.

##### Second Piola-Kirchhoff stress tensor

↑ **Parent:** [Piola-Kirchhoff stress tensors](#piola-kirchhoff-stress-tensors)

The second tensor has two material indices and is symmetric when the [Cauchy stress tensor](#cauchy-stress-tensor) is symmetric. The displayed relation uses the material-first [nominal stress tensor](#nominal-stress-tensor) convention. In particular, $PF$ is generally not this tensor. These conventions agree with [A. F. Bower's definitions of stress measures](https://solidmechanics.org/Text/Chapter2_3/Chapter2_3.htm).

##### First Piola-Kirchhoff stress tensor

↑ **Parent:** [Piola-Kirchhoff stress tensors](#piola-kirchhoff-stress-tensors)

###### Nominal stress tensor

↑ **Parent:** [First Piola-Kirchhoff stress tensor](#first-piola-kirchhoff-stress-tensor)

Here the convention places the material index first: $P_{Ii}$. Its [stress](#stress) power per reference volume is $P_{Ii}\dot F_{iI}$. It is the transpose of the [first Piola-Kirchhoff stress tensor](#first-piola-kirchhoff-stress-tensor); some texts instead call that first tensor itself nominal stress.

#### Cauchy stress tensor

↑ **Parent:** [Stress](#stress)

The stress tensor maps a surface normal to the [traction](#traction) exerted across that surface. Its divergence is the force density in local momentum balance. For an incompressible Newtonian fluid it combines pressure with twice the viscosity times the symmetric strain-rate tensor.

##### Normal stress

↑ **Parent:** [Cauchy stress tensor](#cauchy-stress-tensor)

The component of traction normal to a surface with unit normal $n$. For an incompressible [Newtonian fluid](viscous-fluid-flow.md#newtonian-fluid), $\sigma=-pI+2\mu e$, so $\sigma_{nn}=-p+2\mu n\cdot e n$. A free-interface normal-stress jump includes the curvature force from [surface tension](fluid-mechanics.md#surface-tension).

##### Principal stress

↑ **Parent:** [Cauchy stress tensor](#cauchy-stress-tensor)

The principal stresses are the [eigenvalues](linear-operator-theory.md#eigenvalue) of the symmetric [Cauchy stress tensor](#cauchy-stress-tensor). In their [orthonormal eigenbasis](linear-operator-theory.md#orthonormal-eigenbasis), each [traction](#traction) is normal to its corresponding principal plane.

#### Deviatoric stress

↑ **Parent:** [Stress](#stress)

The deviatoric part of a three-dimensional [stress](#stress) [tensor](linear-algebra.md#tensor) is $\boldsymbol\sigma_{\rm dev}=\boldsymbol\sigma-\operatorname{tr}(\boldsymbol\sigma)\mathbf I/3$. It is traceless. Adding an isotropic pressure does not change a [normal-stress difference](rheology.md#normal-stress-difference).

#### Traction

↑ **Parent:** [Stress](#stress)

Traction is the [force](classical-mechanics.md#force) per unit area transmitted across an oriented surface. For unit [normal vector](differential-geometry.md#normal-vector) $\mathbf n$, the [stress](#stress) [tensor](linear-algebra.md#tensor) gives $\mathbf t=\boldsymbol\sigma\mathbf n$. Its normal component is normal stress, and its tangential component is [shear stress](viscous-fluid-flow.md#shear-stress).

##### Hydrodynamic torque

↑ **Parent:** [Traction](#traction)

The hydrodynamic torque on a body about a reference point is $T=\int_S r\times(\sigma\cdot n)dS$, with $r$ measured from that point and $n$ pointing from the body into the fluid. The [stress](#stress) includes pressure and viscous contributions, and $\sigma\cdot n$ is the fluid [traction](#traction) on the body. Changing the reference point by $d$ changes the [torque](classical-mechanics.md#torque) by $-d\times F$, where $F=\int_S\sigma\cdot n dS$ is the fluid force. A [torque-free](stokes-flow.md#torque-free) body has zero resultant torque, including any external torque.

### Strain

↑ **Parent:** [Constitutive equation](#constitutive-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Strain)

Strain measures local deformation relative to a reference configuration. In small-deformation theory it is the symmetric part of the displacement gradient.

#### Infinitesimal strain tensor

↑ **Parent:** [Strain](#strain)

The [infinitesimal strain tensor](#infinitesimal-strain-tensor) is the symmetric part of a [displacement gradient tensor](#displacement-gradient-tensor). It is the linear approximation to a finite [strain](#strain) measure for small displacement gradients. An infinitesimal rigid rotation contributes no [strain](#strain), so the [elastic energy](#elastic-energy) depends on the symmetric part rather than the entire gradient.

## Velocity gradient

↑ **Parent:** [Continuum mechanics](continuum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Velocity_gradient)

The velocity gradient has components $(\nabla\mathbf u)_{ij}=\partial_j u_i$. Its symmetric part is the deformation-rate tensor and its antisymmetric part is the local spin.

### Velocity divergence

↑ **Parent:** [Velocity gradient](#velocity-gradient)

The velocity divergence is the trace of the [velocity gradient](#velocity-gradient). It is the local fractional rate of volume expansion of a moving material element.

## Mass conservation

↑ **Parent:** [Continuum mechanics](continuum-mechanics.md)

Mass conservation states that matter is neither created nor destroyed. For mass density $\rho$ and velocity $\mathbf v$, its local form is $\partial_t\rho+\nabla\mathbin\cdot(\rho\mathbf v)=0$.

## Material derivative

↑ **Parent:** [Continuum mechanics](continuum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Material_derivative)

The material derivative follows a moving continuum parcel:

$$
\frac D{Dt}=\frac{\partial}{\partial t}+\mathbf u\cdot\nabla.
$$

### Reynolds transport theorem

↑ **Parent:** [Material derivative](#material-derivative)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reynolds_transport_theorem)

For a smoothly moving volume whose boundary has normal velocity $v_b\cdot n$, the derivative of an integral equals the local time-change integral plus the boundary-transport flux. The boundary term comes from the thin layer swept by the moving surface during a short time interval. Taking $f=1$ gives $d|V|/dt=\int v_b\cdot n\,dS$. If the boundary moves with the fluid, this combines with the [divergence theorem](calculus.md#divergence-theorem) to give the integral of the [material derivative](#material-derivative) plus $f$ times the velocity divergence.

### Convective acceleration

↑ **Parent:** [Material derivative](#material-derivative)

Convective acceleration is the spatial part $(\mathbf u\cdot\nabla)\mathbf u$ of the [material derivative](#material-derivative) of fluid velocity. It can remain nonzero in [steady flow](fluid-mechanics.md#steady-flow), because a moving particle passes through positions with different velocities. The identity $(\mathbf u\cdot\nabla)\mathbf u=\nabla(|\mathbf u|^2/2)-\mathbf u\times(\nabla\times\mathbf u)$ relates it to [vorticity](fluid-mechanics.md#vorticity).

### Material acceleration

↑ **Parent:** [Material derivative](#material-derivative)

The material acceleration is the rate of change of velocity following a continuum parcel:

$$
\frac{D\mathbf u}{Dt}
=\frac{\partial\mathbf u}{\partial t}
+(\mathbf u\mathbin\cdot\nabla)\mathbf u.
$$

### Eulerian coordinate

↑ **Parent:** [Material derivative](#material-derivative)

An Eulerian coordinate labels a fixed position in space at which continuum fields are observed.

### Lagrangian coordinate

↑ **Parent:** [Material derivative](#material-derivative)

A Lagrangian coordinate labels a material particle and remains attached to it as the continuum moves.

### Eulerian time average

↑ **Parent:** [Material derivative](#material-derivative)

An Eulerian time average holds spatial position fixed while averaging a time-dependent field:

$$
\langle u\rangle(x)=\frac1T\int_0^Tu(x,t)\,dt.
$$

### Lagrangian trajectory

↑ **Parent:** [Material derivative](#material-derivative)

A Lagrangian trajectory follows one marked fluid particle and solves

$$
\dot X(t)=u(X(t),t).
$$

#### Fluid element

↑ **Parent:** [Lagrangian trajectory](#lagrangian-trajectory)

A fluid element is an infinitesimal material parcel followed along a [Lagrangian trajectory](#lagrangian-trajectory).

#### Stokes drift

↑ **Parent:** [Lagrangian trajectory](#lagrangian-trajectory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stokes_drift)

Stokes drift is the difference between the mean velocity of fluid particles and the Eulerian mean velocity at fixed positions. It appears at second order because particles sample the oscillatory velocity at displaced positions.

##### Cross-wave Stokes drift

↑ **Parent:** [Stokes drift](#stokes-drift)

Two [plane internal gravity waves](gravity-wave.md#plane-internal-gravity-wave) can each have zero [Stokes drift](#stokes-drift) but give a nonzero drift through interference. The displacement of one wave need not be perpendicular to the other wave's [wave vector](#wavevector). For upward waves with wave vectors $(\kappa,-\kappa)$ and $(-\kappa,-\kappa)$ and vertical amplitudes $W$, the cross-wave drift is $(0,-2\kappa W^2\cos(2\kappa x)/\omega)$ with $\omega=N/\sqrt2$. It has zero spatially averaged vertical flux. It cannot on its own satisfy an impermeable oscillating boundary: the second-order [Eulerian mean velocity](geophysical-fluid-dynamics.md#eulerian-mean-flow) supplies the necessary normal correction there.

##### Initial and mean parcel labels in a surface wave

↑ **Parent:** [Stokes drift](#stokes-drift)

A [fluid displacement](fluid-mechanics.md#lagrangian-displacement-fluid-mechanics) measured from an initial position must vanish at the initial time. Integrating a harmonic [velocity](classical-mechanics.md#velocity) therefore introduces phase-dependent constants. Mean-orbit labels absorb those constants and leave purely oscillatory displacements. The instantaneous displacement correction to velocity can differ under the two reference conventions, but its period mean gives the same leading [Stokes drift](#stokes-drift).

## Rayleigh-Taylor instability

↑ **Parent:** [Continuum mechanics](continuum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rayleigh-Taylor_instability)

The Rayleigh-Taylor instability occurs when a denser fluid lies above a lighter fluid in a gravitational field, causing interface perturbations to grow.

### Orthogonal-field magnetic Rayleigh-Taylor dispersion relation

↑ **Parent:** [Rayleigh-Taylor instability](#rayleigh-taylor-instability)

Consider uniform fields $B_-\hat{\mathbf y}$ below and $B_+\hat{\mathbf x}$ above an interface, with local constant densities $\rho_-,\rho_+$. For ideal [magnetohydrodynamics](astrophysical-fluid-dynamics.md#magnetohydrodynamics) and local incompressible [potential flow](fluid-mechanics.md#potential-flow), the interface displacement $h e^{st+ikx+imy}$ has displacement potentials $\chi_-=h e^{Kz}/K$ and $\chi_+=-h e^{-Kz}/K$, $K=\sqrt{k^2+m^2}$. [Magnetic flux freezing](astrophysical-fluid-dynamics.md#magnetic-flux-freezing) gives $\mathbf b_i=(\mathbf B_i\cdot\nabla)\nabla\chi_i$. The linear [magnetohydrodynamic total pressure](astrophysical-fluid-dynamics.md#magnetohydrodynamic-total-pressure) is $-[\rho_i s^2+(\mathbf k_h\cdot\mathbf B_i)^2/\mu_0]\chi_i$. Matching Lagrangian total pressure gives the displayed [dispersion relation](wave-equation.md#dispersion-relation). For $\rho_+>\rho_-$ the most unstable orientation has its wavevector along the weaker field.

// Target: continuum-mechanics.bigb

#### Localization condition for the fastest orthogonal-field interface mode

↑ **Parent:** [Orthogonal-field magnetic Rayleigh-Taylor dispersion relation](#orthogonal-field-magnetic-rayleigh-taylor-dispersion-relation)

For the density jump of a [magnetic pressure discontinuity in an isothermal atmosphere](astrophysical-fluid-dynamics.md#magnetic-pressure-discontinuity-in-an-isothermal-atmosphere), with $0<|B_+|<|B_-|$, the fastest [Rayleigh-Taylor instability](#rayleigh-taylor-instability) has $m=0$ and $|k|=K_*=(B_-^2-B_+^2)/(4B_+^2H)$. Its vertical decay length is $K_*^{-1}$. Hence localization relative to both common [scale heights](statistical-physics.md#scale-height) requires $4B_+^2\ll B_-^2-B_+^2$. This also makes its growth speed small compared with the isothermal sound speed. If $B_+=0$, the ideal sharp-interface [dispersion relation](wave-equation.md#dispersion-relation) instead has unbounded growth as $|k|\to\infty$: there is no finite maximizing mode.

### Viscous overturn of a dense crust

↑ **Parent:** [Rayleigh-Taylor instability](#rayleigh-taylor-instability)

A dense viscous crust of thickness $a$ above lighter liquid can overturn on a [Rayleigh-Taylor instability](#rayleigh-taylor-instability) time $\mu_s/(\Delta\rho ga)$. If diffusive growth gives $a=A\sqrt{\kappa t}$, matching its age to that time gives $\tau_s\sim[\mu_s/(\Delta\rho gA\sqrt\kappa)]^{2/3}$. A renewed crust then supplies average solid-volume flux $J_s\sim(\Delta\rho g/\mu_s)^{1/3}(A^2\kappa)^{2/3}$. This scale assumes that heat supplied by the interior does not arrest the crust before instability.

### Finite-depth Rayleigh-Taylor dispersion relation

↑ **Parent:** [Rayleigh-Taylor instability](#rayleigh-taylor-instability)

For two resting incompressible inviscid layers between impermeable horizontal walls, the upper layer has density $\rho_1$ and depth $L_1$, and the lower layer has $\rho_2<\rho_1$ and depth $L_2$. Solving the [Laplace equation](partial-differential-equation.md#laplace-equation) for the [velocity potential](fluid-mechanics.md#velocity-potential) and imposing the linearized kinematic and capillary pressure conditions gives the displayed [dispersion relation](wave-equation.md#dispersion-relation). With positive [surface tension](fluid-mechanics.md#surface-tension) $\gamma$, exponential [Rayleigh-Taylor instability](#rayleigh-taylor-instability) occurs for $0<k<k_c$, where $k_c=\sqrt{g(\rho_1-\rho_2)/\gamma}$. The depths change the growth rate, but not this cutoff.

#### Thin-layer Rayleigh-Taylor growth asymptotics

↑ **Parent:** [Finite-depth Rayleigh-Taylor dispersion relation](#finite-depth-rayleigh-taylor-dispersion-relation)

For an infinitely deep lower layer and $k_cL_1\ll1$, write $A=g(\rho_1-\rho_2)$. Uniformly over the unstable band, the [finite-depth Rayleigh-Taylor dispersion relation](#finite-depth-rayleigh-taylor-dispersion-relation) gives $\sigma^2\sim(L_1/\rho_1)(Ak^2-\gamma k^4)$. Its maximum occurs at $k_m\sim k_c/\sqrt2$, with the displayed growth rate. In two deep layers the maximum instead occurs at $k_c/\sqrt3$ and obeys $\sigma_m^2=2Ak_c/[3\sqrt3(\rho_1+\rho_2)]$. Thus confinement strongly reduces growth while leaving the cutoff unchanged. These thin-layer expressions are leading asymptotics, not exact finite-depth identities.

## Boundary layer

↑ **Parent:** [Continuum mechanics](continuum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boundary_layer)

A boundary layer is a thin region next to a surface in which viscosity remains significant even when inertia dominates the outer flow.

### Laminar plane jet from a line force

↑ **Parent:** [Boundary layer](#boundary-layer)

A steady two-dimensional laminar jet driven by force $F$ per span has conserved momentum flux $\rho\int u^2dy=F$. The boundary-layer pressure gradient is zero. Balancing inertia and viscosity with this flux gives width proportional to $x^{2/3}$ and centre velocity proportional to $x^{-1/3}$. The streamfunction $(F\nu x/\rho)^{1/3}f(\eta)$, $\eta=y[F/(\rho\nu^2x^2)]^{1/3}$, obeys $3f'''+(f')^2+ff''=0$. The displayed profile has $\int(f')^2d\eta=2A^3/9$, so momentum equality fixes $A$. Merely requiring independence of $x$ does not fix the amplitude. Entrainment makes volume flux $2A(F\nu x/\rho)^{1/3}$ grow downstream.

### Laminar skin-friction scaling along a slender swimmer

↑ **Parent:** [Boundary layer](#boundary-layer)

A steady attached laminar [boundary layer](#boundary-layer) with slip speed $u_t$ and downstream distance $s$ has thickness $\delta\sim\sqrt{\nu s/u_t}$. The wall shear is $\tau_w\sim\mu u_t/\delta$, giving the displayed scaling, where $\mu=\rho\nu$ is [dynamic viscosity](fluid-mechanics.md#dynamic-viscosity). Multiplying by a nearly constant wetted perimeter gives local drag per unit length proportional to $u_t^{3/2}s^{-1/2}$, and integration gives drag proportional to $u_t^{3/2}\sqrt L$. A force density weighted by $s^{1/2}$ instead produces $L^{3/2}$; it can be a separately prescribed phenomenological model but is not this local laminar shear law. Strong curvature, unsteadiness, separation or turbulent transition can invalidate the estimate.

### Conical sink boundary layer

↑ **Parent:** [Boundary layer](#boundary-layer)

An axisymmetric sink inside a cone has outer speed $U=-A/x^2$. With local distance $x$ along the wall and normal distance $y$, leading continuity is $u_x+u/x+v_y=0$ because the circumference is proportional to $x$. Balancing convection with normal viscous diffusion gives the displayed thickness. With streamfunction $\Psi=-\sqrt{A\nu}x^{1/2}F(y/\delta)$, $xu=\Psi_y$ and $xv=-\Psi_x$, the similarity equation is $F'''-FF''/2+2(1-F'^2)=0$, with $F(0)=F'(0)=0$ and $F'(\infty)=1$. The displacement-flux correction scales as $\sqrt{A\nu}\,R^{1/2}$, and the corresponding outer velocity correction as $\sqrt{A\nu}\,R^{-3/2}$.

### Similarity profile of an axisymmetric radial viscous free jet

↑ **Parent:** [Boundary layer](#boundary-layer)

In a symmetric thin radial free jet, $F=\int r u_r^2\,dz$ is conserved by the conservative momentum equation. Balancing advection and viscosity gives thickness $\delta=Cr$, with $C=(\nu^2/F)^{1/3}$. The normalized similarity streamfunction uses $A=(F^2/\nu)^{1/3}$ and $f=2k\tanh(k\eta)$, $k=(3/16)^{1/3}$, so $\int f'^2d\eta=1$. The displayed velocity follows, and the thin-layer requirement is $F\gg\nu^2$.

### Plane laminar jet

↑ **Parent:** [Boundary layer](#boundary-layer)

#### Bickley jet

↑ **Parent:** [Plane laminar jet](#plane-laminar-jet)

A steady planar viscous jet whose conserved momentum flux and convection-diffusion balance give the displayed scaling. Choosing $U\delta^2=\nu x$ and $U$ as centre-line speed gives streamfunction profile $f''' +(ff''+(f')^2)/3=0$, with $f(0)=f''(0)=0$, $f'(0)=1$ and $f'(\pm\infty)=0$. Integration yields $f=\sqrt6\tanh(\eta/\sqrt6)$ and velocity profile $f'=\operatorname{sech}^2(\eta/\sqrt6)$. Its momentum integral is $4\sqrt6/3$, fixing the dimensional prefactors. Transverse entrainment does not require $f(\infty)=0$.

### Boundary-layer equation

↑ **Parent:** [Boundary layer](#boundary-layer)

The leading momentum and mass equations in a thin laminar shear region with flow predominantly along a surface or jet axis. Longitudinal viscous derivatives are smaller than transverse ones, and pressure is supplied by the outer flow. The transverse velocity remains necessary for mass conservation and entrainment even when it is small compared with the axial velocity.

### Turbulent boundary layer

↑ **Parent:** [Boundary layer](#boundary-layer)

A [boundary layer](#boundary-layer) in which turbulent velocity fluctuations transport momentum and scalars. A near-wall constant-stress region supports the [law of the wall](#law-of-the-wall); buoyancy modifies it through [Monin-Obukhov similarity theory](#monin-obukhov-similarity-theory). A viscous or roughness sublayer and an outer-layer scale bound the range of either approximation.

#### Viscous sublayer

↑ **Parent:** [Turbulent boundary layer](#turbulent-boundary-layer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Viscous_sublayer)

The near-wall region where molecular momentum diffusion dominates turbulent transport. Using the [shear velocity](viscous-fluid-flow.md#shear-velocity) $u_*=\sqrt{\tau_d/\rho}$ gives the viscous wall length $\nu/u_*$. The precise extent depends on the chosen crossover criterion and wall condition. In this region constant stress and no slip give $U\simeq u_*^2z/\nu$; the logarithmic [law of the wall](#law-of-the-wall) applies outside it.

#### Monin-Obukhov similarity theory

↑ **Parent:** [Turbulent boundary layer](#turbulent-boundary-layer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Monin–Obukhov_similarity_theory)

A local similarity description for approximately stationary homogeneous surface-layer turbulence with nearly constant momentum and buoyancy fluxes. Besides height and [friction velocity](viscous-fluid-flow.md#shear-velocity), the [Obukhov length](#monin-obukhov-length) enters as a stability parameter. The hypothesis fixes the dimensional shear prefactor and function argument, while empirical or dynamical closures determine the functions themselves.

##### Near-neutral log-linear surface-layer profiles

↑ **Parent:** [Monin-Obukhov similarity theory](#monin-obukhov-similarity-theory)

If the similarity functions of a [turbulent boundary layer](#turbulent-boundary-layer) are differentiable at zero and have finite positive neutral values, expanding $f=a+d z/\ell+O((z/\ell)^2)$ gives a shear proportional to $1/z-d/(a\ell)$. Integration yields a logarithmic term plus a linear correction. Dimensional reasoning alone does not fix the coefficients or guarantee this regular neutral limit. The [gradient Richardson number](gravity-wave.md#gradient-richardson-number) is of order $z/\ell$, so $|z/\ell|\ll1$ is a shear-dominated, nearly neutral regime on either side of stability.

##### Very stable surface-layer similarity

↑ **Parent:** [Monin-Obukhov similarity theory](#monin-obukhov-similarity-theory)

In local continuously turbulent scaling at $z/\ell_O\gg1$, dependence on the distance to the wall disappears at leading order. The velocity profile is linear and the buoyancy frequency is constant. Local energy balance gives $\epsilon=(c_m-1)|B_0|$ and $\mathrm{Ri}_f=1/c_m$, with positive dissipation requiring $c_m>1$. The coefficients depend on a closure, and this regime should not be imposed on fully collapsed turbulence.

##### Monin-Obukhov length

↑ **Parent:** [Monin-Obukhov similarity theory](#monin-obukhov-similarity-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Monin–Obukhov_length)

The signed wall-turbulence length formed from stress velocity and the [vertical turbulent buoyancy flux](turbulence.md#vertical-turbulent-buoyancy-flux). With upward buoyancy transport positive, stable cooling has $B_0<0$ and $\ell_O>0$; heating from below gives $\ell_O<0$. The magnitude marks the transition between shear-dominated and buoyancy-dominated scaling.

#### Law of the wall

↑ **Parent:** [Turbulent boundary layer](#turbulent-boundary-layer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Law_of_the_wall)

In a neutral turbulent constant-stress region, the stress velocity and wall distance give mean shear $U_z=u_*/(\kappa z)$. Its logarithmic integral uses the [roughness length](#roughness-length). The law applies outside the inner sublayer and below the outer boundary-layer scale, not all the way to a smooth wall.

<h5 id="von-karman-constant">Von Kármán constant</h5>

↑ **Parent:** [Law of the wall](#law-of-the-wall)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Von_Kármán_constant)

The dimensionless coefficient in the logarithmic wall law and its mixing-length form $\ell=\kappa z$. Its numerical value is determined from the turbulence closure and measurements, rather than from dimensional analysis alone.

##### Roughness length

↑ **Parent:** [Law of the wall](#law-of-the-wall)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Roughness_length)

The extrapolation height at which a logarithmic wall profile vanishes. For a fully rough wall it is set mainly by the geometry; for a smooth wall it scales with $\nu/u_*$. It is not the thickness of the molecular viscous sublayer or the literal location of a no-slip surface.

### Thermal boundary layer

↑ **Parent:** [Boundary layer](#boundary-layer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thermal_boundary_layer)

A thermal boundary layer is a thin region in which [temperature](thermodynamics.md#temperature) changes rapidly and [thermal conduction](thermodynamics.md#thermal-conduction) remains important. Its thickness can be estimated by balancing thermal diffusion against advection or by requiring a local [Rayleigh number](geophysics.md#rayleigh-number) to be near its critical value.

#### Boundary-layer renewal model

↑ **Parent:** [Thermal boundary layer](#thermal-boundary-layer)

In a renewal model, a diffusive [thermal boundary layer](#thermal-boundary-layer) grows until a convective instability overturns it, after which growth restarts. A layer reaching thickness $\delta\sim\sqrt{\kappa\tau}$ has mean [heat flux](thermodynamics.md#heat-flux-density) of order $k\Delta T/\delta$. A diffusive $t^{-1/2}$ flux averaged over one cycle differs only by an order-one coefficient. Distinct thermal and material layers need not share a renewal time.

### Boundary-layer scaling

↑ **Parent:** [Boundary layer](#boundary-layer)

Balancing $U^2/x$ with $\nu U/\delta^2$ gives $\delta\sim\sqrt{\nu x/U}$.

### Two-dimensional boundary-layer equations

↑ **Parent:** [Boundary layer](#boundary-layer)

For steady incompressible flow with imposed outer pressure gradient,

$$
u_x+v_y=0,
\qquad
uu_x+vu_y=-\frac1\rho p_x+\nu u_{yy}.
$$

The normal momentum equation makes pressure approximately uniform across the layer.

#### Boundary layer over a linearly stretching sheet

↑ **Parent:** [Two-dimensional boundary-layer equations](#two-dimensional-boundary-layer-equations)

For a sheet moving with $u(x,0)=\alpha x$ through otherwise stationary fluid, the layer thickness is $\delta=\sqrt{\nu/\alpha}$. With

$$
\eta=y/\delta,\qquad
\psi=\alpha x\delta f(\eta),
$$

the boundary-layer equations reduce to

$$
f'''+ff''-(f')^2=0,
\qquad
f(0)=0,\quad f'(0)=1,\quad f'(\infty)=0.
$$

The exact solution is $f=1-e^{-\eta}$.

### Flow separation

↑ **Parent:** [Boundary layer](#boundary-layer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Flow_separation)

Boundary-layer separation occurs where near-wall flow detaches from a surface, commonly after an adverse pressure gradient drives the wall shear to zero and then reverses it.

## Falkner-Skan equation

↑ **Parent:** [Continuum mechanics](continuum-mechanics.md)

For $U=Ax^m$, $\psi=\sqrt{\nu xU}f(\eta)$ gives

$$
f'''+\frac{m+1}{2}ff''+m(1-f'^2)=0,
$$

with $f(0)=f'(0)=0$ and $f'(\infty)=1$.

This equation and its boundary conditions determine the [Falkner-Skan boundary layer](#falkner-skan-boundary-layer).

## Acoustic energy flux

↑ **Parent:** [Continuum mechanics](continuum-mechanics.md)

For harmonic acoustic amplitudes, $\langle\mathbf I\rangle=\frac12\operatorname{Re}(p\mathbf u^*)$.

The instantaneous acoustic energy flux is $p\mathbf u$ for linear acoustics. Its time average is the [sound intensity](#sound-intensity).

### Spectral acoustic flux

↑ **Parent:** [Acoustic energy flux](#acoustic-energy-flux)

With the time convention $e^{-i\omega t}$, pressure amplitude $p$ and background density $\rho_0$, the [acoustic energy flux](#acoustic-energy-flux) is $I_x=(2\rho_0\omega)^{-1}\operatorname{Im}(\overline p\,\partial_xp)$. A transverse [plane wave](quantum-mechanics.md#plane-wave) mode with positive axial [wavenumber](wave-equation.md#wavenumber) $\kappa$ carries flux $\kappa|p|^2/(2\rho_0\omega)$. For the reduced pressure $p=e^{ikx}E$, the [parabolic wave equation](partial-differential-equation.md#parabolic-wave-equation) gives $\kappa=k-\nu^2/(2k)$, approximated by $k$ at leading paraxial order. Stationary illumination uses the [infinite-aperture spectral normalization](time-series.md#infinite-aperture-spectral-normalization): replace $|p|^2$ by the corresponding spectral power per unit transverse length. Other acoustic amplitude conventions change the dimensional prefactor.

### Transmitted velocity potential from a piston through an acoustic interface

↑ **Parent:** [Acoustic energy flux](#acoustic-energy-flux)

For a finite duct segment of phase length $\lambda$ joined to a semi-infinite medium, continuity of pressure and velocity gives the outgoing potential amplitude

$$
T=\epsilon c_-
\frac{i(\rho_+/\rho_-)\sin\lambda-(c_-/c_+)\cos\lambda}
{(\rho_+/\rho_-)^2\sin^2\lambda+(c_-/c_+)^2\cos^2\lambda}.
$$

At half-integer $\lambda/\pi$, a large impedance mismatch can strongly enhance transmitted flux for a prescribed piston displacement.

## Burgers vortex

↑ **Parent:** [Continuum mechanics](continuum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Burgers_vortex)

A Burgers vortex balances axial vortex stretching against radial viscous diffusion, producing a Gaussian vorticity profile.

### Burgers vortex sheet

↑ **Parent:** [Burgers vortex](#burgers-vortex)

A planar strained [shear layer](fluid-mechanics.md#shear-layer) is a [Burgers vortex sheet](#burgers-vortex-sheet). For strain $u_x=-\alpha x$, $u_z=\alpha z$ and transverse velocity $u_y=U\operatorname{erf}(x/\delta_s)$, viscous balance gives $\delta_s^2=2\nu/\alpha$. At fixed velocity jump its excess [viscous dissipation](stokes-flow.md#viscous-dissipation) per sheet area scales as $U^2\sqrt{\nu\alpha}$, which vanishes as [kinematic viscosity](fluid-mechanics.md#kinematic-viscosity) tends to zero.

### Excess dissipation of a Burgers vortex

↑ **Parent:** [Burgers vortex](#burgers-vortex)

The swirl [viscous dissipation](stokes-flow.md#viscous-dissipation) of a steady [Burgers vortex](#burgers-vortex), integrated per unit length and per unit density, is $\nu\int\omega_z^2\,dA=\alpha\Gamma^2/(8\pi)$. It remains finite as [kinematic viscosity](fluid-mechanics.md#kinematic-viscosity) tends to zero at fixed strain and [circulation](fluid-mechanics.md#circulation-physics). This is excess over the background strain: the uniform strain itself has infinite total [viscous dissipation](stokes-flow.md#viscous-dissipation) over an infinite cross-section.

### Unsteady Burgers-vortex core radius

↑ **Parent:** [Burgers vortex](#burgers-vortex)

An axisymmetric Gaussian [Burgers vortex](#burgers-vortex) with constant [circulation](fluid-mechanics.md#circulation-physics) in axial strain $\alpha$ has core area parameter $s=\delta^2$ satisfying $\dot s+\alpha s=4\nu$. Thus $s=4\nu/\alpha+(s_0-4\nu/\alpha)e^{-\alpha t}$, an attracting balance of transverse compression and viscous diffusion for every positive finite initial radius.

## Granular material

↑ **Parent:** [Continuum mechanics](continuum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Granular_material)

A granular material is an assembly of macroscopic solid particles whose collective mechanics is governed by contact, friction, rearrangement, and gravity.

### Angle of repose

↑ **Parent:** [Granular material](#granular-material)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Angle_of_repose)

The angle of repose is the steepest free-surface angle at which a loose granular material remains static. A released dry granular pile therefore tends toward a conical surface with slope $\tan\theta_r$.

## Elasticity (physics)

↑ **Parent:** [Continuum mechanics](continuum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Elasticity_(physics))

Elasticity studies reversible deformation and the stresses produced by it.

### Elastic deformation

↑ **Parent:** [Elasticity (physics)](#elasticity-physics)

An elastic deformation is recoverable when the deforming loads are removed. In a local elastic constitutive model the [stress](#stress) depends on the present deformation. When this response also derives from a stored [elastic energy](#elastic-energy), the material is a [hyperelastic material](#hyperelastic-material). In the small-deformation approximation, the relevant kinematic variable is the [infinitesimal strain tensor](#infinitesimal-strain-tensor).

### Perfectly bonded elastic interface

↑ **Parent:** [Elasticity (physics)](#elasticity-physics)

A [perfectly bonded elastic interface](#perfectly-bonded-elastic-interface) has continuous [displacement field](#displacement-field-mechanics) and continuous [traction](#traction), with the same chosen normal on both sides. For piecewise affine [displacement fields](#displacement-field-mechanics), the difference of their gradients annihilates every tangential vector, and hence has the form $a\otimes n$. Their [infinitesimal strain tensors](#infinitesimal-strain-tensor) differ by $\operatorname{sym}(a\otimes n)$.

### Static elastic equilibrium

↑ **Parent:** [Elasticity (physics)](#elasticity-physics)

A symmetric [stress tensor](#cauchy-stress-tensor) is in [static elastic equilibrium](#static-elastic-equilibrium) when its divergence balances the prescribed [body force](fluid-mechanics.md#body-force). Its boundary [traction](#traction) is $t_i=\sigma_{ij}n_j$. With zero [body force](fluid-mechanics.md#body-force), [integration by parts](calculus.md#integration-by-parts) gives $\int_\Omega\sigma:\operatorname{sym}\nabla v=\int_{\partial\Omega}t\cdot v$. This is the weak [principle of virtual work](classical-mechanics.md#virtual-work) for a static elastic body.

### Elastic beam

↑ **Parent:** [Elasticity (physics)](#elasticity-physics)

An [elastic beam](#elastic-beam) is a slender body that supports bending moments and transverse loads. In the small-slope Euler-Bernoulli approximation its bending moment is $M=EIy_{xx}$, and transverse momentum balance gives $\rho Ay_{tt}+EIy_{xxxx}=q$ for a uniform beam under distributed force per length $q$. Here $I$ is the [second moment of area](#second-moment-of-area); boundary conditions specify the end constraints and applied moments and forces.

### Dead loading

↑ **Parent:** [Elasticity (physics)](#elasticity-physics)

In an elastic [boundary value problem](differential-equation.md#boundary-value-problem), a dead load is a prescribed force independent of the incremental displacement. A dead reference [traction](#traction) has $\delta t^0=0$, even when the current face changes orientation. This differs from a follower load, whose direction follows the moving body, and from the structural-engineering use of the same phrase for permanent self-weight. Under pure dead [tractions](#traction), a constant incremental translation remains a zero-frequency mode unless a displacement condition fixes it.

### Magnetostriction

↑ **Parent:** [Elasticity (physics)](#elasticity-physics)

Magnetostriction is the coupling between a material's magnetic state and its mechanical deformation or stress. A constitutive expansion can contain coefficients constrained by rotational symmetry. In particular, an isotropic material cannot support a nonzero symmetric stress that is linear in a single magnetic-field vector through a third-rank isotropic coefficient.

#### Isotropic linear magnetostriction vanishes

↑ **Parent:** [Magnetostriction](#magnetostriction)

Under proper rotations a third-rank [isotropic tensor](linear-algebra.md#isotropic-tensor) is proportional to the [Levi-Civita symbol](calculus.md#levi-civita-symbol). Its contraction with a field vector is antisymmetric in the two stress indices. A physical symmetric stress therefore vanishes in this linear constitutive model. Under the full orthogonal [group](group.md) an ordinary isotropic third-rank [tensor](linear-algebra.md#tensor) is already zero; the orientation-sensitive Levi-Civita [tensor](linear-algebra.md#tensor) requires the usual pseudotensor distinction.

### Betti identity for elastodynamic fields

↑ **Parent:** [Elasticity (physics)](#elasticity-physics)

For two Fourier [elastic wave](wave-equation.md#elastic-wave) fields with the same real [elastic stiffness tensor](#elastic-stiffness-tensor), its major symmetry cancels the cross-strain terms in the [divergence](calculus.md#divergence) displayed above. The force-balance equations supply the remaining volume terms, and the [divergence theorem](calculus.md#divergence-theorem) gives their boundary integral of reciprocal [tractions](#traction). Taking one field to be a [complex conjugate](complex-analysis.md#complex-conjugate) gives energy-work identities and weighted modal [orthogonality](linear-algebra.md#orthogonal-vectors). The bilinear identity uses no [complex conjugation](complex-analysis.md#complex-conjugation) until that field is chosen explicitly.

### Shear modulus

↑ **Parent:** [Elasticity (physics)](#elasticity-physics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Shear_modulus)

### Finite elasticity

↑ **Parent:** [Elasticity (physics)](#elasticity-physics)

#### Inflation and extension of an incompressible tube

↑ **Parent:** [Finite elasticity](#finite-elasticity)

For reference radii $a_0,b_0$, current inner radius $a$ and uniform axial stretch $z>0$, [incompressibility](fluid-mechanics.md#incompressible-flow) integrates to $r^2=a^2+(R^2-a_0^2)/z$. The [principal stretches](#principal-stretch) are $r_{,R}=1/(z\lambda)$, $\lambda=r/R$ and $z$. Write $\widehat W(\lambda,z)=W((z\lambda)^{-1},\lambda,z)$ and $\mathcal E=2\pi\int_{a_0}^{b_0}\widehat W R\,dR$ per reference length. [Virtual work](classical-mechanics.md#virtual-work) gives $p=\mathcal E_{,a}/(2\pi az)$ and the total axial wall load $N_{\rm wall}=\mathcal E_{,z}$, both derivatives holding the other displayed parameter fixed. For pressurized closed ends the independently applied axial load is $N_{\rm ext}=N_{\rm wall}-\pi a^2p$. The distinction follows from the axial [pressure](thermodynamics.md#pressure) power $\pi a^2p\dot z$.

#### Constrained second-variation stability in elasticity

↑ **Parent:** [Finite elasticity](#finite-elasticity)

For an equilibrium with $P_{Ii}=W_{,F_{iI}}+q\phi_{,F_{iI}}$ and dead loads, the constrained [second variation](calculus-of-variations.md#second-variation) on $\phi_{,F}:\delta F=0$ is

$$
\mathcal Q[\delta F]=\int_\Omega(W_{,FF}+q\phi_{,FF})[\delta F,\delta F]\,dX.
$$

Indeed, a constraint-preserving perturbation path has $\phi_{,F}:\delta^2F=-\phi_{,FF}[\delta F,\delta F]$, and stationarity of the total potential supplies the multiplier term. Linearized kinetic energy plus $\mathcal Q/2$ is conserved. Positivity gives the usual energy-norm linear stability; control in a specified displacement norm additionally requires the corresponding coercivity and treatment of rigid-motion modes.

#### Torque and axial force of a twisted incompressible cylinder

↑ **Parent:** [Finite elasticity](#finite-elasticity)

For axial stretch $\lambda$ and twist per reference length $\alpha$, the deformation in local cylindrical orthonormal bases has

$$
F=\begin{pmatrix}\lambda^{-1/2}&0&0\\0&\lambda^{-1/2}&\alpha R\lambda^{-1/2}\\0&0&\lambda\end{pmatrix}.
$$

The [principal stretches](#principal-stretch) follow from the eigenvalues of $F^TF$. For a cylinder of reference radius $A$, stored energy per reference length is $\mathcal E=2\pi\int_0^A W(F)R\,dR$. Reversible power $M\dot\alpha+N\dot\lambda=\dot{\mathcal E}$ gives torque $M=\mathcal E_{,\alpha}$ and axial force $N=\mathcal E_{,\lambda}$. The relevant derivative holds the reference twist fixed, not the twist per current length.

##### Nominal end traction of a twisted neo-Hookean cylinder

↑ **Parent:** [Torque and axial force of a twisted incompressible cylinder](#torque-and-axial-force-of-a-twisted-incompressible-cylinder)

For axial stretch $\lambda$ and twist $\alpha$ per reference length, an incompressible [neo-Hookean solid](#neo-hookean-solid) has current radius $a=R/\sqrt\lambda$. In local cylindrical orthonormal bases the [deformation gradient](#deformation-gradient) is $A=\begin{pmatrix}\lambda^{-1/2}&0&0\\0&\lambda^{-1/2}&\alpha r\\0&0&\lambda\end{pmatrix}$. The [Cauchy stress tensor](#cauchy-stress-tensor) is $\mu AA^T+qI$. Radial equilibrium gives $q'=\mu\alpha^2r$, and a traction-free curved surface gives $q=-\mu/\lambda+\mu\alpha^2(r^2-a^2)/2$. The nominal end [traction](#traction) is the displayed [vector](vector-space.md#vector), measured per reference area. Its moment about the axis is $\int(x_1t_2-x_2t_1)dS_0=\mu\alpha\int r^2dS_0=\mu\pi R^4\alpha/(2\lambda)$. This calculation uses current moment arms with reference-area [tractions](#traction).

#### Twist and inflation of an incompressible tube

↑ **Parent:** [Finite elasticity](#finite-elasticity)

In cylindrical orthonormal bases the [deformation gradient](#deformation-gradient) is $F=\begin{pmatrix}\rho/r&0&0\\0&r/\rho&\alpha r\\0&0&1\end{pmatrix}$ and has unit [determinant](linear-algebra.md#determinant). One [principal stretch](#principal-stretch) is $\rho/r$; the squares of the other two are the roots of $z^2-[(r/\rho)^2+\alpha^2r^2+1]z+(r/\rho)^2=0$. The reference-volume energy per height is $E=2\pi\int\rho W\,d\rho$. [Virtual work](classical-mechanics.md#virtual-work) gives end [torque](classical-mechanics.md#torque) $M=\partial_\alpha E$ and inner pressure $p=(2\pi a)^{-1}\partial_aE$ at fixed reference radii and height.

##### Neo-Hookean tube pressure under twist and inflation

↑ **Parent:** [Twist and inflation of an incompressible tube](#twist-and-inflation-of-an-incompressible-tube)

Here $b^2=b_0^2+a^2-a_0^2$. Substitute the [neo-Hookean solid](#neo-hookean-solid) energy into the [twist and inflation of an incompressible tube](#twist-and-inflation-of-an-incompressible-tube) work identity. Differentiating with respect to $a$ gives the integrand $\mu\rho[\rho^{-2}-\rho^2/(\rho^2+c)^2+\alpha^2]$, with $c=a^2-a_0^2$. Integrating between the two reference radii proves the displayed pressure when the outer surface is traction free.

#### Inextensible fibre constraint

↑ **Parent:** [Finite elasticity](#finite-elasticity)

A unit reference fibre direction $m_0$ retains its length under this constraint on the [deformation gradient](#deformation-gradient). Its reaction contributes an undetermined tension along the current fibre direction, independently of the pressure reaction enforcing [incompressibility](fluid-mechanics.md#incompressible-flow).

##### Two-family inextensible-fibre pure stretch

↑ **Parent:** [Inextensible fibre constraint](#inextensible-fibre-constraint)

For two distinct reference fibre directions $l_\pm=(\cos\theta,\pm\sin\theta,0)$, with $0<\theta<\pi/2$, consider the volume-preserving deformation with [right stretch tensor](#right-stretch-tensor) $U=\operatorname{diag}(\lambda^{-1/2}\alpha,\lambda^{-1/2}\alpha^{-1},\lambda)$, with positive $\lambda,\alpha$. The [inextensible fibre constraint](#inextensible-fibre-constraint) gives $\alpha^2\cos^2\theta+\alpha^{-2}\sin^2\theta=\lambda$. Setting $b=\alpha^2$ gives a quadratic with the displayed roots. There are two distinct positive branches for $\lambda>\sin2\theta$. The smallest possible axial stretch is $\lambda=\sin2\theta$, at which $\alpha^2=\tan\theta$ and $(Ul_+)\cdot(Ul_-)=0$. Since both image fibres have unit length, their mutual area cannot exceed one; their area is $\sin2\theta/\lambda$, which gives the same lower bound. Coincident or antiparallel fibres at the angle endpoints do not give the two-family orthogonality conclusion.

##### Incompressible inextensible-fibre plane strain

↑ **Parent:** [Inextensible fibre constraint](#inextensible-fibre-constraint)

Let $e=(\cos\theta,\sin\theta)$ be the current fibre direction and $n=(-\sin\theta,\cos\theta)$. [Inextensibility](mathematical-biology.md#inextensible-filament) fixes the first column of the [deformation gradient](#deformation-gradient) to $e$, and [incompressibility](fluid-mechanics.md#incompressible-flow) fixes the second to $\gamma e+n$. Commuting mixed derivatives gives $\gamma_{,1}=\theta_{,1}$ and $\theta_{,2}=\gamma\theta_{,1}$. Thus $\gamma=\theta+f(X_2)$, and curves tangent to $(-\gamma,1)$ map to straight transverse curves with constant $\theta$.

###### Triangular equilibrium construction for inextensible-fibre plane strain

↑ **Parent:** [Incompressible inextensible-fibre plane strain](#incompressible-inextensible-fibre-plane-strain)

Write the [Cauchy stress tensor](#cauchy-stress-tensor) in the local fibre frame as $\sigma=s\,e\otimes e+h(e\otimes n+n\otimes e)+t\,n\otimes n$. The compatible geometry has $\nabla\theta=\kappa e$, $\nabla\cdot e=0$ and $\nabla\cdot n=-\kappa$. With zero [body force](fluid-mechanics.md#body-force), [force balance](classical-mechanics.md#force-balance) becomes $e\cdot\nabla s=2\kappa h-n\cdot\nabla h$ and $n\cdot\nabla t-\kappa t=-e\cdot\nabla h-\kappa s$. For specified [shear stress](viscous-fluid-flow.md#shear-stress) $h$, the first equation determines $s$ along fibres, then the second determines $t$ along transverse curves. Pressure and fibre tension supply these two normal constraint reactions. This is a local stress construction; boundary tractions must be chosen consistently with its integration data.

#### Hyperelastic material

↑ **Parent:** [Finite elasticity](#finite-elasticity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hyperelastic_material)

A hyperelastic material derives its elastic [stress](#stress) from a [strain energy density](#strain-energy-density). In reference-volume units its [first Piola-Kirchhoff stress tensor](#first-piola-kirchhoff-stress-tensor) is the derivative of that density with respect to the [deformation gradient](#deformation-gradient).

##### Compatibility condition for pure nonlinear transverse waves

↑ **Parent:** [Hyperelastic material](#hyperelastic-material)

For a plane material-coordinate [elastic wave](wave-equation.md#elastic-wave) with $u=(0,w(X_1,t),0)$, set $q=w_{,X_1}$. The longitudinal equation is $0=\partial_{X_1}P_{11}(1,q,0)$. Arbitrary nonuniform pure transverse profiles thus require the displayed constitutive compatibility, which does not follow from [isotropy](#isotropy) alone. If it holds and $\tau'(q)>0$, the shear equation closes as $\rho_0w_{tt}=\partial_{X_1}\tau(q)$ with speed $c(q)^2=\tau'(q)/\rho_0$.

###### Compatible nonlinear shear energy

↑ **Parent:** [Compatibility condition for pure nonlinear transverse waves](#compatibility-condition-for-pure-nonlinear-transverse-waves)

An explicit objective [isotropic](#isotropy) example is $\mathcal W=\mu(S-1)/2+h(S-1)^2/4+(\lambda+\mu)(J-1)^2/2$, with $J=\det A$, $S=\operatorname{tr}(A^{\mathsf T}A)-2J$, and $\lambda,\mu>0$, $h\ge0$. On $A=[(a,q,0)^{\mathsf T},e_2,e_3]$, $S-1=(a-1)^2+q^2$ and $J=a$, so $P_{11}=0$ at $a=1$ while the shear [nominal stress](#nominal-stress-tensor) is the displayed cubic. The natural-state quadratic energy has [Lamé parameters](#lame-parameter) $\lambda,\mu$, and the shear speed is $\sqrt{(\mu+3hq^2)/\rho_0}$.

<h5 id="saint-venant-kirchhoff-hyperelastic-energy">Saint Venant–Kirchhoff hyperelastic energy</h5>

↑ **Parent:** [Hyperelastic material](#hyperelastic-material)

This objective [isotropic](#isotropy) constitutive model uses the [Green-Lagrange strain tensor](#green-lagrange-strain-tensor) $E=(A^{\mathsf T}A-I)/2$. It reproduces [linear elasticity](#linear-elasticity) at small strain. Under simple shear $A=[(1,q,0)^{\mathsf T},e_2,e_3]$, its longitudinal [nominal stress](#nominal-stress-tensor) is $(\lambda+2\mu)q^2/2$. Nonuniform finite shear therefore generates longitudinal acceleration, even though the corresponding infinitesimal transverse mode is uncoupled.

<h5 id="lame-parameters-from-hyperelastic-energy-hessian">Lamé parameters from hyperelastic energy Hessian</h5>

↑ **Parent:** [Hyperelastic material](#hyperelastic-material)

At a stress-free natural reference state, an objective [isotropic](#isotropy) [hyperelastic material](#hyperelastic-material) with energy $W$ per unit mass has $\rho_0[W(I+H)-W(I)]=\lambda(\operatorname{tr}e)^2/2+\mu e:e+O(|H|^3)$, where $e=\operatorname{sym}H$. Twice differentiating gives the displayed [Lamé parameters](#lame-parameter) and the usual [elastic stiffness tensor](#elastic-stiffness-tensor). A prestressed reference requires initial-stress corrections.

##### Inflation pressure of a thin incompressible elastic balloon

↑ **Parent:** [Hyperelastic material](#hyperelastic-material)

At leading thin-shell order, a spherical balloon with reference radius $a_0$, thickness $h_0$ and current radius $a=\lambda a_0$ has reference [elastic energy](#elastic-energy) $4\pi a_0^2h_0W(\lambda,\lambda,\lambda^{-2})$. Equating its differential to pressure work $p\,4\pi a^2da$ gives the displayed pressure difference. Its thickness becomes $h_0\lambda^{-2}$ by [incompressibility](fluid-mechanics.md#incompressible-flow). The same result follows from the spherical membrane [force](classical-mechanics.md#force) balance $p=2h\sigma_t/a$, with current tangential [Cauchy stress tensor](#cauchy-stress-tensor) component $\sigma_t=\lambda N$ and the [equibiaxial nominal tension of an incompressible sheet](#equibiaxial-nominal-tension-of-an-incompressible-sheet). Thin-shell validity requires $h/a\ll1$.

##### Incremental elastic moduli

↑ **Parent:** [Hyperelastic material](#hyperelastic-material)

For unconstrained [hyperelastic material](#hyperelastic-material), the [Hessian](calculus.md#hessian-matrix) of the [strain energy density](#strain-energy-density) gives $\delta N_{\alpha i}=c_{\alpha i\beta j}\delta A_{j\beta}$. Commuting the second derivatives gives major symmetry $c_{\alpha i\beta j}=c_{\beta j\alpha i}$. These material-coordinate moduli linearize about a finite base deformation; they need not have the minor symmetries of a small-strain [elastic stiffness tensor](#elastic-stiffness-tensor). Material constraints require their additional reaction increments and admissibility equations.

###### Elastic normal-mode energy identity

↑ **Parent:** [Incremental elastic moduli](#incremental-elastic-moduli)

For a static base state with zero incremental [body force](fluid-mechanics.md#body-force), homogeneous incremental [tractions](#traction) or homogeneous [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition) eliminate the boundary term in [integration by parts](calculus.md#integration-by-parts). The displayed [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient) then gives real squared frequencies because of major symmetry. Positive moduli give strictly positive squared frequencies for modes with nonzero displacement gradient. Pure [dead loading](#dead-loading) leaves constant translations at zero; fixed displacement conditions remove those modes.

###### Strong ellipticity in elasticity

↑ **Parent:** [Incremental elastic moduli](#incremental-elastic-moduli)

Strong ellipticity requires the displayed inequality for every nonzero displacement vector $m$ and material direction $\nu$. Equivalently, every [acoustic tensor](#acoustic-tensor) is [positive-definite](linear-algebra.md#positive-definite-bilinear-form). It is weaker than positivity of the moduli on all matrices. A [quadratic minor null Lagrangian](calculus-of-variations.md#quadratic-minor-null-lagrangian) vanishes on rank-one matrices, so adding such a term does not change the acoustic tensor or this condition.

###### Acoustic tensor

↑ **Parent:** [Incremental elastic moduli](#incremental-elastic-moduli)

The acoustic tensor determines the [plane waves](quantum-mechanics.md#plane-wave) of a locally uniform incremental elastic medium. For a unit material direction $\nu$, its [eigenvalues](linear-operator-theory.md#eigenvalue) are $\rho_0c^2$ and its [eigenvectors](linear-operator-theory.md#eigenvector) are displacement polarizations. Major symmetry of the [incremental elastic moduli](#incremental-elastic-moduli) makes $Q$ a real [symmetric matrix](linear-algebra.md#symmetric-matrix). Positivity on every [rank-one matrix](vector-space.md#rank-one-matrix) $m\otimes\nu$ makes all its wave speeds real and nonzero.

##### Constraint reaction in hyperelastic stress

↑ **Parent:** [Hyperelastic material](#hyperelastic-material)

For a regular material constraint $F(A)=0$, admissible rates of the [deformation gradient](#deformation-gradient) lie in the kernel of $F_{,A}$. The difference between the [nominal stress](#nominal-stress-tensor) and the derivative of the [strain energy density](#strain-energy-density) annihilates that tangent space by [virtual work](classical-mechanics.md#virtual-work), so it is a [Lagrange multiplier](mathematical-optimization.md#lagrange-multiplier) times $F_{,A}$. For [incompressibility](fluid-mechanics.md#incompressible-flow), the derivative of the [determinant](linear-algebra.md#determinant) is its [cofactor matrix](linear-algebra.md#cofactor-matrix), and the material-first reaction is $qA^{-1}$ when $\det A=1$.

###### Equibiaxial nominal tension of an incompressible sheet

↑ **Parent:** [Constraint reaction in hyperelastic stress](#constraint-reaction-in-hyperelastic-stress)

A thin isotropic [hyperelastic material](#hyperelastic-material) subject to [incompressibility](fluid-mechanics.md#incompressible-flow), with equal in-plane [principal stretches](#principal-stretch) $\lambda$ has transverse stretch $\lambda^{-2}$. With unloaded transverse faces, $N_{33}=W_3+q\lambda^2=0$. Hence $N_{11}=N_{22}=W_1-\lambda^{-3}W_3$, using isotropy to set $W_1=W_2$. The derivative along the constrained path is $W_1+W_2-2\lambda^{-3}W_3$, proving the displayed formula. The two equal nominal tensions do work $2N\,d\lambda$ per reference volume, exactly the change in [strain energy density](#strain-energy-density).

##### Mooney-Rivlin solid

↑ **Parent:** [Hyperelastic material](#hyperelastic-material)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mooney–Rivlin_solid)

An incompressible [Mooney-Rivlin solid](#mooney-rivlin-solid) has [strain energy density](#strain-energy-density) $W=C_1(I_1-3)+C_2(I_2-3)$, with [right Cauchy-Green deformation tensor](#right-cauchy-green-deformation-tensor) $C=F^TF$, $I_1=\operatorname{tr}C$ and $I_2=\operatorname{tr}C^{-1}$ when $\det C=1$. It extends the [neo-Hookean solid](#neo-hookean-solid) by a second invariant. A convention $W=\mu_1(I_1-3)/2-\mu_2(I_2-3)/2$ means $C_1=\mu_1/2$, $C_2=-\mu_2/2$; the minus sign must be retained when comparing material constants.

##### Neo-Hookean solid

↑ **Parent:** [Hyperelastic material](#hyperelastic-material)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Neo-Hookean_solid)

For an incompressible neo-Hookean solid, a convenient [strain energy density](#strain-energy-density) is $W=\mu(\operatorname{tr}C-3)/2$, where $C$ is the [right Cauchy-Green deformation tensor](#right-cauchy-green-deformation-tensor). An additive constant in $W$ does not affect the [stress](#stress). The [shear modulus](#shear-modulus) $\mu$ fixes the small-strain stiffness.

###### Homogeneous tensile bifurcation of a neo-Hookean cube

↑ **Parent:** [Neo-Hookean solid](#neo-hookean-solid)

For the volume-preserving family $F=\operatorname{diag}(\lambda,\lambda^{-1/2},\lambda^{-1/2})$, equal dead nominal tension $T$ gives potential

$$
\Pi(\lambda)=\frac\mu2(\lambda^2+2\lambda^{-1}-3)-T(\lambda+2\lambda^{-1/2}-3).
$$

Its derivative factors as $\Pi'=(1-\lambda^{-3/2})[\mu(\lambda+\lambda^{-1/2})-T]$. The nontrivial branch has a fold at $\lambda=2^{-2/3}$, $T/\mu=3\,2^{-2/3}$, and meets the trivial branch at $T/\mu=2$. Stability in this one-parameter family is determined by $\Pi''$, not by branch count alone. At $T/\mu=2$ there is only one nontrivial positive solution, $\lambda=(3-\sqrt5)/2$; the other branch value is $\lambda=1$.

##### Strain energy density

↑ **Parent:** [Hyperelastic material](#hyperelastic-material)

###### Nonnegative isotropic elastic strain energy

↑ **Parent:** [Strain energy density](#strain-energy-density)

In three-dimensional isotropic [linear elasticity](#linear-elasticity), decompose the symmetric strain as $e=pI+d$ with $p=\operatorname{tr}(e)/3$ and $\operatorname{tr}d=0$. The stored energy is $E=\mu\sum_{ij}d_{ij}^2+\tfrac32(3\lambda+2\mu)p^2$. Its nonnegativity for every strain is equivalent to the displayed inequalities: the traceless and purely volumetric test strains prove necessity, and the sum of squares proves sufficiency.

#### Material isotropy

↑ **Parent:** [Finite elasticity](#finite-elasticity)

Material isotropy makes the elastic response independent of a rotation of reference material directions: $\sigma(FR)=\sigma(F)$ for proper rotations $R$. Combined with [material frame indifference](#material-frame-indifference), it yields [coaxiality of isotropic elastic stress](#coaxiality-of-isotropic-elastic-stress).

##### Coaxiality of isotropic elastic stress

↑ **Parent:** [Material isotropy](#material-isotropy)

The [polar decomposition in continuum mechanics](#polar-decomposition-in-continuum-mechanics) and [material isotropy](#material-isotropy) remove the reference rotation from an elastic [Cauchy stress tensor](#cauchy-stress-tensor). Half-turns around principal stretch axes leave the diagonal [left stretch tensor](#left-stretch-tensor) fixed, so [material frame indifference](#material-frame-indifference) forces the stress's off-diagonal entries to vanish in those axes. Rotations within repeated-stretch eigenspaces also force isotropic stress there. Consequently stress and the [left Cauchy-Green deformation tensor](#left-cauchy-green-deformation-tensor) are [coaxial symmetric tensors](linear-algebra.md#coaxial-symmetric-tensors).

###### Equivariance of isotropic principal stresses

↑ **Parent:** [Coaxiality of isotropic elastic stress](#coaxiality-of-isotropic-elastic-stress)

For an objective [material isotropy](#material-isotropy) law, permutation of the [principal stretches](#principal-stretch) permutes the labelled [principal stresses](#principal-stress). This follows by conjugating the [left stretch tensor](#left-stretch-tensor) with signed permutation [rotation matrices](linear-algebra.md#rotation-matrix). Each principal stress is symmetric in the other two stretches, but need not be symmetric in all three. The law $\sigma=V^2$ provides the example $\sigma_i=\lambda_i^2$. In an invariant representation $\sigma=\beta_0I+\beta_1V+\beta_2V^2$, the scalar coefficients are symmetric functions of the unordered stretches.

###### Universal simple-shear normal-stress identity

↑ **Parent:** [Coaxiality of isotropic elastic stress](#coaxiality-of-isotropic-elastic-stress)

For [simple shear](#simple-shear), $B=\begin{pmatrix}1+\gamma^2&\gamma\\\gamma&1\end{pmatrix}$. The off-diagonal entry of $\sigma B-B\sigma$ is $\gamma(\sigma_{11}-\sigma_{22})-\gamma^2\sigma_{12}$. [Coaxiality of isotropic elastic stress](#coaxiality-of-isotropic-elastic-stress) therefore proves the identity for $\gamma\ne0$. At $\gamma=0$, [material isotropy](#material-isotropy) makes the stress isotropic, proving the same identity.

### Elastic filament

↑ **Parent:** [Elasticity (physics)](#elasticity-physics)

An elastic filament is a slender elastic body modeled by a centerline and bending rigidities. Its [elastic energy](#elastic-energy) penalizes curvature. In a small-deflection representation $(x,y(x),z(x))$, the bending energy is quadratic in $y^{\prime\prime}$ and $z^{\prime\prime}$. Compression can cause [Euler buckling of an elastic filament](mathematical-biology.md#euler-buckling-of-an-elastic-filament).

#### Filament torsional stiffness

↑ **Parent:** [Elastic filament](#elastic-filament)

For an isotropic elastic rod with shear modulus $G_s$, polar second moment of area $J_p$, and twist rate $\Omega$, the torque is $C\Omega$ and the energy per length is $C\Omega^2/2$. For a circular section of radius $r$, $J_p=\pi r^4/2$. This material twist stiffness is distinct from the energy of bending filament centerlines into a helix.

#### Intrinsic curvature of an elastic filament

↑ **Parent:** [Elastic filament](#elastic-filament)

The intrinsic [signed curvature](differential-geometry.md#signed-curvature) is the curvature of a stress-free filament, measured along material [arc length](riemannian-geometry.md#arc-length). An [elastic filament](#elastic-filament) with actual curvature $\kappa$ stores bending energy $\frac B2\int(\kappa-\kappa_0)^2ds$, with [filament bending modulus](mathematical-biology.md#filament-bending-modulus) $B$. In a planar small-slope [Monge representation](mathematical-biology.md#monge-representation), $\kappa\simeq\zeta''$ and the leading energy is quadratic in $\zeta''-\kappa_0$.

##### Free-end curvature boundary layer

↑ **Parent:** [Intrinsic curvature of an elastic filament](#intrinsic-curvature-of-an-elastic-filament)

Moment-free ends require $\zeta''=\kappa_0$ there, so a highly stretched finite filament can retain curvature in boundary layers of width $\ell=\sqrt{B/F}$. For constant intrinsic curvature $\kappa$, zero transverse end forces give slope $\zeta'(x)=\kappa\ell\sinh[(x-L/2)/\ell]/\cosh[L/(2\ell)]$. Direct integration yields

$$
\mathcal L-L=\frac{\kappa^2\ell^3}2\left[\tanh a-a\operatorname{sech}^2a\right],\qquad a=L/(2\ell).
$$

Its large-force deficit is $\kappa^2\ell^3/2$, of order $F^{-3/2}$, even though the smooth bulk curvature derivative vanishes. This shows why endpoint assumptions matter in [force-extension of an intrinsically curved filament](#force-extension-of-an-intrinsically-curved-filament).

##### Force-extension of an intrinsically curved filament

↑ **Parent:** [Intrinsic curvature of an elastic filament](#intrinsic-curvature-of-an-elastic-filament)

For a planar [elastic filament](#elastic-filament) under positive constant extension force $F$, the quadratic force-controlled energy is

$$
\mathcal H=\frac12\int\left[B(\zeta''-\kappa_0)^2+F(\zeta')^2\right]dx.
$$

The [higher-order Euler-Lagrange equation](analysis.md#higher-order-euler-lagrange-equation) is $B\zeta''''-F\zeta''=B\kappa_0''$. On a periodic interval or in a bulk [Fourier transform](analysis.md#fourier-transform) treatment, every nonzero mode obeys the displayed transfer relation. The length deficit is $\frac12\int(\zeta')^2dx$, so its ensemble value is determined by the [power spectrum](probability-and-statistics.md#power-spectrum) of the [quenched intrinsic curvature](#quenched-intrinsic-curvature). Boundary conditions must be specified for a finite filament.

###### Smooth-curvature high-force extension law

↑ **Parent:** [Force-extension of an intrinsically curved filament](#force-extension-of-an-intrinsically-curved-filament)

For a stationary [quenched intrinsic curvature](#quenched-intrinsic-curvature) with [power spectrum](probability-and-statistics.md#power-spectrum) $S_\kappa(q)$ and finite second spectral moment, the bulk deficit satisfies

$$
\frac{\langle\mathcal L-L\rangle}{L}=\frac{B^2}2\int\frac{dq}{2\pi}\frac{q^2S_\kappa(q)}{(F+Bq^2)^2}
\sim\frac{B^2}{2F^2}\int\frac{dq}{2\pi}q^2S_\kappa(q).
$$

The moment is $\langle(\kappa_0')^2\rangle$ for mean-square differentiable curvature. Infinite-moment disorder and finite endpoint boundary layers can change the exponent, so this is a smooth bulk law rather than a universal law for all random polymers.

##### Quenched intrinsic curvature

↑ **Parent:** [Intrinsic curvature of an elastic filament](#intrinsic-curvature-of-an-elastic-filament)

Quenched [intrinsic curvature of an elastic filament](#intrinsic-curvature-of-an-elastic-filament) is fixed during a mechanical experiment, although different filaments can have different random intrinsic shapes. Ensemble averaging is then over these shapes after mechanical minimization. It differs from averaging over time-dependent thermal bending fluctuations in a [worm-like chain](mathematical-biology.md#worm-like-chain).

#### Spatially varying tension in filament bending

↑ **Parent:** [Elastic filament](#elastic-filament)

Adding $\frac12\int\sigma(x)(h')^2dx$ to the quadratic bending energy of an [elastic filament](#elastic-filament) contributes $-(\sigma h')'$ to its [variational derivative](classical-mechanics.md#variational-derivative). The endpoint term is $Ah''\eta'+(\sigma h'-Ah''')\eta$. If the real [filament tension](mathematical-biology.md#filament-tension) vanishes at both ends, the usual [self-adjoint endpoint conditions for filament bending](#self-adjoint-endpoint-conditions-for-filament-bending) remain valid. A complete [eigenfunction expansion](algebra.md#eigenfunction-expansion) diagonalizes the energy even when the [eigenfunctions](linear-operator-theory.md#eigenfunction) have no explicit formula. Thermal [equipartition theorem](statistical-physics.md#equipartition-theorem) arguments require positive eigenvalues after fixing any [kernel](linear-algebra.md#kernel-of-a-linear-map); strong compression can violate this requirement.

#### Thermal covariance of an elastic filament

↑ **Parent:** [Elastic filament](#elastic-filament)

For a positive quadratic bending operator $K$ with a real [orthonormal basis](linear-algebra.md#orthonormal-basis) of [eigenfunctions](linear-operator-theory.md#eigenfunction), the [equipartition theorem](statistical-physics.md#equipartition-theorem) gives $C(x,y)=k_BT\sum_nW_n(x)W_n(y)/\mu_n$, where $KW_n=\mu_nW_n$. This is the inverse-operator [Green function](analysis.md#green-s-function) multiplied by [Boltzmann constant](thermodynamics.md#boltzmann-constant) and [temperature](thermodynamics.md#temperature). Unconstrained [zero-energy filament modes](#zero-energy-filament-mode) prevent a normalizable [canonical ensemble](statistical-physics.md#canonical-ensemble), and negative modes signal an unstable quadratic model.

For both ends clamped and $K=A\partial_x^4$, the diagonal is $C(x,x)=k_BT x^3(L-x)^3/(3AL^3)$. This differs from a clamped-free tip [variance](variance.md). The center [variance](variance.md) is $k_BT L^3/(192A)$.

##### Rigid-motion-projected thermal covariance of a free filament

↑ **Parent:** [Thermal covariance of an elastic filament](#thermal-covariance-of-an-elastic-filament)

Free bending has two [zero-energy filament modes](#zero-energy-filament-mode), so it does not define an unrestricted normalizable thermal height distribution. Fix the mean displacement and linear tilt, or project out that affine kernel. On the positive complement, the [equipartition theorem](statistical-physics.md#equipartition-theorem) gives independent Gaussian mode [variances](variance.md) $k_BT/(Ak_n^4)$ for normalized modes. The resulting [covariance](variance.md#covariance) is the bending operator pseudoinverse multiplied by $k_BT$. It depends on how the rigid motion is fixed.

###### Curvature-noise representation of a free filament

↑ **Parent:** [Rigid-motion-projected thermal covariance of a free filament](#rigid-motion-projected-thermal-covariance-of-a-free-filament)

The quadratic bending energy makes curvature a [white noise](time-series.md#white-noise) field in the generalized thermal description. Integrate it twice, then subtract the affine least-squares projection to fix translation and tilt. With $u=x/L$ and $t=s/L$, the dimensionless kernel is $(u-t)_+-(1-t)^2/2-(1-3t^2+2t^3)(u-1/2)$. Its second spatial derivative is the source delta and its mean and first moment are zero. Its squared integral yields the [free-filament variance with fixed translation and tilt](#free-filament-variance-with-fixed-translation-and-tilt).

###### Free-filament variance with fixed translation and tilt

↑ **Parent:** [Rigid-motion-projected thermal covariance of a free filament](#rigid-motion-projected-thermal-covariance-of-a-free-filament)

For the frame fixed by zero mean height and zero first height moment, the [variance](variance.md) profile is $P(u)=1/105-11u/105+13u^2/35-u^3/3-u^4/3+3u^5/5-u^6/5$. It obeys $P(1-u)=P(u)$, $P(0)=1/105$ and $P(1/2)=1/320$. Integrating a [white noise](time-series.md#white-noise) curvature field twice, subtracting its affine projection and integrating the squared kernel proves the profile. These free-end conditions must not be confused with physically clamping the ends.

##### Zero-energy filament mode

↑ **Parent:** [Thermal covariance of an elastic filament](#thermal-covariance-of-an-elastic-filament)

A zero-energy mode lies in the [kernel](linear-algebra.md#kernel-of-a-linear-map) of the quadratic [elastic filament](#elastic-filament) operator. For pure bending, zero curvature makes the displacement affine. Free-free endpoints therefore leave translation and tilt modes, while slope-constrained, force-free endpoints leave only translation. Both clamped-clamped and hinged-hinged endpoints remove these modes. An unrestricted modal amplitude has constant [Boltzmann distribution](thermodynamics.md#boltzmann-distribution) weight, so no normalizable [canonical ensemble](statistical-physics.md#canonical-ensemble) or finite displacement [variance](variance.md) exists. Fixing the rigid degrees of freedom allows the [equipartition theorem](statistical-physics.md#equipartition-theorem) on the positive complement.

<h4 id="clamped-clamped-bending-mode">Clamped--clamped bending mode</h4>

↑ **Parent:** [Elastic filament](#elastic-filament)

A [normal mode](wave-equation.md#normal-mode) of a uniformly bending [elastic filament](#elastic-filament) fixed in position and slope at both ends satisfies $W''''=k^4W$. With $\beta=kL>0$, the allowed [wavenumbers](wave-equation.md#wavenumber) solve $\cos\beta\cosh\beta=1$. The first root is $4.730040745$ and $\beta_n=(n+\tfrac12)\pi+O(e^{-(n+1/2)\pi})$ for $n\geq1$. The apparent root at zero is not an [eigenfunction](linear-operator-theory.md#eigenfunction): the zero-eigenvalue cubic polynomial satisfying all four [clamped boundary conditions](differential-equation.md#clamped-boundary-condition) is identically zero. This spectrum differs from that of a filament clamped only at one end.

#### Self-adjoint endpoint conditions for filament bending

↑ **Parent:** [Elastic filament](#elastic-filament)

For the [elastic filament](#elastic-filament) operator $K=A\partial_x^4$, two [integration by parts](calculus.md#integration-by-parts) operations give boundary form $A[\overline u v'''-\overline{u'}v''+\overline{u''}v'-\overline{u'''}v]$. Four elementary homogeneous choices at each endpoint are $h=h'=0$ (clamped), $h=h''=0$ (hinged), $h''=h'''=0$ (free), and $h'=h'''=0$ (slope-constrained and transverse-force-free). Each defines a [self-adjoint operator](linear-operator-theory.md#self-adjoint-operator) on a finite interval when imposed at both ends. More general real [Robin boundary conditions](differential-equation.md#robin-boundary-condition) also give [self-adjointness](linear-operator-theory.md#self-adjoint-operator); the four choices are not an exhaustive classification of all boundary subspaces.

##### Free-end bending boundary conditions

↑ **Parent:** [Self-adjoint endpoint conditions for filament bending](#self-adjoint-endpoint-conditions-for-filament-bending)

Variation of the small-slope bending energy of an [elastic filament](#elastic-filament) gives endpoint work $A[h^{(2)}\delta h^{(1)}-h^{(3)}\delta h]$. Arbitrary endpoint displacement and slope variations force the bending moment and transverse force to vanish. These are $h^{(2)}=h^{(3)}=0$. They define a [self-adjoint](linear-operator-theory.md#self-adjoint-operator) nonnegative fourth-order bending operator on a finite interval; its kernel contains rigid translation and tilt.

###### Free-free bending spectrum

↑ **Parent:** [Free-end bending boundary conditions](#free-end-bending-boundary-conditions)

Nonzero bending modes have the [sine](geometry-and-topology.md#sine), [cosine](geometry-and-topology.md#cosine), [hyperbolic sine](calculus.md#hyperbolic-sine) and [hyperbolic cosine](calculus.md#hyperbolic-cosine) form. Free conditions at the first end identify the [cosine](geometry-and-topology.md#cosine) and [hyperbolic cosine](calculus.md#hyperbolic-cosine) coefficients, and likewise the [sine](geometry-and-topology.md#sine) coefficients. The remaining boundary determinant is $2(1-\cos q\cosh q)$. Its first positive roots are about $4.73004,7.85320,10.99561$. The complete basis additionally includes two [zero-energy filament modes](#zero-energy-filament-mode), constant translation and affine tilt; these are absent from the finite-coefficient formula at $k=0$.

###### Stable characteristic equation for free-free bending modes

↑ **Parent:** [Free-free bending spectrum](#free-free-bending-spectrum)

Writing the characteristic equation with reciprocal [hyperbolic cosine](calculus.md#hyperbolic-cosine) avoids exponentially large products. For the positive roots indexed from one, $q_n=(n+1/2)\pi+2(-1)^{n+1}e^{-(n+1/2)\pi}+O(e^{-2(n+1/2)\pi})$. The apparent root at zero represents the separate affine kernel, not another positive bending mode. Evaluating hyperbolic pieces of high modes with decaying exponential forms also avoids cancellation.

#### Tip-force compliance of a cantilever

↑ **Parent:** [Elastic filament](#elastic-filament)

For a clamped [elastic filament](#elastic-filament) of [filament bending modulus](mathematical-biology.md#filament-bending-modulus) $A$, a transverse tip force $f$ gives $h(x)=fx^2(3L-x)/(6A)$ in the small-slope model. Thus $h(L)/f=L^3/(3A)$. This differs from the effective tip stiffness under a distributed load. The zero-load Gaussian response reproduces the [thermal bending fluctuations of a clamped filament](mathematical-biology.md#thermal-bending-fluctuations-of-a-clamped-filament), $\langle h(L)^2\rangle=k_BTL^3/(3A)$ for one transverse coordinate.

### Elastic energy

↑ **Parent:** [Elasticity (physics)](#elasticity-physics)

Elastic energy is the recoverable energy stored by deforming an elastic material. In the small-deflection model of an [elastic filament](#elastic-filament), the bending contribution is a positive quadratic functional of the curvatures, such as $\tfrac12\int(Ay''^2+Bz''^2)\,dx$. Work by applied loads must also be included when minimizing the total potential energy.

#### Minimum potential energy principle in elasticity

↑ **Parent:** [Elastic energy](#elastic-energy)

Let a convex [strain energy density](#strain-energy-density) have derivative equal to the actual [stress tensor](#cauchy-stress-tensor). Under mixed displacement and [traction](#traction) data, any equilibrated [stress](#stress) $\sigma_0$ with the prescribed [body force](fluid-mechanics.md#body-force) and boundary [tractions](#traction) represents the external work. For any compatible trial [strain](#strain) $\varepsilon'$, the convex supporting-plane inequality gives $W(\varepsilon')-W(\varepsilon)\ge\sigma:(\varepsilon'-\varepsilon)$. The integral of $(\sigma-\sigma_0):(\varepsilon'-\varepsilon)$ vanishes by [integration by parts](calculus.md#integration-by-parts). Thus the actual [strain](#strain) minimizes $\int(W-\sigma_0:\varepsilon)$.

### Linear elasticity

↑ **Parent:** [Elasticity (physics)](#elasticity-physics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_elasticity)

Linear elasticity approximates strain and stress to first order in a small displacement field.

#### Mean stress and strain boundary identities

↑ **Parent:** [Linear elasticity](#linear-elasticity)

Apply the [divergence theorem](calculus.md#divergence-theorem) to $\partial_k(x_i\sigma_{jk})$ and use momentum balance $\sigma_{jk,k}=\rho(a_j-b_j)$ and stress symmetry to obtain the displayed mean [stress](#stress) identity. Applying the same theorem to the [infinitesimal strain tensor](#infinitesimal-strain-tensor) gives $V\overline e_{ij}=\frac12\int_S(u_in_j+u_jn_i)\,dS$. The acceleration term cannot be dropped during a transient.

##### Equilibrium contraction of a self-gravitating elastic sphere

↑ **Parent:** [Mean stress and strain boundary identities](#mean-stress-and-strain-boundary-identities)

For a uniform traction-free sphere, first-order self-gravity is $b=-gx/a$. Static averaging gives $\overline\sigma=-\rho gaI/5$. Homogeneous [linear elasticity](#linear-elasticity) then gives $\overline e=-\rho gaI/(15\kappa)$. The boundary strain identity identifies $\overline e=u(a)I/a$, proving the displayed positive radius decrease. The local strain is not uniform, and the cancellation of the [shear modulus](#shear-modulus) concerns only the mean contraction.

#### Elastic strain Green operator

↑ **Parent:** [Linear elasticity](#linear-elasticity)

For a homogeneous comparison [elastic stiffness tensor](#elastic-stiffness-tensor) $C^0$, the [elastic strain Green operator](#elastic-strain-green-operator) maps an [elastic polarization](#elastic-polarization) to minus the induced [infinitesimal strain tensor](#infinitesimal-strain-tensor). In a bounded domain the induced [displacement field](#displacement-field-mechanics) has zero boundary data; in an infinite medium it is the decaying perturbation. The defining [static elastic equilibrium](#static-elastic-equilibrium) equation is $\nabla\cdot(C^0\operatorname{sym}\nabla u+\tau)=0$. The bounded-domain operator is self-adjoint, annihilates constant [elastic polarizations](#elastic-polarization), has zero mean output, and satisfies $\Gamma C^0\Gamma=\Gamma$.

##### Isotropic elastic strain Green kernel

↑ **Parent:** [Elastic strain Green operator](#elastic-strain-green-operator)

For a three-dimensional isotropic comparison material, the contraction of its [elastic strain Green operator](#elastic-strain-green-operator) is the displayed [distributional derivative](distribution-theory.md#distributional-derivative). Its double trace is $\Gamma_{iikk}=\delta/L$, because $\Delta|x|^{-1}=-4\pi\delta$. Away from zero the contraction is $(\delta_{ij}|x|^2-3x_ix_j)/(4\pi L|x|^5)$; the full [distribution](distribution-theory.md#distribution-mathematical-analysis) also includes $\delta_{ij}\delta/(3L)$. This contact term must not be discarded when computing hydrostatic [strain](#strain).

###### Constant-shear bulk-modulus inclusion

↑ **Parent:** [Isotropic elastic strain Green kernel](#isotropic-elastic-strain-green-kernel)

When only the [bulk modulus](#bulk-modulus) differs from an isotropic matrix, the [elastic polarization](#elastic-polarization) is spherical: $\tau=(\kappa-\kappa^0)\operatorname{tr}(\varepsilon)I$. The double trace of the [isotropic elastic strain Green kernel](#isotropic-elastic-strain-green-kernel) makes the trace equation local, giving the displayed formula. Individual [strain](#strain) components still depend on a nonlocal potential of the spherical polarization, so the complete [infinitesimal strain tensor](#infinitesimal-strain-tensor) is not generally a local multiple of its reference value.

##### Directional elastic strain Green operator

↑ **Parent:** [Elastic strain Green operator](#elastic-strain-green-operator)

Let $B_na=\operatorname{sym}(a\otimes n)$; its adjoint on symmetric [stress tensors](#cauchy-stress-tensor) is $B_n^T\tau=\tau n$. Then $B_n^TCB_n$ is the [acoustic tensor](#acoustic-tensor). The [directional elastic strain Green operator](#directional-elastic-strain-green-operator) satisfies the resolvent identity $\widetilde\Gamma_r(C^r-C^s)\widetilde\Gamma_s=\widetilde\Gamma_s-\widetilde\Gamma_r$, by the elementary inverse identity $K_r^{-1}(K_r-K_s)K_s^{-1}=K_s^{-1}-K_r^{-1}$.

##### Elastic polarization

↑ **Parent:** [Elastic strain Green operator](#elastic-strain-green-operator)

The [elastic polarization](#elastic-polarization) is the excess [stress](#stress) relative to a homogeneous comparison [elastic stiffness tensor](#elastic-stiffness-tensor). In heterogeneous [linear elasticity](#linear-elasticity), $\tau=(C-C^0)\varepsilon$. The comparison [static elastic equilibrium](#static-elastic-equilibrium) equation gives the integral equation $\varepsilon=\varepsilon^0-\Gamma\tau$, where $\varepsilon^0$ is the reference [strain](#strain) under the same external loading.

#### Bulk modulus

↑ **Parent:** [Linear elasticity](#linear-elasticity)

The [bulk modulus](#bulk-modulus) relates hydrostatic compressive pressure to fractional volume compression. In [isotropic](#isotropy) three-dimensional [linear elasticity](#linear-elasticity), the spherical part of the [stress tensor](#cauchy-stress-tensor) is $\kappa\operatorname{tr}(\varepsilon)I$, so uniform dilation has [strain energy density](#strain-energy-density) $\kappa(\operatorname{tr}\varepsilon)^2/2$. Positive [bulk modulus](#bulk-modulus) and positive [shear modulus](#shear-modulus) make the isotropic [elastic stiffness tensor](#elastic-stiffness-tensor) positive on nonzero symmetric [strains](#strain).

#### Antiplane shear

↑ **Parent:** [Linear elasticity](#linear-elasticity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Antiplane_shear)

Antiplane shear has displacement normal to a plane and independent of that normal coordinate. In an isotropic linear elastic body, $\sigma_{13}=\mu w_{,1}$ and $\sigma_{23}=\mu w_{,2}$, together with their symmetric partners, are the only nonzero [stress tensor](#cauchy-stress-tensor) entries. Static balance without [body force](fluid-mechanics.md#body-force) reduces to the [Laplace equation](partial-differential-equation.md#laplace-equation) for $w$.

##### Steadily moving antiplane shear

↑ **Parent:** [Antiplane shear](#antiplane-shear)

For subsonic motion $|V|<c$, an [antiplane shear](#antiplane-shear) [displacement](classical-mechanics.md#displacement) $w(x_1-Vt,x_2)$ satisfies $\beta^2w_{xx}+w_{x_2x_2}=0$. The displayed rescaling makes it a [harmonic function](partial-differential-equation.md#harmonic-function) of $(x,y)$, so locally $w=\operatorname{Re}H(x+iy)$ for a [holomorphic function](complex-analysis.md#holomorphic-function) $H$. Set $F=\beta H$. The [Cauchy-Riemann equations](analysis.md#cauchy-riemann-equations) then give $\mu F'=\beta\sigma_{13}-i\sigma_{23}$. Keeping this potential normalization explicit avoids losing a factor of $\beta$ in the dynamic [stress](#stress) field. At sonic or supersonic speeds the elliptic harmonic reduction does not apply.

##### Complex stress potential for antiplane shear

↑ **Parent:** [Antiplane shear](#antiplane-shear)

A [harmonic conjugate](partial-differential-equation.md#harmonic-conjugate) $\phi$ satisfying $\phi_{,1}=w_{,2}$ and $\phi_{,2}=-w_{,1}$ makes $F=\phi+iw$ a [holomorphic function](complex-analysis.md#holomorphic-function). Its derivative packages the two [antiplane shear](#antiplane-shear) stresses into the displayed complex field. On multiply connected domains a global potential additionally requires the appropriate periods to vanish; prescribed displacement jumps can instead be represented by branches of the potential.

###### Hilbert problem for an antiplane crack

↑ **Parent:** [Complex stress potential for antiplane shear](#complex-stress-potential-for-antiplane-shear)

For a crack on the real axis under applied shear traction $p$, write $G=\mu F'$ for the additional [complex stress potential for antiplane shear](#complex-stress-potential-for-antiplane-shear) derivative. Reflection of the induced displacement gives $G^- =\overline{G^+}$. Traction-free crack faces therefore require $G^++G^-=-2p$; intact portions have $G^+=G^-$. This is a scalar [Riemann-Hilbert problem](differential-equation.md#riemann-hilbert-problem). Endpoint regularity, single-valued displacement and the absence of additional remote loads fix its homogeneous terms.

###### Cauchy solution for a steadily moving semi-infinite antiplane crack

↑ **Parent:** [Hilbert problem for an antiplane crack](#hilbert-problem-for-an-antiplane-crack)

For the moving semi-infinite crack, take the [branch cut](analysis.md#branch-cut) of $\sqrt z$ on the negative real axis and $\sqrt x>0$ ahead of the tip. With [steadily moving antiplane shear](#steadily-moving-antiplane-shear), face [tractions](#traction) $\sigma_{23}^{\pm}=-f(x)$ imply $\operatorname{Im}F'^{\pm}=f/\mu$. The antisymmetric [displacement](classical-mechanics.md#displacement) response gives $F'^-=-\overline{F'^+}$. Hence $G=\sqrt zF'$ has jump $G^+-G^-=-2\sqrt{-x}f(x)/\mu$. The [Sokhotski–Plemelj theorem](complex-analysis.md#sokhotski-plemelj-theorem) gives the displayed [Cauchy integral](complex-analysis.md#cauchy-transform), assuming convergence and no extra remote homogeneous loading. For $x>0$ it is purely imaginary, so $\sigma_{23}=\int_{-\infty}^0\sqrt{-s}f(s)/(x-s)\,ds/(\pi\sqrt x)$. At fixed co-moving loading this ahead-of-tip [stress](#stress) is independent of speed; the [displacement](classical-mechanics.md#displacement) still has the factor $1/\beta$.

###### Homogeneous stress-intensity field of a semi-infinite antiplane crack

↑ **Parent:** [Cauchy solution for a steadily moving semi-infinite antiplane crack](#cauchy-solution-for-a-steadily-moving-semi-infinite-antiplane-crack)

For real $C$, this analytic homogeneous field has real boundary values on both faces of the negative-axis crack, so it adds no face shear [traction](#traction). Ahead of the tip it adds [stress](#stress) $-\mu C/\sqrt x$. Its [stress](#stress) tends to zero at infinity, but its primitive grows like $\sqrt z$, producing unbounded remote [displacement](classical-mechanics.md#displacement) and infinite total [elastic energy](#elastic-energy). Thus merely requiring vanishing far [stress](#stress) does not uniquely fix the face-loaded crack solution. Excluding an added remote stress-intensity field, for example through the localized-load bounded-displacement far condition, removes this homogeneous ambiguity. Ordinary inverse-square-root tip [stress](#stress) remains allowed and has finite energy in any bounded neighbourhood of the tip.

###### Antiplane ligament Cauchy solution

↑ **Parent:** [Hilbert problem for an antiplane crack](#hilbert-problem-for-an-antiplane-crack)

For two semi-infinite cracks separated by a ligament, choose $\chi(z)=\sqrt{a^2-z^2}>0$ on the ligament. Its upper crack values are $-i\sqrt{t^2-a^2}$ on the right and $+i\sqrt{t^2-a^2}$ on the left. Multiplication by $\chi$ converts the [Hilbert problem for an antiplane crack](#hilbert-problem-for-an-antiplane-crack) to an additive jump; the [Sokhotski–Plemelj theorem](complex-analysis.md#sokhotski-plemelj-theorem) gives the displayed solution, assuming convergence. A homogeneous term $C/\chi$ transfers an extra resultant $\pi C$ through the ligament and has logarithmic displacement at infinity. The usual correction with no additional remote resultant excludes it. The far-field normalization is essential to uniqueness.

###### Finite antiplane crack Cauchy solution

↑ **Parent:** [Hilbert problem for an antiplane crack](#hilbert-problem-for-an-antiplane-crack)

Choose $\chi(z)=\sqrt{z^2-a^2}\sim z$ at infinity, cut on the finite crack. Its upper crack value is $i\sqrt{a^2-t^2}$, so $H=\chi G$ has jump $-2i\sqrt{a^2-t^2}p(t)$. The [Sokhotski–Plemelj theorem](complex-analysis.md#sokhotski-plemelj-theorem) gives the displayed [Cauchy integral](complex-analysis.md#cauchy-transform) solution. It decays as $z^{-2}$ for integrable weighted traction. A possible homogeneous term $C/\chi$ would give a logarithmic displacement period; it is removed for a dislocation-free finite crack with no extra remote loading.

#### Elastic stiffness tensor

↑ **Parent:** [Linear elasticity](#linear-elasticity)

An [elastic stiffness tensor](#elastic-stiffness-tensor) maps a small [displacement gradient tensor](#displacement-gradient-tensor) to the [stress tensor](#cauchy-stress-tensor). Minor symmetries in each index pair ensure symmetric [stress](#stress) and dependence only on symmetric [strain](#strain); major symmetry $c_{ijpq}=c_{pqij}$ follows from an [elastic energy](#elastic-energy) and underlies reciprocity. Stability requires positive [elastic energy](#elastic-energy) on nonzero strains. In an isotropic material, $c_{ijpq}=\lambda\delta_{ij}\delta_{pq}+\mu(\delta_{ip}\delta_{jq}+\delta_{iq}\delta_{jp})$, with [Lamé parameters](#lame-parameter) $\lambda,\mu$.

##### Independent elastic stiffness counts

↑ **Parent:** [Elastic stiffness tensor](#elastic-stiffness-tensor)

The two minor symmetries of the [elastic stiffness tensor](#elastic-stiffness-tensor) make it a map between six-dimensional spaces of symmetric [strain](#strain) and [stress](#stress). An [elastic energy](#elastic-energy) gives major symmetry, so the matrix of this map is symmetric and has 21 independent entries. For a symmetry operation acting on strains with parity spaces of dimensions $m$ and $6-m$, invariance eliminates the mixed block and leaves $m(m+1)/2+(6-m)(7-m)/2$ independent coefficients.

###### Twofold elastic symmetry

↑ **Parent:** [Independent elastic stiffness counts](#independent-elastic-stiffness-counts)

A rotation through $\pi$ about the third coordinate axis preserves the [strain](#strain) components $e_{11},e_{22},e_{33},e_{12}$ and reverses $e_{13},e_{23}$. A symmetry-invariant [elastic stiffness tensor](#elastic-stiffness-tensor) cannot couple the two parity spaces. Its independent symmetric blocks therefore contain $4\cdot5/2+2\cdot3/2=13$ coefficients. A twofold axis alone does not impose invariance under every rotation about that axis.

#### Bending moment

↑ **Parent:** [Linear elasticity](#linear-elasticity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bending_moment)

A bending moment is an internal [torque](classical-mechanics.md#torque) transmitted across a cut through a beam or [elastic plate](#elastic-plate). For a slender linear elastic beam, $M=EI\kappa$ up to sign convention, where $E$ is [Young's modulus](#young-s-modulus), $I$ the [second moment of area](#second-moment-of-area), and $\kappa$ the centreline [curvature](differential-geometry.md#curvature). The corresponding bending response of an [elastic plate](#elastic-plate) is described by its [bending stiffness](#bending-stiffness) and curvature tensor.

#### Elastic membrane

↑ **Parent:** [Linear elasticity](#linear-elasticity)

An elastic membrane is a thin deformable sheet whose transverse restoring force is supplied by in-plane tension. For uniform tension $T$ and mass per area $m$, a two-dimensional small-displacement model has $m\eta_{tt}=T\eta_{xx}-[p]$, where the pressure jump is defined from the lower fluid to the upper fluid. Fluid loading modifies its traveling modes through the [acoustic wave on a tensioned massive membrane](linear-acoustics.md#acoustic-wave-on-a-tensioned-massive-membrane).

#### Euler-Bernoulli beam equation

↑ **Parent:** [Linear elasticity](#linear-elasticity)

The Euler-Bernoulli beam equation models transverse linear bending waves in a slender beam. The normalized equation has $c_b=1$ and may be reduced by the [Schrodinger factorization of the elastic beam equation](#schrodinger-factorization-of-the-elastic-beam-equation). Prescribing displacement and curvature at an endpoint supplies two boundary traces for its fourth spatial derivative.

##### Schrodinger factorization of the elastic beam equation

↑ **Parent:** [Euler-Bernoulli beam equation](#euler-bernoulli-beam-equation)

Writing $q=u+iv$ in the [free Schrodinger equation](physics.md#free-schrodinger-equation) gives $u_t=-v_{xx}$ and $v_t=u_{xx}$, hence $u_{tt}+u_{xxxx}=0$. To encode initial velocity $u_1$, choose the decaying primitive $v_0(x)=-\int_x^\infty(s-x)u_1(s)ds$. A prescribed endpoint curvature becomes the time derivative of the imaginary boundary trace. This turns the normalized [Euler-Bernoulli beam equation](#euler-bernoulli-beam-equation) into a complex second-order boundary problem.

#### Second moment of area

↑ **Parent:** [Linear elasticity](#linear-elasticity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Second_moment_of_area)

The second moment of area of a cross-section about an axis is $I=\int y^2\,dA$, where $y$ is the perpendicular distance from that axis. Its dimensions are length to the fourth power. For a circular section of radius $a$, polar integration gives $I=\int_0^a r^3dr\int_0^{2\pi}\sin^2\theta d\theta=\pi a^4/4$. A slender rod with [Young's modulus](#young-s-modulus) $E$ has [filament bending modulus](mathematical-biology.md#filament-bending-modulus) $B=EI$: the axial [strain](#strain) caused by [curvature](differential-geometry.md#curvature) $\kappa$ is $-y\kappa$, and integrating the [linear elasticity](#linear-elasticity) energy density $E y^2\kappa^2/2$ over the section gives $B\kappa^2/2$ per unit length.

<h4 id="poisson-s-ratio">Poisson's ratio</h4>

↑ **Parent:** [Linear elasticity](#linear-elasticity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poisson's_ratio)

Poisson's ratio is minus the transverse strain divided by longitudinal strain under uniaxial loading in isotropic [linear elasticity](#linear-elasticity).

<h4 id="young-s-modulus">Young's modulus</h4>

↑ **Parent:** [Linear elasticity](#linear-elasticity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Young's_modulus)

Young's modulus is the ratio of axial [stress](#stress) to axial [strain](#strain) in uniaxial [linear elasticity](#linear-elasticity). For an isotropic plate, the bending rigidity is $E t^3/[12(1-\nu^2)]$, with thickness $t$ and [Poisson's ratio](#poisson-s-ratio) $\nu$.

#### Fracture toughness

↑ **Parent:** [Linear elasticity](#linear-elasticity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fracture_toughness)

Fracture toughness measures a material's resistance to crack advance. In a thin [elastic plate](#elastic-plate) model, the threshold for advance can be represented by a prescribed front [curvature](differential-geometry.md#curvature) $\kappa_f$. Such a curvature parameter is not numerically interchangeable with a bulk fracture-toughness parameter without specifying the fracture model.

<h4 id="hooke-s-law">Hooke's law</h4>

↑ **Parent:** [Linear elasticity](#linear-elasticity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hooke's_law)

Hooke's law states that the restoring force or stress is proportional to a sufficiently small displacement or strain. For a one-dimensional spring, $f=kx$ in magnitude.

##### Spring

↑ **Parent:** [Hooke's law](#hooke-s-law)

A linear [spring](#spring) stores elastic energy $kx^2/2$ when displaced by $x$ from its relaxed position. The external force maintaining that displacement is $kx$; its restoring force on the moving attachment has the opposite sign. Its stiffness $k$ has units force per length.

#### Elastic plate

↑ **Parent:** [Linear elasticity](#linear-elasticity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Elastic_plate)

An elastic plate is a thin elastic body whose leading deformation is bending of its middle surface.

##### Line-forced fluid-loaded bending plate

↑ **Parent:** [Elastic plate](#elastic-plate)

An [elastic plate](#elastic-plate) coupled to one compressible fluid half-space has an outgoing [Fourier transform](analysis.md#fourier-transform) kernel $D$, where $\gamma^2=k^2-\omega^2/c_0^2$. A harmonic line [force](classical-mechanics.md#force) $F_0$ produces displacement transform $F_0\gamma/D$. Propagating acoustic components have $\gamma=-i\sqrt{\omega^2/c_0^2-k^2}$, whereas guided components decay normally to the plate. The outgoing prescription separates [acoustic energy flux](#acoustic-energy-flux) from guided-wave energy transport.

##### Flexural wave

↑ **Parent:** [Elastic plate](#elastic-plate)

For a thin plate with areal mass $m$ and [bending stiffness](#bending-stiffness) $B$, small free transverse disturbances satisfy $m\eta_{tt}+B\nabla^4\eta=0$. A [plane wave](quantum-mechanics.md#plane-wave) of tangential [wavenumber](wave-equation.md#wavenumber) $k$ therefore satisfies

$$
\omega^2=(B/m)k^4.
$$

The frequency is quadratic in [wavenumber](wave-equation.md#wavenumber), so these waves are dispersive. Matching this free-wave relation cancels the plate's inertial and bending response in an acoustic transmission problem.

###### Flexural-gravity wave

↑ **Parent:** [Flexural wave](#flexural-wave)

A flexural-gravity wave bends a floating [elastic plate](#elastic-plate) while displacing the underlying water. For a uniform plate with areal mass $m$ and [bending stiffness](#bending-stiffness) $D$ above inviscid deep water of [mass density](fluid-mechanics.md#density) $\rho_w$, put $\alpha=m/\rho_w$ and $\beta=D/\rho_w$. Combining the plate equation with the water's [kinematic boundary condition](fluid-mechanics.md#kinematic-boundary-condition) gives the displayed [dispersion relation](wave-equation.md#dispersion-relation). Both [gravitational acceleration](classical-mechanics.md#gravitational-acceleration) and plate bending restore displacement; water and plate inertia resist acceleration. It assumes small amplitude, no prestress and negligible shear deformation of the plate.

###### Minimum phase speed of a flexural-gravity wave

↑ **Parent:** [Flexural-gravity wave](#flexural-gravity-wave)

Write $\beta=D/\rho_w$ and $\alpha=m/\rho_w$ in the [dispersion relation of a floating elastic plate](#dispersion-relation-of-a-floating-elastic-plate). A stationary point of squared [phase velocity](wave-equation.md#phase-velocity) satisfies $\beta k^4(3+2\alpha k)=g(1+2\alpha k)$. If plate inertia is neglected, its solution is $k=(g/(3\beta))^{1/4}$. A steadily translating load can resonate only when its speed matches a [phase velocity](wave-equation.md#phase-velocity); this threshold differs from the [group-velocity minimum of a flexural-gravity wave](#group-velocity-minimum-of-a-flexural-gravity-wave).

###### Dispersion relation of a floating elastic plate

↑ **Parent:** [Flexural-gravity wave](#flexural-gravity-wave)

For [bending stiffness](#bending-stiffness) $D$ and mass per area $m$, a [plane wave](quantum-mechanics.md#plane-wave) of surface displacement $\eta$ satisfies $m\eta_{tt}+D\nabla_H^4\eta=p$. An inviscid deep-water [velocity potential](fluid-mechanics.md#velocity-potential) has vertical dependence $e^{kz}$; the [kinematic boundary condition](fluid-mechanics.md#kinematic-boundary-condition) and linear [Bernoulli equation](fluid-mechanics.md#bernoulli-equation) give $p=(\rho_w\omega^2/k-\rho_wg)\eta$. Eliminating $p$ gives the displayed [dispersion relation](wave-equation.md#dispersion-relation). With water depth $d$, replace it by $\omega^2=(gk+Dk^5/\rho_w)\tanh(kd)/[1+(m/\rho_w)k\tanh(kd)]$.

###### Group-velocity minimum of a flexural-gravity wave

↑ **Parent:** [Flexural-gravity wave](#flexural-gravity-wave)

The [group velocity](wave-equation.md#group-velocity) of a [flexural-gravity wave](#flexural-gravity-wave) diverges on the long-wave gravity branch and on the short-wave bending branch, and therefore has a positive minimum between them when the [bending stiffness](#bending-stiffness) is positive. This minimum bounds the propagation speed of narrow [wave packets](wave-equation.md#wave-packet) within the ideal model. It does not by itself determine a wind-generation threshold: steady forcing requires matching [phase velocity](wave-equation.md#phase-velocity), while dissipation and coupling determine growth.

##### Viscous peeling of an elastic plate

↑ **Parent:** [Elastic plate](#elastic-plate)

A fluid advancing under an [elastic plate](#elastic-plate) can be resisted mainly by [lubrication theory](viscous-fluid-flow.md#lubrication-theory) flow near its front. For front gap $h_f$ and peeling length $l_p$, the elastic pressure gradient is of order $Bh_f/l_p^5$, while the gap [volume flux](fluid-mechanics.md#volumetric-flow-rate) is of order $Bh_f^4/(\mu l_p^5)$. Mass balance therefore gives peeling speed $U_p\sim Bh_f^3/(\mu l_p^5)$.

##### Axisymmetric clamped-plate deflection

↑ **Parent:** [Elastic plate](#elastic-plate)

A circular [elastic plate](#elastic-plate) with [bending stiffness](#bending-stiffness) $B$, constant excess pressure $p$ and [clamped boundary conditions](differential-equation.md#clamped-boundary-condition) at radius $R$ obeys $B\nabla_r^4h=p$, where $\nabla_r^2=r^{-1}\partial_r(r\partial_r)$. Its regular solution is $h=p(R^2-r^2)^2/(64B)$. Consequently its enclosed volume is $V=\pi pR^6/(192B)$, and its edge [curvature](differential-geometry.md#curvature) is $h_{rr}(R)=pR^2/(8B)=24V/(\pi R^4)$.

##### Bending stiffness

↑ **Parent:** [Elastic plate](#elastic-plate)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bending_stiffness)

Bending stiffness is the coefficient relating plate curvature to bending moment. In linear thin-plate theory a transverse displacement $\zeta$ produces a restoring load $B\nabla^4\zeta$.

#### Nondegenerate one-dimensional elastic material

↑ **Parent:** [Linear elasticity](#linear-elasticity)

For the one-dimensional reduction of isotropic [linear elasticity](#linear-elasticity), nondegeneracy means that the effective longitudinal modulus $\lambda+2\mu$ is nonzero. The static [Navier-Cauchy equation](#navier-cauchy-equation) then forces the displacement to be affine.

#### Displacement field (mechanics)

↑ **Parent:** [Linear elasticity](#linear-elasticity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Displacement_field_(mechanics))

A displacement field $\mathbf u(\mathbf x)$ gives the change in position of each material point from a reference configuration.

##### Lagrangian fluid displacement

↑ **Parent:** [Displacement field (mechanics)](#displacement-field-mechanics)

The Lagrangian fluid displacement $\boldsymbol\xi$ compares neighbouring fluid trajectories. Linear [velocity](classical-mechanics.md#velocity) [perturbations](analysis.md#perturbation) about a steady flow $\mathbf U$ obey $\delta\mathbf u=(\partial_t+\mathbf U\cdot\nabla)\boldsymbol\xi-(\boldsymbol\xi\cdot\nabla)\mathbf U$. For a background scalar $f_0$, its material [perturbation](analysis.md#perturbation) is $\Delta f=\delta f+\boldsymbol\xi\cdot\nabla f_0$. In an axisymmetric [normal mode](wave-equation.md#normal-mode) about cylindrical rotation, the radial and vertical [velocities](classical-mechanics.md#velocity) are $-i\omega\xi_r$ and $-i\omega\xi_z$. The displacement of a [free surface](fluid-mechanics.md#free-surface) is needed to impose the [Lagrangian pressure perturbation](fluid-mechanics.md#lagrangian-pressure-perturbation) condition.

// Target: astrophysics.bigb

##### Displacement gradient tensor

↑ **Parent:** [Displacement field (mechanics)](#displacement-field-mechanics)

The displacement gradient has components $(\nabla\mathbf u)_{ij}=\partial_i u_j$ and records local changes of the displacement field.

This tensor is a local derivative of the [displacement field](#displacement-field-mechanics); it enters the deformation gradient and strain measures.

<h4 id="lame-parameter">Lamé parameter</h4>

↑ **Parent:** [Linear elasticity](#linear-elasticity)

The two Lamé parameters $\lambda$ and $\mu$ determine the linear isotropic relation between stress and strain; $\mu$ is the shear modulus.

##### Poisson solid

↑ **Parent:** [Lamé parameter](#lame-parameter)

An isotropic [linear elasticity](#linear-elasticity) material with equal positive [Lamé parameters](#lame-parameter) has [Poisson's ratio](#poisson-s-ratio) $1/4$ and the displayed compressional/shear speed ratio. This simplifying model fixes the relative amplitudes in the [tensile-crack radiation pattern](wave-equation.md#tensile-crack-radiation-pattern); it does not describe every stable isotropic solid.

#### Isotropic linear-elastic energy density

↑ **Parent:** [Linear elasticity](#linear-elasticity)

For the two-dimensional convention $\nabla\mathbf u=(\partial_i u_j)$, the energy density

$$
W=\frac\mu2\nabla\mathbf u:\nabla\mathbf u^T
+\frac{\lambda+\mu}{2}(\nabla\cdot\mathbf u)^2
$$

produces the static isotropic elastic equations by variation.

#### Navier-Cauchy equation

↑ **Parent:** [Linear elasticity](#linear-elasticity)

In a homogeneous isotropic elastic body without body forces, static equilibrium of the displacement field is

$$
\mu\nabla^2\mathbf u
+(\lambda+\mu)\nabla(\nabla\cdot\mathbf u)=0.
$$

This is the static, homogeneous-isotropic displacement form of [linear elasticity](#linear-elasticity).

##### Uniform extension of a one-dimensional elastic body

↑ **Parent:** [Navier-Cauchy equation](#navier-cauchy-equation)

For a one-dimensional body with endpoints displaced by zero and $\Delta$, the static Navier-Cauchy equation reduces to $u''=0$ and gives the uniform strain solution $u(x)=\Delta x/L$.

#### Elastic wave in an isotropic solid

↑ **Parent:** [Linear elasticity](#linear-elasticity)

For density $\rho$ and [Lamé parameters](#lame-parameter) $\lambda,\mu$, the displacement satisfies

$$
\rho\mathbf u_{tt}
=(\lambda+\mu)\nabla(\nabla\cdot\mathbf u)+\mu\nabla^2\mathbf u.
$$

Its longitudinal and transverse wave speeds are

$$
c_P=\sqrt{\frac{\lambda+2\mu}{\rho}},
\qquad
c_S=\sqrt{\frac{\mu}{\rho}}.
$$

##### Shear-horizontal wave

↑ **Parent:** [Elastic wave in an isotropic solid](#elastic-wave-in-an-isotropic-solid)

A shear-horizontal wave propagating in the $x$ direction has displacement perpendicular to the sagittal $xy$ plane, for example $\mathbf u=w(x,y,t)\mathbf e_z$. It is divergence-free and obeys the scalar shear-wave equation $w_{tt}=c_S^2(w_{xx}+w_{yy})$.

###### SH input impedance

↑ **Parent:** [Shear-horizontal wave](#shear-horizontal-wave)

The [SH input impedance](#sh-input-impedance) is the negative ratio of vertical [traction](#traction) to particle [velocity](classical-mechanics.md#velocity) for a [shear-horizontal wave](#shear-horizontal-wave) field, with positive depth and tension-positive [traction](#traction). A superposition of upward and downward waves generally has a depth-dependent complex ratio. A downward progressive wave in a uniform medium has $Z=\mu p_\beta$, while the upward wave has $Z=-\mu p_\beta$. The input ratio includes reflection from deeper structure and can have poles at [velocity](classical-mechanics.md#velocity) nodes.

###### SH impedance Riccati equation

↑ **Parent:** [SH input impedance](#sh-input-impedance)

With $e^{ikx-i\omega t}$ phasors, positive depth $z$, [shear modulus](#shear-modulus) $\mu=\rho\beta^2$, vertical [traction](#traction) $T$ and particle [velocity](classical-mechanics.md#velocity) $V$, the shear-wave equations give $V'=-i\omega T/\mu$ and $T'=-i\omega\mu p_\beta^2V$, where $p_\beta^2=\beta^{-2}-k^2/\omega^2$. Define $Z=-T/V$ wherever $V\ne0$. Differentiation gives the displayed [Riccati equation](analysis.md#riccati-equation) and $V'=i\omega ZV/\mu$. A pole of $Z$ can be an ordinary zero of $V$, not a singular physical wavefield.

###### Uniform-layer SH impedance update

↑ **Parent:** [SH impedance Riccati equation](#sh-impedance-riccati-equation)

In a uniform layer, put $q=\mu p_\beta$, $\kappa=\omega p_\beta$ and $d=z-z_r$. Initial impedance $Z_r$ gives the displayed fractional-linear solution and $V(z)=V_r[\cos\kappa d+i(Z_r/q)\sin\kappa d]$. Expanding into exponentials yields forward and backward [shear-horizontal waves](#shear-horizontal-wave). Negative $d$ propagates a bottom load upward. If the denominator vanishes, the nonsingular pair $(V,T)$ must be propagated through the impedance pole.

###### Reflection from a layered SH impedance

↑ **Parent:** [Uniform-layer SH impedance update](#uniform-layer-sh-impedance-update)

Set the lower [half-space](geometry-and-topology.md#half-space) load to $q_b=\mu_bp_{\beta,b}$ using the [causal vertical wavenumber branch](#causal-vertical-wavenumber-branch), which excludes a wave arriving from depth infinity. Apply the [uniform-layer SH impedance update](#uniform-layer-sh-impedance-update) upwards through every layer, keeping particle [velocity](classical-mechanics.md#velocity) and [traction](#traction) continuous. For upper [half-space](geometry-and-topology.md#half-space) impedance $q_a$, incident [velocity](classical-mechanics.md#velocity) $V_0$ and reflected [velocity](classical-mechanics.md#velocity) $RV_0$, the top values are $V=V_0(1+R)$ and $T=-q_aV_0(1-R)$. Their ratio gives the displayed [reflection coefficient](partial-differential-equation.md#reflection-coefficient), incorporating every underlying interface and multiple reflection.

###### Complex-frequency SH flux monotonicity

↑ **Parent:** [SH impedance Riccati equation](#sh-impedance-riccati-equation)

For positive real [mass density](fluid-mechanics.md#density) and [shear modulus](#shear-modulus), real $k$ and $\operatorname{Im}\omega>0$, the displayed [derivative](calculus.md#derivative) of $S_z=-\tfrac12\operatorname{Re}(V^*T)$ follows from the two first-order shear equations. Every nontrivial solution has strictly decreasing $S_z$. Since $S_z=\tfrac12\operatorname{Re}Z|V|^2$, positive-real impedance at a deeper point remains positive at all shallower points; negative-real impedance at a shallower point remains negative deeper down. A zero field is the necessary exception to strictness. At complex [frequency](physics.md#frequency) this is a spectral flux diagnostic, reducing to a physical cycle average on the real axis.

###### Causal vertical wavenumber branch

↑ **Parent:** [Shear-horizontal wave](#shear-horizontal-wave)

For real horizontal [wavenumber](wave-equation.md#wavenumber) $k$, positive real [wave speed](wave-equation.md#wave-speed) $\beta$ and $\omega=u+iv$ with $v>0$, write $k_\beta=a+ib$ with $k_\beta^2=\omega^2/\beta^2-k^2$. Its imaginary part gives $ab=uv/\beta^2$. The number $b$ cannot vanish, and $\operatorname{Re}(k_\beta/\omega)=v[b+u^2/(\beta^2b)]/|\omega|^2$ has the sign of $b$. The branch $b>0$ makes $e^{ik_\beta z}$ decay towards increasing depth and analytically continues the outgoing propagating or evanescent branch to the upper [frequency](physics.md#frequency) half-plane.

###### Guided shear-horizontal mode

↑ **Parent:** [Shear-horizontal wave](#shear-horizontal-wave)

Between parallel boundaries, a guided shear-horizontal mode has a discrete transverse wavenumber $q_n$ and dispersion relation $\omega_n^2=c_S^2(k^2+q_n^2)$. Its cutoff frequency is $c_Sq_n$.

##### Mode conversion at a planar elastic interface

↑ **Parent:** [Elastic wave in an isotropic solid](#elastic-wave-in-an-isotropic-solid)

An obliquely incident in-plane P- or SV-wave generally produces reflected and transmitted P- and SV-waves. Continuity of displacement and traction supplies four scalar conditions for their four amplitudes, while frequency and tangential wavenumber are shared.

###### Solid-fluid P-wave transmission coefficient

↑ **Parent:** [Mode conversion at a planar elastic interface](#mode-conversion-at-a-planar-elastic-interface)

For incidence from a solid with compressional/shear speeds $\alpha,\beta$ into a fluid of sound speed $\alpha_f$, let $E=\cos^22\theta_S+(\beta^2/\alpha^2)\sin2\theta_P\sin2\theta_S$. The displayed coefficient multiplies the transmitted [displacement field](#displacement-field-mechanics) potential relative to the incident [P wave](wave-equation.md#p-wave) potential, using the same retarded-time waveform. [Snell law for elastic and acoustic waves](#snell-law-for-elastic-and-acoustic-waves) matches the tangential slowness. Continuity of normal [displacement field](#displacement-field-mechanics), zero tangential [traction](#traction), and continuity of normal [traction](#traction) give the coefficient. It is not a displacement-amplitude coefficient: longitudinal [displacement field](#displacement-field-mechanics) acquires an additional ratio $\alpha/\alpha_f$.

###### Snell law for elastic and acoustic waves

↑ **Parent:** [Mode conversion at a planar elastic interface](#mode-conversion-at-a-planar-elastic-interface)

Phase matching at a planar interface preserves frequency and tangential wavenumber. Thus waves of speeds $c_j$ and angles $\theta_j$ from the normal satisfy

$$
\frac{\sin\theta_j}{c_j}=\text{constant}.
$$

##### Acoustic impedance

↑ **Parent:** [Elastic wave in an isotropic solid](#elastic-wave-in-an-isotropic-solid)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Acoustic_impedance)

The acoustic impedance of a fluid is $Z=\rho c$. For a progressive plane acoustic wave, pressure amplitude $P$ and velocity amplitude $U$ in its propagation direction satisfy $P=ZU$. At an oblique planar interface, zero reflection requires a matching condition involving the normal impedances $Z/\cos\theta$ or, equivalently for displacement amplitudes, $Z\cos\theta$.

###### Normal acoustic impedance

↑ **Parent:** [Acoustic impedance](#acoustic-impedance)

The normal acoustic impedance of a progressive [acoustic wave](fluid-mechanics.md#acoustic-wave) at a planar boundary is the pressure amplitude divided by the normal-velocity amplitude. For propagation angle $\theta$ from the normal,

$$
Z_n=\frac{\rho c}{\cos\theta}=\frac{\rho\omega}{k_n}.
$$

The distinction from the [acoustic impedance](#acoustic-impedance) $\rho c$ matters at oblique incidence: interface reflection depends on the ratio of normal impedances. For an evanescent outgoing wave $k_n$ is imaginary and the normal impedance is reactive, giving no mean normal [acoustic energy flux](#acoustic-energy-flux).

###### Surface acoustic impedance

↑ **Parent:** [Normal acoustic impedance](#normal-acoustic-impedance)

At an acoustic boundary, the [surface acoustic impedance](#surface-acoustic-impedance) is the [pressure](thermodynamics.md#pressure) amplitude divided by the [velocity](classical-mechanics.md#velocity) amplitude directed into that boundary. With upward surface [velocity](classical-mechanics.md#velocity) $-V$ and harmonic convention $e^{i\omega t}$, it is $Z=P/V$. Reflection compares this impedance with the incident fluid's [normal acoustic impedance](#normal-acoustic-impedance). The [velocity](classical-mechanics.md#velocity) orientation and harmonic convention must be fixed before interpreting signs of inertial, elastic, and radiation terms.

###### Passive acoustic impedance

↑ **Parent:** [Surface acoustic impedance](#surface-acoustic-impedance)

With [pressure](thermodynamics.md#pressure) amplitude $P=ZV$ and [velocity](classical-mechanics.md#velocity) $V$ directed into a boundary, the mean absorbed [acoustic energy flux](#acoustic-energy-flux) is $\tfrac12\operatorname{Re}(PV^*)=\tfrac12\operatorname{Re}Z|V|^2$. A passive boundary cannot supply net energy, so $\operatorname{Re}Z\geq0$ at a real frequency. Its reflection from a propagating [acoustic plane wave](physics.md#acoustic-plane-wave) has magnitude at most one. A pole continued to a complex incidence angle or frequency must be interpreted separately from real-frequency passive scattering.

###### Acoustic transmission through a uniform layer

↑ **Parent:** [Acoustic impedance](#acoustic-impedance)

A layer of impedance $Z_1$, wavenumber $k_1$, and thickness $L$ between identical media of impedance $Z_0$ has pressure-amplitude transmission coefficient

$$
|T|=\left[\cos^2(k_1L)+\frac14\left(\frac{Z_1}{Z_0}+\frac{Z_0}{Z_1}\right)^2\sin^2(k_1L)\right]^{-1/2}.
$$

It transmits perfectly at the layer resonances $k_1L=n\pi$, irrespective of the impedance mismatch.

###### Coherent acoustic layer above a rough reflector

↑ **Parent:** [Acoustic transmission through a uniform layer](#acoustic-transmission-through-a-uniform-layer)

In a coherent specular model, let $r_b$ be the effective lower pressure reflection coefficient referenced to $z=0$, and let the planar upper interface lie at $z=d$. With layer and upper normal impedances $Z_1,Z_2$, $r_{12}=(Z_2-Z_1)/(Z_2+Z_1)$ and $t_{21}=2Z_1/(Z_1+Z_2)$. Summing repeated round trips gives the displayed downward amplitude at the upper interface. The mean layer field is $De^{i\alpha x}[e^{-i\beta(z-d)}+r_be^{2i\beta d}e^{i\beta(z-d)}]$. Feedback through diffuse roughness channels must be neglected in this scalar model or included in a context-dependent effective reflection coefficient.

###### Displacement reflection from an interface between two inviscid elastic liquids

↑ **Parent:** [Acoustic impedance](#acoustic-impedance)

For a P-wave incident at angle $\theta$ from a liquid $(\rho,c,\lambda)$ onto $(\rho',c',\lambda')$, with transmitted angle $\theta'$ obeying [Snell law for elastic and acoustic waves](#snell-law-for-elastic-and-acoustic-waves),

$$
R=\frac{\lambda'\sin2\theta-\lambda\sin2\theta'}
{\lambda'\sin2\theta+\lambda\sin2\theta'}.
$$

No reflection is equivalent to $\rho'c'\cos\theta=\rho c\cos\theta'$.

### Elastic-wave energy flux

↑ **Parent:** [Elasticity (physics)](#elasticity-physics)

For displacement velocity $\dot u$ and stress $\sigma$, the instantaneous elastic-energy flux is

$$
P_i=-\sigma_{ij}\dot u_j.
$$

For complex harmonic amplitudes, its average over one temporal period is

$$
\langle P_i\rangle=-\frac12\operatorname{Re}(\widehat\sigma_{ij}\widehat{\dot u}_j^*).
$$

#### P-SV directional impedance matrix

↑ **Parent:** [Elastic-wave energy flux](#elastic-wave-energy-flux)

For real [frequency](physics.md#frequency) $\omega>0$ and both vertical wavenumbers $p=k_\alpha>0$, $s=k_\beta>0$, let $D=k^2+ps$, $A=\rho\omega p/D$, $B=\rho\omega s/D$, and $C=k(2\mu D-\rho\omega^2)/(\omega D)$. With [traction](#traction) $\mathbf t=(\sigma_{xz},\sigma_{zz})$ and particle [velocity](classical-mechanics.md#velocity) $\mathbf v=(v_x,v_z)$, each directional [P wave](wave-equation.md#p-wave)/[SV-wave](wave-equation.md#sv-wave) field obeys $\mathbf t=-Z_\pm\mathbf v$. Direct displacement-potential substitution yields $Z_-=-Z_+^\dagger$. The [Hermitian part](hilbert-space.md#hermitian-part-of-a-matrix) of $Z_+$ is positive diagonal; thus forward/backward fluxes have opposite signs and mixed directional flux cross terms cancel.

##### P-SV characteristic reconstruction

↑ **Parent:** [P-SV directional impedance matrix](#p-sv-directional-impedance-matrix)

For a mixture of forward and backward [elastic waves](wave-equation.md#elastic-wave), $\mathbf v=\mathbf v^++\mathbf v^-$ and $\mathbf t=-Z_+\mathbf v^+-Z_-\mathbf v^-$. The diagonal inverse displayed above gives $\mathbf v^+=-(Z_+-Z_-)^{-1}(\mathbf t+Z_-\mathbf v)$ and $\mathbf v^-=(Z_+-Z_-)^{-1}(\mathbf t+Z_+\mathbf v)$. It is well-defined when both modes propagate strictly away from grazing. At a vanishing vertical [wavenumber](wave-equation.md#wavenumber) its singularity signals a failure of this strict directional split.

#### Reflection of an SV-wave from a rigid plane

↑ **Parent:** [Elastic-wave energy flux](#elastic-wave-energy-flux)

An incident SV-wave generally reflects as both an SV-wave and a P-wave. A rigid boundary determines their amplitudes by requiring both displacement components to vanish, while phase matching preserves frequency and tangential wavenumber.

##### Evanescent reflected P-wave at a rigid plane

↑ **Parent:** [Reflection of an SV-wave from a rigid plane](#reflection-of-an-sv-wave-from-a-rigid-plane)

For incident SV angle $\theta$, tangential phase matching gives $\sin\phi=(c_P/c_S)\sin\theta$ for the reflected P-wave. It is evanescent when $\sin\theta>c_S/c_P$.

###### Unit-modulus SV reflection with evanescent P conversion

↑ **Parent:** [Evanescent reflected P-wave at a rigid plane](#evanescent-reflected-p-wave-at-a-rigid-plane)

When the converted P-wave is evanescent, its amplitude decays away from the boundary and the reflected SV amplitude has modulus one. The P field stores reactive energy near the boundary but carries zero mean normal power.

##### Rigid boundary condition for an elastic wave

↑ **Parent:** [Reflection of an SV-wave from a rigid plane](#reflection-of-an-sv-wave-from-a-rigid-plane)

At a perfectly rigid plane, every component of the displacement field vanishes.

#### Wavevector

↑ **Parent:** [Elastic-wave energy flux](#elastic-wave-energy-flux)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wavevector)

A wavevector points in the direction of phase propagation; its magnitude is the wavenumber and its scalar product with position gives the spatial phase.

##### Hamiltonian ray-tracing equations

↑ **Parent:** [Wavevector](#wavevector)

For a slowly varying local dispersion relation $\omega=\Omega(\mathbf k;\mathbf x,t)$, wave-packet rays obey

$$
\dot x_i=\frac{\partial\Omega}{\partial k_i},
\qquad
\dot k_i=-\frac{\partial\Omega}{\partial x_i},
\qquad
\dot\omega=\frac{\partial\Omega}{\partial t}.
$$

###### WKB method

↑ **Parent:** [Hamiltonian ray-tracing equations](#hamiltonian-ray-tracing-equations)

The WKB method seeks a rapidly oscillating field in the form

$$
\phi(x,t)=A(x,t;\varepsilon)e^{i\theta(x,t)/\varepsilon},
\qquad 0<\varepsilon\ll1,
$$

and determines the phase and slowly varying amplitude order by order in $\varepsilon$.

###### Eikonal equation

↑ **Parent:** [WKB method](#wkb-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Eikonal_equation)

The leading WKB phase obeys an eikonal equation. For a local dispersion relation $\omega=\Omega(k;x,t)$ and $k=\nabla\theta$, it is

$$
-\partial_t\theta=\Omega(\nabla\theta;x,t).
$$

###### Total derivative along a ray

↑ **Parent:** [Hamiltonian ray-tracing equations](#hamiltonian-ray-tracing-equations)

Along a ray $\mathbf x(t)$, the derivative of a field $f(\mathbf x,t)$ is

$$
\frac{df}{dt}
=\frac{\partial f}{\partial t}
+\dot{\mathbf x}\cdot\nabla f.
$$

#### Evanescent wave

↑ **Parent:** [Elastic-wave energy flux](#elastic-wave-energy-flux)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Evanescent_wave)

An evanescent wave has an imaginary component of its wavevector and therefore decays exponentially in that direction instead of transporting energy away as a propagating wave.

## Cauchy momentum equation

↑ **Parent:** [Continuum mechanics](continuum-mechanics.md)

The Cauchy momentum equation balances material acceleration against stress divergence and body force:

$$
\rho\frac{D\mathbf u}{Dt}=\nabla\mathbin\cdot\boldsymbol\sigma+\rho\mathbf b.
$$

For an inertialess flow, the left-hand side is neglected.

## Falkner-Skan boundary layer

↑ **Parent:** [Continuum mechanics](continuum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Falkner–Skan_boundary_layer)

A Falkner-Skan boundary layer is a similarity boundary-layer flow driven by an outer velocity proportional to a power of distance along the wall. Its streamfunction reduction gives the [Falkner-Skan equation](#falkner-skan-equation), with no-slip wall and outer-velocity matching conditions. It generalizes the Blasius flat-plate boundary layer.

## Sound intensity

↑ **Parent:** [Continuum mechanics](continuum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sound_intensity)

Sound intensity is acoustic power per unit area, represented by the time-averaged energy-flux vector $\mathbf I=\langle p\mathbf u\rangle$. Its direction gives the net direction of acoustic energy transport.

## ↑ Ancestors (3)

1. [Branches of physics](physics.md#branches-of-physics)
2. [Physics](physics.md)
3. [Codex Wiki](README.md)
