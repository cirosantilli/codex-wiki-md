# Astrophysical fluid dynamics

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Astrophysical_fluid_dynamics)

Astrophysical fluid dynamics studies gases, plasmas, stars, discs, and outflows under gravity, rotation, compressibility, and magnetic fields.

**Table of contents**

- [Gravitational instability](#gravitational-instability)
- [Critically rotating self-gravitating cylinder](#critically-rotating-self-gravitating-cylinder)
  - [Dipolar perturbations of a critically rotating cylinder](#dipolar-perturbations-of-a-critically-rotating-cylinder)
  - [Gravitational potential of a displaced cylindrical interface](#gravitational-potential-of-a-displaced-cylindrical-interface)
- [Uniformly rotating barotropic star](#uniformly-rotating-barotropic-star)
  - [Pressure equation for inertial oscillations of a barotropic star](#pressure-equation-for-inertial-oscillations-of-a-barotropic-star)
    - [Sectoral inertial mode of a slowly rotating barotropic star](#sectoral-inertial-mode-of-a-slowly-rotating-barotropic-star)
    - [Anelastic approximation for a rotating barotropic star](#anelastic-approximation-for-a-rotating-barotropic-star)
- [Self-gravitating incompressible slab](#self-gravitating-incompressible-slab)
  - [Gravitational instability of an incompressible slab](#gravitational-instability-of-an-incompressible-slab)
  - [Surface modes of a self-gravitating incompressible slab](#surface-modes-of-a-self-gravitating-incompressible-slab)
- [Isothermal pressure support during gravitational collapse](#isothermal-pressure-support-during-gravitational-collapse)
- [Adiabatic pressure support during gravitational collapse](#adiabatic-pressure-support-during-gravitational-collapse)
- [Differential rotation](#differential-rotation)
- [Affine stellar model](#affine-stellar-model)
  - [Affine breathing mode of a star](#affine-breathing-mode-of-a-star)
  - [Affine quadrupole mode of a star](#affine-quadrupole-mode-of-a-star)
- [Stellar oscillation](#stellar-oscillation)
  - [Helioseismology](#helioseismology)
    - [Solar rotational mode splitting](#solar-rotational-mode-splitting)
    - [Duvall law](#duvall-law)
      - [Abel inversion of stellar acoustic travel times](#abel-inversion-of-stellar-acoustic-travel-times)
  - [Axisymmetric adiabatic displacement operator](#axisymmetric-adiabatic-displacement-operator)
    - [Cowling energy principle for a rotating barotropic star](#cowling-energy-principle-for-a-rotating-barotropic-star)
      - [Effective-potential stratification coefficient](#effective-potential-stratification-coefficient)
  - [Stellar gravity mode](#stellar-gravity-mode)
  - [Stellar acoustic mode](#stellar-acoustic-mode)
    - [Large frequency separation](#large-frequency-separation)
  - [Lamb frequency](#lamb-frequency)
  - [Linear adiabatic stellar oscillation equations](#linear-adiabatic-stellar-oscillation-equations)
    - [Stellar displacement energy identity](#stellar-displacement-energy-identity)
      - [Pressure-free localized stellar convective trial](#pressure-free-localized-stellar-convective-trial)
    - [Acoustic-gravity propagation relation](#acoustic-gravity-propagation-relation)
    - [Cowling approximation](#cowling-approximation)
      - [Plane-parallel Cowling displacement-pressure equations](#plane-parallel-cowling-displacement-pressure-equations)
        - [Plane-parallel stellar f-mode](#plane-parallel-stellar-f-mode)
          - [Matched chromospheric interfacial mode](#matched-chromospheric-interfacial-mode)
      - [Angular-degree bound on perturbed stellar self-gravity](#angular-degree-bound-on-perturbed-stellar-self-gravity)
    - [Radial stellar pulsation equation](#radial-stellar-pulsation-equation)
      - [Central-density upper bound for a radial stellar frequency](#central-density-upper-bound-for-a-radial-stellar-frequency)
      - [Weighted stellar pulsation Rayleigh quotient](#weighted-stellar-pulsation-rayleigh-quotient)
        - [Positive-square radial pulsation energy](#positive-square-radial-pulsation-energy)
        - [Pressure-weighted radial instability criterion](#pressure-weighted-radial-instability-criterion)
  - [Self-gravitating adiabatic displacement equations](#self-gravitating-adiabatic-displacement-equations)
    - [Uniform-density stellar oscillation](#uniform-density-stellar-oscillation)
      - [Radial stability of a uniform-density star](#radial-stability-of-a-uniform-density-star)
      - [Polynomial stellar-mode coefficient reduction](#polynomial-stellar-mode-coefficient-reduction)
      - [Dynamical frequency of a uniform-density star](#dynamical-frequency-of-a-uniform-density-star)
  - [Incompressible stellar surface mode](#incompressible-stellar-surface-mode)
    - [Kelvin stellar mode](#kelvin-stellar-mode)
    - [Surface gravity perturbation of a uniform-density sphere](#surface-gravity-perturbation-of-a-uniform-density-sphere)
  - [Tidal resonance of a stellar oscillation](#tidal-resonance-of-a-stellar-oscillation)
- [Polytrope](#polytrope)
  - [Polytropic equation of state](#polytropic-equation-of-state)
  - [Polytropic atmosphere](#polytropic-atmosphere)
    - [Surface sound speed of a polytropic star](#surface-sound-speed-of-a-polytropic-star)
    - [Neutrally stratified polytropic atmosphere](#neutrally-stratified-polytropic-atmosphere)
    - [Surface gravito-inertial wave](#surface-gravito-inertial-wave)
    - [Polytropic acoustic mode](#polytropic-acoustic-mode)
- [Magnetohydrodynamics](#magnetohydrodynamics)
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
  - [Resistive magnetohydrodynamics](#resistive-magnetohydrodynamics)
    - [Magnetic reconnection](#magnetic-reconnection)
    - [Magnetic skin layer](#magnetic-skin-layer)
      - [Magnetic skin-layer streaming slip](#magnetic-skin-layer-streaming-slip)
      - [Mean Lorentz force in a magnetic skin layer](#mean-lorentz-force-in-a-magnetic-skin-layer)
    - [Flux expulsion](#flux-expulsion)
      - [Phase mixing in magnetic flux expulsion](#phase-mixing-in-magnetic-flux-expulsion)
        - [Cubic-time resistive damping in a differentially rotating cell](#cubic-time-resistive-damping-in-a-differentially-rotating-cell)
    - [Dynamo action](#dynamo-action)
      - [Radial-flow dynamo energy bound](#radial-flow-dynamo-energy-bound)
      - [Dynamo quenching](#dynamo-quenching)
        - [Algebraic alpha quenching](#algebraic-alpha-quenching)
          - [Alpha-quenching rotating wave](#alpha-quenching-rotating-wave)
            - [Unequal-hemisphere dynamo rotating wave](#unequal-hemisphere-dynamo-rotating-wave)
      - [Equivariant three-mode dynamo normal form](#equivariant-three-mode-dynamo-normal-form)
        - [Magnetic onset on a rotating velocity branch](#magnetic-onset-on-a-rotating-velocity-branch)
        - [Normalization of nonzero dynamo coupling coefficients](#normalization-of-nonzero-dynamo-coupling-coefficients)
      - [Anti-dynamo theorem](#anti-dynamo-theorem)
        - [Periodic two-coordinate anti-dynamo energy bound](#periodic-two-coordinate-anti-dynamo-energy-bound)
        - [Planar anti-dynamo theorem](#planar-anti-dynamo-theorem)
          - [Zeldovich planar flux balance](#zeldovich-planar-flux-balance)
        - [Toroidal-velocity anti-dynamo theorem](#toroidal-velocity-anti-dynamo-theorem)
        - [Cowling anti-dynamo theorem](#cowling-anti-dynamo-theorem)
      - [Magnetic concentration by an incompressible stagnation flow](#magnetic-concentration-by-an-incompressible-stagnation-flow)
        - [Self-similar magnetic mode in a stagnation flow](#self-similar-magnetic-mode-in-a-stagnation-flow)
      - [Backus' necessary condition for dynamo action](#backus-necessary-condition-for-dynamo-action)
        - [Maximum-strain bound on dynamo growth](#maximum-strain-bound-on-dynamo-growth)
      - [Mean-field dynamo](#mean-field-dynamo)
        - [Mean-field shearing-wave transient amplification](#mean-field-shearing-wave-transient-amplification)
        - [Dipole and quadrupole parity in a mean-field dynamo](#dipole-and-quadrupole-parity-in-a-mean-field-dynamo)
          - [Coupled-hemisphere dynamo parity threshold](#coupled-hemisphere-dynamo-parity-threshold)
          - [Parity splitting of a mean-field dynamo threshold](#parity-splitting-of-a-mean-field-dynamo-threshold)
        - [Alpha-Omega dynamo](#alpha-omega-dynamo)
          - [Plane-layer alpha-Omega dynamo threshold](#plane-layer-alpha-omega-dynamo-threshold)
          - [Alpha-squared Omega dynamo threshold](#alpha-squared-omega-dynamo-threshold)
          - [Bounded-modulation alpha-Omega growth estimate](#bounded-modulation-alpha-omega-growth-estimate)
        - [Omega effect](#omega-effect)
        - [First-order smoothing approximation](#first-order-smoothing-approximation)
          - [Isotropic alpha effect of three helical traveling waves](#isotropic-alpha-effect-of-three-helical-traveling-waves)
          - [Helicity formula for isotropic first-order smoothing](#helicity-formula-for-isotropic-first-order-smoothing)
          - [Quasistatic magnetic response of a helical shearing wave](#quasistatic-magnetic-response-of-a-helical-shearing-wave)
          - [Monochromatic coupled magnetic and velocity response](#monochromatic-coupled-magnetic-and-velocity-response)
          - [Oscillatory magnetic response in first-order smoothing](#oscillatory-magnetic-response-in-first-order-smoothing)
        - [Parker dynamo wave](#parker-dynamo-wave)
          - [Local alpha-Omega dynamo wave dispersion](#local-alpha-omega-dynamo-wave-dispersion)
          - [Periodically reversing Parker dynamo coupling](#periodically-reversing-parker-dynamo-coupling)
        - [Alpha effect](#alpha-effect)
          - [Rapidly fluctuating alpha effect](#rapidly-fluctuating-alpha-effect)
          - [Strong-field quenching of an isotropic electromotive force](#strong-field-quenching-of-an-isotropic-electromotive-force)
          - [Alpha-squared dynamo](#alpha-squared-dynamo)
            - [Homogeneous alpha-squared dynamo growth criterion](#homogeneous-alpha-squared-dynamo-growth-criterion)
            - [Anisotropic alpha-squared dynamo](#anisotropic-alpha-squared-dynamo)
              - [Uniaxial alpha dynamo threshold](#uniaxial-alpha-dynamo-threshold)
          - [Alpha tensor](#alpha-tensor)
        - [Mean-field electromotive force](#mean-field-electromotive-force)
          - [Monochromatic small-Reynolds-number mean electromotive force](#monochromatic-small-reynolds-number-mean-electromotive-force)
            - [Antisymmetry of the second-order monochromatic alpha tensor](#antisymmetry-of-the-second-order-monochromatic-alpha-tensor)
            - [Symmetry of the first-order monochromatic alpha tensor](#symmetry-of-the-first-order-monochromatic-alpha-tensor)
          - [Turbulent magnetic pumping](#turbulent-magnetic-pumping)
          - [Integrated electromotive response of a finite cyclonic event](#integrated-electromotive-response-of-a-finite-cyclonic-event)
          - [Space-time average of periodic modes](#space-time-average-of-periodic-modes)
    - [Hartmann flow](#hartmann-flow)
      - [Hartmann flow rate with normal-field walls](#hartmann-flow-rate-with-normal-field-walls)
      - [Hartmann layer](#hartmann-layer)
      - [Hartmann number](#hartmann-number)
    - [Normal magnetic field boundary condition](#normal-magnetic-field-boundary-condition)
    - [Resistive induction equation](#resistive-induction-equation)
      - [Shearing-coordinate magnetic flux equation](#shearing-coordinate-magnetic-flux-equation)
      - [Radial magnetic induction scalar](#radial-magnetic-induction-scalar)
        - [Insulating boundary condition for the radial magnetic scalar](#insulating-boundary-condition-for-the-radial-magnetic-scalar)
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
  - [Ideal magnetohydrodynamics](#ideal-magnetohydrodynamics)
    - [Magnetic relaxation](#magnetic-relaxation)
      - [Collapse of a planar magnetic separatrix](#collapse-of-a-planar-magnetic-separatrix)
      - [Viscous magnetic-relaxation energy identity](#viscous-magnetic-relaxation-energy-identity)
    - [Steady planar ideal-MHD field-line invariants](#steady-planar-ideal-mhd-field-line-invariants)
      - [Alfvénic degeneracy of steady planar MHD](#alfvenic-degeneracy-of-steady-planar-mhd)
      - [Planar ideal-MHD Bernoulli invariant](#planar-ideal-mhd-bernoulli-invariant)
    - [Grad-Shafranov equation](#grad-shafranov-equation)
      - [Grad-Shafranov equation for a force-free magnetic field](#grad-shafranov-equation-for-a-force-free-magnetic-field)
    - [Reduced magnetohydrodynamics](#reduced-magnetohydrodynamics)
      - [Five quadratic cascade invariants of anisotropic magnetohydrodynamic turbulence](#five-quadratic-cascade-invariants-of-anisotropic-magnetohydrodynamic-turbulence)
      - [Slow and entropy fluctuations in reduced magnetohydrodynamics](#slow-and-entropy-fluctuations-in-reduced-magnetohydrodynamics)
    - [Ideal magnetohydrodynamic energy conservation](#ideal-magnetohydrodynamic-energy-conservation)
    - [Ideal magnetohydrodynamic momentum equation](#ideal-magnetohydrodynamic-momentum-equation)
    - [Plane-parallel magnetohydrodynamic flow with imposed shear](#plane-parallel-magnetohydrodynamic-flow-with-imposed-shear)
      - [Alfvén-point compatibility in a plane-parallel sheared flow](#alfven-point-compatibility-in-a-plane-parallel-sheared-flow)
      - [Magnetohydrodynamic shear work](#magnetohydrodynamic-shear-work)
    - [Ideal magnetohydrodynamic equations](#ideal-magnetohydrodynamic-equations)
    - [Magnetohydrodynamic energy principle](#magnetohydrodynamic-energy-principle)
      - [Incompressible magnetic displacement energy identity](#incompressible-magnetic-displacement-energy-identity)
        - [Interchange stability of an incompressible magnetized atmosphere](#interchange-stability-of-an-incompressible-magnetized-atmosphere)
      - [Linear displacement equations for a magnetized atmosphere](#linear-displacement-equations-for-a-magnetized-atmosphere)
    - [Elsässer variable](#elsasser-variable)
      - [Elsässer energy invariant](#elsasser-energy-invariant)
    - [Cross-helicity](#cross-helicity)
      - [Cross-helicity conservation law](#cross-helicity-conservation-law)
        - [Material conservation of cross-helicity density](#material-conservation-of-cross-helicity-density)
    - [Magnetic flux freezing](#magnetic-flux-freezing)
      - [Flux-surface preservation during magnetic-tube expansion](#flux-surface-preservation-during-magnetic-tube-expansion)
      - [Mass-to-flux ratio](#mass-to-flux-ratio)
        - [Critical mass-to-flux ratio](#critical-mass-to-flux-ratio)
    - [Alfvén speed](#alfven-speed)
      - [Alfvén Mach number](#alfven-mach-number)
      - [Alfvén velocity](#alfven-velocity)
      - [Alfvén number](#alfven-number)
    - [Magnetohydrodynamic wave](#magnetohydrodynamic-wave)
      - [Ambipolar damping](#ambipolar-damping)
        - [Equal-density ion-neutral Alfvén dispersion relation](#equal-density-ion-neutral-alfven-dispersion-relation)
          - [Strong-collision ion-neutral Alfvén modes](#strong-collision-ion-neutral-alfven-modes)
      - [Entropy mode](#entropy-mode)
      - [Magnetohydrodynamic wave polarization](#magnetohydrodynamic-wave-polarization)
      - [Uniform-current rotating magnetohydrodynamic wave dispersion](#uniform-current-rotating-magnetohydrodynamic-wave-dispersion)
        - [Single-azimuthal-mode current-driven instability threshold](#single-azimuthal-mode-current-driven-instability-threshold)
      - [Alfvén wave](#alfven-wave)
        - [Alfvén-resonant vorticity in a parallel magnetic shear flow](#alfven-resonant-vorticity-in-a-parallel-magnetic-shear-flow)
        - [Kinetic Alfvén wave](#kinetic-alfven-wave)
        - [Magnetohydrodynamic phase mixing](#magnetohydrodynamic-phase-mixing)
        - [Torsional Alfvén wave](#torsional-alfven-wave)
          - [Pressure compatibility of nonlinear torsional Alfvén profiles](#pressure-compatibility-of-nonlinear-torsional-alfven-profiles)
          - [Cylinder-averaged torsional Alfvén wave](#cylinder-averaged-torsional-alfven-wave)
            - [Conserved energy of a cylinder-averaged torsional wave](#conserved-energy-of-a-cylinder-averaged-torsional-wave)
          - [Magnetic axial angular momentum flux](#magnetic-axial-angular-momentum-flux)
        - [Nonlinear Alfvén wave](#nonlinear-alfven-wave)
          - [Magnetic-pressure obstruction to a linearly polarized Alfvén wave](#magnetic-pressure-obstruction-to-a-linearly-polarized-alfven-wave)
          - [Circularly polarized nonlinear Alfvén wave](#circularly-polarized-nonlinear-alfven-wave)
        - [Alfvén characteristic eigenvector](#alfven-characteristic-eigenvector)
        - [Alfvén frequency](#alfven-frequency)
        - [Alfvén wing](#alfven-wing)
          - [Alfvénic Mach-cone slope](#alfvenic-mach-cone-slope)
      - [Magnetosonic wave](#magnetosonic-wave)
        - [High-pressure limit of magnetosonic waves](#high-pressure-limit-of-magnetosonic-waves)
          - [Pseudo-Alfvén wave](#pseudo-alfven-wave)
        - [Isothermal coplanar magnetohydrodynamic characteristic matrix](#isothermal-coplanar-magnetohydrodynamic-characteristic-matrix)
        - [Magnetosonic critical speed](#magnetosonic-critical-speed)
          - [Regularity at a magnetosonic point](#regularity-at-a-magnetosonic-point)
            - [Cold-limit degeneracy of a slow magnetosonic point](#cold-limit-degeneracy-of-a-slow-magnetosonic-point)
        - [Fast magnetosonic wave](#fast-magnetosonic-wave)
        - [Slow magnetosonic wave](#slow-magnetosonic-wave)
        - [Tube speed](#tube-speed)
      - [Magnetohydrodynamic interface wave](#magnetohydrodynamic-interface-wave)
        - [Magnetic stabilization of an equal-density vortex sheet](#magnetic-stabilization-of-an-equal-density-vortex-sheet)
    - [Force-free magnetic field](#force-free-magnetic-field)
      - [Magnetic-energy injection by differential boundary rotation](#magnetic-energy-injection-by-differential-boundary-rotation)
      - [Force-free parameter](#force-free-parameter)
      - [Cylindrical force-free magnetic field](#cylindrical-force-free-magnetic-field)
    - [Linearized ideal magnetohydrodynamic equations](#linearized-ideal-magnetohydrodynamic-equations)
      - [Displacement equation for a parallel magnetic shear flow](#displacement-equation-for-a-parallel-magnetic-shear-flow)
    - [Ideal magnetohydrodynamic induction equation](#ideal-magnetohydrodynamic-induction-equation)
      - [Ideal magnetic response to a cylindrical cyclonic event](#ideal-magnetic-response-to-a-cylindrical-cyclonic-event)
      - [Cartesian magnetic flux function](#cartesian-magnetic-flux-function)
        - [Magnetic island](#magnetic-island)
        - [Cartesian magnetostatic flux-function equilibrium](#cartesian-magnetostatic-flux-function-equilibrium)
      - [Axisymmetric magnetic winding](#axisymmetric-magnetic-winding)
        - [Magnetic-pressure equality radius under Keplerian winding](#magnetic-pressure-equality-radius-under-keplerian-winding)
        - [Ferraro's law of isorotation](#ferraro-s-law-of-isorotation)
    - [Entropy advection equation](#entropy-advection-equation)
    - [Magnetohydrodynamic shock](#magnetohydrodynamic-shock)
      - [Perpendicular magnetohydrodynamic shock](#perpendicular-magnetohydrodynamic-shock)
        - [Compression ratio of a perpendicular magnetohydrodynamic shock](#compression-ratio-of-a-perpendicular-magnetohydrodynamic-shock)
      - [Parallel magnetohydrodynamic shock](#parallel-magnetohydrodynamic-shock)
      - [Ideal magnetohydrodynamic shock conditions](#ideal-magnetohydrodynamic-shock-conditions)
      - [de Hoffmann–Teller frame](#de-hoffmann-teller-frame)
      - [Rotational discontinuity in magnetohydrodynamics](#rotational-discontinuity-in-magnetohydrodynamics)
    - [Axisymmetric magnetostatic Grad-Shafranov system](#axisymmetric-magnetostatic-grad-shafranov-system)
    - [Axisymmetric magnetohydrodynamic wind](#axisymmetric-magnetohydrodynamic-wind)
      - [Cold radial magnetohydrodynamic wind integral](#cold-radial-magnetohydrodynamic-wind-integral)
      - [Sub-Alfvénic isorotation in a steady axisymmetric wind](#sub-alfvenic-isorotation-in-a-steady-axisymmetric-wind)
      - [Corotating energy invariant of an axisymmetric magnetic wind](#corotating-energy-invariant-of-an-axisymmetric-magnetic-wind)
      - [Field-line angular velocity of an axisymmetric wind](#field-line-angular-velocity-of-an-axisymmetric-wind)
      - [Poloidal magnetic flux function](#poloidal-magnetic-flux-function)
        - [Material advection of an axisymmetric magnetic flux function](#material-advection-of-an-axisymmetric-magnetic-flux-function)
        - [Axisymmetric magnetic flux surface](#axisymmetric-magnetic-flux-surface)
        - [Power-law poloidal field near a disk surface](#power-law-poloidal-field-near-a-disk-surface)
      - [Magnetohydrodynamic mass loading](#magnetohydrodynamic-mass-loading)
        - [Regular-axis alignment of steady poloidal ideal flow](#regular-axis-alignment-of-steady-poloidal-ideal-flow)
      - [Field-line angular velocity](#field-line-angular-velocity)
      - [Magnetohydrodynamic angular-momentum invariant](#magnetohydrodynamic-angular-momentum-invariant)
        - [Maxwell torque conservation in an axisymmetric wind](#maxwell-torque-conservation-in-an-axisymmetric-wind)
      - [Magnetohydrodynamic Bernoulli invariant](#magnetohydrodynamic-bernoulli-invariant)
        - [Isothermal magnetic Bernoulli integral](#isothermal-magnetic-bernoulli-integral)
      - [Alfvén surface](#alfven-surface)
        - [Alfvén radius](#alfven-radius)
        - [Alfvén-surface regularity condition for an axisymmetric wind](#alfven-surface-regularity-condition-for-an-axisymmetric-wind)
      - [Asymptotic energy of a radial magnetohydrodynamic wind](#asymptotic-energy-of-a-radial-magnetohydrodynamic-wind)
      - [Magnetocentrifugal acceleration](#magnetocentrifugal-acceleration)
        - [Thirty-degree magnetocentrifugal launching criterion](#thirty-degree-magnetocentrifugal-launching-criterion)
          - [Marginal straight-line launch at thirty degrees](#marginal-straight-line-launch-at-thirty-degrees)
        - [Magnetocentrifugal launching criterion in a flattened power-law potential](#magnetocentrifugal-launching-criterion-in-a-flattened-power-law-potential)
- [Self-gravitating gaseous filament](#self-gravitating-gaseous-filament)
  - [Magnetized self-gravitating filament](#magnetized-self-gravitating-filament)
  - [Line mass](#line-mass)
- [Parker wind](#parker-wind)
  - [Polytropic Parker wind](#polytropic-parker-wind)
    - [Parker wind equation](#parker-wind-equation)

## Gravitational instability

↑ **Parent:** [Astrophysical fluid dynamics](astrophysical-fluid-dynamics.md)

Gravitational instability is the growth of a perturbation because its increased self-gravity overcomes the opposing support or restoring response. For a uniform nonexpanding gas, linearization gives the [Jeans instability](linear-cosmological-density-perturbation.md#jeans-instability) dispersion relation $\omega^2=c_s^2k^2-4\pi G\rho$: sufficiently long wavelengths grow rather than oscillate. In an expanding universe the background and [Hubble friction](cosmology.md#hubble-friction) modify the growth rate; a pressureless growing density mode can eventually become nonlinear. Rotation, magnetic stress, pressure and geometry can all alter the stability threshold in other systems.

## Critically rotating self-gravitating cylinder

↑ **Parent:** [Astrophysical fluid dynamics](astrophysical-fluid-dynamics.md)

A uniform-[mass density](fluid-mechanics.md#density) self-gravitating cylinder has $\Phi_R=2\pi G\rho_0R$. Radial balance with the displayed rotation law gives $p_R=\rho_0(k^2R^3-2\pi G\rho_0R)$. At central [pressure](thermodynamics.md#pressure) $\pi^2G^2\rho_0^3/k^2$, [pressure](thermodynamics.md#pressure) becomes $\rho_0k^2(R^2-R_0^2)^2/4$ and the [free surface](fluid-mechanics.md#free-surface) has zero effective gravity. The positive radius uses $|k|$ if either rotation direction is allowed.

### Dipolar perturbations of a critically rotating cylinder

↑ **Parent:** [Critically rotating self-gravitating cylinder](#critically-rotating-self-gravitating-cylinder)

The regular $m=1$ [velocity](classical-mechanics.md#velocity) family satisfies the displayed formulas. The surface [pressure](thermodynamics.md#pressure) condition and gravitational matching give $W_s=-\Omega_s^2R_0\eta$, while the kinematic condition is $i(\omega+\Omega_s)\eta=u_R(R_0)$. If the material radial displacement $u_R/[i(\omega+kR)]$ is continued regularly to the boundary, then $\eta=-ia$ and $\omega^2=0$: translation of an isolated cylinder has no restoring force. Using only the Eulerian [velocity](classical-mechanics.md#velocity) conditions instead leaves $\omega^2(\omega+\Omega_s)=0$. The additional surface-corotation case has $\eta=0$, $\Phi'=0$, $u_R=a(kR-\Omega_s)$ and $W=iaR[(kR)^2-\Omega_s^2]$; it satisfies the [velocity](classical-mechanics.md#velocity) equations and zero surface [pressure](thermodynamics.md#pressure). Excluding that degenerate branch is an extra admissibility assumption, not a valid division by a nonzero frequency at every surface.

### Gravitational potential of a displaced cylindrical interface

↑ **Parent:** [Critically rotating self-gravitating cylinder](#critically-rotating-self-gravitating-cylinder)

For a uniform-[mass density](fluid-mechanics.md#density) cylinder with surface displacement $\eta e^{im\phi}$, the interior and exterior potential perturbations solve [Laplace's equation](partial-differential-equation.md#laplace-equation) and are proportional to $R^m$ and $R^{-m}$. Continuity of potential and the Poisson derivative jump $\Phi'_{R,\mathrm{out}}-\Phi'_{R,\mathrm{in}}=4\pi G\rho_0\eta$ give the displayed surface amplitude. The surface [mass density](fluid-mechanics.md#density) term must be retained even though bulk incompressibility makes the interior [mass density](fluid-mechanics.md#density) perturbation zero.

## Uniformly rotating barotropic star

↑ **Parent:** [Astrophysical fluid dynamics](astrophysical-fluid-dynamics.md)

In a connected inviscid uniformly rotating [barotropic fluid](fluid-mechanics.md#barotropic-fluid), momentum balance makes the displayed sum constant. The [pressure](thermodynamics.md#pressure) term is the [barotropic enthalpy function](fluid-mechanics.md#barotropic-enthalpy-function). Perturbations experience [Coriolis acceleration](physics.md#coriolis-acceleration), and their rotating-frame frequency depends on the chosen exponential sign convention.

### Pressure equation for inertial oscillations of a barotropic star

↑ **Parent:** [Uniformly rotating barotropic star](#uniformly-rotating-barotropic-star)

In the [Cowling approximation](#cowling-approximation), a mode with phase $e^{i\omega t+im\phi}$ has rotating-frame frequency $\sigma=\omega+m\Omega$. The horizontal momentum matrix has determinant $4\Omega^2-\sigma^2$. Eliminating [velocities](classical-mechanics.md#velocity) yields a pressure-potential equation with vertical coefficient $1-4\Omega^2/\sigma^2$ and density-gradient term $2m\Omega\rho_RW/(R\sigma)$. Frequencies zero and plus or minus $2\Omega$ need the original system rather than this inversion.

#### Sectoral inertial mode of a slowly rotating barotropic star

↑ **Parent:** [Pressure equation for inertial oscillations of a barotropic star](#pressure-equation-for-inertial-oscillations-of-a-barotropic-star)

For spherical [mass density](fluid-mechanics.md#density) in the [anelastic approximation for a rotating barotropic star](#anelastic-approximation-for-a-rotating-barotropic-star), the displayed [pressure](thermodynamics.md#pressure) amplitude gives [velocity](classical-mechanics.md#velocity) proportional to $(-izR^{m-1},zR^{m-1},iR^m)$. This [velocity](classical-mechanics.md#velocity) is divergence free and tangent to spherical shells, so its mass-weighted divergence vanishes for every spherical [mass density](fluid-mechanics.md#density) profile. It is an inertial r-mode driven by [Coriolis acceleration](physics.md#coriolis-acceleration); with phase $e^{i\omega t+im\phi}$ its inertial frequency is $\omega=-(m-1)(m+2)\Omega/(m+1)$.

#### Anelastic approximation for a rotating barotropic star

↑ **Parent:** [Pressure equation for inertial oscillations of a barotropic star](#pressure-equation-for-inertial-oscillations-of-a-barotropic-star)

For slow rotation and low-frequency inertial motion, neglect the time derivative of the Eulerian [mass density](fluid-mechanics.md#density) perturbation relative to the mass-weighted [velocity](classical-mechanics.md#velocity) divergence. This filters acoustic compressibility while retaining background [mass density](fluid-mechanics.md#density) variation. A spherical background [mass density](fluid-mechanics.md#density) is often sufficient at leading order in rotation.

## Self-gravitating incompressible slab

↑ **Parent:** [Astrophysical fluid dynamics](astrophysical-fluid-dynamics.md)

A uniform [mass density](fluid-mechanics.md#density) slab with free surfaces at $z=\pm H$ has $\rho_0=\Sigma/(2H)$, internal gravity $4\pi G\rho_0z$ and hydrostatic [pressure](thermodynamics.md#pressure) $2\pi G\rho_0^2(H^2-z^2)$ above ambient [pressure](thermodynamics.md#pressure). Its [surface modes of a self-gravitating incompressible slab](#surface-modes-of-a-self-gravitating-incompressible-slab) separate into thickness and bending parities.

### Gravitational instability of an incompressible slab

↑ **Parent:** [Self-gravitating incompressible slab](#self-gravitating-incompressible-slab)

The even surface branch is unstable for $0<kH<q_c$, where $q_c=(1+e^{-2q_c})/2\simeq0.6392322714$, and stable above this threshold. All positive-wavenumber odd modes are stable because $1-e^{-2q}<2q$. The equilibrium nevertheless has a long-wavelength column-density instability.

### Surface modes of a self-gravitating incompressible slab

↑ **Parent:** [Self-gravitating incompressible slab](#self-gravitating-incompressible-slab)

For $q=kH$, the even and odd scalar-potential branches have $\omega_e^2=(2\pi G\Sigma/H)[q\tanh q-1/(1+\coth q)]$ and $\omega_o^2=(2\pi G\Sigma/H)[q\coth q-1/(1+\tanh q)]$. Even potential symmetry moves the surfaces oppositely; odd potential symmetry bends them together. Hydrostatic free-surface [pressure](thermodynamics.md#pressure) gives the positive term and perturbed self-gravity the negative term.

## Isothermal pressure support during gravitational collapse

↑ **Parent:** [Astrophysical fluid dynamics](astrophysical-fluid-dynamics.md)

For fixed mass and [temperature](thermodynamics.md#temperature), $p\propto L^{-3}$, so the pressure-support scale $pL^3$ stays constant while gravitational binding scales as $L^{-1}$. Isothermal [pressure](thermodynamics.md#pressure) therefore becomes relatively less important during homologous contraction.

## Adiabatic pressure support during gravitational collapse

↑ **Parent:** [Astrophysical fluid dynamics](astrophysical-fluid-dynamics.md)

With fixed mass and homologous scale $L$, adiabatic [pressure](thermodynamics.md#pressure) obeys $p\propto L^{-3\gamma}$. Its support relative to gravitational energy scales as $pL^3/|W_g|\propto L^{4-3\gamma}$. [Pressure](thermodynamics.md#pressure) becomes relatively stronger on contraction for $\gamma>4/3$, weaker for $\gamma<4/3$ and has the same scaling at $\gamma=4/3$.

## Differential rotation

↑ **Parent:** [Astrophysical fluid dynamics](astrophysical-fluid-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Differential_rotation)

Differential rotation means that different parts of a rotating body or fluid have different angular velocities. An axisymmetric rotational [velocity field](fluid-mechanics.md#velocity-field) can be written $\mathbf u=R\Omega(R,z)\mathbf e_\phi$.

## Affine stellar model

↑ **Parent:** [Astrophysical fluid dynamics](astrophysical-fluid-dynamics.md)

An affine stellar model represents a fluid body by a time-dependent ellipsoid whose internal velocity is linear in position. Its axis lengths become finitely many dynamical degrees of freedom.

### Affine breathing mode of a star

↑ **Parent:** [Affine stellar model](#affine-stellar-model)

The affine breathing mode changes all three principal axes by the same fraction and therefore changes the stellar volume and density.

### Affine quadrupole mode of a star

↑ **Parent:** [Affine stellar model](#affine-stellar-model)

An affine quadrupole mode has axis perturbations whose fractional sum vanishes. It changes the ellipsoidal shape without changing volume to first order.

## Stellar oscillation

↑ **Parent:** [Astrophysical fluid dynamics](astrophysical-fluid-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stellar_oscillation)

A stellar oscillation is a normal mode of a star or stellar model. Pressure, buoyancy, rotation, self-gravity, or an imposed gravitational potential supplies its restoring force.

### Helioseismology

↑ **Parent:** [Stellar oscillation](#stellar-oscillation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Helioseismology)

Helioseismology infers the [Sun](stellar-astrophysics.md#sun)'s structure and dynamics from its [stellar oscillations](#stellar-oscillation). Spatial projection of resolved surface observations onto [spherical harmonics](analysis.md#spherical-harmonic) identifies angular degree and azimuthal order; a temporal [Fourier transform](analysis.md#fourier-transform) measures mode [frequencies](physics.md#frequency). [Stellar acoustic modes](#stellar-acoustic-mode) constrain the [adiabatic sound speed](compressible-flow.md#adiabatic-sound-speed), while rotational splitting constrains [stellar rotation](stellar-astrophysics.md#stellar-rotation). Their finite wavelength, surface reflection phases and finite observational coverage limit inversion resolution.

#### Solar rotational mode splitting

↑ **Parent:** [Helioseismology](#helioseismology)

Slow [stellar rotation](stellar-astrophysics.md#stellar-rotation) breaks the azimuthal degeneracy of a [stellar oscillation](#stellar-oscillation). First-order rotational [frequency](physics.md#frequency) shifts are weighted [integrals](calculus.md#integral) of the angular velocity with kernels computed from the unperturbed mode. Multiple radial orders and angular degrees provide overlapping constraints on internal rotation. Surface rotation alone cannot replace these internal measurements, and a finite kernel set does not give pointwise uniqueness.

#### Duvall law

↑ **Parent:** [Helioseismology](#helioseismology)

For a high-order [stellar acoustic mode](#stellar-acoustic-mode), neglecting [buoyancy](fluid-mechanics.md#buoyancy) and representing surface reflection by a phase, [WKB quantization](analysis.md#wkb-quantization-condition) gives $F(w)=\int_{r_t}^{R}\sqrt{1-c^2/(w^2r^2)}\,dr/c$, where $w=\omega/L$ and $L=\sqrt{\ell(\ell+1)}$. Thus the scaled frequencies depend mainly on $\omega/L$, rather than independently on degree and radial order. A frequency-dependent surface phase can be fitted when a constant $\alpha$ is inadequate.

##### Abel inversion of stellar acoustic travel times

↑ **Parent:** [Duvall law](#duvall-law)

Assume $a=c/r$ decreases outward, tends to zero at $R$, and define $h(a)=-d\ln r/da$. Differentiation of the [Duvall law](#duvall-law) gives $F'(w)=\int_0^w h(b)b/[w^2\sqrt{w^2-b^2}]\,db$. Interchanging [integrals](calculus.md#integral) and using $\int_b^a dw/[w\sqrt{w^2-b^2}\sqrt{a^2-w^2}]=\pi/(2ab)$ proves the displayed [Abel transform](functional-analysis.md#abel-transform) inversion. For a finite outer reference value $w_s$, both lower limits become $w_s$, after removing the known outer-layer contribution to the travel time. Inversion requires a monotone branch and amplifies errors in differentiated frequency data.

### Axisymmetric adiabatic displacement operator

↑ **Parent:** [Stellar oscillation](#stellar-oscillation)

In the [Cowling approximation](#cowling-approximation), an axisymmetric meridional [fluid displacement](fluid-mechanics.md#lagrangian-displacement-fluid-mechanics) in a cylindrically rotating barotropic star obeys $-\omega^2\xi=\mathcal F\xi$, with $\delta\rho=-\nabla\cdot(\rho\xi)$ and $\delta p=-\xi\cdot\nabla p-\gamma p\nabla\cdot\xi$. Conservation of [specific angular momentum](classical-mechanics.md#specific-angular-momentum) supplies the epicyclic term, with $\kappa^2=R^{-3}d(R^4\Omega^2)/dR$. The [Cowling energy principle for a rotating barotropic star](#cowling-energy-principle-for-a-rotating-barotropic-star) gives its symmetric quadratic form.

#### Cowling energy principle for a rotating barotropic star

↑ **Parent:** [Axisymmetric adiabatic displacement operator](#axisymmetric-adiabatic-displacement-operator)

With vanishing surface [pressure](thermodynamics.md#pressure)/[mass density](fluid-mechanics.md#density) and regular admissible displacements, [integration by parts](calculus.md#integration-by-parts) makes the [axisymmetric adiabatic displacement operator](#axisymmetric-adiabatic-displacement-operator) symmetric in the [mass density](fluid-mechanics.md#density)-weighted [inner product](linear-algebra.md#inner-product). Completing the [pressure](thermodynamics.md#pressure) square gives the displayed energy form. Nonnegative form for every admissible displacement excludes exponentially growing axisymmetric adiabatic modes in the [Cowling approximation](#cowling-approximation). A negative trial [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient) proves negative spectrum by the [Rayleigh-Ritz variational principle](linear-operator-theory.md#rayleigh-ritz-variational-principle). Nonnegative stratification and epicyclic coefficients give a simple sufficient stability condition.

##### Effective-potential stratification coefficient

↑ **Parent:** [Cowling energy principle for a rotating barotropic star](#cowling-energy-principle-for-a-rotating-barotropic-star)

For barotropic equilibrium $dp/d\Psi=-\rho$, this coefficient equals $-\rho^{-1}(dp/d\Psi)[\gamma^{-1}d\ln p/d\Psi-d\ln\rho/d\Psi]$. It weights displacement across effective-potential surfaces in the [Cowling energy principle for a rotating barotropic star](#cowling-energy-principle-for-a-rotating-barotropic-star). Its sign distinguishes stabilizing from destabilizing buoyancy there. It is not itself a squared [frequency](physics.md#frequency): the physical local buoyancy-[frequency](physics.md#frequency) square contains an additional factor $|\nabla\Psi|^2$.

### Stellar gravity mode

↑ **Parent:** [Stellar oscillation](#stellar-oscillation)

A stellar gravity mode is a nonradial [stellar oscillation](#stellar-oscillation) restored by [buoyancy](fluid-mechanics.md#buoyancy) in stable stratification. In the local interior approximation it propagates where $\omega^2<N^2,S_\ell^2$. Such modes are distinct from [stellar acoustic modes](#stellar-acoustic-mode) and do not have a radial $\ell=0$ gravity-wave branch.

### Stellar acoustic mode

↑ **Parent:** [Stellar oscillation](#stellar-oscillation)

A stellar acoustic mode is a pressure-restored [stellar oscillation](#stellar-oscillation). Its local high-frequency propagation branch lies above the [stellar buoyancy frequency](gravity-wave.md#stellar-buoyancy-frequency) and [Lamb frequency](#lamb-frequency). Inner refraction and near-surface reflection form an acoustic cavity; its standing-wave frequencies probe the [adiabatic sound speed](compressible-flow.md#adiabatic-sound-speed) profile.

#### Large frequency separation

↑ **Parent:** [Stellar acoustic mode](#stellar-acoustic-mode)

The leading separation between successive high-order low-degree [stellar acoustic mode](#stellar-acoustic-mode) frequencies is the inverse round-trip acoustic travel time, $\Delta\nu\simeq[2\int_0^Rdr/c_s]^{-1}$. For homologous stars it scales approximately as $(M/R^3)^{1/2}$ and therefore measures mean density.

### Lamb frequency

↑ **Parent:** [Stellar oscillation](#stellar-oscillation)

The Lamb frequency is the horizontal acoustic angular frequency of a spherical-harmonic component of degree $\ell$. With [adiabatic sound speed](compressible-flow.md#adiabatic-sound-speed) $c_s$, $S_\ell^2=\ell(\ell+1)c_s^2/r^2$. It helps determine inner acoustic turning points and vanishes for radial modes.

### Linear adiabatic stellar oscillation equations

↑ **Parent:** [Stellar oscillation](#stellar-oscillation)

For a static spherical star, a [fluid displacement](fluid-mechanics.md#lagrangian-displacement-fluid-mechanics) $\boldsymbol\xi e^{-i\omega t}$ gives $\rho_1=-\nabla\cdot(\rho\boldsymbol\xi)$, $-\omega^2\rho\boldsymbol\xi=-\nabla p_1-\rho_1\nabla\Phi-\rho\nabla\phi_1$ and $\nabla^2\phi_1=4\pi G\rho_1$. The adiabatic relation is $\Delta P=-\Gamma_1P\nabla\cdot\boldsymbol\xi$. Centre regularity and surface mechanical/gravitational boundary conditions select discrete [eigenvalues](linear-operator-theory.md#eigenvalue) in a conservative model.

#### Stellar displacement energy identity

↑ **Parent:** [Linear adiabatic stellar oscillation equations](#linear-adiabatic-stellar-oscillation-equations)

For a nonrotating self-gravitating star, let $p_1,\rho_1,\phi_1$ be Eulerian perturbations and $\Delta p=-\gamma p\nabla\cdot\boldsymbol\xi$ the adiabatic Lagrangian perturbation. Integration of the linear momentum equation against $\boldsymbol\xi^*$, using hydrostatic balance and the perturbed [Poisson equation](partial-differential-equation.md#poisson-equation), yields the displayed [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient). The gravitational integral is over all space and the other integrals over the star. The compression denominator is $\gamma p$, not $\gamma\rho$. Surface terms vanish for compactly supported trials or the physical free-surface and exterior potential conditions.

##### Pressure-free localized stellar convective trial

↑ **Parent:** [Stellar displacement energy identity](#stellar-displacement-energy-identity)

Choose a smooth radial bump $f$ supported inside a shell where the [stellar buoyancy frequency](gravity-wave.md#stellar-buoyancy-frequency) has $N^2<0$. The displayed [fluid displacement](fluid-mechanics.md#lagrangian-displacement-fluid-mechanics) has $\nabla\cdot\boldsymbol\xi=(\rho g/\gamma p)\xi_r$, hence its Eulerian pressure perturbation vanishes identically. Its buoyancy contribution to the [stellar displacement energy identity](#stellar-displacement-energy-identity) is strictly negative and self-gravity is nonpositive. The variational principle therefore proves convective instability with no unsupported assumption that incompressibility alone removes pressure work. Large spherical-harmonic degree also makes perturbed self-gravity small.

#### Acoustic-gravity propagation relation

↑ **Parent:** [Linear adiabatic stellar oscillation equations](#linear-adiabatic-stellar-oscillation-equations)

In the [Cowling approximation](#cowling-approximation) and local short-wavelength limit, the radial wave number satisfies $k_r^2\simeq(\omega^2-S_\ell^2)(\omega^2-N^2)/(c_s^2\omega^2)$. The [Lamb frequency](#lamb-frequency) $S_\ell$ and [stellar buoyancy frequency](gravity-wave.md#stellar-buoyancy-frequency) $N$ delimit acoustic and gravity-wave cavities. This leading interior relation does not replace the near-surface acoustic cutoff or the full gravitational boundary problem.

#### Cowling approximation

↑ **Parent:** [Linear adiabatic stellar oscillation equations](#linear-adiabatic-stellar-oscillation-equations)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cowling_approximation)

The Cowling approximation neglects the perturbation of the gravitational potential while retaining the equilibrium gravitational force in a [stellar oscillation](#stellar-oscillation). It simplifies short-wavelength mode propagation, but can be inaccurate for low-order modes whose perturbed self-gravity matters.

##### Plane-parallel Cowling displacement-pressure equations

↑ **Parent:** [Cowling approximation](#cowling-approximation)

Take depth $z$ positive downward, vertical [fluid displacement](fluid-mechanics.md#lagrangian-displacement-fluid-mechanics) $\xi$ positive upward, and [Lagrangian pressure perturbation](fluid-mechanics.md#lagrangian-pressure-perturbation) $\Pi$. In a [plane-parallel atmosphere](astrophysics.md#plane-parallel-atmosphere) with $p'=\rho g$, the [Cowling approximation](#cowling-approximation) and adiabatic relation give

$$
\xi'=-\frac{gk^2}{\omega^2}\xi-\left(\frac{k^2}{\omega^2}-\frac1{c^2}\right)\frac\Pi\rho,\qquad
\Pi'=-\rho\left(\omega^2-\frac{g^2k^2}{\omega^2}\right)\xi+\frac{gk^2}{\omega^2}\Pi.
$$

Indeed the Eulerian perturbations are $p_1=\Pi+\rho g\xi$ and $\rho_1=\Pi/c^2+\rho'\xi$. Horizontal momentum gives $\boldsymbol\xi_h=i\boldsymbol k p_1/(\rho\omega^2)$; combine this with mass conservation and vertical momentum to eliminate the horizontal displacement. Reversing the sign convention for vertical displacement reverses both displacement-pressure coupling signs.

###### Plane-parallel stellar f-mode

↑ **Parent:** [Plane-parallel Cowling displacement-pressure equations](#plane-parallel-cowling-displacement-pressure-equations)

The [plane-parallel Cowling displacement-pressure equations](#plane-parallel-cowling-displacement-pressure-equations) admit this [stellar oscillation](#stellar-oscillation) for every compatible equilibrium density and [adiabatic sound speed](compressible-flow.md#adiabatic-sound-speed) profile. In the upward-displacement convention its horizontal amplitude is $i\boldsymbol k\xi/k$, its Eulerian pressure amplitude is $\rho g\xi$, and its Lagrangian density and pressure perturbations vanish. Its displacement decays into the star but grows upward without bound, so a pure linear continuation to infinite height is not physical.

###### Matched chromospheric interfacial mode

↑ **Parent:** [Plane-parallel stellar f-mode](#plane-parallel-stellar-f-mode)

For a high-sound-speed, low-density atmosphere over a denser stellar envelope, set $\omega^2=gk(1-\varepsilon)$ in the [plane-parallel Cowling displacement-pressure equations](#plane-parallel-cowling-displacement-pressure-equations). Define $I_a=\int_{-\infty}^{z_0}e^{2k(z-z_0)}\rho^{-1}dz$ and $I_b=\int_{z_0}^{\infty}e^{-2k(z-z_0)}\rho\,dz$. The lower leading solution has $\Pi/\xi=-2\varepsilon gk I_b$ at the match. Above, write $\rho=\varepsilon\widehat\rho$, $\Pi=\varepsilon\psi$, $\xi=\mu\psi$. The upward-decaying solution satisfies $\mu'+2k\mu=-k/(g\widehat\rho)$, so $\mu(z_0)=-(k/g)\varepsilon I_a$. Writing $f=\Pi/(\varepsilon\xi)$ below, continuity of displacement and Lagrangian pressure requires $\mu(z_0)f(z_0)=1$, giving the displayed condition. The integrals must converge and the upper displacement must actually decay. For two constant-density incompressible layers it gives $\varepsilon\simeq2\rho_a/\rho_b$, the expansion of the exact [interfacial gravity-wave dispersion relation](gravity-wave.md#interfacial-gravity-wave-dispersion-relation).

##### Angular-degree bound on perturbed stellar self-gravity

↑ **Parent:** [Cowling approximation](#cowling-approximation)

For a normalized [spherical harmonic](analysis.md#spherical-harmonic) of degree $\ell\geq1$, write $\rho_1=s(r)Y$ and $\phi_1=F(r)Y$. Integration of the radial [Poisson equation](partial-differential-equation.md#poisson-equation) gives $A=-4\pi G\int r^2F^*s\,dr$, where $A=\int[r^2|F'|^2+\ell(\ell+1)|F|^2]dr$. [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) and $\int|F|^2\leq A/[\ell(\ell+1)]$ give the displayed bound on $|E_g|=A/(4\pi G)$. For bounded density amplitudes with fixed radial support this decays as $\ell^{-2}$, giving a quantitative angular short-scale justification of the [Cowling approximation](#cowling-approximation).

#### Radial stellar pulsation equation

↑ **Parent:** [Linear adiabatic stellar oscillation equations](#linear-adiabatic-stellar-oscillation-equations)

For a radial [stellar oscillation](#stellar-oscillation), put $\xi_r=r\eta$. The self-gravitating adiabatic equation is $(\Gamma_1Pr^4\eta^{\prime})^{\prime}+r^3[(3\Gamma_1-4)P]^{\prime}\eta+\rho r^4\omega^2\eta=0$. It is a [Sturm-Liouville problem](analysis.md#sturm-liouville-problem) whose [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient) tests radial stability. The familiar constant-exponent threshold is $\Gamma_1=4/3$; a variable exponent requires the full integral test.

##### Central-density upper bound for a radial stellar frequency

↑ **Parent:** [Radial stellar pulsation equation](#radial-stellar-pulsation-equation)

For constant [adiabatic exponent](thermodynamics.md#heat-capacity-ratio) $\gamma>4/3$ and a star whose central [mass density](fluid-mechanics.md#density) is its maximum, the homologous radial [fluid displacement](fluid-mechanics.md#lagrangian-displacement-fluid-mechanics) $\xi_r=r$ makes the derivative term in the [weighted stellar pulsation Rayleigh quotient](#weighted-stellar-pulsation-rayleigh-quotient) vanish. The remaining quotient is $(3\gamma-4)$ times a positive weighted average of $g/r$. Since $m(r)\leq4\pi\rho_cr^3/3$, $g/r\leq4\pi G\rho_c/3$, proving the bound. For $\gamma<4/3$, the same trial quotient is negative and proves radial instability; the inequality with the central density must not be extended with its sign unchanged.

##### Weighted stellar pulsation Rayleigh quotient

↑ **Parent:** [Radial stellar pulsation equation](#radial-stellar-pulsation-equation)

For radial adiabatic [stellar oscillations](#stellar-oscillation), the quotient is $\mathcal R[\xi]=\int[\gamma p r^4|\xi\prime|^2+r^3((4-3\gamma)p)\prime|\xi|^2]dr/\int\rho r^4|\xi|^2dr$. Regular-centre and free-surface endpoint conditions remove the boundary term. The infimum is the fundamental squared frequency; any negative trial value proves radial instability. A variable [stellar adiabatic exponent](stellar-structure.md#stellar-adiabatic-exponent) must remain inside the derivative.

###### Positive-square radial pulsation energy

↑ **Parent:** [Weighted stellar pulsation Rayleigh quotient](#weighted-stellar-pulsation-rayleigh-quotient)

Integrate the pressure-gradient term in the [weighted stellar pulsation Rayleigh quotient](#weighted-stellar-pulsation-rayleigh-quotient) by parts, with regular centre and zero surface pressure. Writing $\chi=r\xi'+3\xi$ uses $3\xi^2+2r\xi\xi'=(\chi^2-r^2(\xi')^2)/3$ and gives the displayed expression. Thus radial instability requires $\gamma<4/3$ somewhere in the positive-pressure interior. A constant trial function gives $K=3\xi^2\int_0^R(3\gamma-4)pr^2dr$, so strict radial stability requires this weighted integral to be positive, in particular $\gamma>4/3$ somewhere. When $\gamma=4/3$ throughout, constant $\xi$ is an exact zero-frequency homologous mode: the star is marginal, rather than strictly stable. Local threshold crossings alone do not determine stability for a mixed profile; the full [Rayleigh-Ritz variational principle](linear-operator-theory.md#rayleigh-ritz-variational-principle) does.

###### Pressure-weighted radial instability criterion

↑ **Parent:** [Weighted stellar pulsation Rayleigh quotient](#weighted-stellar-pulsation-rayleigh-quotient)

The homologous trial function $\xi=1$ in the [weighted stellar pulsation Rayleigh quotient](#weighted-stellar-pulsation-rayleigh-quotient) has numerator $-3\int_0^{R_s}r^2p(4-3\gamma)dr$. Positivity of that integral therefore proves radial instability. It is a sufficient test: a nonpositive integral does not guarantee stability against every radial shape. For constant $\gamma$, the homologous threshold is $4/3$.

### Self-gravitating adiabatic displacement equations

↑ **Parent:** [Stellar oscillation](#stellar-oscillation)

The [fluid displacement](fluid-mechanics.md#lagrangian-displacement-fluid-mechanics) $\boldsymbol\xi$ determines Eulerian density through $\delta\rho=-\nabla\cdot(\rho\boldsymbol\xi)$. The pressure law is $\delta p+\boldsymbol\xi\cdot\nabla p=-\gamma p\nabla\cdot\boldsymbol\xi$. The linear momentum equation must include both $-\delta\rho\nabla\Phi$ and $-\rho\nabla\delta\Phi$, with $\nabla^2\delta\Phi=4\pi G\delta\rho$. Retaining the last term incorporates perturbed self-gravity.

#### Uniform-density stellar oscillation

↑ **Parent:** [Self-gravitating adiabatic displacement equations](#self-gravitating-adiabatic-displacement-equations)

A constant-density gas sphere in [hydrostatic equilibrium](statistical-physics.md#hydrostatic-equilibrium) has $g=\omega_d^2r$ and $p=\rho\omega_d^2(R^2-r^2)/2$. Its [stellar oscillations](#stellar-oscillation) can be expanded using [regular solid harmonics](analysis.md#regular-solid-harmonic) and radial displacement amplitudes. Uniform density does not imply uniform [specific entropy](thermodynamics.md#specific-entropy), so this equilibrium can be radially stable and still exhibit [convective instability](stellar-structure.md#stellar-convective-instability).

##### Radial stability of a uniform-density star

↑ **Parent:** [Uniform-density stellar oscillation](#uniform-density-stellar-oscillation)

For the even polynomial family of degree $n\geq2$, the physical radial squared frequency is $[\gamma n(n+1)/2-4]\omega_d^2$. The fundamental $n=2$ mode is stable when $\gamma>4/3$ and marginal at $\gamma=4/3$. At angular degree zero the gradient of the [regular solid harmonic](analysis.md#regular-solid-harmonic) vanishes, so the auxiliary displacement amplitude multiplying it is redundant.

##### Polynomial stellar-mode coefficient reduction

↑ **Parent:** [Uniform-density stellar oscillation](#uniform-density-stellar-oscillation)

When the amplitudes of [uniform-density stellar oscillation](#uniform-density-stellar-oscillation) are finite even polynomials, their highest coefficients close algebraically. With $L=n(2l+n+1)$ and $x=\omega^2/\omega_d^2$, the nonradial coefficient determinant is $x^2+(4-\gamma L/2)x-l(l+1)$. A degree balance gives a necessary frequency relation without solving every lower coefficient or imposing surface conditions.

##### Dynamical frequency of a uniform-density star

↑ **Parent:** [Uniform-density stellar oscillation](#uniform-density-stellar-oscillation)

The frequency $\omega_d=(GM/R^3)^{1/2}=(4\pi G\rho/3)^{1/2}$ measures the inverse gravitational timescale of a uniform-density sphere. It is the natural normalization for [uniform-density stellar oscillation](#uniform-density-stellar-oscillation) and the linear restoring or destabilizing accelerations.

### Incompressible stellar surface mode

↑ **Parent:** [Stellar oscillation](#stellar-oscillation)

An incompressible stellar surface mode has vanishing Lagrangian volume perturbation. In a harmonic fixed potential, a displacement generated by a solid spherical harmonic has a frequency fixed by its angular degree.

#### Kelvin stellar mode

↑ **Parent:** [Incompressible stellar surface mode](#incompressible-stellar-surface-mode)

The [Kelvin stellar modes](#kelvin-stellar-mode) are the potential [incompressible stellar surface modes](#incompressible-stellar-surface-mode) of a nonrotating self-gravitating uniform-density sphere with [incompressible flow](fluid-mechanics.md#incompressible-flow). For a regular displacement potential $U=A r^lY_l^m$, the free-surface [Lagrangian pressure perturbation](fluid-mechanics.md#lagrangian-pressure-perturbation) condition and the [surface gravity perturbation of a uniform-density sphere](#surface-gravity-perturbation-of-a-uniform-density-sphere) give

$$
\omega_l^2=\frac{2l(l-1)}{2l+1}\frac{GM}{R^3},\qquad l\geq1.
$$

In detail $\delta p/\rho=\omega^2U-\delta\Phi$ and $\delta p/\rho=(GM/R^2)\xi_r$ at $r=R$, so $\omega_l^2=lGM/R^3-4\pi G\rho l/(2l+1)$. The $l=1$ branch is rigid translation with zero restoring force. This potential family does not exhaust vortical zero-frequency displacements: $\boldsymbol\xi=\boldsymbol\Omega\times\mathbf r$ is tangent to the sphere and has zero restoring force but nonzero [curl](calculus.md#curl).

#### Surface gravity perturbation of a uniform-density sphere

↑ **Parent:** [Incompressible stellar surface mode](#incompressible-stellar-surface-mode)

For a uniform-density sphere with [incompressible flow](fluid-mechanics.md#incompressible-flow) of radius $R$ with one surface [spherical harmonic](analysis.md#spherical-harmonic) displacement $\xi_r(R)=lA R^{l-1}Y_l^m$, the bulk density perturbation vanishes but the surface contributes $\delta\rho=\rho\xi_r(R)\delta(r-R)$. Continuity of the [Newtonian gravitational potential](classical-mechanics.md#newtonian-gravitational-potential) and the [Poisson equation](partial-differential-equation.md#poisson-equation) give $[\partial_r\delta\Phi]_{\mathrm{out}-\mathrm{in}}=4\pi G\rho\xi_r(R)$. The regular interior and decaying exterior solutions are

$$
\delta\Phi_{\mathrm{in}}=C r^lY_l^m,\qquad
\delta\Phi_{\mathrm{out}}=C R^{2l+1}r^{-l-1}Y_l^m,\qquad
C=-\frac{4\pi G\rho l A}{2l+1}.
$$

The coefficient follows because the derivative jump is $-(2l+1)C R^{l-1}Y_l^m$. This surface source is why neglecting the bulk density perturbation does not justify neglecting the perturbed gravity.

### Tidal resonance of a stellar oscillation

↑ **Parent:** [Stellar oscillation](#stellar-oscillation)

Periodic tidal forcing excites a stellar normal mode with response proportional to $(\omega^2-\omega_\ell^2)^{-1}$ in an undamped linear model. Dissipation regularizes the divergence and introduces a phase shift near resonance.

## Polytrope

↑ **Parent:** [Astrophysical fluid dynamics](astrophysical-fluid-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polytrope)

A polytrope obeys $p=K\rho^{1+1/n}$ for constants $K$ and polytropic index $n$.

### Polytropic equation of state

↑ **Parent:** [Polytrope](#polytrope)

A polytropic equation of state relates pressure and density by $p=K\rho^\Gamma$ with constant $K$ and exponent $\Gamma$. Writing $\Gamma=1+1/n$ defines the polytropic index $n$.

### Polytropic atmosphere

↑ **Parent:** [Polytrope](#polytrope)

A polytropic atmosphere obeys $p=K\rho^{1+1/m}$ for polytropic index $m$. Under uniform vertical gravity and a free surface, its density and pressure are powers of depth below that surface.

#### Surface sound speed of a polytropic star

↑ **Parent:** [Polytropic atmosphere](#polytropic-atmosphere)

In a plane-parallel [polytropic atmosphere](#polytropic-atmosphere) of index $m$, let $z$ measure depth from a zero-pressure boundary and take constant [gravitational acceleration](classical-mechanics.md#gravitational-acceleration) $g$. The [stellar hydrostatic equation](stellar-structure.md#hydrostatic-pressure-support-equation) and $p=K\rho^{1+1/m}$ integrate to $(m+1)p/\rho=gz$. Consequently the [adiabatic sound speed](compressible-flow.md#adiabatic-sound-speed) satisfies $c_s^2=\gamma p/\rho=\gamma gz/(m+1)$, so $c_s\propto z^{1/2}$. This local relation does not justify extrapolating a surface model to the stellar core.

#### Neutrally stratified polytropic atmosphere

↑ **Parent:** [Polytropic atmosphere](#polytropic-atmosphere)

A polytropic atmosphere is neutrally stratified when $1+1/m=\gamma$, so its equilibrium pressure-density relation matches the adiabatic relation and its buoyancy frequency vanishes.

#### Surface gravito-inertial wave

↑ **Parent:** [Polytropic atmosphere](#polytropic-atmosphere)

A surface gravito-inertial wave combines free-surface gravity restoration with Coriolis restoration. In a uniformly rotating deep atmosphere its incompressible dispersion relation can be written

$$
\omega^2=2\Omega^2+\sqrt{g^2k_x^2+4\Omega^4}.
$$

#### Polytropic acoustic mode

↑ **Parent:** [Polytropic atmosphere](#polytropic-atmosphere)

In a neutrally stratified polytropic atmosphere, vertically trapped polynomial solutions of degree $n\geq1$ describe acoustic pressure modes. The degree-zero member is the surface-gravity mode.

## Magnetohydrodynamics

↑ **Parent:** [Astrophysical fluid dynamics](astrophysical-fluid-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Magnetohydrodynamics)

Magnetohydrodynamics treats an electrically conducting fluid coupled to a magnetic field through the Lorentz force and electromagnetic induction.

### Magnetic flux concentration

↑ **Parent:** [Magnetohydrodynamics](#magnetohydrodynamics)

Magnetic flux concentration redistributes existing [magnetic flux](electromagnetism.md#magnetic-flux) into a smaller area. For a locally straight flux bundle with conserved flux, $B\mathcal A$ is constant, so decreasing area increases field strength. Converging convection, field-line stretching and [flux expulsion](#flux-expulsion) can produce concentrations; finite [magnetic diffusivity](#magnetic-diffusivity) opposes them and [Lorentz force](electromagnetism.md#lorentz-force) feedback limits the kinematic approximation. Redistribution alone is not evidence of net [dynamo action](#dynamo-action).

#### Equipartition magnetic field

↑ **Parent:** [Magnetic flux concentration](#magnetic-flux-concentration)

Equating magnetic energy density $B^2/(2\mu_0)$ to kinetic energy density $\rho U^2/2$ defines this order-of-magnitude field. It marks when a weak-field kinematic treatment of a given flow can fail, not a universal upper bound on concentrated fields. Gas-pressure confinement, compression, partial evacuation and dynamic pressure can allow stronger local fields.

#### Convective collapse

↑ **Parent:** [Magnetic flux concentration](#magnetic-flux-concentration)

A compressible intensification mechanism for a thin, nearly vertical [flux tube](electromagnetism.md#flux-tube) in a superadiabatic atmosphere. An unstable downflow drains material and lowers internal gas pressure; approximate lateral balance $p_i+B^2/(2\mu_0)=p_e$ then permits the tube to contract and its field to strengthen at nearly conserved [magnetic flux](electromagnetism.md#magnetic-flux). It relies on compressibility and thermal evolution, which are absent from a strict [Boussinesq approximation](geophysical-fluid-dynamics.md#boussinesq-approximation). Dynamic photospheric structures need not satisfy thin-tube equilibrium, so this mechanism does not explain every intense field concentration.

### Magnetostrophic balance

↑ **Parent:** [Magnetohydrodynamics](#magnetohydrodynamics)

The leading force balance in a rapidly rotating conducting fluid when inertial and viscous forces are small, while [Coriolis force](physics.md#coriolis-force), [pressure](thermodynamics.md#pressure), [buoyancy](fluid-mechanics.md#buoyancy) and [Lorentz force density](electromagnetism.md#lorentz-force-density) remain significant. The [Rossby number](geophysical-fluid-dynamics.md#rossby-number) and [Ekman number](geophysical-fluid-dynamics.md#ekman-number) measure the omitted inertia and bulk viscosity. Rotation does not balance an arbitrary magnetic torque: impenetrable axisymmetric boundaries impose the [Taylor constraint](#taylor-constraint). Magnetic diffusion can remain in the induction equation even when viscosity is neglected in momentum balance.

#### Taylor constraint

↑ **Parent:** [Magnetostrophic balance](#magnetostrophic-balance)

In inviscid [magnetostrophic balance](#magnetostrophic-balance) within an impenetrable axisymmetric container, with no azimuthal buoyancy or external mechanical torque, the cylindrically integrated [Lorentz force density](electromagnetism.md#lorentz-force-density) must vanish on every cylinder coaxial with rotation. The azimuthal pressure derivative integrates to zero, and the cylindrical Coriolis integral is proportional to net radial flux, zero by incompressibility and impermeability. Multiplying by cylinder area and lever arm gives the equivalent zero-torque form. This rotating-fluid condition is distinct from magnetic-helicity relaxation to a force-free plasma state. Its original primary source is [Taylor's 1963 rotating-fluid paper](https://mhd.ens.fr/IHP09/Jackson/Biblio/taylor_63.pdf).

##### Viscous regularization of the Taylor constraint

↑ **Parent:** [Taylor constraint](#taylor-constraint)

With small viscosity, the azimuthal cylindrical balance permits [Lorentz force](electromagnetism.md#lorentz-force) torque to be cancelled by viscous stress. For ordinary no-slip rotating boundaries an [Ekman layer](geophysical-fluid-dynamics.md#ekman-layer) gives stress of order $\rho\Omega LU\sqrt E$, larger than the order-$E$ bulk viscous correction at fixed velocity. Thus bounded small-$E$ flows approach a [magnetostrophic Taylor state](#magnetostrophic-taylor-state) but need not satisfy its constraint exactly at finite viscosity. An order-one uncompensated magnetic torque would require a divergent flow as $E\to0$, invalidating the assumed small-inertia balance. Stress-free boundaries remove the leading no-slip friction and require their own torque/regularity conditions.

##### Geostrophic flow preserving the Taylor constraint

↑ **Parent:** [Taylor constraint](#taylor-constraint)

For an instantaneous [magnetostrophic Taylor state](#magnetostrophic-taylor-state), the momentum equation leaves a geostrophic null component $u_g=s\omega(s)\hat\phi$. Decompose the velocity into this component and a particular ageostrophic flow, substitute the induction equation into the displayed derivative constraint, and solve the resulting linear equation for $\omega$ with magnetic boundary conditions imposed. When magnetic surface torque vanishes, the geostrophic part is $\mu_0^{-1}\partial_s[s^3\int_{C_s}B_s^2d\phi dz\,\omega']$. Boundary terms generally cannot be discarded for an insulating exterior; the primary analysis is [Hardy and collaborators' boundary-compatible geostrophic-flow construction](https://arxiv.org/abs/1806.06612). Regularity and an angular-momentum normalization fix remaining homogeneous freedoms when the magnetic coupling is nondegenerate.

##### Magnetostrophic Taylor state

↑ **Parent:** [Taylor constraint](#taylor-constraint)

A divergence-free [magnetic field](electromagnetism.md#magnetic-field) satisfying the [Taylor constraint](#taylor-constraint) on all geostrophic cylinders. It is a compatibility condition for slow rotating-fluid balance, not a local force-free condition. To retain such a state as magnetic induction proceeds, the velocity must also preserve the time derivative of the cylindrical torque constraint.

### Mean-field electrodynamics

↑ **Parent:** [Magnetohydrodynamics](#magnetohydrodynamics)

[Mean-field electrodynamics](#mean-field-electrodynamics) applies averaging and a response closure to magnetic induction in a fluctuating conducting fluid. The mean equation contains the correlated [mean-field electromotive force](#mean-field-electromotive-force) in the title. Scale separation permits a local expansion into alpha transport, [turbulent diffusion](turbulence.md#eddy-diffusion) and higher gradients; general anisotropic or finite-memory statistics require tensorial and nonlocal responses. A [mean-field dynamo](#mean-field-dynamo) is a self-exciting application of this framework, not a consequence of averaging alone.

### Kinematic magnetic dynamo

↑ **Parent:** [Magnetohydrodynamics](#magnetohydrodynamics)

A [kinematic magnetic dynamo](#kinematic-magnetic-dynamo) studies [magnetic field](electromagnetism.md#magnetic-field) amplification by a prescribed [fluid flow](fluid-mechanics.md#fluid-flow), neglecting the field's feedback on the velocity through the [Lorentz force](electromagnetism.md#lorentz-force). With incompressibility and zero [magnetic diffusivity](#magnetic-diffusivity), a Lagrangian field vector evolves by its local velocity-gradient matrix. A growth law derived in this approximation cannot hold indefinitely once magnetic stresses significantly change the flow.

#### Gaussian white-noise magnetic stretching

↑ **Parent:** [Kinematic magnetic dynamo](#kinematic-magnetic-dynamo)

For a trace-free isotropic [Gaussian white noise](stochastic-process.md#gaussian-white-noise) velocity gradient with covariance $\langle\sigma_{im}(t)\sigma_{jn}(t')\rangle=\kappa_2\delta(t-t')[\delta_{ij}\delta_{mn}-(\delta_{im}\delta_{jn}+\delta_{in}\delta_{jm})/4]$, interpret the multiplicative equation as the [Stratonovich integral](stochastic-calculus.md#stratonovich-integral) limit of smooth velocity fluctuations. The causal [Furutsu–Novikov formula](stochastic-process.md#novikov-s-theorem) has endpoint weight one half. It gives $P_t=(\kappa_2/2)\partial_i[(B^2\delta_{ij}-B_iB_j/2)\partial_jP]$ for the vector [probability density function](continuous-probability-distribution.md#probability-density-function).

##### Lognormal magnetic-field amplification

↑ **Parent:** [Gaussian white-noise magnetic stretching](#gaussian-white-noise-magnetic-stretching)

Set $x=\ln(B/B_0)$ and $f=BF$ in the [radial magnetic-field Fokker-Planck equation](#radial-magnetic-field-fokker-planck-equation). Then $f_t=Df_{xx}-3Df_x$, so $f$ is a [Gaussian distribution](probability-theory.md#normal-distribution) drifting at speed $3D$. For initial magnitude $B_0>0$, $F=[B\sqrt{4\pi Dt}]^{-1}\exp[-(\ln(B/B_0)-3Dt)^2/(4Dt)]$. This [lognormal distribution](probability-theory.md#log-normal-distribution) has moments $B_0^q e^{Dq(q+3)t}$; the width of its logarithm grows as $\sqrt{2Dt}$.

##### Magnetic stretching moment growth

↑ **Parent:** [Gaussian white-noise magnetic stretching](#gaussian-white-noise-magnetic-stretching)

Twice integrating the [radial magnetic-field Fokker-Planck equation](#radial-magnetic-field-fokker-planck-equation) by parts gives the displayed law when moments and endpoint terms are controlled. In particular $\langle B^2\rangle$ grows at rate $10D=2\gamma$, with $\gamma=5\kappa_2/4$. The corresponding [magnetic energy](electromagnetism.md#magnetic-energy) density is $\langle B^2\rangle/(8\pi)$ in [Gaussian units](electromagnetism.md#gaussian-units).

##### Radial magnetic-field Fokker-Planck equation

↑ **Parent:** [Gaussian white-noise magnetic stretching](#gaussian-white-noise-magnetic-stretching)

For an isotropic initial ensemble in [Gaussian white-noise magnetic stretching](#gaussian-white-noise-magnetic-stretching), $F(B)=4\pi B^2P(B)$ is the magnitude [probability density function](continuous-probability-distribution.md#probability-density-function). The radial vector equation $P_t=D(B^2P_{BB}+4BP_B)$ gives the displayed conservative [Fokker-Planck equation](probability-theory.md#fokker-planck-equation). Its integral is conserved under zero endpoint probability flux. For an anisotropic initial vector distribution, use the angularly averaged magnitude density instead; isotropic noise alone does not make arbitrary initial data isotropic.

### Theta pinch

↑ **Parent:** [Magnetohydrodynamics](#magnetohydrodynamics)

A [theta pinch](#theta-pinch) is a cylindrical plasma configuration with axial [magnetic field](electromagnetism.md#magnetic-field) and azimuthal [electric current](electromagnetism.md#electric-current). For a static equilibrium without gravity, the radial [Lorentz force](electromagnetism.md#lorentz-force) gives $d[p+B^2/(8\pi)]/dr=0$ in [Gaussian units](electromagnetism.md#gaussian-units). This straight-field configuration has no field-line curvature drive of the usual interchange instability.

#### Positive ideal energy of a theta pinch

↑ **Parent:** [Theta pinch](#theta-pinch)

For an admissible Fourier [fluid Lagrangian displacement](fluid-mechanics.md#lagrangian-displacement-fluid-mechanics) $\boldsymbol\xi(r)e^{im\theta+ikz}$, put $D_\perp=(r\xi_r)'/r+im\xi_\theta/r$ and $D=D_\perp+ik\xi_z$. Force balance cancels every magnetic-field-gradient cross term in the [magnetohydrodynamic energy principle](#magnetohydrodynamic-energy-principle), leaving an integrand $\gamma p|D|^2+B^2[|D_\perp|^2+k^2(|\xi_r|^2+|\xi_\theta|^2)]/(4\pi)$. For $p\ge0$, $\gamma>0$, this is nonnegative. Neutral displacements can exist, so stability here means absence of negative-energy exponentially growing ideal modes, not strictly positive energy for every displacement.

### Hall magnetohydrodynamics

↑ **Parent:** [Magnetohydrodynamics](#magnetohydrodynamics)

[Hall magnetohydrodynamics](#hall-magnetohydrodynamics) retains bulk [ion](chemistry.md#ion) inertia but freezes [magnetic flux](electromagnetism.md#magnetic-flux) into the [Electron](physics.md#electron) velocity $\mathbf u_e=\mathbf u-\mathbf j/(en)$. With constant density, negligible [electrical resistivity](electromagnetism.md#electrical-resistivity) and [Electron](physics.md#electron) inertia, [Gaussian units](electromagnetism.md#gaussian-units) give $\mathbf j=c\nabla\times\mathbf B/(4\pi)$ and $\partial_t\mathbf B=\nabla\times[(\mathbf u-c\nabla\times\mathbf B/(4\pi en))\times\mathbf B]$. The [ion](chemistry.md#ion) velocity still satisfies the [magnetohydrodynamic momentum equation](#magnetohydrodynamic-momentum-equation). Neglecting that velocity gives [electron magnetohydrodynamics](#electron-magnetohydrodynamics), a further approximation rather than a synonym for the complete Hall system.

#### Fast-time electron-MHD limit of Hall magnetohydrodynamics

↑ **Parent:** [Hall magnetohydrodynamics](#hall-magnetohydrodynamics)

For field amplitudes of order the guide field, the [ion](chemistry.md#ion) Lorentz-force response over time $\tau$ is $\Delta u/v_A=O(v_A\tau/l)\ll1$. The electron-current velocity is of order $v_Ad_i/l$, larger than a bulk velocity of order $v_A$. Thus the leading [Hall magnetohydrodynamics](#hall-magnetohydrodynamics) induction equation becomes the closed [electron magnetohydrodynamics](#electron-magnetohydrodynamics) equation, while [ions](chemistry.md#ion) remain fixed to leading order on this fast scale. The first nonzero [ion](chemistry.md#ion) response need not have zero acceleration. This limit retains the fast branch of [incompressible Hall-MHD wave dispersion](#incompressible-hall-mhd-wave-dispersion), not the slow branch; very oblique modes must separately satisfy the fast-time ordering.

#### Incompressible Hall-MHD wave dispersion

↑ **Parent:** [Hall magnetohydrodynamics](#hall-magnetohydrodynamics)

For a uniform guide field, write the transverse perturbation in velocity units as $\mathbf b$. Linear momentum gives $\omega\mathbf u=-k_\parallel v_A\mathbf b$. Linear induction gives $\omega\mathbf b=-k_\parallel v_A\mathbf u+i k_\parallel v_Ad_i\mathbf k\times\mathbf b$. The [helicity decomposition of a transverse Fourier mode](special-relativity.md#helicity-decomposition-of-a-transverse-fourier-mode) then yields the displayed [dispersion relation](wave-equation.md#dispersion-relation). Its two positive frequency magnitudes are $|k_\parallel|v_A[\sqrt{1+(kd_i)^2/4}\pm kd_i/2]$, approaching the [Alfvén wave](#alfven-wave) frequency for $kd_i\ll1$. For $kd_i\gg1$, the fast branch is a [whistler wave](#whistler-wave) and the slow branch tends to $|k_\parallel|v_A/(kd_i)$.

### Electron magnetohydrodynamics

↑ **Parent:** [Magnetohydrodynamics](#magnetohydrodynamics)

[Electron magnetohydrodynamics](#electron-magnetohydrodynamics) neglects [ion](chemistry.md#ion) motion and [Electron](physics.md#electron) inertia while retaining transport of the [magnetic field](electromagnetism.md#magnetic-field) by the [Electron](physics.md#electron) current. At constant [Electron](physics.md#electron) [number density](statistical-physics.md#number-density), $\mathbf u_e=-\mathbf J/(en)=-c\nabla\times\mathbf B/(4\pi en)$. Flux freezing in this [velocity](classical-mechanics.md#velocity) gives

$$
\partial_t\mathbf B=-\frac c{4\pi en}\nabla\times[(\nabla\times\mathbf B)\times\mathbf B].
$$

For a uniform guide field, the [solenoidal](calculus.md#solenoidal-vector-field) linear equation implies $\omega^2=(cB_0/4\pi en)^2k_\parallel^2k^2$. With $v_A=B_0/\sqrt{4\pi nm_i}$ and $d_i=c\sqrt{m_i/(4\pi e^2n)}$, the coefficient is $cB_0/(4\pi en)=v_Ad_i$.

#### Whistler wave

↑ **Parent:** [Electron magnetohydrodynamics](#electron-magnetohydrodynamics)

In the inertia-free, constant-density [electron magnetohydrodynamics](#electron-magnetohydrodynamics) model with uniform guide field $B_0\hat{\mathbf z}$, a transverse magnetic [plane wave](quantum-mechanics.md#plane-wave) obeys $\omega\mathbf b=i v_Ad_i k_\parallel\mathbf k\times\mathbf b$. The [helicity decomposition of a transverse Fourier mode](special-relativity.md#helicity-decomposition-of-a-transverse-fourier-mode) gives the displayed dispersive branches with opposite [circular polarizations](electromagnetism.md#circular-polarization). This electron-current mode is called a whistler wave; see [Lyutikov's analysis of electron magnetohydrodynamics](https://arxiv.org/abs/1306.4544). Its pressure-free induction equation should not be identified with a general kinetic Alfvén model.

#### Reduced electron magnetohydrodynamics

↑ **Parent:** [Electron magnetohydrodynamics](#electron-magnetohydrodynamics)

With $k_\parallel/k_\perp\sim\delta B/B_0\ll1$, define $b=\delta B_\parallel/B_0$ and $\delta\mathbf B_\perp/B_0=\hat{\mathbf z}\times\nabla_\perp\Psi/v_A$ to leading order. Let $\nabla_\parallel=\partial_z+\{\Psi,\cdot\}/v_A$, where $\{f,g\}=f_xg_y-f_yg_x$. The leading [Electron](physics.md#electron) [velocities](classical-mechanics.md#velocity) are $\mathbf u_{e\perp}=v_Ad_i\hat{\mathbf z}\times\nabla_\perp b$ and $u_{e\parallel}=-d_i\nabla_\perp^2\Psi$. Substitution into frozen-in induction yields

$$
\partial_t\Psi=v_A^2d_i\nabla_\parallel b,\qquad \partial_tb=-d_i\nabla_\parallel\nabla_\perp^2\Psi.
$$

[Linearization](algebra.md#linearization) gives $\omega^2=v_A^2d_i^2k_\parallel^2k_\perp^2$, agreeing with the full [EMHD](#electron-magnetohydrodynamics) relation to leading anisotropic order. If $b$ varies along the guide field, an order-smaller perpendicular gradient correction restores exact solenoidality; the two-field representation is not an exact decomposition at arbitrary anisotropy.

### Stratified magneto-Coriolis wave

↑ **Parent:** [Magnetohydrodynamics](#magnetohydrodynamics)

An incompressible [Boussinesq](geophysical-fluid-dynamics.md#boussinesq-approximation) fluid with uniform [magnetic field](electromagnetism.md#magnetic-field), uniform vertical [rotation](riemannian-geometry.md#rotation-mathematics) and uniform temperature gradient supports waves combining [magnetic tension](#magnetic-tension), [Coriolis force](physics.md#coriolis-force) and [buoyancy](fluid-mechanics.md#buoyancy). Put $K=|\mathbf k|$, $h^2=K^2-k_z^2$, $a^2=(\mathbf B\cdot\mathbf k)^2/(\mu_0\rho)$ and $H=g\alpha\beta$, with $\partial_zT_0=-\beta$. Eliminating [pressure](thermodynamics.md#pressure) and the temperature and magnetic perturbations gives the displayed [dispersion relation](wave-equation.md#dispersion-relation) for nonzero frequencies. Stable thermal stratification has $H<0$. Clearing frequency denominators requires checking any resulting zero roots in the original equations; a stationary magnetostatic-buoyancy balance can exist independently of the propagating branches.

#### Rapid-rotation slow magneto-Coriolis branch

↑ **Parent:** [Stratified magneto-Coriolis wave](#stratified-magneto-coriolis-wave)

For fixed wavevector with $k_z\ne0$, fixed nonzero [Alfvén frequency](#alfven-frequency) $a$, and $|\Omega|\to\infty$, the two roots in $X=\omega^2$ of the [stratified magneto-Coriolis wave](#stratified-magneto-coriolis-wave) polynomial have $X_f\sim4\Omega^2k_z^2/K^2$ and the displayed slow root. This follows from the sum of roots being $4\Omega^2k_z^2/K^2+O(1)$ and their product being $a^2(K^2a^2-Hh^2)/K^2$. The slow branch is oscillatory for $K^2a^2>Hh^2$ and growing or decaying for the reversed inequality. At equality its frequency vanishes and the original stationary equations must be used.

### Lehnert number

↑ **Parent:** [Magnetohydrodynamics](#magnetohydrodynamics)

The Lehnert number compares an [Alfvén speed](#alfven-speed) to a rotation speed on length scale $L$. With $\mathrm{Le}\ll1$, magnetic-wave frequencies are small compared with the rotation frequency, allowing nearly [geostrophic flow](geophysical-fluid-dynamics.md#geostrophic-flow). Ideal weakly damped magnetic waves also require $\eta/L^2$ and $\nu/L^2$ to be small compared with their wave frequency; a small Lehnert number alone does not guarantee weak diffusion.

### Magnetohydrodynamic momentum equation

↑ **Parent:** [Magnetohydrodynamics](#magnetohydrodynamics)

For constant [mass density](fluid-mechanics.md#density) $\rho$, [kinematic viscosity](fluid-mechanics.md#kinematic-viscosity) $\nu$ and [magnetic permeability](electromagnetism.md#permeability-electromagnetism) $\mu_0$, the incompressible momentum equation is

$$
\partial_t\mathbf u+(\mathbf u\cdot\nabla)\mathbf u=-\rho^{-1}\nabla p+(\mu_0\rho)^{-1}(\nabla\times\mathbf B)\times\mathbf B+\nu\nabla^2\mathbf u.
$$

It is the [Navier-Stokes equation](viscous-fluid-flow.md#navier-stokes-equation) with [Lorentz force density](electromagnetism.md#lorentz-force-density). The magnetic force decomposes into [magnetic tension](#magnetic-tension) and a [magnetic pressure](#magnetic-pressure) gradient. A uniform streamwise pressure gradient need not make ordinary pressure independent of transverse coordinates.

### Resistive magnetohydrodynamics

↑ **Parent:** [Magnetohydrodynamics](#magnetohydrodynamics)

Resistive magnetohydrodynamics retains finite [magnetic diffusivity](#magnetic-diffusivity) in the coupled evolution of a conducting fluid and its [magnetic field](electromagnetism.md#magnetic-field). The [resistive induction equation](#resistive-induction-equation) allows field diffusion relative to the fluid, while the [magnetohydrodynamic momentum equation](#magnetohydrodynamic-momentum-equation) includes the [Lorentz force density](electromagnetism.md#lorentz-force-density). It contrasts with the zero-diffusivity limit of [ideal magnetohydrodynamics](#ideal-magnetohydrodynamics).

#### Magnetic reconnection

↑ **Parent:** [Resistive magnetohydrodynamics](#resistive-magnetohydrodynamics)

Magnetic reconnection changes connectivity between [magnetic field lines](electromagnetism.md#magnetic-field-line). It requires departure from smooth [magnetic flux freezing](#magnetic-flux-freezing), for example through finite resistivity or other nonideal terms concentrated in a [current sheet](electromagnetism.md#current-sheet). Ideal viscous [magnetic relaxation](#magnetic-relaxation) dissipates mechanical energy while retaining frozen connectivity, so viscosity alone does not provide reconnection.

#### Magnetic skin layer

↑ **Parent:** [Resistive magnetohydrodynamics](#resistive-magnetohydrodynamics)

A magnetic skin layer is the thin region penetrated by an oscillating [magnetic field](electromagnetism.md#magnetic-field) in a conductor. For locally tangential boundary amplitude $C(x)$, negligible material motion and variations along the boundary much slower than those across it, the [resistive induction equation](#resistive-induction-equation) gives $B_x=C(x)e^{-(1+i)y/\delta}$ with time convention $e^{i\omega t}$. The [solenoidal magnetic-field constraint](electromagnetism.md#solenoidal-magnetic-field-constraint) requires the smaller component $B_y=C'(x)e^{-(1+i)y/\delta}\delta/(1+i)$ to leading order. The tangential-field approximation therefore does not mean that the normal component is exactly zero at finite [magnetic diffusivity](#magnetic-diffusivity).

##### Magnetic skin-layer streaming slip

↑ **Parent:** [Magnetic skin layer](#magnetic-skin-layer)

In a thin [magnetic skin layer](#magnetic-skin-layer) next to a rigid [no-slip boundary condition](viscous-fluid-flow.md#no-slip-boundary-condition), vertical [pressure](thermodynamics.md#pressure) balance gives $p=P-C^2e^{-2y/\delta}/(4\mu_0)$. With negligible inertia in the layer, the tangential [Stokes flow](stokes-flow.md) balance is $\rho\nu u_{yy}=p_x$. Matching zero leading shear outside the layer gives $u=U(1-e^{-2y/\delta})$ and the displayed effective tangential slip. The physical wall still has zero [velocity](classical-mechanics.md#velocity); the slip is a boundary condition for the outer flow extrapolated through the unresolved layer. It points toward larger squared boundary-field amplitude.

##### Mean Lorentz force in a magnetic skin layer

↑ **Parent:** [Magnetic skin layer](#magnetic-skin-layer)

For real boundary amplitude $C$ and $q=(1+i)/\delta$, the leading [electric current density](electromagnetism.md#current-density) is $j_z=qCe^{-qy}/\mu_0$. Averaging products of real harmonic fields gives $\overline{\mathbf F}=\operatorname{Re}[(\nabla\times\mathbf B)\times\mathbf B^*]/(2\mu_0)$. Its leading normal component is the displayed positive force. The first candidate tangential contribution is proportional to $\operatorname{Re}(q/q^*)CC'=0$, so retaining the small normal field does not introduce a tangential force of that order.

#### Flux expulsion

↑ **Parent:** [Resistive magnetohydrodynamics](#resistive-magnetohydrodynamics)

Flux expulsion is redistribution of [magnetic flux](electromagnetism.md#magnetic-flux) out of the interiors of persistent circulating flows into their edges and surrounding regions. In two-dimensional [incompressible flow](fluid-mechanics.md#incompressible-flow), a magnetic flux function obeys $\partial_t A+\mathbf u\cdot\nabla A=\eta\nabla^2 A$. At large but finite [magnetic Reynolds number](#magnetic-reynolds-number), circulation stretches gradients of $A$, enabling resistive smoothing and weak interior [magnetic field](electromagnetism.md#magnetic-field) with strong field near the circulation boundary. Finite [magnetic diffusivity](#magnetic-diffusivity) is essential to the eventual rearrangement; exact ideal [magnetic flux freezing](#magnetic-flux-freezing) alone does not justify a flux-free steady cell. Magnetic back reaction can limit the process.

##### Phase mixing in magnetic flux expulsion

↑ **Parent:** [Flux expulsion](#flux-expulsion)

Differential circulation of a weak [magnetic field](electromagnetism.md#magnetic-field) winds its flux function into progressively smaller radial scales. In a smooth eddy with angular-velocity gradient of order $U/L^2$, its radial wavenumber grows as $k_r\sim Ut/L^2$. Resistive damping becomes substantial when $\eta\int_0^t k_r^2dt\sim1$, giving $t\sim(L^4/(\eta U^2))^{1/3}=(L/U)\mathrm{Rm}^{1/3}$. This estimate presumes differential rotation and negligible magnetic feedback; a rigidly rotating eddy does not create this phase mixing. Finite [magnetic diffusivity](#magnetic-diffusivity) then permits weak interior field and boundary concentration, unlike exact ideal flux freezing.

###### Cubic-time resistive damping in a differentially rotating cell

↑ **Parent:** [Phase mixing in magnetic flux expulsion](#phase-mixing-in-magnetic-flux-expulsion)

In a smooth interior region with locally constant shear $\Omega'$, a wound azimuthal [Fourier mode](fourier-analysis.md#fourier-mode) has radial [wavenumber](wave-equation.md#wavenumber) $k_s\simeq-m\Omega't$. Integrating its resistive damping rate $\eta k_s^2$ gives the [exponential decay](analysis.md#exponential-decay) in the title. The characteristic time is $\tau_c=[3/(\eta m^2\Omega'^2)]^{1/3}$. For $m=1$ and $\Omega'=-\Omega_0/d$, $\Omega_0\tau_c=(3\mathrm{Rm})^{1/3}$, where $\mathrm{Rm}=\Omega_0d^2/\eta$. This is a high-[magnetic Reynolds number](#magnetic-reynolds-number) interior transient on a time long compared with the rotation time but short compared with $d^2/\eta$. Physical [magnetic field](electromagnetism.md#magnetic-field) components may have additional algebraic factors from taking [derivatives](calculus.md#derivative) of the wound [magnetic vector potential](electromagnetism.md#magnetic-vector-potential). A maintained exterior field, an axial core and a circulation-edge [boundary layer](continuum-mechanics.md#boundary-layer) prevent interpreting this estimate as an exact, uniform, infinite-time solution.

#### Dynamo action

↑ **Parent:** [Resistive magnetohydrodynamics](#resistive-magnetohydrodynamics)

Dynamo action is growth or sustained maintenance of a [magnetic field](electromagnetism.md#magnetic-field) by conducting-fluid motion despite magnetic diffusion. In the kinematic problem the velocity is prescribed and the [resistive induction equation](#resistive-induction-equation) is linear in the [magnetic field](electromagnetism.md#magnetic-field). Magnetic feedback through the [Lorentz force density](electromagnetism.md#lorentz-force-density) matters once the field becomes dynamically important.

##### Radial-flow dynamo energy bound

↑ **Parent:** [Dynamo action](#dynamo-action)

Let a [solenoidal](calculus.md#solenoidal-vector-field) flow be confined to a sphere $V$, with the [insulating boundary condition for the radial magnetic scalar](#insulating-boundary-condition-for-the-radial-magnetic-scalar). Define $N=\int_VP^2$, $D=\int_{\mathbb R^3}|\nabla P|^2$, $M=\int_{\mathbb R^3}|\mathbf B|^2$ and $q=\max_V|\mathbf u\cdot\mathbf x|$. [Integration by parts](calculus.md#integration-by-parts) inside and outside the sphere gives

$$
\frac12N'=-\int_VQ\,\mathbf B\cdot\nabla P-\eta D\leq q\sqrt{MD}-\eta D.
$$

The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) therefore makes $q^2\geq\eta^2D/M$ necessary whenever $N'\geq0$ and $D>0$. A uniform strict violation with a positive gap forces decay, using a [Sobolev inequality](sobolev-space.md#sobolev-inequality) to bound $N$ by a constant times $D$. A bounded statistically steady field instead requires $q_*^2\geq\eta^2\langle D\rangle/\langle M\rangle$, with $q_*=\sup_tq(t)$. This is a necessary condition for [dynamo action](#dynamo-action), not a sufficient criterion or a pointwise assertion at every instant of an arbitrary time-dependent solution.

// Target: analysis.bigb

##### Dynamo quenching

↑ **Parent:** [Dynamo action](#dynamo-action)

[Dynamo quenching](#dynamo-quenching) is the reduction or modification of magnetic-field generation by magnetic feedback on the generating flow and its correlations. The [Lorentz force](electromagnetism.md#lorentz-force) can change shear or turbulence, while [magnetic helicity](electromagnetism.md#magnetic-helicity) affects mean-field regeneration. A phenomenological [scalar](vector-space.md#scalar) example is $\alpha(B)=\alpha_0/(1+B^2/B_*^2)$. In the illustrative amplitude equation $\dot B=[c\alpha(B)-d]B$ with $c,d>0$, a growing field saturates at $B^2=B_*^2(c\alpha_0/d-1)$ when $c\alpha_0>d$. This demonstrates the negative feedback mechanism without claiming that algebraic quenching is a complete solar closure.

###### Algebraic alpha quenching

↑ **Parent:** [Dynamo quenching](#dynamo-quenching)

Algebraic alpha quenching prescribes a field-dependent [alpha effect](#alpha-effect) as a closure for nonlinear [mean-field dynamo](#mean-field-dynamo) feedback. The polynomial law $\alpha=\alpha_0-p|B|^2$ with $p>0$ decreases alpha, so it can saturate positive alpha but makes negative alpha more negative. It therefore differs importantly from the sign-preserving rational law $\alpha_0/(1+|B|^2/B_*^2)$. Its solutions must satisfy nonnegative squared-amplitude conditions; an assertion based only on large $|\alpha_0|$ need not hold for both signs.

###### Alpha-quenching rotating wave

↑ **Parent:** [Algebraic alpha quenching](#algebraic-alpha-quenching)

A rotating wave in a complex [dynamo quenching](#dynamo-quenching) model has constant amplitude and a common phase factor $e^{i\omega t}$. In the two-hemisphere model with toroidal coupling parameter $\epsilon_2=0$, eliminating the poloidal amplitudes gives

$$
\frac{2\omega-i(1-\omega^2)}{\Omega}\begin{pmatrix}B_1\\B_2\end{pmatrix}=\begin{pmatrix}\alpha_0-p|B_1|^2&\epsilon_1\\\epsilon_1&\alpha_0-p|B_2|^2\end{pmatrix}\begin{pmatrix}B_1\\B_2\end{pmatrix}.
$$

The matrix is [Hermitian](hilbert-space.md#hermitian-operator), so its [eigenvalue](linear-operator-theory.md#eigenvalue) is real and a nonzero rotating wave with $\Omega\ne0$ has $\omega=\pm1$. Writing $a=\alpha_0-2\omega/\Omega$, pure dipole and quadrupole waves have $|B_j|^2=(a-\epsilon_1)/p$ and $(a+\epsilon_1)/p$, respectively, when those quantities are positive.

###### Unequal-hemisphere dynamo rotating wave

↑ **Parent:** [Alpha-quenching rotating wave](#alpha-quenching-rotating-wave)

For nonzero coupling $\epsilon_1$, an [alpha-quenching rotating wave](#alpha-quenching-rotating-wave) can be made real in its toroidal amplitudes by a common phase rotation. Set $a=\alpha_0-2\omega/\Omega$. The amplitude equations are $(a-pB_1^2)B_1+\epsilon_1B_2=0$ and $(a-pB_2^2)B_2+\epsilon_1B_1=0$. Subtracting after cross multiplication gives $(B_1^2-B_2^2)(pB_1B_2+\epsilon_1)=0$. Unequal magnitudes therefore require $B_1B_2=-\epsilon_1/p$ and $B_1^2+B_2^2=a/p$. They exist exactly when $a>2|\epsilon_1|$ and have the displayed squared amplitudes. Exchanging hemispheres yields the companion solution. This breaks equatorial reflection symmetry and combines both [dipole and quadrupole parity in a mean-field dynamo](#dipole-and-quadrupole-parity-in-a-mean-field-dynamo). Existence does not alone prove nonlinear stability.

##### Equivariant three-mode dynamo normal form

↑ **Parent:** [Dynamo action](#dynamo-action)

An axisymmetric magnetic mode is unchanged by axial rotations, while an equatorial magnetic mode and a corresponding velocity mode transform as $A,V\mapsto e^{i\theta}(A,V)$. Magnetic reversal sends $(B,A,V)$ to $(-B,-A,V)$. For magnetic evolution linear in magnetic amplitudes, rotational [equivariance](group-theory.md#equivariant-map) requires $\dot B=Bf(|V|^2)+2\operatorname{Re}[A^*Vg(|V|^2)]$ and $\dot A=Ah(|V|^2)+BVj(|V|^2)+A^*V^2\ell(|V|^2)$, with $f$ real and the other functions complex. Velocity monomials $B^pA^q(A^*)^rV^s(V^*)^t$ must have even $p+q+r$ and weight $q-r+s-t=1$. These conditions enumerate the cubic [normal form](dynamical-systems.md#normal-form-dynamical-systems) without assuming reflection symmetry or nonlinear magnetic self-interactions.

###### Magnetic onset on a rotating velocity branch

↑ **Parent:** [Equivariant three-mode dynamo normal form](#equivariant-three-mode-dynamo-normal-form)

For real $c_2,d_4$ and the simplified magnetic amplitude equations, the pure-velocity branch is $V=se^{i\omega_3t}$ with $A=B=0$. In its rotating frame the magnetic linearization on $(B,\operatorname{Re}A,\operatorname{Im}A)$ has rows $(\mu_1-es^2,2s,0)$, $(c_2s,\mu_2,-\Delta)$ and $(0,\Delta,\mu_2)$, where $\Delta=\omega_2-\omega_3$. Its zero determinant gives the displayed onset relation. A nonzero magnetic branch needs a kernel involving both magnetic amplitudes, a transverse parameter crossing and nondegenerate nonlinear saturation; determinant zero alone is insufficient in degenerate cases.

###### Normalization of nonzero dynamo coupling coefficients

↑ **Parent:** [Equivariant three-mode dynamo normal form](#equivariant-three-mode-dynamo-normal-form)

For nonzero coefficients of $A^*V$ in $\dot B$ and $AB$ in $\dot V$, a relative phase rotation makes $c_1$ real positive. Positive rescalings of $A,V,B$ then normalize both magnitudes to one. The phase of $c_1c_3$ is invariant under these rescalings and remains as the phase of normalized $c_3$. Zero couplings cannot be normalized to one; they are degenerate parameter cases.

##### Anti-dynamo theorem

↑ **Parent:** [Dynamo action](#dynamo-action)

An anti-dynamo theorem gives a geometric or analytic restriction excluding self-sustained [dynamo action](#dynamo-action) under stated [magnetic diffusivity](#magnetic-diffusivity), domain and boundary conditions. It excludes regeneration against resistive decay, not all transient amplification or field induced by an external source. Important restrictions include [Cowling anti-dynamo theorem](#cowling-anti-dynamo-theorem), the [toroidal-velocity anti-dynamo theorem](#toroidal-velocity-anti-dynamo-theorem), and the [planar anti-dynamo theorem](#planar-anti-dynamo-theorem). [Backus' necessary condition for dynamo action](#backus-necessary-condition-for-dynamo-action) instead bounds the stretching required for possible regeneration.

###### Periodic two-coordinate anti-dynamo energy bound

↑ **Parent:** [Anti-dynamo theorem](#anti-dynamo-theorem)

For a solenoidal three-component velocity depending on two periodic coordinates and a zero-mean magnetic field with the same dependence, the in-plane flux potential satisfies a homogeneous [advection-diffusion equation](diffusion-equation.md#advection-diffusion-equation). The [Poincaré inequality](sobolev-space.md#poincare-inequality) gives $\langle A^2\rangle\leq\langle A_0^2\rangle e^{-2\eta k^2t}$. Integrating the vertical stretching term by parts bounds it by $Q\sqrt{\langle A^2\rangle\langle|\nabla B_z|^2\rangle}$, where $Q=\|\nabla u_z\|_\infty$. Maximizing against resistive dissipation and integrating gives the displayed transient bound. Splitting off half the dissipation instead gives $E'+\eta k^2E\leq(Q^2/\eta)\langle A_0^2\rangle e^{-2\eta k^2t}$, proving vertical energy decays. This permits transient generation by a nonzero vertical velocity while excluding sustained fields in this zero-mean, z-independent periodic class.

###### Planar anti-dynamo theorem

↑ **Parent:** [Anti-dynamo theorem](#anti-dynamo-theorem)

In the standard two-dimensional setting, with planar [velocity](classical-mechanics.md#velocity) and [magnetic field](electromagnetism.md#magnetic-field) independent of the third coordinate and homogeneous energy-closed boundary conditions, the in-plane magnetic potential is an advected diffusing scalar. Its quadratic integral decreases, preventing regeneration of a dynamo field. A third field component independent of that coordinate also obeys a passive advection-diffusion equation. A flow depending on two coordinates but possessing a third velocity component is not covered by this strictly planar formulation.

###### Zeldovich planar flux balance

↑ **Parent:** [Planar anti-dynamo theorem](#planar-anti-dynamo-theorem)

For a stationary planar advected magnetic flux potential, average its [advection-diffusion equation](diffusion-equation.md#advection-diffusion-equation) horizontally and split it into mean and fluctuation. The mean transport is $\overline{wa'}=\eta\bar a_z+C$, with $C=\langle wa'\rangle$. Multiplying the fluctuation equation by $a'$ and applying [integration by parts](calculus.md#integration-by-parts) gives $\langle\overline{wa'}\bar a_z\rangle+B_0C=-\eta\langle|\nabla a'|^2\rangle$. A vanishing mean derivative removes the constant term in the first correlation, yielding the displayed dissipative identity. The boundary assumptions must eliminate surface terms; a periodic layer replaces, rather than accompanies, decay at vertical infinity.

###### Toroidal-velocity anti-dynamo theorem

↑ **Parent:** [Anti-dynamo theorem](#anti-dynamo-theorem)

For a bounded conducting sphere with uniform [magnetic diffusivity](#magnetic-diffusivity) and an insulating exterior, an [incompressible flow](fluid-mechanics.md#incompressible-flow) tangent to concentric spheres cannot sustain [dynamo action](#dynamo-action). Neither the [velocity](classical-mechanics.md#velocity) nor the [magnetic field](electromagnetism.md#magnetic-field) needs to be axisymmetric. The radial magnetic scalar has a homogeneous advection-diffusion equation, so the poloidal field decays. Once it is absent, the toroidal magnetic potential also has a homogeneous scalar advection-diffusion equation. This is a theorem about spherical flow geometry, not about a general cylindrical flow with an axial component.

###### Cowling anti-dynamo theorem

↑ **Parent:** [Anti-dynamo theorem](#anti-dynamo-theorem)

An isolated axisymmetric [magnetic field](electromagnetism.md#magnetic-field) cannot be sustained by ordinary resistive [dynamo action](#dynamo-action) with scalar positive [magnetic diffusivity](#magnetic-diffusivity). Its [poloidal magnetic flux function](#poloidal-magnetic-flux-function) satisfies a homogeneous scalar advection-diffusion equation with no toroidal-to-poloidal source. The maximum principle excludes regeneration of that flux; after it decays the toroidal field has no lasting source either. This constrains the symmetry of the field. An [axisymmetric flow](fluid-mechanics.md#axisymmetric-flow) may still generate a nonaxisymmetric field, and a turbulent mean-field electromotive force is not covered by the unmodified scalar-induction proof.

##### Magnetic concentration by an incompressible stagnation flow

↑ **Parent:** [Dynamo action](#dynamo-action)

The linear [incompressible flow](fluid-mechanics.md#incompressible-flow) $\mathbf u=(-\omega x,-\omega y,2\omega z)$ compresses the transverse plane and stretches the axial direction. An axial [magnetic field](electromagnetism.md#magnetic-field) obeys $B_t-\omega rB_r=2\omega B+\eta\Delta_\perp B$. In [ideal magnetohydrodynamics](#ideal-magnetohydrodynamics), its amplitude grows as $e^{2\omega t}$ while its transverse width decreases as $e^{-\omega t}$. Thus its [magnetic energy](electromagnetism.md#magnetic-energy) per unit axial length grows as $e^{2\omega t}$, even when opposite-polarity angular sectors give zero signed [magnetic flux](electromagnetism.md#magnetic-flux). Finite [magnetic diffusivity](#magnetic-diffusivity) limits the amplification of localized finite-flux Gaussian fields.

###### Self-similar magnetic mode in a stagnation flow

↑ **Parent:** [Magnetic concentration by an incompressible stagnation flow](#magnetic-concentration-by-an-incompressible-stagnation-flow)

For [magnetic concentration by an incompressible stagnation flow](#magnetic-concentration-by-an-incompressible-stagnation-flow), one possible normalization gives $(g^2)'=2\eta-2\omega g^2$, $f'/f=2\omega-\lambda\eta/g^2$, and $b''+(q^{-1}+q)b'+(\lambda-m^2/q^2)b=0$. The mode parameter $\lambda$ is not fixed by decay at infinity alone. The regular axisymmetric Gaussian has $\lambda=2$, $b=e^{-q^2/2}$ and conserved axial [magnetic flux](electromagnetism.md#magnetic-flux), with energy proportional to $g^{-2}$. The radial equation also has regular algebraic-tail solutions.

##### Backus' necessary condition for dynamo action

↑ **Parent:** [Dynamo action](#dynamo-action)

For an isolated bounded conductor of uniform [magnetic diffusivity](#magnetic-diffusivity) $\eta>0$, contained in a sphere of radius $R$ and matched to a decaying potential field in an insulating exterior, [dynamo action](#dynamo-action) requires maximum stretching rate $S\geq\eta\pi^2/R^2$. Here $S$ bounds the largest [eigenvalue](linear-operator-theory.md#eigenvalue) of the [rate-of-strain tensor](viscous-fluid-flow.md#strain-rate-tensor) throughout the flow and time. Use fluid boundary conditions eliminating the stretching boundary term, for example a [no-slip boundary condition](viscous-fluid-flow.md#no-slip-boundary-condition), and no imposed energy input. The proof combines the [magnetic free-decay spectral bound](#magnetic-free-decay-spectral-bound) with the [magnetic energy](electromagnetism.md#magnetic-energy) equation. This is a necessary condition, not a sufficiency criterion; changing magnetic boundary conditions changes the spectral constant.

###### Maximum-strain bound on dynamo growth

↑ **Parent:** [Backus' necessary condition for dynamo action](#backus-necessary-condition-for-dynamo-action)

Under the energy-closed boundary assumptions of [Backus' necessary condition for dynamo action](#backus-necessary-condition-for-dynamo-action), the [magnetic energy](electromagnetism.md#magnetic-energy) equation gives $\dot E_B\leq2s(t)E_B$ after discarding nonnegative resistive dissipation. Integrating gives an upper bound by the time average of the largest spatial [eigenvalue](linear-operator-theory.md#eigenvalue) of the [rate-of-strain tensor](viscous-fluid-flow.md#strain-rate-tensor). Thus the field-amplitude exponent is at most its space-time supremum. The exponent of squared energy is twice the field-amplitude exponent.

##### Mean-field dynamo

↑ **Parent:** [Dynamo action](#dynamo-action)

A mean-field dynamo evolves a slowly varying spatially averaged [magnetic field](electromagnetism.md#magnetic-field). Correlations of fluctuating velocity and magnetic field supply a [mean-field electromotive force](#mean-field-electromotive-force). Its local linear response includes the [alpha effect](#alpha-effect); gradients of the mean field can contribute additional transport terms. The distinction between a uniform test field used to measure a response coefficient and a spatially varying mean field used to obtain growth is essential.

###### Mean-field shearing-wave transient amplification

↑ **Parent:** [Mean-field dynamo](#mean-field-dynamo)

For $k(t)=k_0\sqrt{1+(t/T)^2}$, factor resistive damping out of the shearing-mode equations by $R=e^{-D}G$, $S=e^{-D}H$, $D=\eta\int k^2dt$. They imply $G''=\alpha^2k^2G$, so a growing [WKB approximation](analysis.md#wkb-approximation) has $G\propto k^{-1/2}e^{|\alpha|\int kdt}$ and $H\simeq i\operatorname{sgn}(\alpha)kG$. Its [magnetic energy](electromagnetism.md#magnetic-energy) is proportional to $k\exp[2|\alpha|\int kdt-2\eta\int k^2dt]$. At long times the positive quadratic exponent is overtaken by negative cubic resistive damping. A well-separated growing interval exists for sufficiently small positive [magnetic diffusivity](#magnetic-diffusivity), with $\eta k_0/|\alpha|\ll1$ at fixed nonzero $|\alpha|k_0T$, and the displayed leading peak time. This is transient amplification, not an asymptotically self-sustaining dynamo.

###### Dipole and quadrupole parity in a mean-field dynamo

↑ **Parent:** [Mean-field dynamo](#mean-field-dynamo)

In a reflection-symmetric [mean-field dynamo](#mean-field-dynamo) model, dipole parity can be represented by an even poloidal-potential amplitude and an odd toroidal-field amplitude; quadrupole parity reverses these assignments. The names describe the reflection classes appropriate to the model, not arbitrary electric multipoles. A complex amplitude $P=A+iB$ allows a phase rotation by $i$ to interchange the two classes when the unperturbed equations have that phase symmetry.

###### Coupled-hemisphere dynamo parity threshold

↑ **Parent:** [Dipole and quadrupole parity in a mean-field dynamo](#dipole-and-quadrupole-parity-in-a-mean-field-dynamo)

In a two-hemisphere [mean-field dynamo](#mean-field-dynamo), dipole and quadrupole subspaces can reduce to $\dot A=aB-A$, $\dot B=bA-B$, with $(a,b)=(\alpha_0-\epsilon_1,i\Omega-\epsilon_2)$ and $(\alpha_0+\epsilon_1,i\Omega+\epsilon_2)$ respectively. Their [eigenvalues](linear-operator-theory.md#eigenvalue) satisfy $(\lambda+1)^2=ab$. Strict decay is equivalent to $\operatorname{Re}(ab)+[\operatorname{Im}(ab)]^2/4<1$. Thus dipole decay requires $F_d<1$, while quadrupole decay requires $F_q=\Omega^2(\alpha_0+\epsilon_1)^2/4+\epsilon_2(\alpha_0+\epsilon_1)<1$. Their difference is $F_q-F_d=\alpha_0(\Omega^2\epsilon_1+2\epsilon_2)$, which selects the first unstable parity when starting from a state stable in both subspaces.

###### Parity splitting of a mean-field dynamo threshold

↑ **Parent:** [Dipole and quadrupole parity in a mean-field dynamo](#dipole-and-quadrupole-parity-in-a-mean-field-dynamo)

An antisymmetric perturbation can split the thresholds of two degenerate [mean-field dynamo](#mean-field-dynamo) parity classes. At first order, project the perturbation equation onto the adjoint null mode using the [Fredholm alternative](compact-operator.md#fredholm-alternative). If multiplying the unperturbed complex mode by $i$ leaves the parameter-derivative matrix element unchanged but reverses the perturbation matrix element, the two first-order threshold shifts are equal and opposite.

###### Alpha-Omega dynamo

↑ **Parent:** [Mean-field dynamo](#mean-field-dynamo)

An alpha-Omega [mean-field dynamo](#mean-field-dynamo) couples toroidal-field generation by the [Omega effect](#omega-effect) to poloidal-field regeneration by the [alpha effect](#alpha-effect). A simple Fourier model is $\dot A=\alpha_0 f(t)B-\eta k^2A$, $\dot B=ik\Omega A-\eta k^2B$, where $A$ is a component of the [vector potential](calculus.md#vector-potential) for the poloidal field and $B$ is a toroidal-field amplitude. For bounded $|f|\leq1$, the [bounded-modulation alpha-Omega growth estimate](#bounded-modulation-alpha-omega-growth-estimate) controls the maximum amplification.

###### Plane-layer alpha-Omega dynamo threshold

↑ **Parent:** [Alpha-Omega dynamo](#alpha-omega-dynamo)

For a [mean-field dynamo](#mean-field-dynamo) with uniform alpha, shear $\pi V/d$, diffusivity $\eta>0$ and fixed vertical wavenumber $\pi/d$, a horizontal Fourier mode obeys $(s+\eta(k^2+\pi^2/d^2))^2=i\alpha\pi Vk/d$. With $D=\alpha Vd^2/(\pi^2\eta^2)$ and $h=|k|d/\pi$, the growing branch has positive real part exactly when $|D|>2(1+h^2)^2/h$. Differentiation gives $3h^4+2h^2-1=0$, hence $h=1/\sqrt3$. Equality is a neutral oscillation, not exponential growth. The sign of $D$ reverses wave propagation without changing the growth threshold.

###### Alpha-squared Omega dynamo threshold

↑ **Parent:** [Alpha-Omega dynamo](#alpha-omega-dynamo)

For constant coefficients and a transverse wavenumber $\ell\ne0$, a planar [mean-field dynamo](#mean-field-dynamo) retaining both alpha feedback and shear has dispersion $(\sigma+\eta p)^2=\alpha^2p+i\alpha\Omega k$, $p=k^2+\ell^2$. Marginal stability gives $\alpha_m^2=4\eta^4p^4/(4\eta^2p^3+\Omega^2k^2)$. Differentiate with respect to $k^2$: an interior minimum solves $4\eta^2p^3+\Omega^2(3k^2-\ell^2)=0$. Its derivative with respect to $k^2$ is positive, so a unique positive minimizing $k^2$ exists only above the displayed shear threshold. Below it the minimum is at $k=0$. The sign of the marginal oscillation frequency is fixed by $2\eta p\omega=\alpha\Omega k$.

###### Bounded-modulation alpha-Omega growth estimate

↑ **Parent:** [Alpha-Omega dynamo](#alpha-omega-dynamo)

In the two-component [alpha-Omega dynamo](#alpha-omega-dynamo) with $|f(t)|\leq1$, apply the [weighted energy estimate for two coupled modes](differential-equation.md#weighted-energy-estimate-for-two-coupled-modes) with $a=|\alpha_0|$, $c=|k\Omega|$, and $d=\eta k^2$. The field-amplitude growth rate is at most $\sqrt{|\alpha_0\Omega k|}-\eta k^2$. Optimizing over $k$ gives the upper constant $3/2^{8/3}$ multiplying $(\alpha_0^2\Omega^2/\eta)^{1/3}$. The admissible choice $f=1$ gives a lower constant $3/2^{10/3}$, so the maximum possible growth has the displayed scaling. An arbitrary chosen modulation need not grow. The statement concerns the model with freely adjustable wavenumber; physical scale-separation restrictions can constrain that optimization.

###### Omega effect

↑ **Parent:** [Mean-field dynamo](#mean-field-dynamo)

Differential rotation or shear stretches a [poloidal magnetic field](#poloidal-magnetic-field) into a [toroidal magnetic field](#toroidal-magnetic-field). This is the Omega effect. By itself it need not regenerate the poloidal component; the [alpha effect](#alpha-effect) provides one possible feedback mechanism in an [alpha-Omega dynamo](#alpha-omega-dynamo). Without feedback, shear amplification can be transient or algebraic rather than sustained exponential [dynamo action](#dynamo-action).

###### First-order smoothing approximation

↑ **Parent:** [Mean-field dynamo](#mean-field-dynamo)

First-order smoothing neglects the fluctuating nonlinear velocity-magnetic-field product in the fluctuation [resistive induction equation](#resistive-induction-equation), but retains $\langle\mathbf u\times\mathbf b\rangle$ in the [mean-field electromotive force](#mean-field-electromotive-force). For a constant test field it gives $\partial_t\mathbf b-\eta\nabla^2\mathbf b=(\mathbf B_0\cdot\nabla)\mathbf u$. Its validity requires the omitted terms to be small compared with the retained forcing and diffusion terms.

###### Isotropic alpha effect of three helical traveling waves

↑ **Parent:** [First-order smoothing approximation](#first-order-smoothing-approximation)

Three equal-amplitude transverse waves along orthogonal axes, with the same [circular polarization](electromagnetism.md#circular-polarization), each satisfy $\nabla\times\mathbf u_j=\sigma k\mathbf u_j$, $\sigma=\pm1$. Distinct spatial phases have zero cross averages. The periodic [first-order smoothing](#first-order-smoothing-approximation) response to a uniform test field satisfies $(\partial_t-\eta\Delta)\mathbf b_j=(\overline{\mathbf B}\cdot\nabla)\mathbf u_j$. Writing $a=\eta k^2$, the response is $\mathbf b_j=k\overline B_j[a\partial_\phi\mathbf u_j-\Omega\mathbf u_j]/(a^2+\Omega^2)$. Since $\mathbf u_j\times\partial_\phi\mathbf u_j=-\sigma U^2\mathbf e_j$, summing yields the displayed isotropic [alpha effect](#alpha-effect). It includes the resistive and temporal weighting absent from an unqualified instantaneous helicity rule.

###### Helicity formula for isotropic first-order smoothing

↑ **Parent:** [First-order smoothing approximation](#first-order-smoothing-approximation)

For a locally uniform mean [magnetic field](electromagnetism.md#magnetic-field), [first-order smoothing](#first-order-smoothing-approximation) solves $\partial_t\mathbf b-\eta\Delta\mathbf b=(\overline{\mathbf B}\cdot\nabla)\mathbf u$. Inserting its causal diffusion propagator into the [mean-field electromotive force](#mean-field-electromotive-force) and taking the [trace](linear-algebra.md#matrix-trace) of the isotropic response tensor gives the displayed relation to [kinetic helicity](fluid-mechanics.md#hydrodynamical-helicity). When diffusion during a [correlation time](time-series.md#correlation-time) is negligible, it reduces to $\alpha=-\tau_H\langle\mathbf u\cdot\nabla\times\mathbf u\rangle/3$. At small [magnetic Reynolds number](#magnetic-reynolds-number), a quasistatic monochromatic velocity instead gives $\alpha=-\langle\mathbf u\cdot\nabla\times\mathbf u\rangle/(3\eta k_0^2)$. The effective [correlation time](time-series.md#correlation-time) and diffusion weighting should not be silently discarded.

###### Quasistatic magnetic response of a helical shearing wave

↑ **Parent:** [First-order smoothing approximation](#first-order-smoothing-approximation)

For background shear $\Omega y\widehat{\mathbf x}$ and uniform field $B_0\widehat{\mathbf x}$, [first-order smoothing](#first-order-smoothing-approximation) gives the magnetic shearing-wave amplitude equation

$$
\dot{\mathbf c}=\Omega c_y\widehat{\mathbf x}+ik_xB_0\mathbf v-\eta K^2\mathbf c.
$$

If magnetic relaxation is fast compared with shear, $c_y,c_z\simeq ik_xB_0(v_y,v_z)/(\eta K^2)$ after free transients decay. Thus the doubled Fourier-mode electromotive quantity $\mathcal E=\operatorname{Re}(v_yc_z^*-v_zc_y^*)$ is $-B_0H/(\eta K^2)$, where $H=ik_x(v_yv_z^*-v_zv_y^*)$. The spatially averaged [mean-field electromotive force](#mean-field-electromotive-force) of real waves has an extra factor $1/2$. Using the [helicity invariant of an inviscid shearing wave](gravitational-instability-of-an-astrophysical-disk.md#helicity-invariant-of-an-inviscid-shearing-wave), and assuming the approximation holds uniformly in time with $\Omega k_x\ne0$, gives

$$
\int_{-\infty}^{\infty}\mathcal E\,dt\simeq-\frac{\pi B_0H(0)}{2\eta|\Omega k_x|\sqrt{k_x^2+k_z^2}}.
$$

Indeed $K^2=A+\Omega^2k_x^2t^2$, $A=k_x^2+k_z^2$, and substitution $z=|\Omega k_x|t/\sqrt A$ uses $\int_{-\infty}^{\infty}(1+z^2)^{-2}dz=\pi/2$.

###### Monochromatic coupled magnetic and velocity response

↑ **Parent:** [First-order smoothing approximation](#first-order-smoothing-approximation)

For a steady forced [Fourier mode](fourier-analysis.md#fourier-mode) with $|\mathbf q|=k$, coupled viscous and magnetic response gives $\widehat{\mathbf u}=[\eta k^2\widehat{\mathbf f}+i(\mathbf B\cdot\mathbf q)\widehat{\mathbf g}/(\mu_0\rho)]/D$ and $\widehat{\mathbf b}=[\nu k^2\widehat{\mathbf g}+i(\mathbf B\cdot\mathbf q)\widehat{\mathbf f}]/D$. Their [mean-field electromotive force](#mean-field-electromotive-force) contains both forcing helicities and a possible weighted cross-forcing correlation. Jointly isotropic forcing removes the latter; its vanishing at zero mean field alone is insufficient for anisotropic forcing.

###### Oscillatory magnetic response in first-order smoothing

↑ **Parent:** [First-order smoothing approximation](#first-order-smoothing-approximation)

For a velocity [Fourier mode](fourier-analysis.md#fourier-mode) with wavenumber $k$, define $a=\eta k^2$, $d=a^2+\Omega^2$ and $\mathbf C=i(\mathbf B_0\cdot\mathbf k)\hat{\mathbf u}$. A cosine-forced mode has periodic response coefficients $(\mathbf p,\mathbf q)=(a\mathbf C,\Omega\mathbf C)/d$, while a sine-forced mode has $(-\Omega\mathbf C,a\mathbf C)/d$. Homogeneous transients decay as $e^{-at}$. The periodic response is a particular solution, not arbitrary initial data.

###### Parker dynamo wave

↑ **Parent:** [Mean-field dynamo](#mean-field-dynamo)

A Parker dynamo wave is a traveling or oscillatory mode of a mean-field dynamo coupling poloidal and toroidal magnetic-field components through an [alpha effect](#alpha-effect) and shear. A reduced complex-amplitude model can represent fluctuating alpha by a time-dependent coupling. Its periodically switched growth must be calculated from the [monodromy matrix of a periodic linear system](differential-equation.md#monodromy-matrix-of-a-periodic-linear-system), rather than by averaging noncommuting generators.

###### Local alpha-Omega dynamo wave dispersion

↑ **Parent:** [Parker dynamo wave](#parker-dynamo-wave)

Take a right-handed local Cartesian frame with $x$ towards the equator, $y$ azimuthal and $z$ radially outwards in the northern hemisphere. A local radial shear $U_y=Sz$ and a [poloidal magnetic field](#poloidal-magnetic-field) represented by $A\widehat{\mathbf y}$ give the [alpha-Omega dynamo](#alpha-omega-dynamo) equations $A_t=\alpha B+\eta_T A_{xx}$ and $B_t=S A_x+\eta_T B_{xx}$. Substitution of a [Fourier mode](fourier-analysis.md#fourier-mode) proportional to $e^{pt+ikx}$ gives the displayed [dispersion relation](wave-equation.md#dispersion-relation). The growing branch has $\operatorname{Re}p=-\eta_Tk^2+\sqrt{|\alpha Sk|/2}$ and $\operatorname{Im}p=\operatorname{sgn}(\alpha Sk)\sqrt{|\alpha Sk|/2}$. Its phase velocity is $-\operatorname{Im}p/k$: it propagates equatorwards when $\alpha S<0$, polewards when $\alpha S>0$. The result assumes local constant coefficients and no [meridional circulation in a star](stellar-structure.md#meridional-circulation-in-a-star); advection and spatially separated field regeneration can alter migration.

###### Periodically reversing Parker dynamo coupling

↑ **Parent:** [Parker dynamo wave](#parker-dynamo-wave)

For $\dot A=D^2f(t)B$ and $\dot B=iA$, with $f$ alternating between $+1$ and $-1$ for intervals of length $T$, the [monodromy matrix of a periodic linear system](differential-equation.md#monodromy-matrix-of-a-periodic-linear-system) has determinant one and trace $\cosh(\sqrt2DT)+\cos(\sqrt2DT)>2$. Its reciprocal [Floquet multipliers](dynamical-systems.md#floquet-multiplier) give positive dominant [Floquet growth rate](differential-equation.md#floquet-growth-rate) for $D,T>0$, despite the zero mean of $f$. An exceptional initial state in the stable [eigenspace](linear-operator-theory.md#eigenspace) decays.

###### Alpha effect

↑ **Parent:** [Mean-field dynamo](#mean-field-dynamo)

The alpha effect is the part of a [mean-field electromotive force](#mean-field-electromotive-force) linear in the mean [magnetic field](electromagnetism.md#magnetic-field) itself, $\boldsymbol{\mathcal E}=\boldsymbol\alpha\overline{\mathbf B}+\cdots$. The [alpha tensor](#alpha-tensor) can be anisotropic; it need not be a scalar multiple of the identity. Its [curl](calculus.md#curl) can couple transverse mean-field components and produce an [alpha-squared dynamo](#alpha-squared-dynamo).

###### Rapidly fluctuating alpha effect

↑ **Parent:** [Alpha effect](#alpha-effect)

In a [Parker dynamo wave](#parker-dynamo-wave) model, an [alpha effect](#alpha-effect) of the form $\alpha=\epsilon^{-1}\alpha_0\sin(\omega t/\epsilon)$ has zero time average but can generate a finite averaged coupling. The [method of multiple scales](differential-equation.md#method-of-multiple-scales) gives $\widetilde A=-(\alpha_0/\omega)\cos(\omega\tau)\overline B$ and $\widetilde B=-(\Omega\alpha_0/\omega^2)\sin(\omega\tau)\partial_x\overline B$, where $\tau=t/\epsilon$. Consequently $C=\Omega\alpha_0^2/(2\omega^2)$. With diffusion operator $\partial_x^2-\ell^2$, the averaged [Fourier mode](fourier-analysis.md#fourier-mode) growth exponents are $-k^2-\ell^2\pm|k|\sqrt{\Omega C}$. For freely adjustable real $k$, growth requires $\Omega C>4\ell^2$. The result is an asymptotic averaged model for fixed nonzero $\omega$, not an exact replacement at finite $\epsilon$.

###### Strong-field quenching of an isotropic electromotive force

↑ **Parent:** [Alpha effect](#alpha-effect)

For isotropic monochromatic forcing, the longitudinal coefficient in a [mean-field electromotive force](#mean-field-electromotive-force) is proportional to $\int_0^1\mu^2(1+h^2\mu^2)^{-2}d\mu=[\arctan h-h/(1+h^2)]/(2h^3)$, where $h$ is proportional to mean-field strength. This gives generic $|B|^{-3}$ quenching. The natural angular [alpha tensor](#alpha-tensor) is anisotropic in a nonzero mean field: its transverse coefficient instead contains $\int_0^1(1-\mu^2)(1+h^2\mu^2)^{-2}d\mu$ and scales as $|B|^{-1}$. Only the longitudinal contraction enters $\boldsymbol{\mathcal E}=\boldsymbol\alpha\mathbf B$. An effective scalar representation may therefore have every diagonal entry equal to the longitudinal coefficient without being the unique natural response tensor.

###### Alpha-squared dynamo

↑ **Parent:** [Alpha effect](#alpha-effect)

An alpha-squared dynamo generates a mean [magnetic field](electromagnetism.md#magnetic-field) using an [alpha effect](#alpha-effect) without requiring an additional large-scale shear coupling. For $\boldsymbol\alpha=\alpha_0\operatorname{diag}(1,1,0)$ and a transverse mean field varying as $e^{iKz}$, the growth rates are $-\eta K^2\pm\alpha_0K$. A nonzero $\alpha_0$ therefore allows growth for sufficiently long wavelengths, provided the domain and scale separation permit them.

###### Homogeneous alpha-squared dynamo growth criterion

↑ **Parent:** [Alpha-squared dynamo](#alpha-squared-dynamo)

For constant isotropic transport coefficients and zero mean flow, a divergence-free [Fourier mode](fourier-analysis.md#fourier-mode) has two [circular polarizations](electromagnetism.md#circular-polarization) that diagonalize [curl](calculus.md#curl) with eigenvalues $\pm k$. The mean induction equation therefore has the displayed [growth rates](wave-equation.md#growth-rate). Growth requires an admissible $k$ with $|\alpha|>(\eta+\beta)k$. Freely variable wavenumber gives $k_*=|\alpha|/[2(\eta+\beta)]$, provided it respects mean-field scale separation. A uniform field has zero [curl](calculus.md#curl) and cannot grow by constant alpha alone; boundaries fix the longest available spatial mode.

###### Anisotropic alpha-squared dynamo

↑ **Parent:** [Alpha-squared dynamo](#alpha-squared-dynamo)

An [alpha-squared dynamo](#alpha-squared-dynamo) may use a tensorial [alpha effect](#alpha-effect) rather than an isotropic coefficient. For constant [alpha tensor](#alpha-tensor) $\boldsymbol\alpha$ and [magnetic diffusivity](#magnetic-diffusivity) $\eta>0$, a steady nonzero [Fourier mode](fourier-analysis.md#fourier-mode) with wavevector $\mathbf K$ satisfies $\eta K^2\mathbf B=i\mathbf K\times(\boldsymbol\alpha\mathbf B)$ and $\mathbf K\cdot\mathbf B=0$. Anisotropy can change both the critical alpha magnitude and the preferred wavevector direction.

###### Uniaxial alpha dynamo threshold

↑ **Parent:** [Anisotropic alpha-squared dynamo](#anisotropic-alpha-squared-dynamo)

For $\boldsymbol\alpha=\operatorname{diag}(\alpha_0,\alpha_0,\alpha_1)$, set $\gamma=\alpha_0/\eta$, $\delta=\alpha_1/\alpha_0$, and $q^2=k^2+l^2$. A steady nonzero [Fourier mode](fourier-analysis.md#fourier-mode) obeys the displayed condition when the denominator is nonzero. At fixed $q>0$ and $0<\delta<1$, minimizing over $m^2\geq0$ gives $m_*^2=(1-2\delta)q^2$ and $\gamma_{\min}^2=4(1-\delta)q^2$ for $\delta<1/2$; for $\delta\geq1/2$ it gives $m_*^2=0$ and $\gamma_{\min}^2=q^2/\delta$. This is a boundary-constrained threshold of an [anisotropic alpha-squared dynamo](#anisotropic-alpha-squared-dynamo).

###### Alpha tensor

↑ **Parent:** [Alpha effect](#alpha-effect)

The alpha tensor is the linear map from a uniform test [magnetic field](electromagnetism.md#magnetic-field) to the corresponding [mean-field electromotive force](#mean-field-electromotive-force). Its components satisfy $\mathcal E_i=\alpha_{ij}B_{0j}$. Anisotropic helical flows can produce a real symmetric rank-two response, such as $\alpha_0\operatorname{diag}(1,1,0)$.

###### Mean-field electromotive force

↑ **Parent:** [Mean-field dynamo](#mean-field-dynamo)

The mean-field electromotive force is the vector correlation $\boldsymbol{\mathcal E}=\langle\mathbf u\times\mathbf b\rangle$. Its [curl](calculus.md#curl) enters the mean [resistive induction equation](#resistive-induction-equation). It is a local vector with units of velocity times magnetic field, not the scalar circuit voltage called [electromotive force](electromagnetism.md#electromotive-force). A [space-time average of periodic modes](#space-time-average-of-periodic-modes) is often used to measure its transport coefficients.

###### Monochromatic small-Reynolds-number mean electromotive force

↑ **Parent:** [Mean-field electromotive force](#mean-field-electromotive-force)

Suppose a steady [solenoidal](calculus.md#solenoidal-vector-field) velocity satisfies $\Delta\mathbf u=-\mathbf u$, and spatial averaging permits [integration by parts](calculus.md#integration-by-parts) without boundary terms. For a uniform test [magnetic field](electromagnetism.md#magnetic-field) $\mathbf B$, the small-[magnetic Reynolds number](#magnetic-reynolds-number) expansion gives $\mathbf b_1=(\mathbf B\cdot\nabla)\mathbf u$ and $\Delta\mathbf b_2=-\nabla\times(\mathbf u\times\mathbf b_1)$. Using the [self-adjointness](linear-operator-theory.md#self-adjoint-operator) of the [Laplacian](calculus.md#laplacian) inside the average,

$$
\mathcal E^{(1)}=\langle\mathbf u\times(\mathbf B\cdot\nabla)\mathbf u\rangle,\qquad
\mathcal E^{(2)}=\langle\mathbf u\times\nabla\times[\mathbf u\times(\mathbf B\cdot\nabla)\mathbf u]\rangle.
$$

The second equality concerns the averaged [mean-field electromotive force](#mean-field-electromotive-force); it does not assert that the quadratic forcing itself is monochromatic.

// Target: fluid-mechanics.bigb

###### Antisymmetry of the second-order monochromatic alpha tensor

↑ **Parent:** [Monochromatic small-Reynolds-number mean electromotive force](#monochromatic-small-reynolds-number-mean-electromotive-force)

For $\mathbf C=\mathbf u\times(\mathbf B\cdot\nabla)\mathbf u$, the [cross product](vector-space.md#cross-product) identity $(\mathbf u\times\nabla\times\mathbf C)_i=u_j\partial_iC_j-u_j\partial_jC_i$ and [integration by parts](calculus.md#integration-by-parts) give $\mathcal E^{(2)}_i=-\langle\partial_i u_jC_j\rangle$. Its [alpha tensor](#alpha-tensor) is

$$
\alpha^{(2)}_{ij}=-\langle\partial_i\mathbf u\cdot(\mathbf u\times\partial_j\mathbf u)\rangle
=\langle\mathbf u\cdot(\partial_i\mathbf u\times\partial_j\mathbf u)\rangle.
$$

Interchanging $i,j$ reverses the [cross product](vector-space.md#cross-product), showing that the coefficient is an [antisymmetric matrix](linear-algebra.md#skew-symmetric-matrix). Such a coefficient represents a [turbulent magnetic pumping](#turbulent-magnetic-pumping) contribution rather than the symmetric part of the [alpha effect](#alpha-effect).

// Target: fluid-mechanics.bigb

###### Symmetry of the first-order monochromatic alpha tensor

↑ **Parent:** [Monochromatic small-Reynolds-number mean electromotive force](#monochromatic-small-reynolds-number-mean-electromotive-force)

The first coefficient of the [alpha tensor](#alpha-tensor) is $\alpha^{(1)}_{ij}=\epsilon_{ikl}\langle u_k\partial_j u_l\rangle$. Its contraction with the [Levi-Civita symbol](calculus.md#levi-civita-symbol) is

$$
\epsilon_{pij}\alpha^{(1)}_{ij}=\langle u_j\partial_j u_p-u_p\partial_j u_j\rangle=0,
$$

by [incompressibility](fluid-mechanics.md#incompressible-flow) and vanishing averages of total derivatives. Every [antisymmetric second-rank tensor](linear-algebra.md#antisymmetric-second-rank-tensor) in three dimensions is detected by this contraction, so the coefficient is a [symmetric matrix](linear-algebra.md#symmetric-matrix). The proof needs no [Fourier analysis](fourier-analysis.md).

// Target: fluid-mechanics.bigb

###### Turbulent magnetic pumping

↑ **Parent:** [Mean-field electromotive force](#mean-field-electromotive-force)

[Turbulent magnetic pumping](#turbulent-magnetic-pumping) is an effective transport of the mean [magnetic field](electromagnetism.md#magnetic-field) produced by correlations in inhomogeneous or anisotropic turbulence. Its contribution to the [mean-field electromotive force](#mean-field-electromotive-force) is $\boldsymbol{\mathcal E}_{\rm pump}=\boldsymbol\gamma\times\overline{\mathbf B}$. In the mean induction equation this enters as $\nabla\times(\boldsymbol\gamma\times\overline{\mathbf B})$, the same algebraic form as [advection](fluid-mechanics.md#advection) by a [velocity](classical-mechanics.md#velocity) $\boldsymbol\gamma$. Thus it supplements the mean material [velocity](classical-mechanics.md#velocity) without requiring an equal mean mass flow. Downward pumping can help retain or couple fields in a [solar dynamo](stellar-astrophysics.md#solar-dynamo).

###### Integrated electromotive response of a finite cyclonic event

↑ **Parent:** [Mean-field electromotive force](#mean-field-electromotive-force)

For the [ideal magnetic response to a cylindrical cyclonic event](#ideal-magnetic-response-to-a-cylindrical-cyclonic-event), the plane-integrated $x$-component of $\mathbf u\times\mathbf B$ at duration $t$ is

$$
\mathcal E_x(t)=\pi B_0\int_0^\infty\left[t r^2(fg'-gf')\cos(ft)-2rg\sin(ft)\right]dr.
$$

This follows from $(\mathbf u\times\mathbf B)_x=(rfB_z+gA_r)\cos\phi-(g/r)A_\phi\sin\phi$ and azimuthal integration. If boundary terms vanish, integration by parts gives the equivalent form $\pi B_0\int_0^\infty r^2g'[\sin(ft)+tf\cos(ft)]dr$. For $f=g=a^2-r^2$ on $r<a$, zero outside, the response is

$$
\mathcal E_x(t)=\pi B_0a^4\frac{x\cos x-\sin x}{x^2},\qquad x=a^2t.
$$

The value at zero is its continuous limit zero. It is initially $-\pi B_0a^6t/3$, but changes sign repeatedly at the nonzero roots of $\tan x=x$, with oscillatory envelope of order $t^{-1}$. The flow's [kinetic helicity density](fluid-mechanics.md#kinetic-helicity-density) is $2f^2\geq0$, showing that the sign of a finite-duration ideal response is not fixed by the instantaneous helicity sign.

###### Space-time average of periodic modes

↑ **Parent:** [Mean-field electromotive force](#mean-field-electromotive-force)

A space-time average over periodic modes integrates over the spatial periodic cell and one temporal period. For real spatial [Fourier modes](fourier-analysis.md#fourier-mode) sharing a [wavevector](continuum-mechanics.md#wavevector), $\langle\operatorname{Re}(\mathbf v e^{i\mathbf k\cdot\mathbf x})\times\operatorname{Re}(\mathbf w e^{i\mathbf k\cdot\mathbf x})\rangle_x=\operatorname{Re}(\mathbf v^*\times\mathbf w)/2$. A matching sine or cosine temporal factor supplies another $1/2$. Opposite wavevectors can have nonzero spatial cross averages, so their temporal coefficients must be checked rather than discarded merely because the wavevectors are distinct.

#### Hartmann flow

↑ **Parent:** [Resistive magnetohydrodynamics](#resistive-magnetohydrodynamics)

Hartmann flow is a fully developed viscous conducting-fluid flow driven along a planar channel while a uniform [magnetic field](electromagnetism.md#magnetic-field) crosses the walls. Induction and the [Lorentz force density](electromagnetism.md#lorentz-force-density) couple its velocity and tangential induced field. For no-slip, normal-field walls separated by $2L$, the velocity is a [hyperbolic cosine](calculus.md#hyperbolic-cosine) profile that approaches [plane Poiseuille flow](viscous-fluid-flow.md#plane-poiseuille-flow) at zero imposed field and develops a uniform core with [Hartmann layers](#hartmann-layer) at large [Hartmann number](#hartmann-number).

##### Hartmann flow rate with normal-field walls

↑ **Parent:** [Hartmann flow](#hartmann-flow)

For a streamwise pressure gradient $-\rho G$ and walls at $z=\pm L$ with zero tangential [magnetic field](electromagnetism.md#magnetic-field), the [volumetric flow rate](fluid-mechanics.md#volumetric-flow-rate) per unit span is

$$
Q(H)=\frac{2GL^3}{\nu}\frac{H\coth H-1}{H^2}.
$$

Its zero-field value is $2GL^3/(3\nu)$; it decreases strictly for $H>0$ and is asymptotic to $2GL^3/(\nu H)$. The [partial-fraction expansion of the hyperbolic cotangent](calculus.md#partial-fraction-expansion-of-the-hyperbolic-cotangent) proves monotonicity directly.

##### Hartmann layer

↑ **Parent:** [Hartmann flow](#hartmann-flow)

A Hartmann layer is the thin viscous-magnetic [boundary layer](continuum-mechanics.md#boundary-layer) next to a wall crossed by the applied [magnetic field](electromagnetism.md#magnetic-field). For channel half-width $L$ and large [Hartmann number](#hartmann-number) $H$, its thickness is $\delta\sim L/H=\sqrt{\mu_0\rho\nu\eta}/|B_0|$. It restores the [no-slip boundary condition](viscous-fluid-flow.md#no-slip-boundary-condition) and the specified magnetic wall condition outside the nearly uniform [Hartmann flow](#hartmann-flow) core.

##### Hartmann number

↑ **Parent:** [Hartmann flow](#hartmann-flow)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hartmann_number)

The Hartmann number measures the strength of magnetic coupling relative to viscous and resistive effects in a channel:

$$
H=\frac{|B_0|L}{\sqrt{\mu_0\rho\nu\eta}}=|B_0|L\sqrt{\frac{\sigma_c}{\rho\nu}}.
$$

Here $L$ is the channel half-width, $\nu$ the [kinematic viscosity](fluid-mechanics.md#kinematic-viscosity), $\eta$ the [magnetic diffusivity](#magnetic-diffusivity) and $\sigma_c$ the [electrical conductivity](electromagnetism.md#electrical-conductivity). In [Hartmann flow](#hartmann-flow), large $H$ produces thin magnetic-viscous wall layers and a flatter, slower core for fixed [pressure gradient](fluid-mechanics.md#pressure-gradient).

#### Normal magnetic field boundary condition

↑ **Parent:** [Resistive magnetohydrodynamics](#resistive-magnetohydrodynamics)

A normal-field wall imposes zero tangential [magnetic field](electromagnetism.md#magnetic-field): $\mathbf B\times\mathbf n=0$ for the wall [unit normal](differential-geometry.md#unit-normal) $\mathbf n$. In a channel with imposed normal field $B_0\hat{\mathbf z}$, an induced tangential component $b(z)\hat{\mathbf x}$ therefore satisfies $b=0$ on each wall. This condition is distinct from the [no-slip boundary condition](viscous-fluid-flow.md#no-slip-boundary-condition) on fluid velocity.

#### Resistive induction equation

↑ **Parent:** [Resistive magnetohydrodynamics](#resistive-magnetohydrodynamics)

For a [solenoidal vector field](calculus.md#solenoidal-vector-field) $\mathbf B$ and constant [magnetic diffusivity](#magnetic-diffusivity) $\eta$, the magnetic induction equation is

$$
\partial_t\mathbf B=\nabla\times(\mathbf u\times\mathbf B)+\eta\nabla^2\mathbf B,\qquad \nabla\cdot\mathbf B=0.
$$

It combines [Faraday's law](electromagnetism.md#faraday-s-law-of-induction) with the moving-conductor relation for [electrical conductivity](electromagnetism.md#electrical-conductivity), neglecting displacement current. With [incompressible flow](fluid-mechanics.md#incompressible-flow), its advective form is $\partial_t\mathbf B+(\mathbf u\cdot\nabla)\mathbf B=(\mathbf B\cdot\nabla)\mathbf u+\eta\nabla^2\mathbf B$.

##### Shearing-coordinate magnetic flux equation

↑ **Parent:** [Resistive induction equation](#resistive-induction-equation)

For a planar [magnetic field](electromagnetism.md#magnetic-field) written as $\mathbf B=\nabla\times(A\widehat{\mathbf z})$ and a circular [velocity](classical-mechanics.md#velocity) $\mathbf u=s\Omega(s)\widehat{\boldsymbol\phi}$, the [resistive induction equation](#resistive-induction-equation) reduces, after choosing the additive [gauge transformation](electromagnetism.md#gauge-transformation), to $\partial_tA+\Omega\partial_\phi A=\eta\nabla^2A$. A [Fourier mode](fourier-analysis.md#fourier-mode) $A=a(s,t)e^{im[\phi-\Omega(s)t]}$ therefore obeys the equation in the title. Indeed, each radial [derivative](calculus.md#derivative) acting on the exponential replaces $\partial_s$ by $\partial_s-imt\Omega'$, while the azimuthal [Laplacian](calculus.md#laplacian) contributes $-m^2/s^2$. At zero [magnetic diffusivity](#magnetic-diffusivity), $a$ is constant in time, but the physical [magnetic field](electromagnetism.md#magnetic-field) can still be amplified algebraically by [differential rotation](#differential-rotation).

##### Radial magnetic induction scalar

↑ **Parent:** [Resistive induction equation](#resistive-induction-equation)

For [solenoidal](calculus.md#solenoidal-vector-field) velocity and [magnetic field](electromagnetism.md#magnetic-field), with constant [magnetic diffusivity](#magnetic-diffusivity) $\eta$, the [resistive induction equation](#resistive-induction-equation) implies

$$
\partial_tP+\mathbf u\cdot\nabla P=\mathbf B\cdot\nabla Q+\eta\Delta P,\qquad Q=\mathbf u\cdot\mathbf x.
$$

The [product rule](calculus.md#product-rule) gives $D_tP=\mathbf x\cdot D_t\mathbf B+\mathbf u\cdot\mathbf B$ and $\Delta P=\mathbf x\cdot\Delta\mathbf B+2\nabla\cdot\mathbf B$. Consequently the radial velocity, through $Q$, is the source term for the radial [magnetic field](electromagnetism.md#magnetic-field).

// Target: fluid-mechanics.bigb

###### Insulating boundary condition for the radial magnetic scalar

↑ **Parent:** [Radial magnetic induction scalar](#radial-magnetic-induction-scalar)

At a spherical interface with an insulating exterior, equal [magnetic permeability](electromagnetism.md#permeability-electromagnetism) on both sides and no surface current, all components of the [magnetic field](electromagnetism.md#magnetic-field) are continuous. The [solenoidal magnetic-field constraint](electromagnetism.md#solenoidal-magnetic-field-constraint) then makes $P=\mathbf B\cdot\mathbf x$ and $\partial_rP$ continuous. A current-free exterior has $\Delta P=0$. For an isolated field decaying at infinity, its degree-$l$ [spherical harmonic](analysis.md#spherical-harmonic) satisfies $\partial_rP_{lm}=-(l+1)P_{lm}/a$ at a sphere of radius $a$. This [boundary condition](differential-equation.md#boundary-condition) incorporates the exterior field without setting the radial field to zero.

// Target: fluid-mechanics.bigb

### Magnetic diffusion

↑ **Parent:** [Magnetohydrodynamics](#magnetohydrodynamics)

Finite [electrical conductivity](electromagnetism.md#electrical-conductivity) permits resistive smoothing of a [magnetic field](electromagnetism.md#magnetic-field). With uniform coefficients and no motion the field satisfies a diffusion equation; with motion the diffusion term supplements the curl of $\mathbf u\times\mathbf B$. The [magnetic Reynolds number](#magnetic-reynolds-number) compares these effects.

#### Magnetic phase mixing under differential rotation

↑ **Parent:** [Magnetic diffusion](#magnetic-diffusion)

A nonuniform angular velocity $f(r)$ winds an azimuthal magnetic mode into phase $m(\phi-f(r)t)$. Its radial phase gradient grows as $-mt f'(r)$, creating small scales even when its ideal amplitude does not decay. The corresponding leading resistive damping rate is $\eta m^2t^2f'(r)^2$, so a local short-wavelength estimate gives damping factor $\exp[-\eta m^2f'(r)^2t^3/3]$. Hence [magnetic diffusion](#magnetic-diffusion) can become important at time $[\eta m^2f'^2]^{-1/3}$ although it is initially small. This is a local phase-mixing estimate, not a globally exact solution in a finite radial domain: boundary forcing, field stretching and spatial variation of $f'$ must also be retained there.

##### Exact quadratic-shear magnetic flux solution

↑ **Parent:** [Magnetic phase mixing under differential rotation](#magnetic-phase-mixing-under-differential-rotation)

For azimuthal flow $u_\phi=s(\Omega_0+\omega s^2)$, a planar [magnetic flux](electromagnetism.md#magnetic-flux) mode $s^mg(t)e^{im\phi-im\Omega_0t-is^2f(t)}$ obeys the [resistive induction equation](#resistive-induction-equation) if $\dot f=m\omega-4i\eta f^2$ and $\dot g/g=-4i\eta(m+1)f$. With $f(0)=0$ and $g(0)=1$, their solution is $f=(m\omega/\mu)\tanh\mu t$ and $g=(\cosh\mu t)^{-(m+1)}$. Choose $\operatorname{Re}\mu>0$. For positive $\eta,\omega$, the fixed-position field decays asymptotically at rate $(m+1)\sqrt{2\eta m\omega}$. [Differential rotation](#differential-rotation) creates small spatial scales, accelerating [magnetic diffusion](#magnetic-diffusion).

#### Magnetic free-decay spectral bound

↑ **Parent:** [Magnetic diffusion](#magnetic-diffusion)

For a [solenoidal vector field](calculus.md#solenoidal-vector-field) carrying current only in a conductor contained in a sphere of radius $R$, match the exterior field to a decaying potential field and include exterior [magnetic energy](electromagnetism.md#magnetic-energy). The smallest free-decay [eigenvalue](linear-operator-theory.md#eigenvalue) of the enclosing sphere is $\pi^2/R^2$, from its dipolar poloidal mode. The corresponding variational estimate gives the displayed bound. Continuity and the usual insulating-interface magnetic conditions are part of the admissible field class. This bound is the diffusive ingredient in [Backus' necessary condition for dynamo action](#backus-necessary-condition-for-dynamo-action).

#### Magnetic diffusivity

↑ **Parent:** [Magnetic diffusion](#magnetic-diffusion)

Magnetic diffusivity is the coefficient of [magnetic diffusion](#magnetic-diffusion). In a scalar-conductivity fluid with vacuum permeability and negligible [displacement current](electromagnetism.md#displacement-current), $\eta_m=1/(\mu_0\sigma)$. Its dimensions are length squared per time, and a diffusion time on scale $L$ is $L^2/\eta_m$.

##### Magnetic Prandtl number

↑ **Parent:** [Magnetic diffusivity](#magnetic-diffusivity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Magnetic_Prandtl_number)

The magnetic Prandtl number compares [kinematic viscosity](fluid-mechanics.md#kinematic-viscosity) with [magnetic diffusivity](#magnetic-diffusivity). It is the ratio of the viscous and magnetic diffusion coefficients; equivalently it is the [magnetic Reynolds number](#magnetic-reynolds-number) divided by the [Reynolds number](fluid-mechanics.md#reynolds-number) when the same speed and length scale are used.

##### Turbulent magnetic diffusivity

↑ **Parent:** [Magnetic diffusivity](#magnetic-diffusivity)

Turbulent magnetic diffusivity is an effective transport coefficient produced by correlated small-scale [velocity](classical-mechanics.md#velocity) and [magnetic field](electromagnetism.md#magnetic-field). It supplements microscopic [magnetic diffusivity](#magnetic-diffusivity) in a [mean-field dynamo](#mean-field-dynamo) description. Its identification requires a specified mean-field geometry and averaging procedure; in a planar flux problem, the correlation $\overline{wa'}=-\eta_tB_0f(z)$ describes transport relative to a prescribed uniform field.

###### Variance bound for planar turbulent magnetic transport

↑ **Parent:** [Turbulent magnetic diffusivity](#turbulent-magnetic-diffusivity)

For $\overline{wa'}=-\eta_tB_0f$, $\langle f\rangle=1$ and positive diffusivities, the [Zeldovich planar flux balance](#zeldovich-planar-flux-balance) gives $G=(\eta_t/\eta)B_0^2[1-(\eta_t/\eta)\operatorname{Var}(f)]$, where $G=\langle|\nabla a'|^2\rangle$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) and a [Poincaré inequality](sobolev-space.md#poincare-inequality) $\langle a'^2\rangle\leq d^2G/\pi^2$ give $\eta_t^2\operatorname{Var}(f)\leq\langle w^2\rangle d^2s(1-s)/\pi^2$, with $s=(\eta_t/\eta)\operatorname{Var}(f)\in[0,1]$. Maximizing $s(1-s)$ gives the displayed bound. Large turbulent-to-microscopic diffusivity therefore requires $f$ to be close to one in mean square, without guaranteeing pointwise uniformity.

### Magnetic Reynolds number

↑ **Parent:** [Magnetohydrodynamics](#magnetohydrodynamics)

The magnetic Reynolds number compares field advection with resistive [magnetic diffusion](#magnetic-diffusion). With constant [electrical conductivity](electromagnetism.md#electrical-conductivity) and vacuum permeability, magnetic diffusivity is $\eta_m=1/(\mu_0\sigma)$ and $\operatorname{Rm}=UL/\eta_m$. The ideal induction approximation applies when this ratio is large on the scales of interest.

### Moving-conductor Ohm law

↑ **Parent:** [Magnetohydrodynamics](#magnetohydrodynamics)

In the nonrelativistic scalar-conductivity approximation, neglecting Hall and other nonideal electromotive effects, $\mathbf J=\sigma(\mathbf E+\mathbf u\times\mathbf B)$. The ideal finite-current limit gives $\mathbf E=-\mathbf u\times\mathbf B$ and hence the [ideal magnetohydrodynamic induction equation](#ideal-magnetohydrodynamic-induction-equation).

### Magnetoconvection

↑ **Parent:** [Magnetohydrodynamics](#magnetohydrodynamics)

Magnetoconvection is thermal [convection](fluid-mechanics.md#convection) coupled to the evolution and forces of a [magnetic field](electromagnetism.md#magnetic-field). Conserved [magnetic flux](electromagnetism.md#magnetic-flux) can supply a slow field that must be retained along with the convective [complex amplitude](physics.md#complex-amplitude), rather than being eliminated into a single local [amplitude equation](dynamical-systems.md#amplitude-equation).

#### Three-mode porous magnetoconvection

↑ **Parent:** [Magnetoconvection](#magnetoconvection)

A [Galerkin method](partial-differential-equation.md#galerkin-method) using one convective [streamfunction](fluid-mechanics.md#stream-function) mode and two [Cartesian magnetic flux function](#cartesian-magnetic-flux-function) modes yields the displayed system. With $\alpha=\pi/\sqrt3$, use $\psi=4\sqrt2a\sin(\alpha x)\sin(\pi z)$ and $A=(3\sqrt2/\pi)b\sin(\alpha x)\cos(\pi z)+(\sqrt3/\pi)c\sin(2\alpha x)$, time $\tau=(4\pi^2/3)t$, $q=9Q/(16\pi^2)$ and $r=9R/(64\pi^4)$. The origin's planar trace is $\sigma(r-1)-\zeta$ and determinant $\sigma\zeta(1+q-r)$; the third [eigenvalue](linear-operator-theory.md#eigenvalue) is $-\zeta$. The stationary threshold is $r=1+q$, and the oscillatory threshold is $r=1+\zeta/\sigma$ when $q>\zeta/\sigma$. They meet in a symmetric double-zero point at $(q,r)=(\zeta/\sigma,1+\zeta/\sigma)$. Higher spatial harmonics generated by the quadratic terms are discarded, so this is a projected approximation rather than an exact invariant subspace of the original equations.

##### Cubic centre-manifold reduction of porous magnetoconvection

↑ **Parent:** [Three-mode porous magnetoconvection](#three-mode-porous-magnetoconvection)

For [three-mode porous magnetoconvection](#three-mode-porous-magnetoconvection), set $\mu=r-1-q$ and assume $0<q<\zeta/\sigma$. The transverse [eigenvalues](linear-operator-theory.md#eigenvalue) are negative. Centre-manifold invariance gives

$$
c=\frac{3a^2}{\zeta^2}+\cdots,\qquad
b=\frac a\zeta-\frac{\sigma\mu a}{\zeta(\zeta-\sigma q)}-\frac{3a^3}{\zeta^2(\zeta-\sigma q)}+\cdots.
$$

Substitution into the first equation gives the displayed positive linear and cubic coefficients. Thus the bifurcation is a [subcritical pitchfork bifurcation](dynamical-systems.md#subcritical-pitchfork-bifurcation): the origin is stable for $\mu<0$ and unstable for $\mu>0$, while the small nonzero branches at $a^2=-\zeta^2\mu/(3q)$ are unstable. Simply setting $\dot b=0$ misses the time-derivative contribution responsible for the common factor $(1-\sigma q/\zeta)^{-1}$.

#### Thermal-diffusion scaling of planar magnetoconvection

↑ **Parent:** [Magnetoconvection](#magnetoconvection)

Use depth $d$, time $d^2/\kappa$, stream-function scale $\kappa$, temperature perturbation scale $\Delta T$, and magnetic flux-function scale $B_0d$. With $\mathbf u=(-\psi_z,0,\psi_x)$, $\mathbf B=(-A_z,0,A_x)$ and $A=x+\chi$, advection is $J(\psi,f)=\psi_xf_z-\psi_zf_x$. The temperature background contributes $\psi_x$ to the heat equation and the imposed vertical field contributes $\psi_z$ to the perturbation induction equation. Taking the curl of the [magnetohydrodynamic momentum equation](#magnetohydrodynamic-momentum-equation) gives a magnetic term $\sigma\zeta QJ(A,\nabla^2A)$, where $\sigma=\nu/\kappa$, $\zeta=\eta/\kappa$, $R=g\alpha\Delta T d^3/(\nu\kappa)$ and $Q=B_0^2d^2/(\mu_0\rho\nu\eta)$.

#### Quasistatic vertical-field magnetoconvection

↑ **Parent:** [Magnetoconvection](#magnetoconvection)

When the magnetic field supplies instantaneous damping rather than an evolving magnetic perturbation, the roll amplitudes obey a two-variable linear system with [trace](linear-algebra.md#matrix-trace) $-[s+\sigma(s+Q\pi^2/s)]<0$. Its [determinant](linear-algebra.md#determinant) vanishes at the displayed stationary threshold. Therefore its initial instability cannot be a [Hopf bifurcation](dynamical-systems.md#hopf-bifurcation). This reduced model must not be confused with a three-variable magnetoconvection model carrying finite magnetic diffusivity and an additional oscillatory mode.

##### Cubic saturation of quasistatic magnetoconvection

↑ **Parent:** [Quasistatic vertical-field magnetoconvection](#quasistatic-vertical-field-magnetoconvection)

The primary roll and [temperature](thermodynamics.md#temperature) modes force only a horizontally uniform [temperature](thermodynamics.md#temperature) mode proportional to $\sin(2\pi z)$ at quadratic order. Its amplitude is $c=-\alpha ab/(8\pi)$. Its feedback on the primary [temperature](thermodynamics.md#temperature) mode saturates [magnetoconvection](#magnetoconvection), giving the displayed positive squared amplitude above threshold. Thus a simple roll onset is a supercritical [pitchfork bifurcation](dynamical-systems.md#pitchfork-bifurcation-normal-form) for every $Q\ge0$. The three-mode [Fourier truncation](partial-differential-equation.md#fourier-truncation) and full perturbation calculation agree through the cubic solvability condition because all forced quadratic modes are retained; this is not an assertion that the truncation gives an exact finite-amplitude PDE solution.

// Destination: dynamical-systems.bigb

#### Five-mode vertical-field magnetoconvection

↑ **Parent:** [Magnetoconvection](#magnetoconvection)

A [Galerkin method](partial-differential-equation.md#galerkin-method) approximation can retain one roll [streamfunction](fluid-mechanics.md#stream-function) mode, two temperature modes and two magnetic-flux perturbation modes in vertical-field [magnetoconvection](#magnetoconvection). Projection onto these five modes, rather than pointwise equality of the truncated fields, gives a closed system of five [ordinary differential equations](differential-equation.md#ordinary-differential-equation). Products generate higher spatial harmonics that are discarded by orthogonal projection. The system has symmetry $(a,b,c,d,e)\mapsto(-a,-b,c,-d,e)$ and hence admits paired steady roll branches.

##### Conduction double-zero criterion for five-mode magnetoconvection

↑ **Parent:** [Five-mode vertical-field magnetoconvection](#five-mode-vertical-field-magnetoconvection)

The conduction linearization has two negative [eigenvalues](linear-operator-theory.md#eigenvalue) and a cubic factor $s^3+As^2+Bs+C$, where $A=\sigma+1+\zeta$, $B=\sigma(1-r)+\sigma\zeta(1+q)+\zeta$, $C=\sigma\zeta(1+q-r)$. A double zero requires $B=C=0$, giving the displayed [Bogdanov–Takens bifurcation](dynamical-systems.md#bogdanov-takens-bifurcation) location for $0<\zeta<1$. The remaining cubic eigenvalue is $-A$. The imaginary-pair condition $AB=C$ yields $r_H=(\sigma+\zeta)(1+\zeta)/\sigma+\zeta(\sigma+\zeta)q/(\sigma+1)$ and $\omega^2=\sigma\zeta(1-\zeta)q/(\sigma+1)-\zeta^2$. Thus the oscillatory onset exists precisely for $q>q_*$ when $0<\zeta<1$.

##### Stationary branch of five-mode magnetoconvection

↑ **Parent:** [Five-mode vertical-field magnetoconvection](#five-mode-vertical-field-magnetoconvection)

For positive diffusivity ratio $\zeta$ and $0<\varphi<4$, define $\mu=(4-\varphi)\zeta^2/\varphi$. The nonzero steady branch has $b=a/(1+a^2)$, $c=a^2/(1+a^2)$, $d=\mu a/[\zeta(\mu+a^2)]$, and $e=a^2/(\mu+a^2)$. Substitution yields the displayed branch through $r=1+q$. Its initial slope in $a^2$ has the sign of $\varphi q(2-\varphi)+(4-\varphi)\zeta^2(1+q)$. Positive slope is a [supercritical pitchfork bifurcation](dynamical-systems.md#supercritical-pitchfork-bifurcation) direction, negative slope a [subcritical pitchfork bifurcation](dynamical-systems.md#subcritical-pitchfork-bifurcation) direction. This geometric criterion alone does not assert stability against every perturbation.

###### Pitchfork reversal near geometric ratio two in magnetoconvection

↑ **Parent:** [Stationary branch of five-mode magnetoconvection](#stationary-branch-of-five-mode-magnetoconvection)

Put $m=(4-\varphi)\zeta^2/\varphi$. The derivative of the [stationary branch of five-mode magnetoconvection](#stationary-branch-of-five-mode-magnetoconvection) at $a^2=0$ is $r_2=1+q+q(2-\varphi)/m$. For fixed positive $q$ and small $\zeta$, it changes from a forward to a backward [pitchfork bifurcation](dynamical-systems.md#pitchfork-bifurcation-normal-form) direction at the displayed value. Expanding the exact numerator $q\varphi(2-\varphi)+(4-\varphi)\zeta^2(1+q)$ gives this result. The expansion in amplitude requires $a^2\ll m$; branch direction alone does not determine stability against all other modes.

#### Horizontal-field magnetoconvection dispersion relation

↑ **Parent:** [Magnetoconvection](#magnetoconvection)

For a unit-depth [Boussinesq](geophysical-fluid-dynamics.md#boussinesq-approximation) layer with [stress-free boundary conditions](viscous-fluid-flow.md#stress-free-boundary-condition), fixed boundary temperatures, imposed field along $y$, and horizontal magnetic perturbations at the boundaries, put $a_h^2=k^2+m^2$ and $\Lambda=a_h^2+\pi^2$. Poloidal vertical velocity, temperature and vertical field proportional to $e^{st+ikx+imy}\sin\pi z$ have amplitudes satisfying

$$
\Lambda(s/\sigma+\Lambda)W=Ra_h^2\Theta+\zeta Qim\Lambda C,\qquad
(s+\Lambda)\Theta=W,\qquad(s+\zeta\Lambda)C=imW.
$$

The [determinant](linear-algebra.md#determinant) gives the stated [dispersion relation](wave-equation.md#dispersion-relation). Here $\sigma$ is the [Prandtl number](thermodynamics.md#prandtl-number), $\zeta$ the [magnetic-to-thermal diffusivity ratio](#magnetic-to-thermal-diffusivity-ratio), $Q$ the [Chandrasekhar number](#chandrasekhar-number) and $R$ the [Rayleigh number](geophysics.md#rayleigh-number). The steady neutral curve is $R=\Lambda^3/a_h^2+Qm^2\Lambda/a_h^2$.

// Target: fluid-mechanics.bigb

##### Strong-field steady magnetoconvection varying along the field

↑ **Parent:** [Horizontal-field magnetoconvection dispersion relation](#horizontal-field-magnetoconvection-dispersion-relation)

Restrict the [horizontal-field magnetoconvection dispersion relation](#horizontal-field-magnetoconvection-dispersion-relation) to $k=0$, $x=m^2>0$. The steady neutral curve becomes $R=\pi^2Q+(Q+3\pi^2)x+x^2+3\pi^4+\pi^6/x$. Its unique minimum satisfies $x^2(Q+3\pi^2+2x)=\pi^6$, since $R''(x)=2+2\pi^6/x^3>0$. Expanding at large [Chandrasekhar number](#chandrasekhar-number) gives $x\sim\pi^3Q^{-1/2}$ and the stated [asymptotic expansion](analysis.md#asymptotic-expansion). Unlike field-aligned rolls, these disturbances bend the field, and their stationary threshold grows with field strength.

// Target: fluid-mechanics.bigb

##### Magnetic-field-aligned rolls evade steady magnetic inhibition

↑ **Parent:** [Horizontal-field magnetoconvection dispersion relation](#horizontal-field-magnetoconvection-dispersion-relation)

At a fixed horizontal [wavenumber](wave-equation.md#wavenumber) magnitude, the steady neutral curve in the [horizontal-field magnetoconvection dispersion relation](#horizontal-field-magnetoconvection-dispersion-relation) is minimized by $m=0$. The disturbance is then constant along the imposed [magnetic field](electromagnetism.md#magnetic-field); it induces no field bending and incurs no [magnetic tension](#magnetic-tension) penalty. Minimizing $(k^2+\pi^2)^3/k^2$ gives the displayed stationary threshold for every $Q\geq0$. These [convection rolls](fluid-mechanics.md#convection-roll) have axes parallel to the imposed field. This assertion concerns steady onset.

// Target: fluid-mechanics.bigb

#### Magnetic-to-thermal diffusivity ratio

↑ **Parent:** [Magnetoconvection](#magnetoconvection)

The ratio of [magnetic diffusivity](#magnetic-diffusivity) $\eta$ to [thermal diffusivity](thermodynamics.md#thermal-diffusivity) $\kappa$ controls their relative relaxation times. In nonrotating vertical-field [magnetoconvection](#magnetoconvection), oscillatory linear onset in the simple stress-free layer requires $0<\zeta<1$, so thermal perturbations diffuse faster than magnetic perturbations. This is distinct from the [magnetic Prandtl number](#magnetic-prandtl-number), $\nu/\eta$.

#### Subcritical magnetoconvection

↑ **Parent:** [Magnetoconvection](#magnetoconvection)

Subcritical magnetoconvection means finite-amplitude [convection](fluid-mechanics.md#convection) on the stable side of the linear conductive-state threshold. At large [magnetic Reynolds number](#magnetic-reynolds-number), [flux expulsion](#flux-expulsion) can reduce interior magnetic inhibition enough to sustain a nonlinear convective cell even when infinitesimal disturbances decay in the unredistributed imposed field. Stable subcritical states can produce hysteresis and [magnetic flux separation](#magnetic-flux-separation). A schematic saturated [amplitude equation](dynamical-systems.md#amplitude-equation) $\dot A=\mu A+c|A|^2A-d|A|^4A$, $c,d>0$, has an unstable lower branch and stable upper radial branch for $-c^2/(4d)<\mu<0$, coexisting with stable $A=0$. This illustrates bistability; it is not a derivation of coefficients for all magnetoconvection geometries.

#### Magnetic flux separation

↑ **Parent:** [Magnetoconvection](#magnetoconvection)

In nonlinear [magnetoconvection](#magnetoconvection), magnetic flux separation is coexistence of weak-field regions with vigorous broad [convection](fluid-mechanics.md#convection) and strong-field regions with inhibited or small-scale [convection](fluid-mechanics.md#convection). [Flux expulsion](#flux-expulsion) provides a mechanism for segregation. Conserved mean vertical [magnetic flux](electromagnetism.md#magnetic-flux) implies $fB_c+(1-f)B_q=B_0$ for an idealized two-region area fraction $f$. Weak field in convecting regions therefore requires enhanced field elsewhere. The existence and stability of the segregated state depend on parameters and boundaries.

#### Oblique-field plane-wave magnetoconvection

↑ **Parent:** [Magnetoconvection](#magnetoconvection)

In thermal-diffusion units, let an imposed field point along $\mathbf c=(\sin\alpha,0,\cos\alpha)$ and consider a [Fourier mode](fourier-analysis.md#fourier-mode) of wavevector $(k,0,m)$. Put $q=k^2+m^2$ and $d=k\sin\alpha+m\cos\alpha$. The growth exponent $s$ of its buoyant branch satisfies

$$
q(s+q)\left[(s/\sigma+q)(s+\zeta q)+Q\zeta d^2\right]=Rk^2(s+\zeta q),
$$

where $\sigma$ is the [Prandtl number](thermodynamics.md#prandtl-number), $\zeta$ the magnetic-to-thermal diffusivity ratio, $Q$ the [Chandrasekhar number](#chandrasekhar-number), and $R$ the [Rayleigh number](geophysics.md#rayleigh-number). The [resistive induction equation](#resistive-induction-equation) gives $\widehat{\mathbf b}=id\widehat{\mathbf u}/(s+\zeta q)$, and thermal transport gives $\widehat\theta=\widehat w/(s+q)$. Projecting momentum perpendicular to the wavevector removes pressure; the vertical component of the projected buoyancy is $R(k^2/q)\widehat\theta$. Substitution gives the displayed polynomial. The stationary neutral curve is $R=q^3/k^2+Qqd^2/k^2$. No vertical boundary conditions are imposed in this plane-wave calculation.

##### Field-independent stationary threshold in oblique magnetoconvection

↑ **Parent:** [Oblique-field plane-wave magnetoconvection](#oblique-field-plane-wave-magnetoconvection)

At inclination $\alpha=\arctan\sqrt2$ and vertical wavenumber one, the nonmagnetic minimizing wavenumber $k=-1/\sqrt2$ also satisfies $\mathbf c\cdot\mathbf k=0$. The stationary threshold is the sum of $F(k)\geq27/4$ and a nonnegative magnetic penalty that vanishes there. Therefore $k_c=-1/\sqrt2$ and $R_c=27/4$ for every $Q\geq0$. The selected disturbance is constant along the imposed field, so the linear [resistive induction equation](#resistive-induction-equation) produces no magnetic perturbation and there is no field-line tension penalty.

##### Wavenumber selection in oblique-field magnetoconvection

↑ **Parent:** [Oblique-field plane-wave magnetoconvection](#oblique-field-plane-wave-magnetoconvection)

For fixed vertical wavenumber one, write the stationary threshold as $F(k)+QG(k)$, with $F=(1+k^2)^3/k^2$ and $G=(1+k^2)(\cos\alpha+k\sin\alpha)^2/k^2$. The nonmagnetic minima are $k=\pm1/\sqrt2$ with $F=27/4$; a small positive field selects the negative one. Expanding the stationarity condition gives $k_c=a-QG'(a)/F''(a)+O(Q^2)$, $a=-1/\sqrt2$, and

$$
R_c=\frac{27}{4}+3Q(\cos\alpha-\sin\alpha/\sqrt2)^2-\frac{G'(a)^2}{2F''(a)}Q^2+O(Q^3).
$$

For large $Q$, the magnetic penalty forces $k$ toward its unique zero $b=-\cot\alpha$. Since $G''(b)>0$, $k_c=b-F'(b)/[QG''(b)]+O(Q^{-2})$ and $R_c=\csc^6\alpha/\cot^2\alpha-F'(b)^2/[2QG''(b)]+O(Q^{-2})$. Thus strongly magnetized rolls align their wavevector perpendicular to the imposed field, rather than continuing to raise their stationary threshold proportionally to field strength.

#### Vertical-field magnetoconvection dispersion relation

↑ **Parent:** [Magnetoconvection](#magnetoconvection)

For a stress-free, fixed-temperature layer with vertical magnetic perturbation at its boundaries, take vertical velocity and temperature proportional to $\sin\pi z$, vertical magnetic perturbation proportional to $\cos\pi z$, and horizontal magnetic perturbations proportional to $\sin\pi z$. With $s=k^2+\pi^2$, the vertical velocity, temperature and magnetic amplitudes form a three-variable linear system whose determinant is the stated polynomial. The [Prandtl number](thermodynamics.md#prandtl-number) is $\sigma$, magnetic-to-thermal diffusivity ratio is $\zeta$, and field strength is the [Chandrasekhar number](#chandrasekhar-number) $Q$. The steady marginal curve is $R^{(e)}=[s^3+Q\pi^2s]/k^2$.

##### Three-amplitude vertical-field magnetoconvection

↑ **Parent:** [Vertical-field magnetoconvection dispersion relation](#vertical-field-magnetoconvection-dispersion-relation)

For one stress-free planar roll mode, thermal-time rescaling reduces the linear dynamics to $a'=\sigma(-a+rb-\zeta qc)$, $b'=a-b$, $c'=a-\zeta c$. Its characteristic polynomial is $(s+\sigma)(s+1)(s+\zeta)-\sigma r(s+\zeta)+\sigma\zeta q(s+1)$. For $\sigma,\zeta>0$ and $q\ge0$, steady marginality is $r_s=1+q$. Oscillatory marginality is $r_H=(\sigma+\zeta)(1+\zeta)/\sigma+\zeta(\sigma+\zeta)q/(\sigma+1)$, with $\omega_H^2=\zeta[\sigma(1-\zeta)q/(\sigma+1)-\zeta]$. A genuine [Hopf bifurcation](dynamical-systems.md#hopf-bifurcation) onset requires $\omega_H^2>0$; a formal imaginary-root formula with negative frequency squared is not an oscillation. The [Routh-Hurwitz stability criterion](dynamical-systems.md#routh-hurwitz-stability-criterion) selects the first crossing, while nonlinear coefficients determine criticality.

##### Exact critical Rayleigh relation for vertical-field magnetoconvection

↑ **Parent:** [Vertical-field magnetoconvection dispersion relation](#vertical-field-magnetoconvection-dispersion-relation)

At the minimum of the steady [vertical-field magnetoconvection dispersion relation](#vertical-field-magnetoconvection-dispersion-relation), stationarity gives $R_c=2(k_c^2+\pi^2)^3/\pi^2$. With nonmagnetic value $R_0=27\pi^4/4$, eliminating the critical [wavenumber](wave-equation.md#wavenumber) gives the stated relation and $k_c^2=\pi^2[\tfrac32(R_c/R_0)^{1/3}-1]$. These hold for every nonnegative [Chandrasekhar number](#chandrasekhar-number), including its zero-field limit.

##### Strong-field wavenumber selection in magnetoconvection

↑ **Parent:** [Vertical-field magnetoconvection dispersion relation](#vertical-field-magnetoconvection-dispersion-relation)

Both steady and oscillatory neutral curves have the form $R=C(k^2+p)^3/k^2+DQp(k^2+p)/k^2$, with $p=\pi^2$. Their exact minimizing condition is $x^2(2x+3p)=p^3+(D/C)Qp^2$, where $x=k^2$. For fixed positive coefficients and large [Chandrasekhar number](#chandrasekhar-number), $x\sim[Dp^2Q/(2C)]^{1/3}$ and $R_{\rm min}=DpQ+3C^{1/3}(Dp^2Q/2)^{2/3}+O(Q^{1/3})$. The optimum balances transverse diffusion against the magnetic penalty, leading to increasingly narrow rolls.

##### Oscillatory marginality in vertical-field magnetoconvection

↑ **Parent:** [Vertical-field magnetoconvection dispersion relation](#vertical-field-magnetoconvection-dispersion-relation)

A nonzero imaginary root of the [vertical-field magnetoconvection dispersion relation](#vertical-field-magnetoconvection-dispersion-relation) requires $0<\zeta<1$ and $Q>\zeta(1+\sigma)s^2/[\sigma(1-\zeta)\pi^2]$. Its marginal curve is $R^{(o)}=Cs^3/k^2+DQ\pi^2s/k^2$, with $C=(\sigma+\zeta)(1+\zeta)/\sigma$ and $D=\zeta(\sigma+\zeta)/(1+\sigma)$. A formal minimum of that algebraic curve is a physical oscillatory threshold only if the frequency squared there is positive.

###### Steady-Hopf merger in vertical-field magnetoconvection

↑ **Parent:** [Oscillatory marginality in vertical-field magnetoconvection](#oscillatory-marginality-in-vertical-field-magnetoconvection)

For thermal-time [magnetoconvection](#magnetoconvection), a physical oscillatory neutral mode has $\omega^2=\sigma(1-\zeta)Q_\kappa\pi^2/(1+\sigma)-\zeta^2(k^2+\pi^2)^2>0$. The steady and oscillatory neutral curves meet when this frequency tends to zero. Thus $0<\zeta<1$ is necessary and the displayed relation locates the merger. A formal oscillatory-curve minimum with negative frequency squared is not a physical onset.

###### Merger at a magnetoconvection neutral-curve minimum

↑ **Parent:** [Steady-Hopf merger in vertical-field magnetoconvection](#steady-hopf-merger-in-vertical-field-magnetoconvection)

At a steady-curve minimum, differentiation and the [steady-Hopf merger in vertical-field magnetoconvection](#steady-hopf-merger-in-vertical-field-magnetoconvection) give the first displayed wavenumber. At an oscillatory-curve minimum they give the second. For fixed positive [Prandtl number](thermodynamics.md#prandtl-number) $\sigma$ and large $Q_\kappa$, the corresponding merger diffusivity deficits are $1-\zeta_s\sim[(1+\sigma)/\sigma](\pi^2/(4Q_\kappa))^{1/3}$ and $1-\zeta_o\sim[(1+\sigma)\pi^2/(16\sigma Q_\kappa)]^{1/3}$. The two parameter surfaces are distinct: coincidence of neutral curves at one wavenumber does not imply coincidence of their minimizing wavenumbers.

#### Chandrasekhar number

↑ **Parent:** [Magnetoconvection](#magnetoconvection)

For an imposed field $B_0$ in a layer of depth $d$, the [Chandrasekhar number](#chandrasekhar-number) compares magnetic tension with viscous and magnetic-diffusive effects. Here $\eta$ is [magnetic diffusivity](#magnetic-diffusivity) and $\nu$ is [kinematic viscosity](fluid-mechanics.md#kinematic-viscosity). In thermal-diffusion units the linear magnetic-force coefficient is $Q\zeta$, where $\zeta=\eta/\kappa$ and $\kappa$ is [thermal diffusivity](thermodynamics.md#thermal-diffusivity).

##### Thermal-diffusion magnetic-field parameter

↑ **Parent:** [Chandrasekhar number](#chandrasekhar-number)

With [thermal diffusivity](thermodynamics.md#thermal-diffusivity) $\kappa$ and [magnetic diffusivity](#magnetic-diffusivity) $\eta$, the standard [Chandrasekhar number](#chandrasekhar-number) uses $\nu\eta$ in its denominator. A thermal-diffusion alternative uses $\nu\kappa$ and is $\zeta=\eta/\kappa$ times the standard parameter. In thermal-time [magnetoconvection](#magnetoconvection) equations, the linear magnetic-force coefficient is $\sigma Q_\kappa=\sigma\zeta Q_{\mathrm{Ch}}$. Specifying the convention prevents a missing diffusivity factor in a dispersion relation.

#### Convection amplitude coupled to a conserved field

↑ **Parent:** [Magnetoconvection](#magnetoconvection)

A representative scaled amplitude model has complex $A$ and real $B$ with

$$
A_T=A+A_{XX}-A|A|^2-AB,\qquad B_T=\sigma B_{XX}+\mu(|A|^2)_{XX},\qquad\sigma>0.
$$

[Periodic boundary conditions](differential-equation.md#periodic-boundary-conditions) conserve $\int B\,dX$, because the right-hand side is a total second derivative. The slow field can change long-wave [convection roll](fluid-mechanics.md#convection-roll) stability and permit localized pulses. For zero mean $B$, the uniform [convection rolls](fluid-mechanics.md#convection-roll) are $A=Re^{iqX}$, $R^2=1-q^2$, $B=0$.

##### Localized pulse of a conserved-field convection model

↑ **Parent:** [Convection amplitude coupled to a conserved field](#convection-amplitude-coupled-to-a-conserved-field)

For a real steady amplitude and zero-mean field, twice integrating the field equation yields $B=\kappa(\langle A^2\rangle-A^2)$, $\kappa=\mu/\sigma$. The [amplitude equation](dynamical-systems.md#amplitude-equation) becomes $A''+(1-\kappa\langle A^2\rangle)A+(\kappa-1)A^3=0$. Using $(R\operatorname{sech}cX)''=c^2A-2c^2A^3/R^2$ gives $\kappa\langle A^2\rangle=1+c^2$ and $R^2=2c^2/(\kappa-1)$, requiring $\kappa>1$. Its finite-window mean is $2R^2\tanh(cL/2)/(cL)$. For $cL\gg1$, consistency gives $c+c^{-1}=4\kappa/[L(\kappa-1)]$. The leading roots coalesce at $c=1$; for $L>2$ the leading upper parameter limit is $\kappa\leq L/(L-2)$, while retaining the finite-window factor makes the necessary inequality strict. The isolated sech profile has an exponentially small derivative mismatch on a periodic interval, so exact periodic tails need correction. For $L\leq2$ the algebra supplies no finite upper bound of this form.

##### Conserved-field sideband dispersion relation

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

###### Long-wave instability with a conserved mean field

↑ **Parent:** [Conserved-field sideband dispersion relation](#conserved-field-sideband-dispersion-relation)

Putting $\lambda=l^2\nu$ into the sideband cubic and retaining $l^4$ gives

$$
r\nu^2-[(\mu-\sigma-1)r+2q^2]\nu-[(\mu-\sigma)r+2\sigma q^2]=0.
$$

For $r=1-q^2>0$, $\mu/\sigma>(1-3q^2)/(1-q^2)$ makes the constant coefficient negative. There is a positive real $\nu$, so sufficiently small nonzero $l$ grows. On a finite period $L$, however, only $l=2\pi j/L$ are allowed. For $q=0$, $\mu=2$, $\sigma=1$, $L=1$, every nonzero allowed mode has negative growth rates despite this long-wave inequality. Thus an arbitrarily-small-wave-number conclusion cannot be asserted without the domain-size qualification.

### Magnetic buoyancy instability

↑ **Parent:** [Magnetohydrodynamics](#magnetohydrodynamics)

A [magnetic buoyancy instability](#magnetic-buoyancy-instability) is a gravitational instability of a magnetized stratified fluid in which displacements of the gas and [magnetic field](electromagnetism.md#magnetic-field) can release [Newtonian gravitational potential energy](classical-mechanics.md#newtonian-gravitational-potential-energy). [Magnetic pressure](#magnetic-pressure) supports part of the weight. Both interchange displacements and undular displacements can enter this broad category; [Parker instability](#parker-instability) is the undular mechanism involving drainage along bent [magnetic field lines](electromagnetism.md#magnetic-field-line).

#### Isothermal interchange criterion for magnetic buoyancy

↑ **Parent:** [Magnetic buoyancy instability](#magnetic-buoyancy-instability)

A horizontal [flux tube](electromagnetism.md#flux-tube) displaced without bending preserves $B/\rho$ by [magnetic flux freezing](#magnetic-flux-freezing). If thermal exchange keeps its temperature equal to its new surroundings, lateral [magnetic pressure](#magnetic-pressure) balance gives $(c_T^2+v_A^2)(\rho_i'-\rho')=\rho B(B/\rho)'/\mu_0$. Here $c_T^2=p/\rho$, $v_A^2=B^2/(\mu_0\rho)$, and primes denote the response to a small vertical displacement from an equilibrium. Its linear [buoyancy](fluid-mechanics.md#buoyancy) acceleration is $-gB(B/\rho)'\xi/[\mu_0(c_T^2+v_A^2)]$. Thus local interchange is unstable when $B(B/\rho)'<0$, equivalently $(B^2/\rho^2)'<0$. This fast-thermal-exchange criterion differs from the adiabatic [localized interchange criterion for a magnetized atmosphere](#localized-interchange-criterion-for-a-magnetized-atmosphere).

#### Localized interchange criterion for a magnetized atmosphere

↑ **Parent:** [Magnetic buoyancy instability](#magnetic-buoyancy-instability)

For disturbances constant along the horizontal [magnetic field](electromagnetism.md#magnetic-field), the minimized energy [density](fluid-mechanics.md#density) is $\rho g[-(\ln\rho)'-\rho g/(\gamma p+C)]|\xi_z|^2$. If its coefficient is nonnegative everywhere, the full energy is nonnegative. If it is strictly negative at a point of a smooth equilibrium, a compactly supported vertical displacement in a neighbouring interval gives negative energy. These interchange motions compress gas and [magnetic pressure](#magnetic-pressure) together.

#### Parker instability

↑ **Parent:** [Magnetic buoyancy instability](#magnetic-buoyancy-instability)

[Parker instability](#parker-instability) is an undular [magnetic buoyancy instability](#magnetic-buoyancy-instability) of a gravitationally stratified atmosphere supported partly by [magnetic pressure](#magnetic-pressure). A bent horizontal [magnetic field](electromagnetism.md#magnetic-field) can permit gas to drain along its [magnetic field lines](electromagnetism.md#magnetic-field-line), leaving buoyant rising regions. [Magnetic tension](#magnetic-tension) resists bending, so wavelengths and [boundary conditions](differential-equation.md#boundary-condition) affect the instability threshold. For a [magnetized isothermal atmosphere](electromagnetism.md#magnetized-isothermal-atmosphere), the unrestricted-wavevector threshold is given by the [magnetic buoyancy energy criterion](#magnetic-buoyancy-energy-criterion).

##### Long-wavelength undular magnetic buoyancy criterion

↑ **Parent:** [Parker instability](#parker-instability)

At nonzero along-field wavenumber, put $q=ik_y\xi_y$, $P=\gamma p$ and $C=B^2/\mu_0$. After [pressure](thermodynamics.md#pressure) minimization the energy [density](fluid-mechanics.md#density) completes to $CP/(P+C)|q-\rho g\xi_z/P|^2+[Ck_y^2-g\rho'-\rho^2g^2/P]|\xi_z|^2$. Choosing the square to vanish and then taking a sufficiently small nonzero $k_y$ gives negative energy exactly when the displayed strict criterion holds somewhere. A fixed prescribed wavenumber retains the stabilizing $Ck_y^2$ tension term; the criterion asserts existence of an allowed nonzero wavenumber. The associated along-field displacement lets material drain while [magnetic flux](electromagnetism.md#magnetic-flux) bends.

##### Magnetic buoyancy energy criterion

↑ **Parent:** [Parker instability](#parker-instability)

For the [magnetized isothermal atmosphere](electromagnetism.md#magnetized-isothermal-atmosphere), set $a=1/(2H)$, $s=v_s^2>0$, $b=v_a^2>0$ and $\Delta=ik_x\xi_x+ik_y\xi_y+(ik_z+a)\xi_z$. After weighting the displacement by $e^{z/(2H)}$, the restoring [Hermitian matrix](hilbert-space.md#hermitian-operator) $\mathsf K$ satisfies

$$
\boldsymbol\xi^\dagger\mathsf K\boldsymbol\xi=
s\left|\Delta-\frac g{s}\xi_z\right|^2+
b\left|ik_x\xi_x+(ik_z+a)\xi_z\right|^2+
bk_y^2(|\xi_x|^2+|\xi_z|^2)+
\left(\frac gH-\frac{g^2}{s}\right)|\xi_z|^2.
$$

Thus $gH\leq s$ makes the form nonnegative for every [wavevector](continuum-mechanics.md#wavevector). If $gH>s$, choose $k_z=0$, $k_x\ne0$, $\xi_z=1$, $\xi_x=-a/(ik_x)$ and $\xi_y=g/(sik_y)$. The squares vanish, and sufficiently small nonzero $k_y$ gives a negative form. The [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient) proves instability when these wavelengths are admissible. Since $s=\gamma c_s^2$ and $\beta=2c_s^2/b$, the condition is precisely $\beta(\gamma-1)<1$.

###### Short transverse wavelength limit for magnetic buoyancy

↑ **Parent:** [Magnetic buoyancy energy criterion](#magnetic-buoyancy-energy-criterion)

For a horizontal field, set $C=B^2/\mu_0$. Static force balance gives $\delta\Pi=\rho g\xi_z-(\gamma p+C)\nabla\cdot\xi+Cik_y\xi_y$. Given smooth compactly supported vertical and along-field displacements, the displayed choice makes total-pressure perturbation zero while $\xi_x=O(k_x^{-1})$. The nonnegative [pressure](thermodynamics.md#pressure) and transverse-tension terms vanish as $|k_x|\to\infty$. This constructs the infimum needed for the [magnetohydrodynamic energy principle](#magnetohydrodynamic-energy-principle); a strictly negative limit is already negative at some finite wavenumber.

### Poloidal magnetic field

↑ **Parent:** [Magnetohydrodynamics](#magnetohydrodynamics)

A poloidal [magnetic field](electromagnetism.md#magnetic-field) lies in meridional planes through the symmetry axis, in contrast to a [toroidal magnetic field](#toroidal-magnetic-field). For an [axisymmetric vector field](calculus.md#axisymmetric-vector-field), it is represented by a [poloidal magnetic flux function](#poloidal-magnetic-flux-function) as $\mathbf B_p=R^{-1}\nabla\Psi\times\mathbf e_\phi$.

### Magnetic pressure

↑ **Parent:** [Magnetohydrodynamics](#magnetohydrodynamics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Magnetic_pressure)

Magnetic pressure is the isotropic part of magnetic stress. It is $p_B=B^2/(2\mu_0)$ in SI units and $B^2/(8\pi)$ in Gaussian units.

#### Magnetic pressure discontinuity in an isothermal atmosphere

↑ **Parent:** [Magnetic pressure](#magnetic-pressure)

Two uniform horizontal [magnetic fields](electromagnetism.md#magnetic-field) on either side of a horizontal interface exert no bulk force, but their [magnetic pressures](#magnetic-pressure) differ. For a common-temperature [isothermal atmosphere](statistical-physics.md#isothermal-atmosphere) with sound-speed squared $c_T^2=\mathcal RT_0$ and gravity $g$, [hydrostatic equilibrium](statistical-physics.md#hydrostatic-equilibrium) gives $p_i=c_T^2\rho_i$ and $p_i(z)=p_i(0)e^{-z/H}$, $H=c_T^2/g$. Continuity of [magnetohydrodynamic total pressure](#magnetohydrodynamic-total-pressure) gives the displayed density jump. A stronger field below means denser gas above, supplying a [Rayleigh-Taylor instability](continuum-mechanics.md#rayleigh-taylor-instability) even though each half-space is hydrostatic.

// Target: continuum-mechanics.bigb

#### Magnetohydrodynamic total pressure

↑ **Parent:** [Magnetic pressure](#magnetic-pressure)

The [magnetohydrodynamic total pressure](#magnetohydrodynamic-total-pressure) is $\Pi=p+B^2/(2\mu_0)$, the sum of gas [pressure](thermodynamics.md#pressure) and [magnetic pressure](#magnetic-pressure). The remaining [Lorentz force](electromagnetism.md#lorentz-force) is [magnetic tension](#magnetic-tension), so this scalar does not include the entire magnetic stress.

### Magnetic tension

↑ **Parent:** [Magnetohydrodynamics](#magnetohydrodynamics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Magnetic_tension)

Magnetic tension is the restoring stress associated with bending magnetic field lines. In a divergence-free field, the Lorentz-force density splits into a magnetic-pressure gradient and the tension term $(\mathbf B\mathbin\cdot\nabla)\mathbf B/\mu_0$ in SI units.

### Toroidal magnetic field

↑ **Parent:** [Magnetohydrodynamics](#magnetohydrodynamics)

A toroidal magnetic field points in the azimuthal direction around a chosen symmetry axis. Its curved field lines exert inward magnetic tension $-B_\phi^2/(\mu_0R)$ in cylindrical geometry.

#### Toroidal magnetic-field winding equation

↑ **Parent:** [Toroidal magnetic field](#toroidal-magnetic-field)

In axisymmetric [ideal magnetohydrodynamics](#ideal-magnetohydrodynamics), $\Omega=u_\phi/R$ is the material angular velocity. Cylindrical basis-vector derivatives and [mass conservation](continuum-mechanics.md#mass-conservation) give the displayed winding equation. Thus $B_\phi/(\rho R)$ is an advected scalar only when $\mathbf B_p\cdot\nabla\Omega=0$. Differential rotation along a field line otherwise produces toroidal field. This does not violate [magnetic flux freezing](#magnetic-flux-freezing), which concerns flux through a material surface rather than a cylindrical vector component.

##### Steady toroidal induction by spherical differential rotation

↑ **Parent:** [Toroidal magnetic-field winding equation](#toroidal-magnetic-field-winding-equation)

An axial uniform [magnetic field](electromagnetism.md#magnetic-field) and localized radial [differential rotation](#differential-rotation) generate a steady [toroidal magnetic field](#toroidal-magnetic-field). The angular factor $\sin\theta\cos\theta$ is an eigenfunction of the toroidal angular diffusion operator with eigenvalue $-6$. Its radial amplitude satisfies $\eta(f''+2f'/r-6f/r^2)=-B_0r\Omega'$. Differentiating the integral in the title proves the formula. It is regular at the origin and decays at infinity when $\Omega$ is finite at zero and decays sufficiently rapidly.

###### Diffusive establishment time of a wound toroidal field

↑ **Parent:** [Steady toroidal induction by spherical differential rotation](#steady-toroidal-induction-by-spherical-differential-rotation)

With a fixed axial seed field and prescribed localized [differential rotation](#differential-rotation), the winding source is time independent. Early induction gives $B_\phi\sim B_0\Omega t$, while the steady balance has $B_\phi\sim B_0\Omega\ell^2/\eta$. Their comparison gives the [magnetic diffusion](#magnetic-diffusion) time, not merely the rotation period. It diverges as conductivity becomes infinite. In an unbounded domain, this is a local equilibration estimate on scale $\ell$, not finite-time exact convergence everywhere. [Lorentz force](electromagnetism.md#lorentz-force) feedback may invalidate the prescribed-flow approximation sooner.

#### Michael criterion for axisymmetric toroidal-field interchange

↑ **Parent:** [Toroidal magnetic field](#toroidal-magnetic-field)

For constant-density cylindrical rotation $r\Omega(r)\mathbf e_\phi$ and a purely toroidal [magnetic field](electromagnetism.md#magnetic-field), an axisymmetric radial displacement gives $b_\phi=(B_\phi/r-B_\phi')\xi_r$. Combining its curvature force with conservation of angular momentum gives the restoring coefficient $\mathcal D$ above. A local incompressible radial-vertical mode has $\omega^2=(k_z^2/k^2)\mathcal D$. Positive $\mathcal D$ gives stability in this ideal interchange setting; negative $\mathcal D$ permits growth. This is distinct from weak-field [magnetorotational instability](astrophysics.md#magnetorotational-instability): a steeply increasing toroidal field can release current energy even without differential rotation.

##### Toroidal interchange field threshold in a thin Keplerian disk

↑ **Parent:** [Michael criterion for axisymmetric toroidal-field interchange](#michael-criterion-for-axisymmetric-toroidal-field-interchange)

For $B_\phi\propto r^p$, constant [density](fluid-mechanics.md#density) and Keplerian $\kappa^2=\Omega^2$, the [Michael criterion for axisymmetric toroidal-field interchange](#michael-criterion-for-axisymmetric-toroidal-field-interchange) becomes $\Omega^2-2(p-1)v_A^2/r^2$. Instability therefore requires $p>1$ and $v_A^2>r^2\Omega^2/[2(p-1)]$. For a field varying on the radial scale $r$, this is an orbital-speed field, much stronger than a gas-pressure-scale field with $v_A\lesssim c_s\sim H\Omega$ in a [thin disk](astrophysics.md#thin-disk). Steep radial field gradients require the exact derivative criterion rather than this scale estimate. The instability is powered by the toroidal field distribution and is distinct from weak vertical-field [magnetorotational instability](astrophysics.md#magnetorotational-instability).

// Target: fluid-mechanics.bigb

##### Global variational form of the Michael criterion

↑ **Parent:** [Michael criterion for axisymmetric toroidal-field interchange](#michael-criterion-for-axisymmetric-toroidal-field-interchange)

For rigid walls $a<r<b$, a nonzero vertical [wavenumber](wave-equation.md#wavenumber) $k$ and radial [Lagrangian fluid displacement](continuum-mechanics.md#lagrangian-fluid-displacement) $\xi$, set $y=r\xi$ and $\mathcal D=\kappa^2-r(d/dr)(v_A^2/r^2)$. Axisymmetric modes satisfy

$$
\omega^2\left[-\left(\frac{y'}r\right)'+\frac{k^2y}r\right]=\frac{k^2\mathcal D}r y,\qquad y(a)=y(b)=0.
$$

The operator on the left is a positive [self-adjoint operator](linear-operator-theory.md#self-adjoint-operator). Its [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient) is $\omega^2=k^2\int\mathcal D|y|^2/r\,dr\big/\int(|y'|^2+k^2|y|^2)/r\,dr$. All mode squares are real; a growing mode exists exactly when the continuous coefficient $\mathcal D$ is negative somewhere. Sufficiency follows by a test function supported in that negative interval and the [compact operator](compact-operator.md) and [self-adjoint operator](linear-operator-theory.md#self-adjoint-operator) eigenproblem obtained by conjugating the multiplication operator with the inverse square root of the positive differential operator.

// Target: astrophysical-fluid-dynamics.bigb

#### Uniform-current toroidal-field curl reduction

↑ **Parent:** [Toroidal magnetic field](#toroidal-magnetic-field)

For constant-density incompressible [ideal magnetohydrodynamics](#ideal-magnetohydrodynamics) about $\mathbf B=Jr\mathbf e_\phi$, the cylindrical basis contributions make the linearized [Lorentz force](electromagnetism.md#lorentz-force) equal to $imJ\mathbf b+2J\mathbf e_z\times\mathbf b$, apart from a [magnetic pressure](#magnetic-pressure) gradient. The induction equation reduces to $i\omega\mathbf b=imJ\mathbf u$. Taking the curl after eliminating velocity gives the displayed relation, with $\widetilde J=J/\sqrt{\mu_0\rho}$. A second curl gives a vector Helmholtz equation and squared frequencies $\omega^2=\widetilde J^2[m^2\pm2|mk|/(\alpha^2+k^2)^{1/2}]$. The lower $|m|=1$ branch grows when $3k^2>\alpha^2$.

##### Neutral quadrupolar perturbation of a uniform-current toroidal field

↑ **Parent:** [Uniform-current toroidal-field curl reduction](#uniform-current-toroidal-field-curl-reduction)

The displayed [solenoidal vector field](calculus.md#solenoidal-vector-field) has $\nabla\times\mathbf b=k\mathbf b$, $\nabla^2\mathbf b=-k^2\mathbf b$ and $\mathbf e_z\times\mathbf b=-i\mathbf b$. Thus the non-gradient part of its linearized [Lorentz force](electromagnetism.md#lorentz-force) about $\mathbf B=Jr\mathbf e_\phi$ vanishes. Choosing $p_1=-\mathbf B\cdot\mathbf b/\mu_0$ cancels the magnetic-pressure gradient, and $\mathbf u=0$, $\omega=0$ is a neutral perturbation. It is regular at the axis and realizes the endpoint $m=2$, $\alpha=0$. A boundary condition can exclude this growing-in-radius field, but without such a condition strict positivity at the endpoint cannot be asserted.

### Ideal magnetohydrodynamics

↑ **Parent:** [Magnetohydrodynamics](#magnetohydrodynamics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ideal_magnetohydrodynamics)

Ideal magnetohydrodynamics assumes vanishing resistivity, so magnetic flux is frozen into the fluid and the electric field in the fluid rest frame vanishes.

#### Magnetic relaxation

↑ **Parent:** [Ideal magnetohydrodynamics](#ideal-magnetohydrodynamics)

Magnetic relaxation converts [magnetic energy](electromagnetism.md#magnetic-energy) into material motion through the [Lorentz force density](electromagnetism.md#lorentz-force-density), and dissipates the resulting [kinetic energy](classical-mechanics.md#kinetic-energy) through [viscosity](fluid-mechanics.md#dynamic-viscosity). In a [perfect conductor](electromagnetism.md#perfect-conductor), [magnetic flux freezing](#magnetic-flux-freezing) preserves field-line connectivity throughout every smooth stage. A regular limiting state has zero [velocity](classical-mechanics.md#velocity) and is a [magnetostatic equilibrium](electromagnetism.md#magnetostatic-equilibrium), but its [magnetic field](electromagnetism.md#magnetic-field) can contain [current sheets](electromagnetism.md#current-sheet). Conservation of one global [magnetic helicity](electromagnetism.md#magnetic-helicity) is weaker than preservation of the complete frozen field-line structure.

##### Collapse of a planar magnetic separatrix

↑ **Parent:** [Magnetic relaxation](#magnetic-relaxation)

For a planar [magnetic field](electromagnetism.md#magnetic-field) $\mathbf B=(\psi_y,-\psi_x,0)$, ideal induction advects the [Cartesian magnetic flux function](#cartesian-magnetic-flux-function): $D_t\psi=0$. [Incompressible flow](fluid-mechanics.md#incompressible-flow) also preserves the area inside each material contour. During relaxation, the arms of a magnetic [separatrix](dynamical-systems.md#separatrix) can approach each other while their field-line connectivity remains fixed. A transition of width $\epsilon$ with a finite change of tangential field has [electric current density](electromagnetism.md#current-density) of order $\epsilon^{-1}$ and can approach a [current sheet](electromagnetism.md#current-sheet). This is a possible limiting mechanism, not a claim that every planar equilibrium is singular.

##### Viscous magnetic-relaxation energy identity

↑ **Parent:** [Magnetic relaxation](#magnetic-relaxation)

For constant [mass density](fluid-mechanics.md#density) $\rho$, [kinematic viscosity](fluid-mechanics.md#kinematic-viscosity) $\nu>0$, ideal induction, zero boundary [velocity](classical-mechanics.md#velocity) and tangent [magnetic field](electromagnetism.md#magnetic-field), put $E=\int_D[\rho|\mathbf v|^2/2+|\mathbf B|^2/(2\mu_0)]dV$. Multiplying the momentum equation by $\mathbf v$ and integrating cancels pressure work and advective flux. The magnetic-energy derivative is minus the integral of [Lorentz force density](electromagnetism.md#lorentz-force-density) dotted with [velocity](classical-mechanics.md#velocity), canceling the same work in the kinetic-energy equation. [Integration by parts](calculus.md#integration-by-parts) then gives the displayed identity. For [incompressible flow](fluid-mechanics.md#incompressible-flow) with zero boundary velocity, $\int|\nabla\mathbf v|^2=\int|\nabla\times\mathbf v|^2$.

#### Steady planar ideal-MHD field-line invariants

↑ **Parent:** [Ideal magnetohydrodynamics](#ideal-magnetohydrodynamics)

For a stationary, $z$-independent [ideal magnetohydrodynamics](#ideal-magnetohydrodynamics) flow with $E_z=0$, nonzero horizontal [magnetic field](electromagnetism.md#magnetic-field) and nonzero [magnetohydrodynamic mass loading](#magnetohydrodynamic-mass-loading) $k$, the displayed decomposition has $\mathbf B\cdot\nabla k=\mathbf B\cdot\nabla U=0$. The [continuity equation](physics.md#continuity-equation) gives the first invariant, and the [ideal magnetohydrodynamic induction equation](#ideal-magnetohydrodynamic-induction-equation) gives the second. Entropy and $V=u_z-B_z/(\mu_0k)$ are also constant on each [magnetic field line](electromagnetism.md#magnetic-field-line). Stationarity alone permits constant nonzero $E_z$, so it does not imply this decomposition.

<h5 id="alfvenic-degeneracy-of-steady-planar-mhd">Alfvénic degeneracy of steady planar MHD</h5>

↑ **Parent:** [Steady planar ideal-MHD field-line invariants](#steady-planar-ideal-mhd-field-line-invariants)

The two axial invariants in [steady planar ideal-MHD field-line invariants](#steady-planar-ideal-mhd-field-line-invariants) give the displayed identity. When $V-U\ne0$, a finite smooth flow cannot reach horizontal [Alfvén speed](#alfven-speed). When $V=U$, an everywhere Alfvénic branch is possible even with $B_z\ne0$: constant $\rho$ and $\mathbf u=\mathbf B/\sqrt{\mu_0\rho}$ give an example. The nondegenerate exclusion must not be applied to this branch.

##### Planar ideal-MHD Bernoulli invariant

↑ **Parent:** [Steady planar ideal-MHD field-line invariants](#steady-planar-ideal-mhd-field-line-invariants)

Under the hypotheses of [steady planar ideal-MHD field-line invariants](#steady-planar-ideal-mhd-field-line-invariants), the [specific enthalpy](thermodynamics.md#specific-enthalpy) relation and the velocity projection of momentum give $\mathbf B\cdot\nabla Q=0$. The horizontal total energy flux, including the [Poynting vector](electromagnetism.md#poynting-vector), is $k\mathbf B_h Q$. The magnetic correction accounts for work exchanged between the fluid and the field.

#### Grad-Shafranov equation

↑ **Parent:** [Ideal magnetohydrodynamics](#ideal-magnetohydrodynamics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Grad–Shafranov_equation)

The Grad-Shafranov equation governs the poloidal magnetic flux of an axisymmetric magnetohydrostatic equilibrium. Pressure and toroidal-field contributions depend on the flux function. The [Grad-Shafranov equation for a force-free magnetic field](#grad-shafranov-equation-for-a-force-free-magnetic-field) is its zero-pressure-gradient reduction.

##### Grad-Shafranov equation for a force-free magnetic field

↑ **Parent:** [Grad-Shafranov equation](#grad-shafranov-equation)

For an axisymmetric force-free field with $\mathbf B_p=\nabla\psi\times\nabla\phi$ and $rB_\phi=F(\psi)$, the flux function obeys

$$
-r\frac{\partial}{\partial r}\left(\frac1r\frac{\partial\psi}{\partial r}\right)
-\frac{\partial^2\psi}{\partial z^2}
=F\frac{dF}{d\psi}.
$$

#### Reduced magnetohydrodynamics

↑ **Parent:** [Ideal magnetohydrodynamics](#ideal-magnetohydrodynamics)

[Reduced magnetohydrodynamics](#reduced-magnetohydrodynamics) is the leading ideal-fluid description of small, anisotropic fluctuations about a strong uniform guide field, with $k_\parallel/k_\perp\sim\delta B_\perp/B_0\sim\delta u_\perp/v_A\ll1$. Its [solenoidal](calculus.md#solenoidal-vector-field) perpendicular [Elsässer variables](#elsasser-variable) obey

$$
\partial_t\mathbf z^\pm_\perp\mp v_A\partial_z\mathbf z^\pm_\perp+(\mathbf z^\mp_\perp\cdot\nabla_\perp)\mathbf z^\pm_\perp=-\nabla_\perp\Pi.
$$

The parallel magnetic derivative includes bending of field lines: $\nabla_\parallel=\partial_z+(\delta\mathbf B_\perp/B_0)\cdot\nabla_\perp$. Slow compressive and [entropy mode](#entropy-mode) fluctuations are passively transported at this order. The system excludes the rapidly propagating [fast magnetosonic wave](#fast-magnetosonic-wave) sector rather than describing all possible [MHD](#magnetohydrodynamics) perturbations.

##### Five quadratic cascade invariants of anisotropic magnetohydrodynamic turbulence

↑ **Parent:** [Reduced magnetohydrodynamics](#reduced-magnetohydrodynamics)

For ideal [reduced magnetohydrodynamics](#reduced-magnetohydrodynamics) with periodic or vanishing-flux boundaries, the five quadratic cascade channels are $I_A^\pm=\int|\mathbf z_\perp^\pm|^2dV$, $I_S^\pm=\int(f^\pm)^2dV$ and $I_e=\int s^2dV$. The perpendicular [Elsässer variables](#elsasser-variable), slow-wave amplitudes $f^\pm$, and [entropy](thermodynamics.md#entropy) fluctuation $s$ each obey an equation with [divergence-free](calculus.md#solenoidal-vector-field) advection. Multiplying each equation by its own field and integrating makes both advection and propagation terms boundary fluxes, while the perpendicular [pressure](thermodynamics.md#pressure) term vanishes by solenoidality. Each integral is therefore separately conserved. The two Alfvén cascades distort one another without exchanging their integrated invariants; the other three are passively cascaded by the Alfvénic motion without feedback at this order. This count concerns quadratic fluctuation-energy channels: an advected scalar also conserves arbitrary integrals $\int F(s)dV$, which are not extra independent quadratic modal channels.

##### Slow and entropy fluctuations in reduced magnetohydrodynamics

↑ **Parent:** [Reduced magnetohydrodynamics](#reduced-magnetohydrodynamics)

In ideal [reduced magnetohydrodynamics](#reduced-magnetohydrodynamics) with constant background sound and [Alfvén speeds](#alfven-speed), perpendicular total-pressure balance gives $\delta p+\rho_0v_A^2\delta B_\parallel/B_0=0$. Put $s=\delta p/p_0-\gamma\delta\rho/\rho_0$, $r=\delta\rho/\rho_0+s/\gamma$, $c_T=v_Ac_s/(v_A^2+c_s^2)^{1/2}$ and $h=c_s^2r/c_T$. Then the parallel momentum, continuity and induction equations yield

$$
Du_\parallel=-c_T\nabla_\parallel h,\qquad Dh=-c_T\nabla_\parallel u_\parallel,\qquad Ds=0.
$$

Thus $f^\pm=u_\parallel\pm h$ satisfy $Df^\pm=\mp c_T\nabla_\parallel f^\pm$. The two slow-wave populations propagate along bent [magnetic field lines](electromagnetism.md#magnetic-field-line) and are mixed by the perpendicular [Alfvénic turbulence](turbulence.md#alfvenic-turbulence), while the [entropy](thermodynamics.md#entropy) fluctuation is simply advected. They do not force the perpendicular Alfvénic system at this leading order.

#### Ideal magnetohydrodynamic energy conservation

↑ **Parent:** [Ideal magnetohydrodynamics](#ideal-magnetohydrodynamics)

For a fixed [Newtonian gravitational potential](classical-mechanics.md#newtonian-gravitational-potential), total [energy density](statistical-physics.md#energy-density) is $\mathcal E=\rho(u^2/2+\Phi)+p/(\gamma-1)+B^2/(2\mu_0)$. Its flux combines advected kinetic/potential energy, [specific enthalpy](thermodynamics.md#specific-enthalpy) and the [Poynting vector](electromagnetism.md#poynting-vector). Dotting the [ideal magnetohydrodynamic momentum equation](#ideal-magnetohydrodynamic-momentum-equation) with [velocity](classical-mechanics.md#velocity), adding the adiabatic [internal energy](thermodynamics.md#internal-energy) equation and the [magnetic energy](electromagnetism.md#magnetic-energy) equation cancels the magnetic work. The [pressure](thermodynamics.md#pressure) terms combine into $-\nabla\cdot(p\mathbf u)$, proving the conservation law. A time-dependent imposed potential instead contributes $\rho\partial_t\Phi$.

#### Ideal magnetohydrodynamic momentum equation

↑ **Parent:** [Ideal magnetohydrodynamics](#ideal-magnetohydrodynamics)

The inviscid [magnetohydrodynamic momentum equation](#magnetohydrodynamic-momentum-equation) balances inertia, [pressure](thermodynamics.md#pressure), [gravitational acceleration](classical-mechanics.md#gravitational-acceleration) and [Lorentz force density](electromagnetism.md#lorentz-force-density). The magnetic force separates into [magnetic tension](#magnetic-tension) and [magnetic pressure](#magnetic-pressure). It is coupled to the [continuity equation](physics.md#continuity-equation) and the [ideal magnetohydrodynamic induction equation](#ideal-magnetohydrodynamic-induction-equation).

#### Plane-parallel magnetohydrodynamic flow with imposed shear

↑ **Parent:** [Ideal magnetohydrodynamics](#ideal-magnetohydrodynamics)

A useful [ideal magnetohydrodynamics](#ideal-magnetohydrodynamics) reduction has $\mathbf u=\mathbf v(z,t)+ax\mathbf e_y$, $\mathbf B=\mathbf B(z,t)$ and $\rho=\rho(z,t)$. The constant background [shear flow](fluid-mechanics.md#shear-flow) supplies $av_x$ in the axial momentum equation and $aB_x$ in axial magnetic induction. The solenoidal constraint and [MHD induction equation](#ideal-magnetohydrodynamic-induction-equation) together make $B_z$ constant.

<h5 id="alfven-point-compatibility-in-a-plane-parallel-sheared-flow">Alfvén-point compatibility in a plane-parallel sheared flow</h5>

↑ **Parent:** [Plane-parallel magnetohydrodynamic flow with imposed shear](#plane-parallel-magnetohydrodynamic-flow-with-imposed-shear)

At $w^2=v_{az}^2$, the transverse steady equations require $wB_xw'=0$ and $wB_yw'=a(wB_x-B_zv_x)$. These conditions can be lost by division when eliminating transverse magnetic derivatives. A scalar equation displaying the [magnetosonic critical speeds](#magnetosonic-critical-speed) need not display every compatibility condition at an [Alfvén speed](#alfven-speed).

##### Magnetohydrodynamic shear work

↑ **Parent:** [Plane-parallel magnetohydrodynamic flow with imposed shear](#plane-parallel-magnetohydrodynamic-flow-with-imposed-shear)

The energy of the residual flow and [magnetic field](electromagnetism.md#magnetic-field) in a maintained [shear flow](fluid-mechanics.md#shear-flow) has source $S=-aT_{xy}$, where $T_{xy}=\rho v_xv_y-B_xB_y/\mu_0$. The kinetic and magnetic stresses can exchange energy with the imposed background. The source vanishes when their off-diagonal contributions cancel.

#### Ideal magnetohydrodynamic equations

↑ **Parent:** [Ideal magnetohydrodynamics](#ideal-magnetohydrodynamics)

The smooth ideal-MHD system couples [mass conservation](continuum-mechanics.md#mass-conservation), [momentum](classical-mechanics.md#momentum), adiabatic [pressure](thermodynamics.md#pressure) transport and the [ideal magnetohydrodynamic induction equation](#ideal-magnetohydrodynamic-induction-equation), subject to the [solenoidal magnetic-field constraint](electromagnetism.md#solenoidal-magnetic-field-constraint). Without gravity it is a [quasilinear partial differential equation](partial-differential-equation.md#quasilinear-partial-differential-equation) system. Across shocks, conservative total energy replaces smooth adiabatic [pressure](thermodynamics.md#pressure) transport.

#### Magnetohydrodynamic energy principle

↑ **Parent:** [Ideal magnetohydrodynamics](#ideal-magnetohydrodynamics)

For a static smooth [ideal magnetohydrodynamics](#ideal-magnetohydrodynamics) equilibrium with conservative external forces and surface terms eliminated by the [boundary conditions](differential-equation.md#boundary-condition), the linear displacement equation is $\rho\ddot{\boldsymbol\xi}=\mathcal F\boldsymbol\xi$, where the force operator is a [self-adjoint operator](linear-operator-theory.md#self-adjoint-operator) in the appropriate integral pairing. Its restoring [quadratic form](linear-algebra.md#quadratic-form) $\delta W=-\tfrac12\int\boldsymbol\xi^*\cdot\mathcal F\boldsymbol\xi\,dV$ is real. Multiplying the [normal mode](wave-equation.md#normal-mode) equation by the [complex conjugate](complex-analysis.md#complex-conjugate) of the [displacement](classical-mechanics.md#displacement) and integrating gives $\omega^2\int\rho|\boldsymbol\xi|^2dV=2\delta W$. Hence squared frequencies are real, and a negative restoring form gives an unstable mode through the variational [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient), subject to the operator domain and spectral hypotheses. Background [fluid flow](fluid-mechanics.md#fluid-flow) adds terms to this argument; the static hypothesis is essential.

##### Incompressible magnetic displacement energy identity

↑ **Parent:** [Magnetohydrodynamic energy principle](#magnetohydrodynamic-energy-principle)

For a static [ideal magnetohydrodynamics](#ideal-magnetohydrodynamics) equilibrium in fixed gravity, let $\nabla\cdot\xi=0$ and $\Pi=p+B^2/(2\mu_0)$. Frozen flux gives $b=(B\cdot\nabla)\xi-(\xi\cdot\nabla)B$ and continuity gives $\rho'=-\xi\cdot\nabla\rho$. Multiplying the linear momentum equation by the conjugate displacement and integrating by parts gives the displayed identity when surface terms vanish. The two magnetic cross terms cancel; the remaining magnetic equilibrium derivative combines with the [mass density](fluid-mechanics.md#density)-gradient force to give the two [Hessian matrices](calculus.md#hessian-matrix). Real symmetric [Hessian matrices](calculus.md#hessian-matrix) and the nonnegative [magnetic tension](#magnetic-tension) term make $\sigma^2$ real.

###### Interchange stability of an incompressible magnetized atmosphere

↑ **Parent:** [Incompressible magnetic displacement energy identity](#incompressible-magnetic-displacement-energy-identity)

For a horizontal field $B(z)e_x$ in constant downward gravity, equilibrium obeys $(p+B^2/(2\mu_0))_z=-\rho g$. The displacement energy reduces to the displayed [quadratic form](linear-algebra.md#quadratic-form). Perturbations independent of the field direction do not bend [magnetic field lines](electromagnetism.md#magnetic-field-line) and therefore have no [magnetic tension](#magnetic-tension) penalty: an increasing [mass density](fluid-mechanics.md#density) with height permits instability. A nonincreasing [mass density](fluid-mechanics.md#density) gives nonnegative energy for all admitted incompressible perturbations. Along-field variation adds [magnetic tension](#magnetic-tension) proportional to [wavenumber](wave-equation.md#wavenumber) squared, stabilizing sufficiently short waves when buoyancy is unfavorable.

##### Linear displacement equations for a magnetized atmosphere

↑ **Parent:** [Magnetohydrodynamic energy principle](#magnetohydrodynamic-energy-principle)

For a static equilibrium and a [fluid Lagrangian displacement](fluid-mechanics.md#lagrangian-displacement-fluid-mechanics) $\xi$, [conservation of mass](continuum-mechanics.md#mass-conservation), adiabatic [entropy](thermodynamics.md#entropy) and [magnetic flux freezing](#magnetic-flux-freezing) give $\delta p=-\xi\cdot\nabla p-\gamma p\nabla\cdot\xi$ together with the displayed relations. Linearizing the [pressure](thermodynamics.md#pressure)/tension form of the momentum equation yields $\rho\ddot\xi=-\nabla\delta\Pi-g\delta\rho e_z+\mu_0^{-1}(\delta B\cdot\nabla B+B\cdot\nabla\delta B)$, where $\delta\Pi=\delta p+B\cdot\delta B/\mu_0$. Static force balance removes the zeroth-order terms; the [density](fluid-mechanics.md#density) multiplying acceleration is the equilibrium [density](fluid-mechanics.md#density).

<h4 id="elsasser-variable">Elsässer variable</h4>

↑ **Parent:** [Ideal magnetohydrodynamics](#ideal-magnetohydrodynamics)

For an [incompressible flow](fluid-mechanics.md#incompressible-flow) with constant [mass density](fluid-mechanics.md#density), the [Elsässer variables](#elsasser-variable) are $\mathbf z^\pm=\mathbf u\pm\mathbf v_a$, where $\mathbf v_a$ is the [Alfvén velocity](#alfven-velocity). Adding and subtracting the [Euler momentum equation](fluid-mechanics.md#euler-equations-for-an-inviscid-fluid) and [ideal magnetohydrodynamic induction equation](#ideal-magnetohydrodynamic-induction-equation) yields $\partial_t\mathbf z^\pm+(\mathbf z^\mp\cdot\nabla)\mathbf z^\pm=-\nabla\psi$, with $\psi=p/\rho+\Phi+|\mathbf v_a|^2/2$ and $\nabla\cdot\mathbf z^\pm=0$. Thus each field is transported by the other, a useful way to expose interactions of oppositely directed [Alfvén waves](#alfven-wave).

<h5 id="elsasser-energy-invariant">Elsässer energy invariant</h5>

↑ **Parent:** [Elsässer variable](#elsasser-variable)

For smooth [ideal magnetohydrodynamics](#ideal-magnetohydrodynamics) of constant [mass density](fluid-mechanics.md#density), define $I_\pm=\int_V|\mathbf z^\pm|^2dV$. Taking the [dot product](linear-algebra.md#dot-product) of the [Elsässer variable](#elsasser-variable) equation with $2\mathbf z^\pm$ gives

$$
\partial_t|\mathbf z^\pm|^2+\nabla\cdot\left(|\mathbf z^\pm|^2\mathbf z^\mp+2\psi\mathbf z^\pm\right)=0.
$$

Therefore each integral is constant when its outward boundary flux vanishes, for example when both [velocity](classical-mechanics.md#velocity) and [magnetic field](electromagnetism.md#magnetic-field) are tangent to the fixed boundary, or for [periodic boundary conditions](differential-equation.md#periodic-boundary-conditions). The [kinetic energy](classical-mechanics.md#kinetic-energy) plus [magnetic energy](electromagnetism.md#magnetic-energy) is $\rho(I_++I_-)/4$, while the [cross-helicity](#cross-helicity) is $\sqrt{\mu_0\rho}(I_+-I_-)/4$.

#### Cross-helicity

↑ **Parent:** [Ideal magnetohydrodynamics](#ideal-magnetohydrodynamics)

Cross-helicity measures alignment between velocity and magnetic field in a magnetized fluid. Its density is $h_c=\mathbf u\mathbin\cdot\mathbf B$.

##### Cross-helicity conservation law

↑ **Parent:** [Cross-helicity](#cross-helicity)

Let $h_c=\mathbf u\mathbin\cdot\mathbf B$ be the [cross-helicity](#cross-helicity) density. The [ideal magnetohydrodynamic induction equation](#ideal-magnetohydrodynamic-induction-equation) implies $D\mathbf B/Dt=(\mathbf B\mathbin\cdot\nabla)\mathbf u-\mathbf B\nabla\mathbin\cdot\mathbf u$. Dotting the momentum equation with $\mathbf B$ eliminates the [Lorentz force density](electromagnetism.md#lorentz-force-density), since it is perpendicular to the [magnetic field](electromagnetism.md#magnetic-field). The [material derivative](continuum-mechanics.md#material-derivative) of $h_c$ is therefore

$$
\frac{Dh_c}{Dt}
=\mathbf B\mathbin\cdot\nabla\left(\frac{u^2}{2}-\Phi\right)
-\frac{\mathbf B\mathbin\cdot\nabla p}{\rho}
-h_c\nabla\mathbin\cdot\mathbf u.
$$

Using $dh=T\,ds+dp/\rho$ for [specific enthalpy](thermodynamics.md#specific-enthalpy) $h$ and [specific entropy](thermodynamics.md#specific-entropy) $s$, together with [Gauss's law for magnetism](electromagnetism.md#gauss-s-law-for-magnetism), converts this to

$$
\partial_th_c+\nabla\mathbin\cdot\left[
\mathbf u h_c+\mathbf B\left(h+\Phi-\frac{u^2}{2}\right)
\right]
=T\mathbf B\mathbin\cdot\nabla s.
$$

The source vanishes when [magnetic field lines](electromagnetism.md#magnetic-field-line) lie in constant-[specific entropy](thermodynamics.md#specific-entropy) surfaces, in particular in a [homentropic flow](compressible-flow.md#homentropic-flow). Integrating over a volume conserves its total [cross-helicity](#cross-helicity) only if the boundary flux also vanishes. This local law is derived in [Ogilvie's astrophysical fluid dynamics notes](https://arxiv.org/abs/1604.03835).

###### Material conservation of cross-helicity density

↑ **Parent:** [Cross-helicity conservation law](#cross-helicity-conservation-law)

In a [homentropic flow](compressible-flow.md#homentropic-flow), the [cross-helicity conservation law](#cross-helicity-conservation-law) gives

$$
\frac{Dh_c}{Dt}
=\mathbf B\mathbin\cdot\nabla\left(\frac{u^2}{2}-h-\Phi\right)
-h_c\nabla\mathbin\cdot\mathbf u.
$$

Consequently [cross-helicity](#cross-helicity) density is conserved along each trajectory exactly when the right-hand side vanishes. In a [steady state](dynamical-systems.md#steady-state), [mass conservation](continuum-mechanics.md#mass-conservation) gives $\nabla\mathbin\cdot\mathbf u=-\mathbf u\mathbin\cdot\nabla\log\rho$, so the criterion becomes

$$
\mathbf B\mathbin\cdot\nabla\left(h+\Phi-\frac{u^2}{2}\right)
=(\mathbf u\mathbin\cdot\mathbf B)\mathbf u\mathbin\cdot\nabla\log\rho.
$$

The absence of an [entropy](thermodynamics.md#entropy) source in a conservation law does not alone make its density an advected scalar: compression and transport along the [magnetic field](electromagnetism.md#magnetic-field) still change that density.

#### Magnetic flux freezing

↑ **Parent:** [Ideal magnetohydrodynamics](#ideal-magnetohydrodynamics)

Magnetic flux freezing states that every material loop in an ideal conducting fluid encloses constant magnetic flux. A deformation perpendicular to a uniform field that preserves mass per unit length therefore preserves $B/\rho$.

##### Flux-surface preservation during magnetic-tube expansion

↑ **Parent:** [Magnetic flux freezing](#magnetic-flux-freezing)

Suppose the [Cartesian magnetic flux function](#cartesian-magnetic-flux-function) is advected, the initial axial velocity is zero, $B_y=f(\psi)$ initially, and $\nabla\cdot\mathbf u=g(\psi,t)$. Then $B_y=f(\psi)\exp[-\int_0^t g(\psi,s)\,ds]$ remains a function of the flux label and time. The axial [Lorentz force](electromagnetism.md#lorentz-force) vanishes because its transverse derivative along a [magnetic field line](electromagnetism.md#magnetic-field-line) vanishes. Smooth ideal evolution therefore preserves zero axial motion.

##### Mass-to-flux ratio

↑ **Parent:** [Magnetic flux freezing](#magnetic-flux-freezing)

The mass-to-flux ratio is the matter carried per unit magnetic flux by a bundle of field lines. Ideal magnetohydrodynamics preserves it for a material flux tube.

###### Critical mass-to-flux ratio

↑ **Parent:** [Mass-to-flux ratio](#mass-to-flux-ratio)

For fixed cloud shape, gravitational energy scales as $-C_gGM^2/L$ and [magnetic energy](electromagnetism.md#magnetic-energy) as $C_B\Phi^2/(\mu_0L)$. The magnetic-criticality threshold for negligible [pressure](thermodynamics.md#pressure) is $M/\Phi>\sqrt{C_B/C_g}/\sqrt{\mu_0G}$. Ideal flux freezing keeps this ratio fixed during homologous collapse; geometry determines the numerical coefficient.

<h4 id="alfven-speed">Alfvén speed</h4>

↑ **Parent:** [Ideal magnetohydrodynamics](#ideal-magnetohydrodynamics)

The Alfvén speed associated with magnetic-field magnitude $B$ and density $\rho$ is $v_A=B/\sqrt{\mu_0\rho}$.

<h5 id="alfven-mach-number">Alfvén Mach number</h5>

↑ **Parent:** [Alfvén speed](#alfven-speed)

The Alfvén Mach number compares a characteristic flow speed with the [Alfvén speed](#alfven-speed) $v_A=B/\sqrt{\mu_0\rho}$. In an [axisymmetric magnetohydrodynamic wind](#axisymmetric-magnetohydrodynamic-wind), the relevant poloidal quantity is $M_{Ap}=|\mathbf u_p|\sqrt{\mu_0\rho}/|\mathbf B_p|$. With [magnetohydrodynamic mass loading](#magnetohydrodynamic-mass-loading) $\rho\mathbf u_p=\kappa\mathbf B_p$, its square is $\mu_0\kappa^2/\rho$. The [Alfvén surface](#alfven-surface) is the locus $M_{Ap}=1$, and a smooth crossing requires the corresponding [Alfvén-surface regularity condition for an axisymmetric wind](#alfven-surface-regularity-condition-for-an-axisymmetric-wind). The total-speed and poloidal-speed definitions should be distinguished when there is substantial rotation or a strong [toroidal magnetic field](#toroidal-magnetic-field).

<h5 id="alfven-velocity">Alfvén velocity</h5>

↑ **Parent:** [Alfvén speed](#alfven-speed)

The [Alfvén velocity](#alfven-velocity) is the signed vector $\mathbf v_a=\mathbf B/\sqrt{\mu_0\rho}$, whose magnitude is the [Alfvén speed](#alfven-speed). It follows the orientation of the [magnetic field](electromagnetism.md#magnetic-field), unlike the nonnegative scalar [speed](classical-mechanics.md#speed).

<h5 id="alfven-number">Alfvén number</h5>

↑ **Parent:** [Alfvén speed](#alfven-speed)

An Alfvén number is the ratio of a flow speed to the corresponding Alfvén speed. For a poloidal flow parallel to a poloidal magnetic field, $A^2=\mu_0\rho u_p^2/B_p^2$.

#### Magnetohydrodynamic wave

↑ **Parent:** [Ideal magnetohydrodynamics](#ideal-magnetohydrodynamics)

A magnetohydrodynamic wave is a linear disturbance of a conducting fluid and its magnetic field. A uniform ideal plasma supports an Alfvén mode and fast and slow magnetosonic modes.

##### Ambipolar damping

↑ **Parent:** [Magnetohydrodynamic wave](#magnetohydrodynamic-wave)

[Ambipolar damping](#ambipolar-damping) is attenuation of magnetic disturbances by friction between the magnetically coupled charged fluid and a neutral fluid. In a strongly collisional mixture, the fluids nearly move together, but their small relative [velocity](classical-mechanics.md#velocity) dissipates [energy](classical-mechanics.md#energy). With drag coefficient $\rho_i\mu_{in}=\rho_n\mu_{ni}$, the frictional [energy](classical-mechanics.md#energy) loss is $-\rho_i\mu_{in}\int|\mathbf u_i-\mathbf u_n|^2dV$. Neglecting other dissipative processes does not remove this collisional loss.

<h6 id="equal-density-ion-neutral-alfven-dispersion-relation">Equal-density ion-neutral Alfvén dispersion relation</h6>

↑ **Parent:** [Ambipolar damping](#ambipolar-damping)

For equal [ion](chemistry.md#ion) and neutral mass densities, let $\mu=\mu_{in}=\mu_{ni}$, $a=k_\parallel B_0/\sqrt{4\pi\rho_i}$ and use Fourier time dependence $e^{-i\omega t}$. [Solenoidal](calculus.md#solenoidal-vector-field) [displacements](classical-mechanics.md#displacement) obey $\ddot\xi_i=-a^2\xi_i-\mu(\dot\xi_i-\dot\xi_n)$ and $\ddot\xi_n=-\mu(\dot\xi_n-\dot\xi_i)$. For nonzero [frequency](physics.md#frequency), the neutral equation gives $\xi_i=(1-i\omega/\mu)\xi_n$. Substitution in the [ion](chemistry.md#ion) equation gives

$$
\omega^3+2i\mu\omega^2-a^2\omega-i\mu a^2=0.
$$

Equivalently, the [growth rate](wave-equation.md#growth-rate) $s=-i\omega$ obeys $s^3+2\mu s^2+a^2s+\mu a^2=0$. A time-independent neutral [displacement](classical-mechanics.md#displacement) with zero [velocity](classical-mechanics.md#velocity) is a relabeling of a uniform fluid, not an additional [wave](physics.md#wave) root of the [velocity](classical-mechanics.md#velocity)/magnetic-field system.

<h6 id="strong-collision-ion-neutral-alfven-modes">Strong-collision ion-neutral Alfvén modes</h6>

↑ **Parent:** [Equal-density ion-neutral Alfvén dispersion relation](#equal-density-ion-neutral-alfven-dispersion-relation)

For $|a|\ll\mu$, the equal-density ion-neutral cubic has a rapidly damped mode $\omega_d=-2i\mu+ia^2/(4\mu)+O(a^4/\mu^3)$ and two propagating modes $\omega_\pm=\pm a/\sqrt2-ia^2/(8\mu)+O(a^3/\mu^2)$. The reduced [phase speed](wave-equation.md#phase-speed) uses the total [density](fluid-mechanics.md#density) $\rho_i+\rho_n=2\rho_i$. The exact [displacement](classical-mechanics.md#displacement) ratio is $\xi_n/\xi_i=\mu/(\mu-i\omega)$. It is nearly $-1$ for the rapidly damped counterflow and nearly $1\pm ia/(\sqrt2\mu)$ for the propagating modes. Thus the latter have small ion-neutral slippage of relative size $|a|/\mu$, responsible for [ambipolar damping](#ambipolar-damping).

##### Entropy mode

↑ **Parent:** [Magnetohydrodynamic wave](#magnetohydrodynamic-wave)

An [entropy mode](#entropy-mode) is a perturbation of [entropy](thermodynamics.md#entropy) and [density](fluid-mechanics.md#density) with no leading [pressure](thermodynamics.md#pressure) or [velocity](classical-mechanics.md#velocity) perturbation in a uniform ideal fluid. For an [adiabatic equation of state](thermodynamics.md#adiabatic-equation-of-state) define $s=\delta p/p_0-\gamma\delta\rho/\rho_0$. An [entropy](thermodynamics.md#entropy) perturbation can have $\delta p=0$ and $\delta\rho/\rho_0=-s/\gamma$, so it has zero [frequency](physics.md#frequency) in the local fluid frame. In anisotropic [reduced magnetohydrodynamics](#reduced-magnetohydrodynamics), $Ds=0$ with $D=\partial_t+\mathbf u_\perp\cdot\nabla_\perp$, and [turbulence](turbulence.md) mixes its [variance](variance.md) as a [passive scalar](fluid-mechanics.md#passive-scalar).

##### Magnetohydrodynamic wave polarization

↑ **Parent:** [Magnetohydrodynamic wave](#magnetohydrodynamic-wave)

A polarization specifies the direction or trajectory of the oscillating [velocity](classical-mechanics.md#velocity) and [magnetic field](electromagnetism.md#magnetic-field) in a [magnetohydrodynamic wave](#magnetohydrodynamic-wave). The linear [Alfvén wave](#alfven-wave) has velocity perpendicular to the plane of the background [magnetic field](electromagnetism.md#magnetic-field) and [wavevector](continuum-mechanics.md#wavevector); the [magnetosonic waves](#magnetosonic-wave) have velocity in that plane. A real fixed polarization vector gives a linear oscillation. Two orthogonal components of equal amplitude in quadrature give a circular trajectory. For propagation parallel to a uniform field, combining the two degenerate transverse linear polarizations produces circular polarization; at finite amplitude its constant transverse magnetic-field magnitude removes the longitudinal [magnetic pressure](#magnetic-pressure) gradient.

##### Uniform-current rotating magnetohydrodynamic wave dispersion

↑ **Parent:** [Magnetohydrodynamic wave](#magnetohydrodynamic-wave)

For an ideal [incompressible flow](fluid-mechanics.md#incompressible-flow) rotating about the axis of the field $\mathbf B=(J/2)s\widehat{\boldsymbol\phi}$, use cylindrical [Fourier modes](fourier-analysis.md#fourier-mode) $e^{\sigma t+im\phi}$. The [azimuthal derivative of a cylindrical vector Fourier mode](calculus.md#azimuthal-derivative-of-a-cylindrical-vector-fourier-mode) reduces induction to $\sigma\mathbf b=imJ\mathbf u/2$. If the boundary eigenproblem gives $\lambda=i\delta\nu$, with real $|\delta|<1$, eliminating the perturbation gives the displayed [dispersion relation](wave-equation.md#dispersion-relation). Here $J=\nabla\times\mathbf B\cdot\widehat{\mathbf z}=\mu_0J_{\rm phys}$ for SI [current density](electromagnetism.md#current-density); the formula is conditional on that boundary eigenrelation.

###### Single-azimuthal-mode current-driven instability threshold

↑ **Parent:** [Uniform-current rotating magnetohydrodynamic wave dispersion](#uniform-current-rotating-magnetohydrodynamic-wave-dispersion)

In the [uniform-current rotating magnetohydrodynamic wave dispersion](#uniform-current-rotating-magnetohydrodynamic-wave-dispersion), exponential growth requires $J^2(2m\delta-m^2)/(4\mu_0\rho)>\delta^2\Omega^2$. For integer $m$ and $|\delta|<1$ this is possible only for $|m|=1$ and $m\delta>1/2$. Positive and negative $m$ branches are related by [complex conjugation](complex-analysis.md#complex-conjugation). The equality case is a repeated frequency and requires separate analysis of possible algebraic growth.

<h5 id="alfven-wave">Alfvén wave</h5>

↑ **Parent:** [Magnetohydrodynamic wave](#magnetohydrodynamic-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Alfvén_wave)

An Alfvén wave is transverse and incompressible, with displacement perpendicular to both the background magnetic field and the wavevector. Its frequency is $\omega^2=(\mathbf k\mathbin\cdot\mathbf v_A)^2$.

<h6 id="alfven-resonant-vorticity-in-a-parallel-magnetic-shear-flow">Alfvén-resonant vorticity in a parallel magnetic shear flow</h6>

↑ **Parent:** [Alfvén wave](#alfven-wave)

For an incompressible [shear flow](fluid-mechanics.md#shear-flow) $U(z)\mathbf e_x$ with uniform [magnetic field](electromagnetism.md#magnetic-field) $B\mathbf e_x$, define $S=\sigma+k_xU$ for time dependence $e^{i\sigma t}$ and $\zeta=ik_xv-ik_yu$. Eliminating the magnetic perturbations from the horizontal [momentum](classical-mechanics.md#momentum) equations gives the displayed product for $S\ne0$. Away from the [Alfvén wave](#alfven-wave) resonance, it yields $\zeta=k_yU'w/S$. At resonance one must retain the original system: for constant $U$, $k_y=0$, $S^2=k_x^2B^2/\rho$, any smooth transverse amplitude $v(z)$ with $b_y=k_xBv/S$ and all other amplitudes zero is an [Alfvén wave](#alfven-wave). Its nonzero [vorticity](fluid-mechanics.md#vorticity) disproves the unrestricted zero-vorticity reduction. Exponentially growing modes with real background coefficients cannot encounter these real-frequency resonances.

<h6 id="kinetic-alfven-wave">Kinetic Alfvén wave</h6>

↑ **Parent:** [Alfvén wave](#alfven-wave)

A kinetic Alfvén wave is a dispersive extension of the [Alfvén wave](#alfven-wave) in a [plasma](physics.md#plasma-physics) when perpendicular kinetic or two-fluid effects, including a pressure response, matter. Its particular [dispersion relation](wave-equation.md#dispersion-relation) depends on the ordering and plasma parameters. A similar product of parallel and perpendicular wavenumbers can occur in a [whistler wave](#whistler-wave), but agreement of a scaling power does not identify the underlying physical equations.

###### Magnetohydrodynamic phase mixing

↑ **Parent:** [Alfvén wave](#alfven-wave)

Neighboring magnetic surfaces with different [Alfvén speeds](#alfven-speed) carry the same axial waveform at different rates. For a traveling profile $f(R,z+v(R)t)$, differentiation produces the displayed term, so transverse gradients grow even without axial wave steepening. Small [magnetic diffusivity](#magnetic-diffusivity) or [viscosity](fluid-mechanics.md#dynamic-viscosity) can eventually act strongly on these gradients. The ideal process redistributes phase rather than directly dissipating wave energy.

<h6 id="torsional-alfven-wave">Torsional Alfvén wave</h6>

↑ **Parent:** [Alfvén wave](#alfven-wave)

A torsional [Alfvén wave](#alfven-wave) couples azimuthal [velocity](classical-mechanics.md#velocity) to a [toroidal magnetic field](#toroidal-magnetic-field) around a fixed [poloidal magnetic field](#poloidal-magnetic-field). Axisymmetric induction gives $\partial_tB_\phi=R\mathbf B_p\cdot\nabla\Omega$ and magnetic tension gives $\rho R^2\mu_0\partial_t\Omega=\mathbf B_p\cdot\nabla(RB_\phi)$. Their combination is the displayed wave equation. Its local [dispersion relation](wave-equation.md#dispersion-relation) is $\omega^2=(\mathbf k\cdot\mathbf B_p)^2/(\mu_0\rho)$.

<h6 id="pressure-compatibility-of-nonlinear-torsional-alfven-profiles">Pressure compatibility of nonlinear torsional Alfvén profiles</h6>

↑ **Parent:** [Torsional Alfvén wave](#torsional-alfven-wave)

For uniform-density [incompressible flow](fluid-mechanics.md#incompressible-flow) with $u_\phi=f(R,z+vt)+g(R,z-vt)$, $B_\phi/\sqrt{\mu_0\rho}=f-g$ and $B_z/\sqrt{\mu_0\rho}=v(R)$, the azimuthal [magnetohydrodynamic momentum equation](#magnetohydrodynamic-momentum-equation) and [ideal magnetohydrodynamic induction equation](#ideal-magnetohydrodynamic-induction-equation) hold automatically. Let $\Pi=p/\rho+\Phi+[(f-g)^2+v^2]/2$. The remaining equations require $\Pi_z=0$ and $\Pi_R=4fg/R$, so $\partial_z(fg)=0$ is necessary and locally sufficient. A single traveling profile is unrestricted; two nonzero profiles on an unrestricted axial domain must be opposite exponentials or independent of their traveling arguments. Bounded profiles of both signs therefore reduce to steady solutions.

<h6 id="cylinder-averaged-torsional-alfven-wave">Cylinder-averaged torsional Alfvén wave</h6>

↑ **Parent:** [Torsional Alfvén wave](#torsional-alfven-wave)

For a rotating conducting sphere, a geostrophic azimuthal [velocity](classical-mechanics.md#velocity) $U=rV$ couples to the cylinder-integrated magnetic stress $T=\int B_rB_\phi\,dz$. Put $H=\int B_r^2\,dz$ and let $2z_b$ be the cylinder height. With an insulating boundary and no flow through it, cylindrical averaging removes the [Coriolis force](physics.md#coriolis-force) and gives $U_t=(2z_b\mu_0\rho r^2)^{-1}\partial_r(r^2T)$, $T_t=Hr\partial_r(U/r)$. The local squared wave speed is $H/(2z_b\mu_0\rho)$, the cylinder average of $B_r^2/(\mu_0\rho)$.

###### Conserved energy of a cylinder-averaged torsional wave

↑ **Parent:** [Cylinder-averaged torsional Alfvén wave](#cylinder-averaged-torsional-alfven-wave)

For a [cylinder-averaged torsional Alfvén wave](#cylinder-averaged-torsional-alfven-wave) with time-independent $H>0$, differentiating this quadratic form gives $dE/dt=[rUT]_0^a$. Regularity at the axis and vanishing magnetic torque at the outer endpoint therefore imply conservation. By [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality), $T^2/H\leq\int B_\phi^2\,dz$; equality holds for the torsional-wave magnetic component proportional to $B_r$ along each cylinder. A stationary magnetic component orthogonal to $B_r$ is invisible to $T$.

###### Magnetic axial angular momentum flux

↑ **Parent:** [Torsional Alfvén wave](#torsional-alfven-wave)

The [magnetic tension](#magnetic-tension) stress transports axial [angular momentum](classical-mechanics.md#angular-momentum) along a [poloidal magnetic field](#poloidal-magnetic-field). In purely azimuthal ideal flow the poloidal energy flux is $\mathbf F_{E,p}=\Omega\mathbf F_{J,p}$. This proportionality is valid even at vanishing flux, where an ordinary ratio is undefined. The coupled fluxes explain how a [torsional Alfvén wave](#torsional-alfven-wave) redistributes rotation.

<h6 id="nonlinear-alfven-wave">Nonlinear Alfvén wave</h6>

↑ **Parent:** [Alfvén wave](#alfven-wave)

A finite-amplitude ideal-MHD Alfvén wave can rotate the transverse [magnetic field](electromagnetism.md#magnetic-field) at constant magnitude, with constant [mass density](fluid-mechanics.md#density), [pressure](thermodynamics.md#pressure) and longitudinal components. Its transverse velocity obeys $\mathbf u_\perp=\mathbf C-s\mathbf B_\perp/\sqrt{\mu_0\rho}$ and its speed is constant along the wave. The constant [magnetic pressure](#magnetic-pressure) prevents compressive acceleration.

<h6 id="magnetic-pressure-obstruction-to-a-linearly-polarized-alfven-wave">Magnetic-pressure obstruction to a linearly polarized Alfvén wave</h6>

↑ **Parent:** [Nonlinear Alfvén wave](#nonlinear-alfven-wave)

A finite sinusoidal transverse field $B_x=aB_0\cos[k(z-v_at)]$, $B_y=0$, has varying [magnetic pressure](#magnetic-pressure). In a purely transverse traveling [Alfvén wave](#alfven-wave), longitudinal momentum requires $\partial_z[p+B_x^2/(2\mu_0)]=0$, but the adiabatic [pressure](thermodynamics.md#pressure) equation with $u_z=0$ requires $\partial_t p=0$. A traveling compensating gas [pressure](thermodynamics.md#pressure) cannot satisfy both conditions. The uncompensated force is quadratic in amplitude and drives a compressive response. A regular periodic one-dimensional traveling solution cannot evade this by varying [mass density](fluid-mechanics.md#density): its mass, transverse momentum and induction integrals force constant [mass density](fluid-mechanics.md#density) at the zeros of the transverse field and hence throughout the nontrivial wave.

<h6 id="circularly-polarized-nonlinear-alfven-wave">Circularly polarized nonlinear Alfvén wave</h6>

↑ **Parent:** [Nonlinear Alfvén wave](#nonlinear-alfven-wave)

In homogeneous [ideal magnetohydrodynamics](#ideal-magnetohydrodynamics), a constant longitudinal field $B_0>0$ and transverse field $aB_0(\cos\zeta,\sin\zeta)$, $\zeta=k(z-v_at)$, give an exact traveling wave with constant [mass density](fluid-mechanics.md#density) and [pressure](thermodynamics.md#pressure), $u_z=0$, $v_a=B_0/\sqrt{\mu_0\rho_0}$ and the displayed transverse [velocity](classical-mechanics.md#velocity). Induction and transverse momentum reduce to the same wave relation. Since $|\mathbf B_\perp|^2=a^2B_0^2$ is constant, there is no longitudinal [magnetic pressure](#magnetic-pressure) [gradient](calculus.md#gradient). All nonlinear terms are compatible with the constant-density solution, even in a compressible fluid.

<h6 id="alfven-characteristic-eigenvector">Alfvén characteristic eigenvector</h6>

↑ **Parent:** [Alfvén wave](#alfven-wave)

For propagation along $x$, the Alfvén right [eigenvector](linear-operator-theory.md#eigenvector) has $\delta\rho=\delta p=\delta u_x=\delta B_x=0$, $\mathbf B_\perp\cdot\delta\mathbf u_\perp=0$ and $\delta\mathbf B_\perp=-s\sqrt{\mu_0\rho}\,\delta\mathbf u_\perp$. Its speed is $u_x+sB_x/\sqrt{\mu_0\rho}$, $s=\pm1$. When the transverse background field vanishes, both transverse polarizations are allowed.

<h6 id="alfven-frequency">Alfvén frequency</h6>

↑ **Parent:** [Alfvén wave](#alfven-wave)

The Alfvén frequency is the frequency of an [Alfvén wave](#alfven-wave) with [wavevector](continuum-mechanics.md#wavevector) $\mathbf k$ in a uniform [magnetic field](electromagnetism.md#magnetic-field) $\mathbf B$ and [mass density](fluid-mechanics.md#density) $\rho$. For a vertical field and vertical [wavenumber](wave-equation.md#wavenumber) $k$, its square is $\omega_a^2=k^2B_z^2/(\mu_0\rho)$. Its competition with orbital shear determines the [ideal magnetorotational dispersion relation](astrophysics.md#ideal-magnetorotational-dispersion-relation).

<h6 id="alfven-wing">Alfvén wing</h6>

↑ **Parent:** [Alfvén wave](#alfven-wave)

An Alfvén wing is a stationary Alfvénic disturbance attached to a conducting obstacle moving through a magnetized plasma. In a super-Alfvénic flow its boundaries follow downstream characteristics.

<h6 id="alfvenic-mach-cone-slope">Alfvénic Mach-cone slope</h6>

↑ **Parent:** [Alfvén wing](#alfven-wing)

For a stationary cold-plasma disturbance with obstacle speed $u_0>u_A$, the characteristic slope is $m=\sqrt{u_0^2/u_A^2-1}$. It approaches $u_0/u_A$ in the strongly super-Alfvénic limit.

##### Magnetosonic wave

↑ **Parent:** [Magnetohydrodynamic wave](#magnetohydrodynamic-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Magnetosonic_wave)

A magnetosonic wave is a compressive MHD mode polarized in the plane of the wavevector and background magnetic field.

###### High-pressure limit of magnetosonic waves

↑ **Parent:** [Magnetosonic wave](#magnetosonic-wave)

For [sound speed](compressible-flow.md#speed-of-sound) $v_s$ much larger than [Alfvén speed](#alfven-speed) $v_a$, and angle $\theta$ between the [wavevector](continuum-mechanics.md#wavevector) and [magnetic field](electromagnetism.md#magnetic-field), the [fast magnetosonic wave](#fast-magnetosonic-wave) has $v_f^2=v_s^2+v_a^2\sin^2\theta+O(v_a^4/v_s^2)$. The [slow magnetosonic wave](#slow-magnetosonic-wave) has $v_{\rm slow}^2=v_a^2\cos^2\theta[1-(v_a^2/v_s^2)\sin^2\theta+O(v_a^4/v_s^4)]$. The fast mode is predominantly longitudinal sound. The slow mode becomes almost incompressible, polarized in the plane of the [wavevector](continuum-mechanics.md#wavevector) and [magnetic field](electromagnetism.md#magnetic-field); the [Alfvén wave](#alfven-wave) is polarized perpendicular to that plane. The latter two are predominantly magnetic-tension waves with equal leading [phase speeds](wave-equation.md#phase-speed).

<h6 id="pseudo-alfven-wave">Pseudo-Alfvén wave</h6>

↑ **Parent:** [High-pressure limit of magnetosonic waves](#high-pressure-limit-of-magnetosonic-waves)

The high-[pressure](thermodynamics.md#pressure) limit of the [slow magnetosonic wave](#slow-magnetosonic-wave) approaches an incompressible polarization in the plane of the background [magnetic field](electromagnetism.md#magnetic-field) and [wavevector](continuum-mechanics.md#wavevector), perpendicular to the latter. It has the displayed leading [dispersion relation](wave-equation.md#dispersion-relation), the same as the out-of-plane [Alfvén wave](#alfven-wave). [Magnetic tension](#magnetic-tension) is the restoring force, and [pressure](thermodynamics.md#pressure) balances the compressive component of the magnetic force. In exactly incompressible homogeneous [ideal magnetohydrodynamics](#ideal-magnetohydrodynamics) it is one of the two transverse magnetic polarizations.

###### Isothermal coplanar magnetohydrodynamic characteristic matrix

↑ **Parent:** [Magnetosonic wave](#magnetosonic-wave)

For one-dimensional flow obeying an [isothermal equation of state](compressible-flow.md#globally-isothermal-equation-of-state) with $u_z=B_z=0$, the primitive variables $(\rho,u_x,u_y,B_y)$ form a four-variable hyperbolic system and $B_x$ is constant. The speeds relative to $u_x$ satisfy $c^4-(c_s^2+v_a^2)c^2+c_s^2v_{ax}^2=0$. These are the fast and slow [magnetosonic waves](#magnetosonic-wave). The independent out-of-plane [Alfvén wave](#alfven-wave) polarization and a freely advected entropy mode are absent from this reduced isothermal system.

###### Magnetosonic critical speed

↑ **Parent:** [Magnetosonic wave](#magnetosonic-wave)

For propagation in a direction with field component $v_{an}$ of the [Alfvén velocity](#alfven-velocity), the squared [fast magnetosonic wave](#fast-magnetosonic-wave) and [slow magnetosonic wave](#slow-magnetosonic-wave) speeds are the roots of $c^4-(c_s^2+v_a^2)c^2+c_s^2v_{an}^2=0$. They are real and nonnegative, and satisfy $c_{\mathrm s}^2\leq v_{an}^2\leq c_{\mathrm f}^2$. A steady acceleration equation can become singular when the flow equals either of these speeds.

###### Regularity at a magnetosonic point

↑ **Parent:** [Magnetosonic critical speed](#magnetosonic-critical-speed)

If a steady wind equation has the form $(w^2-c_{\mathrm f}^2)(w^2-c_{\mathrm s}^2)w'/w=\mathcal N$, a smooth nondegenerate crossing requires $\mathcal N=0$ at the corresponding [magnetosonic critical speed](#magnetosonic-critical-speed). Subsequent differentiation or the full system determines the admissible slope. The numerator condition alone does not prove that a global smooth wind exists.

###### Cold-limit degeneracy of a slow magnetosonic point

↑ **Parent:** [Regularity at a magnetosonic point](#regularity-at-a-magnetosonic-point)

In a strictly cold flow governed by [ideal magnetohydrodynamics](#ideal-magnetohydrodynamics) the [sound speed](compressible-flow.md#speed-of-sound) vanishes, so the [slow magnetosonic wave](#slow-magnetosonic-wave) speed is zero. A nonzero-speed outflow therefore has no ordinary finite interior slow crossing. For the [cold radial magnetohydrodynamic wind integral](#cold-radial-magnetohydrodynamic-wind-integral), $f_y=-\alpha(x-x^{-1})^2/(y-1)^3-\beta/(x^4y^3)<0$ on the sub-Alfvénic branch $y>1$, assuming $\beta>0$. A small retained [specific enthalpy](thermodynamics.md#specific-enthalpy) is needed to locate a finite slow point; the zero-temperature limit can move it to the launch boundary. The usual simultaneous numerator and denominator regularity conditions still apply to nondegenerate critical points.

###### Fast magnetosonic wave

↑ **Parent:** [Magnetosonic wave](#magnetosonic-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fast_magnetosonic_wave)

The fast magnetosonic mode uses gas and magnetic pressure as reinforcing restoring forces and is the faster root of the magnetosonic dispersion relation.

###### Slow magnetosonic wave

↑ **Parent:** [Magnetosonic wave](#magnetosonic-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Slow_magnetosonic_wave)

The slow magnetosonic mode is the lower-frequency compressive root and is guided more strongly along the magnetic field.

###### Tube speed

↑ **Parent:** [Magnetosonic wave](#magnetosonic-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tube_speed)

The tube speed combines sound and Alfvén speeds according to

$$
v_T^2=\frac{v_s^2v_A^2}{v_s^2+v_A^2}.
$$

It is smaller than both constituent speeds.

##### Magnetohydrodynamic interface wave

↑ **Parent:** [Magnetohydrodynamic wave](#magnetohydrodynamic-wave)

An MHD interface wave propagates along a discontinuity and decays away from it. Continuity of normal displacement and total pressure determines its dispersion relation.

###### Magnetic stabilization of an equal-density vortex sheet

↑ **Parent:** [Magnetohydrodynamic interface wave](#magnetohydrodynamic-interface-wave)

For two incompressible streams of equal density with a common tangential [magnetic field](electromagnetism.md#magnetic-field) parallel to their velocities, decaying [normal modes](wave-equation.md#normal-mode) and interface [displacement](classical-mechanics.md#displacement)/total-pressure continuity give $\rho(\sigma+k_xU_1)^2+\rho(\sigma+k_xU_2)^2=2k_x^2B^2$ in units $\mu_0=1$. The displayed [dispersion relation](wave-equation.md#dispersion-relation) follows, with $v_A^2=B^2/\rho$. Thus $|\Delta U|<2v_A$ excludes exponential [Kelvin-Helmholtz instability](fluid-mechanics.md#kelvin-helmholtz-instability); equality is marginal. Above threshold the [growth rate](wave-equation.md#growth-rate) is $|k_x|\sqrt{(\Delta U)^2/4-v_A^2}$. The transverse horizontal [wavenumber](wave-equation.md#wavenumber) affects the decay length through $k=(k_x^2+k_y^2)^{1/2}$ but not this growth threshold. [Magnetic tension](#magnetic-tension) supplies the stabilizing restoring force.

#### Force-free magnetic field

↑ **Parent:** [Ideal magnetohydrodynamics](#ideal-magnetohydrodynamics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Force-free_magnetic_field)

A force-free magnetic field obeys $(\nabla\times\mathbf B)\times\mathbf B=0$, so its electric current is locally parallel to the magnetic field.

##### Magnetic-energy injection by differential boundary rotation

↑ **Parent:** [Force-free magnetic field](#force-free-magnetic-field)

The general ideal magnetic-energy balance has outward-surface contribution $\mu_0^{-1}\oint[(u\cdot B)B-B^2u]\cdot dS$ and volume contribution $-\int u\cdot(J\times B)dV$. The latter vanishes for a [force-free magnetic field](#force-free-magnetic-field). For an axisymmetric boundary rotating tangentially, $u\cdot B=\Omega f(\psi)$ and the directed flux of a thin tube is $2\pi d\psi$. Pair its exit and entry endpoints to obtain the displayed energy injection, counting each boundary endpoint once. Equal endpoint angular [velocities](classical-mechanics.md#velocity) inject no [magnetic energy](electromagnetism.md#magnetic-energy).

##### Force-free parameter

↑ **Parent:** [Force-free magnetic field](#force-free-magnetic-field)

Writing $\nabla\times\mathbf B=(4\pi/c)\alpha\mathbf B$ defines the force-free parameter $\alpha$. Since the divergence of a curl vanishes and $\nabla\mathbin\cdot\mathbf B=0$, it satisfies $\mathbf B\mathbin\cdot\nabla\alpha=0$.

##### Cylindrical force-free magnetic field

↑ **Parent:** [Force-free magnetic field](#force-free-magnetic-field)

A cylindrical force-free magnetic field depends only on cylindrical radius and has current everywhere parallel to its magnetic field. Regularity on the axis often forces its radial component to vanish.

#### Linearized ideal magnetohydrodynamic equations

↑ **Parent:** [Ideal magnetohydrodynamics](#ideal-magnetohydrodynamics)

The linearized ideal magnetohydrodynamic equations retain terms first order in perturbations about a chosen ideal-MHD background. Around a uniform state they describe [Alfvén waves](#alfven-wave) and [magnetosonic waves](#magnetosonic-wave).

##### Displacement equation for a parallel magnetic shear flow

↑ **Parent:** [Linearized ideal magnetohydrodynamic equations](#linearized-ideal-magnetohydrodynamic-equations)

For nonresonant incompressible [normal modes](wave-equation.md#normal-mode) of a uniform-density [shear flow](fluid-mechanics.md#shear-flow) with aligned uniform [magnetic field](electromagnetism.md#magnetic-field), let $S=\sigma+k_xU(z)$, $k^2=k_x^2+k_y^2$ and $f=w/S$. The normal [displacement](classical-mechanics.md#displacement) is $f/i$. The linearized horizontal equations and incompressibility give $ik^2p_1=\rho(Sw'-S'w)=\rho S^2f'$. Substituting the [ideal magnetohydrodynamic induction equation](#ideal-magnetohydrodynamic-induction-equation) into normal [momentum](classical-mechanics.md#momentum) gives the displayed conservative equation. Across a zero-thickness [shear layer](fluid-mechanics.md#shear-layer), continuity of $f$ and of $(\rho S^2-k_x^2B^2)f'$ supplies the interface conditions. They express common normal [displacement](classical-mechanics.md#displacement) and continuous perturbed [magnetohydrodynamic total pressure](#magnetohydrodynamic-total-pressure), avoiding undefined products of distributional shear gradients.

#### Ideal magnetohydrodynamic induction equation

↑ **Parent:** [Ideal magnetohydrodynamics](#ideal-magnetohydrodynamics)

The ideal magnetohydrodynamic induction equation is $\partial_t\mathbf B=\nabla\times(\mathbf u\times\mathbf B)$. Together with $\nabla\mathbin\cdot\mathbf B=0$, it implies magnetic-flux freezing.

##### Ideal magnetic response to a cylindrical cyclonic event

↑ **Parent:** [Ideal magnetohydrodynamic induction equation](#ideal-magnetohydrodynamic-induction-equation)

For an axisymmetric velocity $\mathbf u=(0,rf(r),g(r))$ independent of $z$, write $\mathbf B=B_z\widehat{\mathbf z}+\nabla\times(A\widehat{\mathbf z})$. Ideal induction becomes

$$
(\partial_t+f\partial_\phi)A=0,\qquad(\partial_t+f\partial_\phi)B_z=\frac{g'}r\partial_\phi A.
$$

The first equation expresses [magnetic flux freezing](#magnetic-flux-freezing) of the transverse flux function, while the second is axial stretching $B_rg'$. Starting from a uniform field $B_0\widehat{\mathbf x}$ gives $A(r,\phi,t)=B_0r\sin(\phi-f(r)t)$ and $B_z(r,\phi,t)=B_0t g'(r)\cos(\phi-f(r)t)$. In complex azimuthal-mode notation, $\widehat A=B_0r e^{-ift}$ and $\widehat B_z=iB_0t g'e^{-ift}$, obtained by elementary integrating factors. The transverse field has $B_r=r^{-1}A_\phi$ and $B_\phi=-A_r$, preserving zero [divergence](calculus.md#divergence).

##### Cartesian magnetic flux function

↑ **Parent:** [Ideal magnetohydrodynamic induction equation](#ideal-magnetohydrodynamic-induction-equation)

For a $y$-independent solenoidal [magnetic field](electromagnetism.md#magnetic-field), the transverse components can be written $B_x=-\psi_z$ and $B_z=\psi_x$. Contours of $\psi$ are transverse [magnetic field lines](electromagnetism.md#magnetic-field-line). The independent axial component $B_y$ can twist the [flux tube](electromagnetism.md#flux-tube). Under the [MHD induction equation](#ideal-magnetohydrodynamic-induction-equation), an additive time-dependent gauge can be chosen so that $D\psi/Dt=0$.

###### Magnetic island

↑ **Parent:** [Cartesian magnetic flux function](#cartesian-magnetic-flux-function)

A magnetic island in a planar [magnetic field](electromagnetism.md#magnetic-field) is a region of closed [magnetic field lines](electromagnetism.md#magnetic-field-line) surrounding an extremum of the [Cartesian magnetic flux function](#cartesian-magnetic-flux-function). A surrounding [separatrix](dynamical-systems.md#separatrix) can pass through a saddle of that function and separate the island from other flux regions. In ideal [incompressible flow](fluid-mechanics.md#incompressible-flow), the flux-function value carried by each fluid particle and the area enclosed by each material contour are conserved.

###### Cartesian magnetostatic flux-function equilibrium

↑ **Parent:** [Cartesian magnetic flux function](#cartesian-magnetic-flux-function)

In a $y$-independent [magnetostatic equilibrium](electromagnetism.md#magnetostatic-equilibrium) with no axial pressure or gravitational force, $\nabla\psi\times\nabla B_y=0$. Thus $B_y=b(\psi)$ on a regular connected flux region. The remaining balance is $[\nabla^2\psi+bb']\nabla\psi/\mu_0+\nabla p+\rho\nabla\Phi=0$. Constancy on separate components of a level set does not automatically give one global single-valued $b$.

##### Axisymmetric magnetic winding

↑ **Parent:** [Ideal magnetohydrodynamic induction equation](#ideal-magnetohydrodynamic-induction-equation)

For prescribed axisymmetric [differential rotation](#differential-rotation) $\mathbf u=R\Omega\mathbf e_\phi$, the [ideal magnetohydrodynamic induction equation](#ideal-magnetohydrodynamic-induction-equation) and [Gauss's law for magnetism](electromagnetism.md#gauss-s-law-for-magnetism) give

$$
\partial_t\mathbf B_p=0,\qquad\partial_tB_\phi=R\mathbf B_p\cdot\nabla\Omega.
$$

The poloidal field is unchanged while rotational shear generates a [toroidal magnetic field](#toroidal-magnetic-field). For time-independent $\Omega$, the toroidal component grows linearly until neglected dynamical feedback becomes relevant.

###### Magnetic-pressure equality radius under Keplerian winding

↑ **Parent:** [Axisymmetric magnetic winding](#axisymmetric-magnetic-winding)

For [Keplerian rotation](astrophysics.md#keplerian-disk), initial $B_R\propto R^{-1}$ and thermal pressure $p\propto R^{-2}$, [axisymmetric magnetic winding](#axisymmetric-magnetic-winding) gives $B_\phi=-(3/2)\Omega tB_R$. If the initial [plasma beta](astrophysics.md#plasma-beta) is $\beta_p>1$, the formal equality of [magnetic pressure](#magnetic-pressure) and gas pressure occurs at

$$
R_{\rm eq}^3=\frac{9GMt^2}{4(\beta_p-1)}.
$$

The magnetic-to-thermal pressure ratio decreases with radius, so magnetic pressure dominates inside this radius. In a disk with a finite radial range, an equality radius exists in the disk only when this formal radius lies within that range.

<h6 id="ferraro-s-law-of-isorotation">Ferraro's law of isorotation</h6>

↑ **Parent:** [Axisymmetric magnetic winding](#axisymmetric-magnetic-winding)

A stationary axisymmetric [magnetic field](electromagnetism.md#magnetic-field) in ideal purely rotational flow requires constant angular velocity along the [magnetic field lines](electromagnetism.md#magnetic-field-line) of its [poloidal magnetic field](#poloidal-magnetic-field). Otherwise [axisymmetric magnetic winding](#axisymmetric-magnetic-winding) generates a time-dependent toroidal component.

#### Entropy advection equation

↑ **Parent:** [Ideal magnetohydrodynamics](#ideal-magnetohydrodynamics)

For an adiabatic ideal fluid, entropy is materially conserved away from shocks: $Ds/Dt=0$. For a perfect gas this is equivalent to $Dp/Dt+\gamma p\nabla\mathbin\cdot\mathbf u=0$.

#### Magnetohydrodynamic shock

↑ **Parent:** [Ideal magnetohydrodynamics](#ideal-magnetohydrodynamics)

A magnetohydrodynamic shock is a discontinuity satisfying conservation of mass, momentum, energy, normal magnetic field, and tangential electric field.

##### Perpendicular magnetohydrodynamic shock

↑ **Parent:** [Magnetohydrodynamic shock](#magnetohydrodynamic-shock)

For a planar [magnetohydrodynamic shock](#magnetohydrodynamic-shock) with normal [velocity](classical-mechanics.md#velocity) and tangential [magnetic field](electromagnetism.md#magnetic-field), [mass conservation](continuum-mechanics.md#mass-conservation) gives $\rho u=m$ and the [ideal magnetohydrodynamic induction equation](#ideal-magnetohydrodynamic-induction-equation) gives $uB$ constant across the front. Hence $B/\rho$ is unchanged, expressing [magnetic flux freezing](#magnetic-flux-freezing). Normal [momentum](classical-mechanics.md#momentum) flux is $\rho u^2+p+B^2/(2\mu_0)$, and energy flux per unit mass flux is $u^2/2+\gamma p/[(\gamma-1)\rho]+B^2/(\mu_0\rho)$, apart from a smooth common [gravitational potential](classical-mechanics.md#newtonian-potential-of-a-point-mass). The amplified tangential field contributes both [magnetic pressure](#magnetic-pressure) and [magnetic energy](electromagnetism.md#magnetic-energy) transport.

###### Compression ratio of a perpendicular magnetohydrodynamic shock

↑ **Parent:** [Perpendicular magnetohydrodynamic shock](#perpendicular-magnetohydrodynamic-shock)

Put $c_1^2=\gamma p_1/\rho_1$ and $v_{A1}^2=B_1^2/(\mu_0\rho_1)$. The mass, [momentum](classical-mechanics.md#momentum) and energy jump conditions for a [perpendicular magnetohydrodynamic shock](#perpendicular-magnetohydrodynamic-shock) factor into the unchanged state $x=1$ and

$$
(2-\gamma)v_{A1}^2x^2+[(\gamma-1)u_1^2+2c_1^2+\gamma v_{A1}^2]x-(\gamma+1)u_1^2=0.
$$

For the compressive physical branch $x>1$, positive downstream [pressure](thermodynamics.md#pressure) implies $x<(\gamma+1)/(\gamma-1)$ when $\gamma>1$ and the upstream [sound speed](compressible-flow.md#speed-of-sound) or [Alfvén speed](#alfven-speed) is nonzero. Indeed the polynomial implies

$$
\frac{p_2}{\rho_1}=
\frac{c_1^2[(\gamma+1)x-(\gamma-1)]/\gamma
+(\gamma-1)v_{A1}^2(x-1)^3/2}
{(\gamma+1)-(\gamma-1)x}.
$$

It then gives $u_1^2>c_1^2+v_{A1}^2$: the upstream flow exceeds the perpendicular fast [magnetosonic wave](#magnetosonic-wave) speed. The exactly cold unmagnetized strong-shock limit reaches the upper compression bound.

##### Parallel magnetohydrodynamic shock

↑ **Parent:** [Magnetohydrodynamic shock](#magnetohydrodynamic-shock)

In a planar [magnetohydrodynamic shock](#magnetohydrodynamic-shock) with both [velocity](classical-mechanics.md#velocity) and [magnetic field](electromagnetism.md#magnetic-field) normal to the front, the normal [magnetic field](electromagnetism.md#magnetic-field) is continuous. Its normal [Maxwell stress tensor](electromagnetism.md#maxwell-stress-tensor) contribution is consequently the same on both sides, and the [Poynting vector](electromagnetism.md#poynting-vector) vanishes because $\mathbf u\times\mathbf B=0$. The remaining jump conditions are the ordinary [Rankine-Hugoniot conditions for a perfect gas](compressible-flow.md#rankine-hugoniot-conditions-for-a-perfect-gas). This is the purely parallel branch; an oblique or switch-on shock has additional transverse fields and is not covered by this reduction.

##### Ideal magnetohydrodynamic shock conditions

↑ **Parent:** [Magnetohydrodynamic shock](#magnetohydrodynamic-shock)

The ideal magnetohydrodynamic shock conditions are the Rankine-Hugoniot jump conditions for mass, momentum, energy, and magnetic flux. For a dynamically weak magnetic field, the normal field is continuous while the tangential field is multiplied by the gas compression ratio.

<h5 id="de-hoffmann-teller-frame">de Hoffmann–Teller frame</h5>

↑ **Parent:** [Magnetohydrodynamic shock](#magnetohydrodynamic-shock)

The de Hoffmann-Teller frame is a tangentially boosted shock frame in which the electric field vanishes. Ideal MHD then makes the fluid velocity parallel to the magnetic field on both sides.

##### Rotational discontinuity in magnetohydrodynamics

↑ **Parent:** [Magnetohydrodynamic shock](#magnetohydrodynamic-shock)

A rotational discontinuity changes the tangential direction of the magnetic field and velocity while leaving density, pressure, and normal components continuous. The normal flow is Alfvénic.

#### Axisymmetric magnetostatic Grad-Shafranov system

↑ **Parent:** [Ideal magnetohydrodynamics](#ideal-magnetohydrodynamics)

For an axisymmetric vector potential $\mathbf A=\nabla\alpha\times\nabla\phi+\beta\nabla\phi$, define

$$
L=-r\partial_r(r^{-1}\partial_r)-\partial_z^2.
$$

Magnetostatic azimuthal force balance gives $L\alpha=F(\beta)$. In a barotropic equilibrium the remaining balance integrates to

$$
L\beta=F(\beta)F'(\beta)+r^2\rho G(\beta)
$$

for flux functions $F$ and $G$.

#### Axisymmetric magnetohydrodynamic wind

↑ **Parent:** [Ideal magnetohydrodynamics](#ideal-magnetohydrodynamics)

A steady axisymmetric magnetohydrodynamic wind follows nested magnetic-flux surfaces and has conserved mass loading, field-line angular velocity, angular momentum, entropy, and Bernoulli quantities along each surface.

##### Cold radial magnetohydrodynamic wind integral

↑ **Parent:** [Axisymmetric magnetohydrodynamic wind](#axisymmetric-magnetohydrodynamic-wind)

For a cold equatorial [axisymmetric magnetohydrodynamic wind](#axisymmetric-magnetohydrodynamic-wind) with $B_p=CR^{-2}$ in the gravity of a [point mass](classical-mechanics.md#point-mass) $M$, smooth crossing of the [Alfvén surface](#alfven-surface) gives $\rho_a=\mu_0k^2$ and $\ell=\omega R_a^2$. Put $x=R/R_a$, $y=\rho/\rho_a$, $\alpha=\omega^2R_a^3/(GM)$ and $\beta=C^2/(\mu_0\rho_a GM R_a^3)$. The corotating [energy](classical-mechanics.md#energy), scaled by $GM/R_a$, is

$$
f=\frac\alpha2\left[\frac{(x-x^{-1})^2}{(y-1)^2}-x^2\right]+\frac\beta{2x^4y^2}-\frac1x.
$$

The azimuthal [velocity](classical-mechanics.md#velocity) relative to field-line rotation is $\omega R_a(x-x^{-1})/(y-1)$ and the poloidal speed is $C/(\sqrt{\mu_0\rho_a}R_a^2x^2y)$. The apparent singularity at $x=y=1$ is interpreted through a smooth limiting slope. A nondegenerate magnetosonic crossing on a constant-$f$ curve requires $f_x=f_y=0$ and a real admissible tangent slope.

<h5 id="sub-alfvenic-isorotation-in-a-steady-axisymmetric-wind">Sub-Alfvénic isorotation in a steady axisymmetric wind</h5>

↑ **Parent:** [Axisymmetric magnetohydrodynamic wind](#axisymmetric-magnetohydrodynamic-wind)

Assume zero toroidal loop voltage in smooth steady [ideal magnetohydrodynamics](#ideal-magnetohydrodynamics), so the poloidal flow aligns with the [poloidal magnetic field](#poloidal-magnetic-field). Write $\rho\mathbf u_p=\eta\mathbf B_p$. The [continuity equation](physics.md#continuity-equation) makes $\eta$ constant along a magnetic line. The induction equation gives the conserved [field-line angular velocity](#field-line-angular-velocity) $\Omega_F=\Omega-\eta B_\phi/(\rho R)$. The azimuthal momentum equation is $\rho\mathbf u_p\cdot\nabla(R^2\Omega)=\mathbf B_p\cdot\nabla(RB_\phi)/\mu_0$; hence $L=R^2\Omega-RB_\phi/(\mu_0\eta)$ is also constant along the line.

With $M_{Ap}^2=\mu_0\eta^2/\rho=|\mathbf u_p|^2/v_{Ap}^2$, eliminating $B_\phi$ gives

$$
\Omega=\frac{\Omega_F-M_{Ap}^2L/R^2}{1-M_{Ap}^2}.
$$

For $M_{Ap}^2\ll1$ and nonsingular invariants, $\Omega=\Omega_F+O(M_{Ap}^2)$ and matter approximately corotates along a field line. With exactly zero poloidal flow, induction directly gives [Ferraro's law of isorotation](#ferraro-s-law-of-isorotation). The approximation requires the correction $M_{Ap}^2(\Omega_F-L/R^2)$ to be small on the segment in question.

##### Corotating energy invariant of an axisymmetric magnetic wind

↑ **Parent:** [Axisymmetric magnetohydrodynamic wind](#axisymmetric-magnetohydrodynamic-wind)

For a pressure-free flowing [poloidal flux surface](#axisymmetric-magnetic-flux-surface), subtracting its angular [velocity](classical-mechanics.md#velocity) times the azimuthal momentum equation from the mechanical energy equation shows that $\epsilon_J$ is constant. It equals poloidal kinetic energy plus $(u_\phi-R\omega)^2/2+\Phi-R^2\omega^2/2$. This is the total [magnetohydrodynamic Bernoulli invariant](#magnetohydrodynamic-bernoulli-invariant) minus $\omega$ times the total [magnetohydrodynamic angular-momentum invariant](#magnetohydrodynamic-angular-momentum-invariant), not the total energy alone.

##### Field-line angular velocity of an axisymmetric wind

↑ **Parent:** [Axisymmetric magnetohydrodynamic wind](#axisymmetric-magnetohydrodynamic-wind)

In steady axisymmetric [ideal magnetohydrodynamics](#ideal-magnetohydrodynamics), induction makes $\omega$ constant on regular connected [poloidal flux surfaces](#axisymmetric-magnetic-flux-surface). It describes field-line rotation. The material angular [velocity](classical-mechanics.md#velocity) is $u_\phi/R=\omega+kB_\phi/(\rho R)$ and differs when the toroidal [magnetic field](electromagnetism.md#magnetic-field) contributes. If the [poloidal magnetic field](#poloidal-magnetic-field) vanishes, the flux-surface integration requires separate treatment.

##### Poloidal magnetic flux function

↑ **Parent:** [Axisymmetric magnetohydrodynamic wind](#axisymmetric-magnetohydrodynamic-wind)

For $\mathbf B_p=\nabla\psi\times\nabla\phi$, surfaces $\psi=\text{constant}$ are poloidal magnetic surfaces and $2\pi\psi$ is magnetic flux up to the choice of axial reference value.

###### Material advection of an axisymmetric magnetic flux function

↑ **Parent:** [Poloidal magnetic flux function](#poloidal-magnetic-flux-function)

For an axisymmetric [poloidal magnetic field](#poloidal-magnetic-field) $\mathbf B_p=\nabla\Psi\times\nabla\phi$, the [ideal magnetohydrodynamic induction equation](#ideal-magnetohydrodynamic-induction-equation) gives $\partial_t\Psi+\mathbf u_p\cdot\nabla\Psi=0$, after fixing the time-dependent additive constant in $\Psi$. A regular axial reference makes $2\pi\Psi$ the enclosed [magnetic flux](electromagnetism.md#magnetic-flux). This scalar statement of [magnetic flux freezing](#magnetic-flux-freezing) holds even when rotation also produces a [toroidal magnetic field](#toroidal-magnetic-field).

###### Axisymmetric magnetic flux surface

↑ **Parent:** [Poloidal magnetic flux function](#poloidal-magnetic-flux-function)

A regular level surface of the axisymmetric [poloidal magnetic flux function](#poloidal-magnetic-flux-function) contains both the poloidal and toroidal [magnetic field](electromagnetism.md#magnetic-field) directions. Conservation along field lines can be expressed locally as a function of the flux label on connected regular surfaces. Degenerate points with no [poloidal magnetic field](#poloidal-magnetic-field) and disconnected branches with the same label require separate treatment.

###### Power-law poloidal field near a disk surface

↑ **Parent:** [Poloidal magnetic flux function](#poloidal-magnetic-flux-function)

If $\Psi(R,0)=\Psi_1+\Psi_0(R/R_0)^\delta$ and the surface inclination to the vertical is a radius-independent $\alpha$, then $B_z=\delta\Psi_0R^{\delta-2}/R_0^\delta$ and $B_R=B_z\tan\alpha$. The [solenoidal vector field](calculus.md#solenoidal-vector-field) condition gives

$$
\left.\partial_zB_z\right|_{0}=-\frac{\delta-1}{R}B_z(R,0)\tan\alpha.
$$

The constant offset in the [poloidal magnetic flux function](#poloidal-magnetic-flux-function) has no effect on the [magnetic field](electromagnetism.md#magnetic-field).

##### Magnetohydrodynamic mass loading

↑ **Parent:** [Axisymmetric magnetohydrodynamic wind](#axisymmetric-magnetohydrodynamic-wind)

When $\rho\mathbf u_p=k\mathbf B_p$, the flux-surface function $k$ is the mass flux per unit poloidal magnetic flux.

###### Regular-axis alignment of steady poloidal ideal flow

↑ **Parent:** [Magnetohydrodynamic mass loading](#magnetohydrodynamic-mass-loading)

For steady axisymmetric ideal flow with only poloidal components, induction implies $\mathbf u\times\mathbf B=C\mathbf e_\phi/R$. Axis regularity, or zero toroidal [electromotive force](electromagnetism.md#electromotive-force), sets $C=0$. Continuity then gives $\rho\mathbf u=k(\psi)\mathbf B$, locally on connected magnetic surfaces of the [poloidal magnetic flux function](#poloidal-magnetic-flux-function). Without the zero-circulation condition, annular domains can support steady cross-field flow.

##### Field-line angular velocity

↑ **Parent:** [Axisymmetric magnetohydrodynamic wind](#axisymmetric-magnetohydrodynamic-wind)

Ideal induction in a steady axisymmetric flow makes each magnetic surface rotate with a constant field-line angular velocity $\omega(\psi)$.

##### Magnetohydrodynamic angular-momentum invariant

↑ **Parent:** [Axisymmetric magnetohydrodynamic wind](#axisymmetric-magnetohydrodynamic-wind)

The total specific angular momentum transported by matter and magnetic stress is

$$
\ell=ru_\phi-\frac{rB_\phi}{\mu_0k},
$$

and is constant on each magnetic surface.

###### Maxwell torque conservation in an axisymmetric wind

↑ **Parent:** [Magnetohydrodynamic angular-momentum invariant](#magnetohydrodynamic-angular-momentum-invariant)

In a steady [axisymmetric magnetohydrodynamic wind](#axisymmetric-magnetohydrodynamic-wind), axisymmetric [pressure](thermodynamics.md#pressure) and [Newtonian gravity](classical-mechanics.md#gravitational-acceleration) exert no azimuthal [torque](classical-mechanics.md#torque). The azimuthal momentum equation is $\rho\mathbf u_p\cdot\nabla(su_\phi)=\mu_0^{-1}\mathbf B_p\cdot\nabla(sB_\phi)$. [Mass conservation](continuum-mechanics.md#mass-conservation) and the [solenoidal vector field](calculus.md#solenoidal-vector-field) condition imply $\nabla\cdot\mathbf F_J=0$. With [magnetohydrodynamic mass loading](#magnetohydrodynamic-mass-loading) $\rho\mathbf u_p=\kappa\mathbf B_p$, the transported [angular momentum](classical-mechanics.md#angular-momentum) per unit poloidal [magnetic flux](electromagnetism.md#magnetic-flux) is $\ell=\kappa s u_\phi-sB_\phi/\mu_0$. It is constant on connected regular [poloidal flux surfaces](#axisymmetric-magnetic-flux-surface). The usual specific [magnetohydrodynamic angular-momentum invariant](#magnetohydrodynamic-angular-momentum-invariant) is $L=\ell/\kappa$, provided $\kappa\ne0$; confusing these two normalizations loses a factor of mass loading in the wind [torque](classical-mechanics.md#torque).

##### Magnetohydrodynamic Bernoulli invariant

↑ **Parent:** [Axisymmetric magnetohydrodynamic wind](#axisymmetric-magnetohydrodynamic-wind)

Along a steady axisymmetric ideal-MHD wind, the total specific energy

$$
\epsilon=\frac12|\mathbf u|^2+\Phi+h
-\frac{r\omega B_\phi}{\mu_0k}
$$

is constant on each magnetic surface. The last term is the electromagnetic energy transported per unit mass flux.

###### Isothermal magnetic Bernoulli integral

↑ **Parent:** [Magnetohydrodynamic Bernoulli invariant](#magnetohydrodynamic-bernoulli-invariant)

In aligned steady ideal flow with $p=c_s^2\rho$ and constant [isothermal sound speed](compressible-flow.md#isothermal-sound-speed), the [Lorentz force density](electromagnetism.md#lorentz-force-density) has no field-parallel component. Projecting momentum along the [magnetic field](electromagnetism.md#magnetic-field) makes $u^2/2+\Phi+c_s^2\ln(\rho/\rho_0)$ constant on each connected magnetic surface. The arbitrary reference density changes only the additive constant.

<h5 id="alfven-surface">Alfvén surface</h5>

↑ **Parent:** [Axisymmetric magnetohydrodynamic wind](#axisymmetric-magnetohydrodynamic-wind)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Alfvén_surface)

An Alfvén surface is where the poloidal flow speed equals the poloidal Alfvén speed. Smooth passage through it imposes a regularity condition relating field-line angular velocity and angular momentum.

<h6 id="alfven-radius">Alfvén radius</h6>

↑ **Parent:** [Alfvén surface](#alfven-surface)

The Alfvén radius characterizes where a magnetized [stellar wind](stellar-astrophysics.md#stellar-wind) crosses its [Alfvén surface](#alfven-surface). For a roughly radial wind, $v_{\rm wind}\simeq B/\sqrt{\mu_0\rho}$ and $\dot M_w\simeq4\pi R_A^2\rho v_{\rm wind}$. The wind's angular-momentum lever arm is of order $R_A$: its torque is $\dot J\sim-\dot M_w\Omega R_A^2$, up to geometry factors. The precise wind invariant uses the cylindrical radius of the surface crossing, rather than necessarily its spherical radius.

<h6 id="alfven-surface-regularity-condition-for-an-axisymmetric-wind">Alfvén-surface regularity condition for an axisymmetric wind</h6>

↑ **Parent:** [Alfvén surface](#alfven-surface)

If $r_A$ is the cylindrical radius at which $M_A^2=\mu_0k^2/\rho=1$, finite azimuthal velocity and magnetic field require

$$
\ell=\omega r_A^2.
$$

This cancels the simultaneous numerator and denominator zeros in the wind's azimuthal integrals.

##### Asymptotic energy of a radial magnetohydrodynamic wind

↑ **Parent:** [Axisymmetric magnetohydrodynamic wind](#axisymmetric-magnetohydrodynamic-wind)

If $r^2|B_p|\to F$ and $u_p\to u_\infty$ along an open magnetic surface, then

$$
B_\phi\sim-\frac{\omega F}{u_\infty r},
\qquad
|v_{A\phi}|\to\omega\sqrt{\frac{F}{\mu_0ku_\infty}}.
$$

When enthalpy and gravity vanish asymptotically, the Bernoulli invariant becomes

$$
\epsilon=\frac12u_\infty^2+\frac{\omega^2F}{\mu_0ku_\infty}.
$$

##### Magnetocentrifugal acceleration

↑ **Parent:** [Axisymmetric magnetohydrodynamic wind](#axisymmetric-magnetohydrodynamic-wind)

Magnetocentrifugal acceleration occurs when matter tied to a rotating inclined magnetic field moves outward under the effective centrifugal force. For a Keplerian disc, cold launching is possible when the field tilts by more than $30^\circ$ from the vertical.

###### Thirty-degree magnetocentrifugal launching criterion

↑ **Parent:** [Magnetocentrifugal acceleration](#magnetocentrifugal-acceleration)

For a cold corotating field line anchored in a circular point-mass orbit, the [effective potential](physics.md#effective-potential) has meridional Hessian $\omega^2\operatorname{diag}(-3,1)$. Along a straight line inclined by $\alpha$ to the vertical its quadratic curvature is $\omega^2(1-4\sin^2\alpha)$. Negative curvature gives the strict local launching criterion. Equality is marginal and global escape requires additional information.

###### Marginal straight-line launch at thirty degrees

↑ **Parent:** [Thirty-degree magnetocentrifugal launching criterion](#thirty-degree-magnetocentrifugal-launching-criterion)

At exactly thirty degrees the quadratic curvature vanishes, but the specified straight-line point-mass [effective potential](physics.md#effective-potential) is downhill for small positive displacement at cubic order. Thus the strict negative-curvature criterion does not exclude every nonlinear one-sided marginal launch. An exactly stationary bead remains at equilibrium until displaced.

###### Magnetocentrifugal launching criterion in a flattened power-law potential

↑ **Parent:** [Magnetocentrifugal acceleration](#magnetocentrifugal-acceleration)

In a [flattened power-law gravitational potential](classical-mechanics.md#flattened-power-law-gravitational-potential) $\Phi=\Phi_0R_0^\beta(R^2+\lambda^2z^2)^{-\beta/2}$, a magnetic surface corotating with its disk footpoint has an [effective potential](physics.md#effective-potential) with meridional [Hessian matrix](calculus.md#hessian-matrix) $\Omega_f^2\operatorname{diag}[-(\beta+2),\lambda^2]$ there. A cold outward displacement along a field inclined by $\alpha$ to the vertical is downhill when $\tan^2\alpha>\lambda^2/(\beta+2)$. Equality is marginal and can depend on higher derivatives and field-line curvature; this is a local launching criterion, not a guarantee of a global escaping wind.

## Self-gravitating gaseous filament

↑ **Parent:** [Astrophysical fluid dynamics](astrophysical-fluid-dynamics.md)

A self-gravitating gaseous filament is an elongated fluid configuration supported against its own radial gravity by gas pressure, magnetic stress, rotation, or turbulence. In an infinite axisymmetric model, its gravitational field obeys the cylindrical Poisson equation.

### Magnetized self-gravitating filament

↑ **Parent:** [Self-gravitating gaseous filament](#self-gravitating-gaseous-filament)

For a filament formed by collapse perpendicular to a frozen axial field, $B_z/\rho$ remains constant. The axial magnetic pressure can then be combined with a quadratic equation of state into an effective polytropic constant.

### Line mass

↑ **Parent:** [Self-gravitating gaseous filament](#self-gravitating-gaseous-filament)

The line mass is mass per unit length along a filament. For an axisymmetric density profile $\rho(R)$,

$$
\lambda=2\pi\int_0^\infty\rho(R)R\,dR,
$$

with the upper limit replaced by the filament radius when the density has compact support.

## Parker wind

↑ **Parent:** [Astrophysical fluid dynamics](astrophysical-fluid-dynamics.md)

A Parker wind is a steady, spherically symmetric outflow accelerated from a gravitating body through a sonic point. Smoothness selects the transonic solution from the family of formal steady solutions.

### Polytropic Parker wind

↑ **Parent:** [Parker wind](#parker-wind)

A polytropic Parker wind is isentropic with $p=K\rho^\gamma$. Its sound speed changes with density, and a wind reaching infinity with positive terminal kinetic energy requires $1<\gamma<5/3$.

#### Parker wind equation

↑ **Parent:** [Polytropic Parker wind](#polytropic-parker-wind)

For radial speed $u$, sound speed $c_s$, and central mass $M$, steady spherical mass and momentum conservation give

$$
\left(u-\frac{c_s^2}{u}\right)\frac{du}{dr}
=\frac{2c_s^2}{r}-\frac{GM}{r^2}.
$$

At a regular sonic point, $u=c_s$ and $r=GM/(2c_s^2)$ simultaneously.

## ↑ Ancestors (4)

1. [Fluid mechanics](fluid-mechanics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)
