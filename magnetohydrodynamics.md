# Magnetohydrodynamics

↑ **Parent:** [Astrophysical fluid dynamics](astrophysical-fluid-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Magnetohydrodynamics)

Magnetohydrodynamics treats an electrically conducting fluid coupled to a magnetic field through the Lorentz force and electromagnetic induction.

**Table of contents**

- [Magnetic flux concentration](#magnetic-flux-concentration)
  - [Equipartition magnetic field](#equipartition-magnetic-field)
  - [Convective collapse](#convective-collapse)
- [Magnetostrophic balance](#magnetostrophic-balance)
  - [Taylor constraint](#taylor-constraint)
    - [Viscous regularization of the Taylor constraint](#viscous-regularization-of-the-taylor-constraint)
    - [Geostrophic flow preserving the Taylor constraint](#geostrophic-flow-preserving-the-taylor-constraint)
    - [Magnetostrophic Taylor state](#magnetostrophic-taylor-state)
- [Mean-field electrodynamics](#mean-field-electrodynamics)
- [Kinematic magnetic dynamo](#kinematic-magnetic-dynamo)
  - [Gaussian white-noise magnetic stretching](#gaussian-white-noise-magnetic-stretching)
    - [Lognormal magnetic-field amplification](#lognormal-magnetic-field-amplification)
    - [Magnetic stretching moment growth](#magnetic-stretching-moment-growth)
    - [Radial magnetic-field Fokker-Planck equation](#radial-magnetic-field-fokker-planck-equation)
- [Theta pinch](#theta-pinch)
  - [Positive ideal energy of a theta pinch](#positive-ideal-energy-of-a-theta-pinch)
- [Hall magnetohydrodynamics](#hall-magnetohydrodynamics)
  - [Fast-time electron-MHD limit of Hall magnetohydrodynamics](#fast-time-electron-mhd-limit-of-hall-magnetohydrodynamics)
  - [Incompressible Hall-MHD wave dispersion](#incompressible-hall-mhd-wave-dispersion)
- [Electron magnetohydrodynamics](#electron-magnetohydrodynamics)
  - [Whistler wave](#whistler-wave)
  - [Reduced electron magnetohydrodynamics](#reduced-electron-magnetohydrodynamics)
- [Stratified magneto-Coriolis wave](#stratified-magneto-coriolis-wave)
  - [Rapid-rotation slow magneto-Coriolis branch](#rapid-rotation-slow-magneto-coriolis-branch)
- [Lehnert number](#lehnert-number)
- [Magnetohydrodynamic momentum equation](#magnetohydrodynamic-momentum-equation)
- [Resistive magnetohydrodynamics](resistive-magnetohydrodynamics.md)
  - [Magnetic reconnection](resistive-magnetohydrodynamics.md#magnetic-reconnection)
  - [Magnetic skin layer](resistive-magnetohydrodynamics.md#magnetic-skin-layer)
    - [Magnetic skin-layer streaming slip](resistive-magnetohydrodynamics.md#magnetic-skin-layer-streaming-slip)
    - [Mean Lorentz force in a magnetic skin layer](resistive-magnetohydrodynamics.md#mean-lorentz-force-in-a-magnetic-skin-layer)
  - [Flux expulsion](resistive-magnetohydrodynamics.md#flux-expulsion)
    - [Phase mixing in magnetic flux expulsion](resistive-magnetohydrodynamics.md#phase-mixing-in-magnetic-flux-expulsion)
      - [Cubic-time resistive damping in a differentially rotating cell](resistive-magnetohydrodynamics.md#cubic-time-resistive-damping-in-a-differentially-rotating-cell)
  - [Dynamo action](resistive-magnetohydrodynamics.md#dynamo-action)
    - [Homopolar disc dynamo](resistive-magnetohydrodynamics.md#homopolar-disc-dynamo)
      - [Torque-controlled homopolar dynamo equilibrium](resistive-magnetohydrodynamics.md#torque-controlled-homopolar-dynamo-equilibrium)
    - [Radial-flow dynamo energy bound](resistive-magnetohydrodynamics.md#radial-flow-dynamo-energy-bound)
    - [Dynamo quenching](resistive-magnetohydrodynamics.md#dynamo-quenching)
      - [Algebraic alpha quenching](resistive-magnetohydrodynamics.md#algebraic-alpha-quenching)
        - [Alpha-quenching rotating wave](resistive-magnetohydrodynamics.md#alpha-quenching-rotating-wave)
          - [Unequal-hemisphere dynamo rotating wave](resistive-magnetohydrodynamics.md#unequal-hemisphere-dynamo-rotating-wave)
    - [Equivariant three-mode dynamo normal form](resistive-magnetohydrodynamics.md#equivariant-three-mode-dynamo-normal-form)
      - [Magnetic onset on a rotating velocity branch](resistive-magnetohydrodynamics.md#magnetic-onset-on-a-rotating-velocity-branch)
      - [Normalization of nonzero dynamo coupling coefficients](resistive-magnetohydrodynamics.md#normalization-of-nonzero-dynamo-coupling-coefficients)
    - [Anti-dynamo theorem](resistive-magnetohydrodynamics.md#anti-dynamo-theorem)
      - [Periodic two-coordinate anti-dynamo energy bound](resistive-magnetohydrodynamics.md#periodic-two-coordinate-anti-dynamo-energy-bound)
      - [Planar anti-dynamo theorem](resistive-magnetohydrodynamics.md#planar-anti-dynamo-theorem)
        - [Zeldovich planar flux balance](resistive-magnetohydrodynamics.md#zeldovich-planar-flux-balance)
      - [Toroidal-velocity anti-dynamo theorem](resistive-magnetohydrodynamics.md#toroidal-velocity-anti-dynamo-theorem)
      - [Cowling anti-dynamo theorem](resistive-magnetohydrodynamics.md#cowling-anti-dynamo-theorem)
    - [Magnetic concentration by an incompressible stagnation flow](resistive-magnetohydrodynamics.md#magnetic-concentration-by-an-incompressible-stagnation-flow)
      - [Self-similar magnetic mode in a stagnation flow](resistive-magnetohydrodynamics.md#self-similar-magnetic-mode-in-a-stagnation-flow)
    - [Backus' necessary condition for dynamo action](resistive-magnetohydrodynamics.md#backus-necessary-condition-for-dynamo-action)
      - [Maximum-strain bound on dynamo growth](resistive-magnetohydrodynamics.md#maximum-strain-bound-on-dynamo-growth)
    - [Mean-field dynamo](resistive-magnetohydrodynamics.md#mean-field-dynamo)
      - [Mean-field shearing-wave transient amplification](resistive-magnetohydrodynamics.md#mean-field-shearing-wave-transient-amplification)
      - [Dipole and quadrupole parity in a mean-field dynamo](resistive-magnetohydrodynamics.md#dipole-and-quadrupole-parity-in-a-mean-field-dynamo)
        - [Coupled-hemisphere dynamo parity threshold](resistive-magnetohydrodynamics.md#coupled-hemisphere-dynamo-parity-threshold)
        - [Parity splitting of a mean-field dynamo threshold](resistive-magnetohydrodynamics.md#parity-splitting-of-a-mean-field-dynamo-threshold)
      - [Alpha-Omega dynamo](resistive-magnetohydrodynamics.md#alpha-omega-dynamo)
        - [Plane-layer alpha-Omega dynamo threshold](resistive-magnetohydrodynamics.md#plane-layer-alpha-omega-dynamo-threshold)
        - [Alpha-squared Omega dynamo threshold](resistive-magnetohydrodynamics.md#alpha-squared-omega-dynamo-threshold)
        - [Bounded-modulation alpha-Omega growth estimate](resistive-magnetohydrodynamics.md#bounded-modulation-alpha-omega-growth-estimate)
      - [Omega effect](resistive-magnetohydrodynamics.md#omega-effect)
      - [First-order smoothing approximation](resistive-magnetohydrodynamics.md#first-order-smoothing-approximation)
        - [Isotropic alpha effect of three helical traveling waves](resistive-magnetohydrodynamics.md#isotropic-alpha-effect-of-three-helical-traveling-waves)
        - [Helicity formula for isotropic first-order smoothing](resistive-magnetohydrodynamics.md#helicity-formula-for-isotropic-first-order-smoothing)
        - [Quasistatic magnetic response of a helical shearing wave](resistive-magnetohydrodynamics.md#quasistatic-magnetic-response-of-a-helical-shearing-wave)
        - [Monochromatic coupled magnetic and velocity response](resistive-magnetohydrodynamics.md#monochromatic-coupled-magnetic-and-velocity-response)
        - [Oscillatory magnetic response in first-order smoothing](resistive-magnetohydrodynamics.md#oscillatory-magnetic-response-in-first-order-smoothing)
      - [Parker dynamo wave](resistive-magnetohydrodynamics.md#parker-dynamo-wave)
        - [Local alpha-Omega dynamo wave dispersion](resistive-magnetohydrodynamics.md#local-alpha-omega-dynamo-wave-dispersion)
        - [Periodically reversing Parker dynamo coupling](resistive-magnetohydrodynamics.md#periodically-reversing-parker-dynamo-coupling)
      - [Alpha effect](resistive-magnetohydrodynamics.md#alpha-effect)
        - [Rapidly fluctuating alpha effect](resistive-magnetohydrodynamics.md#rapidly-fluctuating-alpha-effect)
        - [Strong-field quenching of an isotropic electromotive force](resistive-magnetohydrodynamics.md#strong-field-quenching-of-an-isotropic-electromotive-force)
        - [Alpha-squared dynamo](resistive-magnetohydrodynamics.md#alpha-squared-dynamo)
          - [Homogeneous alpha-squared dynamo growth criterion](resistive-magnetohydrodynamics.md#homogeneous-alpha-squared-dynamo-growth-criterion)
          - [Anisotropic alpha-squared dynamo](resistive-magnetohydrodynamics.md#anisotropic-alpha-squared-dynamo)
            - [Uniaxial alpha dynamo threshold](resistive-magnetohydrodynamics.md#uniaxial-alpha-dynamo-threshold)
        - [Alpha tensor](resistive-magnetohydrodynamics.md#alpha-tensor)
      - [Mean-field electromotive force](resistive-magnetohydrodynamics.md#mean-field-electromotive-force)
        - [Monochromatic small-Reynolds-number mean electromotive force](resistive-magnetohydrodynamics.md#monochromatic-small-reynolds-number-mean-electromotive-force)
          - [Antisymmetry of the second-order monochromatic alpha tensor](resistive-magnetohydrodynamics.md#antisymmetry-of-the-second-order-monochromatic-alpha-tensor)
          - [Symmetry of the first-order monochromatic alpha tensor](resistive-magnetohydrodynamics.md#symmetry-of-the-first-order-monochromatic-alpha-tensor)
        - [Turbulent magnetic pumping](resistive-magnetohydrodynamics.md#turbulent-magnetic-pumping)
        - [Integrated electromotive response of a finite cyclonic event](resistive-magnetohydrodynamics.md#integrated-electromotive-response-of-a-finite-cyclonic-event)
        - [Space-time average of periodic modes](resistive-magnetohydrodynamics.md#space-time-average-of-periodic-modes)
  - [Hartmann flow](resistive-magnetohydrodynamics.md#hartmann-flow)
    - [Hartmann flow rate with normal-field walls](resistive-magnetohydrodynamics.md#hartmann-flow-rate-with-normal-field-walls)
    - [Hartmann layer](resistive-magnetohydrodynamics.md#hartmann-layer)
    - [Hartmann number](resistive-magnetohydrodynamics.md#hartmann-number)
  - [Normal magnetic field boundary condition](resistive-magnetohydrodynamics.md#normal-magnetic-field-boundary-condition)
  - [Resistive induction equation](resistive-magnetohydrodynamics.md#resistive-induction-equation)
    - [Conductivity-gradient term in magnetic induction](resistive-magnetohydrodynamics.md#conductivity-gradient-term-in-magnetic-induction)
    - [Shearing-coordinate magnetic flux equation](resistive-magnetohydrodynamics.md#shearing-coordinate-magnetic-flux-equation)
    - [Radial magnetic induction scalar](resistive-magnetohydrodynamics.md#radial-magnetic-induction-scalar)
      - [Insulating boundary condition for the radial magnetic scalar](resistive-magnetohydrodynamics.md#insulating-boundary-condition-for-the-radial-magnetic-scalar)
- [Magnetic diffusion](#magnetic-diffusion)
  - [Magnetic phase mixing under differential rotation](#magnetic-phase-mixing-under-differential-rotation)
    - [Exact quadratic-shear magnetic flux solution](#exact-quadratic-shear-magnetic-flux-solution)
  - [Magnetic free-decay spectral bound](#magnetic-free-decay-spectral-bound)
  - [Magnetic diffusivity](#magnetic-diffusivity)
    - [Magnetic Prandtl number](#magnetic-prandtl-number)
    - [Turbulent magnetic diffusivity](#turbulent-magnetic-diffusivity)
      - [Variance bound for planar turbulent magnetic transport](#variance-bound-for-planar-turbulent-magnetic-transport)
- [Magnetic Reynolds number](#magnetic-reynolds-number)
- [Moving-conductor Ohm law](#moving-conductor-ohm-law)
- [Magnetoconvection](#magnetoconvection)
  - [Three-mode porous magnetoconvection](#three-mode-porous-magnetoconvection)
    - [Cubic centre-manifold reduction of porous magnetoconvection](#cubic-centre-manifold-reduction-of-porous-magnetoconvection)
  - [Thermal-diffusion scaling of planar magnetoconvection](#thermal-diffusion-scaling-of-planar-magnetoconvection)
  - [Quasistatic vertical-field magnetoconvection](#quasistatic-vertical-field-magnetoconvection)
    - [Cubic saturation of quasistatic magnetoconvection](#cubic-saturation-of-quasistatic-magnetoconvection)
  - [Five-mode vertical-field magnetoconvection](#five-mode-vertical-field-magnetoconvection)
    - [Conduction double-zero criterion for five-mode magnetoconvection](#conduction-double-zero-criterion-for-five-mode-magnetoconvection)
    - [Stationary branch of five-mode magnetoconvection](#stationary-branch-of-five-mode-magnetoconvection)
      - [Pitchfork reversal near geometric ratio two in magnetoconvection](#pitchfork-reversal-near-geometric-ratio-two-in-magnetoconvection)
  - [Horizontal-field magnetoconvection dispersion relation](#horizontal-field-magnetoconvection-dispersion-relation)
    - [Strong-field steady magnetoconvection varying along the field](#strong-field-steady-magnetoconvection-varying-along-the-field)
    - [Magnetic-field-aligned rolls evade steady magnetic inhibition](#magnetic-field-aligned-rolls-evade-steady-magnetic-inhibition)
  - [Magnetic-to-thermal diffusivity ratio](#magnetic-to-thermal-diffusivity-ratio)
  - [Subcritical magnetoconvection](#subcritical-magnetoconvection)
  - [Magnetic flux separation](#magnetic-flux-separation)
  - [Oblique-field plane-wave magnetoconvection](#oblique-field-plane-wave-magnetoconvection)
    - [Field-independent stationary threshold in oblique magnetoconvection](#field-independent-stationary-threshold-in-oblique-magnetoconvection)
    - [Wavenumber selection in oblique-field magnetoconvection](#wavenumber-selection-in-oblique-field-magnetoconvection)
  - [Vertical-field magnetoconvection dispersion relation](#vertical-field-magnetoconvection-dispersion-relation)
    - [Three-amplitude vertical-field magnetoconvection](#three-amplitude-vertical-field-magnetoconvection)
    - [Exact critical Rayleigh relation for vertical-field magnetoconvection](#exact-critical-rayleigh-relation-for-vertical-field-magnetoconvection)
    - [Strong-field wavenumber selection in magnetoconvection](#strong-field-wavenumber-selection-in-magnetoconvection)
    - [Oscillatory marginality in vertical-field magnetoconvection](#oscillatory-marginality-in-vertical-field-magnetoconvection)
      - [Steady-Hopf merger in vertical-field magnetoconvection](#steady-hopf-merger-in-vertical-field-magnetoconvection)
        - [Merger at a magnetoconvection neutral-curve minimum](#merger-at-a-magnetoconvection-neutral-curve-minimum)
  - [Chandrasekhar number](#chandrasekhar-number)
    - [Thermal-diffusion magnetic-field parameter](#thermal-diffusion-magnetic-field-parameter)
  - [Convection amplitude coupled to a conserved field](#convection-amplitude-coupled-to-a-conserved-field)
    - [Localized pulse of a conserved-field convection model](#localized-pulse-of-a-conserved-field-convection-model)
    - [Conserved-field sideband dispersion relation](#conserved-field-sideband-dispersion-relation)
      - [Long-wave instability with a conserved mean field](#long-wave-instability-with-a-conserved-mean-field)
- [Magnetic buoyancy instability](#magnetic-buoyancy-instability)
  - [Isothermal interchange criterion for magnetic buoyancy](#isothermal-interchange-criterion-for-magnetic-buoyancy)
  - [Localized interchange criterion for a magnetized atmosphere](#localized-interchange-criterion-for-a-magnetized-atmosphere)
  - [Parker instability](#parker-instability)
    - [Long-wavelength undular magnetic buoyancy criterion](#long-wavelength-undular-magnetic-buoyancy-criterion)
    - [Magnetic buoyancy energy criterion](#magnetic-buoyancy-energy-criterion)
      - [Short transverse wavelength limit for magnetic buoyancy](#short-transverse-wavelength-limit-for-magnetic-buoyancy)
- [Poloidal magnetic field](#poloidal-magnetic-field)
- [Magnetic pressure](#magnetic-pressure)
  - [Magnetic pressure discontinuity in an isothermal atmosphere](#magnetic-pressure-discontinuity-in-an-isothermal-atmosphere)
  - [Magnetohydrodynamic total pressure](#magnetohydrodynamic-total-pressure)
- [Magnetic tension](#magnetic-tension)
- [Toroidal magnetic field](#toroidal-magnetic-field)
  - [Toroidal magnetic-field winding equation](#toroidal-magnetic-field-winding-equation)
    - [Steady toroidal induction by spherical differential rotation](#steady-toroidal-induction-by-spherical-differential-rotation)
      - [Diffusive establishment time of a wound toroidal field](#diffusive-establishment-time-of-a-wound-toroidal-field)
  - [Michael criterion for axisymmetric toroidal-field interchange](#michael-criterion-for-axisymmetric-toroidal-field-interchange)
    - [Toroidal interchange field threshold in a thin Keplerian disk](#toroidal-interchange-field-threshold-in-a-thin-keplerian-disk)
    - [Global variational form of the Michael criterion](#global-variational-form-of-the-michael-criterion)
  - [Uniform-current toroidal-field curl reduction](#uniform-current-toroidal-field-curl-reduction)
    - [Neutral quadrupolar perturbation of a uniform-current toroidal field](#neutral-quadrupolar-perturbation-of-a-uniform-current-toroidal-field)
- [Ideal magnetohydrodynamics](ideal-magnetohydrodynamics.md)
  - [Magnetic relaxation](ideal-magnetohydrodynamics.md#magnetic-relaxation)
    - [Single-molecule magnet](ideal-magnetohydrodynamics.md#single-molecule-magnet)
    - [Quantum tunnelling of magnetization](ideal-magnetohydrodynamics.md#quantum-tunnelling-of-magnetization)
    - [Collapse of a planar magnetic separatrix](ideal-magnetohydrodynamics.md#collapse-of-a-planar-magnetic-separatrix)
    - [Viscous magnetic-relaxation energy identity](ideal-magnetohydrodynamics.md#viscous-magnetic-relaxation-energy-identity)
  - [Steady planar ideal-MHD field-line invariants](ideal-magnetohydrodynamics.md#steady-planar-ideal-mhd-field-line-invariants)
    - [Alfvénic degeneracy of steady planar MHD](ideal-magnetohydrodynamics.md#alfvenic-degeneracy-of-steady-planar-mhd)
    - [Planar ideal-MHD Bernoulli invariant](ideal-magnetohydrodynamics.md#planar-ideal-mhd-bernoulli-invariant)
  - [Grad-Shafranov equation](ideal-magnetohydrodynamics.md#grad-shafranov-equation)
    - [Grad-Shafranov equation for a force-free magnetic field](ideal-magnetohydrodynamics.md#grad-shafranov-equation-for-a-force-free-magnetic-field)
  - [Reduced magnetohydrodynamics](ideal-magnetohydrodynamics.md#reduced-magnetohydrodynamics)
    - [Five quadratic cascade invariants of anisotropic magnetohydrodynamic turbulence](ideal-magnetohydrodynamics.md#five-quadratic-cascade-invariants-of-anisotropic-magnetohydrodynamic-turbulence)
    - [Slow and entropy fluctuations in reduced magnetohydrodynamics](ideal-magnetohydrodynamics.md#slow-and-entropy-fluctuations-in-reduced-magnetohydrodynamics)
  - [Ideal magnetohydrodynamic energy conservation](ideal-magnetohydrodynamics.md#ideal-magnetohydrodynamic-energy-conservation)
  - [Ideal magnetohydrodynamic momentum equation](ideal-magnetohydrodynamics.md#ideal-magnetohydrodynamic-momentum-equation)
  - [Plane-parallel magnetohydrodynamic flow with imposed shear](ideal-magnetohydrodynamics.md#plane-parallel-magnetohydrodynamic-flow-with-imposed-shear)
    - [Alfvén-point compatibility in a plane-parallel sheared flow](ideal-magnetohydrodynamics.md#alfven-point-compatibility-in-a-plane-parallel-sheared-flow)
    - [Magnetohydrodynamic shear work](ideal-magnetohydrodynamics.md#magnetohydrodynamic-shear-work)
  - [Ideal magnetohydrodynamic equations](ideal-magnetohydrodynamics.md#ideal-magnetohydrodynamic-equations)
  - [Magnetohydrodynamic energy principle](ideal-magnetohydrodynamics.md#magnetohydrodynamic-energy-principle)
    - [Incompressible magnetic displacement energy identity](ideal-magnetohydrodynamics.md#incompressible-magnetic-displacement-energy-identity)
      - [Interchange stability of an incompressible magnetized atmosphere](ideal-magnetohydrodynamics.md#interchange-stability-of-an-incompressible-magnetized-atmosphere)
    - [Linear displacement equations for a magnetized atmosphere](ideal-magnetohydrodynamics.md#linear-displacement-equations-for-a-magnetized-atmosphere)
  - [Elsässer variable](ideal-magnetohydrodynamics.md#elsasser-variable)
    - [Elsässer energy invariant](ideal-magnetohydrodynamics.md#elsasser-energy-invariant)
  - [Cross-helicity](ideal-magnetohydrodynamics.md#cross-helicity)
    - [Cross-helicity conservation law](ideal-magnetohydrodynamics.md#cross-helicity-conservation-law)
      - [Material conservation of cross-helicity density](ideal-magnetohydrodynamics.md#material-conservation-of-cross-helicity-density)
  - [Magnetic flux freezing](ideal-magnetohydrodynamics.md#magnetic-flux-freezing)
    - [Material magnetic-flux transport theorem](ideal-magnetohydrodynamics.md#material-magnetic-flux-transport-theorem)
    - [Flux-surface preservation during magnetic-tube expansion](ideal-magnetohydrodynamics.md#flux-surface-preservation-during-magnetic-tube-expansion)
    - [Mass-to-flux ratio](ideal-magnetohydrodynamics.md#mass-to-flux-ratio)
      - [Critical mass-to-flux ratio](ideal-magnetohydrodynamics.md#critical-mass-to-flux-ratio)
  - [Alfvén speed](ideal-magnetohydrodynamics.md#alfven-speed)
    - [Alfvén Mach number](ideal-magnetohydrodynamics.md#alfven-mach-number)
    - [Alfvén velocity](ideal-magnetohydrodynamics.md#alfven-velocity)
    - [Alfvén number](ideal-magnetohydrodynamics.md#alfven-number)
  - [Magnetohydrodynamic wave](ideal-magnetohydrodynamics.md#magnetohydrodynamic-wave)
    - [Parallel-propagating ideal magnetohydrodynamic wave](ideal-magnetohydrodynamics.md#parallel-propagating-ideal-magnetohydrodynamic-wave)
    - [Ambipolar damping](ideal-magnetohydrodynamics.md#ambipolar-damping)
      - [Equal-density ion-neutral Alfvén dispersion relation](ideal-magnetohydrodynamics.md#equal-density-ion-neutral-alfven-dispersion-relation)
        - [Strong-collision ion-neutral Alfvén modes](ideal-magnetohydrodynamics.md#strong-collision-ion-neutral-alfven-modes)
    - [Entropy mode](ideal-magnetohydrodynamics.md#entropy-mode)
    - [Magnetohydrodynamic wave polarization](ideal-magnetohydrodynamics.md#magnetohydrodynamic-wave-polarization)
    - [Uniform-current rotating magnetohydrodynamic wave dispersion](ideal-magnetohydrodynamics.md#uniform-current-rotating-magnetohydrodynamic-wave-dispersion)
      - [Single-azimuthal-mode current-driven instability threshold](ideal-magnetohydrodynamics.md#single-azimuthal-mode-current-driven-instability-threshold)
    - [Alfvén wave](ideal-magnetohydrodynamics.md#alfven-wave)
      - [Linear Alfvén wave equations](ideal-magnetohydrodynamics.md#linear-alfven-wave-equations)
      - [Alfvén wave energy transport](ideal-magnetohydrodynamics.md#alfven-wave-energy-transport)
      - [Resistive damping of an Alfvén wave](ideal-magnetohydrodynamics.md#resistive-damping-of-an-alfven-wave)
      - [Lundquist liquid-metal Alfvén wave experiment](ideal-magnetohydrodynamics.md#lundquist-liquid-metal-alfven-wave-experiment)
      - [Alfvén-resonant vorticity in a parallel magnetic shear flow](ideal-magnetohydrodynamics.md#alfven-resonant-vorticity-in-a-parallel-magnetic-shear-flow)
      - [Kinetic Alfvén wave](ideal-magnetohydrodynamics.md#kinetic-alfven-wave)
      - [Magnetohydrodynamic phase mixing](ideal-magnetohydrodynamics.md#magnetohydrodynamic-phase-mixing)
      - [Torsional Alfvén wave](ideal-magnetohydrodynamics.md#torsional-alfven-wave)
        - [Pressure compatibility of nonlinear torsional Alfvén profiles](ideal-magnetohydrodynamics.md#pressure-compatibility-of-nonlinear-torsional-alfven-profiles)
        - [Cylinder-averaged torsional Alfvén wave](ideal-magnetohydrodynamics.md#cylinder-averaged-torsional-alfven-wave)
          - [Conserved energy of a cylinder-averaged torsional wave](ideal-magnetohydrodynamics.md#conserved-energy-of-a-cylinder-averaged-torsional-wave)
        - [Magnetic axial angular momentum flux](ideal-magnetohydrodynamics.md#magnetic-axial-angular-momentum-flux)
      - [Nonlinear Alfvén wave](ideal-magnetohydrodynamics.md#nonlinear-alfven-wave)
        - [Magnetic-pressure obstruction to a linearly polarized Alfvén wave](ideal-magnetohydrodynamics.md#magnetic-pressure-obstruction-to-a-linearly-polarized-alfven-wave)
        - [Circularly polarized nonlinear Alfvén wave](ideal-magnetohydrodynamics.md#circularly-polarized-nonlinear-alfven-wave)
      - [Alfvén characteristic eigenvector](ideal-magnetohydrodynamics.md#alfven-characteristic-eigenvector)
      - [Alfvén frequency](ideal-magnetohydrodynamics.md#alfven-frequency)
      - [Alfvén wing](ideal-magnetohydrodynamics.md#alfven-wing)
        - [Alfvénic Mach-cone slope](ideal-magnetohydrodynamics.md#alfvenic-mach-cone-slope)
    - [Magnetosonic wave](ideal-magnetohydrodynamics.md#magnetosonic-wave)
      - [High-pressure limit of magnetosonic waves](ideal-magnetohydrodynamics.md#high-pressure-limit-of-magnetosonic-waves)
        - [Pseudo-Alfvén wave](ideal-magnetohydrodynamics.md#pseudo-alfven-wave)
      - [Isothermal coplanar magnetohydrodynamic characteristic matrix](ideal-magnetohydrodynamics.md#isothermal-coplanar-magnetohydrodynamic-characteristic-matrix)
      - [Magnetosonic critical speed](ideal-magnetohydrodynamics.md#magnetosonic-critical-speed)
        - [Regularity at a magnetosonic point](ideal-magnetohydrodynamics.md#regularity-at-a-magnetosonic-point)
          - [Cold-limit degeneracy of a slow magnetosonic point](ideal-magnetohydrodynamics.md#cold-limit-degeneracy-of-a-slow-magnetosonic-point)
      - [Fast magnetosonic wave](ideal-magnetohydrodynamics.md#fast-magnetosonic-wave)
      - [Slow magnetosonic wave](ideal-magnetohydrodynamics.md#slow-magnetosonic-wave)
      - [Tube speed](ideal-magnetohydrodynamics.md#tube-speed)
    - [Magnetohydrodynamic interface wave](ideal-magnetohydrodynamics.md#magnetohydrodynamic-interface-wave)
      - [Magnetic stabilization of an equal-density vortex sheet](ideal-magnetohydrodynamics.md#magnetic-stabilization-of-an-equal-density-vortex-sheet)
  - [Force-free magnetic field](ideal-magnetohydrodynamics.md#force-free-magnetic-field)
    - [Magnetic-energy injection by differential boundary rotation](ideal-magnetohydrodynamics.md#magnetic-energy-injection-by-differential-boundary-rotation)
    - [Force-free parameter](ideal-magnetohydrodynamics.md#force-free-parameter)
    - [Cylindrical force-free magnetic field](ideal-magnetohydrodynamics.md#cylindrical-force-free-magnetic-field)
  - [Linearized ideal magnetohydrodynamic equations](ideal-magnetohydrodynamics.md#linearized-ideal-magnetohydrodynamic-equations)
    - [Displacement equation for a parallel magnetic shear flow](ideal-magnetohydrodynamics.md#displacement-equation-for-a-parallel-magnetic-shear-flow)
  - [Ideal magnetohydrodynamic induction equation](ideal-magnetohydrodynamics.md#ideal-magnetohydrodynamic-induction-equation)
    - [Ideal magnetic response to a cylindrical cyclonic event](ideal-magnetohydrodynamics.md#ideal-magnetic-response-to-a-cylindrical-cyclonic-event)
    - [Cartesian magnetic flux function](ideal-magnetohydrodynamics.md#cartesian-magnetic-flux-function)
      - [Magnetic island](ideal-magnetohydrodynamics.md#magnetic-island)
      - [Cartesian magnetostatic flux-function equilibrium](ideal-magnetohydrodynamics.md#cartesian-magnetostatic-flux-function-equilibrium)
    - [Axisymmetric magnetic winding](ideal-magnetohydrodynamics.md#axisymmetric-magnetic-winding)
      - [Magnetic-pressure equality radius under Keplerian winding](ideal-magnetohydrodynamics.md#magnetic-pressure-equality-radius-under-keplerian-winding)
      - [Ferraro's law of isorotation](ideal-magnetohydrodynamics.md#ferraro-s-law-of-isorotation)
  - [Entropy advection equation](ideal-magnetohydrodynamics.md#entropy-advection-equation)
  - [Magnetohydrodynamic shock](ideal-magnetohydrodynamics.md#magnetohydrodynamic-shock)
    - [Perpendicular magnetohydrodynamic shock](ideal-magnetohydrodynamics.md#perpendicular-magnetohydrodynamic-shock)
      - [Compression ratio of a perpendicular magnetohydrodynamic shock](ideal-magnetohydrodynamics.md#compression-ratio-of-a-perpendicular-magnetohydrodynamic-shock)
    - [Parallel magnetohydrodynamic shock](ideal-magnetohydrodynamics.md#parallel-magnetohydrodynamic-shock)
    - [Ideal magnetohydrodynamic shock conditions](ideal-magnetohydrodynamics.md#ideal-magnetohydrodynamic-shock-conditions)
    - [de Hoffmann–Teller frame](ideal-magnetohydrodynamics.md#de-hoffmann-teller-frame)
    - [Rotational discontinuity in magnetohydrodynamics](ideal-magnetohydrodynamics.md#rotational-discontinuity-in-magnetohydrodynamics)
  - [Axisymmetric magnetostatic Grad-Shafranov system](ideal-magnetohydrodynamics.md#axisymmetric-magnetostatic-grad-shafranov-system)
  - [Axisymmetric magnetohydrodynamic wind](ideal-magnetohydrodynamics.md#axisymmetric-magnetohydrodynamic-wind)
    - [Cold radial magnetohydrodynamic wind integral](ideal-magnetohydrodynamics.md#cold-radial-magnetohydrodynamic-wind-integral)
    - [Sub-Alfvénic isorotation in a steady axisymmetric wind](ideal-magnetohydrodynamics.md#sub-alfvenic-isorotation-in-a-steady-axisymmetric-wind)
    - [Corotating energy invariant of an axisymmetric magnetic wind](ideal-magnetohydrodynamics.md#corotating-energy-invariant-of-an-axisymmetric-magnetic-wind)
    - [Field-line angular velocity of an axisymmetric wind](ideal-magnetohydrodynamics.md#field-line-angular-velocity-of-an-axisymmetric-wind)
    - [Poloidal magnetic flux function](ideal-magnetohydrodynamics.md#poloidal-magnetic-flux-function)
      - [Material advection of an axisymmetric magnetic flux function](ideal-magnetohydrodynamics.md#material-advection-of-an-axisymmetric-magnetic-flux-function)
      - [Axisymmetric magnetic flux surface](ideal-magnetohydrodynamics.md#axisymmetric-magnetic-flux-surface)
      - [Power-law poloidal field near a disk surface](ideal-magnetohydrodynamics.md#power-law-poloidal-field-near-a-disk-surface)
    - [Magnetohydrodynamic mass loading](ideal-magnetohydrodynamics.md#magnetohydrodynamic-mass-loading)
      - [Regular-axis alignment of steady poloidal ideal flow](ideal-magnetohydrodynamics.md#regular-axis-alignment-of-steady-poloidal-ideal-flow)
    - [Field-line angular velocity](ideal-magnetohydrodynamics.md#field-line-angular-velocity)
    - [Magnetohydrodynamic angular-momentum invariant](ideal-magnetohydrodynamics.md#magnetohydrodynamic-angular-momentum-invariant)
      - [Maxwell torque conservation in an axisymmetric wind](ideal-magnetohydrodynamics.md#maxwell-torque-conservation-in-an-axisymmetric-wind)
    - [Magnetohydrodynamic Bernoulli invariant](ideal-magnetohydrodynamics.md#magnetohydrodynamic-bernoulli-invariant)
      - [Isothermal magnetic Bernoulli integral](ideal-magnetohydrodynamics.md#isothermal-magnetic-bernoulli-integral)
    - [Alfvén surface](ideal-magnetohydrodynamics.md#alfven-surface)
      - [Alfvén radius](ideal-magnetohydrodynamics.md#alfven-radius)
      - [Alfvén-surface regularity condition for an axisymmetric wind](ideal-magnetohydrodynamics.md#alfven-surface-regularity-condition-for-an-axisymmetric-wind)
    - [Asymptotic energy of a radial magnetohydrodynamic wind](ideal-magnetohydrodynamics.md#asymptotic-energy-of-a-radial-magnetohydrodynamic-wind)
    - [Magnetocentrifugal acceleration](ideal-magnetohydrodynamics.md#magnetocentrifugal-acceleration)
      - [Thirty-degree magnetocentrifugal launching criterion](ideal-magnetohydrodynamics.md#thirty-degree-magnetocentrifugal-launching-criterion)
        - [Marginal straight-line launch at thirty degrees](ideal-magnetohydrodynamics.md#marginal-straight-line-launch-at-thirty-degrees)
      - [Magnetocentrifugal launching criterion in a flattened power-law potential](ideal-magnetohydrodynamics.md#magnetocentrifugal-launching-criterion-in-a-flattened-power-law-potential)

## Magnetic flux concentration

↑ **Parent:** [Magnetohydrodynamics](magnetohydrodynamics.md)

Magnetic flux concentration redistributes existing [magnetic flux](magnetic-field.md#magnetic-flux) into a smaller area. For a locally straight flux bundle with conserved flux, $B\mathcal A$ is constant, so decreasing area increases field strength. Converging convection, field-line stretching and [flux expulsion](resistive-magnetohydrodynamics.md#flux-expulsion) can produce concentrations; finite [magnetic diffusivity](#magnetic-diffusivity) opposes them and [Lorentz force](relativistic-electromagnetism.md#lorentz-force) feedback limits the kinematic approximation. Redistribution alone is not evidence of net [dynamo action](resistive-magnetohydrodynamics.md#dynamo-action).

### Equipartition magnetic field

↑ **Parent:** [Magnetic flux concentration](#magnetic-flux-concentration)

Equating magnetic energy density $B^2/(2\mu_0)$ to kinetic energy density $\rho U^2/2$ defines this order-of-magnitude field. It marks when a weak-field kinematic treatment of a given flow can fail, not a universal upper bound on concentrated fields. Gas-pressure confinement, compression, partial evacuation and dynamic pressure can allow stronger local fields.

### Convective collapse

↑ **Parent:** [Magnetic flux concentration](#magnetic-flux-concentration)

A compressible intensification mechanism for a thin, nearly vertical [flux tube](magnetic-field.md#flux-tube) in a superadiabatic atmosphere. An unstable downflow drains material and lowers internal gas pressure; approximate lateral balance $p_i+B^2/(2\mu_0)=p_e$ then permits the tube to contract and its field to strengthen at nearly conserved [magnetic flux](magnetic-field.md#magnetic-flux). It relies on compressibility and thermal evolution, which are absent from a strict [Boussinesq approximation](geophysical-fluid-dynamics.md#boussinesq-approximation). Dynamic photospheric structures need not satisfy thin-tube equilibrium, so this mechanism does not explain every intense field concentration.

## Magnetostrophic balance

↑ **Parent:** [Magnetohydrodynamics](magnetohydrodynamics.md)

The leading force balance in a rapidly rotating conducting fluid when inertial and viscous forces are small, while [Coriolis force](mathematical-physics.md#coriolis-force), [pressure](pressure.md), [buoyancy](fluid-mechanics.md#buoyancy) and [Lorentz force density](relativistic-electromagnetism.md#lorentz-force-density) remain significant. The [Rossby number](geophysical-fluid-dynamics.md#rossby-number) and [Ekman number](geophysical-fluid-dynamics.md#ekman-number) measure the omitted inertia and bulk viscosity. Rotation does not balance an arbitrary magnetic torque: impenetrable axisymmetric boundaries impose the [Taylor constraint](#taylor-constraint). Magnetic diffusion can remain in the induction equation even when viscosity is neglected in momentum balance.

### Taylor constraint

↑ **Parent:** [Magnetostrophic balance](#magnetostrophic-balance)

In inviscid [magnetostrophic balance](#magnetostrophic-balance) within an impenetrable axisymmetric container, with no azimuthal buoyancy or external mechanical torque, the cylindrically integrated [Lorentz force density](relativistic-electromagnetism.md#lorentz-force-density) must vanish on every cylinder coaxial with rotation. The azimuthal pressure derivative integrates to zero, and the cylindrical Coriolis integral is proportional to net radial flux, zero by incompressibility and impermeability. Multiplying by cylinder area and lever arm gives the equivalent zero-torque form. This rotating-fluid condition is distinct from magnetic-helicity relaxation to a force-free plasma state. Its original primary source is [Taylor's 1963 rotating-fluid paper](https://mhd.ens.fr/IHP09/Jackson/Biblio/taylor_63.pdf).

#### Viscous regularization of the Taylor constraint

↑ **Parent:** [Taylor constraint](#taylor-constraint)

With small viscosity, the azimuthal cylindrical balance permits [Lorentz force](relativistic-electromagnetism.md#lorentz-force) torque to be cancelled by viscous stress. For ordinary no-slip rotating boundaries an [Ekman layer](geophysical-fluid-dynamics.md#ekman-layer) gives stress of order $\rho\Omega LU\sqrt E$, larger than the order-$E$ bulk viscous correction at fixed velocity. Thus bounded small-$E$ flows approach a [magnetostrophic Taylor state](#magnetostrophic-taylor-state) but need not satisfy its constraint exactly at finite viscosity. An order-one uncompensated magnetic torque would require a divergent flow as $E\to0$, invalidating the assumed small-inertia balance. Stress-free boundaries remove the leading no-slip friction and require their own torque/regularity conditions.

#### Geostrophic flow preserving the Taylor constraint

↑ **Parent:** [Taylor constraint](#taylor-constraint)

For an instantaneous [magnetostrophic Taylor state](#magnetostrophic-taylor-state), the momentum equation leaves a geostrophic null component $u_g=s\omega(s)\hat\phi$. Decompose the velocity into this component and a particular ageostrophic flow, substitute the induction equation into the displayed derivative constraint, and solve the resulting linear equation for $\omega$ with magnetic boundary conditions imposed. When magnetic surface torque vanishes, the geostrophic part is $\mu_0^{-1}\partial_s[s^3\int_{C_s}B_s^2d\phi dz\,\omega']$. Boundary terms generally cannot be discarded for an insulating exterior; the primary analysis is [Hardy and collaborators' boundary-compatible geostrophic-flow construction](https://arxiv.org/abs/1806.06612). Regularity and an angular-momentum normalization fix remaining homogeneous freedoms when the magnetic coupling is nondegenerate.

#### Magnetostrophic Taylor state

↑ **Parent:** [Taylor constraint](#taylor-constraint)

A divergence-free [magnetic field](magnetic-field.md) satisfying the [Taylor constraint](#taylor-constraint) on all geostrophic cylinders. It is a compatibility condition for slow rotating-fluid balance, not a local force-free condition. To retain such a state as magnetic induction proceeds, the velocity must also preserve the time derivative of the cylindrical torque constraint.

## Mean-field electrodynamics

↑ **Parent:** [Magnetohydrodynamics](magnetohydrodynamics.md)

[Mean-field electrodynamics](#mean-field-electrodynamics) applies averaging and a response closure to magnetic induction in a fluctuating conducting fluid. The mean equation contains the correlated [mean-field electromotive force](resistive-magnetohydrodynamics.md#mean-field-electromotive-force) in the title. Scale separation permits a local expansion into alpha transport, [turbulent diffusion](turbulence.md#eddy-diffusion) and higher gradients; general anisotropic or finite-memory statistics require tensorial and nonlocal responses. A [mean-field dynamo](resistive-magnetohydrodynamics.md#mean-field-dynamo) is a self-exciting application of this framework, not a consequence of averaging alone.

## Kinematic magnetic dynamo

↑ **Parent:** [Magnetohydrodynamics](magnetohydrodynamics.md)

A [kinematic magnetic dynamo](#kinematic-magnetic-dynamo) studies [magnetic field](magnetic-field.md) amplification by a prescribed [fluid flow](fluid-mechanics.md#fluid-flow), neglecting the field's feedback on the velocity through the [Lorentz force](relativistic-electromagnetism.md#lorentz-force). With incompressibility and zero [magnetic diffusivity](#magnetic-diffusivity), a Lagrangian field vector evolves by its local velocity-gradient matrix. A growth law derived in this approximation cannot hold indefinitely once magnetic stresses significantly change the flow.

### Gaussian white-noise magnetic stretching

↑ **Parent:** [Kinematic magnetic dynamo](#kinematic-magnetic-dynamo)

For a trace-free isotropic [Gaussian white noise](gaussian-process.md#gaussian-white-noise) velocity gradient with covariance $\langle\sigma_{im}(t)\sigma_{jn}(t')\rangle=\kappa_2\delta(t-t')[\delta_{ij}\delta_{mn}-(\delta_{im}\delta_{jn}+\delta_{in}\delta_{jm})/4]$, interpret the multiplicative equation as the [Stratonovich integral](stochastic-calculus.md#stratonovich-integral) limit of smooth velocity fluctuations. The causal [Furutsu–Novikov formula](gaussian-process.md#novikov-s-theorem) has endpoint weight one half. It gives $P_t=(\kappa_2/2)\partial_i[(B^2\delta_{ij}-B_iB_j/2)\partial_jP]$ for the vector [probability density function](continuous-probability-distribution.md#probability-density-function).

#### Lognormal magnetic-field amplification

↑ **Parent:** [Gaussian white-noise magnetic stretching](#gaussian-white-noise-magnetic-stretching)

Set $x=\ln(B/B_0)$ and $f=BF$ in the [radial magnetic-field Fokker-Planck equation](#radial-magnetic-field-fokker-planck-equation). Then $f_t=Df_{xx}-3Df_x$, so $f$ is a [Gaussian distribution](probability-distribution.md#normal-distribution) drifting at speed $3D$. For initial magnitude $B_0>0$, $F=[B\sqrt{4\pi Dt}]^{-1}\exp[-(\ln(B/B_0)-3Dt)^2/(4Dt)]$. This [lognormal distribution](probability-distribution.md#log-normal-distribution) has moments $B_0^q e^{Dq(q+3)t}$; the width of its logarithm grows as $\sqrt{2Dt}$.

#### Magnetic stretching moment growth

↑ **Parent:** [Gaussian white-noise magnetic stretching](#gaussian-white-noise-magnetic-stretching)

Twice integrating the [radial magnetic-field Fokker-Planck equation](#radial-magnetic-field-fokker-planck-equation) by parts gives the displayed law when moments and endpoint terms are controlled. In particular $\langle B^2\rangle$ grows at rate $10D=2\gamma$, with $\gamma=5\kappa_2/4$. The corresponding [magnetic energy](electromagnetic-wave.md#magnetic-energy) density is $\langle B^2\rangle/(8\pi)$ in [Gaussian units](electromagnetism.md#gaussian-units).

#### Radial magnetic-field Fokker-Planck equation

↑ **Parent:** [Gaussian white-noise magnetic stretching](#gaussian-white-noise-magnetic-stretching)

For an isotropic initial ensemble in [Gaussian white-noise magnetic stretching](#gaussian-white-noise-magnetic-stretching), $F(B)=4\pi B^2P(B)$ is the magnitude [probability density function](continuous-probability-distribution.md#probability-density-function). The radial vector equation $P_t=D(B^2P_{BB}+4BP_B)$ gives the displayed conservative [Fokker-Planck equation](probability-theory.md#fokker-planck-equation). Its integral is conserved under zero endpoint probability flux. For an anisotropic initial vector distribution, use the angularly averaged magnitude density instead; isotropic noise alone does not make arbitrary initial data isotropic.

## Theta pinch

↑ **Parent:** [Magnetohydrodynamics](magnetohydrodynamics.md)

A [theta pinch](#theta-pinch) is a cylindrical plasma configuration with axial [magnetic field](magnetic-field.md) and azimuthal [electric current](electric-charge.md#electric-current). For a static equilibrium without gravity, the radial [Lorentz force](relativistic-electromagnetism.md#lorentz-force) gives $d[p+B^2/(8\pi)]/dr=0$ in [Gaussian units](electromagnetism.md#gaussian-units). This straight-field configuration has no field-line curvature drive of the usual interchange instability.

### Positive ideal energy of a theta pinch

↑ **Parent:** [Theta pinch](#theta-pinch)

For an admissible Fourier [fluid Lagrangian displacement](fluid-mechanics.md#lagrangian-displacement-fluid-mechanics) $\boldsymbol\xi(r)e^{im\theta+ikz}$, put $D_\perp=(r\xi_r)'/r+im\xi_\theta/r$ and $D=D_\perp+ik\xi_z$. Force balance cancels every magnetic-field-gradient cross term in the [magnetohydrodynamic energy principle](ideal-magnetohydrodynamics.md#magnetohydrodynamic-energy-principle), leaving an integrand $\gamma p|D|^2+B^2[|D_\perp|^2+k^2(|\xi_r|^2+|\xi_\theta|^2)]/(4\pi)$. For $p\ge0$, $\gamma>0$, this is nonnegative. Neutral displacements can exist, so stability here means absence of negative-energy exponentially growing ideal modes, not strictly positive energy for every displacement.

## Hall magnetohydrodynamics

↑ **Parent:** [Magnetohydrodynamics](magnetohydrodynamics.md)

[Hall magnetohydrodynamics](#hall-magnetohydrodynamics) retains bulk [ion](chemistry.md#ion) inertia but freezes [magnetic flux](magnetic-field.md#magnetic-flux) into the [electron](physics.md#electron) velocity $\mathbf u_e=\mathbf u-\mathbf j/(en)$. With constant density, negligible [electrical resistivity](electric-charge.md#electrical-resistivity) and [electron](physics.md#electron) inertia, [Gaussian units](electromagnetism.md#gaussian-units) give $\mathbf j=c\nabla\times\mathbf B/(4\pi)$ and $\partial_t\mathbf B=\nabla\times[(\mathbf u-c\nabla\times\mathbf B/(4\pi en))\times\mathbf B]$. The [ion](chemistry.md#ion) velocity still satisfies the [magnetohydrodynamic momentum equation](#magnetohydrodynamic-momentum-equation). Neglecting that velocity gives [electron magnetohydrodynamics](#electron-magnetohydrodynamics), a further approximation rather than a synonym for the complete Hall system.

### Fast-time electron-MHD limit of Hall magnetohydrodynamics

↑ **Parent:** [Hall magnetohydrodynamics](#hall-magnetohydrodynamics)

For field amplitudes of order the guide field, the [ion](chemistry.md#ion) Lorentz-force response over time $\tau$ is $\Delta u/v_A=O(v_A\tau/l)\ll1$. The electron-current velocity is of order $v_Ad_i/l$, larger than a bulk velocity of order $v_A$. Thus the leading [Hall magnetohydrodynamics](#hall-magnetohydrodynamics) induction equation becomes the closed [electron magnetohydrodynamics](#electron-magnetohydrodynamics) equation, while [ions](chemistry.md#ion) remain fixed to leading order on this fast scale. The first nonzero [ion](chemistry.md#ion) response need not have zero acceleration. This limit retains the fast branch of [incompressible Hall-MHD wave dispersion](#incompressible-hall-mhd-wave-dispersion), not the slow branch; very oblique modes must separately satisfy the fast-time ordering.

### Incompressible Hall-MHD wave dispersion

↑ **Parent:** [Hall magnetohydrodynamics](#hall-magnetohydrodynamics)

For a uniform guide field, write the transverse perturbation in velocity units as $\mathbf b$. Linear momentum gives $\omega\mathbf u=-k_\parallel v_A\mathbf b$. Linear induction gives $\omega\mathbf b=-k_\parallel v_A\mathbf u+i k_\parallel v_Ad_i\mathbf k\times\mathbf b$. The [helicity decomposition of a transverse Fourier mode](special-relativity.md#helicity-decomposition-of-a-transverse-fourier-mode) then yields the displayed [dispersion relation](dispersion-relation.md). Its two positive frequency magnitudes are $|k_\parallel|v_A[\sqrt{1+(kd_i)^2/4}\pm kd_i/2]$, approaching the [Alfvén wave](ideal-magnetohydrodynamics.md#alfven-wave) frequency for $kd_i\ll1$. For $kd_i\gg1$, the fast branch is a [whistler wave](#whistler-wave) and the slow branch tends to $|k_\parallel|v_A/(kd_i)$.

## Electron magnetohydrodynamics

↑ **Parent:** [Magnetohydrodynamics](magnetohydrodynamics.md)

[Electron magnetohydrodynamics](#electron-magnetohydrodynamics) neglects [ion](chemistry.md#ion) motion and [electron](physics.md#electron) inertia while retaining transport of the [magnetic field](magnetic-field.md) by the [electron](physics.md#electron) current. At constant [electron](physics.md#electron) [number density](statistical-physics.md#number-density), $\mathbf u_e=-\mathbf J/(en)=-c\nabla\times\mathbf B/(4\pi en)$. Flux freezing in this [velocity](classical-mechanics.md#velocity) gives

$$
\partial_t\mathbf B=-\frac c{4\pi en}\nabla\times[(\nabla\times\mathbf B)\times\mathbf B].
$$

For a uniform guide field, the [solenoidal](multivariable-calculus.md#solenoidal-vector-field) linear equation implies $\omega^2=(cB_0/4\pi en)^2k_\parallel^2k^2$. With $v_A=B_0/\sqrt{4\pi nm_i}$ and $d_i=c\sqrt{m_i/(4\pi e^2n)}$, the coefficient is $cB_0/(4\pi en)=v_Ad_i$.

### Whistler wave

↑ **Parent:** [Electron magnetohydrodynamics](#electron-magnetohydrodynamics)

In the inertia-free, constant-density [electron magnetohydrodynamics](#electron-magnetohydrodynamics) model with uniform guide field $B_0\hat{\mathbf z}$, a transverse magnetic [plane wave](wave-function.md#plane-wave) obeys $\omega\mathbf b=i v_Ad_i k_\parallel\mathbf k\times\mathbf b$. The [helicity decomposition of a transverse Fourier mode](special-relativity.md#helicity-decomposition-of-a-transverse-fourier-mode) gives the displayed dispersive branches with opposite [circular polarizations](electromagnetic-wave.md#circular-polarization). This electron-current mode is called a whistler wave; see [Lyutikov's analysis of electron magnetohydrodynamics](https://arxiv.org/abs/1306.4544). Its pressure-free induction equation should not be identified with a general kinetic Alfvén model.

### Reduced electron magnetohydrodynamics

↑ **Parent:** [Electron magnetohydrodynamics](#electron-magnetohydrodynamics)

With $k_\parallel/k_\perp\sim\delta B/B_0\ll1$, define $b=\delta B_\parallel/B_0$ and $\delta\mathbf B_\perp/B_0=\hat{\mathbf z}\times\nabla_\perp\Psi/v_A$ to leading order. Let $\nabla_\parallel=\partial_z+\{\Psi,\cdot\}/v_A$, where $\{f,g\}=f_xg_y-f_yg_x$. The leading [electron](physics.md#electron) [velocities](classical-mechanics.md#velocity) are $\mathbf u_{e\perp}=v_Ad_i\hat{\mathbf z}\times\nabla_\perp b$ and $u_{e\parallel}=-d_i\nabla_\perp^2\Psi$. Substitution into frozen-in induction yields

$$
\partial_t\Psi=v_A^2d_i\nabla_\parallel b,\qquad \partial_tb=-d_i\nabla_\parallel\nabla_\perp^2\Psi.
$$

[Linearization](algebra.md#linearization) gives $\omega^2=v_A^2d_i^2k_\parallel^2k_\perp^2$, agreeing with the full [EMHD](#electron-magnetohydrodynamics) relation to leading anisotropic order. If $b$ varies along the guide field, an order-smaller perpendicular gradient correction restores exact solenoidality; the two-field representation is not an exact decomposition at arbitrary anisotropy.

## Stratified magneto-Coriolis wave

↑ **Parent:** [Magnetohydrodynamics](magnetohydrodynamics.md)

An incompressible [Boussinesq](geophysical-fluid-dynamics.md#boussinesq-approximation) fluid with uniform [magnetic field](magnetic-field.md), uniform vertical [rotation](riemannian-geometry.md#rotation-mathematics) and uniform temperature gradient supports waves combining [magnetic tension](#magnetic-tension), [Coriolis force](mathematical-physics.md#coriolis-force) and [buoyancy](fluid-mechanics.md#buoyancy). Put $K=|\mathbf k|$, $h^2=K^2-k_z^2$, $a^2=(\mathbf B\cdot\mathbf k)^2/(\mu_0\rho)$ and $H=g\alpha\beta$, with $\partial_zT_0=-\beta$. Eliminating [pressure](pressure.md) and the temperature and magnetic perturbations gives the displayed [dispersion relation](dispersion-relation.md) for nonzero frequencies. Stable thermal stratification has $H<0$. Clearing frequency denominators requires checking any resulting zero roots in the original equations; a stationary magnetostatic-buoyancy balance can exist independently of the propagating branches.

### Rapid-rotation slow magneto-Coriolis branch

↑ **Parent:** [Stratified magneto-Coriolis wave](#stratified-magneto-coriolis-wave)

For fixed wavevector with $k_z\ne0$, fixed nonzero [Alfvén frequency](ideal-magnetohydrodynamics.md#alfven-frequency) $a$, and $|\Omega|\to\infty$, the two roots in $X=\omega^2$ of the [stratified magneto-Coriolis wave](#stratified-magneto-coriolis-wave) polynomial have $X_f\sim4\Omega^2k_z^2/K^2$ and the displayed slow root. This follows from the sum of roots being $4\Omega^2k_z^2/K^2+O(1)$ and their product being $a^2(K^2a^2-Hh^2)/K^2$. The slow branch is oscillatory for $K^2a^2>Hh^2$ and growing or decaying for the reversed inequality. At equality its frequency vanishes and the original stationary equations must be used.

## Lehnert number

↑ **Parent:** [Magnetohydrodynamics](magnetohydrodynamics.md)

The Lehnert number compares an [Alfvén speed](ideal-magnetohydrodynamics.md#alfven-speed) to a rotation speed on length scale $L$. With $\mathrm{Le}\ll1$, magnetic-wave frequencies are small compared with the rotation frequency, allowing nearly [geostrophic flow](geophysical-fluid-dynamics.md#geostrophic-flow). Ideal weakly damped magnetic waves also require $\eta/L^2$ and $\nu/L^2$ to be small compared with their wave frequency; a small Lehnert number alone does not guarantee weak diffusion.

## Magnetohydrodynamic momentum equation

↑ **Parent:** [Magnetohydrodynamics](magnetohydrodynamics.md)

For constant [mass density](fluid-mechanics.md#density) $\rho$, [kinematic viscosity](dynamic-viscosity.md#kinematic-viscosity) $\nu$ and [magnetic permeability](maxwell-equations.md#permeability-electromagnetism) $\mu_0$, the incompressible momentum equation is

$$
\partial_t\mathbf u+(\mathbf u\cdot\nabla)\mathbf u=-\rho^{-1}\nabla p+(\mu_0\rho)^{-1}(\nabla\times\mathbf B)\times\mathbf B+\nu\nabla^2\mathbf u.
$$

It is the [Navier-Stokes equation](viscous-fluid-flow.md#navier-stokes-equation) with [Lorentz force density](relativistic-electromagnetism.md#lorentz-force-density). The magnetic force decomposes into [magnetic tension](#magnetic-tension) and a [magnetic pressure](#magnetic-pressure) gradient. A uniform streamwise pressure gradient need not make ordinary pressure independent of transverse coordinates.

## Resistive magnetohydrodynamics

↑ **Parent:** [Magnetohydrodynamics](magnetohydrodynamics.md)

[This section is present in another page, follow this link to view it.](resistive-magnetohydrodynamics.md)

## Magnetic diffusion

↑ **Parent:** [Magnetohydrodynamics](magnetohydrodynamics.md)

Finite [electrical conductivity](electric-charge.md#electrical-conductivity) permits resistive smoothing of a [magnetic field](magnetic-field.md). With uniform coefficients and no motion the field satisfies a diffusion equation; with motion the diffusion term supplements the curl of $\mathbf u\times\mathbf B$. The [magnetic Reynolds number](#magnetic-reynolds-number) compares these effects.

### Magnetic phase mixing under differential rotation

↑ **Parent:** [Magnetic diffusion](#magnetic-diffusion)

A nonuniform angular velocity $f(r)$ winds an azimuthal magnetic mode into phase $m(\phi-f(r)t)$. Its radial phase gradient grows as $-mt f'(r)$, creating small scales even when its ideal amplitude does not decay. The corresponding leading resistive damping rate is $\eta m^2t^2f'(r)^2$, so a local short-wavelength estimate gives damping factor $\exp[-\eta m^2f'(r)^2t^3/3]$. Hence [magnetic diffusion](#magnetic-diffusion) can become important at time $[\eta m^2f'^2]^{-1/3}$ although it is initially small. This is a local phase-mixing estimate, not a globally exact solution in a finite radial domain: boundary forcing, field stretching and spatial variation of $f'$ must also be retained there.

#### Exact quadratic-shear magnetic flux solution

↑ **Parent:** [Magnetic phase mixing under differential rotation](#magnetic-phase-mixing-under-differential-rotation)

For azimuthal flow $u_\phi=s(\Omega_0+\omega s^2)$, a planar [magnetic flux](magnetic-field.md#magnetic-flux) mode $s^mg(t)e^{im\phi-im\Omega_0t-is^2f(t)}$ obeys the [resistive induction equation](resistive-magnetohydrodynamics.md#resistive-induction-equation) if $\dot f=m\omega-4i\eta f^2$ and $\dot g/g=-4i\eta(m+1)f$. With $f(0)=0$ and $g(0)=1$, their solution is $f=(m\omega/\mu)\tanh\mu t$ and $g=(\cosh\mu t)^{-(m+1)}$. Choose $\operatorname{Re}\mu>0$. For positive $\eta,\omega$, the fixed-position field decays asymptotically at rate $(m+1)\sqrt{2\eta m\omega}$. [Differential rotation](astrophysical-fluid-dynamics.md#differential-rotation) creates small spatial scales, accelerating [magnetic diffusion](#magnetic-diffusion).

### Magnetic free-decay spectral bound

↑ **Parent:** [Magnetic diffusion](#magnetic-diffusion)

For a [solenoidal vector field](multivariable-calculus.md#solenoidal-vector-field) carrying current only in a conductor contained in a sphere of radius $R$, match the exterior field to a decaying potential field and include exterior [magnetic energy](electromagnetic-wave.md#magnetic-energy). The smallest free-decay [eigenvalue](linear-operator-theory.md#eigenvalue) of the enclosing sphere is $\pi^2/R^2$, from its dipolar poloidal mode. The corresponding variational estimate gives the displayed bound. Continuity and the usual insulating-interface magnetic conditions are part of the admissible field class. This bound is the diffusive ingredient in [Backus' necessary condition for dynamo action](resistive-magnetohydrodynamics.md#backus-necessary-condition-for-dynamo-action).

### Magnetic diffusivity

↑ **Parent:** [Magnetic diffusion](#magnetic-diffusion)

Magnetic diffusivity is the coefficient of [magnetic diffusion](#magnetic-diffusion). In a scalar-conductivity fluid with vacuum permeability and negligible [displacement current](maxwell-equations.md#displacement-current), $\eta_m=1/(\mu_0\sigma)$. Its dimensions are length squared per time, and a diffusion time on scale $L$ is $L^2/\eta_m$.

#### Magnetic Prandtl number

↑ **Parent:** [Magnetic diffusivity](#magnetic-diffusivity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Magnetic_Prandtl_number)

The magnetic Prandtl number compares [kinematic viscosity](dynamic-viscosity.md#kinematic-viscosity) with [magnetic diffusivity](#magnetic-diffusivity). It is the ratio of the viscous and magnetic diffusion coefficients; equivalently it is the [magnetic Reynolds number](#magnetic-reynolds-number) divided by the [Reynolds number](dynamic-viscosity.md#reynolds-number) when the same speed and length scale are used.

#### Turbulent magnetic diffusivity

↑ **Parent:** [Magnetic diffusivity](#magnetic-diffusivity)

Turbulent magnetic diffusivity is an effective transport coefficient produced by correlated small-scale [velocity](classical-mechanics.md#velocity) and [magnetic field](magnetic-field.md). It supplements microscopic [magnetic diffusivity](#magnetic-diffusivity) in a [mean-field dynamo](resistive-magnetohydrodynamics.md#mean-field-dynamo) description. Its identification requires a specified mean-field geometry and averaging procedure; in a planar flux problem, the correlation $\overline{wa'}=-\eta_tB_0f(z)$ describes transport relative to a prescribed uniform field.

##### Variance bound for planar turbulent magnetic transport

↑ **Parent:** [Turbulent magnetic diffusivity](#turbulent-magnetic-diffusivity)

For $\overline{wa'}=-\eta_tB_0f$, $\langle f\rangle=1$ and positive diffusivities, the [Zeldovich planar flux balance](resistive-magnetohydrodynamics.md#zeldovich-planar-flux-balance) gives $G=(\eta_t/\eta)B_0^2[1-(\eta_t/\eta)\operatorname{Var}(f)]$, where $G=\langle|\nabla a'|^2\rangle$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) and a [Poincaré inequality](sobolev-space.md#poincare-inequality) $\langle a'^2\rangle\leq d^2G/\pi^2$ give $\eta_t^2\operatorname{Var}(f)\leq\langle w^2\rangle d^2s(1-s)/\pi^2$, with $s=(\eta_t/\eta)\operatorname{Var}(f)\in[0,1]$. Maximizing $s(1-s)$ gives the displayed bound. Large turbulent-to-microscopic diffusivity therefore requires $f$ to be close to one in mean square, without guaranteeing pointwise uniformity.

## Magnetic Reynolds number

↑ **Parent:** [Magnetohydrodynamics](magnetohydrodynamics.md)

The magnetic Reynolds number compares field advection with resistive [magnetic diffusion](#magnetic-diffusion). With constant [electrical conductivity](electric-charge.md#electrical-conductivity) and vacuum permeability, magnetic diffusivity is $\eta_m=1/(\mu_0\sigma)$ and $\operatorname{Rm}=UL/\eta_m$. The ideal induction approximation applies when this ratio is large on the scales of interest.

## Moving-conductor Ohm law

↑ **Parent:** [Magnetohydrodynamics](magnetohydrodynamics.md)

In the nonrelativistic scalar-conductivity approximation, neglecting Hall and other nonideal electromotive effects, $\mathbf J=\sigma(\mathbf E+\mathbf u\times\mathbf B)$. The ideal finite-current limit gives $\mathbf E=-\mathbf u\times\mathbf B$ and hence the [ideal magnetohydrodynamic induction equation](ideal-magnetohydrodynamics.md#ideal-magnetohydrodynamic-induction-equation).

## Magnetoconvection

↑ **Parent:** [Magnetohydrodynamics](magnetohydrodynamics.md)

Magnetoconvection is thermal [convection](convection.md) coupled to the evolution and forces of a [magnetic field](magnetic-field.md). Conserved [magnetic flux](magnetic-field.md#magnetic-flux) can supply a slow field that must be retained along with the convective [complex amplitude](wave.md#complex-amplitude), rather than being eliminated into a single local [amplitude equation](bifurcation-theory.md#amplitude-equation).

### Three-mode porous magnetoconvection

↑ **Parent:** [Magnetoconvection](#magnetoconvection)

A [Galerkin method](partial-differential-equation.md#galerkin-method) using one convective [streamfunction](fluid-mechanics.md#stream-function) mode and two [Cartesian magnetic flux function](ideal-magnetohydrodynamics.md#cartesian-magnetic-flux-function) modes yields the displayed system. With $\alpha=\pi/\sqrt3$, use $\psi=4\sqrt2a\sin(\alpha x)\sin(\pi z)$ and $A=(3\sqrt2/\pi)b\sin(\alpha x)\cos(\pi z)+(\sqrt3/\pi)c\sin(2\alpha x)$, time $\tau=(4\pi^2/3)t$, $q=9Q/(16\pi^2)$ and $r=9R/(64\pi^4)$. The origin's planar trace is $\sigma(r-1)-\zeta$ and determinant $\sigma\zeta(1+q-r)$; the third [eigenvalue](linear-operator-theory.md#eigenvalue) is $-\zeta$. The stationary threshold is $r=1+q$, and the oscillatory threshold is $r=1+\zeta/\sigma$ when $q>\zeta/\sigma$. They meet in a symmetric double-zero point at $(q,r)=(\zeta/\sigma,1+\zeta/\sigma)$. Higher spatial harmonics generated by the quadratic terms are discarded, so this is a projected approximation rather than an exact invariant subspace of the original equations.

#### Cubic centre-manifold reduction of porous magnetoconvection

↑ **Parent:** [Three-mode porous magnetoconvection](#three-mode-porous-magnetoconvection)

For [three-mode porous magnetoconvection](#three-mode-porous-magnetoconvection), set $\mu=r-1-q$ and assume $0<q<\zeta/\sigma$. The transverse [eigenvalues](linear-operator-theory.md#eigenvalue) are negative. Centre-manifold invariance gives

$$
c=\frac{3a^2}{\zeta^2}+\cdots,\qquad
b=\frac a\zeta-\frac{\sigma\mu a}{\zeta(\zeta-\sigma q)}-\frac{3a^3}{\zeta^2(\zeta-\sigma q)}+\cdots.
$$

Substitution into the first equation gives the displayed positive linear and cubic coefficients. Thus the bifurcation is a [subcritical pitchfork bifurcation](bifurcation-theory.md#subcritical-pitchfork-bifurcation): the origin is stable for $\mu<0$ and unstable for $\mu>0$, while the small nonzero branches at $a^2=-\zeta^2\mu/(3q)$ are unstable. Simply setting $\dot b=0$ misses the time-derivative contribution responsible for the common factor $(1-\sigma q/\zeta)^{-1}$.

### Thermal-diffusion scaling of planar magnetoconvection

↑ **Parent:** [Magnetoconvection](#magnetoconvection)

Use depth $d$, time $d^2/\kappa$, stream-function scale $\kappa$, temperature perturbation scale $\Delta T$, and magnetic flux-function scale $B_0d$. With $\mathbf u=(-\psi_z,0,\psi_x)$, $\mathbf B=(-A_z,0,A_x)$ and $A=x+\chi$, advection is $J(\psi,f)=\psi_xf_z-\psi_zf_x$. The temperature background contributes $\psi_x$ to the heat equation and the imposed vertical field contributes $\psi_z$ to the perturbation induction equation. Taking the curl of the [magnetohydrodynamic momentum equation](#magnetohydrodynamic-momentum-equation) gives a magnetic term $\sigma\zeta QJ(A,\nabla^2A)$, where $\sigma=\nu/\kappa$, $\zeta=\eta/\kappa$, $R=g\alpha\Delta T d^3/(\nu\kappa)$ and $Q=B_0^2d^2/(\mu_0\rho\nu\eta)$.

### Quasistatic vertical-field magnetoconvection

↑ **Parent:** [Magnetoconvection](#magnetoconvection)

When the magnetic field supplies instantaneous damping rather than an evolving magnetic perturbation, the roll amplitudes obey a two-variable linear system with [trace](linear-algebra.md#matrix-trace) $-[s+\sigma(s+Q\pi^2/s)]<0$. Its [determinant](multilinear-algebra.md#determinant) vanishes at the displayed stationary threshold. Therefore its initial instability cannot be a [Hopf bifurcation](bifurcation-theory.md#hopf-bifurcation). This reduced model must not be confused with a three-variable magnetoconvection model carrying finite magnetic diffusivity and an additional oscillatory mode.

#### Cubic saturation of quasistatic magnetoconvection

↑ **Parent:** [Quasistatic vertical-field magnetoconvection](#quasistatic-vertical-field-magnetoconvection)

The primary roll and [temperature](temperature.md) modes force only a horizontally uniform [temperature](temperature.md) mode proportional to $\sin(2\pi z)$ at quadratic order. Its amplitude is $c=-\alpha ab/(8\pi)$. Its feedback on the primary [temperature](temperature.md) mode saturates [magnetoconvection](#magnetoconvection), giving the displayed positive squared amplitude above threshold. Thus a simple roll onset is a supercritical [pitchfork bifurcation](bifurcation-theory.md#pitchfork-bifurcation-normal-form) for every $Q\ge0$. The three-mode [Fourier truncation](partial-differential-equation.md#fourier-truncation) and full perturbation calculation agree through the cubic solvability condition because all forced quadratic modes are retained; this is not an assertion that the truncation gives an exact finite-amplitude PDE solution.

// Destination: dynamical-systems.bigb

### Five-mode vertical-field magnetoconvection

↑ **Parent:** [Magnetoconvection](#magnetoconvection)

A [Galerkin method](partial-differential-equation.md#galerkin-method) approximation can retain one roll [streamfunction](fluid-mechanics.md#stream-function) mode, two temperature modes and two magnetic-flux perturbation modes in vertical-field [magnetoconvection](#magnetoconvection). Projection onto these five modes, rather than pointwise equality of the truncated fields, gives a closed system of five [ordinary differential equations](differential-equation.md#ordinary-differential-equation). Products generate higher spatial harmonics that are discarded by orthogonal projection. The system has symmetry $(a,b,c,d,e)\mapsto(-a,-b,c,-d,e)$ and hence admits paired steady roll branches.

#### Conduction double-zero criterion for five-mode magnetoconvection

↑ **Parent:** [Five-mode vertical-field magnetoconvection](#five-mode-vertical-field-magnetoconvection)

The conduction linearization has two negative [eigenvalues](linear-operator-theory.md#eigenvalue) and a cubic factor $s^3+As^2+Bs+C$, where $A=\sigma+1+\zeta$, $B=\sigma(1-r)+\sigma\zeta(1+q)+\zeta$, $C=\sigma\zeta(1+q-r)$. A double zero requires $B=C=0$, giving the displayed [Bogdanov–Takens bifurcation](bifurcation-theory.md#bogdanov-takens-bifurcation) location for $0<\zeta<1$. The remaining cubic eigenvalue is $-A$. The imaginary-pair condition $AB=C$ yields $r_H=(\sigma+\zeta)(1+\zeta)/\sigma+\zeta(\sigma+\zeta)q/(\sigma+1)$ and $\omega^2=\sigma\zeta(1-\zeta)q/(\sigma+1)-\zeta^2$. Thus the oscillatory onset exists precisely for $q>q_*$ when $0<\zeta<1$.

#### Stationary branch of five-mode magnetoconvection

↑ **Parent:** [Five-mode vertical-field magnetoconvection](#five-mode-vertical-field-magnetoconvection)

For positive diffusivity ratio $\zeta$ and $0<\varphi<4$, define $\mu=(4-\varphi)\zeta^2/\varphi$. The nonzero steady branch has $b=a/(1+a^2)$, $c=a^2/(1+a^2)$, $d=\mu a/[\zeta(\mu+a^2)]$, and $e=a^2/(\mu+a^2)$. Substitution yields the displayed branch through $r=1+q$. Its initial slope in $a^2$ has the sign of $\varphi q(2-\varphi)+(4-\varphi)\zeta^2(1+q)$. Positive slope is a [supercritical pitchfork bifurcation](bifurcation-theory.md#supercritical-pitchfork-bifurcation) direction, negative slope a [subcritical pitchfork bifurcation](bifurcation-theory.md#subcritical-pitchfork-bifurcation) direction. This geometric criterion alone does not assert stability against every perturbation.

##### Pitchfork reversal near geometric ratio two in magnetoconvection

↑ **Parent:** [Stationary branch of five-mode magnetoconvection](#stationary-branch-of-five-mode-magnetoconvection)

Put $m=(4-\varphi)\zeta^2/\varphi$. The derivative of the [stationary branch of five-mode magnetoconvection](#stationary-branch-of-five-mode-magnetoconvection) at $a^2=0$ is $r_2=1+q+q(2-\varphi)/m$. For fixed positive $q$ and small $\zeta$, it changes from a forward to a backward [pitchfork bifurcation](bifurcation-theory.md#pitchfork-bifurcation-normal-form) direction at the displayed value. Expanding the exact numerator $q\varphi(2-\varphi)+(4-\varphi)\zeta^2(1+q)$ gives this result. The expansion in amplitude requires $a^2\ll m$; branch direction alone does not determine stability against all other modes.

### Horizontal-field magnetoconvection dispersion relation

↑ **Parent:** [Magnetoconvection](#magnetoconvection)

For a unit-depth [Boussinesq](geophysical-fluid-dynamics.md#boussinesq-approximation) layer with [stress-free boundary conditions](viscous-fluid-flow.md#stress-free-boundary-condition), fixed boundary temperatures, imposed field along $y$, and horizontal magnetic perturbations at the boundaries, put $a_h^2=k^2+m^2$ and $\Lambda=a_h^2+\pi^2$. Poloidal vertical velocity, temperature and vertical field proportional to $e^{st+ikx+imy}\sin\pi z$ have amplitudes satisfying

$$
\Lambda(s/\sigma+\Lambda)W=Ra_h^2\Theta+\zeta Qim\Lambda C,\qquad
(s+\Lambda)\Theta=W,\qquad(s+\zeta\Lambda)C=imW.
$$

The [determinant](multilinear-algebra.md#determinant) gives the stated [dispersion relation](dispersion-relation.md). Here $\sigma$ is the [Prandtl number](heat.md#prandtl-number), $\zeta$ the [magnetic-to-thermal diffusivity ratio](#magnetic-to-thermal-diffusivity-ratio), $Q$ the [Chandrasekhar number](#chandrasekhar-number) and $R$ the [Rayleigh number](geophysics.md#rayleigh-number). The steady neutral curve is $R=\Lambda^3/a_h^2+Qm^2\Lambda/a_h^2$.

// Target: fluid-mechanics.bigb

#### Strong-field steady magnetoconvection varying along the field

↑ **Parent:** [Horizontal-field magnetoconvection dispersion relation](#horizontal-field-magnetoconvection-dispersion-relation)

Restrict the [horizontal-field magnetoconvection dispersion relation](#horizontal-field-magnetoconvection-dispersion-relation) to $k=0$, $x=m^2>0$. The steady neutral curve becomes $R=\pi^2Q+(Q+3\pi^2)x+x^2+3\pi^4+\pi^6/x$. Its unique minimum satisfies $x^2(Q+3\pi^2+2x)=\pi^6$, since $R''(x)=2+2\pi^6/x^3>0$. Expanding at large [Chandrasekhar number](#chandrasekhar-number) gives $x\sim\pi^3Q^{-1/2}$ and the stated [asymptotic expansion](asymptotic-expansion.md). Unlike field-aligned rolls, these disturbances bend the field, and their stationary threshold grows with field strength.

// Target: fluid-mechanics.bigb

#### Magnetic-field-aligned rolls evade steady magnetic inhibition

↑ **Parent:** [Horizontal-field magnetoconvection dispersion relation](#horizontal-field-magnetoconvection-dispersion-relation)

At a fixed horizontal [wavenumber](wave-equation.md#wavenumber) magnitude, the steady neutral curve in the [horizontal-field magnetoconvection dispersion relation](#horizontal-field-magnetoconvection-dispersion-relation) is minimized by $m=0$. The disturbance is then constant along the imposed [magnetic field](magnetic-field.md); it induces no field bending and incurs no [magnetic tension](#magnetic-tension) penalty. Minimizing $(k^2+\pi^2)^3/k^2$ gives the displayed stationary threshold for every $Q\geq0$. These [convection rolls](convection.md#convection-roll) have axes parallel to the imposed field. This assertion concerns steady onset.

// Target: fluid-mechanics.bigb

### Magnetic-to-thermal diffusivity ratio

↑ **Parent:** [Magnetoconvection](#magnetoconvection)

The ratio of [magnetic diffusivity](#magnetic-diffusivity) $\eta$ to [thermal diffusivity](heat.md#thermal-diffusivity) $\kappa$ controls their relative relaxation times. In nonrotating vertical-field [magnetoconvection](#magnetoconvection), oscillatory linear onset in the simple stress-free layer requires $0<\zeta<1$, so thermal perturbations diffuse faster than magnetic perturbations. This is distinct from the [magnetic Prandtl number](#magnetic-prandtl-number), $\nu/\eta$.

### Subcritical magnetoconvection

↑ **Parent:** [Magnetoconvection](#magnetoconvection)

Subcritical magnetoconvection means finite-amplitude [convection](convection.md) on the stable side of the linear conductive-state threshold. At large [magnetic Reynolds number](#magnetic-reynolds-number), [flux expulsion](resistive-magnetohydrodynamics.md#flux-expulsion) can reduce interior magnetic inhibition enough to sustain a nonlinear convective cell even when infinitesimal disturbances decay in the unredistributed imposed field. Stable subcritical states can produce hysteresis and [magnetic flux separation](#magnetic-flux-separation). A schematic saturated [amplitude equation](bifurcation-theory.md#amplitude-equation) $\dot A=\mu A+c|A|^2A-d|A|^4A$, $c,d>0$, has an unstable lower branch and stable upper radial branch for $-c^2/(4d)<\mu<0$, coexisting with stable $A=0$. This illustrates bistability; it is not a derivation of coefficients for all magnetoconvection geometries.

### Magnetic flux separation

↑ **Parent:** [Magnetoconvection](#magnetoconvection)

In nonlinear [magnetoconvection](#magnetoconvection), magnetic flux separation is coexistence of weak-field regions with vigorous broad [convection](convection.md) and strong-field regions with inhibited or small-scale [convection](convection.md). [Flux expulsion](resistive-magnetohydrodynamics.md#flux-expulsion) provides a mechanism for segregation. Conserved mean vertical [magnetic flux](magnetic-field.md#magnetic-flux) implies $fB_c+(1-f)B_q=B_0$ for an idealized two-region area fraction $f$. Weak field in convecting regions therefore requires enhanced field elsewhere. The existence and stability of the segregated state depend on parameters and boundaries.

### Oblique-field plane-wave magnetoconvection

↑ **Parent:** [Magnetoconvection](#magnetoconvection)

In thermal-diffusion units, let an imposed field point along $\mathbf c=(\sin\alpha,0,\cos\alpha)$ and consider a [Fourier mode](fourier-analysis.md#fourier-mode) of wavevector $(k,0,m)$. Put $q=k^2+m^2$ and $d=k\sin\alpha+m\cos\alpha$. The growth exponent $s$ of its buoyant branch satisfies

$$
q(s+q)\left[(s/\sigma+q)(s+\zeta q)+Q\zeta d^2\right]=Rk^2(s+\zeta q),
$$

where $\sigma$ is the [Prandtl number](heat.md#prandtl-number), $\zeta$ the magnetic-to-thermal diffusivity ratio, $Q$ the [Chandrasekhar number](#chandrasekhar-number), and $R$ the [Rayleigh number](geophysics.md#rayleigh-number). The [resistive induction equation](resistive-magnetohydrodynamics.md#resistive-induction-equation) gives $\widehat{\mathbf b}=id\widehat{\mathbf u}/(s+\zeta q)$, and thermal transport gives $\widehat\theta=\widehat w/(s+q)$. Projecting momentum perpendicular to the wavevector removes pressure; the vertical component of the projected buoyancy is $R(k^2/q)\widehat\theta$. Substitution gives the displayed polynomial. The stationary neutral curve is $R=q^3/k^2+Qqd^2/k^2$. No vertical boundary conditions are imposed in this plane-wave calculation.

#### Field-independent stationary threshold in oblique magnetoconvection

↑ **Parent:** [Oblique-field plane-wave magnetoconvection](#oblique-field-plane-wave-magnetoconvection)

At inclination $\alpha=\arctan\sqrt2$ and vertical wavenumber one, the nonmagnetic minimizing wavenumber $k=-1/\sqrt2$ also satisfies $\mathbf c\cdot\mathbf k=0$. The stationary threshold is the sum of $F(k)\geq27/4$ and a nonnegative magnetic penalty that vanishes there. Therefore $k_c=-1/\sqrt2$ and $R_c=27/4$ for every $Q\geq0$. The selected disturbance is constant along the imposed field, so the linear [resistive induction equation](resistive-magnetohydrodynamics.md#resistive-induction-equation) produces no magnetic perturbation and there is no field-line tension penalty.

#### Wavenumber selection in oblique-field magnetoconvection

↑ **Parent:** [Oblique-field plane-wave magnetoconvection](#oblique-field-plane-wave-magnetoconvection)

For fixed vertical wavenumber one, write the stationary threshold as $F(k)+QG(k)$, with $F=(1+k^2)^3/k^2$ and $G=(1+k^2)(\cos\alpha+k\sin\alpha)^2/k^2$. The nonmagnetic minima are $k=\pm1/\sqrt2$ with $F=27/4$; a small positive field selects the negative one. Expanding the stationarity condition gives $k_c=a-QG'(a)/F''(a)+O(Q^2)$, $a=-1/\sqrt2$, and

$$
R_c=\frac{27}{4}+3Q(\cos\alpha-\sin\alpha/\sqrt2)^2-\frac{G'(a)^2}{2F''(a)}Q^2+O(Q^3).
$$

For large $Q$, the magnetic penalty forces $k$ toward its unique zero $b=-\cot\alpha$. Since $G''(b)>0$, $k_c=b-F'(b)/[QG''(b)]+O(Q^{-2})$ and $R_c=\csc^6\alpha/\cot^2\alpha-F'(b)^2/[2QG''(b)]+O(Q^{-2})$. Thus strongly magnetized rolls align their wavevector perpendicular to the imposed field, rather than continuing to raise their stationary threshold proportionally to field strength.

### Vertical-field magnetoconvection dispersion relation

↑ **Parent:** [Magnetoconvection](#magnetoconvection)

For a stress-free, fixed-temperature layer with vertical magnetic perturbation at its boundaries, take vertical velocity and temperature proportional to $\sin\pi z$, vertical magnetic perturbation proportional to $\cos\pi z$, and horizontal magnetic perturbations proportional to $\sin\pi z$. With $s=k^2+\pi^2$, the vertical velocity, temperature and magnetic amplitudes form a three-variable linear system whose determinant is the stated polynomial. The [Prandtl number](heat.md#prandtl-number) is $\sigma$, magnetic-to-thermal diffusivity ratio is $\zeta$, and field strength is the [Chandrasekhar number](#chandrasekhar-number) $Q$. The steady marginal curve is $R^{(e)}=[s^3+Q\pi^2s]/k^2$.

#### Three-amplitude vertical-field magnetoconvection

↑ **Parent:** [Vertical-field magnetoconvection dispersion relation](#vertical-field-magnetoconvection-dispersion-relation)

For one stress-free planar roll mode, thermal-time rescaling reduces the linear dynamics to $a'=\sigma(-a+rb-\zeta qc)$, $b'=a-b$, $c'=a-\zeta c$. Its characteristic polynomial is $(s+\sigma)(s+1)(s+\zeta)-\sigma r(s+\zeta)+\sigma\zeta q(s+1)$. For $\sigma,\zeta>0$ and $q\ge0$, steady marginality is $r_s=1+q$. Oscillatory marginality is $r_H=(\sigma+\zeta)(1+\zeta)/\sigma+\zeta(\sigma+\zeta)q/(\sigma+1)$, with $\omega_H^2=\zeta[\sigma(1-\zeta)q/(\sigma+1)-\zeta]$. A genuine [Hopf bifurcation](bifurcation-theory.md#hopf-bifurcation) onset requires $\omega_H^2>0$; a formal imaginary-root formula with negative frequency squared is not an oscillation. The [Routh-Hurwitz stability criterion](dynamical-systems.md#routh-hurwitz-stability-criterion) selects the first crossing, while nonlinear coefficients determine criticality.

#### Exact critical Rayleigh relation for vertical-field magnetoconvection

↑ **Parent:** [Vertical-field magnetoconvection dispersion relation](#vertical-field-magnetoconvection-dispersion-relation)

At the minimum of the steady [vertical-field magnetoconvection dispersion relation](#vertical-field-magnetoconvection-dispersion-relation), stationarity gives $R_c=2(k_c^2+\pi^2)^3/\pi^2$. With nonmagnetic value $R_0=27\pi^4/4$, eliminating the critical [wavenumber](wave-equation.md#wavenumber) gives the stated relation and $k_c^2=\pi^2[\tfrac32(R_c/R_0)^{1/3}-1]$. These hold for every nonnegative [Chandrasekhar number](#chandrasekhar-number), including its zero-field limit.

#### Strong-field wavenumber selection in magnetoconvection

↑ **Parent:** [Vertical-field magnetoconvection dispersion relation](#vertical-field-magnetoconvection-dispersion-relation)

Both steady and oscillatory neutral curves have the form $R=C(k^2+p)^3/k^2+DQp(k^2+p)/k^2$, with $p=\pi^2$. Their exact minimizing condition is $x^2(2x+3p)=p^3+(D/C)Qp^2$, where $x=k^2$. For fixed positive coefficients and large [Chandrasekhar number](#chandrasekhar-number), $x\sim[Dp^2Q/(2C)]^{1/3}$ and $R_{\rm min}=DpQ+3C^{1/3}(Dp^2Q/2)^{2/3}+O(Q^{1/3})$. The optimum balances transverse diffusion against the magnetic penalty, leading to increasingly narrow rolls.

#### Oscillatory marginality in vertical-field magnetoconvection

↑ **Parent:** [Vertical-field magnetoconvection dispersion relation](#vertical-field-magnetoconvection-dispersion-relation)

A nonzero imaginary root of the [vertical-field magnetoconvection dispersion relation](#vertical-field-magnetoconvection-dispersion-relation) requires $0<\zeta<1$ and $Q>\zeta(1+\sigma)s^2/[\sigma(1-\zeta)\pi^2]$. Its marginal curve is $R^{(o)}=Cs^3/k^2+DQ\pi^2s/k^2$, with $C=(\sigma+\zeta)(1+\zeta)/\sigma$ and $D=\zeta(\sigma+\zeta)/(1+\sigma)$. A formal minimum of that algebraic curve is a physical oscillatory threshold only if the frequency squared there is positive.

##### Steady-Hopf merger in vertical-field magnetoconvection

↑ **Parent:** [Oscillatory marginality in vertical-field magnetoconvection](#oscillatory-marginality-in-vertical-field-magnetoconvection)

For thermal-time [magnetoconvection](#magnetoconvection), a physical oscillatory neutral mode has $\omega^2=\sigma(1-\zeta)Q_\kappa\pi^2/(1+\sigma)-\zeta^2(k^2+\pi^2)^2>0$. The steady and oscillatory neutral curves meet when this frequency tends to zero. Thus $0<\zeta<1$ is necessary and the displayed relation locates the merger. A formal oscillatory-curve minimum with negative frequency squared is not a physical onset.

###### Merger at a magnetoconvection neutral-curve minimum

↑ **Parent:** [Steady-Hopf merger in vertical-field magnetoconvection](#steady-hopf-merger-in-vertical-field-magnetoconvection)

At a steady-curve minimum, differentiation and the [steady-Hopf merger in vertical-field magnetoconvection](#steady-hopf-merger-in-vertical-field-magnetoconvection) give the first displayed wavenumber. At an oscillatory-curve minimum they give the second. For fixed positive [Prandtl number](heat.md#prandtl-number) $\sigma$ and large $Q_\kappa$, the corresponding merger diffusivity deficits are $1-\zeta_s\sim[(1+\sigma)/\sigma](\pi^2/(4Q_\kappa))^{1/3}$ and $1-\zeta_o\sim[(1+\sigma)\pi^2/(16\sigma Q_\kappa)]^{1/3}$. The two parameter surfaces are distinct: coincidence of neutral curves at one wavenumber does not imply coincidence of their minimizing wavenumbers.

### Chandrasekhar number

↑ **Parent:** [Magnetoconvection](#magnetoconvection)

For an imposed field $B_0$ in a layer of depth $d$, the [Chandrasekhar number](#chandrasekhar-number) compares magnetic tension with viscous and magnetic-diffusive effects. Here $\eta$ is [magnetic diffusivity](#magnetic-diffusivity) and $\nu$ is [kinematic viscosity](dynamic-viscosity.md#kinematic-viscosity). In thermal-diffusion units the linear magnetic-force coefficient is $Q\zeta$, where $\zeta=\eta/\kappa$ and $\kappa$ is [thermal diffusivity](heat.md#thermal-diffusivity).

#### Thermal-diffusion magnetic-field parameter

↑ **Parent:** [Chandrasekhar number](#chandrasekhar-number)

With [thermal diffusivity](heat.md#thermal-diffusivity) $\kappa$ and [magnetic diffusivity](#magnetic-diffusivity) $\eta$, the standard [Chandrasekhar number](#chandrasekhar-number) uses $\nu\eta$ in its denominator. A thermal-diffusion alternative uses $\nu\kappa$ and is $\zeta=\eta/\kappa$ times the standard parameter. In thermal-time [magnetoconvection](#magnetoconvection) equations, the linear magnetic-force coefficient is $\sigma Q_\kappa=\sigma\zeta Q_{\mathrm{Ch}}$. Specifying the convention prevents a missing diffusivity factor in a dispersion relation.

### Convection amplitude coupled to a conserved field

↑ **Parent:** [Magnetoconvection](#magnetoconvection)

A representative scaled amplitude model has complex $A$ and real $B$ with

$$
A_T=A+A_{XX}-A|A|^2-AB,\qquad B_T=\sigma B_{XX}+\mu(|A|^2)_{XX},\qquad\sigma>0.
$$

[Periodic boundary conditions](differential-equation.md#periodic-boundary-conditions) conserve $\int B\,dX$, because the right-hand side is a total second derivative. The slow field can change long-wave [convection roll](convection.md#convection-roll) stability and permit localized pulses. For zero mean $B$, the uniform [convection rolls](convection.md#convection-roll) are $A=Re^{iqX}$, $R^2=1-q^2$, $B=0$.

#### Localized pulse of a conserved-field convection model

↑ **Parent:** [Convection amplitude coupled to a conserved field](#convection-amplitude-coupled-to-a-conserved-field)

For a real steady amplitude and zero-mean field, twice integrating the field equation yields $B=\kappa(\langle A^2\rangle-A^2)$, $\kappa=\mu/\sigma$. The [amplitude equation](bifurcation-theory.md#amplitude-equation) becomes $A''+(1-\kappa\langle A^2\rangle)A+(\kappa-1)A^3=0$. Using $(R\operatorname{sech}cX)''=c^2A-2c^2A^3/R^2$ gives $\kappa\langle A^2\rangle=1+c^2$ and $R^2=2c^2/(\kappa-1)$, requiring $\kappa>1$. Its finite-window mean is $2R^2\tanh(cL/2)/(cL)$. For $cL\gg1$, consistency gives $c+c^{-1}=4\kappa/[L(\kappa-1)]$. The leading roots coalesce at $c=1$; for $L>2$ the leading upper parameter limit is $\kappa\leq L/(L-2)$, while retaining the finite-window factor makes the necessary inequality strict. The isolated sech profile has an exponentially small derivative mismatch on a periodic interval, so exact periodic tails need correction. For $L\leq2$ the algebra supplies no finite upper bound of this form.

#### Conserved-field sideband dispersion relation

↑ **Parent:** [Convection amplitude coupled to a conserved field](#convection-amplitude-coupled-to-a-conserved-field)

Linearize around $A=Re^{iqX}$ and write $r=R^2>0$. For sideband [wavenumber](wave-equation.md#wavenumber) $l$, the sum and difference of the two amplitude sidebands, together with the field amplitude $b$, evolve under

$$
M_l=\begin{pmatrix}-l^2-2r&-2ql&-2\\-2ql&-l^2&0\\-\mu r l^2&0&-\sigma l^2\end{pmatrix}.
$$

Expanding $\det(\lambda I-M_l)$ gives

$$
(\lambda+\sigma l^2)[(\lambda+l^2)(\lambda+l^2+2r)-4q^2l^2]-2\mu r l^2(\lambda+l^2)=0.
$$

At $l=0$, the [eigenvalues](linear-operator-theory.md#eigenvalue) are $-2r,0,0$; the field's constant mode must be removed if its mean is prescribed. Nonzero long-wave field modes are still dynamically active.

##### Long-wave instability with a conserved mean field

↑ **Parent:** [Conserved-field sideband dispersion relation](#conserved-field-sideband-dispersion-relation)

Putting $\lambda=l^2\nu$ into the sideband cubic and retaining $l^4$ gives

$$
r\nu^2-[(\mu-\sigma-1)r+2q^2]\nu-[(\mu-\sigma)r+2\sigma q^2]=0.
$$

For $r=1-q^2>0$, $\mu/\sigma>(1-3q^2)/(1-q^2)$ makes the constant coefficient negative. There is a positive real $\nu$, so sufficiently small nonzero $l$ grows. On a finite period $L$, however, only $l=2\pi j/L$ are allowed. For $q=0$, $\mu=2$, $\sigma=1$, $L=1$, every nonzero allowed mode has negative growth rates despite this long-wave inequality. Thus an arbitrarily-small-wave-number conclusion cannot be asserted without the domain-size qualification.

## Magnetic buoyancy instability

↑ **Parent:** [Magnetohydrodynamics](magnetohydrodynamics.md)

A [magnetic buoyancy instability](#magnetic-buoyancy-instability) is a gravitational instability of a magnetized stratified fluid in which displacements of the gas and [magnetic field](magnetic-field.md) can release [Newtonian gravitational potential energy](newton-s-law-of-universal-gravitation.md#newtonian-gravitational-potential-energy). [Magnetic pressure](#magnetic-pressure) supports part of the weight. Both interchange displacements and undular displacements can enter this broad category; [Parker instability](#parker-instability) is the undular mechanism involving drainage along bent [magnetic field lines](magnetic-field.md#magnetic-field-line).

### Isothermal interchange criterion for magnetic buoyancy

↑ **Parent:** [Magnetic buoyancy instability](#magnetic-buoyancy-instability)

A horizontal [flux tube](magnetic-field.md#flux-tube) displaced without bending preserves $B/\rho$ by [magnetic flux freezing](ideal-magnetohydrodynamics.md#magnetic-flux-freezing). If thermal exchange keeps its temperature equal to its new surroundings, lateral [magnetic pressure](#magnetic-pressure) balance gives $(c_T^2+v_A^2)(\rho_i'-\rho')=\rho B(B/\rho)'/\mu_0$. Here $c_T^2=p/\rho$, $v_A^2=B^2/(\mu_0\rho)$, and primes denote the response to a small vertical displacement from an equilibrium. Its linear [buoyancy](fluid-mechanics.md#buoyancy) acceleration is $-gB(B/\rho)'\xi/[\mu_0(c_T^2+v_A^2)]$. Thus local interchange is unstable when $B(B/\rho)'<0$, equivalently $(B^2/\rho^2)'<0$. This fast-thermal-exchange criterion differs from the adiabatic [localized interchange criterion for a magnetized atmosphere](#localized-interchange-criterion-for-a-magnetized-atmosphere).

### Localized interchange criterion for a magnetized atmosphere

↑ **Parent:** [Magnetic buoyancy instability](#magnetic-buoyancy-instability)

For disturbances constant along the horizontal [magnetic field](magnetic-field.md), the minimized energy [density](fluid-mechanics.md#density) is $\rho g[-(\ln\rho)'-\rho g/(\gamma p+C)]|\xi_z|^2$. If its coefficient is nonnegative everywhere, the full energy is nonnegative. If it is strictly negative at a point of a smooth equilibrium, a compactly supported vertical displacement in a neighbouring interval gives negative energy. These interchange motions compress gas and [magnetic pressure](#magnetic-pressure) together.

### Parker instability

↑ **Parent:** [Magnetic buoyancy instability](#magnetic-buoyancy-instability)

[Parker instability](#parker-instability) is an undular [magnetic buoyancy instability](#magnetic-buoyancy-instability) of a gravitationally stratified atmosphere supported partly by [magnetic pressure](#magnetic-pressure). A bent horizontal [magnetic field](magnetic-field.md) can permit gas to drain along its [magnetic field lines](magnetic-field.md#magnetic-field-line), leaving buoyant rising regions. [Magnetic tension](#magnetic-tension) resists bending, so wavelengths and [boundary conditions](differential-equation.md#boundary-condition) affect the instability threshold. For a [magnetized isothermal atmosphere](magnetic-field.md#magnetized-isothermal-atmosphere), the unrestricted-wavevector threshold is given by the [magnetic buoyancy energy criterion](#magnetic-buoyancy-energy-criterion).

#### Long-wavelength undular magnetic buoyancy criterion

↑ **Parent:** [Parker instability](#parker-instability)

At nonzero along-field wavenumber, put $q=ik_y\xi_y$, $P=\gamma p$ and $C=B^2/\mu_0$. After [pressure](pressure.md) minimization the energy [density](fluid-mechanics.md#density) completes to $CP/(P+C)|q-\rho g\xi_z/P|^2+[Ck_y^2-g\rho'-\rho^2g^2/P]|\xi_z|^2$. Choosing the square to vanish and then taking a sufficiently small nonzero $k_y$ gives negative energy exactly when the displayed strict criterion holds somewhere. A fixed prescribed wavenumber retains the stabilizing $Ck_y^2$ tension term; the criterion asserts existence of an allowed nonzero wavenumber. The associated along-field displacement lets material drain while [magnetic flux](magnetic-field.md#magnetic-flux) bends.

#### Magnetic buoyancy energy criterion

↑ **Parent:** [Parker instability](#parker-instability)

For the [magnetized isothermal atmosphere](magnetic-field.md#magnetized-isothermal-atmosphere), set $a=1/(2H)$, $s=v_s^2>0$, $b=v_a^2>0$ and $\Delta=ik_x\xi_x+ik_y\xi_y+(ik_z+a)\xi_z$. After weighting the displacement by $e^{z/(2H)}$, the restoring [Hermitian matrix](hilbert-space.md#hermitian-operator) $\mathsf K$ satisfies

$$
\boldsymbol\xi^\dagger\mathsf K\boldsymbol\xi=
s\left|\Delta-\frac g{s}\xi_z\right|^2+
b\left|ik_x\xi_x+(ik_z+a)\xi_z\right|^2+
bk_y^2(|\xi_x|^2+|\xi_z|^2)+
\left(\frac gH-\frac{g^2}{s}\right)|\xi_z|^2.
$$

Thus $gH\leq s$ makes the form nonnegative for every [wavevector](elasticity-physics.md#wavevector). If $gH>s$, choose $k_z=0$, $k_x\ne0$, $\xi_z=1$, $\xi_x=-a/(ik_x)$ and $\xi_y=g/(sik_y)$. The squares vanish, and sufficiently small nonzero $k_y$ gives a negative form. The [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient) proves instability when these wavelengths are admissible. Since $s=\gamma c_s^2$ and $\beta=2c_s^2/b$, the condition is precisely $\beta(\gamma-1)<1$.

##### Short transverse wavelength limit for magnetic buoyancy

↑ **Parent:** [Magnetic buoyancy energy criterion](#magnetic-buoyancy-energy-criterion)

For a horizontal field, set $C=B^2/\mu_0$. Static force balance gives $\delta\Pi=\rho g\xi_z-(\gamma p+C)\nabla\cdot\xi+Cik_y\xi_y$. Given smooth compactly supported vertical and along-field displacements, the displayed choice makes total-pressure perturbation zero while $\xi_x=O(k_x^{-1})$. The nonnegative [pressure](pressure.md) and transverse-tension terms vanish as $|k_x|\to\infty$. This constructs the infimum needed for the [magnetohydrodynamic energy principle](ideal-magnetohydrodynamics.md#magnetohydrodynamic-energy-principle); a strictly negative limit is already negative at some finite wavenumber.

## Poloidal magnetic field

↑ **Parent:** [Magnetohydrodynamics](magnetohydrodynamics.md)

A poloidal [magnetic field](magnetic-field.md) lies in meridional planes through the symmetry axis, in contrast to a [toroidal magnetic field](#toroidal-magnetic-field). For an [axisymmetric vector field](multivariable-calculus.md#axisymmetric-vector-field), it is represented by a [poloidal magnetic flux function](ideal-magnetohydrodynamics.md#poloidal-magnetic-flux-function) as $\mathbf B_p=R^{-1}\nabla\Psi\times\mathbf e_\phi$.

## Magnetic pressure

↑ **Parent:** [Magnetohydrodynamics](magnetohydrodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Magnetic_pressure)

Magnetic pressure is the isotropic part of magnetic stress. It is $p_B=B^2/(2\mu_0)$ in SI units and $B^2/(8\pi)$ in Gaussian units.

### Magnetic pressure discontinuity in an isothermal atmosphere

↑ **Parent:** [Magnetic pressure](#magnetic-pressure)

Two uniform horizontal [magnetic fields](magnetic-field.md) on either side of a horizontal interface exert no bulk force, but their [magnetic pressures](#magnetic-pressure) differ. For a common-temperature [isothermal atmosphere](statistical-physics.md#isothermal-atmosphere) with sound-speed squared $c_T^2=\mathcal RT_0$ and gravity $g$, [hydrostatic equilibrium](statistical-physics.md#hydrostatic-equilibrium) gives $p_i=c_T^2\rho_i$ and $p_i(z)=p_i(0)e^{-z/H}$, $H=c_T^2/g$. Continuity of [magnetohydrodynamic total pressure](#magnetohydrodynamic-total-pressure) gives the displayed density jump. A stronger field below means denser gas above, supplying a [Rayleigh-Taylor instability](continuum-mechanics.md#rayleigh-taylor-instability) even though each half-space is hydrostatic.

// Target: continuum-mechanics.bigb

### Magnetohydrodynamic total pressure

↑ **Parent:** [Magnetic pressure](#magnetic-pressure)

The [magnetohydrodynamic total pressure](#magnetohydrodynamic-total-pressure) is $\Pi=p+B^2/(2\mu_0)$, the sum of gas [pressure](pressure.md) and [magnetic pressure](#magnetic-pressure). The remaining [Lorentz force](relativistic-electromagnetism.md#lorentz-force) is [magnetic tension](#magnetic-tension), so this scalar does not include the entire magnetic stress.

## Magnetic tension

↑ **Parent:** [Magnetohydrodynamics](magnetohydrodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Magnetic_tension)

Magnetic tension is the restoring stress associated with bending magnetic field lines. In a divergence-free field, the Lorentz-force density splits into a magnetic-pressure gradient and the tension term $(\mathbf B\mathbin\cdot\nabla)\mathbf B/\mu_0$ in SI units.

## Toroidal magnetic field

↑ **Parent:** [Magnetohydrodynamics](magnetohydrodynamics.md)

A toroidal magnetic field points in the azimuthal direction around a chosen symmetry axis. Its curved field lines exert inward magnetic tension $-B_\phi^2/(\mu_0R)$ in cylindrical geometry.

### Toroidal magnetic-field winding equation

↑ **Parent:** [Toroidal magnetic field](#toroidal-magnetic-field)

In axisymmetric [ideal magnetohydrodynamics](ideal-magnetohydrodynamics.md), $\Omega=u_\phi/R$ is the material angular velocity. Cylindrical basis-vector derivatives and [mass conservation](continuum-mechanics.md#mass-conservation) give the displayed winding equation. Thus $B_\phi/(\rho R)$ is an advected scalar only when $\mathbf B_p\cdot\nabla\Omega=0$. Differential rotation along a field line otherwise produces toroidal field. This does not violate [magnetic flux freezing](ideal-magnetohydrodynamics.md#magnetic-flux-freezing), which concerns flux through a material surface rather than a cylindrical vector component.

#### Steady toroidal induction by spherical differential rotation

↑ **Parent:** [Toroidal magnetic-field winding equation](#toroidal-magnetic-field-winding-equation)

An axial uniform [magnetic field](magnetic-field.md) and localized radial [differential rotation](astrophysical-fluid-dynamics.md#differential-rotation) generate a steady [toroidal magnetic field](#toroidal-magnetic-field). The angular factor $\sin\theta\cos\theta$ is an eigenfunction of the toroidal angular diffusion operator with eigenvalue $-6$. Its radial amplitude satisfies $\eta(f''+2f'/r-6f/r^2)=-B_0r\Omega'$. Differentiating the integral in the title proves the formula. It is regular at the origin and decays at infinity when $\Omega$ is finite at zero and decays sufficiently rapidly.

##### Diffusive establishment time of a wound toroidal field

↑ **Parent:** [Steady toroidal induction by spherical differential rotation](#steady-toroidal-induction-by-spherical-differential-rotation)

With a fixed axial seed field and prescribed localized [differential rotation](astrophysical-fluid-dynamics.md#differential-rotation), the winding source is time independent. Early induction gives $B_\phi\sim B_0\Omega t$, while the steady balance has $B_\phi\sim B_0\Omega\ell^2/\eta$. Their comparison gives the [magnetic diffusion](#magnetic-diffusion) time, not merely the rotation period. It diverges as conductivity becomes infinite. In an unbounded domain, this is a local equilibration estimate on scale $\ell$, not finite-time exact convergence everywhere. [Lorentz force](relativistic-electromagnetism.md#lorentz-force) feedback may invalidate the prescribed-flow approximation sooner.

### Michael criterion for axisymmetric toroidal-field interchange

↑ **Parent:** [Toroidal magnetic field](#toroidal-magnetic-field)

For constant-density cylindrical rotation $r\Omega(r)\mathbf e_\phi$ and a purely toroidal [magnetic field](magnetic-field.md), an axisymmetric radial displacement gives $b_\phi=(B_\phi/r-B_\phi')\xi_r$. Combining its curvature force with conservation of angular momentum gives the restoring coefficient $\mathcal D$ above. A local incompressible radial-vertical mode has $\omega^2=(k_z^2/k^2)\mathcal D$. Positive $\mathcal D$ gives stability in this ideal interchange setting; negative $\mathcal D$ permits growth. This is distinct from weak-field [magnetorotational instability](astrophysical-disk.md#magnetorotational-instability): a steeply increasing toroidal field can release current energy even without differential rotation.

#### Toroidal interchange field threshold in a thin Keplerian disk

↑ **Parent:** [Michael criterion for axisymmetric toroidal-field interchange](#michael-criterion-for-axisymmetric-toroidal-field-interchange)

For $B_\phi\propto r^p$, constant [density](fluid-mechanics.md#density) and Keplerian $\kappa^2=\Omega^2$, the [Michael criterion for axisymmetric toroidal-field interchange](#michael-criterion-for-axisymmetric-toroidal-field-interchange) becomes $\Omega^2-2(p-1)v_A^2/r^2$. Instability therefore requires $p>1$ and $v_A^2>r^2\Omega^2/[2(p-1)]$. For a field varying on the radial scale $r$, this is an orbital-speed field, much stronger than a gas-pressure-scale field with $v_A\lesssim c_s\sim H\Omega$ in a [thin disk](astrophysical-disk.md#thin-disk). Steep radial field gradients require the exact derivative criterion rather than this scale estimate. The instability is powered by the toroidal field distribution and is distinct from weak vertical-field [magnetorotational instability](astrophysical-disk.md#magnetorotational-instability).

// Target: fluid-mechanics.bigb

#### Global variational form of the Michael criterion

↑ **Parent:** [Michael criterion for axisymmetric toroidal-field interchange](#michael-criterion-for-axisymmetric-toroidal-field-interchange)

For rigid walls $a<r<b$, a nonzero vertical [wavenumber](wave-equation.md#wavenumber) $k$ and radial [Lagrangian fluid displacement](elasticity-physics.md#lagrangian-fluid-displacement) $\xi$, set $y=r\xi$ and $\mathcal D=\kappa^2-r(d/dr)(v_A^2/r^2)$. Axisymmetric modes satisfy

$$
\omega^2\left[-\left(\frac{y'}r\right)'+\frac{k^2y}r\right]=\frac{k^2\mathcal D}r y,\qquad y(a)=y(b)=0.
$$

The operator on the left is a positive [self-adjoint operator](linear-operator-theory.md#self-adjoint-operator). Its [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient) is $\omega^2=k^2\int\mathcal D|y|^2/r\,dr\big/\int(|y'|^2+k^2|y|^2)/r\,dr$. All mode squares are real; a growing mode exists exactly when the continuous coefficient $\mathcal D$ is negative somewhere. Sufficiency follows by a test function supported in that negative interval and the [compact operator](compact-operator.md) and [self-adjoint operator](linear-operator-theory.md#self-adjoint-operator) eigenproblem obtained by conjugating the multiplication operator with the inverse square root of the positive differential operator.

// Target: astrophysical-fluid-dynamics.bigb

### Uniform-current toroidal-field curl reduction

↑ **Parent:** [Toroidal magnetic field](#toroidal-magnetic-field)

For constant-density incompressible [ideal magnetohydrodynamics](ideal-magnetohydrodynamics.md) about $\mathbf B=Jr\mathbf e_\phi$, the cylindrical basis contributions make the linearized [Lorentz force](relativistic-electromagnetism.md#lorentz-force) equal to $imJ\mathbf b+2J\mathbf e_z\times\mathbf b$, apart from a [magnetic pressure](#magnetic-pressure) gradient. The induction equation reduces to $i\omega\mathbf b=imJ\mathbf u$. Taking the curl after eliminating velocity gives the displayed relation, with $\widetilde J=J/\sqrt{\mu_0\rho}$. A second curl gives a vector Helmholtz equation and squared frequencies $\omega^2=\widetilde J^2[m^2\pm2|mk|/(\alpha^2+k^2)^{1/2}]$. The lower $|m|=1$ branch grows when $3k^2>\alpha^2$.

#### Neutral quadrupolar perturbation of a uniform-current toroidal field

↑ **Parent:** [Uniform-current toroidal-field curl reduction](#uniform-current-toroidal-field-curl-reduction)

The displayed [solenoidal vector field](multivariable-calculus.md#solenoidal-vector-field) has $\nabla\times\mathbf b=k\mathbf b$, $\nabla^2\mathbf b=-k^2\mathbf b$ and $\mathbf e_z\times\mathbf b=-i\mathbf b$. Thus the non-gradient part of its linearized [Lorentz force](relativistic-electromagnetism.md#lorentz-force) about $\mathbf B=Jr\mathbf e_\phi$ vanishes. Choosing $p_1=-\mathbf B\cdot\mathbf b/\mu_0$ cancels the magnetic-pressure gradient, and $\mathbf u=0$, $\omega=0$ is a neutral perturbation. It is regular at the axis and realizes the endpoint $m=2$, $\alpha=0$. A boundary condition can exclude this growing-in-radius field, but without such a condition strict positivity at the endpoint cannot be asserted.

## Ideal magnetohydrodynamics

↑ **Parent:** [Magnetohydrodynamics](magnetohydrodynamics.md)

[This section is present in another page, follow this link to view it.](ideal-magnetohydrodynamics.md)

## ↑ Ancestors (5)

1. [Astrophysical fluid dynamics](astrophysical-fluid-dynamics.md)
2. [Fluid mechanics](fluid-mechanics.md)
3. [Branches of physics](physics.md#branches-of-physics)
4. [Physics](physics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (7)

- [Magnetic energy](electromagnetic-wave.md#magnetic-energy)
- [Nobel Prize in Physics in 1970](nobel-prize-in-physics.md#nobel-prize-in-physics-in-1970)
- [Orthogonal-field magnetic Rayleigh-Taylor dispersion relation](continuum-mechanics.md#orthogonal-field-magnetic-rayleigh-taylor-dispersion-relation)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2017.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-65.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-74.md#4/solution)
- [Plasma (physics)](physics.md#plasma-physics)
