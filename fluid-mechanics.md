# Fluid mechanics

↑ **Parent:** [Branches of physics](physics.md#branches-of-physics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fluid_mechanics)

Fluid mechanics studies the motion and forces of liquids and gases.

**Table of contents**

- [Void fraction](#void-fraction)
  - [Kinematic bubble transport in an exponentially narrowing vessel](#kinematic-bubble-transport-in-an-exponentially-narrowing-vessel)
  - [Bubble clearing in a cylindrical vessel](#bubble-clearing-in-a-cylindrical-vessel)
- [Strouhal number](#strouhal-number)
- [Lift (force)](#lift-force)
- [Airfoil](#airfoil)
- [Uniform flow](#uniform-flow)
- [Volume viscosity](#volume-viscosity)
- [Hydraulic resistance](#hydraulic-resistance)
- [Physiological fluid dynamics](#physiological-fluid-dynamics)
  - [Lubrication model of a compliant translating plug](#lubrication-model-of-a-compliant-translating-plug)
    - [Force-free pressure drop of an annular lubrication plug](#force-free-pressure-drop-of-an-annular-lubrication-plug)
      - [Small-speed compliant-plug lubrication asymptotics](#small-speed-compliant-plug-lubrication-asymptotics)
  - [Annular inviscid-core displacement](#annular-inviscid-core-displacement)
    - [Forced annular displacement equation](#forced-annular-displacement-equation)
      - [Opposite propagation directions in the annular displacement equation](#opposite-propagation-directions-in-the-annular-displacement-equation)
  - [Peristaltic pumping](#peristaltic-pumping)
    - [Weak peristaltic pumping of a collapsible tube](#weak-peristaltic-pumping-of-a-collapsible-tube)
  - [Collapsible tube flow](#collapsible-tube-flow)
    - [Choking by wall thickness in an elastic tube](#choking-by-wall-thickness-in-an-elastic-tube)
    - [Subcritical tube flow](#subcritical-tube-flow)
    - [Supercritical tube flow](#supercritical-tube-flow)
    - [Elastic jump in a quadratic pressure-area tube](#elastic-jump-in-a-quadratic-pressure-area-tube)
    - [Spatial attraction of a uniform downhill tube flow](#spatial-attraction-of-a-uniform-downhill-tube-flow)
    - [Friction-induced instability of a collapsible-tube flow](#friction-induced-instability-of-a-collapsible-tube-flow)
    - [Pressure-area law of a collapsible tube](#pressure-area-law-of-a-collapsible-tube)
      - [Tube wave speed](#tube-wave-speed)
  - [Arterial pressure wave](#arterial-pressure-wave)
    - [Bifurcation reflection of an arterial pressure wave](#bifurcation-reflection-of-an-arterial-pressure-wave)
      - [Pressure-flow phase lag from one arterial reflection](#pressure-flow-phase-lag-from-one-arterial-reflection)
    - [Reflection of an arterial pressure wave](#reflection-of-an-arterial-pressure-wave)
    - [Wave transfer matrix of an arterial segment](#wave-transfer-matrix-of-an-arterial-segment)
      - [Wave transmission through a resistively loaded arterial loop](#wave-transmission-through-a-resistively-loaded-arterial-loop)
    - [Characteristic admittance of an arterial wave](#characteristic-admittance-of-an-arterial-wave)
- [Fluid](#fluid)
- [Buoyant plume](#buoyant-plume)
- [Pathline](#pathline)
- [Control volume](#control-volume)
- [Navier slip boundary condition](#navier-slip-boundary-condition)
  - [Slip length](#slip-length)
- [Fluid free boundary](#fluid-free-boundary)
- [Material surface](#material-surface)
  - [Material surface element](#material-surface-element)
- [Material curve](#material-curve)
- [Scalar transport](#scalar-transport)
  - [Active scalar](#active-scalar)
  - [Passive scalar](#passive-scalar)
    - [Gaussian scalar packet in a linear incompressible flow](#gaussian-scalar-packet-in-a-linear-incompressible-flow)
      - [Diffusion arrest of Gaussian packet compression](#diffusion-arrest-of-gaussian-packet-compression)
        - [Large-deviation decay rates of a Gaussian scalar packet](#large-deviation-decay-rates-of-a-gaussian-scalar-packet)
    - [Schmidt number (fluid mechanics)](#schmidt-number-fluid-mechanics)
    - [Covector evolution of a material scalar gradient](#covector-evolution-of-a-material-scalar-gradient)
      - [Scalar-gradient inclination in a steady planar strain](#scalar-gradient-inclination-in-a-steady-planar-strain)
        - [White-noise vertical shear gives an Ornstein-Uhlenbeck inclination](#white-noise-vertical-shear-gives-an-ornstein-uhlenbeck-inclination)
        - [Gaussian-over-Rayleigh inclination distribution](#gaussian-over-rayleigh-inclination-distribution)
    - [Scalar structure function](#scalar-structure-function)
    - [Obukhov-Corrsin theory](#obukhov-corrsin-theory)
      - [Inertial-diffusive scalar range](#inertial-diffusive-scalar-range)
        - [Corrsin scalar microscale](#corrsin-scalar-microscale)
      - [Viscous-convective scalar range](#viscous-convective-scalar-range)
        - [Batchelor scalar microscale](#batchelor-scalar-microscale)
      - [Inertial-convective scalar range](#inertial-convective-scalar-range)
    - [Horizontally integrated plume concentration](#horizontally-integrated-plume-concentration)
      - [Horizontally averaged plume concentration](#horizontally-averaged-plume-concentration)
  - [Adjoint equations for Boussinesq scalar mixing](#adjoint-equations-for-boussinesq-scalar-mixing)
  - [Scalar variance](#scalar-variance)
    - [Scalar dissipation rate](#scalar-dissipation-rate)
- [Fluid flow](#fluid-flow)
  - [Unidirectional flow](#unidirectional-flow)
  - [Steady flow](#steady-flow)
  - [Inviscid flow](#inviscid-flow)
    - [Inviscid falling jet and radial impact film](#inviscid-falling-jet-and-radial-impact-film)
- [Sediment transport](#sediment-transport)
  - [Sediment resuspension](#sediment-resuspension)
    - [Equilibrium settling-diffusion profile](#equilibrium-settling-diffusion-profile)
  - [Sediment transport saturation](#sediment-transport-saturation)
    - [Equilibrium sediment flux](#equilibrium-sediment-flux)
    - [Saturation length](#saturation-length)
  - [Exner equation](#exner-equation)
  - [Shields parameter](#shields-parameter)
    - [Sediment entrainment threshold](#sediment-entrainment-threshold)
      - [Inclined-bed sediment threshold](#inclined-bed-sediment-threshold)
  - [Bedform](#bedform)
    - [Sediment-bed linear instability](#sediment-bed-linear-instability)
    - [Bed shear response](#bed-shear-response)
- [Ram pressure](#ram-pressure)
- [Turbulence](turbulence.md)
  - [Reynolds averaging](turbulence.md#reynolds-averaging)
  - [External intermittency](turbulence.md#external-intermittency)
  - [Wave turbulence](turbulence.md#wave-turbulence)
    - [Weak wave cascade](turbulence.md#weak-wave-cascade)
  - [Magnetohydrodynamic turbulence](turbulence.md#magnetohydrodynamic-turbulence)
    - [Dimensional freedom of an MHD spectrum](turbulence.md#dimensional-freedom-of-an-mhd-spectrum)
    - [Electron-magnetohydrodynamic cascade](turbulence.md#electron-magnetohydrodynamic-cascade)
      - [Critically balanced electron-magnetohydrodynamic cascade](turbulence.md#critically-balanced-electron-magnetohydrodynamic-cascade)
      - [Weak electron-magnetohydrodynamic cascade](turbulence.md#weak-electron-magnetohydrodynamic-cascade)
    - [Critical balance](turbulence.md#critical-balance)
    - [Alfvénic turbulence](turbulence.md#alfvenic-turbulence)
      - [Weak Alfvénic cascade](turbulence.md#weak-alfvenic-cascade)
        - [Weak-to-strong transition of an Alfvénic cascade](turbulence.md#weak-to-strong-transition-of-an-alfvenic-cascade)
      - [Iroshnikov-Kraichnan spectrum](turbulence.md#iroshnikov-kraichnan-spectrum)
      - [Goldreich–Sridhar turbulence](turbulence.md#goldreich-sridhar-turbulence)
  - [Turbulence closure](turbulence.md#turbulence-closure)
    - [Constant-skewness turbulence closure](turbulence.md#constant-skewness-turbulence-closure)
      - [Normalized constant-skewness structure-function equation](turbulence.md#normalized-constant-skewness-structure-function-equation)
    - [Eddy-damped quasi-normal Markovian closure](turbulence.md#eddy-damped-quasi-normal-markovian-closure)
  - [K-epsilon turbulence model](turbulence.md#k-epsilon-turbulence-model)
    - [K-epsilon turbulence front](turbulence.md#k-epsilon-turbulence-front)
    - [Log-layer solution of the k-epsilon model](turbulence.md#log-layer-solution-of-the-k-epsilon-model)
  - [Turbulent mixing](turbulence.md#turbulent-mixing)
    - [Richardson pair dispersion](turbulence.md#richardson-pair-dispersion)
      - [Three-regime turbulent pair-separation model](turbulence.md#three-regime-turbulent-pair-separation-model)
      - [Diffusive large-scale pair dispersion](turbulence.md#diffusive-large-scale-pair-dispersion)
      - [Richardson constant](turbulence.md#richardson-constant)
    - [Taylor turbulent dispersion](turbulence.md#taylor-turbulent-dispersion)
      - [Power-law velocity-correlation dispersion](turbulence.md#power-law-velocity-correlation-dispersion)
      - [Lagrangian velocity autocorrelation](turbulence.md#lagrangian-velocity-autocorrelation)
      - [Lagrangian integral time](turbulence.md#lagrangian-integral-time)
    - [Forced stratified mixing with square-root power input](turbulence.md#forced-stratified-mixing-with-square-root-power-input)
    - [Stratified mixing energy budget](turbulence.md#stratified-mixing-energy-budget)
      - [Instantaneous mixing efficiency](turbulence.md#instantaneous-mixing-efficiency)
        - [Cumulative mixing efficiency](turbulence.md#cumulative-mixing-efficiency)
  - [Turbulent plane jet similarity](turbulence.md#turbulent-plane-jet-similarity)
    - [Finite-edge stress condition for a mixing-length jet](turbulence.md#finite-edge-stress-condition-for-a-mixing-length-jet)
  - [Mixing length](turbulence.md#mixing-length)
    - [Mixing-length closure](turbulence.md#mixing-length-closure)
  - [Turbulent kinetic energy](turbulence.md#turbulent-kinetic-energy)
    - [Mean-shear production of turbulent kinetic energy](turbulence.md#mean-shear-production-of-turbulent-kinetic-energy)
    - [Local turbulent kinetic energy balance](turbulence.md#local-turbulent-kinetic-energy-balance)
      - [Fixed-correlation equilibrium model for stratified turbulence](turbulence.md#fixed-correlation-equilibrium-model-for-stratified-turbulence)
  - [Reynolds stress](turbulence.md#reynolds-stress)
    - [Nondiffusive convective angular momentum transport](turbulence.md#nondiffusive-convective-angular-momentum-transport)
    - [Reynolds-stress energy production in a shearing sheet](turbulence.md#reynolds-stress-energy-production-in-a-shearing-sheet)
    - [Constant-stress Reynolds-averaged wall flow](turbulence.md#constant-stress-reynolds-averaged-wall-flow)
    - [Eddy viscosity](turbulence.md#eddy-viscosity)
    - [Reynolds-averaged momentum equation](turbulence.md#reynolds-averaged-momentum-equation)
  - [Internal intermittency](turbulence.md#internal-intermittency)
    - [Kolmogorov refined similarity hypothesis](turbulence.md#kolmogorov-refined-similarity-hypothesis)
      - [Lognormal intermittency model](turbulence.md#lognormal-intermittency-model)
    - [Coarse-grained energy dissipation](turbulence.md#coarse-grained-energy-dissipation)
    - [Integral-scale intermittency](turbulence.md#integral-scale-intermittency)
      - [Landau intermittency counterexample](turbulence.md#landau-intermittency-counterexample)
  - [Energy cascade](turbulence.md#energy-cascade)
    - [Spectral triad interaction](turbulence.md#spectral-triad-interaction)
    - [Zeroth law of turbulence](turbulence.md#zeroth-law-of-turbulence)
      - [Turbulent dissipation anomaly](turbulence.md#turbulent-dissipation-anomaly)
    - [Eddy turnover time](turbulence.md#eddy-turnover-time)
    - [Two-dimensional enstrophy cascade](turbulence.md#two-dimensional-enstrophy-cascade)
      - [Logarithmic structure function in an enstrophy cascade](turbulence.md#logarithmic-structure-function-in-an-enstrophy-cascade)
    - [Townsend-Betchov cascade cartoon](turbulence.md#townsend-betchov-cascade-cartoon)
    - [Kolmogorov 1941 theory](turbulence.md#kolmogorov-1941-theory)
      - [Kolmogorov second similarity hypothesis](turbulence.md#kolmogorov-second-similarity-hypothesis)
        - [Kolmogorov two-thirds law](turbulence.md#kolmogorov-two-thirds-law)
      - [Kolmogorov first similarity hypothesis](turbulence.md#kolmogorov-first-similarity-hypothesis)
    - [Equilibrium range](turbulence.md#equilibrium-range)
    - [Dissipation range](turbulence.md#dissipation-range)
      - [Kolmogorov microscales](turbulence.md#kolmogorov-microscales)
        - [Kolmogorov length scale](turbulence.md#kolmogorov-length-scale)
    - [Inertial range](turbulence.md#inertial-range)
  - [Homogeneous turbulence](turbulence.md#homogeneous-turbulence)
    - [Integral scale of turbulence](turbulence.md#integral-scale-of-turbulence)
    - [Betchov relation](turbulence.md#betchov-relation)
    - [Isotropic turbulence](turbulence.md#isotropic-turbulence)
      - [Local isotropy of turbulence](turbulence.md#local-isotropy-of-turbulence)
      - [Loitsyansky integral](turbulence.md#loitsyansky-integral)
        - [Landau angular-momentum argument for turbulent decay](turbulence.md#landau-angular-momentum-argument-for-turbulent-decay)
        - [Kolmogorov decay law](turbulence.md#kolmogorov-decay-law)
      - [Saffman integral](turbulence.md#saffman-integral)
        - [Saffman decay law](turbulence.md#saffman-decay-law)
        - [Small-wavenumber spectrum with nonzero Saffman integral](turbulence.md#small-wavenumber-spectrum-with-nonzero-saffman-integral)
      - [Velocity correlation tensor](turbulence.md#velocity-correlation-tensor)
        - [Kármán-Howarth equation](turbulence.md#karman-howarth-equation)
          - [Kolmogorov equation for structure functions](turbulence.md#kolmogorov-equation-for-structure-functions)
            - [Kolmogorov four-fifths law](turbulence.md#kolmogorov-four-fifths-law)
        - [Longitudinal velocity correlation](turbulence.md#longitudinal-velocity-correlation)
          - [Longitudinal velocity structure function](turbulence.md#longitudinal-velocity-structure-function)
            - [Velocity increment](turbulence.md#velocity-increment)
            - [Large-scale contributions to structure functions](turbulence.md#large-scale-contributions-to-structure-functions)
            - [Structure-function spectral filter](turbulence.md#structure-function-spectral-filter)
      - [Turbulent energy spectrum](turbulence.md#turbulent-energy-spectrum)
      - [Longitudinal velocity-gradient skewness](turbulence.md#longitudinal-velocity-gradient-skewness)
  - [Eddy diffusion](turbulence.md#eddy-diffusion)
    - [Buoyancy-driven turbulent density diffusion](turbulence.md#buoyancy-driven-turbulent-density-diffusion)
      - [Quintic density-profile similarity in an unstable tube](turbulence.md#quintic-density-profile-similarity-in-an-unstable-tube)
    - [Density-variance dissipation rate](turbulence.md#density-variance-dissipation-rate)
    - [Turbulent Prandtl number](turbulence.md#turbulent-prandtl-number)
      - [Reynolds analogy](turbulence.md#reynolds-analogy)
    - [Vertical turbulent buoyancy flux](turbulence.md#vertical-turbulent-buoyancy-flux)
    - [Buoyancy-gradient mixing-length closure](turbulence.md#buoyancy-gradient-mixing-length-closure)
      - [Arrested cubic buoyancy profile](turbulence.md#arrested-cubic-buoyancy-profile)
      - [Flux convergence in turbulent buoyancy mixing](turbulence.md#flux-convergence-in-turbulent-buoyancy-mixing)
  - [Eddy diffusivity](turbulence.md#eddy-diffusivity)
    - [Turbulent Schmidt number](turbulence.md#turbulent-schmidt-number)
  - [Turbulent round jet](turbulence.md#turbulent-round-jet)
- [Acoustic wave](#acoustic-wave)
  - [Burgers reduction of weakly nonlinear rightgoing acoustics](#burgers-reduction-of-weakly-nonlinear-rightgoing-acoustics)
  - [Adiabatic vertical modes of a Gaussian atmosphere](#adiabatic-vertical-modes-of-a-gaussian-atmosphere)
  - [Acoustically rigid boundary](#acoustically-rigid-boundary)
  - [Acoustic cutoff frequency](#acoustic-cutoff-frequency)
  - [Pressure-release boundary](#pressure-release-boundary)
- [Velocity field](#velocity-field)
  - [Secondary flow](#secondary-flow)
  - [Velocity gradient tensor](#velocity-gradient-tensor)
  - [Vertical velocity](#vertical-velocity)
  - [Axisymmetric flow](#axisymmetric-flow)
- [Advection](#advection)
  - [Chaotic advection](#chaotic-advection)
  - [Ballistic transport](#ballistic-transport)
- [Convection](#convection)
  - [Convection cell](#convection-cell)
  - [Convection zone](#convection-zone)
  - [Compositional convection](#compositional-convection)
  - [Long-wave convection equation with broken Boussinesq symmetry](#long-wave-convection-equation-with-broken-boussinesq-symmetry)
    - [Second-harmonic feedback in a long-wave convection amplitude equation](#second-harmonic-feedback-in-a-long-wave-convection-amplitude-equation)
    - [Energy square completion for long-wave convection](#energy-square-completion-for-long-wave-convection)
  - [Thermal convection](#thermal-convection)
    - [Horizontal convection](#horizontal-convection)
      - [Shallow horizontal convection with an insulated bottom](#shallow-horizontal-convection-with-an-insulated-bottom)
        - [Advection correction in shallow horizontal convection](#advection-correction-in-shallow-horizontal-convection)
    - [Forced convection](#forced-convection)
    - [Natural convection](#natural-convection)
      - [Free-convection surface-layer scaling](#free-convection-surface-layer-scaling)
    - [Hexagonal convection amplitude equations](#hexagonal-convection-amplitude-equations)
      - [Rotational hexagon amplitude equations](#rotational-hexagon-amplitude-equations)
        - [Roll and hexagon spectra without reflection symmetry](#roll-and-hexagon-spectra-without-reflection-symmetry)
        - [Axial isotropy of rolls and hexagons](#axial-isotropy-of-rolls-and-hexagons)
      - [Roll instability from broken up-down symmetry](#roll-instability-from-broken-up-down-symmetry)
    - [Convection roll](#convection-roll)
    - [Oscillatory convection](#oscillatory-convection)
      - [Travelling and standing convection rolls](#travelling-and-standing-convection-rolls)
    - [Stationary convection](#stationary-convection)
    - [Convective stability](#convective-stability)
    - [Convective overshoot](#convective-overshoot)
    - [Double-diffusive convection](#double-diffusive-convection)
      - [Thermosolutal convection](#thermosolutal-convection)
        - [Double-diffusive overflow reservoir](#double-diffusive-overflow-reservoir)
          - [Post-shutdown double-diffusive reservoir cooling](#post-shutdown-double-diffusive-reservoir-cooling)
        - [Lorenz model of thermosolutal convection](#lorenz-model-of-thermosolutal-convection)
          - [Oscillatory threshold of a thermosolutal Lorenz model](#oscillatory-threshold-of-a-thermosolutal-lorenz-model)
          - [Steady fold of a thermosolutal Lorenz model](#steady-fold-of-a-thermosolutal-lorenz-model)
      - [Layered convection](#layered-convection)
- [Buoyancy](#buoyancy)
  - [Buoyancy gradient](#buoyancy-gradient)
  - [Magnetic buoyancy](#magnetic-buoyancy)
  - [Archimedes' principle](#archimedes-principle)
  - [Submerged weight](#submerged-weight)
  - [Buoyancy perturbation](#buoyancy-perturbation)
    - [Buoyancy displacement variable](#buoyancy-displacement-variable)
  - [Isopycnal](#isopycnal)
- [Hydrodynamic stability](hydrodynamic-stability.md)
  - [Global hydrodynamic mode](hydrodynamic-stability.md#global-hydrodynamic-mode)
  - [Global hydrodynamic instability](hydrodynamic-stability.md#global-hydrodynamic-instability)
    - [Global modes of a quadratically confined Ginzburg-Landau equation](hydrodynamic-stability.md#global-modes-of-a-quadratically-confined-ginzburg-landau-equation)
  - [Critical layer in a shear flow](hydrodynamic-stability.md#critical-layer-in-a-shear-flow)
    - [Neutral-mode critical-layer matching](hydrodynamic-stability.md#neutral-mode-critical-layer-matching)
      - [Neutral Rayleigh-mode dispersion correction](hydrodynamic-stability.md#neutral-rayleigh-mode-dispersion-correction)
    - [Prandtl critical layer at a stationary shear profile](hydrodynamic-stability.md#prandtl-critical-layer-at-a-stationary-shear-profile)
      - [High-wavenumber instability of a non-monotone Prandtl layer](hydrodynamic-stability.md#high-wavenumber-instability-of-a-non-monotone-prandtl-layer)
  - [Critical level of a shear-flow wave](hydrodynamic-stability.md#critical-level-of-a-shear-flow-wave)
  - [Baroclinic instability](hydrodynamic-stability.md#baroclinic-instability)
  - [Three-layer long-wave shear-flow matching](hydrodynamic-stability.md#three-layer-long-wave-shear-flow-matching)
    - [Airy wall-layer matching determinant](hydrodynamic-stability.md#airy-wall-layer-matching-determinant)
  - [Pressure equation for a shear-flow normal mode](hydrodynamic-stability.md#pressure-equation-for-a-shear-flow-normal-mode)
  - [Adjoint linearized Navier-Stokes evolution](hydrodynamic-stability.md#adjoint-linearized-navier-stokes-evolution)
  - [Kinetic-energy inner product](hydrodynamic-stability.md#kinetic-energy-inner-product)
  - [Stability diagram of the linear complex Ginzburg-Landau equation](hydrodynamic-stability.md#stability-diagram-of-the-linear-complex-ginzburg-landau-equation)
  - [Saddle growth rate along a ray](hydrodynamic-stability.md#saddle-growth-rate-along-a-ray)
  - [Convective hydrodynamic instability](hydrodynamic-stability.md#convective-hydrodynamic-instability)
  - [Absolute hydrodynamic instability](hydrodynamic-stability.md#absolute-hydrodynamic-instability)
    - [Anisotropic absolute-instability threshold for positive diffusion](hydrodynamic-stability.md#anisotropic-absolute-instability-threshold-for-positive-diffusion)
    - [Absolute frequency](hydrodynamic-stability.md#absolute-frequency)
      - [Absolute-frequency conservation in steady shear](hydrodynamic-stability.md#absolute-frequency-conservation-in-steady-shear)
      - [Absolute growth rate](hydrodynamic-stability.md#absolute-growth-rate)
      - [Absolute wavenumber](hydrodynamic-stability.md#absolute-wavenumber)
  - [Orr-Sommerfeld equation](hydrodynamic-stability.md#orr-sommerfeld-equation)
    - [Squire's theorem](hydrodynamic-stability.md#squire-s-theorem)
      - [Squire transformation](hydrodynamic-stability.md#squire-transformation)
    - [Airy reduction of the Orr-Sommerfeld equation in constant shear](hydrodynamic-stability.md#airy-reduction-of-the-orr-sommerfeld-equation-in-constant-shear)
      - [Velocity reconstruction from the Orr-Sommerfeld vorticity](hydrodynamic-stability.md#velocity-reconstruction-from-the-orr-sommerfeld-vorticity)
    - [Squire equation](hydrodynamic-stability.md#squire-equation)
      - [Squire mode](hydrodynamic-stability.md#squire-mode)
        - [Dissipation identity for a homogeneous Squire mode](hydrodynamic-stability.md#dissipation-identity-for-a-homogeneous-squire-mode)
    - [Orr-Sommerfeld mode](hydrodynamic-stability.md#orr-sommerfeld-mode)
  - [Inertial instability](hydrodynamic-stability.md#inertial-instability)
  - [Rayleigh equation for inviscid shear flow](hydrodynamic-stability.md#rayleigh-equation-for-inviscid-shear-flow)
    - [Inviscid instability of a piecewise-linear mixing layer](hydrodynamic-stability.md#inviscid-instability-of-a-piecewise-linear-mixing-layer)
    - [Axisymmetric inviscid pipe stability equation](hydrodynamic-stability.md#axisymmetric-inviscid-pipe-stability-equation)
      - [Evanescent potential modes of inviscid Poiseuille flow](hydrodynamic-stability.md#evanescent-potential-modes-of-inviscid-poiseuille-flow)
    - [Inviscid instability of a triangular jet](hydrodynamic-stability.md#inviscid-instability-of-a-triangular-jet)
    - [Pressure matching at a piecewise-linear shear interface](hydrodynamic-stability.md#pressure-matching-at-a-piecewise-linear-shear-interface)
    - [Fjørtoft theorem](hydrodynamic-stability.md#fjortoft-theorem)
    - [Inviscid Couette continuous spectrum](hydrodynamic-stability.md#inviscid-couette-continuous-spectrum)
      - [Inviscid Couette initial-value Green function](hydrodynamic-stability.md#inviscid-couette-initial-value-green-function)
      - [Linear inviscid damping in unbounded Couette flow](hydrodynamic-stability.md#linear-inviscid-damping-in-unbounded-couette-flow)
      - [Vorticity-sheet eigenfunction of inviscid Couette flow](hydrodynamic-stability.md#vorticity-sheet-eigenfunction-of-inviscid-couette-flow)
    - [Vorticity-jump matching for an inviscid shear flow](hydrodynamic-stability.md#vorticity-jump-matching-for-an-inviscid-shear-flow)
    - [Inviscid parallel shear flow](hydrodynamic-stability.md#inviscid-parallel-shear-flow)
      - [Unbounded piecewise-linear shear layer](hydrodynamic-stability.md#unbounded-piecewise-linear-shear-layer)
      - [Three-layer stratified piecewise-linear shear flow](hydrodynamic-stability.md#three-layer-stratified-piecewise-linear-shear-flow)
        - [Quartic dispersion relation for a three-layer stratified shear flow](hydrodynamic-stability.md#quartic-dispersion-relation-for-a-three-layer-stratified-shear-flow)
        - [Unstable band of a three-layer stratified shear flow](hydrodynamic-stability.md#unstable-band-of-a-three-layer-stratified-shear-flow)
      - [Hazel model](hydrodynamic-stability.md#hazel-model)
        - [Neutral mode of the equal-width Hazel model](hydrodynamic-stability.md#neutral-mode-of-the-equal-width-hazel-model)
          - [Critical-layer regularity of a neutral Hazel mode](hydrodynamic-stability.md#critical-layer-regularity-of-a-neutral-hazel-mode)
      - [Bounded piecewise-linear shear layer](hydrodynamic-stability.md#bounded-piecewise-linear-shear-layer)
        - [Instability threshold for a bounded piecewise-linear shear layer](hydrodynamic-stability.md#instability-threshold-for-a-bounded-piecewise-linear-shear-layer)
    - [Rayleigh's inflection-point theorem](hydrodynamic-stability.md#rayleigh-s-inflection-point-theorem)
    - [Howard's semicircle theorem](hydrodynamic-stability.md#howard-s-semicircle-theorem)
      - [Weighted identity for Howard's semicircle theorem](hydrodynamic-stability.md#weighted-identity-for-howard-s-semicircle-theorem)
  - [Counterpropagating wave instability](hydrodynamic-stability.md#counterpropagating-wave-instability)
    - [Counterpropagating wave resonance in a three-layer shear flow](hydrodynamic-stability.md#counterpropagating-wave-resonance-in-a-three-layer-shear-flow)
  - [Transient growth from non-normal modes](hydrodynamic-stability.md#transient-growth-from-non-normal-modes)
    - [Orr mechanism](hydrodynamic-stability.md#orr-mechanism)
    - [Lift-up effect](hydrodynamic-stability.md#lift-up-effect)
  - [Energy-stability threshold](hydrodynamic-stability.md#energy-stability-threshold)
  - [Symmetric instability](hydrodynamic-stability.md#symmetric-instability)
  - [Eady model](hydrodynamic-stability.md#eady-model)
    - [Eady model with parallel sloping boundaries](hydrodynamic-stability.md#eady-model-with-parallel-sloping-boundaries)
    - [Boundary pseudomomentum of a sloping Eady layer](hydrodynamic-stability.md#boundary-pseudomomentum-of-a-sloping-eady-layer)
    - [Finite-depth Eady dispersion relation](hydrodynamic-stability.md#finite-depth-eady-dispersion-relation)
    - [Semi-infinite Eady model](hydrodynamic-stability.md#semi-infinite-eady-model)
      - [Absence of exponential instability in the semi-infinite Eady model](hydrodynamic-stability.md#absence-of-exponential-instability-in-the-semi-infinite-eady-model)
      - [Semi-infinite Eady edge wave](hydrodynamic-stability.md#semi-infinite-eady-edge-wave)
        - [Dispersion relation of a semi-infinite Eady edge wave](hydrodynamic-stability.md#dispersion-relation-of-a-semi-infinite-eady-edge-wave)
          - [Steering height of a semi-infinite Eady edge wave](hydrodynamic-stability.md#steering-height-of-a-semi-infinite-eady-edge-wave)
        - [Decaying vertical structure of a semi-infinite Eady edge wave](hydrodynamic-stability.md#decaying-vertical-structure-of-a-semi-infinite-eady-edge-wave)
    - [Eady model with a sloping lower boundary](hydrodynamic-stability.md#eady-model-with-a-sloping-lower-boundary)
      - [Instability for negative slopes in the sloping-boundary Eady model](hydrodynamic-stability.md#instability-for-negative-slopes-in-the-sloping-boundary-eady-model)
    - [Eady instability](hydrodynamic-stability.md#eady-instability)
    - [Boundary Rossby wave](hydrodynamic-stability.md#boundary-rossby-wave)
      - [Eady edge wave](hydrodynamic-stability.md#eady-edge-wave)
        - [Forced Eady edge wave](hydrodynamic-stability.md#forced-eady-edge-wave)
        - [Sloping-boundary Eady edge wave](hydrodynamic-stability.md#sloping-boundary-eady-edge-wave)
      - [Quasi-geostrophic wave at a stratification interface](hydrodynamic-stability.md#quasi-geostrophic-wave-at-a-stratification-interface)
    - [Damped Eady-wave dispersion relation](hydrodynamic-stability.md#damped-eady-wave-dispersion-relation)
  - [Dissipation-induced instability](hydrodynamic-stability.md#dissipation-induced-instability)
  - [Rayleigh discriminant](hydrodynamic-stability.md#rayleigh-discriminant)
    - [Rayleigh's circulation criterion](hydrodynamic-stability.md#rayleigh-s-circulation-criterion)
- [Barotropic fluid](#barotropic-fluid)
  - [Barotropic cylindrical rotation theorem](#barotropic-cylindrical-rotation-theorem)
  - [Barotropic spherical accretion equation](#barotropic-spherical-accretion-equation)
    - [Polytropic accretion in a mixed inverse-power potential](#polytropic-accretion-in-a-mixed-inverse-power-potential)
    - [Critical-point slope of barotropic spherical accretion](#critical-point-slope-of-barotropic-spherical-accretion)
  - [Barotropic enthalpy function](#barotropic-enthalpy-function)
  - [Centrifugal potential of cylindrical rotation](#centrifugal-potential-of-cylindrical-rotation)
  - [Barotropic energy density](#barotropic-energy-density)
  - [Barotropic magnetic energy equation](#barotropic-magnetic-energy-equation)
  - [Barotropic vorticity transport](#barotropic-vorticity-transport)
- [Shear flow](#shear-flow)
  - [Renovating shear flow](#renovating-shear-flow)
    - [Mean logarithmic stretching in an isotropic renovating shear](#mean-logarithmic-stretching-in-an-isotropic-renovating-shear)
      - [Log-stretch fluctuations in an isotropic renovating shear](#log-stretch-fluctuations-in-an-isotropic-renovating-shear)
  - [Linear shear flow](#linear-shear-flow)
- [Lagrangian displacement (fluid mechanics)](#lagrangian-displacement-fluid-mechanics)
  - [Eulerian perturbation of a fluid variable](#eulerian-perturbation-of-a-fluid-variable)
  - [Lagrangian perturbation of a fluid variable](#lagrangian-perturbation-of-a-fluid-variable)
    - [Adiabatic fluid perturbation](#adiabatic-fluid-perturbation)
- [Eulerian and Lagrangian fluid perturbations](#eulerian-and-lagrangian-fluid-perturbations)
  - [Eulerian fluid perturbation](#eulerian-fluid-perturbation)
  - [Surface density perturbation of a displaced uniform interface](#surface-density-perturbation-of-a-displaced-uniform-interface)
  - [Lagrangian pressure perturbation](#lagrangian-pressure-perturbation)
- [Torricelli's law](#torricelli-s-law)
  - [Drainage time of a conical tank](#drainage-time-of-a-conical-tank)
- [Density](#density)
  - [Gas clumping factor](#gas-clumping-factor)
  - [Projected surface mass density](#projected-surface-mass-density)
- [Fluid pressure](#fluid-pressure)
  - [Cavitation](#cavitation)
  - [Pressure gradient](#pressure-gradient)
- [Drag (physics)](#drag-physics)
  - [Linear drag](#linear-drag)
    - [Overdamped particle dynamics](#overdamped-particle-dynamics)
    - [Linear friction coefficient](#linear-friction-coefficient)
    - [Vertical ascent under linear drag](#vertical-ascent-under-linear-drag)
  - [Drag coefficient](#drag-coefficient)
  - [Quadratic drag](#quadratic-drag)
    - [Descent from rest under quadratic drag](#descent-from-rest-under-quadratic-drag)
    - [Quadratic-drag turning angle](#quadratic-drag-turning-angle)
      - [Mass per drag area](#mass-per-drag-area)
    - [Quadratic damping](#quadratic-damping)
  - [Pressure drag](#pressure-drag)
  - [Stokes number](#stokes-number)
  - [Gas drag](#gas-drag)
  - [Aerodynamic stopping time](#aerodynamic-stopping-time)
- [Suspension (chemistry)](#suspension-chemistry)
  - [Density inversion in a settling suspension](#density-inversion-in-a-settling-suspension)
  - [Heated particle-laden layer](#heated-particle-laden-layer)
  - [Particle volume fraction](#particle-volume-fraction)
  - [Bidisperse particle suspension](#bidisperse-particle-suspension)
    - [Composition wave in a bidisperse suspension](#composition-wave-in-a-bidisperse-suspension)
  - [Settling velocity](#settling-velocity)
    - [Settling-velocity radius scaling](#settling-velocity-radius-scaling)
    - [Particle Reynolds number](#particle-reynolds-number)
    - [Particle deposition flux](#particle-deposition-flux)
    - [Stokes settling velocity](#stokes-settling-velocity)
    - [Hindered settling](#hindered-settling)
      - [Kinematic sedimentation](#kinematic-sedimentation)
        - [Hindered-settling flux inflection](#hindered-settling-flux-inflection)
        - [Bidisperse kinematic sedimentation](#bidisperse-kinematic-sedimentation)
          - [Two-stage bidisperse batch sedimentation](#two-stage-bidisperse-batch-sedimentation)
          - [Deposit composition from sedimentation jump conditions](#deposit-composition-from-sedimentation-jump-conditions)
        - [Sedimentation shock](#sedimentation-shock)
        - [Sediment mass determines final deposit thickness](#sediment-mass-determines-final-deposit-thickness)
        - [Two-layer sedimentation with a compression shock](#two-layer-sedimentation-with-a-compression-shock)
          - [Triple-shock sedimentation point](#triple-shock-sedimentation-point)
        - [Quadratic hindered-settling flux](#quadratic-hindered-settling-flux)
          - [Parabolic-profile sedimentation shock](#parabolic-profile-sedimentation-shock)
          - [Settling rarefaction fan](#settling-rarefaction-fan)
            - [Early extinction of a settling rarefaction fan](#early-extinction-of-a-settling-rarefaction-fan)
            - [Curved settling fronts within a rarefaction fan](#curved-settling-fronts-within-a-rarefaction-fan)
              - [Last surviving characteristic of a settling fan](#last-surviving-characteristic-of-a-settling-fan)
          - [Settling shock speed](#settling-shock-speed)
- [Dynamic viscosity](#dynamic-viscosity)
  - [Zero-shear viscosity](#zero-shear-viscosity)
  - [Kinematic viscosity](#kinematic-viscosity)
    - [Density-weighted mean kinematic viscosity](#density-weighted-mean-kinematic-viscosity)
    - [Density-weighted viscosity of a disk](#density-weighted-viscosity-of-a-disk)
  - [Viscous stress tensor](#viscous-stress-tensor)
  - [Reynolds number](#reynolds-number)
- [Mass diffusivity](#mass-diffusivity)
- [Vorticity](#vorticity)
  - [Vortex line](#vortex-line)
  - [Vortex (fluid mechanics)](#vortex-fluid-mechanics)
    - [Vortex dynamics](#vortex-dynamics)
      - [Nonrotating layerwise-two-dimensional vortex dynamics](#nonrotating-layerwise-two-dimensional-vortex-dynamics)
      - [Two-dimensional vortex dynamics](#two-dimensional-vortex-dynamics)
        - [Steady planar vorticity as a local function of stream function](#steady-planar-vorticity-as-a-local-function-of-stream-function)
    - [Line vortex](#line-vortex)
      - [Motion of two point vortices](#motion-of-two-point-vortices)
      - [Image vortex at a plane wall](#image-vortex-at-a-plane-wall)
        - [Line-vortex trajectory in a quarter-plane](#line-vortex-trajectory-in-a-quarter-plane)
  - [Hydrodynamic Biot-Savart kernel](#hydrodynamic-biot-savart-kernel)
  - [Hydrodynamic impulse](#hydrodynamic-impulse)
    - [Dipolar velocity field of a localized eddy](#dipolar-velocity-field-of-a-localized-eddy)
  - [Vortex tube](#vortex-tube)
  - [Enstrophy](#enstrophy)
    - [Mean enstrophy balance](#mean-enstrophy-balance)
  - [Planar vorticity velocity kernel](#planar-vorticity-velocity-kernel)
  - [Uniform-vorticity circular flow in an annulus](#uniform-vorticity-circular-flow-in-an-annulus)
  - [Vorticity cross-product identity](#vorticity-cross-product-identity)
    - [Convective acceleration identity](#convective-acceleration-identity)
  - [Hydrodynamical helicity](#hydrodynamical-helicity)
    - [Kinetic helicity density](#kinetic-helicity-density)
      - [Helicity vector of a solenoidal Fourier mode](#helicity-vector-of-a-solenoidal-fourier-mode)
      - [Kinetic helicity conservation law](#kinetic-helicity-conservation-law)
        - [Material conservation of kinetic helicity density](#material-conservation-of-kinetic-helicity-density)
  - [Absolute vorticity](#absolute-vorticity)
    - [Planetary vorticity](#planetary-vorticity)
    - [Absolute-vorticity flux tensor](#absolute-vorticity-flux-tensor)
      - [Radial vorticity conservation in a shearing sheet](#radial-vorticity-conservation-in-a-shearing-sheet)
  - [Relative vorticity](#relative-vorticity)
  - [Circulation (physics)](#circulation-physics)
    - [Kelvin's circulation theorem](#kelvin-s-circulation-theorem)
      - [Irrotational circulation in an exterior domain](#irrotational-circulation-in-an-exterior-domain)
  - [Irrotational flow](#irrotational-flow)
- [Circular vortex-sheet mode](#circular-vortex-sheet-mode)
- [Gravity wave](gravity-wave.md)
  - [Internal wave](gravity-wave.md#internal-wave)
    - [Internal-wave response of a sharp buoyancy interface](gravity-wave.md#internal-wave-response-of-a-sharp-buoyancy-interface)
    - [Pressure projection in a displaced stratified blob](gravity-wave.md#pressure-projection-in-a-displaced-stratified-blob)
    - [Finite-amplitude stationary channel internal waves](gravity-wave.md#finite-amplitude-stationary-channel-internal-waves)
    - [Internal-wave momentum deposition](gravity-wave.md#internal-wave-momentum-deposition)
      - [Boundary work and mean-flow energy of an internal wave](gravity-wave.md#boundary-work-and-mean-flow-energy-of-an-internal-wave)
    - [Energy partition of rotating internal waves](gravity-wave.md#energy-partition-of-rotating-internal-waves)
    - [Internal-wave breaking](gravity-wave.md#internal-wave-breaking)
    - [Plane internal gravity wave](gravity-wave.md#plane-internal-gravity-wave)
      - [Displacement pseudomomentum of an internal gravity wave](gravity-wave.md#displacement-pseudomomentum-of-an-internal-gravity-wave)
        - [Viscous attenuation of an internal gravity wave](gravity-wave.md#viscous-attenuation-of-an-internal-gravity-wave)
      - [Internal-wave transmission across a buoyancy-frequency jump](gravity-wave.md#internal-wave-transmission-across-a-buoyancy-frequency-jump)
        - [Internal-wave cavity response](gravity-wave.md#internal-wave-cavity-response)
      - [Monochromatic internal-wave overturning criterion](gravity-wave.md#monochromatic-internal-wave-overturning-criterion)
    - [Dispersion relation for interfacial gravity waves between rigid boundaries](gravity-wave.md#dispersion-relation-for-interfacial-gravity-waves-between-rigid-boundaries)
    - [Stratified internal-wave guide](gravity-wave.md#stratified-internal-wave-guide)
    - [Boundary-forced internal gravity wave](gravity-wave.md#boundary-forced-internal-gravity-wave)
      - [Slowly modulated internal-wave boundary forcing](gravity-wave.md#slowly-modulated-internal-wave-boundary-forcing)
        - [Internal-wave work in a phase-speed frame](gravity-wave.md#internal-wave-work-in-a-phase-speed-frame)
      - [Two-beam radiation from a localized oscillating boundary](gravity-wave.md#two-beam-radiation-from-a-localized-oscillating-boundary)
      - [Stationary topographic internal gravity wave](gravity-wave.md#stationary-topographic-internal-gravity-wave)
        - [Rigid-lid resonance of stationary topographic internal waves](gravity-wave.md#rigid-lid-resonance-of-stationary-topographic-internal-waves)
        - [Stationary phase of topographic internal waves](gravity-wave.md#stationary-phase-of-topographic-internal-waves)
      - [Internal-wave transmission across a stratification step](gravity-wave.md#internal-wave-transmission-across-a-stratification-step)
    - [Interfacial gravity wave](gravity-wave.md#interfacial-gravity-wave)
      - [Interfacial gravity-wave dispersion relation](gravity-wave.md#interfacial-gravity-wave-dispersion-relation)
    - [Atmospheric internal gravity wave](gravity-wave.md#atmospheric-internal-gravity-wave)
      - [Intrinsic frequency](gravity-wave.md#intrinsic-frequency)
        - [Critical level of an internal gravity wave](gravity-wave.md#critical-level-of-an-internal-gravity-wave)
          - [Wave-action criterion for critical-level overturning](gravity-wave.md#wave-action-criterion-for-critical-level-overturning)
          - [Critical-height approach of a stationary wave in linear shear](gravity-wave.md#critical-height-approach-of-a-stationary-wave-in-linear-shear)
      - [Radiation condition](gravity-wave.md#radiation-condition)
        - [Internal-wave envelope radiation condition](gravity-wave.md#internal-wave-envelope-radiation-condition)
        - [Limiting absorption principle](gravity-wave.md#limiting-absorption-principle)
      - [Wave momentum flux](gravity-wave.md#wave-momentum-flux)
      - [Taylor–Goldstein equation](gravity-wave.md#taylor-goldstein-equation)
        - [Exponential-profile stationary stratified waves](gravity-wave.md#exponential-profile-stationary-stratified-waves)
        - [Nonlinear exactness test for a stratified streamfunction mode](gravity-wave.md#nonlinear-exactness-test-for-a-stratified-streamfunction-mode)
        - [Variational group velocity of a Taylor-Goldstein mode](gravity-wave.md#variational-group-velocity-of-a-taylor-goldstein-mode)
        - [Power-transformed Taylor–Goldstein energy identity](gravity-wave.md#power-transformed-taylor-goldstein-energy-identity)
          - [Miles–Howard theorem](gravity-wave.md#miles-howard-theorem)
          - [Phase-speed bound for unstable stratified shear modes](gravity-wave.md#phase-speed-bound-for-unstable-stratified-shear-modes)
        - [Jump conditions for stratified inviscid shear flow](gravity-wave.md#jump-conditions-for-stratified-inviscid-shear-flow)
          - [Endpoint derivative map for an evanescent wave layer](gravity-wave.md#endpoint-derivative-map-for-an-evanescent-wave-layer)
          - [Gravity-vorticity interface wave](gravity-wave.md#gravity-vorticity-interface-wave)
          - [Internal-wave transmission across a velocity jump](gravity-wave.md#internal-wave-transmission-across-a-velocity-jump)
            - [Displacement impedance for an internal wave at a velocity jump](gravity-wave.md#displacement-impedance-for-an-internal-wave-at-a-velocity-jump)
          - [Dispersion relation for two density interfaces in uniform shear](gravity-wave.md#dispersion-relation-for-two-density-interfaces-in-uniform-shear)
        - [Scorer parameter](gravity-wave.md#scorer-parameter)
          - [Stationary internal-wave WKB solution](gravity-wave.md#stationary-internal-wave-wkb-solution)
          - [Vertical trapping of an atmospheric gravity wave](gravity-wave.md#vertical-trapping-of-an-atmospheric-gravity-wave)
            - [Turning level of a stationary internal wave](gravity-wave.md#turning-level-of-a-stationary-internal-wave)
            - [Turning height of a stationary wave in linear shear](gravity-wave.md#turning-height-of-a-stationary-wave-in-linear-shear)
    - [Density stratification](gravity-wave.md#density-stratification)
      - [Density gradient](gravity-wave.md#density-gradient)
      - [Halocline](gravity-wave.md#halocline)
        - [Cold halocline](gravity-wave.md#cold-halocline)
      - [Ocean mixed layer](gravity-wave.md#ocean-mixed-layer)
      - [Stable density stratification](gravity-wave.md#stable-density-stratification)
        - [Ozmidov length](gravity-wave.md#ozmidov-length)
        - [Potential-energy cost of homogenizing a linear stratification](gravity-wave.md#potential-energy-cost-of-homogenizing-a-linear-stratification)
        - [Unstable density stratification](gravity-wave.md#unstable-density-stratification)
    - [Buoyancy frequency](gravity-wave.md#buoyancy-frequency)
      - [Radial buoyancy frequency](gravity-wave.md#radial-buoyancy-frequency)
        - [Radial Solberg–Høiland instability criterion](gravity-wave.md#radial-solberg-hoiland-instability-criterion)
      - [Dry parcel buoyancy in a homogeneous atmosphere](gravity-wave.md#dry-parcel-buoyancy-in-a-homogeneous-atmosphere)
      - [Richardson number](gravity-wave.md#richardson-number)
        - [Flux Richardson number](gravity-wave.md#flux-richardson-number)
          - [Buoyancy fraction of total turbulent sinks](gravity-wave.md#buoyancy-fraction-of-total-turbulent-sinks)
        - [Interfacial Richardson number](gravity-wave.md#interfacial-richardson-number)
          - [Entrainment exponent from a local interfacial Richardson closure](gravity-wave.md#entrainment-exponent-from-a-local-interfacial-richardson-closure)
        - [Bulk Richardson number](gravity-wave.md#bulk-richardson-number)
        - [Gradient Richardson number](gravity-wave.md#gradient-richardson-number)
      - [Stellar buoyancy frequency](gravity-wave.md#stellar-buoyancy-frequency)
    - [Internal-wave phase and group velocity](gravity-wave.md#internal-wave-phase-and-group-velocity)
      - [Right-triangle geometry of internal-wave velocities](gravity-wave.md#right-triangle-geometry-of-internal-wave-velocities)
      - [Internal-wave polarization](gravity-wave.md#internal-wave-polarization)
        - [Buoyancy polarization of a plane internal gravity wave](gravity-wave.md#buoyancy-polarization-of-a-plane-internal-gravity-wave)
      - [Constant-phase line of an internal gravity wave](gravity-wave.md#constant-phase-line-of-an-internal-gravity-wave)
    - [Reflection of an internal-wave ray](gravity-wave.md#reflection-of-an-internal-wave-ray)
      - [Internal-wave slope criticality](gravity-wave.md#internal-wave-slope-criticality)
        - [Subcritical internal-wave reflection](gravity-wave.md#subcritical-internal-wave-reflection)
        - [Critical internal-wave reflection](gravity-wave.md#critical-internal-wave-reflection)
      - [Topographic sideband of an internal gravity wave](gravity-wave.md#topographic-sideband-of-an-internal-gravity-wave)
      - [Internal-wave ray tracing](gravity-wave.md#internal-wave-ray-tracing)
        - [Internal-wave ray in uniform vertical shear](gravity-wave.md#internal-wave-ray-in-uniform-vertical-shear)
          - [Circular mountain-wave ray in linear shear](gravity-wave.md#circular-mountain-wave-ray-in-linear-shear)
        - [Internal-wave attractor](gravity-wave.md#internal-wave-attractor)
          - [Internal-wave ray return map](gravity-wave.md#internal-wave-ray-return-map)
        - [Double-zero internal-wave turning level](gravity-wave.md#double-zero-internal-wave-turning-level)
        - [Causal envelope of stationary internal waves](gravity-wave.md#causal-envelope-of-stationary-internal-waves)
          - [Refraction of a stationary internal-wave causal envelope](gravity-wave.md#refraction-of-a-stationary-internal-wave-causal-envelope)
          - [First arrival of a stationary internal wavefront at a layer boundary](gravity-wave.md#first-arrival-of-a-stationary-internal-wavefront-at-a-layer-boundary)
      - [Focusing power of internal-wave reflection](gravity-wave.md#focusing-power-of-internal-wave-reflection)
    - [Viscous attenuation of an internal-wave beam](gravity-wave.md#viscous-attenuation-of-an-internal-wave-beam)
      - [Oscillatory drift of an attenuated internal-wave beam](gravity-wave.md#oscillatory-drift-of-an-attenuated-internal-wave-beam)
    - [Vertical trapping of an internal gravity wave by planar strain](gravity-wave.md#vertical-trapping-of-an-internal-gravity-wave-by-planar-strain)
    - [Mountain-wave cutoff](gravity-wave.md#mountain-wave-cutoff)
- [Stream function](#stream-function)
  - [Sinusoidal cellular flow](#sinusoidal-cellular-flow)
    - [Melnikov splitting of a periodically perturbed cellular flow](#melnikov-splitting-of-a-periodically-perturbed-cellular-flow)
  - [Linear planar strain and rotation streamlines](#linear-planar-strain-and-rotation-streamlines)
  - [Axisymmetric hydrodynamic mass flux function](#axisymmetric-hydrodynamic-mass-flux-function)
  - [Stokes streamfunction](#stokes-streamfunction)
  - [Streamline classification of a planar linear saddle or centre](#streamline-classification-of-a-planar-linear-saddle-or-centre)
    - [Linear planar flow with strain and rotation](#linear-planar-flow-with-strain-and-rotation)
- [Streamline](#streamline)
  - [Stream tube](#stream-tube)
- [Velocity potential](#velocity-potential)
  - [Potential flow around a circular cylinder](#potential-flow-around-a-circular-cylinder)
    - [Potential flow around a circular cylinder with circulation](#potential-flow-around-a-circular-cylinder-with-circulation)
      - [Kutta–Joukowski theorem](#kutta-joukowski-theorem)
        - [Advective and pressure contributions to circulatory lift](#advective-and-pressure-contributions-to-circulatory-lift)
  - [Radially symmetric incompressible flow in a planar annulus](#radially-symmetric-incompressible-flow-in-a-planar-annulus)
    - [Pressure in radially symmetric annular potential flow](#pressure-in-radially-symmetric-annular-potential-flow)
      - [Small oscillation of a planar gas bubble in an annular liquid](#small-oscillation-of-a-planar-gas-bubble-in-an-annular-liquid)
- [Plume (fluid dynamics)](#plume-fluid-dynamics)
  - [Laminar plume](#laminar-plume)
    - [Integral momentum-flux balance for a two-dimensional plume](#integral-momentum-flux-balance-for-a-two-dimensional-plume)
    - [Similarity scaling of a two-dimensional laminar plume](#similarity-scaling-of-a-two-dimensional-laminar-plume)
      - [Similarity equation for a two-dimensional laminar plume](#similarity-equation-for-a-two-dimensional-laminar-plume)
- [Euler equations for an inviscid fluid](#euler-equations-for-an-inviscid-fluid)
  - [Linearized Euler equations](#linearized-euler-equations)
  - [Conservative energy flux of a polytropic ideal gas](#conservative-energy-flux-of-a-polytropic-ideal-gas)
  - [Crocco form of the unsteady Euler equation](#crocco-form-of-the-unsteady-euler-equation)
  - [Yudovich characteristic flow](#yudovich-characteristic-flow)
  - [Bernoulli's principle](#bernoulli-s-principle)
    - [Venturi effect](#venturi-effect)
  - [Axisymmetric inviscid flow between moving parallel plates](#axisymmetric-inviscid-flow-between-moving-parallel-plates)
  - [Radial velocity](#radial-velocity)
  - [Unsteady Bernoulli equation](#unsteady-bernoulli-equation)
    - [Constant-tension balloon discharge](#constant-tension-balloon-discharge)
    - [Inviscid startup in a pressure-driven tube](#inviscid-startup-in-a-pressure-driven-tube)
    - [Linearly elastic balloon discharge](#linearly-elastic-balloon-discharge)
  - [Clebsch-potential variational derivation of incompressible Euler flow](#clebsch-potential-variational-derivation-of-incompressible-euler-flow)
  - [Bernoulli equation](#bernoulli-equation)
    - [Bernoulli invariant](#bernoulli-invariant)
    - [Hydraulic control over a smooth hump](#hydraulic-control-over-a-smooth-hump)
    - [Bernoulli function for planar constant-vorticity flow](#bernoulli-function-for-planar-constant-vorticity-flow)
    - [Steady rotating-frame Bernoulli integral](#steady-rotating-frame-bernoulli-integral)
    - [Bernoulli function](#bernoulli-function)
    - [Bernoulli equation over topography](#bernoulli-equation-over-topography)
    - [Draining time of a uniform tank through a siphon](#draining-time-of-a-uniform-tank-through-a-siphon)
  - [Integral momentum equation](#integral-momentum-equation)
    - [Holding force on a contracting nozzle](#holding-force-on-a-contracting-nozzle)
    - [Force on a pipe junction](#force-on-a-pipe-junction)
- [Conservation of mass in a pipe](#conservation-of-mass-in-a-pipe)
- [Viscous fluid flow](viscous-fluid-flow.md)
  - [Euler limit](viscous-fluid-flow.md#euler-limit)
    - [Inviscid core](viscous-fluid-flow.md#inviscid-core)
  - [Pressure-driven channel flow](viscous-fluid-flow.md#pressure-driven-channel-flow)
    - [Corner expansion of pressure-driven sector flow](viscous-fluid-flow.md#corner-expansion-of-pressure-driven-sector-flow)
  - [Plane Poiseuille flow](viscous-fluid-flow.md#plane-poiseuille-flow)
    - [Symmetric viscous interaction in an indented Poiseuille channel](viscous-fluid-flow.md#symmetric-viscous-interaction-in-an-indented-poiseuille-channel)
      - [One-third-power similarity of an indented channel boundary layer](viscous-fluid-flow.md#one-third-power-similarity-of-an-indented-channel-boundary-layer)
    - [Two-layer plane Poiseuille flow with unequal viscosities](viscous-fluid-flow.md#two-layer-plane-poiseuille-flow-with-unequal-viscosities)
  - [Fully developed flow](viscous-fluid-flow.md#fully-developed-flow)
  - [Velocity profile](viscous-fluid-flow.md#velocity-profile)
  - [Viscous boundary layer](viscous-fluid-flow.md#viscous-boundary-layer)
    - [Prandtl limit](viscous-fluid-flow.md#prandtl-limit)
    - [Prandtl boundary-layer equation](viscous-fluid-flow.md#prandtl-boundary-layer-equation)
      - [Blasius equation](viscous-fluid-flow.md#blasius-equation)
      - [Unsteady Prandtl equation](viscous-fluid-flow.md#unsteady-prandtl-equation)
        - [Linearized unsteady Prandtl equation](viscous-fluid-flow.md#linearized-unsteady-prandtl-equation)
          - [Prandtl normal-mode equation](viscous-fluid-flow.md#prandtl-normal-mode-equation)
    - [Boundary-layer thickness from an advection-diffusion balance](viscous-fluid-flow.md#boundary-layer-thickness-from-an-advection-diffusion-balance)
  - [Viscous diffusion time](viscous-fluid-flow.md#viscous-diffusion-time)
  - [Couette flow](viscous-fluid-flow.md#couette-flow)
    - [Couette-Poiseuille flow](viscous-fluid-flow.md#couette-poiseuille-flow)
    - [Zero-flux Couette-Poiseuille flow](viscous-fluid-flow.md#zero-flux-couette-poiseuille-flow)
    - [Two-layer Couette flow](viscous-fluid-flow.md#two-layer-couette-flow)
  - [Falling film flow](viscous-fluid-flow.md#falling-film-flow)
    - [Two-layer falling film of equal-density viscous fluids](viscous-fluid-flow.md#two-layer-falling-film-of-equal-density-viscous-fluids)
    - [Residual wall films in a receding gravity current](viscous-fluid-flow.md#residual-wall-films-in-a-receding-gravity-current)
    - [Inclined viscous film with opposing surface shear](viscous-fluid-flow.md#inclined-viscous-film-with-opposing-surface-shear)
  - [Stress boundary condition](viscous-fluid-flow.md#stress-boundary-condition)
    - [Stress-free boundary condition](viscous-fluid-flow.md#stress-free-boundary-condition)
    - [No-penetration boundary condition](viscous-fluid-flow.md#no-penetration-boundary-condition)
  - [No-slip boundary condition](viscous-fluid-flow.md#no-slip-boundary-condition)
    - [Pressure compatibility at a no-slip wall](viscous-fluid-flow.md#pressure-compatibility-at-a-no-slip-wall)
    - [Taylor-expanded no-slip boundary condition](viscous-fluid-flow.md#taylor-expanded-no-slip-boundary-condition)
  - [Newtonian fluid](viscous-fluid-flow.md#newtonian-fluid)
    - [Newtonian fluid stress tensor](viscous-fluid-flow.md#newtonian-fluid-stress-tensor)
      - [Shear stress](viscous-fluid-flow.md#shear-stress)
        - [Shear velocity](viscous-fluid-flow.md#shear-velocity)
      - [Strain-rate tensor](viscous-fluid-flow.md#strain-rate-tensor)
        - [Principal strain rates](viscous-fluid-flow.md#principal-strain-rates)
          - [Bi-axial strain](viscous-fluid-flow.md#bi-axial-strain)
        - [Shear rate](viscous-fluid-flow.md#shear-rate)
          - [Simple shear flow](viscous-fluid-flow.md#simple-shear-flow)
        - [Spin tensor](viscous-fluid-flow.md#spin-tensor)
      - [Polar shear stress in a Newtonian fluid](viscous-fluid-flow.md#polar-shear-stress-in-a-newtonian-fluid)
  - [Navier-Stokes equation](viscous-fluid-flow.md#navier-stokes-equation)
    - [Pressure Poisson equation for incompressible flow](viscous-fluid-flow.md#pressure-poisson-equation-for-incompressible-flow)
      - [Long-range pressure correlations in turbulence](viscous-fluid-flow.md#long-range-pressure-correlations-in-turbulence)
    - [Leray-Helmholtz projection](viscous-fluid-flow.md#leray-helmholtz-projection)
    - [Stokes operator](viscous-fluid-flow.md#stokes-operator)
      - [Spectral projection of the Stokes operator](viscous-fluid-flow.md#spectral-projection-of-the-stokes-operator)
    - [Skew-symmetry of incompressible transport](viscous-fluid-flow.md#skew-symmetry-of-incompressible-transport)
      - [Skew-symmetrized transport form](viscous-fluid-flow.md#skew-symmetrized-transport-form)
    - [Navier-Stokes equation with spectrally truncated advection](viscous-fluid-flow.md#navier-stokes-equation-with-spectrally-truncated-advection)
    - [Steady skew-symmetrized Navier-Stokes equation](viscous-fluid-flow.md#steady-skew-symmetrized-navier-stokes-equation)
    - [Rayleigh-Bénard convection](viscous-fluid-flow.md#rayleigh-benard-convection)
      - [Four-thirds convective heat-transfer law](viscous-fluid-flow.md#four-thirds-convective-heat-transfer-law)
        - [Convective cooling under the four-thirds heat-transfer law](viscous-fluid-flow.md#convective-cooling-under-the-four-thirds-heat-transfer-law)
      - [Stress-free convection growth-rate polynomial](viscous-fluid-flow.md#stress-free-convection-growth-rate-polynomial)
        - [Exchange of stabilities in stress-free convection](viscous-fluid-flow.md#exchange-of-stabilities-in-stress-free-convection)
      - [Thermal-diffusion scaling of a convection layer](viscous-fluid-flow.md#thermal-diffusion-scaling-of-a-convection-layer)
      - [Conductive state of Rayleigh-Bénard convection](viscous-fluid-flow.md#conductive-state-of-rayleigh-benard-convection)
      - [Rotating Rayleigh-Bénard convection](viscous-fluid-flow.md#rotating-rayleigh-benard-convection)
        - [Five-mode rotating-convection truncation](viscous-fluid-flow.md#five-mode-rotating-convection-truncation)
        - [Counterpropagating Hopf amplitudes in rotating convection](viscous-fluid-flow.md#counterpropagating-hopf-amplitudes-in-rotating-convection)
        - [Weakly nonlinear rotating-convection roll stability](viscous-fluid-flow.md#weakly-nonlinear-rotating-convection-roll-stability)
          - [Small-angle instability of rotating convection rolls](viscous-fluid-flow.md#small-angle-instability-of-rotating-convection-rolls)
          - [Küppers–Lortz instability](viscous-fluid-flow.md#kuppers-lortz-instability)
        - [Wavenumber selection in rotating convection](viscous-fluid-flow.md#wavenumber-selection-in-rotating-convection)
        - [Rotating-convection growth-rate polynomial](viscous-fluid-flow.md#rotating-convection-growth-rate-polynomial)
          - [Oscillatory neutral curve of rotating convection](viscous-fluid-flow.md#oscillatory-neutral-curve-of-rotating-convection)
          - [Stationary neutral curve of rotating convection](viscous-fluid-flow.md#stationary-neutral-curve-of-rotating-convection)
      - [Free-slip convection neutral curve](viscous-fluid-flow.md#free-slip-convection-neutral-curve)
      - [Infinite-Prandtl-number convection](viscous-fluid-flow.md#infinite-prandtl-number-convection)
        - [Fastest growth in infinite-Prandtl convection](viscous-fluid-flow.md#fastest-growth-in-infinite-prandtl-convection)
        - [Stokes temperature-slaving operator](viscous-fluid-flow.md#stokes-temperature-slaving-operator)
    - [Damped-driven Navier-Stokes equation](viscous-fluid-flow.md#damped-driven-navier-stokes-equation)
      - [Damped-vorticity maximum estimate](viscous-fluid-flow.md#damped-vorticity-maximum-estimate)
      - [Vanishing-viscosity limit](viscous-fluid-flow.md#vanishing-viscosity-limit)
  - [Pipe flow](viscous-fluid-flow.md#pipe-flow)
    - [Hagen-Poiseuille equation](viscous-fluid-flow.md#hagen-poiseuille-equation)
  - [Kinetic-energy balance for an incompressible Newtonian fluid](viscous-fluid-flow.md#kinetic-energy-balance-for-an-incompressible-newtonian-fluid)
    - [Dissipation estimate for high-Reynolds-number bubble drag](viscous-fluid-flow.md#dissipation-estimate-for-high-reynolds-number-bubble-drag)
      - [Drag on a two-dimensional circular bubble from outer-flow dissipation](viscous-fluid-flow.md#drag-on-a-two-dimensional-circular-bubble-from-outer-flow-dissipation)
  - [Stokes flow](stokes-flow.md)
    - [Relaxation of a symmetric viscous layer](stokes-flow.md#relaxation-of-a-symmetric-viscous-layer)
      - [Uniform high-viscosity limit of viscous-layer relaxation](stokes-flow.md#uniform-high-viscosity-limit-of-viscous-layer-relaxation)
    - [Fourier traction map for a viscous half-space](stokes-flow.md#fourier-traction-map-for-a-viscous-half-space)
    - [Stokes far-field multipoles of a deforming body](stokes-flow.md#stokes-far-field-multipoles-of-a-deforming-body)
    - [Mutual drag reduction of two distant translating spheres](stokes-flow.md#mutual-drag-reduction-of-two-distant-translating-spheres)
    - [Oseen approximation](stokes-flow.md#oseen-approximation)
      - [Potential-source and wake decomposition of sphere Oseen flow](stokes-flow.md#potential-source-and-wake-decomposition-of-sphere-oseen-flow)
    - [Cylinder in a simple shear Stokes flow](stokes-flow.md#cylinder-in-a-simple-shear-stokes-flow)
    - [Zero total flux for localized tube Stokes flow](stokes-flow.md#zero-total-flux-for-localized-tube-stokes-flow)
    - [Surface independence of Stokes force and torque integrals](stokes-flow.md#surface-independence-of-stokes-force-and-torque-integrals)
    - [Brinkman equation](stokes-flow.md#brinkman-equation)
      - [Matrix-relative Brinkman velocity](stokes-flow.md#matrix-relative-brinkman-velocity)
    - [Viscous buoyant conduit](stokes-flow.md#viscous-buoyant-conduit)
      - [Conduit equation](stokes-flow.md#conduit-equation)
        - [Solitary-wave amplitude-speed relation for the conduit equation](stokes-flow.md#solitary-wave-amplitude-speed-relation-for-the-conduit-equation)
    - [Hydrodynamic interaction](stokes-flow.md#hydrodynamic-interaction)
      - [Stresslet reflection between two force-free and forced spheres](stokes-flow.md#stresslet-reflection-between-two-force-free-and-forced-spheres)
        - [Rotation-clamped reflection between two spheres](stokes-flow.md#rotation-clamped-reflection-between-two-spheres)
      - [Externally driven two-sphere pump](stokes-flow.md#externally-driven-two-sphere-pump)
        - [Minimum separation of phase-shifted sphere oscillations](stokes-flow.md#minimum-separation-of-phase-shifted-sphere-oscillations)
        - [Phase-dependent mean force of an externally driven sphere pair](stokes-flow.md#phase-dependent-mean-force-of-an-externally-driven-sphere-pair)
      - [Longitudinal two-sphere mobility](stokes-flow.md#longitudinal-two-sphere-mobility)
    - [Particle stresslet tensor](stokes-flow.md#particle-stresslet-tensor)
    - [Sphere in a uniform straining Stokes flow](stokes-flow.md#sphere-in-a-uniform-straining-stokes-flow)
      - [Papkovich potentials for a strained sphere](stokes-flow.md#papkovich-potentials-for-a-strained-sphere)
    - [Stokes equation](stokes-flow.md#stokes-equation)
    - [Linearity of Stokes flow](stokes-flow.md#linearity-of-stokes-flow)
    - [Uniqueness of Stokes flow](stokes-flow.md#uniqueness-of-stokes-flow)
    - [Pressure-driven thinning of a uniform Stokes layer](stokes-flow.md#pressure-driven-thinning-of-a-uniform-stokes-layer)
    - [Stokeslet](stokes-flow.md#stokeslet)
      - [No-slip image system of a normal Stokeslet](stokes-flow.md#no-slip-image-system-of-a-normal-stokeslet)
      - [Stress-free image of a normal Stokeslet](stokes-flow.md#stress-free-image-of-a-normal-stokeslet)
      - [Rate of strain and vorticity of a Stokeslet](stokes-flow.md#rate-of-strain-and-vorticity-of-a-stokeslet)
      - [Normal Stokeslet below a stress-free plane](stokes-flow.md#normal-stokeslet-below-a-stress-free-plane)
    - [Slender-body theory](stokes-flow.md#slender-body-theory)
      - [Straight-rod resistance in a linear flow](stokes-flow.md#straight-rod-resistance-in-a-linear-flow)
        - [Force-free straight-rod orientation equation](stokes-flow.md#force-free-straight-rod-orientation-equation)
          - [Rod excess dissipation in shear](stokes-flow.md#rod-excess-dissipation-in-shear)
      - [Slender-body force density](stokes-flow.md#slender-body-force-density)
        - [Right-angle two-rod resistance matrix](stokes-flow.md#right-angle-two-rod-resistance-matrix)
          - [Sedimentation drift of a weighted two-rod body](stokes-flow.md#sedimentation-drift-of-a-weighted-two-rod-body)
        - [Axial resistance matrix of a slender helix](stokes-flow.md#axial-resistance-matrix-of-a-slender-helix)
          - [Axial coupling of an elliptic helix](stokes-flow.md#axial-coupling-of-an-elliptic-helix)
          - [Determinant of helical resistance in resistive-force theory](stokes-flow.md#determinant-of-helical-resistance-in-resistive-force-theory)
          - [Handedness reversal of helical hydrodynamic resistance](stokes-flow.md#handedness-reversal-of-helical-hydrodynamic-resistance)
    - [Hydrodynamic resistance matrix](stokes-flow.md#hydrodynamic-resistance-matrix)
      - [Hydrodynamic mobility matrix](stokes-flow.md#hydrodynamic-mobility-matrix)
      - [Symmetry and positivity of a rigid-body resistance matrix](stokes-flow.md#symmetry-and-positivity-of-a-rigid-body-resistance-matrix)
    - [Lorentz reciprocal theorem for Stokes flow](stokes-flow.md#lorentz-reciprocal-theorem-for-stokes-flow)
      - [Body-force-driven rotation of a torque-free sphere](stokes-flow.md#body-force-driven-rotation-of-a-torque-free-sphere)
      - [Boundary integral representation of Stokes flow](stokes-flow.md#boundary-integral-representation-of-stokes-flow)
        - [Capillary boundary integral equation for a viscous drop](stokes-flow.md#capillary-boundary-integral-equation-for-a-viscous-drop)
    - [Viscous dissipation](stokes-flow.md#viscous-dissipation)
      - [Turbulent kinetic energy dissipation rate](stokes-flow.md#turbulent-kinetic-energy-dissipation-rate)
      - [Minimum-dissipation theorem for Stokes flow](stokes-flow.md#minimum-dissipation-theorem-for-stokes-flow)
        - [Extra dissipation due to a rigid inclusion](stokes-flow.md#extra-dissipation-due-to-a-rigid-inclusion)
          - [Force-free inclusions increase rotational resistance](stokes-flow.md#force-free-inclusions-increase-rotational-resistance)
          - [Einstein viscosity formula for a dilute suspension](stokes-flow.md#einstein-viscosity-formula-for-a-dilute-suspension)
        - [Fixed-force comparison of minimum viscous dissipation](stokes-flow.md#fixed-force-comparison-of-minimum-viscous-dissipation)
          - [Force-free inclusion reduces axial mobility of a centred settling sphere](stokes-flow.md#force-free-inclusion-reduces-axial-mobility-of-a-centred-settling-sphere)
    - [Biharmonic stream function for planar Stokes flow](stokes-flow.md#biharmonic-stream-function-for-planar-stokes-flow)
      - [Zero-mean normal velocity in periodic half-space Stokes flow](stokes-flow.md#zero-mean-normal-velocity-in-periodic-half-space-stokes-flow)
      - [Similarity solution for tangentially forced Stokes wedge](stokes-flow.md#similarity-solution-for-tangentially-forced-stokes-wedge)
      - [Stokes flow between touching counter-rotating cylinders](stokes-flow.md#stokes-flow-between-touching-counter-rotating-cylinders)
      - [Biharmonic stream function for a fixed disk in planar shear](stokes-flow.md#biharmonic-stream-function-for-a-fixed-disk-in-planar-shear)
        - [Hydrodynamic torque on a fixed disk in planar shear](stokes-flow.md#hydrodynamic-torque-on-a-fixed-disk-in-planar-shear)
    - [Harmonic pressure and vorticity in Stokes flow](stokes-flow.md#harmonic-pressure-and-vorticity-in-stokes-flow)
    - [Velocity gradient of translating-sphere Stokes flow](stokes-flow.md#velocity-gradient-of-translating-sphere-stokes-flow)
    - [Vorticity of translating-sphere Stokes flow](stokes-flow.md#vorticity-of-translating-sphere-stokes-flow)
    - [Harmonicity of derivatives of the Newtonian potential](stokes-flow.md#harmonicity-of-derivatives-of-the-newtonian-potential)
    - [Direct incompressibility check for translating-sphere flow](stokes-flow.md#direct-incompressibility-check-for-translating-sphere-flow)
    - [Surface traction in translating-sphere Stokes flow](stokes-flow.md#surface-traction-in-translating-sphere-stokes-flow)
      - [Stokes's law](stokes-flow.md#stokes-s-law)
        - [Clean-bubble Stokes drag](stokes-flow.md#clean-bubble-stokes-drag)
          - [Bubble rise near a distant stress-free free surface](stokes-flow.md#bubble-rise-near-a-distant-stress-free-free-surface)
          - [Spherical clean bubble without surface tension](stokes-flow.md#spherical-clean-bubble-without-surface-tension)
        - [Stokes–Einstein relation](stokes-flow.md#stokes-einstein-relation)
    - [Kinematic reversibility of Stokes flow](stokes-flow.md#kinematic-reversibility-of-stokes-flow)
      - [Reflection symmetry of a two-sphere passing trajectory](stokes-flow.md#reflection-symmetry-of-a-two-sphere-passing-trajectory)
      - [No lateral migration of a single sphere in a uniform tube in Stokes flow](stokes-flow.md#no-lateral-migration-of-a-single-sphere-in-a-uniform-tube-in-stokes-flow)
      - [Fore-aft symmetry of a sedimenting-sphere encounter](stokes-flow.md#fore-aft-symmetry-of-a-sedimenting-sphere-encounter)
      - [Scallop theorem](stokes-flow.md#scallop-theorem)
        - [Force-free two-sphere stroke](stokes-flow.md#force-free-two-sphere-stroke)
      - [Reflection argument for zero Stokes migration](stokes-flow.md#reflection-argument-for-zero-stokes-migration)
    - [Rotational Stokes flow between concentric spheres](stokes-flow.md#rotational-stokes-flow-between-concentric-spheres)
      - [Torque in rotational Stokes flow between concentric spheres](stokes-flow.md#torque-in-rotational-stokes-flow-between-concentric-spheres)
    - [Papkovich–Neuber representation](stokes-flow.md#papkovich-neuber-representation)
      - [Unscaled Papkovich–Neuber representation](stokes-flow.md#unscaled-papkovich-neuber-representation)
        - [Traction of translating-sphere Papkovich–Neuber potentials](stokes-flow.md#traction-of-translating-sphere-papkovich-neuber-potentials)
    - [Rotating sphere in Stokes flow](stokes-flow.md#rotating-sphere-in-stokes-flow)
      - [Rotlet](stokes-flow.md#rotlet)
        - [Rotlet dipole](stokes-flow.md#rotlet-dipole)
          - [Free-surface image of a rotlet dipole](stokes-flow.md#free-surface-image-of-a-rotlet-dipole)
            - [Surface-induced yaw of a rotlet dipole](stokes-flow.md#surface-induced-yaw-of-a-rotlet-dipole)
    - [Translating sphere in Stokes flow](stokes-flow.md#translating-sphere-in-stokes-flow)
      - [Holding force and torque for a sphere in a distant Stokeslet](stokes-flow.md#holding-force-and-torque-for-a-sphere-in-a-distant-stokeslet)
      - [Faxén's first law](stokes-flow.md#faxen-s-first-law)
        - [Rotne--Prager mobility](stokes-flow.md#rotne-prager-mobility)
          - [Hydrodynamic displacement of a force-free sphere](stokes-flow.md#hydrodynamic-displacement-of-a-force-free-sphere)
    - [Faxén's rotational law](stokes-flow.md#faxen-s-rotational-law)
    - [Method of reflections for Stokes flow](stokes-flow.md#method-of-reflections-for-stokes-flow)
      - [Forced-sphere rotation reflected from a held sphere](stokes-flow.md#forced-sphere-rotation-reflected-from-a-held-sphere)
      - [Leading interaction of two sedimenting spheres](stokes-flow.md#leading-interaction-of-two-sedimenting-spheres)
        - [Vertical bound pair in the point-force sedimentation model](stokes-flow.md#vertical-bound-pair-in-the-point-force-sedimentation-model)
        - [Passing invariant for unequal point-force spheres](stokes-flow.md#passing-invariant-for-unequal-point-force-spheres)
      - [Reversible scattering of two spheres in simple shear](stokes-flow.md#reversible-scattering-of-two-spheres-in-simple-shear)
      - [Mobility correction from a fixed distant sphere](stokes-flow.md#mobility-correction-from-a-fixed-distant-sphere)
        - [Deflection and spin in a distant sphere encounter](stokes-flow.md#deflection-and-spin-in-a-distant-sphere-encounter)
      - [Squirmer reflection from a held sphere](stokes-flow.md#squirmer-reflection-from-a-held-sphere)
      - [Rotational constraint correction to sphere mobility](stokes-flow.md#rotational-constraint-correction-to-sphere-mobility)
      - [Self-mobility correction from a distant force-free sphere](stokes-flow.md#self-mobility-correction-from-a-distant-force-free-sphere)
        - [Suppressed spin from a force-free distant sphere](stokes-flow.md#suppressed-spin-from-a-force-free-distant-sphere)
      - [Rotlet interaction of two spheres](stokes-flow.md#rotlet-interaction-of-two-spheres)
    - [Microswimmer](stokes-flow.md#microswimmer)
      - [Opposite-handed counterrotating helical swimmer](stokes-flow.md#opposite-handed-counterrotating-helical-swimmer)
        - [Large reaction helix limit](stokes-flow.md#large-reaction-helix-limit)
        - [Vanishing reaction rotor in a helical swimmer](stokes-flow.md#vanishing-reaction-rotor-in-a-helical-swimmer)
        - [Equal-length opposite-handed helices](stokes-flow.md#equal-length-opposite-handed-helices)
      - [Helical microswimmer with a spherical head](stokes-flow.md#helical-microswimmer-with-a-spherical-head)
        - [Entrained-head approximation for a helical microswimmer](stokes-flow.md#entrained-head-approximation-for-a-helical-microswimmer)
        - [Optimal pitch of a helical microswimmer](stokes-flow.md#optimal-pitch-of-a-helical-microswimmer)
      - [Squirmer](stokes-flow.md#squirmer)
        - [Torque-free rotation of a spherical squirmer](stokes-flow.md#torque-free-rotation-of-a-spherical-squirmer)
          - [Flow-free rotation of a spherical squirmer](stokes-flow.md#flow-free-rotation-of-a-spherical-squirmer)
        - [Two-mode tensorial squirmer flow](stokes-flow.md#two-mode-tensorial-squirmer-flow)
        - [Surface slip velocity](stokes-flow.md#surface-slip-velocity)
      - [Taylor swimming sheet](stokes-flow.md#taylor-swimming-sheet)
        - [Brinkman swimming sheet](stokes-flow.md#brinkman-swimming-sheet)
          - [Power of a Brinkman sheet](stokes-flow.md#power-of-a-brinkman-sheet)
          - [Swimming speed of a Brinkman sheet](stokes-flow.md#swimming-speed-of-a-brinkman-sheet)
          - [Screened first-order transverse sheet flow](stokes-flow.md#screened-first-order-transverse-sheet-flow)
        - [Navier-slip Taylor swimming sheet](stokes-flow.md#navier-slip-taylor-swimming-sheet)
          - [Slip-enhanced swimming speed of a transverse sheet](stokes-flow.md#slip-enhanced-swimming-speed-of-a-transverse-sheet)
          - [First-order slip independence of a transverse sheet](stokes-flow.md#first-order-slip-independence-of-a-transverse-sheet)
        - [Longitudinal mode of a Taylor swimming sheet](stokes-flow.md#longitudinal-mode-of-a-taylor-swimming-sheet)
        - [Transverse mode of a Taylor swimming sheet](stokes-flow.md#transverse-mode-of-a-taylor-swimming-sheet)
        - [Mean boundary velocity determines Taylor-sheet swimming speed](stokes-flow.md#mean-boundary-velocity-determines-taylor-sheet-swimming-speed)
          - [Fourier orthogonality of sheet swimming modes](stokes-flow.md#fourier-orthogonality-of-sheet-swimming-modes)
            - [Different-wavenumber cancellation in sheet swimming](stokes-flow.md#different-wavenumber-cancellation-in-sheet-swimming)
        - [Taylor-sheet swimming next to a rigid wall](stokes-flow.md#taylor-sheet-swimming-next-to-a-rigid-wall)
      - [Force-dipole flow](stokes-flow.md#force-dipole-flow)
        - [Axial repulsion of pusher stresslets](stokes-flow.md#axial-repulsion-of-pusher-stresslets)
        - [Orientation averaging of an axisymmetric stresslet](stokes-flow.md#orientation-averaging-of-an-axisymmetric-stresslet)
          - [Far-field orbit average of a tangent stresslet](stokes-flow.md#far-field-orbit-average-of-a-tangent-stresslet)
            - [Even displacement correction in an orbit-averaged stresslet](stokes-flow.md#even-displacement-correction-in-an-orbit-averaged-stresslet)
        - [Axisymmetric stresslet from a Stokeslet pair](stokes-flow.md#axisymmetric-stresslet-from-a-stokeslet-pair)
        - [Pusher microswimmer](stokes-flow.md#pusher-microswimmer)
        - [Puller microswimmer](stokes-flow.md#puller-microswimmer)
        - [Free-surface image of a force dipole](stokes-flow.md#free-surface-image-of-a-force-dipole)
          - [Free-surface interaction of two parallel stresslets](stokes-flow.md#free-surface-interaction-of-two-parallel-stresslets)
          - [Finite-time free-surface approach of a point stresslet](stokes-flow.md#finite-time-free-surface-approach-of-a-point-stresslet)
    - [Force-free](stokes-flow.md#force-free)
    - [Torque-free](stokes-flow.md#torque-free)
    - [Boundary perturbation of a nearly spherical particle](stokes-flow.md#boundary-perturbation-of-a-nearly-spherical-particle)
      - [First-order mobility of a nearly spherical particle](stokes-flow.md#first-order-mobility-of-a-nearly-spherical-particle)
  - [Viscous sheet](viscous-fluid-flow.md#viscous-sheet)
    - [Planar viscous-sheet stretching equations](viscous-fluid-flow.md#planar-viscous-sheet-stretching-equations)
      - [Uniform material thinning under planar-sheet tension](viscous-fluid-flow.md#uniform-material-thinning-under-planar-sheet-tension)
        - [Finite-time extension of a quadratically thickened sheet](viscous-fluid-flow.md#finite-time-extension-of-a-quadratically-thickened-sheet)
      - [Capillary drainage of a film between two bubbles](viscous-fluid-flow.md#capillary-drainage-of-a-film-between-two-bubbles)
    - [Axisymmetric viscous-sheet stretching equations](viscous-fluid-flow.md#axisymmetric-viscous-sheet-stretching-equations)
      - [Self-similar spreading of a viscous oil slick](viscous-fluid-flow.md#self-similar-spreading-of-a-viscous-oil-slick)
      - [Capillary growth of a hole in a viscous sheet](viscous-fluid-flow.md#capillary-growth-of-a-hole-in-a-viscous-sheet)
  - [Lubrication theory](viscous-fluid-flow.md#lubrication-theory)
    - [Normal-stress smallness in lubrication](viscous-fluid-flow.md#normal-stress-smallness-in-lubrication)
    - [Gravity-driven spreading of a planar viscous drop](viscous-fluid-flow.md#gravity-driven-spreading-of-a-planar-viscous-drop)
    - [Capillary instability of a thin film on a rigid cylinder](viscous-fluid-flow.md#capillary-instability-of-a-thin-film-on-a-rigid-cylinder)
      - [Volume-constrained capillary energy of a cylindrical coating](viscous-fluid-flow.md#volume-constrained-capillary-energy-of-a-cylindrical-coating)
      - [Quasisteady sliding collar on a coated cylinder](viscous-fluid-flow.md#quasisteady-sliding-collar-on-a-coated-cylinder)
        - [Collar-to-film capillary matching](viscous-fluid-flow.md#collar-to-film-capillary-matching)
    - [Cylinder translating parallel to a wall in a thin gap](viscous-fluid-flow.md#cylinder-translating-parallel-to-a-wall-in-a-thin-gap)
    - [Cusp flow between touching cylinders](viscous-fluid-flow.md#cusp-flow-between-touching-cylinders)
      - [Hydrostatic rise in a cylindrical cusp](viscous-fluid-flow.md#hydrostatic-rise-in-a-cylindrical-cusp)
      - [Fixed-volume capillary spreading in a cylindrical cusp](viscous-fluid-flow.md#fixed-volume-capillary-spreading-in-a-cylindrical-cusp)
    - [Lubrication model of a crawling snail](viscous-fluid-flow.md#lubrication-model-of-a-crawling-snail)
      - [Optimal sinusoidal waveform for viscous snail locomotion](viscous-fluid-flow.md#optimal-sinusoidal-waveform-for-viscous-snail-locomotion)
    - [Rotating roller under a nearly flat free surface](viscous-fluid-flow.md#rotating-roller-under-a-nearly-flat-free-surface)
    - [Lubrication resistance](viscous-fluid-flow.md#lubrication-resistance)
      - [Axial rotational resistance of eccentric nested spheres](viscous-fluid-flow.md#axial-rotational-resistance-of-eccentric-nested-spheres)
      - [Squeeze resistance of eccentric nested spheres](viscous-fluid-flow.md#squeeze-resistance-of-eccentric-nested-spheres)
      - [Lubrication prevents finite-time collision of smooth spheres](viscous-fluid-flow.md#lubrication-prevents-finite-time-collision-of-smooth-spheres)
    - [Viscous mountain spreading over an underthrust plate](viscous-fluid-flow.md#viscous-mountain-spreading-over-an-underthrust-plate)
      - [Sediment-lubricated viscous mountain model](viscous-fluid-flow.md#sediment-lubricated-viscous-mountain-model)
        - [Upstream basin profile of a sediment-lubricated mountain](viscous-fluid-flow.md#upstream-basin-profile-of-a-sediment-lubricated-mountain)
    - [Squeegee lubrication model](viscous-fluid-flow.md#squeegee-lubrication-model)
      - [Finite-blade side-drainage pile](viscous-fluid-flow.md#finite-blade-side-drainage-pile)
      - [Squeegee gap leakage flux](viscous-fluid-flow.md#squeegee-gap-leakage-flux)
      - [Infinite-blade gravity pile](viscous-fluid-flow.md#infinite-blade-gravity-pile)
    - [Journal bearing](viscous-fluid-flow.md#journal-bearing)
      - [Full-film journal bearing](viscous-fluid-flow.md#full-film-journal-bearing)
      - [Full-film journal-bearing whirl](viscous-fluid-flow.md#full-film-journal-bearing-whirl)
      - [Squeeze resistance of an eccentric journal bearing](viscous-fluid-flow.md#squeeze-resistance-of-an-eccentric-journal-bearing)
      - [Full-film eccentric journal-bearing rotation](viscous-fluid-flow.md#full-film-eccentric-journal-bearing-rotation)
    - [Lubrication gravity-current flux](viscous-fluid-flow.md#lubrication-gravity-current-flux)
    - [Draining viscous film on a finite horizontal plate](viscous-fluid-flow.md#draining-viscous-film-on-a-finite-horizontal-plate)
      - [Edge region of a draining viscous film](viscous-fluid-flow.md#edge-region-of-a-draining-viscous-film)
    - [Lubrication pressure](viscous-fluid-flow.md#lubrication-pressure)
    - [Hele-Shaw flow](viscous-fluid-flow.md#hele-shaw-flow)
    - [Long-wave approximation](viscous-fluid-flow.md#long-wave-approximation)
    - [Lubrication pressure dominates shear stress](viscous-fluid-flow.md#lubrication-pressure-dominates-shear-stress)
    - [Lubrication-limit scaling for a moving thin gap](viscous-fluid-flow.md#lubrication-limit-scaling-for-a-moving-thin-gap)
    - [Porous-plate lubrication cushion](viscous-fluid-flow.md#porous-plate-lubrication-cushion)
    - [Gravity-driven thin film on an incline](viscous-fluid-flow.md#gravity-driven-thin-film-on-an-incline)
      - [Inertia criterion for an inclined viscous film](viscous-fluid-flow.md#inertia-criterion-for-an-inclined-viscous-film)
      - [Travelling front of a gravity-driven thin film](viscous-fluid-flow.md#travelling-front-of-a-gravity-driven-thin-film)
        - [Small-slope breakdown at an inclined-current nose](viscous-fluid-flow.md#small-slope-breakdown-at-an-inclined-current-nose)
      - [Viscous gravity current on a cone](viscous-fluid-flow.md#viscous-gravity-current-on-a-cone)
      - [Finite-volume gravity-driven thin-film current](viscous-fluid-flow.md#finite-volume-gravity-driven-thin-film-current)
        - [Constant-head supply for a gravity-driven thin film](viscous-fluid-flow.md#constant-head-supply-for-a-gravity-driven-thin-film)
    - [Parabolic lubrication gap](viscous-fluid-flow.md#parabolic-lubrication-gap)
      - [Pressure-driven flux through a parabolic lubrication gap](viscous-fluid-flow.md#pressure-driven-flux-through-a-parabolic-lubrication-gap)
      - [Lubrication resistance integrals for a nearly occluding sphere](viscous-fluid-flow.md#lubrication-resistance-integrals-for-a-nearly-occluding-sphere)
        - [Radius-deficit normalization of sphere-tube lubrication integrals](viscous-fluid-flow.md#radius-deficit-normalization-of-sphere-tube-lubrication-integrals)
        - [Settling speed of a nearly occluding sphere without through-flow](viscous-fluid-flow.md#settling-speed-of-a-nearly-occluding-sphere-without-through-flow)
          - [Eccentricity increases narrow-gap bypass mobility](viscous-fluid-flow.md#eccentricity-increases-narrow-gap-bypass-mobility)
        - [Control-volume drag formula for a sphere in a tube](viscous-fluid-flow.md#control-volume-drag-formula-for-a-sphere-in-a-tube)
          - [Three drag regimes for a nearly occluding sphere](viscous-fluid-flow.md#three-drag-regimes-for-a-nearly-occluding-sphere)
            - [Sphere-tube drag regimes with a radius-deficit gap](viscous-fluid-flow.md#sphere-tube-drag-regimes-with-a-radius-deficit-gap)
            - [Load sharing between co-moving spheres in a tube](viscous-fluid-flow.md#load-sharing-between-co-moving-spheres-in-a-tube)
    - [Couette-Poiseuille flow in a thin gap](viscous-fluid-flow.md#couette-poiseuille-flow-in-a-thin-gap)
      - [Couette-Poiseuille flow with a stress-free stationary wall](viscous-fluid-flow.md#couette-poiseuille-flow-with-a-stress-free-stationary-wall)
      - [Moving-boundary lubrication flux](viscous-fluid-flow.md#moving-boundary-lubrication-flux)
        - [Sphere-frame flux in a tube](viscous-fluid-flow.md#sphere-frame-flux-in-a-tube)
        - [Drag on a plane beneath a translating cylinder](viscous-fluid-flow.md#drag-on-a-plane-beneath-a-translating-cylinder)
        - [Reynolds equation](viscous-fluid-flow.md#reynolds-equation)
          - [Horizontal rotation in a nearly touching spherical shell](viscous-fluid-flow.md#horizontal-rotation-in-a-nearly-touching-spherical-shell)
          - [Weakly compliant sphere-plane squeeze flow](viscous-fluid-flow.md#weakly-compliant-sphere-plane-squeeze-flow)
            - [Load-controlled breakdown of weak squeeze-flow compliance](viscous-fluid-flow.md#load-controlled-breakdown-of-weak-squeeze-flow-compliance)
          - [Logarithmic lubrication resistance of a sphere near a wall](viscous-fluid-flow.md#logarithmic-lubrication-resistance-of-a-sphere-near-a-wall)
            - [Logarithmic integrals in a parabolic lubrication gap](viscous-fluid-flow.md#logarithmic-integrals-in-a-parabolic-lubrication-gap)
          - [Pressure gradient in a translating and squeezing finite gap](viscous-fluid-flow.md#pressure-gradient-in-a-translating-and-squeezing-finite-gap)
            - [Zero-shear lower wall in a translating and squeezing finite gap](viscous-fluid-flow.md#zero-shear-lower-wall-in-a-translating-and-squeezing-finite-gap)
        - [Annular lubrication drag on a settling cylinder](viscous-fluid-flow.md#annular-lubrication-drag-on-a-settling-cylinder)
    - [Pressure recovery condition in lubrication flow](viscous-fluid-flow.md#pressure-recovery-condition-in-lubrication-flow)
    - [Nearly occluding sphere in a cylindrical tube](viscous-fluid-flow.md#nearly-occluding-sphere-in-a-cylindrical-tube)
      - [Force-free transport of a nearly occluding sphere](viscous-fluid-flow.md#force-free-transport-of-a-nearly-occluding-sphere)
      - [Wall-shear and pressure-drop balance in a tube](viscous-fluid-flow.md#wall-shear-and-pressure-drop-balance-in-a-tube)
    - [Thin-film equation](viscous-fluid-flow.md#thin-film-equation)
      - [Thermocapillary thin-film equation](viscous-fluid-flow.md#thermocapillary-thin-film-equation)
        - [Balanced scales for a thermocapillary film](viscous-fluid-flow.md#balanced-scales-for-a-thermocapillary-film)
        - [Zero-flux thermocapillary film profiles](viscous-fluid-flow.md#zero-flux-thermocapillary-film-profiles)
        - [Quasistatic temperature of a conductively cooled film](viscous-fluid-flow.md#quasistatic-temperature-of-a-conductively-cooled-film)
      - [Thin liquid film on a vertical cylinder](viscous-fluid-flow.md#thin-liquid-film-on-a-vertical-cylinder)
        - [Large solitary pulse on a cylindrical film](viscous-fluid-flow.md#large-solitary-pulse-on-a-cylindrical-film)
      - [Thin-film equations with insoluble surfactant](viscous-fluid-flow.md#thin-film-equations-with-insoluble-surfactant)
        - [Zero-liquid-flux surfactant film](viscous-fluid-flow.md#zero-liquid-flux-surfactant-film)
        - [Steady surfactant film with zero surface flux](viscous-fluid-flow.md#steady-surfactant-film-with-zero-surface-flux)
        - [Finite-mass Marangoni spreading on a liquid film](viscous-fluid-flow.md#finite-mass-marangoni-spreading-on-a-liquid-film)
          - [Gravity smoothing of a Marangoni front](viscous-fluid-flow.md#gravity-smoothing-of-a-marangoni-front)
            - [Gravity-levelled surfactant film](viscous-fluid-flow.md#gravity-levelled-surfactant-film)
          - [Capillary smoothing of a Marangoni front](viscous-fluid-flow.md#capillary-smoothing-of-a-marangoni-front)
          - [Linear similarity profiles for surfactant spreading](viscous-fluid-flow.md#linear-similarity-profiles-for-surfactant-spreading)
      - [Disjoining pressure](viscous-fluid-flow.md#disjoining-pressure)
        - [Van der Waals rupture instability of a viscous sheet](viscous-fluid-flow.md#van-der-waals-rupture-instability-of-a-viscous-sheet)
          - [Clean-sheet long-wave rupture plateau](viscous-fluid-flow.md#clean-sheet-long-wave-rupture-plateau)
      - [Thin-film mass flux](viscous-fluid-flow.md#thin-film-mass-flux)
    - [Slender viscous bubble](viscous-fluid-flow.md#slender-viscous-bubble)
      - [Lubrication equation for a bubble with viscous exterior](viscous-fluid-flow.md#lubrication-equation-for-a-bubble-with-viscous-exterior)
      - [Uniform-pressure evolution of a slender viscous bubble](viscous-fluid-flow.md#uniform-pressure-evolution-of-a-slender-viscous-bubble)
      - [Viscous-capillary pinch-off similarity](viscous-fluid-flow.md#viscous-capillary-pinch-off-similarity)
        - [Linear pinch-off scaling of a slender viscous bubble](viscous-fluid-flow.md#linear-pinch-off-scaling-of-a-slender-viscous-bubble)
    - [Slender viscous thread](viscous-fluid-flow.md#slender-viscous-thread)
      - [Annular viscous extension](viscous-fluid-flow.md#annular-viscous-extension)
        - [Capillary collapse of an annular viscous cylinder](viscous-fluid-flow.md#capillary-collapse-of-an-annular-viscous-cylinder)
      - [Capillary tensile force of a slender thread](viscous-fluid-flow.md#capillary-tensile-force-of-a-slender-thread)
        - [Capillary tensile force of a hollow slender thread](viscous-fluid-flow.md#capillary-tensile-force-of-a-hollow-slender-thread)
          - [Capillary closure of a falling hollow thread](viscous-fluid-flow.md#capillary-closure-of-a-falling-hollow-thread)
      - [Viscous-thread drawing](viscous-fluid-flow.md#viscous-thread-drawing)
        - [Localized-neck and uniform-thread stretching exponents](viscous-fluid-flow.md#localized-neck-and-uniform-thread-stretching-exponents)
      - [Viscous-sheet drawing](viscous-fluid-flow.md#viscous-sheet-drawing)
  - [Viscous shear torque](viscous-fluid-flow.md#viscous-shear-torque)
    - [Torque-free cylinder in a lubrication gap](viscous-fluid-flow.md#torque-free-cylinder-in-a-lubrication-gap)
      - [Falling cylinder near a wall](viscous-fluid-flow.md#falling-cylinder-near-a-wall)
        - [Shear and pressure force partition in cylinder lubrication](viscous-fluid-flow.md#shear-and-pressure-force-partition-in-cylinder-lubrication)
      - [Force-free cylinder in confined Couette flow](viscous-fluid-flow.md#force-free-cylinder-in-confined-couette-flow)
- [Surface tension](#surface-tension)
  - [Surface energy](#surface-energy)
  - [Wetting](#wetting)
    - [Contact line](#contact-line)
  - [Bond number](#bond-number)
  - [Oil lens capillary balance](#oil-lens-capillary-balance)
  - [Contact angle](#contact-angle)
  - [Capillary number](#capillary-number)
  - [Capillary pressure](#capillary-pressure)
  - [Surfactant](#surfactant)
    - [Surfactant transport with exchange relaxation](#surfactant-transport-with-exchange-relaxation)
      - [Translating surfactant-coated bubble](#translating-surfactant-coated-bubble)
        - [Normal stress balance on a translating bubble](#normal-stress-balance-on-a-translating-bubble)
        - [Dipolar surfactant distribution](#dipolar-surfactant-distribution)
    - [Surfactant stabilization of film rupture](#surfactant-stabilization-of-film-rupture)
      - [Strong-surfactant long-wave rupture maximum](#strong-surfactant-long-wave-rupture-maximum)
    - [Insoluble surfactant](#insoluble-surfactant)
      - [Surface diffusion](#surface-diffusion)
      - [Conservation of insoluble surfactant on a moving interface](#conservation-of-insoluble-surfactant-on-a-moving-interface)
        - [Quadrupolar surfactant distribution on a spherical interface](#quadrupolar-surfactant-distribution-on-a-spherical-interface)
  - [Marangoni effect](#marangoni-effect)
    - [Thermocapillary migration of an insulating bubble](#thermocapillary-migration-of-an-insulating-bubble)
    - [Interfacial stress balance with variable surface tension](#interfacial-stress-balance-with-variable-surface-tension)
      - [Marangoni immobilization of a bubble in straining flow](#marangoni-immobilization-of-a-bubble-in-straining-flow)
    - [Chemophoresis](#chemophoresis)
  - [Rayleigh–Plateau instability](#rayleigh-plateau-instability)
    - [Capillary instability of an annular liquid lining](#capillary-instability-of-an-annular-liquid-lining)
      - [Surfactant stabilization of an annular liquid lining](#surfactant-stabilization-of-an-annular-liquid-lining)
  - [Young–Laplace equation](#young-laplace-equation)
    - [Gibbs--Thomson relation](#gibbs-thomson-relation)
      - [Curvature-induced melting-temperature depression](#curvature-induced-melting-temperature-depression)
  - [Capillary length](#capillary-length)
  - [Dynamic meniscus](#dynamic-meniscus)
  - [Capillary wave](#capillary-wave)
    - [Deep-water capillary-wave dispersion relation](#deep-water-capillary-wave-dispersion-relation)
      - [Surface response to a localized impulsive velocity](#surface-response-to-a-localized-impulsive-velocity)
        - [Stationary-phase wake of an impulsive capillary wave](#stationary-phase-wake-of-an-impulsive-capillary-wave)
    - [Diffusion-limited relaxation of an interface](#diffusion-limited-relaxation-of-an-interface)
- [Body force](#body-force)
  - [Elastic force dipole](#elastic-force-dipole)
- [Hydrostatic pressure](#hydrostatic-pressure)
  - [Hydrostatic approximation](#hydrostatic-approximation)
    - [Hydrostatic balance](#hydrostatic-balance)
- [Volumetric flow rate](#volumetric-flow-rate)
  - [Mass flow rate](#mass-flow-rate)
  - [Volume flux per unit width](#volume-flux-per-unit-width)
  - [Discharge coefficient](#discharge-coefficient)
- [Potential flow](#potential-flow)
  - [Corner sink in a semi-infinite channel](#corner-sink-in-a-semi-infinite-channel)
  - [Rankine half-body](#rankine-half-body)
  - [Radial source flow](#radial-source-flow)
  - [Potential dipole](#potential-dipole)
  - [Point source](#point-source)
    - [Source dipole](#source-dipole)
    - [Three-dimensional point source](#three-dimensional-point-source)
    - [Hydrodynamic attraction of a plane wall to a point source](#hydrodynamic-attraction-of-a-plane-wall-to-a-point-source)
  - [Sink flow in a sector](#sink-flow-in-a-sector)
    - [Similarity solution for a sink-flow boundary layer](#similarity-solution-for-a-sink-flow-boundary-layer)
  - [Potential flow around a translating sphere](#potential-flow-around-a-translating-sphere)
  - [Spherically symmetric incompressible radial flow](#spherically-symmetric-incompressible-radial-flow)
    - [Rayleigh equation for an inviscid spherical bubble](#rayleigh-equation-for-an-inviscid-spherical-bubble)
      - [Pressure-work energy balance for a spherical bubble](#pressure-work-energy-balance-for-a-spherical-bubble)
      - [First integral of polytropic spherical-bubble motion](#first-integral-of-polytropic-spherical-bubble-motion)
    - [Rayleigh-Plesset equation](#rayleigh-plesset-equation)
      - [Rayleigh collapse of a spherical cavity](#rayleigh-collapse-of-a-spherical-cavity)
  - [Squeezing wedge flow](#squeezing-wedge-flow)
- [Free surface](#free-surface)
  - [Surface gravity wave](#surface-gravity-wave)
    - [Surface-wave breaking](#surface-wave-breaking)
    - [Normal modes of surface gravity waves in a rectangular tank](#normal-modes-of-surface-gravity-waves-in-a-rectangular-tank)
    - [Power-law near-shore ray asymptotics](#power-law-near-shore-ray-asymptotics)
    - [Wave fetch](#wave-fetch)
    - [Radiation stress](#radiation-stress)
    - [Surface-gravity-wave energy](#surface-gravity-wave-energy)
    - [Wave steepness](#wave-steepness)
    - [Airy wave theory](#airy-wave-theory)
      - [Deep-water gravity wave](#deep-water-gravity-wave)
        - [Dispersive swell source inversion](#dispersive-swell-source-inversion)
        - [Viscous decay of a deep-water gravity wave](#viscous-decay-of-a-deep-water-gravity-wave)
        - [Linearized free-surface boundary conditions](#linearized-free-surface-boundary-conditions)
          - [Rectangular standing surface-gravity mode](#rectangular-standing-surface-gravity-mode)
            - [Resonance of a pressure-forced rectangular surface-gravity mode](#resonance-of-a-pressure-forced-rectangular-surface-gravity-mode)
- [Streamfunction in polar coordinates](#streamfunction-in-polar-coordinates)
- [Stagnation point](#stagnation-point)
- [Incompressible flow](#incompressible-flow)
  - [Rectilinear flow](#rectilinear-flow)
  - [Streamfunction advection bracket](#streamfunction-advection-bracket)
  - [Cartesian streamfunction](#cartesian-streamfunction)
  - [Divergence-free vector field](#divergence-free-vector-field)
- [Streakline](#streakline)
- [Kinematic boundary condition](#kinematic-boundary-condition)
  - [Kinematic boundary condition for a free-surface graph](#kinematic-boundary-condition-for-a-free-surface-graph)
  - [Linearized boundary condition](#linearized-boundary-condition)
- [Dynamic boundary condition for an inviscid interface](#dynamic-boundary-condition-for-an-inviscid-interface)
  - [Pressure continuity](#pressure-continuity)
- [Wake (physics)](#wake-physics)
- [Shear layer](#shear-layer)
  - [Vortex sheet](#vortex-sheet)
    - [Cylindrical vortex sheet](#cylindrical-vortex-sheet)
    - [Kelvin-Helmholtz instability](#kelvin-helmholtz-instability)
      - [Bending-membrane Kelvin-Helmholtz dispersion relation](#bending-membrane-kelvin-helmholtz-dispersion-relation)
      - [Kelvin-Helmholtz dispersion relation with gravity](#kelvin-helmholtz-dispersion-relation-with-gravity)
      - [Top-hat planar jet](#top-hat-planar-jet)
        - [Varicose mode of a planar jet](#varicose-mode-of-a-planar-jet)
        - [Sinuous mode of a planar jet](#sinuous-mode-of-a-planar-jet)
        - [Equal-density top-hat planar-jet dispersion relation](#equal-density-top-hat-planar-jet-dispersion-relation)
          - [Equality of top-hat jet parity growth rates](#equality-of-top-hat-jet-parity-growth-rates)
      - [Finite-depth vortex-sheet dispersion relation](#finite-depth-vortex-sheet-dispersion-relation)
- [Compressible flow](compressible-flow.md)
  - [Self-similar blast wave](compressible-flow.md#self-similar-blast-wave)
    - [Thin-shell approximation for a spherical blast wave](compressible-flow.md#thin-shell-approximation-for-a-spherical-blast-wave)
    - [Spherical blast wave in a power-law ambient density](compressible-flow.md#spherical-blast-wave-in-a-power-law-ambient-density)
      - [Linear-profile spherical blast wave](compressible-flow.md#linear-profile-spherical-blast-wave)
    - [Planar blast-wave energy scaling](compressible-flow.md#planar-blast-wave-energy-scaling)
  - [Polytropic flow](compressible-flow.md#polytropic-flow)
  - [Spherically symmetric adiabatic flow](compressible-flow.md#spherically-symmetric-adiabatic-flow)
    - [Transonic spherical flow in a power-law potential](compressible-flow.md#transonic-spherical-flow-in-a-power-law-potential)
      - [Transonic spherical accretion rate in a power-law potential](compressible-flow.md#transonic-spherical-accretion-rate-in-a-power-law-potential)
        - [Endpoint limits of power-law spherical accretion](compressible-flow.md#endpoint-limits-of-power-law-spherical-accretion)
      - [Critical adiabatic exponent for spherical power-law flow](compressible-flow.md#critical-adiabatic-exponent-for-spherical-power-law-flow)
  - [Isothermal shock](compressible-flow.md#isothermal-shock)
    - [Cooling across an isothermal shock](compressible-flow.md#cooling-across-an-isothermal-shock)
  - [Fluid total-energy equation](compressible-flow.md#fluid-total-energy-equation)
  - [Spherical polytropic flow with adiabatic exponent three halves](compressible-flow.md#spherical-polytropic-flow-with-adiabatic-exponent-three-halves)
  - [Speed of sound](compressible-flow.md#speed-of-sound)
    - [Sound-crossing time](compressible-flow.md#sound-crossing-time)
    - [Isothermal sound speed](compressible-flow.md#isothermal-sound-speed)
    - [Adiabatic sound speed](compressible-flow.md#adiabatic-sound-speed)
  - [Isentropic flow](compressible-flow.md#isentropic-flow)
    - [Isentropic Euler equations](compressible-flow.md#isentropic-euler-equations)
    - [Homentropic flow](compressible-flow.md#homentropic-flow)
  - [Globally isothermal equation of state](compressible-flow.md#globally-isothermal-equation-of-state)
  - [Sonic point](compressible-flow.md#sonic-point)
    - [Plane-parallel isothermal sonic transition at a potential maximum](compressible-flow.md#plane-parallel-isothermal-sonic-transition-at-a-potential-maximum)
    - [Sonic-point slope discriminant](compressible-flow.md#sonic-point-slope-discriminant)
    - [Critical speed of a polytropic flow](compressible-flow.md#critical-speed-of-a-polytropic-flow)
    - [Transonic branch](compressible-flow.md#transonic-branch)
      - [Transonic accretion in a power-law tube](compressible-flow.md#transonic-accretion-in-a-power-law-tube)
  - [Mach number](compressible-flow.md#mach-number)
    - [Radial Mach number](compressible-flow.md#radial-mach-number)
    - [Subsonic flow](compressible-flow.md#subsonic-flow)
    - [Supersonic flow](compressible-flow.md#supersonic-flow)
  - [Riemann invariant](compressible-flow.md#riemann-invariant)
    - [Riemann invariants for one-dimensional isentropic flow](compressible-flow.md#riemann-invariants-for-one-dimensional-isentropic-flow)
      - [Vacuum formation at an accelerating withdrawing piston](compressible-flow.md#vacuum-formation-at-an-accelerating-withdrawing-piston)
    - [Simple wave](compressible-flow.md#simple-wave)
      - [Area transformation of a nonlinear acoustic simple wave](compressible-flow.md#area-transformation-of-a-nonlinear-acoustic-simple-wave)
        - [Shock distance for a spherical simple wave launched at finite radius](compressible-flow.md#shock-distance-for-a-spherical-simple-wave-launched-at-finite-radius)
      - [Linearly degenerate characteristic field](compressible-flow.md#linearly-degenerate-characteristic-field)
      - [Simple wave in magnetohydrodynamics](compressible-flow.md#simple-wave-in-magnetohydrodynamics)
        - [Perpendicular fast magnetosonic simple wave](compressible-flow.md#perpendicular-fast-magnetosonic-simple-wave)
          - [Isothermal perpendicular magnetosonic simple wave](compressible-flow.md#isothermal-perpendicular-magnetosonic-simple-wave)
      - [Damping threshold for a simple wave](compressible-flow.md#damping-threshold-for-a-simple-wave)
      - [Receding-piston rarefaction wave](compressible-flow.md#receding-piston-rarefaction-wave)
        - [Vacuum formation behind a receding piston](compressible-flow.md#vacuum-formation-behind-a-receding-piston)
        - [Singular small-power piston emission time](compressible-flow.md#singular-small-power-piston-emission-time)
    - [Pressure in a perfect-gas simple wave](compressible-flow.md#pressure-in-a-perfect-gas-simple-wave)
    - [Shock formation by characteristic intersection](compressible-flow.md#shock-formation-by-characteristic-intersection)
  - [Normal shock wave](compressible-flow.md#normal-shock-wave)
    - [Normal shock reflection at a rigid wall](compressible-flow.md#normal-shock-reflection-at-a-rigid-wall)
    - [Moving-interface conservation jump identity](compressible-flow.md#moving-interface-conservation-jump-identity)
    - [Normal shock tables](compressible-flow.md#normal-shock-tables)
    - [Shock frame](compressible-flow.md#shock-frame)
    - [Rankine-Hugoniot conditions for a perfect gas](compressible-flow.md#rankine-hugoniot-conditions-for-a-perfect-gas)
      - [Prandtl shock relation](compressible-flow.md#prandtl-shock-relation)
      - [Strong-shock Rankine-Hugoniot conditions](compressible-flow.md#strong-shock-rankine-hugoniot-conditions)
        - [Shock compression ratio](compressible-flow.md#shock-compression-ratio)
      - [Piston-driven normal shock](compressible-flow.md#piston-driven-normal-shock)
        - [Piston-driven shock with specific-heat ratio three](compressible-flow.md#piston-driven-shock-with-specific-heat-ratio-three)
      - [Pressure-density Hugoniot relation for a perfect gas](compressible-flow.md#pressure-density-hugoniot-relation-for-a-perfect-gas)
        - [Entropy production in a perfect-gas shock](compressible-flow.md#entropy-production-in-a-perfect-gas-shock)
          - [Entropy production in successive weak shocks](compressible-flow.md#entropy-production-in-successive-weak-shocks)
    - [Weak shock](compressible-flow.md#weak-shock)
    - [Oblique shock](compressible-flow.md#oblique-shock)
      - [Shock polar](compressible-flow.md#shock-polar)
        - [Strong-shock polar for a perfect gas](compressible-flow.md#strong-shock-polar-for-a-perfect-gas)
          - [Maximum deflection through a strong perfect-gas shock](compressible-flow.md#maximum-deflection-through-a-strong-perfect-gas-shock)
      - [Weak-oblique-shock deflection](compressible-flow.md#weak-oblique-shock-deflection)
      - [Mach angle](compressible-flow.md#mach-angle)
        - [Mach cone](compressible-flow.md#mach-cone)
- [Linear acoustics](linear-acoustics.md)
  - [Stationary vorticity mode in linear acoustics](linear-acoustics.md#stationary-vorticity-mode-in-linear-acoustics)
  - [Rayleigh integral for baffled acoustic radiation](linear-acoustics.md#rayleigh-integral-for-baffled-acoustic-radiation)
  - [Acoustic far field](linear-acoustics.md#acoustic-far-field)
    - [Acoustic directivity](linear-acoustics.md#acoustic-directivity)
  - [Moving-surface retarded Jacobian](linear-acoustics.md#moving-surface-retarded-jacobian)
  - [Stratified acoustic pressure equation](linear-acoustics.md#stratified-acoustic-pressure-equation)
  - [Acoustic density perturbation](linear-acoustics.md#acoustic-density-perturbation)
  - [Acoustic compact-source approximation](linear-acoustics.md#acoustic-compact-source-approximation)
  - [Acoustic multipole source](linear-acoustics.md#acoustic-multipole-source)
    - [Acoustic quadrupole](linear-acoustics.md#acoustic-quadrupole)
      - [Compact rotating two-blade loading source](linear-acoustics.md#compact-rotating-two-blade-loading-source)
      - [Compact acoustic quadrupole Mach-number scaling](linear-acoustics.md#compact-acoustic-quadrupole-mach-number-scaling)
        - [Two-dimensional compact quadrupole scaling](linear-acoustics.md#two-dimensional-compact-quadrupole-scaling)
    - [Acoustic dipole](linear-acoustics.md#acoustic-dipole)
      - [Acoustic dipole Mach-number scaling](linear-acoustics.md#acoustic-dipole-mach-number-scaling)
    - [Acoustic monopole](linear-acoustics.md#acoustic-monopole)
      - [Rotating acoustic point source](linear-acoustics.md#rotating-acoustic-point-source)
  - [Lighthill acoustic analogy](linear-acoustics.md#lighthill-acoustic-analogy)
    - [Mass-injection term in the acoustic analogy](linear-acoustics.md#mass-injection-term-in-the-acoustic-analogy)
    - [Far-field acoustic force and stress moments](linear-acoustics.md#far-field-acoustic-force-and-stress-moments)
    - [Distributional acoustic analogy across a moving interface](linear-acoustics.md#distributional-acoustic-analogy-across-a-moving-interface)
      - [Ffowcs Williams-Hawkings equation](linear-acoustics.md#ffowcs-williams-hawkings-equation)
        - [Fixed-body retarded acoustic loading formula](linear-acoustics.md#fixed-body-retarded-acoustic-loading-formula)
        - [Acoustic loading noise](linear-acoustics.md#acoustic-loading-noise)
          - [Small-body loading-noise threshold](linear-acoustics.md#small-body-loading-noise-threshold)
        - [Acoustic thickness noise](linear-acoustics.md#acoustic-thickness-noise)
          - [Compact radiation moments of a pulsating spherical bubble](linear-acoustics.md#compact-radiation-moments-of-a-pulsating-spherical-bubble)
          - [Translating-sphere acoustic thickness dipole](linear-acoustics.md#translating-sphere-acoustic-thickness-dipole)
    - [Lighthill stress tensor](linear-acoustics.md#lighthill-stress-tensor)
      - [Surface sources of a discontinuous Lighthill stress tensor](linear-acoustics.md#surface-sources-of-a-discontinuous-lighthill-stress-tensor)
  - [Linear homentropic acoustic equations](linear-acoustics.md#linear-homentropic-acoustic-equations)
    - [Acoustic pressure wave equation](linear-acoustics.md#acoustic-pressure-wave-equation)
      - [Outgoing acoustic square-root branch](linear-acoustics.md#outgoing-acoustic-square-root-branch)
  - [Homentropic pressure perturbation](linear-acoustics.md#homentropic-pressure-perturbation)
  - [Acoustic velocity potential](linear-acoustics.md#acoustic-velocity-potential)
    - [Outgoing acoustic field of a pulsating sphere](linear-acoustics.md#outgoing-acoustic-field-of-a-pulsating-sphere)
      - [Mean acoustic power of a pulsating sphere](linear-acoustics.md#mean-acoustic-power-of-a-pulsating-sphere)
      - [Surface acoustic energy-to-flux ratio of a pulsating sphere](linear-acoustics.md#surface-acoustic-energy-to-flux-ratio-of-a-pulsating-sphere)
    - [Pressure-forced standing acoustic wave in a spherical annulus](linear-acoustics.md#pressure-forced-standing-acoustic-wave-in-a-spherical-annulus)
      - [Radial acoustic resonance in a spherical annulus](linear-acoustics.md#radial-acoustic-resonance-in-a-spherical-annulus)
    - [Spherically symmetric vibration of a gas-filled elastic shell](linear-acoustics.md#spherically-symmetric-vibration-of-a-gas-filled-elastic-shell)
  - [Acoustic energy conservation](linear-acoustics.md#acoustic-energy-conservation)
    - [Near-field energy imbalance in a spherical acoustic wave](linear-acoustics.md#near-field-energy-imbalance-in-a-spherical-acoustic-wave)
    - [Acoustic energy density](linear-acoustics.md#acoustic-energy-density)
  - [Evanescent acoustic surface wave](linear-acoustics.md#evanescent-acoustic-surface-wave)
    - [Acoustic wave on a tensioned massive membrane](linear-acoustics.md#acoustic-wave-on-a-tensioned-massive-membrane)
      - [Elastic-sheet tension](linear-acoustics.md#elastic-sheet-tension)
      - [Point-force radiation from a fluid-loaded sheet](linear-acoustics.md#point-force-radiation-from-a-fluid-loaded-sheet)
        - [One-sided fluid-loaded membrane radiation](linear-acoustics.md#one-sided-fluid-loaded-membrane-radiation)
      - [Tensioned-sheet acoustic impedance](linear-acoustics.md#tensioned-sheet-acoustic-impedance)
        - [Reflection pole of a fluid-loaded membrane](linear-acoustics.md#reflection-pole-of-a-fluid-loaded-membrane)
      - [Fluid-loaded membrane edge scattering](linear-acoustics.md#fluid-loaded-membrane-edge-scattering)
        - [Plane-wave forcing of a pinned elastic half-sheet](linear-acoustics.md#plane-wave-forcing-of-a-pinned-elastic-half-sheet)
        - [Incoming-pole cancellation at a pinned membrane edge](linear-acoustics.md#incoming-pole-cancellation-at-a-pinned-membrane-edge)
    - [Spring-supported acoustic membrane wave](linear-acoustics.md#spring-supported-acoustic-membrane-wave)
      - [Acoustic membrane dispersion asymptotics](linear-acoustics.md#acoustic-membrane-dispersion-asymptotics)
    - [Added mass of an evanescent fluid layer](linear-acoustics.md#added-mass-of-an-evanescent-fluid-layer)
  - [Time average of harmonic power](linear-acoustics.md#time-average-of-harmonic-power)
    - [Reactive acoustic energy flux](linear-acoustics.md#reactive-acoustic-energy-flux)
- [Astrophysical fluid dynamics](astrophysical-fluid-dynamics.md)
  - [Gravitational instability](astrophysical-fluid-dynamics.md#gravitational-instability)
  - [Critically rotating self-gravitating cylinder](astrophysical-fluid-dynamics.md#critically-rotating-self-gravitating-cylinder)
    - [Dipolar perturbations of a critically rotating cylinder](astrophysical-fluid-dynamics.md#dipolar-perturbations-of-a-critically-rotating-cylinder)
    - [Gravitational potential of a displaced cylindrical interface](astrophysical-fluid-dynamics.md#gravitational-potential-of-a-displaced-cylindrical-interface)
  - [Uniformly rotating barotropic star](astrophysical-fluid-dynamics.md#uniformly-rotating-barotropic-star)
    - [Pressure equation for inertial oscillations of a barotropic star](astrophysical-fluid-dynamics.md#pressure-equation-for-inertial-oscillations-of-a-barotropic-star)
      - [Sectoral inertial mode of a slowly rotating barotropic star](astrophysical-fluid-dynamics.md#sectoral-inertial-mode-of-a-slowly-rotating-barotropic-star)
      - [Anelastic approximation for a rotating barotropic star](astrophysical-fluid-dynamics.md#anelastic-approximation-for-a-rotating-barotropic-star)
  - [Self-gravitating incompressible slab](astrophysical-fluid-dynamics.md#self-gravitating-incompressible-slab)
    - [Gravitational instability of an incompressible slab](astrophysical-fluid-dynamics.md#gravitational-instability-of-an-incompressible-slab)
    - [Surface modes of a self-gravitating incompressible slab](astrophysical-fluid-dynamics.md#surface-modes-of-a-self-gravitating-incompressible-slab)
  - [Isothermal pressure support during gravitational collapse](astrophysical-fluid-dynamics.md#isothermal-pressure-support-during-gravitational-collapse)
  - [Adiabatic pressure support during gravitational collapse](astrophysical-fluid-dynamics.md#adiabatic-pressure-support-during-gravitational-collapse)
  - [Differential rotation](astrophysical-fluid-dynamics.md#differential-rotation)
  - [Affine stellar model](astrophysical-fluid-dynamics.md#affine-stellar-model)
    - [Affine breathing mode of a star](astrophysical-fluid-dynamics.md#affine-breathing-mode-of-a-star)
    - [Affine quadrupole mode of a star](astrophysical-fluid-dynamics.md#affine-quadrupole-mode-of-a-star)
  - [Stellar oscillation](astrophysical-fluid-dynamics.md#stellar-oscillation)
    - [Helioseismology](astrophysical-fluid-dynamics.md#helioseismology)
      - [Solar rotational mode splitting](astrophysical-fluid-dynamics.md#solar-rotational-mode-splitting)
      - [Duvall law](astrophysical-fluid-dynamics.md#duvall-law)
        - [Abel inversion of stellar acoustic travel times](astrophysical-fluid-dynamics.md#abel-inversion-of-stellar-acoustic-travel-times)
    - [Axisymmetric adiabatic displacement operator](astrophysical-fluid-dynamics.md#axisymmetric-adiabatic-displacement-operator)
      - [Cowling energy principle for a rotating barotropic star](astrophysical-fluid-dynamics.md#cowling-energy-principle-for-a-rotating-barotropic-star)
        - [Effective-potential stratification coefficient](astrophysical-fluid-dynamics.md#effective-potential-stratification-coefficient)
    - [Stellar gravity mode](astrophysical-fluid-dynamics.md#stellar-gravity-mode)
    - [Stellar acoustic mode](astrophysical-fluid-dynamics.md#stellar-acoustic-mode)
      - [Large frequency separation](astrophysical-fluid-dynamics.md#large-frequency-separation)
    - [Lamb frequency](astrophysical-fluid-dynamics.md#lamb-frequency)
    - [Linear adiabatic stellar oscillation equations](astrophysical-fluid-dynamics.md#linear-adiabatic-stellar-oscillation-equations)
      - [Stellar displacement energy identity](astrophysical-fluid-dynamics.md#stellar-displacement-energy-identity)
        - [Pressure-free localized stellar convective trial](astrophysical-fluid-dynamics.md#pressure-free-localized-stellar-convective-trial)
      - [Acoustic-gravity propagation relation](astrophysical-fluid-dynamics.md#acoustic-gravity-propagation-relation)
      - [Cowling approximation](astrophysical-fluid-dynamics.md#cowling-approximation)
        - [Plane-parallel Cowling displacement-pressure equations](astrophysical-fluid-dynamics.md#plane-parallel-cowling-displacement-pressure-equations)
          - [Plane-parallel stellar f-mode](astrophysical-fluid-dynamics.md#plane-parallel-stellar-f-mode)
            - [Matched chromospheric interfacial mode](astrophysical-fluid-dynamics.md#matched-chromospheric-interfacial-mode)
        - [Angular-degree bound on perturbed stellar self-gravity](astrophysical-fluid-dynamics.md#angular-degree-bound-on-perturbed-stellar-self-gravity)
      - [Radial stellar pulsation equation](astrophysical-fluid-dynamics.md#radial-stellar-pulsation-equation)
        - [Central-density upper bound for a radial stellar frequency](astrophysical-fluid-dynamics.md#central-density-upper-bound-for-a-radial-stellar-frequency)
        - [Weighted stellar pulsation Rayleigh quotient](astrophysical-fluid-dynamics.md#weighted-stellar-pulsation-rayleigh-quotient)
          - [Positive-square radial pulsation energy](astrophysical-fluid-dynamics.md#positive-square-radial-pulsation-energy)
          - [Pressure-weighted radial instability criterion](astrophysical-fluid-dynamics.md#pressure-weighted-radial-instability-criterion)
    - [Self-gravitating adiabatic displacement equations](astrophysical-fluid-dynamics.md#self-gravitating-adiabatic-displacement-equations)
      - [Uniform-density stellar oscillation](astrophysical-fluid-dynamics.md#uniform-density-stellar-oscillation)
        - [Radial stability of a uniform-density star](astrophysical-fluid-dynamics.md#radial-stability-of-a-uniform-density-star)
        - [Polynomial stellar-mode coefficient reduction](astrophysical-fluid-dynamics.md#polynomial-stellar-mode-coefficient-reduction)
        - [Dynamical frequency of a uniform-density star](astrophysical-fluid-dynamics.md#dynamical-frequency-of-a-uniform-density-star)
    - [Incompressible stellar surface mode](astrophysical-fluid-dynamics.md#incompressible-stellar-surface-mode)
      - [Kelvin stellar mode](astrophysical-fluid-dynamics.md#kelvin-stellar-mode)
      - [Surface gravity perturbation of a uniform-density sphere](astrophysical-fluid-dynamics.md#surface-gravity-perturbation-of-a-uniform-density-sphere)
    - [Tidal resonance of a stellar oscillation](astrophysical-fluid-dynamics.md#tidal-resonance-of-a-stellar-oscillation)
  - [Polytrope](astrophysical-fluid-dynamics.md#polytrope)
    - [Polytropic equation of state](astrophysical-fluid-dynamics.md#polytropic-equation-of-state)
    - [Polytropic atmosphere](astrophysical-fluid-dynamics.md#polytropic-atmosphere)
      - [Surface sound speed of a polytropic star](astrophysical-fluid-dynamics.md#surface-sound-speed-of-a-polytropic-star)
      - [Neutrally stratified polytropic atmosphere](astrophysical-fluid-dynamics.md#neutrally-stratified-polytropic-atmosphere)
      - [Surface gravito-inertial wave](astrophysical-fluid-dynamics.md#surface-gravito-inertial-wave)
      - [Polytropic acoustic mode](astrophysical-fluid-dynamics.md#polytropic-acoustic-mode)
  - [Magnetohydrodynamics](astrophysical-fluid-dynamics.md#magnetohydrodynamics)
    - [Magnetic flux concentration](astrophysical-fluid-dynamics.md#magnetic-flux-concentration)
      - [Equipartition magnetic field](astrophysical-fluid-dynamics.md#equipartition-magnetic-field)
      - [Convective collapse](astrophysical-fluid-dynamics.md#convective-collapse)
    - [Magnetostrophic balance](astrophysical-fluid-dynamics.md#magnetostrophic-balance)
      - [Taylor constraint](astrophysical-fluid-dynamics.md#taylor-constraint)
        - [Viscous regularization of the Taylor constraint](astrophysical-fluid-dynamics.md#viscous-regularization-of-the-taylor-constraint)
        - [Geostrophic flow preserving the Taylor constraint](astrophysical-fluid-dynamics.md#geostrophic-flow-preserving-the-taylor-constraint)
        - [Magnetostrophic Taylor state](astrophysical-fluid-dynamics.md#magnetostrophic-taylor-state)
    - [Mean-field electrodynamics](astrophysical-fluid-dynamics.md#mean-field-electrodynamics)
    - [Kinematic magnetic dynamo](astrophysical-fluid-dynamics.md#kinematic-magnetic-dynamo)
      - [Gaussian white-noise magnetic stretching](astrophysical-fluid-dynamics.md#gaussian-white-noise-magnetic-stretching)
        - [Lognormal magnetic-field amplification](astrophysical-fluid-dynamics.md#lognormal-magnetic-field-amplification)
        - [Magnetic stretching moment growth](astrophysical-fluid-dynamics.md#magnetic-stretching-moment-growth)
        - [Radial magnetic-field Fokker-Planck equation](astrophysical-fluid-dynamics.md#radial-magnetic-field-fokker-planck-equation)
    - [Theta pinch](astrophysical-fluid-dynamics.md#theta-pinch)
      - [Positive ideal energy of a theta pinch](astrophysical-fluid-dynamics.md#positive-ideal-energy-of-a-theta-pinch)
    - [Hall magnetohydrodynamics](astrophysical-fluid-dynamics.md#hall-magnetohydrodynamics)
      - [Fast-time electron-MHD limit of Hall magnetohydrodynamics](astrophysical-fluid-dynamics.md#fast-time-electron-mhd-limit-of-hall-magnetohydrodynamics)
      - [Incompressible Hall-MHD wave dispersion](astrophysical-fluid-dynamics.md#incompressible-hall-mhd-wave-dispersion)
    - [Electron magnetohydrodynamics](astrophysical-fluid-dynamics.md#electron-magnetohydrodynamics)
      - [Whistler wave](astrophysical-fluid-dynamics.md#whistler-wave)
      - [Reduced electron magnetohydrodynamics](astrophysical-fluid-dynamics.md#reduced-electron-magnetohydrodynamics)
    - [Stratified magneto-Coriolis wave](astrophysical-fluid-dynamics.md#stratified-magneto-coriolis-wave)
      - [Rapid-rotation slow magneto-Coriolis branch](astrophysical-fluid-dynamics.md#rapid-rotation-slow-magneto-coriolis-branch)
    - [Lehnert number](astrophysical-fluid-dynamics.md#lehnert-number)
    - [Magnetohydrodynamic momentum equation](astrophysical-fluid-dynamics.md#magnetohydrodynamic-momentum-equation)
    - [Resistive magnetohydrodynamics](astrophysical-fluid-dynamics.md#resistive-magnetohydrodynamics)
      - [Magnetic reconnection](astrophysical-fluid-dynamics.md#magnetic-reconnection)
      - [Magnetic skin layer](astrophysical-fluid-dynamics.md#magnetic-skin-layer)
        - [Magnetic skin-layer streaming slip](astrophysical-fluid-dynamics.md#magnetic-skin-layer-streaming-slip)
        - [Mean Lorentz force in a magnetic skin layer](astrophysical-fluid-dynamics.md#mean-lorentz-force-in-a-magnetic-skin-layer)
      - [Flux expulsion](astrophysical-fluid-dynamics.md#flux-expulsion)
        - [Phase mixing in magnetic flux expulsion](astrophysical-fluid-dynamics.md#phase-mixing-in-magnetic-flux-expulsion)
          - [Cubic-time resistive damping in a differentially rotating cell](astrophysical-fluid-dynamics.md#cubic-time-resistive-damping-in-a-differentially-rotating-cell)
      - [Dynamo action](astrophysical-fluid-dynamics.md#dynamo-action)
        - [Radial-flow dynamo energy bound](astrophysical-fluid-dynamics.md#radial-flow-dynamo-energy-bound)
        - [Dynamo quenching](astrophysical-fluid-dynamics.md#dynamo-quenching)
          - [Algebraic alpha quenching](astrophysical-fluid-dynamics.md#algebraic-alpha-quenching)
            - [Alpha-quenching rotating wave](astrophysical-fluid-dynamics.md#alpha-quenching-rotating-wave)
              - [Unequal-hemisphere dynamo rotating wave](astrophysical-fluid-dynamics.md#unequal-hemisphere-dynamo-rotating-wave)
        - [Equivariant three-mode dynamo normal form](astrophysical-fluid-dynamics.md#equivariant-three-mode-dynamo-normal-form)
          - [Magnetic onset on a rotating velocity branch](astrophysical-fluid-dynamics.md#magnetic-onset-on-a-rotating-velocity-branch)
          - [Normalization of nonzero dynamo coupling coefficients](astrophysical-fluid-dynamics.md#normalization-of-nonzero-dynamo-coupling-coefficients)
        - [Anti-dynamo theorem](astrophysical-fluid-dynamics.md#anti-dynamo-theorem)
          - [Periodic two-coordinate anti-dynamo energy bound](astrophysical-fluid-dynamics.md#periodic-two-coordinate-anti-dynamo-energy-bound)
          - [Planar anti-dynamo theorem](astrophysical-fluid-dynamics.md#planar-anti-dynamo-theorem)
            - [Zeldovich planar flux balance](astrophysical-fluid-dynamics.md#zeldovich-planar-flux-balance)
          - [Toroidal-velocity anti-dynamo theorem](astrophysical-fluid-dynamics.md#toroidal-velocity-anti-dynamo-theorem)
          - [Cowling anti-dynamo theorem](astrophysical-fluid-dynamics.md#cowling-anti-dynamo-theorem)
        - [Magnetic concentration by an incompressible stagnation flow](astrophysical-fluid-dynamics.md#magnetic-concentration-by-an-incompressible-stagnation-flow)
          - [Self-similar magnetic mode in a stagnation flow](astrophysical-fluid-dynamics.md#self-similar-magnetic-mode-in-a-stagnation-flow)
        - [Backus' necessary condition for dynamo action](astrophysical-fluid-dynamics.md#backus-necessary-condition-for-dynamo-action)
          - [Maximum-strain bound on dynamo growth](astrophysical-fluid-dynamics.md#maximum-strain-bound-on-dynamo-growth)
        - [Mean-field dynamo](astrophysical-fluid-dynamics.md#mean-field-dynamo)
          - [Mean-field shearing-wave transient amplification](astrophysical-fluid-dynamics.md#mean-field-shearing-wave-transient-amplification)
          - [Dipole and quadrupole parity in a mean-field dynamo](astrophysical-fluid-dynamics.md#dipole-and-quadrupole-parity-in-a-mean-field-dynamo)
            - [Coupled-hemisphere dynamo parity threshold](astrophysical-fluid-dynamics.md#coupled-hemisphere-dynamo-parity-threshold)
            - [Parity splitting of a mean-field dynamo threshold](astrophysical-fluid-dynamics.md#parity-splitting-of-a-mean-field-dynamo-threshold)
          - [Alpha-Omega dynamo](astrophysical-fluid-dynamics.md#alpha-omega-dynamo)
            - [Plane-layer alpha-Omega dynamo threshold](astrophysical-fluid-dynamics.md#plane-layer-alpha-omega-dynamo-threshold)
            - [Alpha-squared Omega dynamo threshold](astrophysical-fluid-dynamics.md#alpha-squared-omega-dynamo-threshold)
            - [Bounded-modulation alpha-Omega growth estimate](astrophysical-fluid-dynamics.md#bounded-modulation-alpha-omega-growth-estimate)
          - [Omega effect](astrophysical-fluid-dynamics.md#omega-effect)
          - [First-order smoothing approximation](astrophysical-fluid-dynamics.md#first-order-smoothing-approximation)
            - [Isotropic alpha effect of three helical traveling waves](astrophysical-fluid-dynamics.md#isotropic-alpha-effect-of-three-helical-traveling-waves)
            - [Helicity formula for isotropic first-order smoothing](astrophysical-fluid-dynamics.md#helicity-formula-for-isotropic-first-order-smoothing)
            - [Quasistatic magnetic response of a helical shearing wave](astrophysical-fluid-dynamics.md#quasistatic-magnetic-response-of-a-helical-shearing-wave)
            - [Monochromatic coupled magnetic and velocity response](astrophysical-fluid-dynamics.md#monochromatic-coupled-magnetic-and-velocity-response)
            - [Oscillatory magnetic response in first-order smoothing](astrophysical-fluid-dynamics.md#oscillatory-magnetic-response-in-first-order-smoothing)
          - [Parker dynamo wave](astrophysical-fluid-dynamics.md#parker-dynamo-wave)
            - [Local alpha-Omega dynamo wave dispersion](astrophysical-fluid-dynamics.md#local-alpha-omega-dynamo-wave-dispersion)
            - [Periodically reversing Parker dynamo coupling](astrophysical-fluid-dynamics.md#periodically-reversing-parker-dynamo-coupling)
          - [Alpha effect](astrophysical-fluid-dynamics.md#alpha-effect)
            - [Rapidly fluctuating alpha effect](astrophysical-fluid-dynamics.md#rapidly-fluctuating-alpha-effect)
            - [Strong-field quenching of an isotropic electromotive force](astrophysical-fluid-dynamics.md#strong-field-quenching-of-an-isotropic-electromotive-force)
            - [Alpha-squared dynamo](astrophysical-fluid-dynamics.md#alpha-squared-dynamo)
              - [Homogeneous alpha-squared dynamo growth criterion](astrophysical-fluid-dynamics.md#homogeneous-alpha-squared-dynamo-growth-criterion)
              - [Anisotropic alpha-squared dynamo](astrophysical-fluid-dynamics.md#anisotropic-alpha-squared-dynamo)
                - [Uniaxial alpha dynamo threshold](astrophysical-fluid-dynamics.md#uniaxial-alpha-dynamo-threshold)
            - [Alpha tensor](astrophysical-fluid-dynamics.md#alpha-tensor)
          - [Mean-field electromotive force](astrophysical-fluid-dynamics.md#mean-field-electromotive-force)
            - [Monochromatic small-Reynolds-number mean electromotive force](astrophysical-fluid-dynamics.md#monochromatic-small-reynolds-number-mean-electromotive-force)
              - [Antisymmetry of the second-order monochromatic alpha tensor](astrophysical-fluid-dynamics.md#antisymmetry-of-the-second-order-monochromatic-alpha-tensor)
              - [Symmetry of the first-order monochromatic alpha tensor](astrophysical-fluid-dynamics.md#symmetry-of-the-first-order-monochromatic-alpha-tensor)
            - [Turbulent magnetic pumping](astrophysical-fluid-dynamics.md#turbulent-magnetic-pumping)
            - [Integrated electromotive response of a finite cyclonic event](astrophysical-fluid-dynamics.md#integrated-electromotive-response-of-a-finite-cyclonic-event)
            - [Space-time average of periodic modes](astrophysical-fluid-dynamics.md#space-time-average-of-periodic-modes)
      - [Hartmann flow](astrophysical-fluid-dynamics.md#hartmann-flow)
        - [Hartmann flow rate with normal-field walls](astrophysical-fluid-dynamics.md#hartmann-flow-rate-with-normal-field-walls)
        - [Hartmann layer](astrophysical-fluid-dynamics.md#hartmann-layer)
        - [Hartmann number](astrophysical-fluid-dynamics.md#hartmann-number)
      - [Normal magnetic field boundary condition](astrophysical-fluid-dynamics.md#normal-magnetic-field-boundary-condition)
      - [Resistive induction equation](astrophysical-fluid-dynamics.md#resistive-induction-equation)
        - [Shearing-coordinate magnetic flux equation](astrophysical-fluid-dynamics.md#shearing-coordinate-magnetic-flux-equation)
        - [Radial magnetic induction scalar](astrophysical-fluid-dynamics.md#radial-magnetic-induction-scalar)
          - [Insulating boundary condition for the radial magnetic scalar](astrophysical-fluid-dynamics.md#insulating-boundary-condition-for-the-radial-magnetic-scalar)
    - [Magnetic diffusion](astrophysical-fluid-dynamics.md#magnetic-diffusion)
      - [Magnetic phase mixing under differential rotation](astrophysical-fluid-dynamics.md#magnetic-phase-mixing-under-differential-rotation)
        - [Exact quadratic-shear magnetic flux solution](astrophysical-fluid-dynamics.md#exact-quadratic-shear-magnetic-flux-solution)
      - [Magnetic free-decay spectral bound](astrophysical-fluid-dynamics.md#magnetic-free-decay-spectral-bound)
      - [Magnetic diffusivity](astrophysical-fluid-dynamics.md#magnetic-diffusivity)
        - [Magnetic Prandtl number](astrophysical-fluid-dynamics.md#magnetic-prandtl-number)
        - [Turbulent magnetic diffusivity](astrophysical-fluid-dynamics.md#turbulent-magnetic-diffusivity)
          - [Variance bound for planar turbulent magnetic transport](astrophysical-fluid-dynamics.md#variance-bound-for-planar-turbulent-magnetic-transport)
    - [Magnetic Reynolds number](astrophysical-fluid-dynamics.md#magnetic-reynolds-number)
    - [Moving-conductor Ohm law](astrophysical-fluid-dynamics.md#moving-conductor-ohm-law)
    - [Magnetoconvection](astrophysical-fluid-dynamics.md#magnetoconvection)
      - [Three-mode porous magnetoconvection](astrophysical-fluid-dynamics.md#three-mode-porous-magnetoconvection)
        - [Cubic centre-manifold reduction of porous magnetoconvection](astrophysical-fluid-dynamics.md#cubic-centre-manifold-reduction-of-porous-magnetoconvection)
      - [Thermal-diffusion scaling of planar magnetoconvection](astrophysical-fluid-dynamics.md#thermal-diffusion-scaling-of-planar-magnetoconvection)
      - [Quasistatic vertical-field magnetoconvection](astrophysical-fluid-dynamics.md#quasistatic-vertical-field-magnetoconvection)
        - [Cubic saturation of quasistatic magnetoconvection](astrophysical-fluid-dynamics.md#cubic-saturation-of-quasistatic-magnetoconvection)
      - [Five-mode vertical-field magnetoconvection](astrophysical-fluid-dynamics.md#five-mode-vertical-field-magnetoconvection)
        - [Conduction double-zero criterion for five-mode magnetoconvection](astrophysical-fluid-dynamics.md#conduction-double-zero-criterion-for-five-mode-magnetoconvection)
        - [Stationary branch of five-mode magnetoconvection](astrophysical-fluid-dynamics.md#stationary-branch-of-five-mode-magnetoconvection)
          - [Pitchfork reversal near geometric ratio two in magnetoconvection](astrophysical-fluid-dynamics.md#pitchfork-reversal-near-geometric-ratio-two-in-magnetoconvection)
      - [Horizontal-field magnetoconvection dispersion relation](astrophysical-fluid-dynamics.md#horizontal-field-magnetoconvection-dispersion-relation)
        - [Strong-field steady magnetoconvection varying along the field](astrophysical-fluid-dynamics.md#strong-field-steady-magnetoconvection-varying-along-the-field)
        - [Magnetic-field-aligned rolls evade steady magnetic inhibition](astrophysical-fluid-dynamics.md#magnetic-field-aligned-rolls-evade-steady-magnetic-inhibition)
      - [Magnetic-to-thermal diffusivity ratio](astrophysical-fluid-dynamics.md#magnetic-to-thermal-diffusivity-ratio)
      - [Subcritical magnetoconvection](astrophysical-fluid-dynamics.md#subcritical-magnetoconvection)
      - [Magnetic flux separation](astrophysical-fluid-dynamics.md#magnetic-flux-separation)
      - [Oblique-field plane-wave magnetoconvection](astrophysical-fluid-dynamics.md#oblique-field-plane-wave-magnetoconvection)
        - [Field-independent stationary threshold in oblique magnetoconvection](astrophysical-fluid-dynamics.md#field-independent-stationary-threshold-in-oblique-magnetoconvection)
        - [Wavenumber selection in oblique-field magnetoconvection](astrophysical-fluid-dynamics.md#wavenumber-selection-in-oblique-field-magnetoconvection)
      - [Vertical-field magnetoconvection dispersion relation](astrophysical-fluid-dynamics.md#vertical-field-magnetoconvection-dispersion-relation)
        - [Three-amplitude vertical-field magnetoconvection](astrophysical-fluid-dynamics.md#three-amplitude-vertical-field-magnetoconvection)
        - [Exact critical Rayleigh relation for vertical-field magnetoconvection](astrophysical-fluid-dynamics.md#exact-critical-rayleigh-relation-for-vertical-field-magnetoconvection)
        - [Strong-field wavenumber selection in magnetoconvection](astrophysical-fluid-dynamics.md#strong-field-wavenumber-selection-in-magnetoconvection)
        - [Oscillatory marginality in vertical-field magnetoconvection](astrophysical-fluid-dynamics.md#oscillatory-marginality-in-vertical-field-magnetoconvection)
          - [Steady-Hopf merger in vertical-field magnetoconvection](astrophysical-fluid-dynamics.md#steady-hopf-merger-in-vertical-field-magnetoconvection)
            - [Merger at a magnetoconvection neutral-curve minimum](astrophysical-fluid-dynamics.md#merger-at-a-magnetoconvection-neutral-curve-minimum)
      - [Chandrasekhar number](astrophysical-fluid-dynamics.md#chandrasekhar-number)
        - [Thermal-diffusion magnetic-field parameter](astrophysical-fluid-dynamics.md#thermal-diffusion-magnetic-field-parameter)
      - [Convection amplitude coupled to a conserved field](astrophysical-fluid-dynamics.md#convection-amplitude-coupled-to-a-conserved-field)
        - [Localized pulse of a conserved-field convection model](astrophysical-fluid-dynamics.md#localized-pulse-of-a-conserved-field-convection-model)
        - [Conserved-field sideband dispersion relation](astrophysical-fluid-dynamics.md#conserved-field-sideband-dispersion-relation)
          - [Long-wave instability with a conserved mean field](astrophysical-fluid-dynamics.md#long-wave-instability-with-a-conserved-mean-field)
    - [Magnetic buoyancy instability](astrophysical-fluid-dynamics.md#magnetic-buoyancy-instability)
      - [Isothermal interchange criterion for magnetic buoyancy](astrophysical-fluid-dynamics.md#isothermal-interchange-criterion-for-magnetic-buoyancy)
      - [Localized interchange criterion for a magnetized atmosphere](astrophysical-fluid-dynamics.md#localized-interchange-criterion-for-a-magnetized-atmosphere)
      - [Parker instability](astrophysical-fluid-dynamics.md#parker-instability)
        - [Long-wavelength undular magnetic buoyancy criterion](astrophysical-fluid-dynamics.md#long-wavelength-undular-magnetic-buoyancy-criterion)
        - [Magnetic buoyancy energy criterion](astrophysical-fluid-dynamics.md#magnetic-buoyancy-energy-criterion)
          - [Short transverse wavelength limit for magnetic buoyancy](astrophysical-fluid-dynamics.md#short-transverse-wavelength-limit-for-magnetic-buoyancy)
    - [Poloidal magnetic field](astrophysical-fluid-dynamics.md#poloidal-magnetic-field)
    - [Magnetic pressure](astrophysical-fluid-dynamics.md#magnetic-pressure)
      - [Magnetic pressure discontinuity in an isothermal atmosphere](astrophysical-fluid-dynamics.md#magnetic-pressure-discontinuity-in-an-isothermal-atmosphere)
      - [Magnetohydrodynamic total pressure](astrophysical-fluid-dynamics.md#magnetohydrodynamic-total-pressure)
    - [Magnetic tension](astrophysical-fluid-dynamics.md#magnetic-tension)
    - [Toroidal magnetic field](astrophysical-fluid-dynamics.md#toroidal-magnetic-field)
      - [Toroidal magnetic-field winding equation](astrophysical-fluid-dynamics.md#toroidal-magnetic-field-winding-equation)
        - [Steady toroidal induction by spherical differential rotation](astrophysical-fluid-dynamics.md#steady-toroidal-induction-by-spherical-differential-rotation)
          - [Diffusive establishment time of a wound toroidal field](astrophysical-fluid-dynamics.md#diffusive-establishment-time-of-a-wound-toroidal-field)
      - [Michael criterion for axisymmetric toroidal-field interchange](astrophysical-fluid-dynamics.md#michael-criterion-for-axisymmetric-toroidal-field-interchange)
        - [Toroidal interchange field threshold in a thin Keplerian disk](astrophysical-fluid-dynamics.md#toroidal-interchange-field-threshold-in-a-thin-keplerian-disk)
        - [Global variational form of the Michael criterion](astrophysical-fluid-dynamics.md#global-variational-form-of-the-michael-criterion)
      - [Uniform-current toroidal-field curl reduction](astrophysical-fluid-dynamics.md#uniform-current-toroidal-field-curl-reduction)
        - [Neutral quadrupolar perturbation of a uniform-current toroidal field](astrophysical-fluid-dynamics.md#neutral-quadrupolar-perturbation-of-a-uniform-current-toroidal-field)
    - [Ideal magnetohydrodynamics](astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamics)
      - [Magnetic relaxation](astrophysical-fluid-dynamics.md#magnetic-relaxation)
        - [Collapse of a planar magnetic separatrix](astrophysical-fluid-dynamics.md#collapse-of-a-planar-magnetic-separatrix)
        - [Viscous magnetic-relaxation energy identity](astrophysical-fluid-dynamics.md#viscous-magnetic-relaxation-energy-identity)
      - [Steady planar ideal-MHD field-line invariants](astrophysical-fluid-dynamics.md#steady-planar-ideal-mhd-field-line-invariants)
        - [Alfvénic degeneracy of steady planar MHD](astrophysical-fluid-dynamics.md#alfvenic-degeneracy-of-steady-planar-mhd)
        - [Planar ideal-MHD Bernoulli invariant](astrophysical-fluid-dynamics.md#planar-ideal-mhd-bernoulli-invariant)
      - [Grad-Shafranov equation](astrophysical-fluid-dynamics.md#grad-shafranov-equation)
        - [Grad-Shafranov equation for a force-free magnetic field](astrophysical-fluid-dynamics.md#grad-shafranov-equation-for-a-force-free-magnetic-field)
      - [Reduced magnetohydrodynamics](astrophysical-fluid-dynamics.md#reduced-magnetohydrodynamics)
        - [Five quadratic cascade invariants of anisotropic magnetohydrodynamic turbulence](astrophysical-fluid-dynamics.md#five-quadratic-cascade-invariants-of-anisotropic-magnetohydrodynamic-turbulence)
        - [Slow and entropy fluctuations in reduced magnetohydrodynamics](astrophysical-fluid-dynamics.md#slow-and-entropy-fluctuations-in-reduced-magnetohydrodynamics)
      - [Ideal magnetohydrodynamic energy conservation](astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamic-energy-conservation)
      - [Ideal magnetohydrodynamic momentum equation](astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamic-momentum-equation)
      - [Plane-parallel magnetohydrodynamic flow with imposed shear](astrophysical-fluid-dynamics.md#plane-parallel-magnetohydrodynamic-flow-with-imposed-shear)
        - [Alfvén-point compatibility in a plane-parallel sheared flow](astrophysical-fluid-dynamics.md#alfven-point-compatibility-in-a-plane-parallel-sheared-flow)
        - [Magnetohydrodynamic shear work](astrophysical-fluid-dynamics.md#magnetohydrodynamic-shear-work)
      - [Ideal magnetohydrodynamic equations](astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamic-equations)
      - [Magnetohydrodynamic energy principle](astrophysical-fluid-dynamics.md#magnetohydrodynamic-energy-principle)
        - [Incompressible magnetic displacement energy identity](astrophysical-fluid-dynamics.md#incompressible-magnetic-displacement-energy-identity)
          - [Interchange stability of an incompressible magnetized atmosphere](astrophysical-fluid-dynamics.md#interchange-stability-of-an-incompressible-magnetized-atmosphere)
        - [Linear displacement equations for a magnetized atmosphere](astrophysical-fluid-dynamics.md#linear-displacement-equations-for-a-magnetized-atmosphere)
      - [Elsässer variable](astrophysical-fluid-dynamics.md#elsasser-variable)
        - [Elsässer energy invariant](astrophysical-fluid-dynamics.md#elsasser-energy-invariant)
      - [Cross-helicity](astrophysical-fluid-dynamics.md#cross-helicity)
        - [Cross-helicity conservation law](astrophysical-fluid-dynamics.md#cross-helicity-conservation-law)
          - [Material conservation of cross-helicity density](astrophysical-fluid-dynamics.md#material-conservation-of-cross-helicity-density)
      - [Magnetic flux freezing](astrophysical-fluid-dynamics.md#magnetic-flux-freezing)
        - [Flux-surface preservation during magnetic-tube expansion](astrophysical-fluid-dynamics.md#flux-surface-preservation-during-magnetic-tube-expansion)
        - [Mass-to-flux ratio](astrophysical-fluid-dynamics.md#mass-to-flux-ratio)
          - [Critical mass-to-flux ratio](astrophysical-fluid-dynamics.md#critical-mass-to-flux-ratio)
      - [Alfvén speed](astrophysical-fluid-dynamics.md#alfven-speed)
        - [Alfvén Mach number](astrophysical-fluid-dynamics.md#alfven-mach-number)
        - [Alfvén velocity](astrophysical-fluid-dynamics.md#alfven-velocity)
        - [Alfvén number](astrophysical-fluid-dynamics.md#alfven-number)
      - [Magnetohydrodynamic wave](astrophysical-fluid-dynamics.md#magnetohydrodynamic-wave)
        - [Ambipolar damping](astrophysical-fluid-dynamics.md#ambipolar-damping)
          - [Equal-density ion-neutral Alfvén dispersion relation](astrophysical-fluid-dynamics.md#equal-density-ion-neutral-alfven-dispersion-relation)
            - [Strong-collision ion-neutral Alfvén modes](astrophysical-fluid-dynamics.md#strong-collision-ion-neutral-alfven-modes)
        - [Entropy mode](astrophysical-fluid-dynamics.md#entropy-mode)
        - [Magnetohydrodynamic wave polarization](astrophysical-fluid-dynamics.md#magnetohydrodynamic-wave-polarization)
        - [Uniform-current rotating magnetohydrodynamic wave dispersion](astrophysical-fluid-dynamics.md#uniform-current-rotating-magnetohydrodynamic-wave-dispersion)
          - [Single-azimuthal-mode current-driven instability threshold](astrophysical-fluid-dynamics.md#single-azimuthal-mode-current-driven-instability-threshold)
        - [Alfvén wave](astrophysical-fluid-dynamics.md#alfven-wave)
          - [Alfvén-resonant vorticity in a parallel magnetic shear flow](astrophysical-fluid-dynamics.md#alfven-resonant-vorticity-in-a-parallel-magnetic-shear-flow)
          - [Kinetic Alfvén wave](astrophysical-fluid-dynamics.md#kinetic-alfven-wave)
          - [Magnetohydrodynamic phase mixing](astrophysical-fluid-dynamics.md#magnetohydrodynamic-phase-mixing)
          - [Torsional Alfvén wave](astrophysical-fluid-dynamics.md#torsional-alfven-wave)
            - [Pressure compatibility of nonlinear torsional Alfvén profiles](astrophysical-fluid-dynamics.md#pressure-compatibility-of-nonlinear-torsional-alfven-profiles)
            - [Cylinder-averaged torsional Alfvén wave](astrophysical-fluid-dynamics.md#cylinder-averaged-torsional-alfven-wave)
              - [Conserved energy of a cylinder-averaged torsional wave](astrophysical-fluid-dynamics.md#conserved-energy-of-a-cylinder-averaged-torsional-wave)
            - [Magnetic axial angular momentum flux](astrophysical-fluid-dynamics.md#magnetic-axial-angular-momentum-flux)
          - [Nonlinear Alfvén wave](astrophysical-fluid-dynamics.md#nonlinear-alfven-wave)
            - [Magnetic-pressure obstruction to a linearly polarized Alfvén wave](astrophysical-fluid-dynamics.md#magnetic-pressure-obstruction-to-a-linearly-polarized-alfven-wave)
            - [Circularly polarized nonlinear Alfvén wave](astrophysical-fluid-dynamics.md#circularly-polarized-nonlinear-alfven-wave)
          - [Alfvén characteristic eigenvector](astrophysical-fluid-dynamics.md#alfven-characteristic-eigenvector)
          - [Alfvén frequency](astrophysical-fluid-dynamics.md#alfven-frequency)
          - [Alfvén wing](astrophysical-fluid-dynamics.md#alfven-wing)
            - [Alfvénic Mach-cone slope](astrophysical-fluid-dynamics.md#alfvenic-mach-cone-slope)
        - [Magnetosonic wave](astrophysical-fluid-dynamics.md#magnetosonic-wave)
          - [High-pressure limit of magnetosonic waves](astrophysical-fluid-dynamics.md#high-pressure-limit-of-magnetosonic-waves)
            - [Pseudo-Alfvén wave](astrophysical-fluid-dynamics.md#pseudo-alfven-wave)
          - [Isothermal coplanar magnetohydrodynamic characteristic matrix](astrophysical-fluid-dynamics.md#isothermal-coplanar-magnetohydrodynamic-characteristic-matrix)
          - [Magnetosonic critical speed](astrophysical-fluid-dynamics.md#magnetosonic-critical-speed)
            - [Regularity at a magnetosonic point](astrophysical-fluid-dynamics.md#regularity-at-a-magnetosonic-point)
              - [Cold-limit degeneracy of a slow magnetosonic point](astrophysical-fluid-dynamics.md#cold-limit-degeneracy-of-a-slow-magnetosonic-point)
          - [Fast magnetosonic wave](astrophysical-fluid-dynamics.md#fast-magnetosonic-wave)
          - [Slow magnetosonic wave](astrophysical-fluid-dynamics.md#slow-magnetosonic-wave)
          - [Tube speed](astrophysical-fluid-dynamics.md#tube-speed)
        - [Magnetohydrodynamic interface wave](astrophysical-fluid-dynamics.md#magnetohydrodynamic-interface-wave)
          - [Magnetic stabilization of an equal-density vortex sheet](astrophysical-fluid-dynamics.md#magnetic-stabilization-of-an-equal-density-vortex-sheet)
      - [Force-free magnetic field](astrophysical-fluid-dynamics.md#force-free-magnetic-field)
        - [Magnetic-energy injection by differential boundary rotation](astrophysical-fluid-dynamics.md#magnetic-energy-injection-by-differential-boundary-rotation)
        - [Force-free parameter](astrophysical-fluid-dynamics.md#force-free-parameter)
        - [Cylindrical force-free magnetic field](astrophysical-fluid-dynamics.md#cylindrical-force-free-magnetic-field)
      - [Linearized ideal magnetohydrodynamic equations](astrophysical-fluid-dynamics.md#linearized-ideal-magnetohydrodynamic-equations)
        - [Displacement equation for a parallel magnetic shear flow](astrophysical-fluid-dynamics.md#displacement-equation-for-a-parallel-magnetic-shear-flow)
      - [Ideal magnetohydrodynamic induction equation](astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamic-induction-equation)
        - [Ideal magnetic response to a cylindrical cyclonic event](astrophysical-fluid-dynamics.md#ideal-magnetic-response-to-a-cylindrical-cyclonic-event)
        - [Cartesian magnetic flux function](astrophysical-fluid-dynamics.md#cartesian-magnetic-flux-function)
          - [Magnetic island](astrophysical-fluid-dynamics.md#magnetic-island)
          - [Cartesian magnetostatic flux-function equilibrium](astrophysical-fluid-dynamics.md#cartesian-magnetostatic-flux-function-equilibrium)
        - [Axisymmetric magnetic winding](astrophysical-fluid-dynamics.md#axisymmetric-magnetic-winding)
          - [Magnetic-pressure equality radius under Keplerian winding](astrophysical-fluid-dynamics.md#magnetic-pressure-equality-radius-under-keplerian-winding)
          - [Ferraro's law of isorotation](astrophysical-fluid-dynamics.md#ferraro-s-law-of-isorotation)
      - [Entropy advection equation](astrophysical-fluid-dynamics.md#entropy-advection-equation)
      - [Magnetohydrodynamic shock](astrophysical-fluid-dynamics.md#magnetohydrodynamic-shock)
        - [Perpendicular magnetohydrodynamic shock](astrophysical-fluid-dynamics.md#perpendicular-magnetohydrodynamic-shock)
          - [Compression ratio of a perpendicular magnetohydrodynamic shock](astrophysical-fluid-dynamics.md#compression-ratio-of-a-perpendicular-magnetohydrodynamic-shock)
        - [Parallel magnetohydrodynamic shock](astrophysical-fluid-dynamics.md#parallel-magnetohydrodynamic-shock)
        - [Ideal magnetohydrodynamic shock conditions](astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamic-shock-conditions)
        - [de Hoffmann–Teller frame](astrophysical-fluid-dynamics.md#de-hoffmann-teller-frame)
        - [Rotational discontinuity in magnetohydrodynamics](astrophysical-fluid-dynamics.md#rotational-discontinuity-in-magnetohydrodynamics)
      - [Axisymmetric magnetostatic Grad-Shafranov system](astrophysical-fluid-dynamics.md#axisymmetric-magnetostatic-grad-shafranov-system)
      - [Axisymmetric magnetohydrodynamic wind](astrophysical-fluid-dynamics.md#axisymmetric-magnetohydrodynamic-wind)
        - [Cold radial magnetohydrodynamic wind integral](astrophysical-fluid-dynamics.md#cold-radial-magnetohydrodynamic-wind-integral)
        - [Sub-Alfvénic isorotation in a steady axisymmetric wind](astrophysical-fluid-dynamics.md#sub-alfvenic-isorotation-in-a-steady-axisymmetric-wind)
        - [Corotating energy invariant of an axisymmetric magnetic wind](astrophysical-fluid-dynamics.md#corotating-energy-invariant-of-an-axisymmetric-magnetic-wind)
        - [Field-line angular velocity of an axisymmetric wind](astrophysical-fluid-dynamics.md#field-line-angular-velocity-of-an-axisymmetric-wind)
        - [Poloidal magnetic flux function](astrophysical-fluid-dynamics.md#poloidal-magnetic-flux-function)
          - [Material advection of an axisymmetric magnetic flux function](astrophysical-fluid-dynamics.md#material-advection-of-an-axisymmetric-magnetic-flux-function)
          - [Axisymmetric magnetic flux surface](astrophysical-fluid-dynamics.md#axisymmetric-magnetic-flux-surface)
          - [Power-law poloidal field near a disk surface](astrophysical-fluid-dynamics.md#power-law-poloidal-field-near-a-disk-surface)
        - [Magnetohydrodynamic mass loading](astrophysical-fluid-dynamics.md#magnetohydrodynamic-mass-loading)
          - [Regular-axis alignment of steady poloidal ideal flow](astrophysical-fluid-dynamics.md#regular-axis-alignment-of-steady-poloidal-ideal-flow)
        - [Field-line angular velocity](astrophysical-fluid-dynamics.md#field-line-angular-velocity)
        - [Magnetohydrodynamic angular-momentum invariant](astrophysical-fluid-dynamics.md#magnetohydrodynamic-angular-momentum-invariant)
          - [Maxwell torque conservation in an axisymmetric wind](astrophysical-fluid-dynamics.md#maxwell-torque-conservation-in-an-axisymmetric-wind)
        - [Magnetohydrodynamic Bernoulli invariant](astrophysical-fluid-dynamics.md#magnetohydrodynamic-bernoulli-invariant)
          - [Isothermal magnetic Bernoulli integral](astrophysical-fluid-dynamics.md#isothermal-magnetic-bernoulli-integral)
        - [Alfvén surface](astrophysical-fluid-dynamics.md#alfven-surface)
          - [Alfvén radius](astrophysical-fluid-dynamics.md#alfven-radius)
          - [Alfvén-surface regularity condition for an axisymmetric wind](astrophysical-fluid-dynamics.md#alfven-surface-regularity-condition-for-an-axisymmetric-wind)
        - [Asymptotic energy of a radial magnetohydrodynamic wind](astrophysical-fluid-dynamics.md#asymptotic-energy-of-a-radial-magnetohydrodynamic-wind)
        - [Magnetocentrifugal acceleration](astrophysical-fluid-dynamics.md#magnetocentrifugal-acceleration)
          - [Thirty-degree magnetocentrifugal launching criterion](astrophysical-fluid-dynamics.md#thirty-degree-magnetocentrifugal-launching-criterion)
            - [Marginal straight-line launch at thirty degrees](astrophysical-fluid-dynamics.md#marginal-straight-line-launch-at-thirty-degrees)
          - [Magnetocentrifugal launching criterion in a flattened power-law potential](astrophysical-fluid-dynamics.md#magnetocentrifugal-launching-criterion-in-a-flattened-power-law-potential)
  - [Self-gravitating gaseous filament](astrophysical-fluid-dynamics.md#self-gravitating-gaseous-filament)
    - [Magnetized self-gravitating filament](astrophysical-fluid-dynamics.md#magnetized-self-gravitating-filament)
    - [Line mass](astrophysical-fluid-dynamics.md#line-mass)
  - [Parker wind](astrophysical-fluid-dynamics.md#parker-wind)
    - [Polytropic Parker wind](astrophysical-fluid-dynamics.md#polytropic-parker-wind)
      - [Parker wind equation](astrophysical-fluid-dynamics.md#parker-wind-equation)
- [Geophysical fluid dynamics](geophysical-fluid-dynamics.md)
  - [Ekman number](geophysical-fluid-dynamics.md#ekman-number)
  - [Deacon cell](geophysical-fluid-dynamics.md#deacon-cell)
    - [Eddy-induced overturning](geophysical-fluid-dynamics.md#eddy-induced-overturning)
    - [Meridional overturning streamfunction](geophysical-fluid-dynamics.md#meridional-overturning-streamfunction)
  - [Deformation radius](geophysical-fluid-dynamics.md#deformation-radius)
    - [Two-layer internal deformation radius](geophysical-fluid-dynamics.md#two-layer-internal-deformation-radius)
  - [Burger number](geophysical-fluid-dynamics.md#burger-number)
  - [General circulation model](geophysical-fluid-dynamics.md#general-circulation-model)
  - [Eulerian mean flow](geophysical-fluid-dynamics.md#eulerian-mean-flow)
  - [Thermal wind](geophysical-fluid-dynamics.md#thermal-wind)
    - [Geostrophic thermal wind with separable buoyancy](geophysical-fluid-dynamics.md#geostrophic-thermal-wind-with-separable-buoyancy)
  - [Log-pressure coordinate](geophysical-fluid-dynamics.md#log-pressure-coordinate)
  - [Rossby number](geophysical-fluid-dynamics.md#rossby-number)
    - [Stellar activity Rossby number](geophysical-fluid-dynamics.md#stellar-activity-rossby-number)
  - [Burgers number](geophysical-fluid-dynamics.md#burgers-number)
  - [Boussinesq approximation](geophysical-fluid-dynamics.md#boussinesq-approximation)
    - [Strong Boussinesq approximation](geophysical-fluid-dynamics.md#strong-boussinesq-approximation)
    - [Stratification–rotation analogy](geophysical-fluid-dynamics.md#stratification-rotation-analogy)
      - [Causal pressure adjustment by internal waves](geophysical-fluid-dynamics.md#causal-pressure-adjustment-by-internal-waves)
        - [Hydrostatic response to a localized horizontal force](geophysical-fluid-dynamics.md#hydrostatic-response-to-a-localized-horizontal-force)
    - [Boussinesq up-down symmetry](geophysical-fluid-dynamics.md#boussinesq-up-down-symmetry)
    - [Boussinesq equations](geophysical-fluid-dynamics.md#boussinesq-equations)
      - [Linearized Boussinesq equations](geophysical-fluid-dynamics.md#linearized-boussinesq-equations)
    - [Inertial wave](geophysical-fluid-dynamics.md#inertial-wave)
      - [Inertial modes in a rigid rotating sphere](geophysical-fluid-dynamics.md#inertial-modes-in-a-rigid-rotating-sphere)
        - [Cubic axisymmetric inertial mode of a rigid sphere](geophysical-fluid-dynamics.md#cubic-axisymmetric-inertial-mode-of-a-rigid-sphere)
  - [Rotating fluid](geophysical-fluid-dynamics.md#rotating-fluid)
    - [Taylor–Proudman theorem](geophysical-fluid-dynamics.md#taylor-proudman-theorem)
      - [Geostrophic contour](geophysical-fluid-dynamics.md#geostrophic-contour)
    - [Taylor number](geophysical-fluid-dynamics.md#taylor-number)
    - [Traditional approximation (geophysical fluid dynamics)](geophysical-fluid-dynamics.md#traditional-approximation-geophysical-fluid-dynamics)
    - [Coriolis parameter](geophysical-fluid-dynamics.md#coriolis-parameter)
      - [f-plane](geophysical-fluid-dynamics.md#f-plane)
      - [beta plane](geophysical-fluid-dynamics.md#beta-plane)
      - [Inertial oscillation](geophysical-fluid-dynamics.md#inertial-oscillation)
        - [Beta drift of an inertial oscillation](geophysical-fluid-dynamics.md#beta-drift-of-an-inertial-oscillation)
  - [Potential vorticity](geophysical-fluid-dynamics.md#potential-vorticity)
    - [Potential-vorticity inversion](geophysical-fluid-dynamics.md#potential-vorticity-inversion)
      - [Two-dimensional potential-vorticity inversion](geophysical-fluid-dynamics.md#two-dimensional-potential-vorticity-inversion)
      - [Shallow-water quasi-geostrophic inversion](geophysical-fluid-dynamics.md#shallow-water-quasi-geostrophic-inversion)
      - [Stratified quasi-geostrophic inversion](geophysical-fluid-dynamics.md#stratified-quasi-geostrophic-inversion)
        - [Prandtl ratio of scales](geophysical-fluid-dynamics.md#prandtl-ratio-of-scales)
        - [Stretched coordinates for quasi-geostrophic inversion](geophysical-fluid-dynamics.md#stretched-coordinates-for-quasi-geostrophic-inversion)
          - [Spherical potential-vorticity anomaly](geophysical-fluid-dynamics.md#spherical-potential-vorticity-anomaly)
    - [Potential-vorticity gradient](geophysical-fluid-dynamics.md#potential-vorticity-gradient)
    - [Potential-vorticity evolution equation](geophysical-fluid-dynamics.md#potential-vorticity-evolution-equation)
      - [Potential-vorticity conservation](geophysical-fluid-dynamics.md#potential-vorticity-conservation)
        - [Momentum loss from uniform potential-vorticity mixing](geophysical-fluid-dynamics.md#momentum-loss-from-uniform-potential-vorticity-mixing)
          - [Rossby-wave PV mixing and zonal momentum](geophysical-fluid-dynamics.md#rossby-wave-pv-mixing-and-zonal-momentum)
    - [Ertel potential vorticity](geophysical-fluid-dynamics.md#ertel-potential-vorticity)
      - [Ertel's theorem](geophysical-fluid-dynamics.md#ertel-s-theorem)
    - [Shallow-water potential vorticity](geophysical-fluid-dynamics.md#shallow-water-potential-vorticity)
      - [Circular topographic anticyclone](geophysical-fluid-dynamics.md#circular-topographic-anticyclone)
        - [Closed-streamline threshold for a circular topographic anticyclone](geophysical-fluid-dynamics.md#closed-streamline-threshold-for-a-circular-topographic-anticyclone)
      - [Zero-potential-vorticity rotating channel flow](geophysical-fluid-dynamics.md#zero-potential-vorticity-rotating-channel-flow)
        - [Hydraulic control of a zero-PV rotating channel](geophysical-fluid-dynamics.md#hydraulic-control-of-a-zero-pv-rotating-channel)
      - [Linearized shallow-water potential-vorticity anomaly](geophysical-fluid-dynamics.md#linearized-shallow-water-potential-vorticity-anomaly)
      - [Shallow-water quasi-geostrophic potential vorticity](geophysical-fluid-dynamics.md#shallow-water-quasi-geostrophic-potential-vorticity)
        - [Cosine-ridge shallow-water geostrophic response](geophysical-fluid-dynamics.md#cosine-ridge-shallow-water-geostrophic-response)
        - [Uniform-current obstruction to constant shallow-water QG potential vorticity](geophysical-fluid-dynamics.md#uniform-current-obstruction-to-constant-shallow-water-qg-potential-vorticity)
          - [Gaussian topographic response with compensated uniform potential vorticity](geophysical-fluid-dynamics.md#gaussian-topographic-response-with-compensated-uniform-potential-vorticity)
            - [Closed-streamline threshold for a Gaussian disturbance in uniform flow](geophysical-fluid-dynamics.md#closed-streamline-threshold-for-a-gaussian-disturbance-in-uniform-flow)
        - [Potential-vorticity mixing over a finite bottom slope](geophysical-fluid-dynamics.md#potential-vorticity-mixing-over-a-finite-bottom-slope)
        - [Potential-vorticity step edge wave](geophysical-fluid-dynamics.md#potential-vorticity-step-edge-wave)
        - [Barotropic deformation radius](geophysical-fluid-dynamics.md#barotropic-deformation-radius)
  - [Quasi-geostrophic approximation](geophysical-fluid-dynamics.md#quasi-geostrophic-approximation)
    - [Two-layer quasi-geostrophic potential vorticity](geophysical-fluid-dynamics.md#two-layer-quasi-geostrophic-potential-vorticity)
      - [Two-layer quasi-geostrophic energy conservation](geophysical-fluid-dynamics.md#two-layer-quasi-geostrophic-energy-conservation)
        - [Baroclinic energy ratio and deformation scale](geophysical-fluid-dynamics.md#baroclinic-energy-ratio-and-deformation-scale)
      - [Vortex stretching in layered quasi-geostrophic flow](geophysical-fluid-dynamics.md#vortex-stretching-in-layered-quasi-geostrophic-flow)
    - [Quasi-geostrophic omega equation](geophysical-fluid-dynamics.md#quasi-geostrophic-omega-equation)
    - [Quasi-geostrophic streamfunction](geophysical-fluid-dynamics.md#quasi-geostrophic-streamfunction)
    - [Geostrophic flow](geophysical-fluid-dynamics.md#geostrophic-flow)
      - [Strict geostrophic balance](geophysical-fluid-dynamics.md#strict-geostrophic-balance)
    - [Ageostrophic flow](geophysical-fluid-dynamics.md#ageostrophic-flow)
    - [Three-dimensional quasi-geostrophic potential vorticity](geophysical-fluid-dynamics.md#three-dimensional-quasi-geostrophic-potential-vorticity)
      - [Reference-buoyancy convention in quasi-geostrophic potential vorticity](geophysical-fluid-dynamics.md#reference-buoyancy-convention-in-quasi-geostrophic-potential-vorticity)
      - [Quasi-geostrophic vertical mode](geophysical-fluid-dynamics.md#quasi-geostrophic-vertical-mode)
        - [Barotropic mode](geophysical-fluid-dynamics.md#barotropic-mode)
        - [Baroclinic mode](geophysical-fluid-dynamics.md#baroclinic-mode)
      - [Quasi-geostrophic potential-vorticity equation](geophysical-fluid-dynamics.md#quasi-geostrophic-potential-vorticity-equation)
        - [Topographic buoyancy boundary condition for quasi-geostrophic flow](geophysical-fluid-dynamics.md#topographic-buoyancy-boundary-condition-for-quasi-geostrophic-flow)
        - [Rigid-boundary buoyancy condition for quasi-geostrophic waves](geophysical-fluid-dynamics.md#rigid-boundary-buoyancy-condition-for-quasi-geostrophic-waves)
        - [Diabatically forced quasi-geostrophic potential vorticity](geophysical-fluid-dynamics.md#diabatically-forced-quasi-geostrophic-potential-vorticity)
          - [Harmonic heating response of quasi-geostrophic flow](geophysical-fluid-dynamics.md#harmonic-heating-response-of-quasi-geostrophic-flow)
          - [Steady quasi-geostrophic response to localized heating](geophysical-fluid-dynamics.md#steady-quasi-geostrophic-response-to-localized-heating)
      - [Log-pressure quasi-geostrophic potential vorticity](geophysical-fluid-dynamics.md#log-pressure-quasi-geostrophic-potential-vorticity)
        - [Vertical-advection consistency criterion for log-pressure quasi-geostrophy](geophysical-fluid-dynamics.md#vertical-advection-consistency-criterion-for-log-pressure-quasi-geostrophy)
      - [Isopycnal displacement](geophysical-fluid-dynamics.md#isopycnal-displacement)
      - [Quasi-geostrophic mountain wave](geophysical-fluid-dynamics.md#quasi-geostrophic-mountain-wave)
        - [Resonant topographic quasi-geostrophic wave](geophysical-fluid-dynamics.md#resonant-topographic-quasi-geostrophic-wave)
          - [Phase of a resonantly forced topographic edge wave](geophysical-fluid-dynamics.md#phase-of-a-resonantly-forced-topographic-edge-wave)
        - [Thermally damped quasi-geostrophic mountain wave](geophysical-fluid-dynamics.md#thermally-damped-quasi-geostrophic-mountain-wave)
  - [Geostrophic adjustment](geophysical-fluid-dynamics.md#geostrophic-adjustment)
    - [Geostrophic adjustment of a Gaussian height ridge](geophysical-fluid-dynamics.md#geostrophic-adjustment-of-a-gaussian-height-ridge)
    - [Geostrophic adjustment of a finite-width height ramp](geophysical-fluid-dynamics.md#geostrophic-adjustment-of-a-finite-width-height-ramp)
    - [Coastal adjustment of an elevated strip](geophysical-fluid-dynamics.md#coastal-adjustment-of-an-elevated-strip)
    - [Balanced shallow-water energy as a signed potential-vorticity pairing](geophysical-fluid-dynamics.md#balanced-shallow-water-energy-as-a-signed-potential-vorticity-pairing)
    - [Geostrophic adjustment of a finite-width current](geophysical-fluid-dynamics.md#geostrophic-adjustment-of-a-finite-width-current)
      - [Energy retention in finite-width geostrophic adjustment](geophysical-fluid-dynamics.md#energy-retention-in-finite-width-geostrophic-adjustment)
    - [Geostrophic adjustment of a surface-height jump](geophysical-fluid-dynamics.md#geostrophic-adjustment-of-a-surface-height-jump)
    - [Inertia-gravity wave](geophysical-fluid-dynamics.md#inertia-gravity-wave)
      - [Linear pressure equation for rotating stratified flow](geophysical-fluid-dynamics.md#linear-pressure-equation-for-rotating-stratified-flow)
      - [Particle ellipses for rotating shallow-water waves](geophysical-fluid-dynamics.md#particle-ellipses-for-rotating-shallow-water-waves)
      - [External gravity wave](geophysical-fluid-dynamics.md#external-gravity-wave)
      - [Linear rotating shallow-water dispersion relation](geophysical-fluid-dynamics.md#linear-rotating-shallow-water-dispersion-relation)
    - [Kelvin wave](geophysical-fluid-dynamics.md#kelvin-wave)
      - [Kelvin-wave channel invariant](geophysical-fluid-dynamics.md#kelvin-wave-channel-invariant)
  - [Ocean circulation](geophysical-fluid-dynamics.md#ocean-circulation)
    - [Antarctic Convergence](geophysical-fluid-dynamics.md#antarctic-convergence)
    - [Antarctic Coastal Current](geophysical-fluid-dynamics.md#antarctic-coastal-current)
    - [Antarctic Circumpolar Current](geophysical-fluid-dynamics.md#antarctic-circumpolar-current)
    - [Antarctic bottom water](geophysical-fluid-dynamics.md#antarctic-bottom-water)
    - [Wind stress](geophysical-fluid-dynamics.md#wind-stress)
      - [Wind stress curl](geophysical-fluid-dynamics.md#wind-stress-curl)
      - [Ekman layer](geophysical-fluid-dynamics.md#ekman-layer)
        - [Laminar Ekman boundary stress](geophysical-fluid-dynamics.md#laminar-ekman-boundary-stress)
        - [Surface Ekman layer](geophysical-fluid-dynamics.md#surface-ekman-layer)
        - [Bottom Ekman layer](geophysical-fluid-dynamics.md#bottom-ekman-layer)
      - [Ekman transport](geophysical-fluid-dynamics.md#ekman-transport)
        - [Ekman pumping](geophysical-fluid-dynamics.md#ekman-pumping)
          - [Ekman spin-down in a shallow-water layer](geophysical-fluid-dynamics.md#ekman-spin-down-in-a-shallow-water-layer)
          - [Quasi-geostrophic Ekman spin-down](geophysical-fluid-dynamics.md#quasi-geostrophic-ekman-spin-down)
      - [Ocean gyre](geophysical-fluid-dynamics.md#ocean-gyre)
        - [Sverdrup balance](geophysical-fluid-dynamics.md#sverdrup-balance)
          - [Ocean basin equation with bottom drag and lateral viscosity](geophysical-fluid-dynamics.md#ocean-basin-equation-with-bottom-drag-and-lateral-viscosity)
            - [Drag-dominated basin solution with no-slip layers](geophysical-fluid-dynamics.md#drag-dominated-basin-solution-with-no-slip-layers)
          - [Two-layer Sverdrup interior](geophysical-fluid-dynamics.md#two-layer-sverdrup-interior)
            - [Linear stability of a meridional two-layer current](geophysical-fluid-dynamics.md#linear-stability-of-a-meridional-two-layer-current)
              - [Meridional-wave instability of a two-layer Sverdrup flow](geophysical-fluid-dynamics.md#meridional-wave-instability-of-a-two-layer-sverdrup-flow)
            - [Potential-vorticity gradients in a meridional two-layer current](geophysical-fluid-dynamics.md#potential-vorticity-gradients-in-a-meridional-two-layer-current)
          - [Point-forced Sverdrup–drag Green function](geophysical-fluid-dynamics.md#point-forced-sverdrup-drag-green-function)
          - [Ocean transport streamfunction](geophysical-fluid-dynamics.md#ocean-transport-streamfunction)
            - [Relative vorticity from a variable-depth transport streamfunction](geophysical-fluid-dynamics.md#relative-vorticity-from-a-variable-depth-transport-streamfunction)
          - [Godfrey island rule](geophysical-fluid-dynamics.md#godfrey-island-rule)
          - [Topographic Sverdrup balance](geophysical-fluid-dynamics.md#topographic-sverdrup-balance)
            - [Wind-driven circulation over parabolic basin topography](geophysical-fluid-dynamics.md#wind-driven-circulation-over-parabolic-basin-topography)
            - [Topographic potential-vorticity pseudovelocity](geophysical-fluid-dynamics.md#topographic-potential-vorticity-pseudovelocity)
            - [Topographic potential-vorticity steering](geophysical-fluid-dynamics.md#topographic-potential-vorticity-steering)
        - [Western boundary current](geophysical-fluid-dynamics.md#western-boundary-current)
          - [Stommel boundary layer](geophysical-fluid-dynamics.md#stommel-boundary-layer)
          - [Munk boundary layer](geophysical-fluid-dynamics.md#munk-boundary-layer)
  - [Rossby wave](geophysical-fluid-dynamics.md#rossby-wave)
    - [Rossby-wave equation for a sheared zonal current](geophysical-fluid-dynamics.md#rossby-wave-equation-for-a-sheared-zonal-current)
      - [Local Rossby-wave dispersion relation in a zonal jet](geophysical-fluid-dynamics.md#local-rossby-wave-dispersion-relation-in-a-zonal-jet)
        - [Stationary Rossby waves in a sinusoidal zonal jet](geophysical-fluid-dynamics.md#stationary-rossby-waves-in-a-sinusoidal-zonal-jet)
    - [Linear Rossby-wave equation](geophysical-fluid-dynamics.md#linear-rossby-wave-equation)
      - [Shallow-water Rossby-wave dispersion relation](geophysical-fluid-dynamics.md#shallow-water-rossby-wave-dispersion-relation)
        - [Reflection of a Rossby wave at a meridional wall](geophysical-fluid-dynamics.md#reflection-of-a-rossby-wave-at-a-meridional-wall)
        - [Rossby-wave isofrequency circle](geophysical-fluid-dynamics.md#rossby-wave-isofrequency-circle)
    - [Topographic Rossby-wave dispersion relation](geophysical-fluid-dynamics.md#topographic-rossby-wave-dispersion-relation)
      - [Square-basin topographic Rossby mode](geophysical-fluid-dynamics.md#square-basin-topographic-rossby-mode)
      - [Step-trapped topographic Rossby wave](geophysical-fluid-dynamics.md#step-trapped-topographic-rossby-wave)
        - [Double Kelvin-wave adjustment at a depth step](geophysical-fluid-dynamics.md#double-kelvin-wave-adjustment-at-a-depth-step)
        - [Long-wave transport along a depth step](geophysical-fluid-dynamics.md#long-wave-transport-along-a-depth-step)
    - [Barotropic Rossby wave](geophysical-fluid-dynamics.md#barotropic-rossby-wave)
      - [Stationary Rossby-wave ray envelope](geophysical-fluid-dynamics.md#stationary-rossby-wave-ray-envelope)
    - [Baroclinic Rossby wave](geophysical-fluid-dynamics.md#baroclinic-rossby-wave)
      - [Rossby wave in a log-pressure atmosphere](geophysical-fluid-dynamics.md#rossby-wave-in-a-log-pressure-atmosphere)
  - [Wave activity](geophysical-fluid-dynamics.md#wave-activity)
    - [Wave action (fluid dynamics)](geophysical-fluid-dynamics.md#wave-action-fluid-dynamics)
      - [Wave pseudomomentum](geophysical-fluid-dynamics.md#wave-pseudomomentum)
    - [Quasi-geostrophic wave pseudomomentum](geophysical-fluid-dynamics.md#quasi-geostrophic-wave-pseudomomentum)
  - [Equatorial wave](geophysical-fluid-dynamics.md#equatorial-wave)
    - [Equivalent depth](geophysical-fluid-dynamics.md#equivalent-depth)
    - [Equatorial shallow-water dispersion relation](geophysical-fluid-dynamics.md#equatorial-shallow-water-dispersion-relation)
      - [Equatorial wave velocity polarization](geophysical-fluid-dynamics.md#equatorial-wave-velocity-polarization)
      - [Frequency gap for higher equatorial wave modes](geophysical-fluid-dynamics.md#frequency-gap-for-higher-equatorial-wave-modes)
    - [Equatorial Kelvin wave](geophysical-fluid-dynamics.md#equatorial-kelvin-wave)
    - [Equatorial Rossby wave](geophysical-fluid-dynamics.md#equatorial-rossby-wave)
      - [Equatorial Rossby-wave dispersion relation](geophysical-fluid-dynamics.md#equatorial-rossby-wave-dispersion-relation)
    - [Equatorial inertia--gravity wave](geophysical-fluid-dynamics.md#equatorial-inertia-gravity-wave)
    - [Rossby-gravity waves](geophysical-fluid-dynamics.md#rossby-gravity-waves)
      - [Exceptional root of the mixed Rossby-gravity mode](geophysical-fluid-dynamics.md#exceptional-root-of-the-mixed-rossby-gravity-mode)
    - [Damped equatorial Kelvin and Rossby response](geophysical-fluid-dynamics.md#damped-equatorial-kelvin-and-rossby-response)
  - [Transformed Eulerian mean](geophysical-fluid-dynamics.md#transformed-eulerian-mean)
    - [Eddy buoyancy flux](geophysical-fluid-dynamics.md#eddy-buoyancy-flux)
    - [Eliassen–Palm flux](geophysical-fluid-dynamics.md#eliassen-palm-flux)
      - [Taylor identity for quasi-geostrophic flux](geophysical-fluid-dynamics.md#taylor-identity-for-quasi-geostrophic-flux)
      - [Non-acceleration theorem for quasi-geostrophic waves](geophysical-fluid-dynamics.md#non-acceleration-theorem-for-quasi-geostrophic-waves)
      - [Wave-activity deposition](geophysical-fluid-dynamics.md#wave-activity-deposition)
      - [Quasi-geostrophic wave-activity conservation law](geophysical-fluid-dynamics.md#quasi-geostrophic-wave-activity-conservation-law)
    - [Residual mean circulation](geophysical-fluid-dynamics.md#residual-mean-circulation)
      - [Eliassen equation for residual circulation](geophysical-fluid-dynamics.md#eliassen-equation-for-residual-circulation)
        - [Step-flux residual circulation in a stratified channel](geophysical-fluid-dynamics.md#step-flux-residual-circulation-in-a-stratified-channel)
        - [Localized wave-drag response in a stratified channel](geophysical-fluid-dynamics.md#localized-wave-drag-response-in-a-stratified-channel)
          - [Vertically integrated wave-drag acceleration](geophysical-fluid-dynamics.md#vertically-integrated-wave-drag-acceleration)
- [Dispersion of a solute by flow](#dispersion-of-a-solute-by-flow)
  - [Irreversible capture of an advecting tracer](#irreversible-capture-of-an-advecting-tracer)
  - [Transverse dispersion](#transverse-dispersion)
  - [Péclet number](#peclet-number)
  - [Taylor dispersion](#taylor-dispersion)
    - [Longitudinal moment hierarchy for shear transport](#longitudinal-moment-hierarchy-for-shear-transport)
      - [Oscillating shear dispersion in an insulating channel](#oscillating-shear-dispersion-in-an-insulating-channel)
    - [Effective diffusivity of a periodic sinusoidal shear](#effective-diffusivity-of-a-periodic-sinusoidal-shear)
      - [Impulsively kicked sinusoidal shear dispersion](#impulsively-kicked-sinusoidal-shear-dispersion)
    - [Taylor dispersion in a parabolic porous-layer velocity profile](#taylor-dispersion-in-a-parabolic-porous-layer-velocity-profile)
    - [Taylor dispersion in a linear porous-layer velocity profile](#taylor-dispersion-in-a-linear-porous-layer-velocity-profile)
    - [Taylor dispersion in plane Couette flow](#taylor-dispersion-in-plane-couette-flow)
- [Rheology](rheology.md)
  - [Viscous dissipation potential](rheology.md#viscous-dissipation-potential)
    - [Convex viscous potential minimum principle](rheology.md#convex-viscous-potential-minimum-principle)
  - [Rheometer](rheology.md#rheometer)
    - [Cone-and-plate rheometer](rheology.md#cone-and-plate-rheometer)
    - [Parallel-plate rheometer](rheology.md#parallel-plate-rheometer)
    - [Small-amplitude oscillatory shear](rheology.md#small-amplitude-oscillatory-shear)
      - [Storage modulus](rheology.md#storage-modulus)
      - [Loss modulus](rheology.md#loss-modulus)
      - [Loss tangent](rheology.md#loss-tangent)
      - [Viscoelastic relaxation time](rheology.md#viscoelastic-relaxation-time)
  - [Non-Newtonian fluid](rheology.md#non-newtonian-fluid)
    - [Simple fluid](rheology.md#simple-fluid)
      - [Viscometric flow](rheology.md#viscometric-flow)
    - [Shear banding](rheology.md#shear-banding)
    - [Generalized Newtonian fluid](rheology.md#generalized-newtonian-fluid)
      - [Differential shear viscosity](rheology.md#differential-shear-viscosity)
        - [Weak-pressure Couette-Poiseuille expansion](rheology.md#weak-pressure-couette-poiseuille-expansion)
      - [Weissenberg–Rabinowitsch equation](rheology.md#weissenberg-rabinowitsch-equation)
    - [Thixotropy](rheology.md#thixotropy)
    - [Yield-stress fluid](rheology.md#yield-stress-fluid)
      - [Bingham plastic](rheology.md#bingham-plastic)
        - [Plane Poiseuille flow of a Bingham fluid](rheology.md#plane-poiseuille-flow-of-a-bingham-fluid)
        - [Yield surface](rheology.md#yield-surface)
        - [Pressure-driven annular Bingham flow with a free surface](rheology.md#pressure-driven-annular-bingham-flow-with-a-free-surface)
        - [Bingham sliding law](rheology.md#bingham-sliding-law)
      - [Herschel–Bulkley fluid](rheology.md#herschel-bulkley-fluid)
      - [Plug flow of a yield-stress fluid](rheology.md#plug-flow-of-a-yield-stress-fluid)
      - [Slump test for yield stress](rheology.md#slump-test-for-yield-stress)
    - [Power-law fluid](rheology.md#power-law-fluid)
      - [Power-law coating on a rotating cylinder](rheology.md#power-law-coating-on-a-rotating-cylinder)
      - [Power-law Couette-Poiseuille flow](rheology.md#power-law-couette-poiseuille-flow)
      - [Shear thinning](rheology.md#shear-thinning)
    - [Viscoelasticity](rheology.md#viscoelasticity)
      - [Phan-Thien-Tanner fluid](rheology.md#phan-thien-tanner-fluid)
        - [Uniaxial extension of an affine linear PTT fluid](rheology.md#uniaxial-extension-of-an-affine-linear-ptt-fluid)
        - [Shear and pipe flow of an affine linear PTT fluid](rheology.md#shear-and-pipe-flow-of-an-affine-linear-ptt-fluid)
      - [Weissenberg number](rheology.md#weissenberg-number)
      - [Deborah number](rheology.md#deborah-number)
      - [Differential pom-pom model](rheology.md#differential-pom-pom-model)
        - [Steady uniaxial extension of the differential pom-pom model](rheology.md#steady-uniaxial-extension-of-the-differential-pom-pom-model)
        - [Linear and second-order response of the differential pom-pom model](rheology.md#linear-and-second-order-response-of-the-differential-pom-pom-model)
      - [Dashpot](rheology.md#dashpot)
      - [Kelvin-Voigt model](rheology.md#kelvin-voigt-model)
        - [Kelvin-Voigt cantilever creep](rheology.md#kelvin-voigt-cantilever-creep)
      - [Stress relaxation](rheology.md#stress-relaxation)
      - [Linear viscoelastic fluid](rheology.md#linear-viscoelastic-fluid)
        - [Creep compliance](rheology.md#creep-compliance)
        - [Complex viscosity](rheology.md#complex-viscosity)
        - [Relaxation modulus](rheology.md#relaxation-modulus)
          - [Instantaneous solvent term in a relaxation modulus](rheology.md#instantaneous-solvent-term-in-a-relaxation-modulus)
      - [Viscometric functions](rheology.md#viscometric-functions)
      - [Corotational Jeffreys fluid](rheology.md#corotational-jeffreys-fluid)
      - [Linear Maxwell fluid](rheology.md#linear-maxwell-fluid)
        - [Oscillatory channel flux of a linear Maxwell fluid](rheology.md#oscillatory-channel-flux-of-a-linear-maxwell-fluid)
        - [Maxwell start-up shear layer](rheology.md#maxwell-start-up-shear-layer)
        - [Maxwell cantilever creep](rheology.md#maxwell-cantilever-creep)
        - [Maxwell-filtered local drag](rheology.md#maxwell-filtered-local-drag)
      - [Conformation tensor](rheology.md#conformation-tensor)
        - [Objective time derivative](rheology.md#objective-time-derivative)
          - [Rivlin-Ericksen tensor](rheology.md#rivlin-ericksen-tensor)
          - [Corotational derivative of a polar vector](rheology.md#corotational-derivative-of-a-polar-vector)
          - [Upper-convected derivative](rheology.md#upper-convected-derivative)
            - [Rotating-frame reduction of circular viscoelastic shear](rheology.md#rotating-frame-reduction-of-circular-viscoelastic-shear)
            - [Upper-convected rate as a stress push-forward](rheology.md#upper-convected-rate-as-a-stress-push-forward)
            - [Upper-convected Maxwell model](rheology.md#upper-convected-maxwell-model)
              - [Giesekus model](rheology.md#giesekus-model)
          - [Lower-convected derivative](rheology.md#lower-convected-derivative)
            - [Lower-convected stress pull-back](rheology.md#lower-convected-stress-pull-back)
          - [Jaumann derivative](rheology.md#jaumann-derivative)
            - [Corotating-frame representation of a Jaumann derivative](rheology.md#corotating-frame-representation-of-a-jaumann-derivative)
            - [Corotational Maxwell fluid](rheology.md#corotational-maxwell-fluid)
              - [Steady shear of a corotational Maxwell fluid](rheology.md#steady-shear-of-a-corotational-maxwell-fluid)
            - [Covariance of the Jaumann derivative](rheology.md#covariance-of-the-jaumann-derivative)
      - [Oldroyd-B model](rheology.md#oldroyd-b-model)
        - [Torque reversal of a linear Oldroyd fluid](rheology.md#torque-reversal-of-a-linear-oldroyd-fluid)
        - [Inertialess Oldroyd-B circular Couette pressure](rheology.md#inertialess-oldroyd-b-circular-couette-pressure)
        - [FENE-P model](rheology.md#fene-p-model)
      - [Oldroyd-A model](rheology.md#oldroyd-a-model)
        - [Steady simple shear of an Oldroyd-A fluid](rheology.md#steady-simple-shear-of-an-oldroyd-a-fluid)
        - [Fading-memory representation of the Oldroyd-A model](rheology.md#fading-memory-representation-of-the-oldroyd-a-model)
      - [Second-order fluid](rheology.md#second-order-fluid)
        - [Elastic secondary circulation around a rotating sphere](rheology.md#elastic-secondary-circulation-around-a-rotating-sphere)
        - [Newtonian velocity preservation in a second-order fluid](rheology.md#newtonian-velocity-preservation-in-a-second-order-fluid)
      - [Johnson--Segalman--Oldroyd model](rheology.md#johnson-segalman-oldroyd-model)
        - [Johnson-Segalman extensional response](rheology.md#johnson-segalman-extensional-response)
        - [Johnson-Segalman steady viscometric functions](rheology.md#johnson-segalman-steady-viscometric-functions)
          - [Johnson-Segalman negative-slope shear threshold](rheology.md#johnson-segalman-negative-slope-shear-threshold)
        - [Gordon--Schowalter derivative](rheology.md#gordon-schowalter-derivative)
        - [Retardation time of an Oldroyd fluid](rheology.md#retardation-time-of-an-oldroyd-fluid)
        - [Linear oscillatory response of a Johnson--Segalman--Oldroyd fluid](rheology.md#linear-oscillatory-response-of-a-johnson-segalman-oldroyd-fluid)
        - [Steady shear viscosity of a Johnson--Segalman--Oldroyd fluid](rheology.md#steady-shear-viscosity-of-a-johnson-segalman-oldroyd-fluid)
      - [Normal-stress difference](rheology.md#normal-stress-difference)
        - [Die swell](rheology.md#die-swell)
        - [Weissenberg effect](rheology.md#weissenberg-effect)
      - [Extensional viscosity](rheology.md#extensional-viscosity)
        - [Uniaxial extensional flow](rheology.md#uniaxial-extensional-flow)
          - [Extensional equations for a slender Newtonian column](rheology.md#extensional-equations-for-a-slender-newtonian-column)
            - [Annular return flow around a slumping column](rheology.md#annular-return-flow-around-a-slumping-column)
              - [Extensional screening length of a slumping column](rheology.md#extensional-screening-length-of-a-slumping-column)
                - [Initial velocity profile of an annularly confined column](rheology.md#initial-velocity-profile-of-an-annularly-confined-column)
            - [Plug-flow criterion for a column in a low-viscosity annulus](rheology.md#plug-flow-criterion-for-a-column-in-a-low-viscosity-annulus)
          - [Axial strain rate](rheology.md#axial-strain-rate)
        - [Trouton ratio](rheology.md#trouton-ratio)
    - [Suspension rheology](rheology.md#suspension-rheology)
      - [Dilute rod suspension](rheology.md#dilute-rod-suspension)
      - [Jamming](rheology.md#jamming)
      - [Viscous number](rheology.md#viscous-number)
      - [Shear-induced dilation](rheology.md#shear-induced-dilation)
- [Porous-media flow](porous-media-flow.md)
  - [Aquifer](porous-media-flow.md#aquifer)
    - [Unconfined aquifer](porous-media-flow.md#unconfined-aquifer)
      - [Boussinesq equation for an unconfined aquifer](porous-media-flow.md#boussinesq-equation-for-an-unconfined-aquifer)
        - [Conserved first moment of a draining porous current](porous-media-flow.md#conserved-first-moment-of-a-draining-porous-current)
          - [Dipole similarity solution of a draining porous current](porous-media-flow.md#dipole-similarity-solution-of-a-draining-porous-current)
            - [Drainage volume decay in a dipole porous current](porous-media-flow.md#drainage-volume-decay-in-a-dipole-porous-current)
        - [Separable aquifer drawdown](porous-media-flow.md#separable-aquifer-drawdown)
      - [Dupuit approximation](porous-media-flow.md#dupuit-approximation)
        - [Dupuit flow in a channel with cubic wetted area](porous-media-flow.md#dupuit-flow-in-a-channel-with-cubic-wetted-area)
      - [Unconfined aquifer with depth-dependent permeability](porous-media-flow.md#unconfined-aquifer-with-depth-dependent-permeability)
        - [Outlet layer in a deep unconfined aquifer](porous-media-flow.md#outlet-layer-in-a-deep-unconfined-aquifer)
      - [Poroelastic aquifer](porous-media-flow.md#poroelastic-aquifer)
        - [Poroelastic compaction length](porous-media-flow.md#poroelastic-compaction-length)
  - [Delayed polymer diversion in parallel porous layers](porous-media-flow.md#delayed-polymer-diversion-in-parallel-porous-layers)
  - [Thermal front in a porous medium](porous-media-flow.md#thermal-front-in-a-porous-medium)
  - [Porous medium](porous-media-flow.md#porous-medium)
  - [Resident-weighted transit time in a layered flow](porous-media-flow.md#resident-weighted-transit-time-in-a-layered-flow)
  - [Capillary imbibition](porous-media-flow.md#capillary-imbibition)
    - [Hemispherical capillary imbibition](porous-media-flow.md#hemispherical-capillary-imbibition)
      - [Evaporation-limited hemispherical imbibition](porous-media-flow.md#evaporation-limited-hemispherical-imbibition)
  - [Two-phase porous-media flow](porous-media-flow.md#two-phase-porous-media-flow)
    - [Capillary residual trapping](porous-media-flow.md#capillary-residual-trapping)
      - [Residual-trapping attenuation of a porous current](porous-media-flow.md#residual-trapping-attenuation-of-a-porous-current)
        - [Mobile-volume peak of an exponentially forced porous current](porous-media-flow.md#mobile-volume-peak-of-an-exponentially-forced-porous-current)
      - [Triangular current with capillary retention](porous-media-flow.md#triangular-current-with-capillary-retention)
        - [Maximum-invasion envelope of a retained current](porous-media-flow.md#maximum-invasion-envelope-of-a-retained-current)
    - [Waterflooding](porous-media-flow.md#waterflooding)
    - [Buckley-Leverett equation](porous-media-flow.md#buckley-leverett-equation)
      - [Capillary diffusion](porous-media-flow.md#capillary-diffusion)
      - [Fractional-flow tangent construction](porous-media-flow.md#fractional-flow-tangent-construction)
    - [Fractional flow](porous-media-flow.md#fractional-flow)
    - [Fluid saturation](porous-media-flow.md#fluid-saturation)
  - [Flux-weighted residence time in a porous layer](porous-media-flow.md#flux-weighted-residence-time-in-a-porous-layer)
  - [Vertical imbibition under a draining liquid layer](porous-media-flow.md#vertical-imbibition-under-a-draining-liquid-layer)
  - [Darcy law](porous-media-flow.md#darcy-law)
    - [Darcy flow](porous-media-flow.md#darcy-flow)
      - [Lubrication boundary condition for a crack in a Darcy medium](porous-media-flow.md#lubrication-boundary-condition-for-a-crack-in-a-darcy-medium)
        - [Crack pressure in elliptic coordinates](porous-media-flow.md#crack-pressure-in-elliptic-coordinates)
          - [Elliptic crack pressure dipole](porous-media-flow.md#elliptic-crack-pressure-dipole)
            - [Fixed-throughflow dissipation reduction of a conductive crack](porous-media-flow.md#fixed-throughflow-dissipation-reduction-of-a-conductive-crack)
    - [Uniformly heated vertical plate in a porous medium](porous-media-flow.md#uniformly-heated-vertical-plate-in-a-porous-medium)
      - [Integral exponential profile for porous wall convection](porous-media-flow.md#integral-exponential-profile-for-porous-wall-convection)
    - [Fixed-pressure planar Darcy displacement](porous-media-flow.md#fixed-pressure-planar-darcy-displacement)
      - [Thermal-front retardation in Darcy flow](porous-media-flow.md#thermal-front-retardation-in-darcy-flow)
    - [Porous thermal plume](porous-media-flow.md#porous-thermal-plume)
      - [Conserved momentum flux of a porous thermal plume](porous-media-flow.md#conserved-momentum-flux-of-a-porous-thermal-plume)
      - [Hyperbolic-secant porous plume profile](porous-media-flow.md#hyperbolic-secant-porous-plume-profile)
        - [Heat-weighted head speed of a porous plume](porous-media-flow.md#heat-weighted-head-speed-of-a-porous-plume)
    - [Darcy dissipation](porous-media-flow.md#darcy-dissipation)
    - [Darcy velocity](porous-media-flow.md#darcy-velocity)
      - [Pore velocity](porous-media-flow.md#pore-velocity)
    - [Darcy-Bénard convection](porous-media-flow.md#darcy-benard-convection)
      - [Insulated square-column Darcy convection onset](porous-media-flow.md#insulated-square-column-darcy-convection-onset)
      - [Conducting-square Darcy convection](porous-media-flow.md#conducting-square-darcy-convection)
        - [Growth-rate solvability for conducting-square Darcy convection](porous-media-flow.md#growth-rate-solvability-for-conducting-square-darcy-convection)
        - [Gauge transformation for conducting-square Darcy onset](porous-media-flow.md#gauge-transformation-for-conducting-square-darcy-onset)
      - [Darcy thermal-time Rayleigh number](porous-media-flow.md#darcy-thermal-time-rayleigh-number)
      - [Onset of convection in a horizontal Darcy layer](porous-media-flow.md#onset-of-convection-in-a-horizontal-darcy-layer)
        - [Supercritical saturation of Darcy convection rolls](porous-media-flow.md#supercritical-saturation-of-darcy-convection-rolls)
          - [Mean-temperature correction in weakly nonlinear Darcy convection](porous-media-flow.md#mean-temperature-correction-in-weakly-nonlinear-darcy-convection)
    - [Saffman–Taylor instability](porous-media-flow.md#saffman-taylor-instability)
      - [Planar viscous-fingering dispersion relation](porous-media-flow.md#planar-viscous-fingering-dispersion-relation)
        - [Thermal-front viscous-fingering dispersion relation](porous-media-flow.md#thermal-front-viscous-fingering-dispersion-relation)
        - [Buoyancy-modified Darcy fingering dispersion relation](porous-media-flow.md#buoyancy-modified-darcy-fingering-dispersion-relation)
        - [Surface-tension-gradient stabilization of viscous fingering](porous-media-flow.md#surface-tension-gradient-stabilization-of-viscous-fingering)
    - [Permeability of a porous medium](porous-media-flow.md#permeability-of-a-porous-medium)
      - [Relative permeability](porous-media-flow.md#relative-permeability)
        - [Phase mobility](porous-media-flow.md#phase-mobility)
      - [Effective permeability](porous-media-flow.md#effective-permeability)
        - [Dilute permeability enhancement by aligned cracks](porous-media-flow.md#dilute-permeability-enhancement-by-aligned-cracks)
        - [Effective permeability of complementary wedges](porous-media-flow.md#effective-permeability-of-complementary-wedges)
      - [Porosity](porous-media-flow.md#porosity)
    - [Pressure-dependent Darcy drainage](porous-media-flow.md#pressure-dependent-darcy-drainage)
  - [Reactive infiltration instability](porous-media-flow.md#reactive-infiltration-instability)
    - [Melting-front instability due to permeability contrast](porous-media-flow.md#melting-front-instability-due-to-permeability-contrast)
  - [Porous gravity current](porous-media-flow.md#porous-gravity-current)
    - [Inclined porous gravity current](porous-media-flow.md#inclined-porous-gravity-current)
      - [Volume Jacobian for downslope stretched coordinates](porous-media-flow.md#volume-jacobian-for-downslope-stretched-coordinates)
      - [Depth-dependent inclined porous-current equation](porous-media-flow.md#depth-dependent-inclined-porous-current-equation)
        - [Far-downslope width of a constant-flux porous current](porous-media-flow.md#far-downslope-width-of-a-constant-flux-porous-current)
      - [Advection limit of an inclined porous current](porous-media-flow.md#advection-limit-of-an-inclined-porous-current)
    - [One-sided constant-volume porous gravity current](porous-media-flow.md#one-sided-constant-volume-porous-gravity-current)
    - [Slope-driven porous gravity current](porous-media-flow.md#slope-driven-porous-gravity-current)
      - [Caprock leakage threshold](porous-media-flow.md#caprock-leakage-threshold)
      - [Moving thermal front in a porous current](porous-media-flow.md#moving-thermal-front-in-a-porous-current)
    - [Porous gravity current with background flow](porous-media-flow.md#porous-gravity-current-with-background-flow)
      - [Advected constant-volume porous gravity current](porous-media-flow.md#advected-constant-volume-porous-gravity-current)
      - [Constant-flux porous gravity current](porous-media-flow.md#constant-flux-porous-gravity-current)
        - [Diffusive nose of an advected porous gravity current](porous-media-flow.md#diffusive-nose-of-an-advected-porous-gravity-current)
    - [Leaky porous gravity current](porous-media-flow.md#leaky-porous-gravity-current)
      - [Hydrostatic leakage through a basal seal](porous-media-flow.md#hydrostatic-leakage-through-a-basal-seal)
      - [Exponential drainage transform for porous-medium diffusion](porous-media-flow.md#exponential-drainage-transform-for-porous-medium-diffusion)
        - [Invasion envelope of an exponentially draining porous current](porous-media-flow.md#invasion-envelope-of-an-exponentially-draining-porous-current)
- [Reduced gravity](reduced-gravity.md)
  - [Entraining shallow-water layer](reduced-gravity.md#entraining-shallow-water-layer)
  - [Gravity current](reduced-gravity.md#gravity-current)
    - [Finite-volume inertial gravity current](reduced-gravity.md#finite-volume-inertial-gravity-current)
    - [Finite-Froude lock-release rarefaction](reduced-gravity.md#finite-froude-lock-release-rarefaction)
      - [Reflected information in a finite lock release](reduced-gravity.md#reflected-information-in-a-finite-lock-release)
    - [Front-regularized triangular-channel dam break](reduced-gravity.md#front-regularized-triangular-channel-dam-break)
    - [Entraining shallow-water current in a triangular channel](reduced-gravity.md#entraining-shallow-water-current-in-a-triangular-channel)
      - [Characteristic compatibility for an entraining triangular-channel current](reduced-gravity.md#characteristic-compatibility-for-an-entraining-triangular-channel-current)
    - [Floating extensional viscous gravity current](reduced-gravity.md#floating-extensional-viscous-gravity-current)
      - [Constant-flux floating extensional gravity current](reduced-gravity.md#constant-flux-floating-extensional-gravity-current)
    - [Axisymmetric viscous gravity current](reduced-gravity.md#axisymmetric-viscous-gravity-current)
    - [V-shaped channel gravity current](reduced-gravity.md#v-shaped-channel-gravity-current)
      - [Shallow V-channel lubrication flux](reduced-gravity.md#shallow-v-channel-lubrication-flux)
        - [Porous-medium transformation of V-channel spreading](reduced-gravity.md#porous-medium-transformation-of-v-channel-spreading)
      - [Constant-volume similarity in a V-shaped channel](reduced-gravity.md#constant-volume-similarity-in-a-v-shaped-channel)
    - [Shear-driven viscous gravity current](reduced-gravity.md#shear-driven-viscous-gravity-current)
      - [Line-source upstream reach under imposed shear](reduced-gravity.md#line-source-upstream-reach-under-imposed-shear)
      - [Downstream similarity of a shear-driven gravity current](reduced-gravity.md#downstream-similarity-of-a-shear-driven-gravity-current)
    - [Subglacial current with constant viscous wall layers](reduced-gravity.md#subglacial-current-with-constant-viscous-wall-layers)
      - [Melting-source gravity-current equation](reduced-gravity.md#melting-source-gravity-current-equation)
        - [Meltwater production over an advancing footprint](reduced-gravity.md#meltwater-production-over-an-advancing-footprint)
    - [Constant-speed entraining gravity current on a slope](reduced-gravity.md#constant-speed-entraining-gravity-current-on-a-slope)
    - [Interfacial viscous gravity current](reduced-gravity.md#interfacial-viscous-gravity-current)
      - [Diffusion-controlled solute gravity current](reduced-gravity.md#diffusion-controlled-solute-gravity-current)
      - [Ambient-controlled interfacial plug current](reduced-gravity.md#ambient-controlled-interfacial-plug-current)
        - [Disc-traction analogy for an interfacial current](reduced-gravity.md#disc-traction-analogy-for-an-interfacial-current)
          - [Interfacial plug-current similarity profile](reduced-gravity.md#interfacial-plug-current-similarity-profile)
        - [Viscosity window for an interfacial plug current](reduced-gravity.md#viscosity-window-for-an-interfacial-plug-current)
      - [Isostatic depth partition of an interfacial current](reduced-gravity.md#isostatic-depth-partition-of-an-interfacial-current)
    - [Froude number](reduced-gravity.md#froude-number)
      - [Critical width of a rectangular open-channel contraction](reduced-gravity.md#critical-width-of-a-rectangular-open-channel-contraction)
      - [Hydraulic control](reduced-gravity.md#hydraulic-control)
        - [Weir](reduced-gravity.md#weir)
          - [Broad-crested weir](reduced-gravity.md#broad-crested-weir)
        - [Hydraulic flow in an inverted channel](reduced-gravity.md#hydraulic-flow-in-an-inverted-channel)
          - [Two successive hydraulic controls](reduced-gravity.md#two-successive-hydraulic-controls)
        - [Hydraulic control with prescribed seepage](reduced-gravity.md#hydraulic-control-with-prescribed-seepage)
        - [Head-loss correction to hydraulic control](reduced-gravity.md#head-loss-correction-to-hydraulic-control)
        - [Hydraulic control in a variable-width channel](reduced-gravity.md#hydraulic-control-in-a-variable-width-channel)
      - [Supercritical flow](reduced-gravity.md#supercritical-flow)
      - [Subcritical flow](reduced-gravity.md#subcritical-flow)
      - [Gravity-current front condition](reduced-gravity.md#gravity-current-front-condition)
        - [Benjamin deep-ambient front condition](reduced-gravity.md#benjamin-deep-ambient-front-condition)
        - [Saint-Venant dry-front condition](reduced-gravity.md#saint-venant-dry-front-condition)
    - [Gravity-current box model](reduced-gravity.md#gravity-current-box-model)
      - [Finite-volume triangular-channel current](reduced-gravity.md#finite-volume-triangular-channel-current)
      - [Hindered-settling runout in a rectangular channel](reduced-gravity.md#hindered-settling-runout-in-a-rectangular-channel)
      - [Inertial dam-break current in a triangular valley](reduced-gravity.md#inertial-dam-break-current-in-a-triangular-valley)
      - [Parabolic-channel sediment-current box model](reduced-gravity.md#parabolic-channel-sediment-current-box-model)
      - [Prismatic triangular-channel gravity-current box model](reduced-gravity.md#prismatic-triangular-channel-gravity-current-box-model)
        - [Finite-volume inertial spreading in a triangular channel](reduced-gravity.md#finite-volume-inertial-spreading-in-a-triangular-channel)
        - [Constant-settling runout in a triangular valley](reduced-gravity.md#constant-settling-runout-in-a-triangular-valley)
          - [Deposit profile of a finite triangular-valley particle current](reduced-gravity.md#deposit-profile-of-a-finite-triangular-valley-particle-current)
        - [Hindered-settling runout invariant in a prismatic triangular channel](reduced-gravity.md#hindered-settling-runout-invariant-in-a-prismatic-triangular-channel)
      - [Detrainment-limited gravity-current runout](reduced-gravity.md#detrainment-limited-gravity-current-runout)
      - [Particle-laden gravity current](reduced-gravity.md#particle-laden-gravity-current)
        - [Particle-laden current with suction](reduced-gravity.md#particle-laden-current-with-suction)
        - [Sedimenting rectangular-channel characteristic compatibility](reduced-gravity.md#sedimenting-rectangular-channel-characteristic-compatibility)
        - [Axisymmetric settling box model](reduced-gravity.md#axisymmetric-settling-box-model)
          - [Settling exposure for a particle size distribution](reduced-gravity.md#settling-exposure-for-a-particle-size-distribution)
          - [Monodisperse circular ash runout](reduced-gravity.md#monodisperse-circular-ash-runout)
            - [Circular ash deposit profile](reduced-gravity.md#circular-ash-deposit-profile)
        - [Prismatic triangular-channel shallow water equations](reduced-gravity.md#prismatic-triangular-channel-shallow-water-equations)
          - [Sedimenting triangular-channel characteristic compatibility](reduced-gravity.md#sedimenting-triangular-channel-characteristic-compatibility)
        - [Buoyancy production in a particle-laden current](reduced-gravity.md#buoyancy-production-in-a-particle-laden-current)
        - [Weak-settling attenuation of a sloping gravity current](reduced-gravity.md#weak-settling-attenuation-of-a-sloping-gravity-current)
          - [Formal sedimentation runout of a sloping gravity current](reduced-gravity.md#formal-sedimentation-runout-of-a-sloping-gravity-current)
        - [Steady depositing gravity current](reduced-gravity.md#steady-depositing-gravity-current)
          - [Bidisperse gravity-current deposition](reduced-gravity.md#bidisperse-gravity-current-deposition)
          - [Depth branches of a steady depositing gravity current](reduced-gravity.md#depth-branches-of-a-steady-depositing-gravity-current)
        - [Heated particle-laden gravity current](reduced-gravity.md#heated-particle-laden-gravity-current)
          - [Heated gravity-current runout](reduced-gravity.md#heated-gravity-current-runout)
        - [Triangular-channel shallow water equations](reduced-gravity.md#triangular-channel-shallow-water-equations)
        - [Triangular-channel gravity-current box model](reduced-gravity.md#triangular-channel-gravity-current-box-model)
        - [Runout length of a gravity current](reduced-gravity.md#runout-length-of-a-gravity-current)
    - [Draining gravity current](reduced-gravity.md#draining-gravity-current)
      - [Deep-substrate drainage of a gravity current](reduced-gravity.md#deep-substrate-drainage-of-a-gravity-current)
        - [Cubic-input similarity for a draining gravity current](reduced-gravity.md#cubic-input-similarity-for-a-draining-gravity-current)
      - [Similarity exponents of a draining gravity current](reduced-gravity.md#similarity-exponents-of-a-draining-gravity-current)
    - [Lock-exchange flow](reduced-gravity.md#lock-exchange-flow)
- [Laminar round jet](#laminar-round-jet)
  - [Conserved momentum flux of a laminar round jet](#conserved-momentum-flux-of-a-laminar-round-jet)
  - [Similarity solution for a laminar round jet](#similarity-solution-for-a-laminar-round-jet)
- [Fluid entrainment](#fluid-entrainment)
  - [Entrainment velocity](#entrainment-velocity)
  - [Interfacial power model for entrainment](#interfacial-power-model-for-entrainment)
  - [Potential energy of two-layer entrainment](#potential-energy-of-two-layer-entrainment)
    - [Potential energy of mixed-layer deepening with an initial buoyancy jump](#potential-energy-of-mixed-layer-deepening-with-an-initial-buoyancy-jump)
  - [Fixed-energy turbulent mixed layer](#fixed-energy-turbulent-mixed-layer)
    - [Fixed-energy two-layer entrainment law](#fixed-energy-two-layer-entrainment-law)
    - [Rotating-disc mixed-layer depth law](#rotating-disc-mixed-layer-depth-law)
- [Turbulent plume](turbulent-plume.md)
  - [Lazy plume](turbulent-plume.md#lazy-plume)
  - [Filling box model](turbulent-plume.md#filling-box-model)
    - [Finite-source filling-box front with a side opening](turbulent-plume.md#finite-source-filling-box-front-with-a-side-opening)
    - [Filling-box first front](turbulent-plume.md#filling-box-first-front)
      - [Symmetric line-plume filling-box front](turbulent-plume.md#symmetric-line-plume-filling-box-front)
  - [Forced plume](turbulent-plume.md#forced-plume)
    - [Jet length](turbulent-plume.md#jet-length)
    - [Inclined forced plume](turbulent-plume.md#inclined-forced-plume)
      - [Horizontal forced-plume trajectory](turbulent-plume.md#horizontal-forced-plume-trajectory)
  - [Buoyancy flux](turbulent-plume.md#buoyancy-flux)
  - [Batchelor entrainment hypothesis](turbulent-plume.md#batchelor-entrainment-hypothesis)
    - [Entrainment coefficient](turbulent-plume.md#entrainment-coefficient)
  - [Top-hat plume model](turbulent-plume.md#top-hat-plume-model)
    - [Confined plume with compensating return flow](turbulent-plume.md#confined-plume-with-compensating-return-flow)
      - [Confined-plume momentum fold](turbulent-plume.md#confined-plume-momentum-fold)
    - [Source-volume length of a turbulent plume](turbulent-plume.md#source-volume-length-of-a-turbulent-plume)
    - [Jet limit of the top-hat plume model](turbulent-plume.md#jet-limit-of-the-top-hat-plume-model)
    - [Weak hyperbolicity of the unsteady top-hat plume](turbulent-plume.md#weak-hyperbolicity-of-the-unsteady-top-hat-plume)
    - [Unsteady top-hat line-plume balances](turbulent-plume.md#unsteady-top-hat-line-plume-balances)
      - [Separable decaying top-hat line plume](turbulent-plume.md#separable-decaying-top-hat-line-plume)
    - [Merger of two equal pure plumes](turbulent-plume.md#merger-of-two-equal-pure-plumes)
      - [Fixed-speed pure-plume merger and flux conservation](turbulent-plume.md#fixed-speed-pure-plume-merger-and-flux-conservation)
    - [Boussinesq top-hat plume in a stratified ambient](turbulent-plume.md#boussinesq-top-hat-plume-in-a-stratified-ambient)
      - [Plume similarity in power-law stratification](turbulent-plume.md#plume-similarity-in-power-law-stratification)
        - [Top-hat plume in constant unstable stratification](turbulent-plume.md#top-hat-plume-in-constant-unstable-stratification)
        - [Amplitudes and physical branches of a power-law stratified plume](turbulent-plume.md#amplitudes-and-physical-branches-of-a-power-law-stratified-plume)
        - [Logarithmic-height plume equations](turbulent-plume.md#logarithmic-height-plume-equations)
          - [Growing mode of power-law plume similarity](turbulent-plume.md#growing-mode-of-power-law-plume-similarity)
    - [Kinematic plume fluxes](turbulent-plume.md#kinematic-plume-fluxes)
    - [Non-Boussinesq top-hat plume equations](turbulent-plume.md#non-boussinesq-top-hat-plume-equations)
      - [Non-Boussinesq pure-plume density transition](turbulent-plume.md#non-boussinesq-pure-plume-density-transition)
    - [Pure plume](turbulent-plume.md#pure-plume)
      - [Pure plume balance](turbulent-plume.md#pure-plume-balance)
        - [Plume flux-balance invariant](turbulent-plume.md#plume-flux-balance-invariant)
          - [Finite-source forced-plume quadrature](turbulent-plume.md#finite-source-forced-plume-quadrature)
          - [Attraction to pure plume similarity](turbulent-plume.md#attraction-to-pure-plume-similarity)
        - [Plume balance parameter](turbulent-plume.md#plume-balance-parameter)
      - [Axisymmetric pure plume](turbulent-plume.md#axisymmetric-pure-plume)
        - [Radius growth of an axisymmetric pure plume](turbulent-plume.md#radius-growth-of-an-axisymmetric-pure-plume)
        - [Neutral buoyancy-flux mode of a pure plume](turbulent-plume.md#neutral-buoyancy-flux-mode-of-a-pure-plume)
        - [Boussinesq point-source plume](turbulent-plume.md#boussinesq-point-source-plume)
      - [Line plume](turbulent-plume.md#line-plume)
        - [Triangular-profile line plume](turbulent-plume.md#triangular-profile-line-plume)
          - [Unsteady Boussinesq triangular-profile line-plume balances](turbulent-plume.md#unsteady-boussinesq-triangular-profile-line-plume-balances)
            - [Separable decaying line-plume similarity](turbulent-plume.md#separable-decaying-line-plume-similarity)
          - [Non-Boussinesq triangular-profile line-plume balances](turbulent-plume.md#non-boussinesq-triangular-profile-line-plume-balances)
        - [Two-sided top-hat line plume](turbulent-plume.md#two-sided-top-hat-line-plume)
        - [Wall line plume](turbulent-plume.md#wall-line-plume)
          - [Melting-driven saline wall plume](turbulent-plume.md#melting-driven-saline-wall-plume)
          - [Ice-bearing wall-plume thermodynamic invariant](turbulent-plume.md#ice-bearing-wall-plume-thermodynamic-invariant)
            - [Self-similar ice-bearing wall plume](turbulent-plume.md#self-similar-ice-bearing-wall-plume)
          - [Triangular-profile wall line plume](turbulent-plume.md#triangular-profile-wall-line-plume)
        - [Stratified line-plume height scale](turbulent-plume.md#stratified-line-plume-height-scale)
      - [Plume virtual origin](turbulent-plume.md#plume-virtual-origin)
        - [Forced-plume virtual-origin geometry](turbulent-plume.md#forced-plume-virtual-origin-geometry)
  - [Heated wall plume](turbulent-plume.md#heated-wall-plume)
  - [Buoyant thermal](turbulent-plume.md#buoyant-thermal)
    - [Thermal erosion of a two-layer interface](turbulent-plume.md#thermal-erosion-of-a-two-layer-interface)
    - [Point-source spherical thermal similarity](turbulent-plume.md#point-source-spherical-thermal-similarity)
    - [Dilute bubbly thermal](turbulent-plume.md#dilute-bubbly-thermal)
      - [Neutral height of a bubbly thermal in a stratified fluid](turbulent-plume.md#neutral-height-of-a-bubbly-thermal-in-a-stratified-fluid)
    - [Buoyant thermal mass balance](turbulent-plume.md#buoyant-thermal-mass-balance)
  - [Starting plume](turbulent-plume.md#starting-plume)
    - [Self-similar starting plume](turbulent-plume.md#self-similar-starting-plume)
      - [Starting-plume thermal Froude-number ratio](turbulent-plume.md#starting-plume-thermal-froude-number-ratio)
  - [Buoyant intrusion](turbulent-plume.md#buoyant-intrusion)
- [Natural ventilation](#natural-ventilation)
  - [Ventilation after a heating reduction](#ventilation-after-a-heating-reduction)
  - [Well-mixed ventilation temperature balance](#well-mixed-ventilation-temperature-balance)
    - [Opposing-wind ventilation bistability](#opposing-wind-ventilation-bistability)
      - [Ventilation switching under wind and heating changes](#ventilation-switching-under-wind-and-heating-changes)
  - [Effective opening area for pressure-driven ventilation](#effective-opening-area-for-pressure-driven-ventilation)
  - [Displacement ventilation](#displacement-ventilation)
    - [Plume-fed doorway ventilation](#plume-fed-doorway-ventilation)
    - [Two-plume three-layer displacement ventilation](#two-plume-three-layer-displacement-ventilation)
    - [Source-volume blocking of displacement ventilation](#source-volume-blocking-of-displacement-ventilation)
    - [Ventilated filling-box relaxation](#ventilated-filling-box-relaxation)
    - [No steady displacement layer without ambient supply](#no-steady-displacement-layer-without-ambient-supply)
    - [Multiple-plume displacement ventilation](#multiple-plume-displacement-ventilation)
    - [Displacement-ventilation interface height](#displacement-ventilation-interface-height)
  - [Single-opening exchange flow](#single-opening-exchange-flow)
    - [Neutral pressure level](#neutral-pressure-level)
  - [Stratified-room plume-exchange model](#stratified-room-plume-exchange-model)
- [Homologous spherical flow](#homologous-spherical-flow)
  - [Self-similar ansatz](#self-similar-ansatz)

## Void fraction

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

The [void fraction](#void-fraction) is the fraction of a mixture's local volume occupied by gas. For a horizontally uniform bubbly liquid it is the transported concentration in a one-dimensional gas-volume [continuity equation](physics.md#continuity-equation). It is distinct from gas mass fraction because gas and liquid have different [mass densities](#density).

### Kinematic bubble transport in an exponentially narrowing vessel

↑ **Parent:** [Void fraction](#void-fraction)

If the vessel radius is proportional to $e^{-\beta z}$, its area is proportional to $e^{-2\beta z}$. Gas-volume conservation gives the displayed equation. Along concentration [characteristic curves](partial-differential-equation.md#characteristic-curve), $\dot z=V_s(1-2\phi)$ and $\dot\phi=2\beta V_s\phi(1-\phi)$. Uniform initial concentration stays uniform in the uninterrupted bubbly region and follows this logistic law. Individual bubbles move at $V_s(1-\phi)$ instead: their rise distance there is $\eta=-(2\beta)^{-1}\log[\phi_0+(1-\phi_0)e^{-2\beta V_st}]$. Boundary interactions and dense-mixture backflow can invalidate the simplified closure.

### Bubble clearing in a cylindrical vessel

↑ **Parent:** [Void fraction](#void-fraction)

For initially uniform bubbles with upward speed $V_s(1-\phi)$, no new gas production and free escape at the top, gas conservation gives flux $V_s\phi(1-\phi)$. A clearing [shock](partial-differential-equation.md#shock-wave) rises from the impermeable bottom with speed $V_s(1-\phi_0)$ by the [Rankine-Hugoniot condition](partial-differential-equation.md#rankine-hugoniot-conditions). The displayed mean [void fraction](#void-fraction) averages the remaining uniform region over the whole liquid depth $H$. This assumes the dilute regime and no retained foam layer.

## Strouhal number

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

The Strouhal number compares the advective time $h/U$ with a prescribed forcing time $1/\omega$. Some conventions use ordinary frequency instead of angular frequency, introducing a factor $2\pi$. For a longitudinal disturbance extending over length $\lambda h$, the relevant ratio is $\lambda St$ rather than $St$ alone.

## Lift (force)

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lift_(force))

Lift is the component of the fluid force on a body perpendicular to its far-field relative [velocity](classical-mechanics.md#velocity); the parallel component is [drag](#drag-physics). In a two-dimensional ideal circulatory flow, the [Kutta–Joukowski theorem](#kutta-joukowski-theorem) gives the lift per unit span from the far-field speed and [circulation](#circulation-physics).

## Airfoil

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Airfoil)

An airfoil is a body profile designed to generate [lift](#lift-force) in a surrounding flow. In two-dimensional [potential flow](#potential-flow), its circulation-dependent lift per unit span is described by the [Kutta–Joukowski theorem](#kutta-joukowski-theorem).

## Uniform flow

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A uniform flow has the same [velocity](classical-mechanics.md#velocity) at every position. A constant velocity field has zero [divergence](calculus.md#divergence) and zero [vorticity](#vorticity); a [velocity potential](#velocity-potential) is $\phi(\mathbf x)=\mathbf U\cdot\mathbf x$. It describes the remote ambient flow in idealized obstacle and [line vortex](#line-vortex) problems.

## Volume viscosity

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Volume_viscosity)

Bulk viscosity is the dissipative response to a fluid's volume expansion or compression, distinct from the shear response. For a Newtonian isotropic fluid its isotropic dissipative stress includes $\zeta_B(\nabla\cdot\mathbf v)I$, and nonnegative $\zeta_B$ gives nonnegative compression-related dissipation. A condensate's relative-density-flow bulk coefficient must be identified from its particular hydrodynamic equation; it is not automatically numerically identical to a dimensional Newtonian viscosity.

## Hydraulic resistance

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[Hydraulic resistance](#hydraulic-resistance) relates the [pressure](thermodynamics.md#pressure) drop across a resistive fluid element to its [volumetric flow rate](#volumetric-flow-rate). In a linear model, $\Delta p=RQ$ with $R>0$, so dissipated mechanical power is $\Delta p\,Q=RQ^2$. A peripheral circulatory bed can be represented by such a resistance when its detailed dynamics are not retained. This terminal [pressure](thermodynamics.md#pressure)-to-flow resistance differs from the area-dependent friction rate multiplying [velocity](classical-mechanics.md#velocity) in a distributed tube momentum equation.

## Physiological fluid dynamics

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

Physiological fluid dynamics studies the motion of fluids in biological systems, including blood flow in elastic arteries, flow through deformable vessels, and liquid layers lining airways. Wall compliance couples [pressure](thermodynamics.md#pressure) to geometry, so wave propagation and mechanical feedback are as important as [viscosity](#dynamic-viscosity).

### Lubrication model of a compliant translating plug

↑ **Parent:** [Physiological fluid dynamics](#physiological-fluid-dynamics)

For a freely translating compliant body separated from a cylindrical wall by a thin [lubrication](viscous-fluid-flow.md#lubrication-theory) gap $h$, the body frame has wall speed $-U$ and body surface speed zero. The local axial flow is $w=-U(1-y/h)+p_xy(y-h)/(2\mu)$, so its flux per circumference is $-Uh/2-p_xh^3/(12\mu)=-Q$. Rearranging proves the displayed pressure gradient. A linear compliance $p=p_0+\alpha(r_0-r)$ couples this flow to deformation. Specified end pressures and zero net axial body force close the problem.

#### Force-free pressure drop of an annular lubrication plug

↑ **Parent:** [Lubrication model of a compliant translating plug](#lubrication-model-of-a-compliant-translating-plug)

The pressure force on a plug-and-film control volume is $\pi a^2\Delta p$. Its opposing wall traction is $2\pi a\mu\int w_y(0)\,dx$, where $w_y(0)=4U/h-6Q/h^2$. Equating them for a freely moving body proves the displayed formula. Writing $s=2Q/U$, $h=sH$ and $x=\sqrt{s/\kappa}X$ converts it into $H(-\widetilde L)-H(\widetilde L)=C\lambda\int[4/(3H)-1/H^2]dX$, with $C=s/a$ and $\lambda=6\mu U/(\alpha\sqrt\kappa s^{5/2})$.

##### Small-speed compliant-plug lubrication asymptotics

↑ **Parent:** [Force-free pressure drop of an annular lubrication plug](#force-free-pressure-drop-of-an-annular-lubrication-plug)

For $H_X+\lambda(H^{-2}-H^{-3})=X$, small $\lambda$ gives $H_0=(b^2+X^2)/2$. In the large-domain limit its inverse-power integrals are $I_1=2\pi/b$, $I_2=2\pi/b^3$ and $I_3=3\pi/b^5$. The force-free condition is $I_2-I_3=C(4I_1/3-I_2)$, or $2b^2-3=C(8b^4/3-2b^2)$. Expanding the root near $b^{-2}=2/3$ proves the displayed minus sign and leading pressure drop. The absolute downstream pressure relative to the elastic reference pressure fixes $s$ and therefore closes the speed-pressure relation.

### Annular inviscid-core displacement

↑ **Parent:** [Physiological fluid dynamics](#physiological-fluid-dynamics)

For a long, weak, axisymmetric indentation of an annular [fully developed flow](viscous-fluid-flow.md#fully-developed-flow), use $r=R+y$ and scale normal velocity by the inverse longitudinal scale ratio. The leading [Euler equations for an inviscid fluid](#euler-equations-for-an-inviscid-fluid) give zero longitudinal pressure gradient and $u_0u_{1x}+v_1u_0'=0$. Together with $u_{1x}+(rv_1)_y/r=0$, this yields $\psi_1=A u_0$, hence the displayed displacement fields. Thin [viscous boundary layers](viscous-fluid-flow.md#viscous-boundary-layer) enforce tangential wall conditions separately.

#### Forced annular displacement equation

↑ **Parent:** [Annular inviscid-core displacement](#annular-inviscid-core-displacement)

A distinguished annular indentation limit has $\lambda^{-2}=O(\epsilon)$, $\lambda St=O(\epsilon)$ and $Re\gg\lambda\epsilon^{-3}$. Define $\beta=\lambda St/\epsilon$, $\sigma=(\lambda^2\epsilon)^{-1}\int_0^1u_0^2/(R+y)\,dy$, $\alpha_1=\gamma_0/R+\gamma_1/(R+1)$ and $\alpha_2=\gamma_0^2/R^2-\gamma_1^2/(R+1)^2$. Radial inertia supplies the pressure difference $\sigma A_{xx}$ between the walls. The axial momentum limits and the moving-wall condition supply its derivative, giving the displayed forced [KdV equation](integrable-systems.md#korteweg-de-vries-equation). This reduction assumes the [viscous boundary layers](viscous-fluid-flow.md#viscous-boundary-layer) remain thin and their displaced flux is smaller than $O(\epsilon^2)$.

##### Opposite propagation directions in the annular displacement equation

↑ **Parent:** [Forced annular displacement equation](#forced-annular-displacement-equation)

With no forcing, the linear [dispersion relation](wave-equation.md#dispersion-relation) has positive [phase velocity](wave-equation.md#phase-velocity) $\sigma k^2/(\beta\alpha_1)$ and [group velocity](wave-equation.md#group-velocity) three times this. A decaying permanent wave with $\xi=x+ct$ instead obeys $\sigma(A')^2=A^2(\beta\alpha_1c+\alpha_2A/3)$. For positive coefficients a nonzero homoclinic wave requires $c>0$ and is negative, travelling upstream. Its inverse width is $k_s=\frac12\sqrt{\beta\alpha_1c/\sigma}$. The opposite directions reflect the nonlinear amplitude-dependent propagation speed.

### Peristaltic pumping

↑ **Parent:** [Physiological fluid dynamics](#physiological-fluid-dynamics)

[Peristaltic pumping](#peristaltic-pumping) transports fluid by a travelling deformation or travelling external [pressure](thermodynamics.md#pressure) acting on a tube. With wave coordinate $X=x-ct$, [mass conservation](continuum-mechanics.md#mass-conservation) makes the relative flux $Q=\alpha(u-c)$ constant. The laboratory flux is $\alpha u=c\alpha+Q$, so a negative relative flux does not rule out forward mean pumping.

#### Weak peristaltic pumping of a collapsible tube

↑ **Parent:** [Peristaltic pumping](#peristaltic-pumping)

For negligible inertia, periodic forcing $p_e=\epsilon P_e\sin kX$, resistance $R\propto\alpha^{-n}$ and prescribed mean area $\alpha_0$, write $Q=-c\alpha_0+\epsilon^2Q_2+\cdots$. First-order area obeys $\widetilde P'_0\alpha_1'+R_0c\alpha_1/\alpha_0=-kP_e\cos kX$. Its mean square is $P_e^2/[2(\widetilde P_0'^2+(R_0c/(k\alpha_0))^2)]$. Averaging the second-order friction balance gives $Q_2=c(n+1)\langle\alpha_1^2\rangle/\alpha_0$, proving the displayed forward pumping rate. Periodicity entails zero mean [pressure](thermodynamics.md#pressure) drop; the mean-area convention fixes the expansion's otherwise free constant.

### Collapsible tube flow

↑ **Parent:** [Physiological fluid dynamics](#physiological-fluid-dynamics)

A one-dimensional collapsible tube model couples area $\alpha$, mean axial [velocity](classical-mechanics.md#velocity) $u$ and internal [pressure](thermodynamics.md#pressure) $p$: $\alpha_t+(\alpha u)_x=0$ and $u_t+uu_x=-p_x-R(\alpha)u$. A wall relation specifies internal minus external [pressure](thermodynamics.md#pressure) as a function of area. Decreasing area generally increases the friction coefficient $R$, while positive wall stiffness gives real small-amplitude [wave speed](wave-equation.md#wave-speed).

#### Choking by wall thickness in an elastic tube

↑ **Parent:** [Collapsible tube flow](#collapsible-tube-flow)

For steady uniform-density inviscid flow with pressure law $p=p_0+k(r-R)$ and a prescribed thickness $h$, mass conservation and the [Bernoulli equation](#bernoulli-equation) give $h/R=1-s^{-1/2}+\lambda(1-s^2)/4$, where $s=u/V$ and $\lambda=2\rho V^2/(kR)$. The function has a unique maximum at $s=\lambda^{-2/5}$, producing the displayed choking bound. Below it there are two positive roots; continuity from the upstream state selects the lower-speed root for $\lambda<1$ and higher-speed root for $\lambda>1$. At $\lambda=1$, the maximum is zero and any positive prescribed thickness is incompatible with this model.

#### Subcritical tube flow

↑ **Parent:** [Collapsible tube flow](#collapsible-tube-flow)

A positive [collapsible tube flow](#collapsible-tube-flow) is subcritical when its [characteristic speeds](partial-differential-equation.md#characteristic-speed) $u+c$ and $u-c$ have opposite signs. A downstream boundary can then send information upstream. For a quadratic pressure-area law and fixed dimensionless flux $q$, this corresponds to $A/A_0>\sqrt q$.

#### Supercritical tube flow

↑ **Parent:** [Collapsible tube flow](#collapsible-tube-flow)

A positive [collapsible tube flow](#collapsible-tube-flow) is supercritical when both [characteristic speeds](partial-differential-equation.md#characteristic-speed) $u\pm c$ are positive relative to the wall. Information then propagates downstream on both branches. For a quadratic pressure-area law and fixed dimensionless flux $q$, the condition is $A/A_0<\sqrt q$.

#### Elastic jump in a quadratic pressure-area tube

↑ **Parent:** [Collapsible tube flow](#collapsible-tube-flow)

An elastic jump is a short transition from a fast, narrow supercritical [collapsible tube flow](#collapsible-tube-flow) to a slower, wider subcritical flow. Neglecting body force and distributed friction across the jump conserves flux and the momentum flux shown above. Distinct upstream and downstream areas therefore obey $\alpha_2^3+\alpha_1\alpha_2^2+\alpha_1^2\alpha_2=3q^2/\alpha_1$. The flux function has its unique minimum at $\alpha=\sqrt q$, so an upstream state below this value has one conjugate state above it. The jump dissipates mechanical energy; it does not conserve a Bernoulli constant.

#### Spatial attraction of a uniform downhill tube flow

↑ **Parent:** [Collapsible tube flow](#collapsible-tube-flow)

For $p=P_0+\rho c_0^2\alpha^2/2$ and constant flux $c_0A_0q$, a downhill [collapsible tube flow](#collapsible-tube-flow) obeys the displayed steady equation. Uniform area satisfies $qR(\alpha_1)=\beta$. Since $R'<0$, linearizing about this root gives downstream exponential decay precisely when $\alpha_1^2<q$. This is spatial stability of a steady inlet-value problem, not a guarantee of temporal stability of the driven flow. The [wave speed](wave-equation.md#wave-speed) is $c_0\alpha$, so the stable spatial branch is supercritical.

#### Friction-induced instability of a collapsible-tube flow

↑ **Parent:** [Collapsible tube flow](#collapsible-tube-flow)

Let $R(\alpha)\propto\alpha^{-n}$, with $n>0$, and use disturbances $e^{i(kx-\omega t)}$ about uniform [velocity](classical-mechanics.md#velocity) $U$. The intrinsic [frequency](physics.md#frequency) is $\nu=\omega-kU$. Linearized [mass conservation](continuum-mechanics.md#mass-conservation) and the decrease in friction as area grows give the displayed [dispersion relation](wave-equation.md#dispersion-relation). For nonzero $k$ and positive flow, one branch grows exactly when $nU>c_0$. At $nU=c_0$, one branch is neutral, $\nu=kc_0$, while the other remains damped, $\nu=-kc_0-iR_0$. The maintained external-[pressure gradient](#pressure-gradient) supplies the energy; positive friction alone does not imply linear stability of a driven flow.

#### Pressure-area law of a collapsible tube

↑ **Parent:** [Collapsible tube flow](#collapsible-tube-flow)

The [pressure-area law of a collapsible tube](#pressure-area-law-of-a-collapsible-tube) describes transverse mechanical equilibrium of a deformable tube wall. On a stable branch $\widetilde P'(\alpha)>0$. Linearizing mass and momentum conservation about a stationary uniform tube gives the displayed [wave speed](wave-equation.md#wave-speed). External [pressure](thermodynamics.md#pressure) is prescribed separately and is not part of the elastic wall stiffness.

##### Tube wave speed

↑ **Parent:** [Pressure-area law of a collapsible tube](#pressure-area-law-of-a-collapsible-tube)

Linearizing area conservation and the axial momentum equation of a [collapsible tube flow](#collapsible-tube-flow) gives waves travelling relative to the fluid at speeds $\pm c$, where the displayed relation uses the area derivative at fixed external pressure. For $p=P_0+\rho c_0^2(A/A_0)^2/2$, it gives $c=c_0A/A_0$.

### Arterial pressure wave

↑ **Parent:** [Physiological fluid dynamics](#physiological-fluid-dynamics)

A small [pressure](thermodynamics.md#pressure) disturbance in an elastic artery propagates through the coupled inertia of blood and compliance of the wall. If $\mathcal A$ is the undisturbed area, $\rho$ the [mass density](#density) and $c$ the [wave speed](wave-equation.md#wave-speed), the linearized equations give $c^2=\mathcal A/\rho\,dp/d\mathcal A$. A travelling [pressure](thermodynamics.md#pressure) amplitude $p_+$ carries flow amplitude $\mathcal A p_+/(\rho c)$; the oppositely travelling wave has the opposite flow sign.

#### Bifurcation reflection of an arterial pressure wave

↑ **Parent:** [Arterial pressure wave](#arterial-pressure-wave)

At a lossless vascular junction, [pressure](thermodynamics.md#pressure) continuity and [volumetric flow rate](#volumetric-flow-rate) balance give $1+r=t$ and $Y_1(1-r)=Y_dt$, where $Y_d$ is the sum of daughter [characteristic admittances of an arterial wave](#characteristic-admittance-of-an-arterial-wave). Eliminating transmission amplitude $t$ gives the displayed [reflection coefficient](partial-differential-equation.md#reflection-coefficient). A decrease in total area yields positive reflection if parent and daughter wave speeds are equal; differing stiffnesses require comparison of the admittances rather than areas alone.

##### Pressure-flow phase lag from one arterial reflection

↑ **Parent:** [Bifurcation reflection of an arterial pressure wave](#bifurcation-reflection-of-an-arterial-pressure-wave)

For incident and reflected harmonic [arterial pressure waves](#arterial-pressure-wave) with real $0<r<1$, the local [pressure](thermodynamics.md#pressure) and flow phasors are proportional to $1+re^{-i\vartheta}$ and $1-re^{-i\vartheta}$. Their maximum-time difference is the displayed phase lag, on the branch $0<\vartheta<\pi$. Here $\vartheta=2\omega d/c$ is the round-trip phase to the reflector. Its derivative has the sign of $\cos\vartheta$. Raising the [wave speed](wave-equation.md#wave-speed) reduces the lag when $0<\vartheta<\pi/2$, but increases it when $\pi/2<\vartheta<\pi$. This conditional harmonic model does not establish an age trend for arbitrary vascular geometry or measurement stations beyond the sole reflector.

#### Reflection of an arterial pressure wave

↑ **Parent:** [Arterial pressure wave](#arterial-pressure-wave)

A [hydraulic resistance](#hydraulic-resistance) $R$ imposes $q=p/R$. Combining this with forward and backward [arterial pressure waves](#arterial-pressure-wave), $p=p_++p_-$ and $q=Y(p_+-p_-)$, gives the displayed [reflection coefficient](partial-differential-equation.md#reflection-coefficient). A matched load $RY=1$ has no reflected [pressure](thermodynamics.md#pressure) wave, while a closed end has [reflection coefficient](partial-differential-equation.md#reflection-coefficient) one. At a network junction the combined downstream input admittance replaces $1/R$.

#### Wave transfer matrix of an arterial segment

↑ **Parent:** [Arterial pressure wave](#arterial-pressure-wave)

For time dependence $e^{i\omega t}$ and a segment of length $\ell$, let $\beta=\omega\ell/c$. Adding the forward and backward [arterial pressure waves](#arterial-pressure-wave) gives the displayed upstream-to-downstream matrix. The flow orientation is downstream at both ends. At a junction, [pressure](thermodynamics.md#pressure) is continuous and incoming [volumetric flow rates](#volumetric-flow-rate) balance outgoing ones.

##### Wave transmission through a resistively loaded arterial loop

↑ **Parent:** [Wave transfer matrix of an arterial segment](#wave-transfer-matrix-of-an-arterial-segment)

Consider two identical two-segment paths from an inlet to a distal junction, with equal resistive beds at the two intermediate junctions and the distal junction. The segment transfer matrix and junction flow balances determine all [pressures](thermodynamics.md#pressure). If one inlet branch is removed and the beds are weakly loading the waves, the remaining segments form a three-segment chain with an effectively closed far end. The altered reflection pattern can raise peripheral oscillatory flow amplitudes even though a branch was lost; the incident wave amplitude, rather than total inlet [pressure](thermodynamics.md#pressure) or flow, is the prescribed forcing.

#### Characteristic admittance of an arterial wave

↑ **Parent:** [Arterial pressure wave](#arterial-pressure-wave)

The [characteristic admittance of an arterial wave](#characteristic-admittance-of-an-arterial-wave) relates the [volumetric flow rate](#volumetric-flow-rate) of a travelling [arterial pressure wave](#arterial-pressure-wave) to its [pressure](thermodynamics.md#pressure). For forward and backward amplitudes, $p=p_++p_-$ and $q=Y(p_+-p_-)$. It is the reciprocal of characteristic [pressure](thermodynamics.md#pressure)-to-flow impedance, and should not be confused with the reciprocal [hydraulic resistance](#hydraulic-resistance) of a steadily resistive segment.

## Fluid

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A fluid is a material that flows under sustained shear and cannot maintain a static shear stress in its fluid state. Liquids and gases are the usual examples. A [Newtonian fluid](viscous-fluid-flow.md#newtonian-fluid) has deviatoric stress proportional to its rate of deformation, whereas more general fluid constitutive laws can be nonlinear or have memory. In a [porous medium](porous-media-flow.md#porous-medium), the fluid occupies connected voids within a load-bearing solid framework.

## Buoyant plume

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A buoyant plume rises because its density differs from the surrounding fluid and entrains ambient fluid as it travels.

## Pathline

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A [pathline](#pathline) is a fluid particle's material trajectory through a time-dependent velocity field. Unlike a [streamline](#streamline), which follows the velocity field at one frozen time, a [pathline](#pathline) solves the displayed ODE. The two curves coincide in a steady flow but generally differ in an unsteady one.

## Control volume

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A [control volume](#control-volume) is a chosen region over which fluid [mass conservation](continuum-mechanics.md#mass-conservation) and momentum balance are integrated. It may be fixed or move with a prescribed [velocity](classical-mechanics.md#velocity). Boundary fluxes must use [velocity](classical-mechanics.md#velocity) relative to the moving boundary. In [Stokes flow](stokes-flow.md), negligible inertia reduces the momentum balance to the sum of body [forces](classical-mechanics.md#force) and boundary tractions, making a carefully chosen [control volume](#control-volume) useful for finding drag without integrating directly over a curved body.

## Navier slip boundary condition

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A Navier slip boundary condition relates fluid velocity relative to a stationary flat wall to the wall-normal tangential velocity gradient, $u_b=\ell_s u_z$, with positive [slip length](#slip-length) $\ell_s$. For a [Newtonian fluid](viscous-fluid-flow.md#newtonian-fluid), it is equivalent to linear resisting wall traction of magnitude $\mu u_b/\ell_s$. The normal points from the wall into the fluid; this fixes the sign convention.

### Slip length

↑ **Parent:** [Navier slip boundary condition](#navier-slip-boundary-condition)

The slip length is the distance obtained by extrapolating a locally linear tangential velocity profile back to zero velocity beneath a wall. A [Navier slip boundary condition](#navier-slip-boundary-condition) has $u_b=\ell_s\partial_nu$. Zero [slip length](#slip-length) gives a [no-slip boundary condition](viscous-fluid-flow.md#no-slip-boundary-condition); large slip permits approximately plug-like motion when the surrounding geometry and forces allow it.

## Fluid free boundary

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A [fluid free boundary](#fluid-free-boundary) is an initially unknown material interface separating a fluid from its exterior. For a [polytropic elliptical patch in a shearing sheet](gravitational-instability-of-an-astrophysical-disk.md#polytropic-elliptical-patch-in-a-shearing-sheet) bounded by vacuum, it is the level set $p=\rho=Q=0$, and the velocity is tangent to it in a steady solution.

## Material surface

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A material surface is transported with its [fluid elements](continuum-mechanics.md#fluid-element), including its boundary when open. Its oriented [material surface element](#material-surface-element) evolves by tangent transport. [Magnetic flux freezing](astrophysical-fluid-dynamics.md#magnetic-flux-freezing) conserves the flux through such an open surface.

### Material surface element

↑ **Parent:** [Material surface](#material-surface)

If $\mathbf A=\mathbf t_a\times\mathbf t_b\,da\,db$ and each tangent satisfies $D\mathbf t/Dt=(\nabla\mathbf u)\mathbf t$, differentiation of the cross product gives $D\mathbf A/Dt=(\nabla\cdot\mathbf u)\mathbf A-(\nabla\mathbf u)^T\mathbf A$. Combining this with ideal induction proves pointwise conservation of $\mathbf B\cdot\mathbf A$.

## Material curve

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A material curve consists of the same [fluid elements](continuum-mechanics.md#fluid-element) at all times. Differentiating their flow map gives $D\boldsymbol\ell/Dt=(\boldsymbol\ell\cdot\nabla)\mathbf u$ for its tangent. In [ideal magnetohydrodynamics](astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamics) a magnetic-field tangent obeys this same transport law after division by [mass density](#density).

## Scalar transport

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[Scalar transport](#scalar-transport) follows a material quantity through [advection](#advection) and [diffusion equation](diffusion-equation.md) terms, for example $\Theta_t+\mathbf U\cdot\nabla\Theta=\kappa\Delta\Theta$. A [passive scalar](#passive-scalar) does not affect the [velocity field](#velocity-field); an [active scalar](#active-scalar) feeds back through forces such as [buoyancy](#buoyancy). With [incompressible flow](#incompressible-flow) bounded by impermeable walls and homogeneous [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition), the spatial mean is conserved.

### Active scalar

↑ **Parent:** [Scalar transport](#scalar-transport)

An [active scalar](#active-scalar) is a transported [scalar field](quantum-field-theory.md#scalar-field) that feeds back on the [velocity field](#velocity-field), for example a density anomaly producing [buoyancy](#buoyancy). In an [adjoint equations for Boussinesq scalar mixing](#adjoint-equations-for-boussinesq-scalar-mixing) calculation its dynamical coupling must also be transposed; a passive-scalar sensitivity equation generally omits that feedback.

### Passive scalar

↑ **Parent:** [Scalar transport](#scalar-transport)

A [passive scalar](#passive-scalar) is an advected and diffusing [scalar field](quantum-field-theory.md#scalar-field) whose value has no dynamical effect on the transporting [velocity field](#velocity-field). Concentration of a dilute nonreacting dye is a common example. Its transport can depend on the flow while the flow equations remain independent of it.

#### Gaussian scalar packet in a linear incompressible flow

↑ **Parent:** [Passive scalar](#passive-scalar)

For $\chi=f\exp(-\boldsymbol x^TB\boldsymbol x)$ in two dimensions, take $B$ positive definite, $\operatorname{tr}C=0$ and positive conserved mass $Q=\int\chi\,dA$. The [Gaussian integral](calculus.md#gaussian-integral) gives $Q=\pi f/\sqrt{\det B}$, $J=(Q/2)B^{-1}$ and $f=Q^2/(2\pi\sqrt{\det J})$. Substitution in the [advection-diffusion equation](diffusion-equation.md#advection-diffusion-equation) gives $\dot B=-C^TB-BC-4\kappa B^2$ and $\dot f/f=-2\kappa\operatorname{tr}B$, equivalently the displayed moment equation. If $\dot F=CF$, its solution is $J=F[J_0+2\kappa Q\int_0^tF^{-1}(s)F^{-T}(s)ds]F^T$, with $\det F=1$.

##### Diffusion arrest of Gaussian packet compression

↑ **Parent:** [Gaussian scalar packet in a linear incompressible flow](#gaussian-scalar-packet-in-a-linear-incompressible-flow)

For a chaotic incompressible planar flow with [Lyapunov exponent](dynamical-systems.md#lyapunov-exponent) pair $\lambda,-\lambda$, an initially broad [Gaussian scalar packet in a linear incompressible flow](#gaussian-scalar-packet-in-a-linear-incompressible-flow) stretches and compresses exponentially while diffusion is negligible. Its compressed variance stops decreasing around $\kappa/\lambda$, the [Batchelor scalar microscale](#batchelor-scalar-microscale) balance, while the larger variance continues to grow. In a constant principal strain, the normalized covariance eigenvalues obey $\dot j_\pm=\pm2\lambda j_\pm+2\kappa$, proving that the compressed one approaches $\kappa/\lambda$. Random finite-correlation strain instead gives a fluctuating compressed width; stationarity and integrability assumptions are required to turn this into exponential statistics of the packet amplitude.

###### Large-deviation decay rates of a Gaussian scalar packet

↑ **Parent:** [Diffusion arrest of Gaussian packet compression](#diffusion-arrest-of-gaussian-packet-compression)

After [diffusion arrest of Gaussian packet compression](#diffusion-arrest-of-gaussian-packet-compression), define the logarithmic area increase $A_t=\tfrac12\log[\det J(t)/\det J(0)]$. It is nonnegative. Assume $A_t/t$ has a [large deviation principle](convergence-of-random-variables.md#large-deviation-principle) with convex [rate function](convergence-of-random-variables.md#rate-function) $\mathcal I$, minimized at $\lambda>0$. The exact amplitude relation $f(t)=f(0)e^{-A_t}$ and the [Laplace principle for probability measures](convergence-of-random-variables.md#laplace-principle-for-probability-measures) give the displayed moment decay rate. The rate function refers to area, so rare width fluctuations are included rather than discarded without justification. For differentiable strictly convex $\mathcal I$, the interior minimizer satisfies $\mathcal I'(s_\mu)=-\mu$. If $\mu_*=-\mathcal I'(0)$ is finite, then $\gamma_\mu=\mathcal I(0)$ for $\mu\ge\mu_*$: rare nearly unstretched packets dominate high moments. Below the threshold, $d(\gamma_\mu/\mu)/d\mu=-\mathcal I(s_\mu)/\mu^2<0$. These statements concern a positive Gaussian packet with flow-only averaging; a homogeneous signed random initial scalar requires a different averaging kernel. Arbitrary random $C(t)$ alone does not imply this statistical model.

#### Schmidt number (fluid mechanics)

↑ **Parent:** [Passive scalar](#passive-scalar)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schmidt_number)

The molecular Schmidt number is the ratio of [kinematic viscosity](#kinematic-viscosity) to scalar [diffusivity](brownian-motion.md#diffusion-coefficient). A large value allows a [passive scalar](#passive-scalar) to develop structure below the viscous smoothing scale of the [velocity field](#velocity-field). It is distinct from the [turbulent Schmidt number](turbulence.md#turbulent-schmidt-number), which compares effective turbulent transport coefficients, and from the [Schmidt number](von-neumann-entropy.md#schmidt-number) used for quantum entanglement.

#### Covector evolution of a material scalar gradient

↑ **Parent:** [Passive scalar](#passive-scalar)

Differentiate the [advection equation](partial-differential-equation.md#transport-equation) componentwise: $D_t(\partial_i\theta)=-(\partial_i u_j)\partial_j\theta$. Along a [Lagrangian trajectory](continuum-mechanics.md#lagrangian-trajectory), the scalar [gradient](calculus.md#gradient) therefore evolves by the negative transpose of the [velocity gradient tensor](#velocity-gradient-tensor). If $F$ is the [deformation gradient](continuum-mechanics.md#deformation-gradient), this says $\boldsymbol k(t)=F(t)^{-T}\boldsymbol k(0)$, as expected for a [covector](linear-algebra.md#covector). Fluid material vectors and scalar gradients transform oppositely under stretching.

##### Scalar-gradient inclination in a steady planar strain

↑ **Parent:** [Covector evolution of a material scalar gradient](#covector-evolution-of-a-material-scalar-gradient)

For horizontal strain matrix $S=\bigl(\begin{smallmatrix}a&b\\b&-a\end{smallmatrix}\bigr)$ and zero vertical velocity, horizontal scalar gradients obey $\dot k_h=-Sk_h$. Since $S^2=c^2I$ with $c=\sqrt{a^2+b^2}$, the growing projection is $(I-S/c)k_h(0)/2$. If nonzero it equals $k_0(\cos\phi,\sin\phi)$ and grows as $e^{ct}$. Fixed vertical shears give $\dot k_3=-\sigma_{13}k_1-\sigma_{23}k_2$, so $k_3\sim-k_0D e^{ct}/c$ with $D=\sigma_{13}\cos\phi+\sigma_{23}\sin\phi$. The ratio $\alpha=|k_3|/|k_h|$ tends to the displayed value. It measures scalar-isosurface orientation; zero growing projection or $D=0$ must not be described as generic exponential vertical-gradient growth.

###### White-noise vertical shear gives an Ornstein-Uhlenbeck inclination

↑ **Parent:** [Scalar-gradient inclination in a steady planar strain](#scalar-gradient-inclination-in-a-steady-planar-strain)

In the long-time growing horizontal-gradient branch, independent vertical shear noises combine as $\cos\phi\,dW_1+\sin\phi\,dW_2=dW$. The signed inclination $\beta=k_3e^{-ct}/k_0$ satisfies the displayed [Ornstein-Uhlenbeck stochastic differential equation](stochastic-process.md#ornstein-uhlenbeck-stochastic-differential-equation). For $c>0$ its stationary density is $\sqrt{c/(\pi g^2)}e^{-cB^2/g^2}$, with variance $g^2/(2c)$. The [Fokker-Planck probability current](probability-theory.md#fokker-planck-probability-current) vanishes at infinity and gives this Gaussian by one integration. At $c=0$ and nonzero noise there is no normalizable stationary density.

###### Gaussian-over-Rayleigh inclination distribution

↑ **Parent:** [Scalar-gradient inclination in a steady planar strain](#scalar-gradient-inclination-in-a-steady-planar-strain)

Let $c=\sqrt{a^2+b^2}$ with independent $a,b\sim N(0,\Gamma^2)$, and let $D\sim N(0,\Lambda^2)$ be independent of them. Then $c$ has [Rayleigh distribution](continuous-probability-distribution.md#rayleigh-distribution) and $\alpha=|D|/c$ has the displayed [cumulative distribution function](probability-theory.md#cumulative-distribution-function) for $A\ge0$ and density $\Lambda^2\Gamma(\Gamma^2A^2+\Lambda^2)^{-3/2}$. Indeed, conditioning on $D$ gives $\mathbb P(c\ge|D|/A)=\exp[-D^2/(2\Gamma^2A^2)]$, and a [Gaussian integral](calculus.md#gaussian-integral) completes the calculation. Independence is essential: choosing $D=(\Lambda/\Gamma)a$ has the same Gaussian marginal but makes the ratio bounded by $\Lambda/\Gamma$.

#### Scalar structure function

↑ **Parent:** [Passive scalar](#passive-scalar)

For a homogeneous scalar, $S_C(r)=2[\langle C^2\rangle-\langle CC'\rangle]$. Decorrelation at large separation gives saturation at twice the variance. If the scalar is mean-square differentiable and isotropic, $S_C(r)=r^2\langle|\nabla C|^2\rangle/3+o(r^2)$ at small separation. Statistical isotropy and zero mean alone do not imply decorrelation at infinity.

#### Obukhov-Corrsin theory

↑ **Parent:** [Passive scalar](#passive-scalar)

Obukhov-Corrsin theory concerns transfer of [scalar variance](#scalar-variance) across scales in turbulent mixing. In the inertial-convective range, a constant scalar-variance flux and an eddy turnover time $\epsilon^{-1/3}r^{2/3}$ predict the displayed second-order [scalar structure function](#scalar-structure-function). It assumes a passive scalar, local transfer, approximate statistical equilibrium and separation from the molecular diffusion and forcing scales.

##### Inertial-diffusive scalar range

↑ **Parent:** [Obukhov-Corrsin theory](#obukhov-corrsin-theory)

For scalar diffusivity much larger than [kinematic viscosity](#kinematic-viscosity), scalar diffusion dominates at lengths between the Kolmogorov and scalar cutoff scales. The velocity may still have inertial-range variations, but the scalar is smooth to leading order. The leading isotropic [scalar structure function](#scalar-structure-function) is quadratic, with coefficient fixed by the mean-square gradient and the [scalar dissipation rate](#scalar-dissipation-rate), rather than by a continuing inertial-convective two-thirds law.

###### Corrsin scalar microscale

↑ **Parent:** [Inertial-diffusive scalar range](#inertial-diffusive-scalar-range)

In the large-diffusivity regime, equate diffusion rate $\alpha/r^2$ with inertial eddy rate $\epsilon^{1/3}r^{-2/3}$. This gives the Corrsin scalar microscale, which exceeds the [Kolmogorov length scale](turbulence.md#kolmogorov-length-scale) when $\alpha\gg\nu$.

##### Viscous-convective scalar range

↑ **Parent:** [Obukhov-Corrsin theory](#obukhov-corrsin-theory)

For scalar diffusivity much smaller than [kinematic viscosity](#kinematic-viscosity), a scalar has structure below the [Kolmogorov length scale](turbulence.md#kolmogorov-length-scale) while the velocity is smooth. The strain rate $s\sim(\epsilon/\nu)^{1/2}$ transfers scalar variance, giving $dS_C/dr\sim\epsilon_c/(sr)$. Integration produces a logarithm plus an additive matching constant.

###### Batchelor scalar microscale

↑ **Parent:** [Viscous-convective scalar range](#viscous-convective-scalar-range)

At the Batchelor scalar microscale, molecular diffusion rate $\alpha/r^2$ balances the smooth Kolmogorov strain rate $(\epsilon/\nu)^{1/2}$. For $\alpha\ll\nu$ this scale is much smaller than the [Kolmogorov length scale](turbulence.md#kolmogorov-length-scale).

##### Inertial-convective scalar range

↑ **Parent:** [Obukhov-Corrsin theory](#obukhov-corrsin-theory)

This range lies above both the [Kolmogorov length scale](turbulence.md#kolmogorov-length-scale) and the scalar diffusion cutoff, but below the forcing scale. Molecular viscosity and scalar diffusion have negligible direct influence on transfer at those scales. The [Obukhov-Corrsin theory](#obukhov-corrsin-theory) predicts a two-thirds [scalar structure function](#scalar-structure-function) there.

#### Horizontally integrated plume concentration

↑ **Parent:** [Passive scalar](#passive-scalar)

The horizontally integrated plume concentration is the [integral](calculus.md#integral) of a local [concentration](physics.md#concentration) $C$ across the plume. It measures scalar amount per unit vertical length and unit span, and its vertical [integral](calculus.md#integral) is total scalar amount per unit span. Unlike a local [concentration](physics.md#concentration), its dimensions include one horizontal length. It must be distinguished from [horizontally averaged plume concentration](#horizontally-averaged-plume-concentration) when a plume's width varies with height.

##### Horizontally averaged plume concentration

↑ **Parent:** [Horizontally integrated plume concentration](#horizontally-integrated-plume-concentration)

For a plume of full width $w(z)$, its horizontally averaged [concentration](physics.md#concentration) is $\overline C(z,t)=c(z,t)/w(z)$, where $c$ is [horizontally integrated plume concentration](#horizontally-integrated-plume-concentration). In a [line plume](turbulent-plume.md#line-plume) with $w=\mu z$, division by $z$ generally changes the location of maximum [concentration](physics.md#concentration). A gradient closure for $c$ differs from one for $\overline C$: $w\partial_z\overline C=c_z-c/z$, so integrated diffusive flux $-Kw\partial_z\overline C$ equals $-K(c_z-c/z)$.

### Adjoint equations for Boussinesq scalar mixing

↑ **Parent:** [Scalar transport](#scalar-transport)

For a smooth incompressible direct trajectory with total [velocity field](#velocity-field) $\mathbf U$ and [active scalar](#active-scalar) $\Theta$, the negative-constraint [Lagrangian function in constrained optimization](calculus-of-variations.md#lagrangian-function-in-constrained-optimization) convention gives

$$
\partial_t\mathbf u^\dagger+\mathbf U\cdot\nabla\mathbf u^\dagger-(\nabla\mathbf U)^T\mathbf u^\dagger+\nabla p^\dagger+\nu\Delta\mathbf u^\dagger-\theta^\dagger\nabla\Theta=0,\qquad \nabla\cdot\mathbf u^\dagger=0,
$$



$$
\partial_t\theta^\dagger+\mathbf U\cdot\nabla\theta^\dagger+\kappa\Delta\theta^\dagger-\mathrm{Ri}_B u_y^\dagger=0.
$$

The transpose term is the [formal adjoint](hilbert-space.md#formal-adjoint) of $\delta\mathbf u\cdot\nabla\mathbf U$; the two couplings transpose [scalar transport](#scalar-transport) by [advection](#advection) and [buoyancy](#buoyancy). For terminal cost $\int\Theta(T)^2$, the terminal data are $\mathbf u^\dagger(T)=0$, $\theta^\dagger(T)=2\Theta(T)$. They are integrated backward along the stored direct trajectory. [No-slip boundary conditions](viscous-fluid-flow.md#no-slip-boundary-condition) and [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition) for the adjoint [velocity](classical-mechanics.md#velocity) and homogeneous [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition) for the adjoint scalar remove the spatial boundary terms.

### Scalar variance

↑ **Parent:** [Scalar transport](#scalar-transport)

[Scalar variance](#scalar-variance) measures spatial departure from the conserved mean. For zero mean, [incompressible flow](#incompressible-flow) bounded by impermeable walls and homogeneous scalar [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition), [integration by parts](calculus.md#integration-by-parts) gives $d\int\Theta^2/dt=-2\kappa\int|\nabla\Theta|^2$. [Advection](#advection) preserves the instantaneous quadratic integral but can sharpen [gradients](calculus.md#gradient), allowing the [diffusion equation](diffusion-equation.md) to remove [scalar variance](#scalar-variance) faster.

#### Scalar dissipation rate

↑ **Parent:** [Scalar variance](#scalar-variance)

With this half-variance convention, the unforced scalar equation gives $d\langle C^2/2\rangle/dt=-\epsilon_c$ in a homogeneous incompressible flow. Authors defining dissipation of the full variance instead use $2\alpha\langle|\nabla C|^2\rangle$. Stating the convention is necessary when relating the dissipation rate to a [scalar structure function](#scalar-structure-function).

## Fluid flow

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A [fluid flow](#fluid-flow) is motion described by a [velocity field](#velocity-field) $\mathbf u(\mathbf x,t)$. The trajectories of [fluid elements](continuum-mechanics.md#fluid-element) satisfy $d\mathbf x/dt=\mathbf u(\mathbf x,t)$; the [mass density](#density) and other fields obey their [conservation laws](physics.md#conservation-law) and [constitutive equations](continuum-mechanics.md#constitutive-equation). This physical motion differs from a [flow](graph-theory.md#flow) on a [flow network](graph-theory.md#flow-network).

### Unidirectional flow

↑ **Parent:** [Fluid flow](#fluid-flow)

A unidirectional flow has velocity parallel to a single fixed direction, for example $\boldsymbol u=u(y)\boldsymbol e_x$. If the speed is independent of the coordinate along that direction, the convective acceleration $(\boldsymbol u\cdot\nabla)\boldsymbol u$ vanishes. The steady [Navier-Stokes equation](viscous-fluid-flow.md#navier-stokes-equation) then reduces to a linear balance of the pressure gradient and viscosity, as in [Couette flow](viscous-fluid-flow.md#couette-flow) and [Poiseuille flow](viscous-fluid-flow.md#hagen-poiseuille-equation).

### Steady flow

↑ **Parent:** [Fluid flow](#fluid-flow)

In steady flow, the velocity and other relevant flow fields are independent of time in the chosen reference frame. [Streamlines](#streamline) then coincide with the paths of moving particles, while [convective acceleration](continuum-mechanics.md#convective-acceleration) can still be nonzero.

### Inviscid flow

↑ **Parent:** [Fluid flow](#fluid-flow)

An inviscid flow neglects [viscosity](#dynamic-viscosity) in the [fluid flow](#fluid-flow). Its [momentum](classical-mechanics.md#momentum) balance is described by the [Euler equations for an inviscid fluid](#euler-equations-for-an-inviscid-fluid).

#### Inviscid falling jet and radial impact film

↑ **Parent:** [Inviscid flow](#inviscid-flow)

A steady incompressible jet at atmospheric [pressure](thermodynamics.md#pressure) conserves [Bernoulli's equation](#bernoulli-equation) and [volume flux](#volumetric-flow-rate). Its radius contracts as $R=a[u/u_0]^{-1/2}$. After impact, a thin nearly horizontal axisymmetric film has $2\pi rhv=\pi a^2u_0$. Evaluating [Bernoulli's equation](#bernoulli-equation) on its [free surface](#free-surface) gives $v^2=u_0^2+2g(H-h)$, hence $a^4/(4r^2h^2)=1+2g(H-h)/u_0^2$. This inviscid thin-film description applies away from the impact region and does not describe a dissipative hydraulic jump.

## Sediment transport

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sediment_transport)

### Sediment resuspension

↑ **Parent:** [Sediment transport](#sediment-transport)

Sediment resuspension transfers deposited bed particles into a [particle suspension](#suspension-chemistry). It can supply particle [buoyancy flux](turbulent-plume.md#buoyancy-flux) to a [particle-laden gravity current](reduced-gravity.md#particle-laden-gravity-current) if erosion or upward mixing exceeds settling losses. Ambient fluid without particles dilutes concentration without supplying particle mass.

#### Equilibrium settling-diffusion profile

↑ **Parent:** [Sediment resuspension](#sediment-resuspension)

For downward [settling velocity](#settling-velocity) magnitude $W_s>0$ and [eddy diffusivity](turbulence.md#eddy-diffusivity) $\kappa_T=Kz$, the total upward particle flux is $J=-W_s\phi-Kz\phi_z$. A stationary profile tending to zero at infinity has $J=0$, giving the displayed power law. The exponent compares settling with turbulent mixing. It describes a region above the bed; entrainment from the bed and viscous near-wall effects determine the reference concentration separately.

### Sediment transport saturation

↑ **Parent:** [Sediment transport](#sediment-transport)

#### Equilibrium sediment flux

↑ **Parent:** [Sediment transport saturation](#sediment-transport-saturation)

The [equilibrium sediment flux](#equilibrium-sediment-flux) is the transport supported locally by a prescribed bed [shear stress](viscous-fluid-flow.md#shear-stress). A common idealization is $q_{\mathrm{sat}}=\phi_b\chi(\tau-\tau_{\mathrm{th}})_+^\gamma$. Linearization above the [sediment entrainment threshold](#sediment-entrainment-threshold) requires perturbations small compared with the positive excess stress.

#### Saturation length

↑ **Parent:** [Sediment transport saturation](#sediment-transport-saturation)

The [saturation length](#saturation-length) measures downstream relaxation of a transported grain population toward its equilibrium [sediment transport](#sediment-transport) flux. The elementary steady relaxation law is $L_{\mathrm{sat}}q_x=q_{\mathrm{sat}}-q$; it introduces a phase lag between forcing and actual transport.

### Exner equation

↑ **Parent:** [Sediment transport](#sediment-transport)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Exner_equation)

The [Exner equation](#exner-equation) is local sediment [mass conservation](continuum-mechanics.md#mass-conservation) expressed in terms of solid volume: accumulation raises the bed and flux divergence lowers it. Here $\phi_b$ is the solid volume fraction of the packed bed and $q$ is solid volume flux per unit width.

### Shields parameter

↑ **Parent:** [Sediment transport](#sediment-transport)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Shields_parameter)

The [Shields parameter](#shields-parameter) is $\Theta=\tau/[(\rho_p-\rho_f)gd]$, comparing bed [shear stress](viscous-fluid-flow.md#shear-stress) with a grain-scale [submerged weight](#submerged-weight) per area. Its critical value depends on the assumed [drag coefficient](#drag-coefficient), [static friction](classical-mechanics.md#static-friction), lift, and contact geometry.

#### Sediment entrainment threshold

↑ **Parent:** [Shields parameter](#shields-parameter)

The [sediment entrainment threshold](#sediment-entrainment-threshold) is the bed [shear stress](viscous-fluid-flow.md#shear-stress) at which resting grains begin moving. An elementary [force balance](classical-mechanics.md#force-balance) using spherical grains, tangential [quadratic drag](#quadratic-drag), and [static friction](classical-mechanics.md#static-friction) gives $\Theta_{\mathrm{th},0}=4\mu_s/(3C_D)$ when the [drag coefficient](#drag-coefficient) is defined relative to the bed [shear velocity](viscous-fluid-flow.md#shear-velocity).

##### Inclined-bed sediment threshold

↑ **Parent:** [Sediment entrainment threshold](#sediment-entrainment-threshold)

For locally bed-tangent [drag force](#drag-physics) and an upslope angle $a$, a spherical-grain [force balance](classical-mechanics.md#force-balance) gives $\tau_{\mathrm{th}}(a)=\tau_{\mathrm{th},0}(\cos a+\sin a/\mu_s)$. The small-slope term is $\delta\tau_{\mathrm{th}}=(\tau_{\mathrm{th},0}/\mu_s)\eta_x$. A horizontal [drag force](#drag-physics) instead changes the normal contact [force](classical-mechanics.md#force) and gives a different slope correction.

### Bedform

↑ **Parent:** [Sediment transport](#sediment-transport)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bedform)

#### Sediment-bed linear instability

↑ **Parent:** [Bedform](#bedform)

Combining the [Exner equation](#exner-equation), [sediment transport saturation](#sediment-transport-saturation), [bed shear response](#bed-shear-response), and [inclined-bed sediment threshold](#inclined-bed-sediment-threshold) gives a competition between upstream forcing and downstream relaxation. With $a=\tau_0A$, $b=\tau_0B-\tau_{\mathrm{th},0}/\mu_s$, $C=\chi\gamma(\tau_0-\tau_{\mathrm{th},0})^{\gamma-1}$, and positive [wavenumber](wave-equation.md#wavenumber) $k$, the [growth rate](wave-equation.md#growth-rate) is $\sigma=Ck^2(b-akL_{\mathrm{sat}})/(1+k^2L_{\mathrm{sat}}^2)$. Thus $b>0$ permits long-wave growth when $a>0$, while a finite [saturation length](#saturation-length) stabilizes shorter waves.

#### Bed shear response

↑ **Parent:** [Bedform](#bedform)

For a small sinusoidal [bedform](#bedform), a fluid-dynamical closure can be written $\hat\tau=\tau_0k(A+iB)\hat\eta$ for $k>0$. The real coefficient $A$ is in phase with the bed height and $B$ describes an upstream phase lead. Neither coefficient follows from the [Exner equation](#exner-equation) or sediment relaxation alone; they require a flow calculation or measurement.

## Ram pressure

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ram_pressure)

The momentum-flux [pressure](thermodynamics.md#pressure) associated with a moving fluid. Some energy-density balances use $\rho v^2/2$ instead; the numerical convention must be stated when balancing [magnetic pressure](astrophysical-fluid-dynamics.md#magnetic-pressure).

## Turbulence

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](turbulence.md)

## Acoustic wave

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Acoustic_wave)

An acoustic wave is a propagating pressure and density disturbance in a material medium. Linear sound waves oscillate when pressure restores a displaced fluid element.

### Burgers reduction of weakly nonlinear rightgoing acoustics

↑ **Parent:** [Acoustic wave](#acoustic-wave)

For a pure rightgoing [acoustic wave](#acoustic-wave), retarded time $\theta=t-x$ and slow distance $X=Mx$ separate fast oscillations from nonlinear steepening. Expanding the [equation of state](thermodynamics.md#equation-of-state) gives $p=\rho+M(\gamma-1)\rho^2/2+O(M^2)$. The leading perturbations satisfy $u_0=\rho_0=p_0$. Adding the first-order [mass conservation](continuum-mechanics.md#mass-conservation) and [momentum conservation](classical-mechanics.md#momentum-conservation) equations cancels the unknown first corrections and yields the displayed [viscous Burgers equation](partial-differential-equation.md#viscous-burgers-equation). Inviscid characteristics satisfy $\theta=s-(\gamma+1)F(s)X/2$, $p=F(s)$; loss of invertibility marks [shock](partial-differential-equation.md#shock-wave) formation and the end of the smooth inviscid approximation.

### Adiabatic vertical modes of a Gaussian atmosphere

↑ **Parent:** [Acoustic wave](#acoustic-wave)

A [plane-parallel atmosphere](astrophysics.md#plane-parallel-atmosphere) with [isothermal sound speed](compressible-flow.md#isothermal-sound-speed) $c_s$ in gravity $-\Omega^2z$ has [mass density](#density) $\rho_0e^{-z^2/(2H^2)}$, $H=c_s/\Omega$. Above a rigid base, vertically directed [adiabatic fluid perturbations](#adiabatic-fluid-perturbation) satisfy $w''-zw'/H^2+(\sigma^2/\Omega^2-1)w/(\gamma H^2)=0$ and $w(0)=0$. Set $x=z/H$ and $\lambda=(\sigma^2/\Omega^2-1)/\gamma$. The substitution $y=e^{-x^2/4}w$ converts finite Gaussian-weighted [kinetic energy](classical-mechanics.md#kinetic-energy) into square integrability for $-y''+x^2y/4=(\lambda+1/2)y$. Odd extension across the base and the oscillator lowering operator force $\lambda$ to be an odd positive integer. Thus $w_n$ is proportional to the [Probabilists' Hermite polynomial](numerical-analysis.md#probabilists-hermite-polynomial) $\mathrm{He}_{2n+1}(z/H)$. These are vertical [acoustic waves](#acoustic-wave); a general stably stratified atmosphere also admits [internal gravity waves](gravity-wave.md#internal-wave) with horizontal structure.

### Acoustically rigid boundary

↑ **Parent:** [Acoustic wave](#acoustic-wave)

An acoustically rigid boundary has zero perturbation [normal velocity](classical-mechanics.md#normal-velocity). For a reflected [acoustic plane wave](physics.md#acoustic-plane-wave), [pressure](thermodynamics.md#pressure) amplitudes add in phase and the [reflection coefficient](partial-differential-equation.md#reflection-coefficient) is $+1$. It is the infinite-[surface acoustic impedance](continuum-mechanics.md#surface-acoustic-impedance) limit. A [pressure-release boundary](#pressure-release-boundary) instead fixes the [pressure](thermodynamics.md#pressure) perturbation to zero and reflects with coefficient $-1$.

### Acoustic cutoff frequency

↑ **Parent:** [Acoustic wave](#acoustic-wave)

A stratified atmosphere can reflect low-frequency [acoustic waves](#acoustic-wave) while permitting sufficiently high-frequency waves to escape. In a plane-parallel isothermal atmosphere, the angular acoustic cutoff is approximately $c_s/(2H_\rho)$, where $H_\rho$ is the density scale height. Its detailed form depends on the atmospheric profile and on the wave-variable approximation.

### Pressure-release boundary

↑ **Parent:** [Acoustic wave](#acoustic-wave)

A pressure-release boundary imposes zero acoustic pressure disturbance, $\widetilde p=0$. The incident and reflected pressure amplitudes therefore obey $1+R=0$, so the pressure [reflection coefficient](partial-differential-equation.md#reflection-coefficient) is $R=-1$. It contrasts with a rigid inviscid boundary, where zero normal velocity gives $R=+1$. A much lower normal impedance on the far side approximates the pressure-release condition.

## Velocity field

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A velocity field assigns a velocity vector to every position and time in a moving continuum. Its spatial derivatives describe local deformation, rotation, and volume change.

### Secondary flow

↑ **Parent:** [Velocity field](#velocity-field)

A secondary flow is a usually smaller velocity component superposed on a primary flow selected by symmetry or a simplified force balance. Examples include meridional circulation around a rotating sphere, or transverse circulation in a curved channel. Its direction depends on the forcing mechanism: elastic [normal stresses](continuum-mechanics.md#normal-stress) and inertial effects can produce opposite circulations.

### Velocity gradient tensor

↑ **Parent:** [Velocity field](#velocity-field)

The [velocity gradient tensor](#velocity-gradient-tensor) is $A_{ij}=\partial_j u_i$. Its symmetric part is the [rate-of-strain tensor](viscous-fluid-flow.md#strain-rate-tensor) $S$ and its antisymmetric part describes local rotation. For [incompressible flow](#incompressible-flow), $\operatorname{tr}A=\operatorname{tr}S=0$. The sign convention for a cubic invariant must be specified explicitly.

### Vertical velocity

↑ **Parent:** [Velocity field](#velocity-field)

The vertical velocity is the component of a fluid [velocity field](#velocity-field) along the selected upward vertical direction. In [incompressible flow](#incompressible-flow), impermeable horizontal boundaries impose $w=0$. Eliminating [pressure](thermodynamics.md#pressure) often yields a closed [hydrodynamic stability](hydrodynamic-stability.md) equation for this component.

### Axisymmetric flow

↑ **Parent:** [Velocity field](#velocity-field)

An axisymmetric flow is invariant under rotations about one fixed axis, so scalar fields and cylindrical-coordinate velocity components do not depend on the azimuthal angle.

## Advection

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Advection)

Advection transports a quantity with a [velocity field](#velocity-field). For a scalar field $f$, its local advective rate is $\mathbf u\mathbin\cdot\nabla f$, the spatial contribution to the [material derivative](continuum-mechanics.md#material-derivative). The same term transports the components of a vector field.

### Chaotic advection

↑ **Parent:** [Advection](#advection)

Chaotic advection is complicated, sensitive material motion generated by a smooth [velocity field](#velocity-field), often even when the Eulerian flow is periodic and simple. Transverse intersections of [stable manifolds](dynamical-systems.md#stable-manifold) and [unstable manifolds](dynamical-systems.md#unstable-manifold) create stretching, folding and lobe transport across former [separatrices](dynamical-systems.md#separatrix). [Incompressible flow](#incompressible-flow) preserves parcel area and advected scalar values in the absence of [diffusion](thermodynamics.md#diffusion), so chaotic motion can create fine filaments without independently producing molecular homogenization.

### Ballistic transport

↑ **Parent:** [Advection](#advection)

A trajectory with a persistent random velocity $V$ has $X(t)-X(0)=Vt$. An ensemble with finite velocity variance therefore has displacement variance $t^2\operatorname{Var}V$, contrasting with the linear-in-time variance of [diffusion](thermodynamics.md#diffusion). In an [impulsively kicked sinusoidal shear dispersion](#impulsively-kicked-sinusoidal-shear-dispersion) model with zero transverse diffusivity, the shear phase never changes and repeated identical kicks have this ballistic scaling. Transverse diffusion instead decorrelates the velocity and permits a long-time diffusive limit.

## Convection

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Convection)

Convection transports properties such as [energy](classical-mechanics.md#energy) or composition through bulk fluid motion. [Thermal convection](#thermal-convection) is driven by temperature-dependent [buoyancy](#buoyancy).

### Convection cell

↑ **Parent:** [Convection](#convection)

An organized region of buoyant rising fluid and compensating descending flow that transports heat or composition. [Convection rolls](#convection-roll) are a simple planar example; [solar granules](stellar-astrophysics.md#solar-granule) are evolving compressible examples. A cellular pattern does not require every material trajectory to form a closed streamline, especially near a radiating free surface.

### Convection zone

↑ **Parent:** [Convection](#convection)

A stellar [convection zone](#convection-zone) is a region where buoyant fluid motion transports a significant part of the stellar heat flux. Rising and sinking parcels carry enthalpy, so heat transport is not entirely radiative. The [Sun](stellar-astrophysics.md#sun)'s outer [convection zone](#convection-zone) extends from near $0.7R_\odot$ to the surface and overlies its radiative interior. The [tachocline](stellar-astrophysics.md#tachocline) lies near this transition, and the [convection](#convection) helps power the [solar dynamo](stellar-astrophysics.md#solar-dynamo).

### Compositional convection

↑ **Parent:** [Convection](#convection)

Compositional convection is buoyancy-driven motion caused by composition-dependent density variations. In a planetary core, freezing can expel light elements into the surrounding liquid, making that liquid buoyant and supplying mechanical power for a [planetary dynamo](planetary-science.md#planetary-dynamo). It can operate alongside thermally driven [convection](#convection) and release of [latent heat](thermodynamics.md#latent-heat).

### Long-wave convection equation with broken Boussinesq symmetry

↑ **Parent:** [Convection](#convection)

A reduced long-wave [convection](#convection) model can combine linear damping, destabilizing second derivatives, stabilizing fourth derivatives and gradient nonlinearities. In the displayed normalization the quadratic coefficient $s$ breaks [Boussinesq symmetry](geophysical-fluid-dynamics.md#boussinesq-up-down-symmetry), while the cubic gradient term dissipates the mean-square temperature. The linear [dispersion relation](wave-equation.md#dispersion-relation) is $\lambda(k)=-1+\mu k^2-k^4$, with critical [wavenumber](wave-equation.md#wavenumber) $k=1$ at $\mu=2$. Smoothness and spatial averaging hypotheses must be specified before applying the [energy method](numerical-analysis.md#energy-method) on an infinite interval.

#### Second-harmonic feedback in a long-wave convection amplitude equation

↑ **Parent:** [Long-wave convection equation with broken Boussinesq symmetry](#long-wave-convection-equation-with-broken-boussinesq-symmetry)

In a [weakly nonlinear expansion](differential-equation.md#weakly-nonlinear-expansion) of the [long-wave convection equation with broken Boussinesq symmetry](#long-wave-convection-equation-with-broken-boussinesq-symmetry) at $\mu=2$, a critical [Fourier mode](fourier-analysis.md#fourier-mode) $\Theta_1=Ae^{ix}+\mathrm{c.c.}$ generates $\Theta_2=(2is/9)A^2e^{2ix}+\mathrm{c.c.}$. The quadratic interaction of these first and second harmonics feeds back $8s^2|A|^2A/9$ into the critical [Fourier mode](fourier-analysis.md#fourier-mode), while the cubic gradient nonlinearity contributes $-3|A|^2A$. The [Fredholm solvability condition](analysis.md#fredholm-solvability-condition) is consequently $\mu_2A-g|A|^2A=0$. The sign of $g$ distinguishes supercritical and subcritical branches; $g=0$ requires a higher-order [amplitude equation](dynamical-systems.md#amplitude-equation).

#### Energy square completion for long-wave convection

↑ **Parent:** [Long-wave convection equation with broken Boussinesq symmetry](#long-wave-convection-equation-with-broken-boussinesq-symmetry)

For a real smooth solution of the [long-wave convection equation with broken Boussinesq symmetry](#long-wave-convection-equation-with-broken-boussinesq-symmetry), assume a periodic spatial average or an existing long-interval average with vanishing endpoint fluxes. [Integration by parts](calculus.md#integration-by-parts) gives the exact [energy method](numerical-analysis.md#energy-method) identity

$$
\frac12\partial_t\langle\Theta^2\rangle
=-\langle(\Theta+\Theta_{xx})^2\rangle
-\langle\Theta_x^2(\Theta_x-s/2)^2\rangle
+(\mu-2+s^2/4)\langle\Theta_x^2\rangle.
$$

Thus $\mu<\mu_E$ prevents growth of the mean-square temperature at arbitrary amplitude in this averaging class. This sufficient nonlinear bound need not equal the linear instability threshold, and it does not imply pointwise monotonicity of the temperature.

### Thermal convection

↑ **Parent:** [Convection](#convection)

Thermal convection is fluid motion driven by temperature-dependent [buoyancy](#buoyancy). It transports [heat](thermodynamics.md#heat) by bulk motion in addition to [thermal conduction](thermodynamics.md#thermal-conduction).

#### Horizontal convection

↑ **Parent:** [Thermal convection](#thermal-convection)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Horizontal_convection)

Horizontal convection is [buoyancy](#buoyancy)-driven circulation forced by lateral variations of [temperature](thermodynamics.md#temperature) along one horizontal boundary. Hot and cold surface regions drive a circulation even though all thermal forcing is applied at the same height. An insulated bottom and sides require zero net heat exchange through the remaining surface in steady state, but permit heat to enter its warmer region and leave its colder region.

##### Shallow horizontal convection with an insulated bottom

↑ **Parent:** [Horizontal convection](#horizontal-convection)

For downward depth $z=\epsilon y$, take $(u,w)=(\psi_z,-\psi_x)$, surface temperature $T=x$, a flat impermeable stress-free upper boundary and a no-slip insulated bottom. In the steady infinite-[Prandtl number](thermodynamics.md#prandtl-number) thin-layer interior, $\psi_{zzzz}=-\operatorname{Ra}$ with $\psi=\psi_{zz}=0$ at the surface and $\psi=\psi_z=0$ at the bottom. The displayed profile follows. Sidewall end layers close the circulation; the interior profile must not be imposed unchanged at those walls.

###### Advection correction in shallow horizontal convection

↑ **Parent:** [Shallow horizontal convection with an insulated bottom](#shallow-horizontal-convection-with-an-insulated-bottom)

The interior first temperature correction obeys $\Theta_{zz}=u=\psi_z$, $\Theta(0)=0$ and $\Theta_z(\epsilon)=0$. Hence $\Theta_z=\psi$, which integrates to the displayed polynomial. Its contribution to depth-integrated horizontal advective [heat flux](thermodynamics.md#heat-flux-density) is $\int u\Theta\,dz=-\int\psi^2dz=-19\operatorname{Ra}^2\epsilon^9/1451520$. The leading conductive flux is $-\epsilon$. These statements apply away from the sidewall end layers at fixed Rayleigh number as the layer becomes shallow.

#### Forced convection

↑ **Parent:** [Thermal convection](#thermal-convection)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Forced_convection)

Heat-carrying fluid motion dominated by an externally imposed flow or shear. Buoyancy may still influence it; forced and free contributions can coexist. In surface-layer scaling, $z\ll|\ell_O|$ is predominantly shear-driven, while $z\gg|\ell_O|$ is predominantly buoyancy-driven for lower-boundary heating.

#### Natural convection

↑ **Parent:** [Thermal convection](#thermal-convection)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Natural_convection)

Convection driven primarily by buoyancy generated by heating or cooling, rather than an externally imposed mean flow. In a constant-flux unstable surface layer, the local speed scales as $(B_0z)^{1/3}$.

##### Free-convection surface-layer scaling

↑ **Parent:** [Natural convection](#natural-convection)

For a positive approximately constant [vertical turbulent buoyancy flux](turbulence.md#vertical-turbulent-buoyancy-flux), dimensional turnover scaling gives $K_b\sim B_0^{1/3}z^{4/3}$ and $N^2\sim-B_0^{2/3}z^{-4/3}$. The negative squared frequency describes unstable overturning, not a real restoring oscillation. The leading dissipation is height-independent, unlike neutral wall turbulence.

#### Hexagonal convection amplitude equations

↑ **Parent:** [Thermal convection](#thermal-convection)

A finite-[wavenumber](wave-equation.md#wavenumber) convection instability with a [resonant three-wave triad](differential-equation.md#resonant-three-wave-triad) can yield three coupled [amplitude equations](dynamical-systems.md#amplitude-equation). For the gradient nonlinearity $\nabla\cdot(|\nabla\Theta|^2\nabla\Theta)$ and weak quadratic asymmetry $-\epsilon\gamma\nabla\cdot(\Theta\nabla\Theta)$, projection onto a triad of length squared $K$ gives the stated equation and its cyclic copies. The quadratic coefficient is $+\gamma K$, while both self and cross cubic coefficients are $-3K^2$ for angles of $120$ degrees. The finite critical mode requires positive linear damping in the underlying long-wave equation.

##### Rotational hexagon amplitude equations

↑ **Parent:** [Hexagonal convection amplitude equations](#hexagonal-convection-amplitude-equations)

For a [resonant three-wave triad](differential-equation.md#resonant-three-wave-triad) with rotational and translational [symmetry](physics.md#symmetry-physics) but no spatial [reflection](linear-algebra.md#reflection-mathematics), the cubic [amplitude equations](dynamical-systems.md#amplitude-equation) have the cyclic form $\dot A=\mu A+\overline B\,\overline C-\nu_1|A|^2A-(\nu_2+\delta)|B|^2A-(\nu_2-\delta)|C|^2A$. A half-turn induces [complex conjugation](complex-analysis.md#complex-conjugation), so all coefficients are real. The coefficient $\delta$ distinguishes the two cyclic cross-couplings that a [reflection](linear-algebra.md#reflection-mathematics) would interchange.

###### Roll and hexagon spectra without reflection symmetry

↑ **Parent:** [Rotational hexagon amplitude equations](#rotational-hexagon-amplitude-equations)

For the [rotational hexagon amplitude equations](#rotational-hexagon-amplitude-equations), put $d=\nu_2-\nu_1$ and $N=\nu_1+2\nu_2$. A roll with $r^2=\mu/\nu_1$ has transverse [eigenvalues](linear-operator-theory.md#eigenvalue) $-dr^2\pm\sqrt{\delta^2r^4+r^2}$, each twice, radial [eigenvalue](linear-operator-theory.md#eigenvalue) $-2\mu$, and one neutral translation. A hexagon with $\mu=Nh^2-h$ has real-amplitude [eigenvalues](linear-operator-theory.md#eigenvalue) $h-2Nh^2$ and $-2h+2dh^2\pm2i\sqrt3\delta h^2$; its imaginary-amplitude [eigenvalues](linear-operator-theory.md#eigenvalue) are $-3h,0,0$. These follow by diagonalizing the cyclic [Jacobian matrix](calculus.md#jacobian-matrix). Stability is understood modulo translations. If $\nu_2>\nu_1>0$ and $\delta\ne0$, the upper positive hexagon branch reaches a [Hopf bifurcation](dynamical-systems.md#hopf-bifurcation) at $h=1/d$, $\mu=(2\nu_1+\nu_2)/d^2$.

###### Axial isotropy of rolls and hexagons

↑ **Parent:** [Rotational hexagon amplitude equations](#rotational-hexagon-amplitude-equations)

Write the translation [group action](group-theory.md#group-action) as $(A,B,C)\mapsto(e^{i\theta_1}A,e^{i\theta_2}B,e^{-i(\theta_1+\theta_2)}C)$. Modulo lattice translations, the [stabilizer subgroup](group-theory.md#stabilizer-subgroup) of $(h,h,h)$, with nonzero real $h$, is the sixfold rotation group. Its [fixed-point subspace of a group action](representation-theory.md#fixed-point-subspace-of-a-group-action) is the real line $(a,a,a)$. The [stabilizer subgroup](group-theory.md#stabilizer-subgroup) of $(r,0,0)$, with nonzero real $r$, consists of the circle $\theta_1=0$ together with a half-turn; its [fixed-point subspace of a group action](representation-theory.md#fixed-point-subspace-of-a-group-action) is the real line $(a,0,0)$. The [equivariant branching lemma](dynamical-systems.md#equivariant-branching-lemma) therefore supplies generic branches of both axial types.

##### Roll instability from broken up-down symmetry

↑ **Parent:** [Hexagonal convection amplitude equations](#hexagonal-convection-amplitude-equations)

In the [hexagonal convection amplitude equations](#hexagonal-convection-amplitude-equations), a pure [convection roll](#convection-roll) has $|A|^2=\mu_2/(3K)$ and $B=C=0$. The transverse diagonal linear growth cancels because self and cross cubic coefficients coincide. Broken up-down symmetry leaves the off-diagonal coupling $\gamma K A$, giving eigenvalues $\pm|\gamma|K|A|$ and an unstable orientation perturbation whenever $\gamma\ne0$. With zero quadratic coupling these directions are neutral at the retained order, so that degenerate case cannot be declared strictly unstable by this calculation.

#### Convection roll

↑ **Parent:** [Thermal convection](#thermal-convection)

A [convection roll](#convection-roll) is a circulating cell pattern whose ideal [velocity](classical-mechanics.md#velocity) and [temperature](thermodynamics.md#temperature) fields are periodic across a chosen horizontal direction and independent of the coordinate along the [convection roll](#convection-roll) axis. In a two-dimensional [stream function](#stream-function) representation, its [velocity field](#velocity-field) is $(-\psi_z,0,\psi_x)$. [Rayleigh-Bénard convection](viscous-fluid-flow.md#rayleigh-benard-convection) can select stationary or oscillatory [convection rolls](#convection-roll); a two-dimensional [convection roll](#convection-roll) may be unstable to three-dimensional disturbances, a different [convection roll](#convection-roll) orientation, or slow amplitude and phase modulations. Existence of a saturated [Landau amplitude equation](dynamical-systems.md#landau-amplitude-equation) branch does not alone establish its stability.

#### Oscillatory convection

↑ **Parent:** [Thermal convection](#thermal-convection)

[oscillatory convection](#oscillatory-convection) is time-dependent convection emerging through nonzero-frequency [overstability](dynamical-systems.md#overstability) or a [Hopf bifurcation](dynamical-systems.md#hopf-bifurcation). At onset a complex-conjugate growth-rate pair crosses the imaginary axis. Travelling and standing [convection rolls](#convection-roll) are distinct nonlinear possibilities, and their stability cannot be decided from the linear [angular frequency](classical-mechanics.md#angular-frequency) alone.

##### Travelling and standing convection rolls

↑ **Parent:** [Oscillatory convection](#oscillatory-convection)

At fixed orientation, opposite travelling amplitudes can obey $\dot Z_\pm=(r+i\omega_0)Z_\pm-(g|Z_\pm|^2+h|Z_\mp|^2)Z_\pm$. For $r>0$ and $g_r=\operatorname{Re}g>0$, a travelling branch has one nonzero intensity $r/g_r$ and is stable to its counter-propagating amplitude when $h_r>g_r$. A standing branch has both intensities $r/(g_r+h_r)$ and is stable within the pair when $g_r>h_r$ and $g_r+h_r>0$. These follow by linearizing the real intensity equations. Spatial modulation and other orientations remain separate stability tests.

#### Stationary convection

↑ **Parent:** [Thermal convection](#thermal-convection)

[stationary convection](#stationary-convection) has a time-independent [velocity](classical-mechanics.md#velocity) and [temperature](thermodynamics.md#temperature) field, in the chosen fixed frame. Its onset from a conduction state corresponds to a real growth rate passing through zero. Stability of a resulting steady [convection roll](#convection-roll) is a separate nonlinear question.

#### Convective stability

↑ **Parent:** [Thermal convection](#thermal-convection)

A stable stratification gives a restoring [buoyancy](#buoyancy) force and positive squared [buoyancy frequency](gravity-wave.md#buoyancy-frequency) for an adiabatically displaced parcel. An adverse [specific entropy](thermodynamics.md#specific-entropy) gradient can instead drive [convection](#convection); other forces such as rotation can modify the full stability criterion.

#### Convective overshoot

↑ **Parent:** [Thermal convection](#thermal-convection)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Convective_overshoot)

Convective overshoot carries material from an unstable convecting region into an adjacent stably stratified region because its [momentum](classical-mechanics.md#momentum) does not vanish at the stability boundary. In stars this mixes material beyond the boundary determined by a local [stellar convective stability](stellar-structure.md#stellar-convective-stability) criterion, changing stellar core masses and nuclear lifetimes.

#### Double-diffusive convection

↑ **Parent:** [Thermal convection](#thermal-convection)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Double-diffusive_convection)

Double-diffusive convection occurs when two properties, such as [temperature](thermodynamics.md#temperature) and composition, affect [buoyancy](#buoyancy) but diffuse at different rates. A stabilizing composition gradient can oppose a destabilizing thermal gradient and change the form of heat transport.

##### Thermosolutal convection

↑ **Parent:** [Double-diffusive convection](#double-diffusive-convection)

[Thermosolutal convection](#thermosolutal-convection) is [double-diffusive convection](#double-diffusive-convection) driven by temperature and concentration gradients. Their buoyancy contributions can oppose one another, while unequal [thermal diffusivity](thermodynamics.md#thermal-diffusivity) and [solutal diffusivity](brownian-motion.md#solutal-diffusivity) allow steady, oscillatory and finite-amplitude states. For a layer heated from below with a stabilizing concentration gradient, thermal buoyancy is destabilizing and solutal buoyancy restoring.

###### Double-diffusive overflow reservoir

↑ **Parent:** [Thermosolutal convection](#thermosolutal-convection)

A steady well-mixed hot salty reservoir receives volume flux $Q$ and loses the same flux over a weir. Heat and salt balances are $Q(T_i-T)=AF_T$ and $Q(S_i-S)=AF_S$. If $\beta F_S/(\alpha F_T)=R_F$ and $\alpha F_T=b(\alpha\Delta T)^{4/3}/R_\rho^2$, define $R_0=\beta(S_i-S_\infty)/[\alpha(T_i-T_\infty)]$. Then $\eta_s=(R_F/R_0)\theta_s$ and $C=Ab[\alpha(T_i-T_\infty)]^{1/3}/(Q R_0^2)$. For $R_0>1$ and $0\leq R_F<1$ the interface is statically stable while preferential heat transfer can drive [double-diffusive convection](#double-diffusive-convection).

###### Post-shutdown double-diffusive reservoir cooling

↑ **Parent:** [Double-diffusive overflow reservoir](#double-diffusive-overflow-reservoir)

After inflow and overflow cease, a fixed-volume reservoir initially in the preceding steady state obeys $\eta=q\theta$ and $\dot\theta=k(1-\theta)^{10/3}/(1-q\theta)^2$, with $k=Ab[\alpha(T_i-T_\infty)]^{1/3}/(V R_0^2)$. Integrating gives $k(t-t_0)=G(\theta)-G(\theta_s)$, where $G=3(1-q)^2(1-\theta)^{-7/3}/7+3q(1-q)(1-\theta)^{-4/3}/2+3q^2(1-\theta)^{-1/3}$. For $q<1$, heat contrast tends to zero only at infinite time, while a nonzero salt contrast remains.

###### Lorenz model of thermosolutal convection

↑ **Parent:** [Thermosolutal convection](#thermosolutal-convection)

A five-mode [Galerkin method](partial-differential-equation.md#galerkin-method) model retains the roll velocity $a$, its correlated temperature and concentration modes $b,d$, and the mean-profile distortions $c,e$. Its parameters include the [Prandtl number](thermodynamics.md#prandtl-number) $\sigma$, diffusivity ratio $\tau$, thermal forcing $r$, stabilizing solutal forcing $r_s$, and a positive geometric decay ratio $\varpi$. The velocity equation is $\dot a=\sigma(-a+rb-r_sd)$, while the scalar equations are $\dot b=-b+a(1-c)$, $\dot c=\varpi(-c+ab)$, $\dot d=-\tau d+a(1-e)$ and $\dot e=\varpi(-\tau e+ad)$. The solutal forcing is normalized using the thermal diffusion scale, so its steady stabilizing effect is $r_s/\tau$.

###### Oscillatory threshold of a thermosolutal Lorenz model

↑ **Parent:** [Lorenz model of thermosolutal convection](#lorenz-model-of-thermosolutal-convection)

Linearization of the [Lorenz model of thermosolutal convection](#lorenz-model-of-thermosolutal-convection) at conduction yields $(\lambda+\sigma)(\lambda+1)(\lambda+\tau)-\sigma r(\lambda+\tau)+\sigma r_s(\lambda+1)=0$. A [Hopf bifurcation](dynamical-systems.md#hopf-bifurcation) requires the cubic coefficient identity $a_3=a_1a_2$ and positive frequency squared. Its threshold is the stated $r_H$, with $\omega^2=\sigma r_s(1-\tau)/(\sigma+1)-\tau^2>0$. If $r_s=\beta^2\tau$ and $\delta=\sigma/(1+\sigma)$, then $r_H=1+\tau/\delta+\beta^2\tau\delta+O(\tau^2)$. Comparing with the [steady fold of a thermosolutal Lorenz model](#steady-fold-of-a-thermosolutal-lorenz-model) gives a leading nonnegative difference $\tau(\beta\delta-1)^2/\delta$ for $\beta\ge0$.

###### Steady fold of a thermosolutal Lorenz model

↑ **Parent:** [Lorenz model of thermosolutal convection](#lorenz-model-of-thermosolutal-convection)

A nonzero steady [Lorenz model of thermosolutal convection](#lorenz-model-of-thermosolutal-convection) branch obeys $r(x)=(1+x)+r_s\tau(1+x)/(\tau^2+x)$, with $x=a^2$. For $0<\tau<1$, it has an interior [saddle-node bifurcation](dynamical-systems.md#saddle-node-bifurcation) precisely when $r_s>\tau^3/(1-\tau^2)$. Differentiating gives $x_*=-\tau^2+\sqrt{r_s\tau(1-\tau^2)}$ and the stated minimum. The weaker-versus-stronger threshold distinction matters: a sufficient bound need not be the sharp subcriticality condition. Steady-branch existence alone does not decide oscillatory stability.

##### Layered convection

↑ **Parent:** [Double-diffusive convection](#double-diffusive-convection)

Layered convection consists of mixed convecting layers separated by more weakly transporting interfaces. In a giant planet, composition gradients can support such interfaces and reduce heat loss, contributing to [delayed cooling of an inflated giant planet](exoplanet.md#delayed-cooling-of-an-inflated-giant-planet).

## Buoyancy

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Buoyancy)

Buoyancy is the net force on a body or fluid parcel produced by a pressure gradient in a gravitational or accelerating fluid. Density differences make displaced parcels rise or sink relative to their surroundings.

### Buoyancy gradient

↑ **Parent:** [Buoyancy](#buoyancy)

The spatial [gradient](calculus.md#gradient) of [buoyancy](#buoyancy) determines the buoyancy anomaly produced by a small parcel [displacement](classical-mechanics.md#displacement): $b'=-\boldsymbol\xi\cdot\nabla\bar b$. Its vertical component is the squared [buoyancy frequency](gravity-wave.md#buoyancy-frequency) in a stably stratified [Boussinesq approximation](geophysical-fluid-dynamics.md#boussinesq-approximation). A horizontal component enters [thermal wind](geophysical-fluid-dynamics.md#thermal-wind) and the propagation of a [Boundary Rossby wave](hydrodynamic-stability.md#boundary-rossby-wave).

### Magnetic buoyancy

↑ **Parent:** [Buoyancy](#buoyancy)

[Magnetic buoyancy](#magnetic-buoyancy) is the tendency of magnetized fluid to rise when [magnetic pressure](astrophysical-fluid-dynamics.md#magnetic-pressure) support reduces its density relative to its surroundings. For a thin flux concentration in lateral balance, $p_{\rm in}+B^2/(2\mu_0)=p_{\rm out}$. At equal [temperature](thermodynamics.md#temperature) and composition an ideal-gas equation of state then gives $\rho_{\rm in}<\rho_{\rm out}$, producing an upward buoyant force. Thermal exchange, [magnetic tension](astrophysical-fluid-dynamics.md#magnetic-tension) and stable stratification modify this simple argument. In a [solar dynamo](stellar-astrophysics.md#solar-dynamo), buoyant toroidal flux can emerge as tilted bipolar active regions.

### Archimedes' principle

↑ **Parent:** [Buoyancy](#buoyancy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Archimedes'_principle)

A body immersed in a fluid experiences an upward [buoyancy](#buoyancy) force equal to the weight of the fluid it displaces. In a uniform fluid of [mass density](#density) $\rho_f$, displaced volume $V$ gives $F_b=\rho_fgV$. A freely floating body displaces a fluid mass equal to its own mass.

### Submerged weight

↑ **Parent:** [Buoyancy](#buoyancy)

For a grain of [mass density](#density) $\rho_p$ and volume $\mathcal V$ in a fluid of [mass density](#density) $\rho_f$, its effective downward [force](classical-mechanics.md#force) is $(\rho_p-\rho_f)g\mathcal V$, after subtracting [buoyancy](#buoyancy) from weight.

### Buoyancy perturbation

↑ **Parent:** [Buoyancy](#buoyancy)

A buoyancy perturbation is the departure $b'$ from a prescribed basic buoyancy field. In a fluid with constant [buoyancy frequency](gravity-wave.md#buoyancy-frequency) $N$, vertical velocity $w'$ changes it according to $(\partial_t+\mathbf U\cdot\nabla)b'=-N^2w'$.

#### Buoyancy displacement variable

↑ **Parent:** [Buoyancy perturbation](#buoyancy-perturbation)

In a radially stratified [shearing sheet](gravitational-instability-of-an-astrophysical-disk.md#shearing-sheet), one can normalize the scalar [buoyancy perturbation](#buoyancy-perturbation) by writing $b_x=-N^2\theta$ and $D_t\theta=u_x+\xi\nabla^2\theta$. With this convention $\theta$ has dimensions of length, rather than [temperature](thermodynamics.md#temperature); $\xi$ is [thermal diffusivity](thermodynamics.md#thermal-diffusivity).

### Isopycnal

↑ **Parent:** [Buoyancy](#buoyancy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Isopycnal)

An isopycnal is a surface of constant [mass density](#density). In a [Boussinesq approximation](geophysical-fluid-dynamics.md#boussinesq-approximation), it is equivalently a surface of constant buoyancy.

## Hydrodynamic stability

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](hydrodynamic-stability.md)

## Barotropic fluid

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Barotropic_fluid)

A barotropic fluid has pressure determined by density alone, $P=P(\rho)$, so pressure and density surfaces coincide in hydrostatic equilibrium.

### Barotropic cylindrical rotation theorem

↑ **Parent:** [Barotropic fluid](#barotropic-fluid)

In a steady axisymmetric [barotropic fluid](#barotropic-fluid) with purely azimuthal velocity $r\Omega\mathbf e_\phi$ and a conservative body force, the [barotropic enthalpy function](#barotropic-enthalpy-function) obeys $\nabla(w+\Phi)=r\Omega^2\mathbf e_r$. Taking its curl yields the displayed cylindrical rotation law. The first integral is $w+\Phi-\int r\Omega^2dr=C$ in a connected fluid region. Baroclinic pressure and density need not satisfy this conclusion.

### Barotropic spherical accretion equation

↑ **Parent:** [Barotropic fluid](#barotropic-fluid)

Steady spherical [continuity equation](physics.md#continuity-equation) gives $r^2\rho u=\text{constant}$. Combining this with [Euler equations for an inviscid fluid](#euler-equations-for-an-inviscid-fluid) and $c_s^2=dp/d\rho$ gives the displayed equation. Smooth transonic passage requires $u^2=c_s^2$ and $\Phi^{\prime}=2c_s^2/r$ simultaneously. The [barotropic enthalpy function](#barotropic-enthalpy-function) gives the integral $u^2/2+h+\Phi=\text{constant}$.

#### Polytropic accretion in a mixed inverse-power potential

↑ **Parent:** [Barotropic spherical accretion equation](#barotropic-spherical-accretion-equation)

For $p=K\rho^{1+1/m}$, the [barotropic enthalpy function](#barotropic-enthalpy-function) is $mc_s^2$. In $\Phi=-\lambda/R^2-\mu/R$, a regular [sonic point](compressible-flow.md#sonic-point) obeys $c_{s,s}^2=\lambda/R_s^2+\mu/(2R_s)$, and its Bernoulli integral yields the displayed quadratic. For $K,\lambda,\mu>0$ and the usual positive polytropic index, its unique positive root exists precisely when $m>1/2$. The [mass accretion rate](astrophysics.md#mass-accretion-rate) is $4\pi R_s^2\rho_\infty c_{s,s}(c_{s,s}^2/c_\infty^2)^m$. If indices with $0<1+1/m<1$ are admitted, $m<-1$ also permits a positive sonic root; negative compressibility indices do not.

#### Critical-point slope of barotropic spherical accretion

↑ **Parent:** [Barotropic spherical accretion equation](#barotropic-spherical-accretion-equation)

At a regular [sonic point](compressible-flow.md#sonic-point), differentiating the vanishing coefficient and numerator yields $(2+C/c_s^2)(u^{\prime})^2+4Cu^{\prime}/(ru)+(4C+2c_s^2)/r^2+\Phi^{\prime\prime}=0$. A real slope compatible with the desired branch is needed in addition to the sonic equalities. For constant [sound speed](compressible-flow.md#speed-of-sound) this reduces to $(u^{\prime})^2=-c_s^2/r^2-\Phi^{\prime\prime}/2$.

### Barotropic enthalpy function

↑ **Parent:** [Barotropic fluid](#barotropic-fluid)

This [barotropic pressure potential](#barotropic-enthalpy-function) obeys $\nabla h=\nabla p/\rho$ for a [barotropic fluid](#barotropic-fluid). It gives the [pressure](thermodynamics.md#pressure) contribution to a steady [Bernoulli equation](#bernoulli-equation). In isentropic thermodynamics it agrees with [specific enthalpy](thermodynamics.md#specific-enthalpy) up to a constant; for an externally maintained isothermal ideal gas it is $c_s^2\log\rho$ and is not the constant thermodynamic enthalpy at fixed temperature.

### Centrifugal potential of cylindrical rotation

↑ **Parent:** [Barotropic fluid](#barotropic-fluid)

For [angular velocity](classical-mechanics.md#angular-velocity) depending only on cylindrical radius, the centrifugal acceleration is a [gradient](calculus.md#gradient). Steady barotropic balance is $\nabla p/\rho=-\nabla\Psi$, hence [specific enthalpy](thermodynamics.md#specific-enthalpy) satisfies $h(\rho)+\Psi=\text{constant}$. On an invertible equation-of-state branch, [mass density](#density) and [pressure](thermodynamics.md#pressure) are functions of $\Psi$. Cylindrical rotation is essential to this scalar centrifugal-potential representation.

### Barotropic energy density

↑ **Parent:** [Barotropic fluid](#barotropic-fluid)

For a [barotropic fluid](#barotropic-fluid) with [pressure](thermodynamics.md#pressure) $P=P(\rho)$, choose an energy density $U$ satisfying $\rho U'(\rho)-U=P$. The [continuity equation](physics.md#continuity-equation) then gives $\partial_tU+\nabla\cdot(U\mathbf u)=-P\nabla\cdot\mathbf u$. For an [isothermal equation of state](compressible-flow.md#globally-isothermal-equation-of-state) $P=c_s^2\rho$, one choice is $U=c_s^2\rho\ln(\rho/\rho_{\rm ref})$. A fixed reference density changes $U$ only by a conserved mass term. The same construction holds with [surface density](astrophysics.md#surface-density-of-a-disk) and vertically integrated [pressure](thermodynamics.md#pressure). This closure energy need not equal the microscopic internal energy of a gas maintained at fixed [temperature](thermodynamics.md#temperature).

### Barotropic magnetic energy equation

↑ **Parent:** [Barotropic fluid](#barotropic-fluid)

For a [barotropic fluid](#barotropic-fluid), an energy per mass $e$ can be defined by $de/d\rho=p/\rho^2$. For the [isothermal equation of state](compressible-flow.md#globally-isothermal-equation-of-state), $e=c_s^2\ln(\rho/\rho_0)$. Adding kinetic, gravitational and [magnetic energy](electromagnetism.md#magnetic-energy) gives the ideal magnetic energy flux $\mathbf u(E+p+B^2/(2\mu_0))-\mathbf B(\mathbf u\cdot\mathbf B)/\mu_0$. This is a mechanical barotropic energy identity; it does not say that an isothermal gas is thermally isolated.

### Barotropic vorticity transport

↑ **Parent:** [Barotropic fluid](#barotropic-fluid)

For an inviscid [barotropic fluid](#barotropic-fluid) with only potential body forces, the [vorticity](#vorticity) $\boldsymbol\omega=\nabla\times\mathbf u$ obeys

$$
\partial_t\boldsymbol\omega=\nabla\times(\mathbf u\times\boldsymbol\omega).
$$

The pressure force is a [gradient](calculus.md#gradient) because $\rho^{-1}\nabla p=\nabla\int^\rho p'(s)\,ds/s$. A spatially uniform [specific entropy](thermodynamics.md#specific-entropy) makes a fixed-composition fluid barotropic. Merely having $Ds/Dt=0$ does not exclude [baroclinic vorticity generation](physics.md#baroclinic-vorticity-generation) from spatial entropy gradients.

## Shear flow

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A shear flow has a [velocity field](#velocity-field) varying across adjacent fluid layers, giving a nonzero [shear rate](viscous-fluid-flow.md#shear-rate). A parallel example is $\mathbf u=U(z)\mathbf e_x$, with vertical shear $U'$. [Linear shear flow](#linear-shear-flow) has constant shear, while a [shear layer](#shear-layer) concentrates the velocity change in a narrow region.

### Renovating shear flow

↑ **Parent:** [Shear flow](#shear-flow)

A renovating shear flow holds a planar [shear flow](#shear-flow) fixed for an interval $T$, then chooses a fresh orientation independently of preceding intervals. Each interval acts on a [material line](#material-curve) by a rotated copy of the displayed [deformation gradient](continuum-mechanics.md#deformation-gradient). The orientation law must be specified: independent uniformly distributed orientations define the isotropic model, whereas a biased orientation law generally gives another [Lyapunov exponent](dynamical-systems.md#lyapunov-exponent).

#### Mean logarithmic stretching in an isotropic renovating shear

↑ **Parent:** [Renovating shear flow](#renovating-shear-flow)

For independent uniform orientations in a [renovating shear flow](#renovating-shear-flow), the incident angle relative to each new shear is uniform even after earlier deformations. One interval stretches a unit [material line](#material-curve) by $\ell(\theta)^2=1+a\sin2\theta+a^2\sin^2\theta$. Write this as $A+B\cos(2\theta-\delta)$, where $A=1+a^2/2$ and $A^2-B^2=1$. The angular logarithmic integral gives $\langle\log\ell\rangle=\tfrac12\log[(A+1)/2]$. Add these independent logarithmic increments to get the displayed rate. At fixed shear rate, small $T$ gives $\mu\sim\Lambda^2T/8$ and large $T$ gives $\mu\sim\log(|\Lambda|T/2)/T$. The unique positive maximum is at $|\Lambda|T\approx3.9605826$, obtained from $\log z=2(1-z^{-1})$ with $z=1+a^2/4$.

##### Log-stretch fluctuations in an isotropic renovating shear

↑ **Parent:** [Mean logarithmic stretching in an isotropic renovating shear](#mean-logarithmic-stretching-in-an-isotropic-renovating-shear)

The logarithm of the stretch after $N$ independent uniform renovations is a sum of independent identically distributed bounded increments. For singular stretching $e^\gamma$, $\gamma=\operatorname{arsinh}(|a|/2)$, the increment has Fourier expansion $r+\sum_{n\geq1}(-1)^{n+1}q^n\cos(2n\theta)/n$, with $q=\tanh\gamma$ and $r=\tfrac12\log(1+a^2/4)$. Orthogonality proves the displayed variance. The [central limit theorem](convergence-of-random-variables.md#central-limit-theorem) gives an approximate central [log-normal distribution](probability-theory.md#log-normal-distribution) of $\lambda_N$, not an exact description of extreme tails. For $|a|\ll1$, both the mean and variance of $\log\lambda_N$ are $Na^2/8$ to leading order. Direct expansion of fixed-power moments gives $\langle\lambda_N^p\rangle=\exp[Np(p+2)a^2/16+O(Na^4)]$; in particular mean stretch grows faster than typical stretch.

### Linear shear flow

↑ **Parent:** [Shear flow](#shear-flow)

A linear shear flow has velocity that varies linearly in a transverse coordinate, such as $\mathbf u=-Sx\mathbf e_y$. Its velocity gradient and shear rate are spatially constant.

## Lagrangian displacement (fluid mechanics)

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A Lagrangian displacement maps each equilibrium fluid element to its perturbed position. Its time derivative is the velocity perturbation when the equilibrium is static.

### Eulerian perturbation of a fluid variable

↑ **Parent:** [Lagrangian displacement (fluid mechanics)](#lagrangian-displacement-fluid-mechanics)

The Eulerian perturbation compares field values at the same spatial location, rather than following a fluid element. To first order it satisfies $\delta q=\Delta q-\xi\cdot\nabla q$. Thus a field advected unchanged by individual elements can still have a nonzero Eulerian perturbation in an inhomogeneous background.

### Lagrangian perturbation of a fluid variable

↑ **Parent:** [Lagrangian displacement (fluid mechanics)](#lagrangian-displacement-fluid-mechanics)

The Lagrangian perturbation compares a variable on the same moving fluid element before and after a displacement. Taylor expansion of the background value at the displaced position gives the displayed relation to an Eulerian perturbation. For an adiabatic [ideal gas](thermodynamics.md#ideal-gas), $\Delta(p/\rho^\gamma)=0$ even when the equilibrium [entropy](thermodynamics.md#entropy) varies spatially.

#### Adiabatic fluid perturbation

↑ **Parent:** [Lagrangian perturbation of a fluid variable](#lagrangian-perturbation-of-a-fluid-variable)

An adiabatic fluid perturbation preserves the [specific entropy](thermodynamics.md#specific-entropy) of each displaced parcel. For a [perfect gas](thermodynamics.md#ideal-gas), [mass conservation](continuum-mechanics.md#mass-conservation) gives $\Delta\rho=-\rho\nabla\cdot\boldsymbol\xi$ and the [adiabatic equation of state](thermodynamics.md#adiabatic-equation-of-state) gives $\Delta p=\gamma p\Delta\rho/\rho$. The corresponding [Eulerian perturbation of a fluid variable](#eulerian-perturbation-of-a-fluid-variable) is $\delta p=-\gamma p\nabla\cdot\boldsymbol\xi-\boldsymbol\xi\cdot\nabla p$. An isothermal equilibrium may still have adiabatic perturbations, because the thermodynamic constraint on displaced parcels differs from the equilibrium temperature profile.

## Eulerian and Lagrangian fluid perturbations

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

For a background scalar field $f$ and fluid displacement $\boldsymbol\xi$, the Lagrangian perturbation follows the displaced fluid element while the Eulerian perturbation compares fields at one fixed position. To first order,

$$
\Delta_L f=\delta f+\boldsymbol\xi\mathbin\cdot\nabla f.
$$

### Eulerian fluid perturbation

↑ **Parent:** [Eulerian and Lagrangian fluid perturbations](#eulerian-and-lagrangian-fluid-perturbations)

An Eulerian fluid perturbation compares a perturbed field with its equilibrium value at one fixed spatial point. It differs from the perturbation following a displaced material element: $\Delta f=f_1+\boldsymbol\xi\cdot\nabla f$. Linearizing a static fluid velocity gives $\mathbf v_1=\partial_t\boldsymbol\xi$.

### Surface density perturbation of a displaced uniform interface

↑ **Parent:** [Eulerian and Lagrangian fluid perturbations](#eulerian-and-lagrangian-fluid-perturbations)

Moving a uniform-density boundary produces a delta-function sheet in the Eulerian [mass density](#density) perturbation. For a slab displaced vertically by $\eta_\pm$, $\rho^{\prime}=\rho_0\eta_+\delta(z-H)-\rho_0\eta_-\delta(z+H)$. [Poisson equation](partial-differential-equation.md#poisson-equation) then gives a continuous gravitational potential with derivative jumps fixed by those sheets.

### Lagrangian pressure perturbation

↑ **Parent:** [Eulerian and Lagrangian fluid perturbations](#eulerian-and-lagrangian-fluid-perturbations)

The [Lagrangian pressure perturbation](#lagrangian-pressure-perturbation) is the change in [pressure](thermodynamics.md#pressure) experienced by a displaced [fluid element](continuum-mechanics.md#fluid-element): $\Delta p=\delta p+\boldsymbol\xi\cdot\nabla p_0$. For a free surface against fixed external [pressure](thermodynamics.md#pressure), $\Delta p=0$, rather than $\delta p=0$ at the original surface.

<h2 id="torricelli-s-law">Torricelli's law</h2>

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Torricelli's_law)

An ideal fluid issuing from a small hole a vertical depth $h$ below a free surface has speed

$$
v=\sqrt{2gh}.
$$

### Drainage time of a conical tank

↑ **Parent:** [Torricelli's law](#torricelli-s-law)

For a cone of half angle $\pi/4$ draining through a small circular aperture of radius $\epsilon$, the horizontal area at height $h$ is $\pi h^2$. [Torricelli's law](#torricelli-s-law) gives speed $\sqrt{2gh}$, so [conservation of mass](continuum-mechanics.md#mass-conservation) gives $h^2\dot h=-\epsilon^2\sqrt{2gh}$. Integration yields the displayed leading drainage time when $h_0\gg\epsilon$. The final layer $h=O(\epsilon)$ is outside the quasi-steady approximation and contributes only order $\sqrt{\epsilon/g}$, compared with the leading time of order $h_0^{5/2}/(\epsilon^2\sqrt g)$. This is an ideal inviscid estimate without a discharge coefficient.

## Density

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Density)

Mass density is mass per unit volume.

### Gas clumping factor

↑ **Parent:** [Density](#density)

The [gas clumping factor](#gas-clumping-factor) measures unresolved inhomogeneity in electron [number density](statistical-physics.md#number-density) within a chosen averaging region. Nonnegative [variance](variance.md) gives $C_e\ge1$. At a uniform [temperature](thermodynamics.md#temperature), [thermal bremsstrahlung](astrophysics.md#thermal-bremsstrahlung) scales with $\langle n_e^2\rangle$, whereas the [thermal Sunyaev-Zeldovich effect](cosmology.md#thermal-sunyaev-zeldovich-effect) scales with $\langle n_e\rangle$. A homogeneous [cluster distance from Sunyaev-Zeldovich and X-ray signals](cosmology.md#cluster-distance-from-sunyaev-zeldovich-and-x-ray-signals) inference then gives $d_{A,\mathrm{inferred}}=d_{A,\mathrm{true}}/C_e$, for the same geometry and temperature. Correlated temperature variations require additional weighted averages.

### Projected surface mass density

↑ **Parent:** [Density](#density)

Projected surface mass density is mass per unit projected area, obtained by integrating [mass density](#density) along the line of sight. It determines the enclosed cylindrical mass used by a [thin gravitational lens equation](general-relativity.md#thin-gravitational-lens-equation). It need not equal a physical disk's density, and its aperture mass differs from a spherical three-dimensional enclosed mass.

## Fluid pressure

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

Fluid pressure is the isotropic normal compressive stress in a fluid at rest.

### Cavitation

↑ **Parent:** [Fluid pressure](#fluid-pressure)

Cavitation is the formation of gas or vapour cavities when a liquid's [pressure](thermodynamics.md#pressure) becomes sufficiently low. A [journal bearing](viscous-fluid-flow.md#journal-bearing) model with [cavitation](#cavitation) must specify how a partly filled film and its boundaries behave, so periodic [pressure](thermodynamics.md#pressure) alone cannot determine the flow there.

### Pressure gradient

↑ **Parent:** [Fluid pressure](#fluid-pressure)

The pressure gradient is the vector $\nabla p$ pointing in the direction of fastest pressure increase. The force density exerted by pressure on a continuum is $-\nabla p$.

## Drag (physics)

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Drag_(physics))

A drag force opposes an object's motion relative to a surrounding fluid and transfers momentum between them.

### Linear drag

↑ **Parent:** [Drag (physics)](#drag-physics)

Linear drag opposes the [velocity](classical-mechanics.md#velocity) relative to the surrounding medium with magnitude proportional to its [speed](classical-mechanics.md#speed), where $\alpha>0$. Its [power](classical-mechanics.md#power) is $\mathbf F_d\cdot\mathbf v=-\alpha|\mathbf v|^2$, so it dissipates [kinetic energy](classical-mechanics.md#kinetic-energy). Under a constant external [force](classical-mechanics.md#force), the resulting [linear ordinary differential equation](differential-equation.md#linear-ordinary-differential-equation) relaxes exponentially on the [time](classical-mechanics.md#time-in-physics) scale $m/\alpha$.

#### Overdamped particle dynamics

↑ **Parent:** [Linear drag](#linear-drag)

When momentum relaxes much faster than the imposed motion, [force](classical-mechanics.md#force) balance replaces the inertial equation: $\zeta\dot x=F(x,t)$ in a deterministic one-dimensional model. The [linear friction coefficient](#linear-friction-coefficient) sets the time scale. Thermal forcing, if included, gives [overdamped Langevin dynamics](stochastic-calculus.md#overdamped-langevin-dynamics).

#### Linear friction coefficient

↑ **Parent:** [Linear drag](#linear-drag)

The dimensional linear friction coefficient relates [drag force](#drag-physics) and [velocity](classical-mechanics.md#velocity), $F_d=-\zeta v$, and has units of [force](classical-mechanics.md#force) divided by speed. It differs from the dimensionless aerodynamic [drag coefficient](#drag-coefficient). For an isolated sphere in [Stokes flow](stokes-flow.md), the [Stokes drag law](stokes-flow.md#stokes-s-law) gives $\zeta=6\pi\eta a$.

#### Vertical ascent under linear drag

↑ **Parent:** [Linear drag](#linear-drag)

For constant downward gravitational [acceleration](classical-mechanics.md#acceleration) $g$ and [linear drag](#linear-drag) $-\alpha v$, the upward [velocity](classical-mechanics.md#velocity) solves $m\dot v=-mg-\alpha v$ with $v(0)=u_0\ge0$. Its first zero occurs at the displayed [time](classical-mechanics.md#time-in-physics). The dimensionless control variable is $\alpha u_0/(mg)$, and the limit $\alpha\to0$ gives $u_0/g$.

### Drag coefficient

↑ **Parent:** [Drag (physics)](#drag-physics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Drag_coefficient)

### Quadratic drag

↑ **Parent:** [Drag (physics)](#drag-physics)

Quadratic drag has magnitude proportional to the square of the relative speed and points opposite to the relative velocity.

#### Descent from rest under quadratic drag

↑ **Parent:** [Quadratic drag](#quadratic-drag)

For positive downward speed, gravity and [quadratic drag](#quadratic-drag) give $m\dot v=mg-\alpha v^2$, $v(0)=0$. Separation and the integral of $(1-s^2)^{-1}$ give the displayed approach to [terminal velocity](classical-mechanics.md#terminal-velocity). The fallen distance is $(m/\alpha)\log\cosh(\sqrt{\alpha g/m}\,t)$. The limit as $\alpha\to0$ recovers $v=gt$ and distance $gt^2/2$.

#### Quadratic-drag turning angle

↑ **Parent:** [Quadratic drag](#quadratic-drag)

For an ice mass in still water, approximate the wind stress by a fixed vector $a\mathbf e_x$ while retaining [quadratic drag](#quadratic-drag) in the water. With mass per water-drag area $\mu=m/A_w$, water coefficient $b=\rho_wC_w$ and $f=2\Omega\sin\phi$, the steady balance is $a\mathbf e_x=bU\mathbf u+\mu f\widehat{\mathbf z}\times\mathbf u$. Resolving along the drift and perpendicular to it gives $a\cos\theta=bU^2$, $a\sin\theta=\mu|f|U$. Thus $b^2U^4+(\mu f)^2U^2=a^2$ and $\tan\theta=\mu|f|/(bU)$. The direction is right of the wind in the northern hemisphere and left in the southern hemisphere. This angle neglects intrinsic boundary-layer turning, ocean currents and contact forces; it is not a universal observed sea-ice turning angle.

##### Mass per drag area

↑ **Parent:** [Quadratic-drag turning angle](#quadratic-drag-turning-angle)

The normalization $\mu=m/A_w$ has units $\mathrm{kg\,m^{-2}}$. It converts the [Coriolis force](physics.md#coriolis-force) into a force per water-drag area and allows comparison with wind and water stresses. [Icebergs](geophysics.md#iceberg) generally have much larger $\mu$ than thin [ice floes](geophysics.md#ice-floe), but their effective air-to-water drag-area ratio also matters. A geometric depth becomes a mass per area only after multiplication by density.

#### Quadratic damping

↑ **Parent:** [Quadratic drag](#quadratic-drag)

A resistive velocity term proportional to the speed squared removes energy at rate proportional to $|\omega|^3$. Its derivative at zero velocity vanishes, so it does not appear in the [linearization of a dynamical system](algebra.md#linearization-of-a-dynamical-system) at rest. Nonlinear energy arguments can still prove [asymptotic stability](dynamical-systems.md#asymptotic-stability).

### Pressure drag

↑ **Parent:** [Drag (physics)](#drag-physics)

Pressure drag is the component of force produced by integrating pressure over a body's surface. For flow over topography $z=h(x)$, the horizontal force on the fluid is $-\overline{p h_x}$ to leading order.

### Stokes number

↑ **Parent:** [Drag (physics)](#drag-physics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stokes_number)

The Stokes number compares a particle's drag stopping time $\tau$ with a characteristic flow time $T$: $\operatorname{St}=\tau/T$. In an orbiting disk, the natural choice is $\operatorname{St}=\tau\Omega$.

### Gas drag

↑ **Parent:** [Drag (physics)](#drag-physics)

Gas drag is a [drag force](#drag-physics) on a solid body due to its motion relative to surrounding gas. With [aerodynamic stopping time](#aerodynamic-stopping-time) $t_s$, the linear approximation gives $\dot{\mathbf v}|_{\rm drag}=-(\mathbf v-\mathbf v_g)/t_s$.

### Aerodynamic stopping time

↑ **Parent:** [Drag (physics)](#drag-physics)

The aerodynamic stopping time is the characteristic time on which [drag force](#drag-physics) damps a solid particle's velocity relative to the surrounding fluid. Linear drag gives relative acceleration $-\mathbf v_{\rm rel}/\tau$.

## Suspension (chemistry)

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Suspension_(chemistry))

A particle suspension is a dispersed population of solid particles carried by a fluid. Its dynamics couple particle transport, [drag force](#drag-physics), gravity, and the compensating motion of the carrier fluid.

### Density inversion in a settling suspension

↑ **Parent:** [Suspension (chemistry)](#suspension-chemistry)

More suspended heavy particles above fewer particles puts denser fluid above lighter fluid. Such a [particle suspension](#suspension-chemistry) may develop [Rayleigh-Taylor instability](continuum-mechanics.md#rayleigh-taylor-instability) and overturning in addition to one-dimensional [kinematic sedimentation](#kinematic-sedimentation). A rarefaction solution alone does not establish hydrodynamic stability.

### Heated particle-laden layer

↑ **Parent:** [Suspension (chemistry)](#suspension-chemistry)

A dilute [particle suspension](#suspension-chemistry) can supply both excess [mass density](#density) and heat. To first order its [equation of state](thermodynamics.md#equation-of-state) is $\rho/\rho_0=1+\gamma\phi-\theta$, where $\phi$ is the [particle volume fraction](#particle-volume-fraction) and $\theta$ is fractional [thermal expansion](thermodynamics.md#thermal-expansion). [Particle deposition flux](#particle-deposition-flux) reduces $\phi$, while particle heating increases $\theta$. The competition can reverse the [reduced gravity](reduced-gravity.md) and create [unstable density stratification](gravity-wave.md#unstable-density-stratification).

### Particle volume fraction

↑ **Parent:** [Suspension (chemistry)](#suspension-chemistry)

The particle volume fraction is the fraction of a representative mixture volume occupied by particles. Several particle species have fractions $\phi_i$, while the carrier-fluid fraction is $1-\sum_i\phi_i$.

### Bidisperse particle suspension

↑ **Parent:** [Suspension (chemistry)](#suspension-chemistry)

A bidisperse particle suspension contains two distinguishable particle populations, commonly with different sizes, densities, or [settling velocities](#settling-velocity).

#### Composition wave in a bidisperse suspension

↑ **Parent:** [Bidisperse particle suspension](#bidisperse-particle-suspension)

When two species share the same local settling velocity, their total [particle volume fraction](#particle-volume-fraction) supports a nonlinear [kinematic wave](partial-differential-equation.md#kinematic-wave), while their relative composition is transported as a contact-like wave at the common particle speed.

### Settling velocity

↑ **Parent:** [Suspension (chemistry)](#suspension-chemistry)

The settling velocity is a particle's vertical velocity relative to a stated frame. With height increasing upward, a sedimenting particle has $W<0$.

#### Settling-velocity radius scaling

↑ **Parent:** [Settling velocity](#settling-velocity)

For spheres with the same density contrast, balance submerged weight, proportional to $r^3$, against [Stokes drag law](stokes-flow.md#stokes-s-law), proportional to $rW_s$, to obtain $W_s\propto r^2$. With constant [drag coefficient](#drag-coefficient), [quadratic drag](#quadratic-drag) is proportional to $r^2W_s^2$, giving $W_s\propto r^{1/2}$. The two radius laws require their corresponding [particle Reynolds number](#particle-reynolds-number) limits.

#### Particle Reynolds number

↑ **Parent:** [Settling velocity](#settling-velocity)

A [Reynolds number](#reynolds-number) based on particle diameter and relative speed in the carrier fluid. Small values justify [Stokes drag law](stokes-flow.md#stokes-s-law); a high-Reynolds-number regime with nearly constant [drag coefficient](#drag-coefficient) instead gives [quadratic drag](#quadratic-drag). The drag law must be evaluated in the appropriate regime for every species.

#### Particle deposition flux

↑ **Parent:** [Settling velocity](#settling-velocity)

For downward [settling velocity](#settling-velocity) magnitude $W_s$ and near-bed [particle volume fraction](#particle-volume-fraction) $\phi_b$, a horizontal absorbing bed receives particle volume per area per time $J_s=W_s\phi_b$. A bed inclined at angle $\vartheta$ to the horizontal receives $W_s\phi_b\cos\vartheta$ per unit actual area, in the absence of resuspension or additional normal fluid motion.

#### Stokes settling velocity

↑ **Parent:** [Settling velocity](#settling-velocity)

The Stokes settling velocity is the terminal relative velocity obtained by balancing gravity, buoyancy, and the [Stokes drag law](stokes-flow.md#stokes-s-law) for a dilute isolated sphere.

#### Hindered settling

↑ **Parent:** [Settling velocity](#settling-velocity)

Hindered settling is the reduction or modification of particle settling by the displaced carrier-fluid backflow and by interactions with other particles. A simple dilute mixture model gives every species the same volume-averaged backflow.

##### Kinematic sedimentation

↑ **Parent:** [Hindered settling](#hindered-settling)

A one-dimensional [particle suspension](#suspension-chemistry) settling without particle diffusion or overturning obeys the [scalar conservation law](partial-differential-equation.md#scalar-conservation-law) $\phi_t+\partial_zj(\phi)=0$. The upward flux is negative for downward settling. [Characteristic curves](partial-differential-equation.md#characteristic-curve), compressive [shocks](partial-differential-equation.md#shock-wave) and [rarefaction waves](partial-differential-equation.md#rarefaction-wave) describe concentration transport rather than individual particle paths.

###### Hindered-settling flux inflection

↑ **Parent:** [Kinematic sedimentation](#kinematic-sedimentation)

For [hindered settling](#hindered-settling) with normalized [particle volume fraction](#particle-volume-fraction) $s$, upward coordinate and downward isolated [settling velocity](#settling-velocity) magnitude $V_0$, the [scalar conservation law](partial-differential-equation.md#scalar-conservation-law) has [conservation law flux](partial-differential-equation.md#conservation-law-flux) $f(s)=-V_0s(1-s)^\alpha$. For $\alpha>0$, its [convexity](real-analysis.md#convex-function) changes at $s=2/(\alpha+1)$ when this lies in the physical interval. This change distinguishes spreading [rarefaction waves](partial-differential-equation.md#rarefaction-wave) from compressing [characteristic curves](partial-differential-equation.md#characteristic-curve); a flux with an inflection can produce both a [shock wave](partial-differential-equation.md#shock-wave) and a [rarefaction wave](partial-differential-equation.md#rarefaction-wave) in one transition. At $\alpha=0$ the flux is linear and the profile simply translates.

###### Bidisperse kinematic sedimentation

↑ **Parent:** [Kinematic sedimentation](#kinematic-sedimentation)

A [particle suspension](#suspension-chemistry) contains two particle species with separate [particle volume fractions](#particle-volume-fraction). In an independent-settling model, each species obeys its own flux conservation equation, while a shared stationary deposit can couple the jump conditions through its maximum total [packing fraction](geometry-and-topology.md#packing-fraction). Such independence is an imposed model; general [hindered settling](#hindered-settling) need not decouple species.

###### Two-stage bidisperse batch sedimentation

↑ **Parent:** [Bidisperse kinematic sedimentation](#bidisperse-kinematic-sedimentation)

Initially, separate clearing fronts of fast and slow species coexist with a mixed deposition front. After the fast clearing front meets that deposit, the remaining suspension contains only the slow species. Its later [sedimentation shock](#sedimentation-shock) builds a pure-slow layer above the earlier mixed deposit. Final layer thicknesses and composition follow from separate particle-volume conservation.

###### Deposit composition from sedimentation jump conditions

↑ **Parent:** [Bidisperse kinematic sedimentation](#bidisperse-kinematic-sedimentation)

For a [bidisperse kinematic sedimentation](#bidisperse-kinematic-sedimentation) model with normalized suspension concentrations $q_i$, isolated speeds $W_i$, and a stationary deposit with $p_1+p_2=1$, the upward deposit-front speed magnitude obeys $s(p_i-q_i)=W_iq_i(1-q_i)$. Adding gives $s=\sum_iW_iq_i(1-q_i)/(1-\sum_iq_i)$; substitution determines each deposited fraction. These are [Rankine-Hugoniot conditions](partial-differential-equation.md#rankine-hugoniot-conditions) with a stationary compacted branch.

###### Sedimentation shock

↑ **Parent:** [Kinematic sedimentation](#kinematic-sedimentation)

A moving discontinuity of [particle volume fraction](#particle-volume-fraction) in [kinematic sedimentation](#kinematic-sedimentation). Conservation of particle [volume](geometry-and-topology.md#volume) gives the [Rankine-Hugoniot condition](partial-differential-equation.md#rankine-hugoniot-conditions) $U[\phi]=[j]$ in a consistently oriented coordinate. A clearing front and a deposit front can both be [sedimentation shocks](#sedimentation-shock). A stationary deposit uses zero particle flux; its compacted branch need not obey the suspension flux law.

###### Sediment mass determines final deposit thickness

↑ **Parent:** [Kinematic sedimentation](#kinematic-sedimentation)

Particle [mass conservation](continuum-mechanics.md#mass-conservation) gives $h_c=[\phi_1(H-z_m)+\phi_2z_m]/\phi_{\max}$. Averaging concentration over the entire original container gives $\bar\phi=\phi_{\max}h_c/H$. This average differs from the concentration inside the deposit itself.

###### Two-layer sedimentation with a compression shock

↑ **Parent:** [Kinematic sedimentation](#kinematic-sedimentation)

With upper concentration $a$ and lower concentration $2a$, the clearing, internal and deposit fronts have speeds $-u_s(1-a)$, $-u_s(1-3a)$ and $2u_sa$. If the lower two merge, the resulting deposit/upper-suspension front has speed $u_sa$. Final deposit thickness is $a(H+z_m)$ by [mass conservation](continuum-mechanics.md#mass-conservation).

###### Triple-shock sedimentation point

↑ **Parent:** [Two-layer sedimentation with a compression shock](#two-layer-sedimentation-with-a-compression-shock)

For initial concentrations $a$ above $z_m$ and $2a$ below it, all three straight [shocks](partial-differential-equation.md#shock-wave) meet when $z_m=H(1-a)/(1+a)$. The common time is $H/[u_s(1+a)]$ and height is $2aH/(1+a)$. Afterwards only a stationary deposit/clear-fluid boundary remains.

###### Quadratic hindered-settling flux

↑ **Parent:** [Kinematic sedimentation](#kinematic-sedimentation)

For downward settling speed $u_s(1-\phi)$ in upward coordinate $z$, particle flux is $j=-u_s\phi(1-\phi)$. The concentration-characteristic speed is $j^{\prime}=u_s(2\phi-1)$ and differs from particle speed. Since $j^{\prime\prime}=2u_s>0$, decreasing concentration with height creates a compressive [shock](partial-differential-equation.md#shock-wave), while increasing concentration creates a [rarefaction wave](partial-differential-equation.md#rarefaction-wave).

###### Parabolic-profile sedimentation shock

↑ **Parent:** [Quadratic hindered-settling flux](#quadratic-hindered-settling-flux)

For $\phi_0(z)=\phi_{\max}(1-z^2/h^2)/3$ on $0\le z\le h$, with clear fluid above and no imposed bed discontinuity, the first compression of the smooth profile occurs at $t=3h/(4V_s)$ and $z=h/4$. The nascent shock enters clear fluid with initial signed speed $-V_s$. Its downward speed subsequently decreases as the state behind it becomes more concentrated, until a boundary interaction changes the problem. This is characteristic breaking, not the time of initiation of a separately imposed packed-bed front.

###### Settling rarefaction fan

↑ **Parent:** [Quadratic hindered-settling flux](#quadratic-hindered-settling-flux)

If lower initial concentration $b$ is less than upper concentration $a$, the [entropy solution](partial-differential-equation.md#entropy-solution) expands into a fan with $\phi=[1+(z-z_m)/(u_st)]/2$. Its characteristic speeds range from $u_s(2b-1)$ to $u_s(2a-1)$. The fan can be clipped by a clearing or deposition [shock](partial-differential-equation.md#shock-wave).

###### Early extinction of a settling rarefaction fan

↑ **Parent:** [Settling rarefaction fan](#settling-rarefaction-fan)

For upper concentration $a$, lower $a/2$ and interface height $4H/5$, both curved fronts meet inside the fan only if $a\geq1-\sqrt{2/3}$. At smaller $a$, the deposition front reaches the fan upper edge first, then advances through uniform concentration $a$. The clearing front remains straight and final time is $H(1-3a/5)/[u_s(1-a)]$.

###### Curved settling fronts within a rarefaction fan

↑ **Parent:** [Settling rarefaction fan](#settling-rarefaction-fan)

For upper concentration $a$, lower concentration $b<a$ and $L=H-z_m$, define $A=aL$ and $D=(1-b)z_m$. Once inside the [settling rarefaction fan](#settling-rarefaction-fan), clearing and deposition [shocks](partial-differential-equation.md#shock-wave) obey $z_u=z_m-u_st+2\sqrt{u_sAt}$ and $z_d=z_m+u_st-2\sqrt{u_sDt}$. These curves apply only while their neighboring concentration remains within the fan.

###### Last surviving characteristic of a settling fan

↑ **Parent:** [Curved settling fronts within a rarefaction fan](#curved-settling-fronts-within-a-rarefaction-fan)

If both [shocks](partial-differential-equation.md#shock-wave) meet inside a [settling rarefaction fan](#settling-rarefaction-fan), $t_c=(\sqrt A+\sqrt D)^2/u_s$ and the last characteristic has concentration $\phi_*=\sqrt A/(\sqrt A+\sqrt D)$. It runs from the initial internal interface to the final deposit point. This construction requires $b\leq\phi_*\leq a$; otherwise a front exits the fan before final deposition.

###### Settling shock speed

↑ **Parent:** [Quadratic hindered-settling flux](#quadratic-hindered-settling-flux)

The [Rankine-Hugoniot condition](partial-differential-equation.md#rankine-hugoniot-conditions) for the [quadratic hindered-settling flux](#quadratic-hindered-settling-flux) gives $V=u_s(\phi_L+\phi_R-1)$, with lower and upper states labelled $L,R$. It includes a downward clearing front ($\phi_R=0$), an upward deposition front ($\phi_L=1$), and a stationary final deposit/clear-fluid interface.

## Dynamic viscosity

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

Dynamic viscosity $\mu$ relates Newtonian shear stress to rate of strain.

### Zero-shear viscosity

↑ **Parent:** [Dynamic viscosity](#dynamic-viscosity)

For an integrable [relaxation modulus](rheology.md#relaxation-modulus), a small constant shear rate sustained from the remote past gives stress equal to that rate times the displayed integral, including any instantaneous solvent mass. For the linear [Oldroyd-B model](rheology.md#oldroyd-b-model) it is $\mu_0+G_0\tau$. A nondecaying elastic modulus would make this integral infinite rather than describe a fluid with finite steady viscosity.

### Kinematic viscosity

↑ **Parent:** [Dynamic viscosity](#dynamic-viscosity)

Kinematic viscosity is dynamic viscosity divided by mass density: $\nu=\mu/\rho$.

#### Density-weighted mean kinematic viscosity

↑ **Parent:** [Kinematic viscosity](#kinematic-viscosity)

For a vertically stratified [accretion disk](astrophysics.md#accretion-disk) with [surface density](astrophysics.md#surface-density-of-a-disk) $\Sigma=\int\rho\,dz$, the density-weighted mean [kinematic viscosity](#kinematic-viscosity) is $\bar\nu=\Sigma^{-1}\int\rho\nu\,dz$. In an [alpha disk](astrophysics.md#alpha-disk) with $\nu=\alpha p/(\rho\Omega)$, this becomes $\bar\nu=\alpha(\Sigma\Omega)^{-1}\int p\,dz$.

// Target: astrophysics.bigb

#### Density-weighted viscosity of a disk

↑ **Parent:** [Kinematic viscosity](#kinematic-viscosity)

If angular [velocity](classical-mechanics.md#velocity) is independent of height, integrating the viscous stress $\rho\nu r\Omega'$ gives $\Sigma\bar\nu r\Omega'$. Thus the [surface density](astrophysics.md#surface-density-of-a-disk) weighted average, rather than an unweighted height average, enters [vertically averaged viscous disk equations](astrophysics.md#vertically-averaged-viscous-disk-equations).

### Viscous stress tensor

↑ **Parent:** [Dynamic viscosity](#dynamic-viscosity)

The viscous stress tensor records momentum flux caused by velocity gradients. For a Newtonian compressible fluid it separates into shear and bulk contributions.

### Reynolds number

↑ **Parent:** [Dynamic viscosity](#dynamic-viscosity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reynolds_number)

The Reynolds number $\operatorname{Re}=UL/\nu$ compares inertial and viscous effects.

## Mass diffusivity

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mass_diffusivity)

Mass diffusivity is the coefficient multiplying the Laplacian in a diffusion law for a concentration or density anomaly.

## Vorticity

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vorticity)

Vorticity is the curl of the velocity field, $\omega=\nabla\times u$.

### Vortex line

↑ **Parent:** [Vorticity](#vorticity)

A [vortex line](#vortex-line) is an [integral](calculus.md#integral) curve of the [vorticity](#vorticity) vector field: its tangent is parallel to $\boldsymbol\omega=\nabla\times\mathbf u$. In a two-dimensional [incompressible flow](#incompressible-flow), these lines are perpendicular to the flow plane and the [vorticity equation](physics.md#vorticity-equation) gives $D\omega/Dt=0$. Since material cross-sectional area is preserved, the flux of [vorticity](#vorticity) through a material [vortex tube](#vortex-tube), equal to its [circulation](#circulation-physics), is constant.

### Vortex (fluid mechanics)

↑ **Parent:** [Vorticity](#vorticity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vortex)

A fluid vortex is a region in which [velocity field](#velocity-field) circulates about an axis or center. [Vorticity](#vorticity) measures local rotation, while [circulation](#circulation-physics) measures the integral of velocity around a closed path. A [phase vortex](critical-phenomenon.md#phase-vortex) is instead a [topological defect](critical-phenomenon.md#topological-defect) defined by winding of an order parameter; superfluid examples connect the two notions.

#### Vortex dynamics

↑ **Parent:** [Vortex (fluid mechanics)](#vortex-fluid-mechanics)

The evolution of a [vorticity](#vorticity) distribution together with the [velocity field](#velocity-field) it induces. A transport equation advances [vorticity](#vorticity); diagnostic inversion recovers [velocity](classical-mechanics.md#velocity) from it and the specified [boundary conditions](differential-equation.md#boundary-condition).

##### Nonrotating layerwise-two-dimensional vortex dynamics

↑ **Parent:** [Vortex dynamics](#vortex-dynamics)

In the limiting model of infinitely strong stable [density stratification](gravity-wave.md#density-stratification), small [Froude number](reduced-gravity.md#froude-number) and fixed vertical scales suppress vertical displacement. Each horizontal level evolves by [two-dimensional vortex dynamics](#two-dimensional-vortex-dynamics); $z$ labels independent copies of the horizontal [Poisson equation](partial-differential-equation.md#poisson-equation). The leading normalized [Ertel potential vorticity](geophysical-fluid-dynamics.md#ertel-potential-vorticity) is $Q/N^2=\zeta$. This is a constrained asymptotic model: finite [buoyancy frequency](gravity-wave.md#buoyancy-frequency) restores vertical motion and coupling, and arbitrarily short vertical scales invalidate the independent-layer limit. [McIntyre's discussion of potential-vorticity inversion](https://pordlabs.ucsd.edu/wryoung/theorySeminar/pdf14/McIntyrePV.pdf) explains the limiting independent-layer picture.

##### Two-dimensional vortex dynamics

↑ **Parent:** [Vortex dynamics](#vortex-dynamics)

For inviscid planar [incompressible flow](#incompressible-flow), write [velocity](classical-mechanics.md#velocity) as $(-\psi_y,\psi_x)$ and [vorticity](#vorticity) as $\zeta=\nabla^2\psi$. Taking [curl](calculus.md#curl) of the [Euler equations for an inviscid fluid](#euler-equations-for-an-inviscid-fluid) removes [pressure](thermodynamics.md#pressure) and gives the displayed transport equation, with $J(\psi,\zeta)=\psi_x\zeta_y-\psi_y\zeta_x$. The [Poisson equation](partial-differential-equation.md#poisson-equation) then recovers the [streamfunction](#stream-function) at each instant. A velocity tangent to the plane cannot stretch its perpendicular [vorticity](#vorticity) vector.

###### Steady planar vorticity as a local function of stream function

↑ **Parent:** [Two-dimensional vortex dynamics](#two-dimensional-vortex-dynamics)

In a steady inviscid planar [incompressible flow](#incompressible-flow), [vorticity](#vorticity) is constant along [streamlines](#streamline). A regular [stream function](#stream-function) supplies a local transverse coordinate, so locally $\Delta\psi$ depends only on $\psi$. A global single-valued function needs the same value on every component of each level set. This can fail: $\psi=x^3-x$ gives the steady Euler shear $(u,v)=(0,1-3x^2)$ with constant pressure, but $\psi(0)=\psi(1)=0$ while $\Delta\psi$ is respectively $0$ and $6$.

#### Line vortex

↑ **Parent:** [Vortex (fluid mechanics)](#vortex-fluid-mechanics)

An ideal straight [line vortex](#line-vortex) in a two-dimensional [incompressible flow](#incompressible-flow) has [circulation](#circulation-physics) $\Gamma$ and induces velocity

$$
\mathbf u(\mathbf r)=\frac{\Gamma}{2\pi}\frac{\mathbf e_z\times(\mathbf r-\mathbf r_0)}{|\mathbf r-\mathbf r_0|^2}.
$$

Its [stream function](#stream-function), with $\mathbf u=(\psi_y,-\psi_x)$, is $\psi=-\Gamma\log|\mathbf r-\mathbf r_0|/(2\pi)$. Positive $\Gamma$ means counterclockwise [circulation](#circulation-physics). In an ideal point-vortex description, the vortex position is advected by the regular velocity produced by the other vortices and the boundaries; its own singular velocity is excluded.

##### Motion of two point vortices

↑ **Parent:** [Line vortex](#line-vortex)

Take vortex strength to mean circulation and $J(x,y)=(-y,x)$. Each [point vortex](#line-vortex) moves with the [velocity](classical-mechanics.md#velocity) induced by the other, so for $\mathbf d=\mathbf x_1-\mathbf x_2$ the displayed equation holds. Since $\mathbf d\cdot J\mathbf d=0$, separation is constant; weighting the two velocities also gives $d(\kappa_1\mathbf x_1+\kappa_2\mathbf x_2)/dt=0$. Equal strengths at opposite points of a circle of radius $a$ rotate with angular speed $\kappa/(4\pi a^2)$.

##### Image vortex at a plane wall

↑ **Parent:** [Line vortex](#line-vortex)

The [method of images](mathematics.md#method-of-images) enforces impermeability at a plane wall by reflecting a [line vortex](#line-vortex) across it and reversing its [circulation](#circulation-physics). The two logarithmic [stream functions](#stream-function) cancel on the wall, which is consequently a [streamline](#streamline). For a vortex of [circulation](#circulation-physics) $\Gamma$ at $(0,b)$ above $y=0$, the image of [circulation](#circulation-physics) $-\Gamma$ at $(0,-b)$ induces velocity $(\Gamma/(4\pi b),0)$ at the real vortex. The signed drift parallel to the wall is therefore $\Gamma/(4\pi b)$.

###### Line-vortex trajectory in a quarter-plane

↑ **Parent:** [Image vortex at a plane wall](#image-vortex-at-a-plane-wall)

In the quadrant $x,y>0$, a [line vortex](#line-vortex) of [circulation](#circulation-physics) $\Gamma$ at $(x,y)$ has three images: circulations $-\Gamma$ at $(-x,y)$ and $(x,-y)$, and $+\Gamma$ at $(-x,-y)$. Their induced velocity is

$$
\dot x=\frac{\Gamma x^2}{4\pi y(x^2+y^2)},\qquad\dot y=-\frac{\Gamma y^2}{4\pi x(x^2+y^2)}.
$$

In [polar coordinates](calculus.md#polar-coordinates), these equations give $\dot r=\Gamma\cot(2\theta)/(2\pi r)$ and $\dot\theta=-\Gamma/(4\pi r^2)$. Direct [differentiation](calculus.md#differentiation) yields $\frac d{dt}(r\sin2\theta)=0$, so the trajectory obeys $r\sin2\theta=\text{constant}$.

### Hydrodynamic Biot-Savart kernel

↑ **Parent:** [Vorticity](#vorticity)

In an unbounded incompressible fluid with localized [vorticity](#vorticity) and no added harmonic background, velocity is reconstructed by $\mathbf u(\mathbf x)=(4\pi)^{-1}\int\boldsymbol\omega(\mathbf y)\times(\mathbf x-\mathbf y)/|\mathbf x-\mathbf y|^3\,d^3y$. Its multipole expansion relates [hydrodynamic impulse](#hydrodynamic-impulse) to a dipolar far-field velocity.

### Hydrodynamic impulse

↑ **Parent:** [Vorticity](#vorticity)

[Hydrodynamic impulse](#hydrodynamic-impulse) per unit density is $\mathbf I=\tfrac12\int\mathbf x\times\boldsymbol\omega\,dV$ for localized [vorticity](#vorticity). In unforced all-space [incompressible flow](#incompressible-flow) its derivative vanishes when far-field fluxes vanish. For a spherical all-space limit, $\mathbf I=(3/2)\lim_R\int_{V_R}\mathbf u\,dV$; a dipolar velocity tail makes the distinction from a bare [momentum](classical-mechanics.md#momentum) integral important.

#### Dipolar velocity field of a localized eddy

↑ **Parent:** [Hydrodynamic impulse](#hydrodynamic-impulse)

A localized [vorticity](#vorticity) distribution with nonzero [hydrodynamic impulse](#hydrodynamic-impulse) induces $\mathbf u\sim[3\mathbf n(\mathbf I\cdot\mathbf n)-\mathbf I]/(4\pi r^3)$. This [curl](calculus.md#curl)-free exterior velocity can remain long-ranged even when the [vorticity](#vorticity) is localized. In a random ensemble it produces dipolar longitudinal and transverse correlation tails.

### Vortex tube

↑ **Parent:** [Vorticity](#vorticity)

A [vortex tube](#vortex-tube) is a bundle of vortex lines bounded by a surface to which [vorticity](#vorticity) is tangent. [Circulation](#circulation-physics) measures its [vorticity](#vorticity) flux. Stretching a nearly incompressible tube reduces its cross-sectional area and increases its [vorticity](#vorticity). The [Burgers vortex](continuum-mechanics.md#burgers-vortex) is a local model in which this concentration balances viscous diffusion.

### Enstrophy

↑ **Parent:** [Vorticity](#vorticity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Enstrophy)

[Enstrophy](#enstrophy) measures squared [vorticity](#vorticity): a local density is $\omega^2/2$, and its spatial integral or ensemble mean gives a global measure. In homogeneous [incompressible flow](#incompressible-flow), [viscous dissipation](stokes-flow.md#viscous-dissipation) satisfies $\epsilon=\nu\langle\omega^2\rangle$. [Vortex stretching](physics.md#vortex-stretching) can produce [enstrophy](#enstrophy) in three dimensions; [kinematic viscosity](#kinematic-viscosity) destroys it.

#### Mean enstrophy balance

↑ **Parent:** [Enstrophy](#enstrophy)

For unforced homogeneous [incompressible flow](#incompressible-flow), the [vorticity equation](physics.md#vorticity-equation) gives $\dot Z=\langle\omega_i\omega_jS_{ij}\rangle-\nu\langle|\nabla\times\boldsymbol\omega|^2\rangle$. [Curl](calculus.md#curl) and full-gradient squared averages agree because the [vorticity](#vorticity) is divergence free and boundary divergences average to zero. In established high-Reynolds-number [turbulence](turbulence.md), slow integral-time evolution makes production and destruction nearly balance.

### Planar vorticity velocity kernel

↑ **Parent:** [Vorticity](#vorticity)

The [velocity](classical-mechanics.md#velocity) induced by planar [vorticity](#vorticity) is a [convolution](fourier-analysis.md#convolution) with this kernel, whose sign depends on the [stream function](#stream-function) and vorticity conventions. Its magnitude is $(2\pi|z|)^{-1}$ and its derivative is bounded by $C|z|^{-2}$. Splitting the convolution at radius $R$ gives $\|K*\omega\|_\infty\leq R\|\omega\|_\infty+\|\omega\|_1/(2\pi R)$. The same singularity yields a [log-Lipschitz modulus](topological-analysis.md#log-lipschitz-modulus), enough for a [Yudovich characteristic flow](#yudovich-characteristic-flow).

### Uniform-vorticity circular flow in an annulus

↑ **Parent:** [Vorticity](#vorticity)

Circular streamlines and constant [vorticity](#vorticity) imply $u_\phi=\omega r/2+C/r$. Zero velocity at $2a$ and positive azimuthal velocity $V$ at $a$ give

$$
u_\phi=\frac V{3a}(4a^2/r-r),\qquad \omega=-\frac{2V}{3a}.
$$

The radial [Euler equations for an inviscid fluid](#euler-equations-for-an-inviscid-fluid) give $p_r=\rho u_\phi^2/r$, yielding outer-minus-inner pressure $(15-16\log2)\rho V^2/18$. The pressure difference is independent of circulation orientation.

### Vorticity cross-product identity

↑ **Parent:** [Vorticity](#vorticity)

For differentiable vector fields, the displayed identity relates [vorticity](#vorticity) to the antisymmetric part of the [velocity gradient](continuum-mechanics.md#velocity-gradient). Together with the [curl of a cross product](calculus.md#curl-of-a-cross-product), it converts the [adjoint linearized Navier-Stokes evolution](hydrodynamic-stability.md#adjoint-linearized-navier-stokes-evolution) between component and rotational forms.

#### Convective acceleration identity

↑ **Parent:** [Vorticity cross-product identity](#vorticity-cross-product-identity)

The local vector-calculus identity

$$
(\mathbf u\cdot\nabla)\mathbf u=\nabla(\tfrac12|\mathbf u|^2)-\mathbf u\times(\nabla\times\mathbf u)
$$

separates the convective [acceleration](classical-mechanics.md#acceleration) into a kinetic-energy gradient and a [vorticity](#vorticity) cross-product contribution. Substitution into the steady [Euler equations for an inviscid fluid](#euler-equations-for-an-inviscid-fluid) yields the vorticity form of the [Bernoulli equation](#bernoulli-equation).

### Hydrodynamical helicity

↑ **Parent:** [Vorticity](#vorticity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hydrodynamical_helicity)

Kinetic helicity measures the alignment and linking of a [velocity field](#velocity-field) and its [vorticity](#vorticity). It is the volume integral of $\mathbf u\cdot\boldsymbol\omega$, with boundary conditions needed for its conservation.

The integral measures linkage and twisting of [vortex lines](#vortex-line) through the [velocity](classical-mechanics.md#velocity) and [vorticity](#vorticity) fields.

#### Kinetic helicity density

↑ **Parent:** [Hydrodynamical helicity](#hydrodynamical-helicity)

The local density of [kinetic helicity](#hydrodynamical-helicity) is $q=\mathbf u\cdot\boldsymbol\omega$. Conservation of its volume integral does not imply that $q$ is a materially advected scalar.

##### Helicity vector of a solenoidal Fourier mode

↑ **Parent:** [Kinetic helicity density](#kinetic-helicity-density)

For a transverse complex velocity amplitude $\hat{\mathbf u}$ and real nonzero [wavevector](continuum-mechanics.md#wavevector) $\mathbf k$, write $\hat{\mathbf u}=\mathbf a+i\mathbf c$. Solenoidality makes both real vectors perpendicular to $\mathbf k$, so $\tfrac12\operatorname{Re}(i\hat{\mathbf u}^*\times\hat{\mathbf u})=-\mathbf a\times\mathbf c=H\mathbf k$. The corresponding spatial average of [kinetic helicity density](#kinetic-helicity-density) is $-Hk^2$. Cross-product order determines this sign.

##### Kinetic helicity conservation law

↑ **Parent:** [Kinetic helicity density](#kinetic-helicity-density)

For smooth inviscid [barotropic fluid](#barotropic-fluid) motion without gravity or magnetic forces, let $w$ be the [specific enthalpy](thermodynamics.md#specific-enthalpy) with $\nabla w=\rho^{-1}\nabla p$, and set $q=\mathbf u\cdot\boldsymbol\omega$. Then

$$
\partial_tq+\nabla\cdot\left[q\mathbf u+\left(w-\frac{u^2}{2}\right)\boldsymbol\omega\right]=0.
$$

This follows by dotting the [barotropic vorticity transport](#barotropic-vorticity-transport) equation with $\mathbf u$ and using the [divergence of a cross product](calculus.md#divergence-of-a-cross-product). A volume integral is constant when the resulting boundary flux vanishes.

###### Material conservation of kinetic helicity density

↑ **Parent:** [Kinetic helicity conservation law](#kinetic-helicity-conservation-law)

The [kinetic helicity conservation law](#kinetic-helicity-conservation-law) implies

$$
\frac{Dq}{Dt}=\boldsymbol\omega\cdot\nabla\left(\frac{u^2}{2}-w\right)-q\nabla\cdot\mathbf u.
$$

Therefore $q$ is materially constant exactly when the right side vanishes. [Incompressible flow](#incompressible-flow) together with constancy of $w-u^2/2$ along vortex lines is sufficient. In compressible flow, the density-normalized quantity satisfies $D(q/\rho)/Dt=-(\boldsymbol\omega/\rho)\cdot\nabla(w-u^2/2)$.

### Absolute vorticity

↑ **Parent:** [Vorticity](#vorticity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Absolute_vorticity)

Absolute vorticity is the vorticity measured in an inertial frame. In a frame rotating with angular velocity $\boldsymbol\Omega$, it is $\boldsymbol\omega+2\boldsymbol\Omega$.

#### Planetary vorticity

↑ **Parent:** [Absolute vorticity](#absolute-vorticity)

The planetary contribution to absolute [vorticity](#vorticity) is supplied by the rotating frame. Its local vertical component is the [Coriolis parameter](geophysical-fluid-dynamics.md#coriolis-parameter) $f=2\Omega\sin\phi$. On a [beta plane](geophysical-fluid-dynamics.md#beta-plane), motion with northward velocity $v$ changes this contribution at the rate $\beta v$.

#### Absolute-vorticity flux tensor

↑ **Parent:** [Absolute vorticity](#absolute-vorticity)

For a flow satisfying [incompressibility](#incompressible-flow), this antisymmetric tensor writes advection and [vortex stretching](physics.md#vortex-stretching) in conservative form. With its first index as transport direction, $(\nabla\cdot T)_j=\partial_iT_{ij}$.

##### Radial vorticity conservation in a shearing sheet

↑ **Parent:** [Absolute-vorticity flux tensor](#absolute-vorticity-flux-tensor)

When the only nonpotential force points radially, its [curl](calculus.md#curl) has no radial component. The radial [absolute vorticity](#absolute-vorticity) therefore obeys a local flux [conservation law](physics.md#conservation-law), although [vortex stretching](physics.md#vortex-stretching) can change it along a fluid trajectory.

### Relative vorticity

↑ **Parent:** [Vorticity](#vorticity)

Relative vorticity is the curl of velocity measured in the chosen rotating frame. Adding the planetary vorticity gives [absolute vorticity](#absolute-vorticity).

### Circulation (physics)

↑ **Parent:** [Vorticity](#vorticity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Circulation_(physics))

The circulation around a closed curve is $\Gamma=\oint u\mathbin{\cdot}dl$.

<h4 id="kelvin-s-circulation-theorem">Kelvin's circulation theorem</h4>

↑ **Parent:** [Circulation (physics)](#circulation-physics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kelvin's_circulation_theorem)

In an inviscid barotropic fluid subject to conservative body force, the [circulation](#circulation-physics) of a material loop is constant. For constant density, parameterize that loop by $\mathbf r(s,t)$ with $\mathbf r_t=\mathbf u$. Differentiating $\Gamma=\int\mathbf u\cdot\mathbf r_s\,ds$ gives an integral of $(D\mathbf u/Dt)\cdot d\mathbf r$ plus $\int\partial_s(|\mathbf u|^2/2)ds$. The latter vanishes on a closed loop, and the [Euler equations](#euler-equations-for-an-inviscid-fluid) make the former the integral of a gradient, also zero. For a barotropic density, $\nabla p/\rho$ is still a gradient of specific enthalpy. Constant circulation is consistent with changing local [vorticity](#vorticity) when a vortex tube changes its cross-sectional area.

##### Irrotational circulation in an exterior domain

↑ **Parent:** [Kelvin's circulation theorem](#kelvin-s-circulation-theorem)

In smooth barotropic inviscid flow with conservative [body force](#body-force), [Kelvin's circulation theorem](#kelvin-s-circulation-theorem) preserves circulation of [material curves](#material-curve). Initially zero [vorticity](#vorticity) therefore gives zero circulation on contractible loops for all times. A loop winding around an excluded obstacle can have a nonzero constant circulation: the planar field $\mathbf u=\Gamma\mathbf e_\theta/(2\pi r)$ is [irrotational](calculus.md#irrotational-vector-field) outside the origin but has circulation $\Gamma$ on a positively oriented enclosing loop.

### Irrotational flow

↑ **Parent:** [Vorticity](#vorticity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Irrotational_flow)

An irrotational flow has zero vorticity and locally admits a velocity potential.

## Circular vortex-sheet mode

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

For a circular patch in solid-body rotation next to stationary fluid, a sinusoidal boundary displacement couples an interior $r^k$ potential to an exterior $r^{-k}$ potential. The tangential velocity jump makes the interface Kelvin--Helmholtz unstable.

## Gravity wave

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](gravity-wave.md)

## Stream function

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stream_function)

A two-dimensional incompressible velocity field can be written either as $u=\psi_y$, $v=-\psi_x$ or with both signs reversed. The continuity equation then holds identically.

### Sinusoidal cellular flow

↑ **Parent:** [Stream function](#stream-function)

Using $\mathbf u=(-\psi_y,\psi_x)$, the displayed [stream function](#stream-function) gives $\mathbf u_0=(\sin x\cos y,-\cos x\sin y)$. Its [streamlines](#streamline) are level sets of $\psi_0$. At $(n\pi,m\pi)$, the [Jacobian matrix](calculus.md#jacobian-matrix) is $\operatorname{diag}((-1)^{n+m},-(-1)^{n+m})$, so the points are [saddle equilibria](dynamical-systems.md#saddle-equilibrium). At $(\pi/2+n\pi,\pi/2+m\pi)$ the eigenvalues are $\pm i$, giving [center equilibria](dynamical-systems.md#center-equilibrium) surrounded by closed [streamlines](#streamline). The grid lines $x=n\pi$ and $y=m\pi$ form [heteroclinic orbits](dynamical-systems.md#heteroclinic-orbit) between adjacent saddles; circulation alternates between cells.

#### Melnikov splitting of a periodically perturbed cellular flow

↑ **Parent:** [Sinusoidal cellular flow](#sinusoidal-cellular-flow)

Perturb the [sinusoidal cellular flow](#sinusoidal-cellular-flow) by $\epsilon\cos x\cos y\sin(\omega t)$ in its [stream function](#stream-function). On $y=0$, parameterizing the unperturbed orbit with $q_0(0)=(X_0,0)$ gives $x(s)=2\arctan e^{s+a}$, $a=\log\tan(X_0/2)$. The [heteroclinic Melnikov function for a periodic planar flow](dynamical-systems.md#heteroclinic-melnikov-function-for-a-periodic-planar-flow) has integrand $\operatorname{sech}^2(t-t_0+a)\sin(\omega t)$. Its odd part vanishes and the Fourier transform of $\operatorname{sech}^2$ gives the displayed result. For each fixed nonzero frequency its simple zeros produce transverse intersections at sufficiently small perturbation, hence exchange of fluid lobes across the former cell boundary. The leading splitting is exponentially small at high frequency; that estimate is not uniform in frequency and perturbation size.

### Linear planar strain and rotation streamlines

↑ **Parent:** [Stream function](#stream-function)

The incompressible planar field $(\alpha x-\beta y,\beta x-\alpha y)$ has the displayed [stream function](#stream-function) under $(u,v)=(\psi_y,-\psi_x)$ and vorticity $2\beta$. In rotated coordinates $s=(x+y)/\sqrt2$, $t=(x-y)/\sqrt2$, $\psi=((\alpha-\beta)s^2-(\alpha+\beta)t^2)/2$. For positive parameters its nonstationary [streamlines](#streamline) are closed ellipses if $\alpha<\beta$, hyperbolas and straight separatrices if $\alpha>\beta$, and parallel straight lines with a stationary diagonal if $\alpha=\beta$.

### Axisymmetric hydrodynamic mass flux function

↑ **Parent:** [Stream function](#stream-function)

For a steady axisymmetric compressible [fluid flow](#fluid-flow), [mass conservation](continuum-mechanics.md#mass-conservation) permits this representation. The mass flow through an annulus between two stream surfaces is $2\pi\Delta\psi$. In a steady adiabatic wind without magnetic forces, the [specific entropy](thermodynamics.md#specific-entropy), [specific angular momentum](classical-mechanics.md#specific-angular-momentum) and [Bernoulli function](#bernoulli-function) are locally functions of $\psi$ on connected regular stream surfaces.

### Stokes streamfunction

↑ **Parent:** [Stream function](#stream-function)

For axisymmetric incompressible flow without swirl, $u_r=-\psi_z/r$ and $u_z=\psi_r/r$. These identities enforce incompressibility, and $2\pi\psi$ measures axial volume flux from the symmetry axis when its additive constant is chosen there.

### Streamline classification of a planar linear saddle or centre

↑ **Parent:** [Stream function](#stream-function)

For $(u,v)=(y,ax)$, the stream function $\psi=(y^2-ax^2)/2$ gives hyperbolic streamlines and a saddle when $a>0$, while $a<0$ gives elliptical streamlines and a centre.

#### Linear planar flow with strain and rotation

↑ **Parent:** [Streamline classification of a planar linear saddle or centre](#streamline-classification-of-a-planar-linear-saddle-or-centre)

The incompressible linear flow $(u,v)=(\epsilon x-\gamma y,\gamma x-\epsilon y)$ has [streamfunction](#stream-function) $\psi=\epsilon xy-\gamma(x^2+y^2)/2$. Its velocity matrix squares to $(\epsilon^2-\gamma^2)I$. Thus strain-dominated flow has saddle trajectories, rotation-dominated flow has closed elliptical trajectories, and equal nonzero strain and rotation gives [simple shear flow](viscous-fluid-flow.md#simple-shear-flow) along parallel lines with a stationary line. Pure rotation is counterclockwise for positive $\gamma$.

## Streamline

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Streamline)

A streamline is a curve tangent everywhere to the instantaneous velocity field. In steady two-dimensional incompressible flow, streamlines are level sets of the stream function.

### Stream tube

↑ **Parent:** [Streamline](#streamline)

A [stream tube](#stream-tube) is a narrow tube whose side boundary consists of [streamlines](#streamline). In steady flow no fluid crosses its sides, so continuity makes its [mass flux](physics.md#mass-flux) $A\rho u$ constant. If flow follows a [magnetic field](electromagnetism.md#magnetic-field) with constant [magnetohydrodynamic mass loading](astrophysical-fluid-dynamics.md#magnetohydrodynamic-mass-loading), its normal area obeys $A|\mathbf B|=\mathrm{constant}$.

## Velocity potential

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Velocity_potential)

An irrotational velocity field is locally a gradient $u=\nabla\phi$. The scalar $\phi$ is its velocity potential.

### Potential flow around a circular cylinder

↑ **Parent:** [Velocity potential](#velocity-potential)

Uniform irrotational flow of speed $U$ past a circular cylinder of radius $a$, with zero circulation, has [velocity potential](#velocity-potential)

$$
\phi=U\left(r+\frac{a^2}{r}\right)\cos\theta.
$$

On the cylinder, the tangential speed is $-2U\sin\theta$, so the [Bernoulli equation](#bernoulli-equation) gives

$$
p(a,\theta)=p_\infty+\frac12\rho U^2(1-4\sin^2\theta).
$$

#### Potential flow around a circular cylinder with circulation

↑ **Parent:** [Potential flow around a circular cylinder](#potential-flow-around-a-circular-cylinder)

Adding circulation $\kappa$ gives the possibly multivalued [velocity potential](#velocity-potential)

$$
\phi=U\left(r+\frac{a^2}{r}\right)\cos\theta+\frac\kappa{2\pi}\theta.
$$

The velocity remains single-valued, and on the cylinder its tangential component is $-2U\sin\theta+\kappa/(2\pi a)$.

<h5 id="kutta-joukowski-theorem">Kutta–Joukowski theorem</h5>

↑ **Parent:** [Potential flow around a circular cylinder with circulation](#potential-flow-around-a-circular-cylinder-with-circulation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kutta–Joukowski_theorem)

For steady two-dimensional inviscid flow of density $\rho$, far-field velocity $\mathbf U$, and circulation $\kappa$, the force per unit span is perpendicular to the flow. With counterclockwise circulation taken positive and $\mathbf U=U\mathbf e_x$, it is $-\rho\kappa U\mathbf e_y$.

###### Advective and pressure contributions to circulatory lift

↑ **Parent:** [Kutta–Joukowski theorem](#kutta-joukowski-theorem)

For [uniform flow](#uniform-flow) $\mathbf U$ plus a [line vortex](#line-vortex) of counterclockwise [circulation](#circulation-physics) $\Gamma$, the outward advective [momentum flux](physics.md#momentum-flux) around a large circle is $\rho\boldsymbol\Gamma\times\mathbf U/2$. The [Bernoulli equation](#bernoulli-equation) supplies an equal [pressure](thermodynamics.md#pressure) contribution. Their sum is the force on the fluid; the force on an obstacle per unit span is its negative, $\rho\mathbf U\times\boldsymbol\Gamma$. Retaining only the advective term loses half the lift and obscures its sign.

### Radially symmetric incompressible flow in a planar annulus

↑ **Parent:** [Velocity potential](#velocity-potential)

For liquid occupying $a(t)<r<b(t)$, radial symmetry and [incompressible flow](#incompressible-flow) imply

$$
u_r(r,t)=\frac{a\dot a}{r},
\qquad
\phi(r,t)=a\dot a\log r+C(t).
$$

The [kinematic boundary condition](#kinematic-boundary-condition) at the outer interface gives

$$
b^2-a^2=\text{constant},
$$

which expresses conservation of the liquid's area.

#### Pressure in radially symmetric annular potential flow

↑ **Parent:** [Radially symmetric incompressible flow in a planar annulus](#radially-symmetric-incompressible-flow-in-a-planar-annulus)

If the pressure at $r=b(t)$ is $p_\infty$, the [Unsteady Bernoulli equation](#unsteady-bernoulli-equation) gives

$$
p(a,t)-p_\infty
=\rho\left[\frac d{dt}(a\dot a)\log\frac ba
-\frac{(a\dot a)^2}{2}\left(\frac1{a^2}-\frac1{b^2}\right)\right].
$$

##### Small oscillation of a planar gas bubble in an annular liquid

↑ **Parent:** [Pressure in radially symmetric annular potential flow](#pressure-in-radially-symmetric-annular-potential-flow)

For $a=a_0(1+\epsilon)$, equilibrium outer radius $b_0$, and a bubble gas obeying $p_0\pi a^2=\text{constant}$, the [linearization](algebra.md#linearization) is

$$
\rho a_0^2\log\frac{b_0}{a_0}\,\ddot\epsilon
=-2p_\infty\epsilon.
$$

The bubble therefore undergoes [simple harmonic motion](classical-mechanics.md#simple-harmonic-motion) with

$$
\omega^2=\frac{2p_\infty}{\rho a_0^2\log(b_0/a_0)}.
$$

## Plume (fluid dynamics)

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Plume_(fluid_dynamics))

A [plume](#plume-fluid-dynamics) is a localized buoyancy-driven flow generated by a source of heat or another density-changing substance. A plume can be laminar or turbulent; the transport regime is an additional condition.

### Laminar plume

↑ **Parent:** [Plume (fluid dynamics)](#plume-fluid-dynamics)

A laminar plume is a narrow buoyancy-driven flow in which viscous diffusion balances inertia across the plume.

#### Integral momentum-flux balance for a two-dimensional plume

↑ **Parent:** [Laminar plume](#laminar-plume)

For a steady incompressible plume with localized vertical body force $b(x)\delta(y)$, decay of velocity and shear at transverse infinity gives

$$
\frac{d}{dx}\int_{-\infty}^{\infty}\rho u^2\,dy=b(x).
$$

#### Similarity scaling of a two-dimensional laminar plume

↑ **Parent:** [Laminar plume](#laminar-plume)

If $b(x)=Bx^{-1/5}$, balancing the momentum flux and transverse viscosity gives

$$
\Delta\sim\left(\frac{\mu^2}{\rho B}\right)^{1/3}x^{2/5},
\qquad
U\sim\left(\frac{B^2}{\rho\mu}\right)^{1/3}x^{1/5}.
$$

##### Similarity equation for a two-dimensional laminar plume

↑ **Parent:** [Similarity scaling of a two-dimensional laminar plume](#similarity-scaling-of-a-two-dimensional-laminar-plume)

With $u=-\psi_y$, $v=\psi_x$, $\eta=y/\Delta$, and $\psi=U\Delta f(\eta)$, the plume boundary-layer equation reduces to

$$
f'''+\frac15(f')^2-\frac35ff''=\delta(\eta).
$$

## Euler equations for an inviscid fluid

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euler_equations_for_an_inviscid_fluid)

Euler’s equations express momentum conservation in a fluid without viscosity.

### Linearized Euler equations

↑ **Parent:** [Euler equations for an inviscid fluid](#euler-equations-for-an-inviscid-fluid)

The linearized Euler equations retain only first-order perturbations about a specified inviscid fluid state. Together with the linearized [continuity equation](physics.md#continuity-equation) and a pressure-density constitutive relation, they describe small-amplitude [acoustic waves](#acoustic-wave). About a uniform resting state, $\rho_0\partial_t\mathbf u'=-\nabla p'$, $\partial_t\rho'+\rho_0\nabla\cdot\mathbf u'=0$, and an isentropic pressure perturbation has $p'=c_0^2\rho'$. Gradients and advection of a moving background must be retained when its variation is not negligible.

### Conservative energy flux of a polytropic ideal gas

↑ **Parent:** [Euler equations for an inviscid fluid](#euler-equations-for-an-inviscid-fluid)

For an unmagnetized [ideal gas](thermodynamics.md#ideal-gas) without gravity, the [pressure](thermodynamics.md#pressure) equation gives internal-energy balance $\partial_te+\partial_x(u_xe)=-p\partial_xu_x$, where $e=p/(\gamma-1)$. The momentum equation gives kinetic-energy balance with source $-u_x\partial_xp$. Their sum is conservative with the displayed total-energy flux. Tangential [velocities](classical-mechanics.md#velocity) contribute to [kinetic energy](classical-mechanics.md#kinetic-energy) even when all derivatives are in the normal direction. Smooth [polytropic flow](compressible-flow.md#polytropic-flow) advects its [entropy](thermodynamics.md#entropy) parameter; a physical shock need not preserve that parameter across the discontinuity.

### Crocco form of the unsteady Euler equation

↑ **Parent:** [Euler equations for an inviscid fluid](#euler-equations-for-an-inviscid-fluid)

For a fixed-composition inviscid fluid, [specific enthalpy](thermodynamics.md#specific-enthalpy) satisfies $dw=Tds+dp/\rho$. Combining this identity with the [vorticity cross-product identity](#vorticity-cross-product-identity) gives the displayed equation, with $\boldsymbol\omega=\nabla\times\mathbf u$ and $\varepsilon=u^2/2+\Phi+w$. It exposes entropy gradients as the thermodynamic source of a mismatch between [Bernoulli function](#bernoulli-function) gradients and the vorticity term. In a steady [adiabatic process](thermodynamics.md#adiabatic-process), its projection along a [streamline](#streamline) makes $\varepsilon$ constant there.

### Yudovich characteristic flow

↑ **Parent:** [Euler equations for an inviscid fluid](#euler-equations-for-an-inviscid-fluid)

For a planar Euler velocity obtained from vorticity in $L^\infty_{\mathrm{loc}}(dt;L^1\cap L^\infty)$, the [planar vorticity velocity kernel](#planar-vorticity-velocity-kernel) gives a locally integrable speed bound and [log-Lipschitz modulus](topological-analysis.md#log-lipschitz-modulus). Spatial mollification gives existence of global trajectories; the [Osgood uniqueness criterion](differential-equation.md#osgood-uniqueness-criterion) gives uniqueness and continuous dependence. Measurability in time and an initial trace are needed. This establishes the flow for a fixed Euler solution; nonlinear uniqueness of the Euler solution itself requires further comparison arguments.

<h3 id="bernoulli-s-principle">Bernoulli's principle</h3>

↑ **Parent:** [Euler equations for an inviscid fluid](#euler-equations-for-an-inviscid-fluid)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bernoulli's_principle)

The [Bernoulli principle](#bernoulli-s-principle) relates [pressure](thermodynamics.md#pressure), [kinetic energy](classical-mechanics.md#kinetic-energy) per unit volume and [Newtonian gravitational potential](classical-mechanics.md#newtonian-gravitational-potential) along a streamline of steady [inviscid flow](#inviscid-flow). For constant [mass density](#density), the [Bernoulli equation](#bernoulli-equation) gives $p/\rho+u^2/2+\Phi$ constant along that streamline. Constancy across different streamlines requires further hypotheses, such as [irrotational flow](#irrotational-flow).

#### Venturi effect

↑ **Parent:** [Bernoulli's principle](#bernoulli-s-principle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Venturi_effect)

In ideal steady flow, a contraction of a pipe increases the speed and lowers the pressure. For constant [mass density](#density), equal body-force potential at the ends and approximately uniform endpoint speeds, [conservation of mass](continuum-mechanics.md#mass-conservation) and the [Bernoulli equation](#bernoulli-equation) give $\dot M=S_1S_2\sqrt{2\rho(p_1-p_2)/(S_1^2-S_2^2)}$ for flow from a wider to a narrower section. Elevation changes contribute a body-force potential difference, and nonuniform profiles or viscous losses require additional information.

// Target: probability-and-statistics.bigb

### Axisymmetric inviscid flow between moving parallel plates

↑ **Parent:** [Euler equations for an inviscid fluid](#euler-equations-for-an-inviscid-fluid)

For plates $z=\pm h(t)$, incompressibility, impermeability and regularity on the axis determine a z-independent radial velocity $u_r=-r\dot h/(2h)$ and vertical velocity $u_z=z\dot h/h$. A possible azimuthal velocity requires additional rotational data; continuity alone does not determine it. For a smooth regular initial profile $U(r)$ independent of $z$, its azimuthal Euler equation transports it as $u_\theta(r,t)=\lambda U(\lambda r)$, where $\lambda=\sqrt{h/h_0}$. If the rotation is solid-body with angular velocity $\Omega(t)$, the [vorticity equation](physics.md#vorticity-equation) gives $\Omega=\Omega_0h/h_0$. Along a particle path, $r^2h$ and $r^2\Omega$ are constant, illustrating [conservation of angular momentum](classical-mechanics.md#conservation-of-angular-momentum).

### Radial velocity

↑ **Parent:** [Euler equations for an inviscid fluid](#euler-equations-for-an-inviscid-fluid)

Radial velocity is the component of a velocity field along the line from a chosen centre to the point of observation.

### Unsteady Bernoulli equation

↑ **Parent:** [Euler equations for an inviscid fluid](#euler-equations-for-an-inviscid-fluid)

For time-dependent [irrotational flow](#irrotational-flow) with $u=\nabla\phi$, constant [mass density](#density), and no body force, the [Euler equations for an inviscid fluid](#euler-equations-for-an-inviscid-fluid) integrate to

$$
\partial_t\phi+\frac12|\nabla\phi|^2+\frac p\rho=C(t).
$$

A time-dependent change of gauge in $\phi$ may set $C(t)=0$.

This is the unsteady potential-flow version of [Bernoulli's principle](#bernoulli-s-principle), with a time-dependent potential gauge.

#### Constant-tension balloon discharge

↑ **Parent:** [Unsteady Bernoulli equation](#unsteady-bernoulli-equation)

A spherical balloon feeding an inviscid uniform tube plug, with entrance excess [pressure](thermodynamics.md#pressure) $2\gamma/R$, satisfies $L\dot u=2\gamma/(\rho R)$ and $4\pi R^2\dot R=-\pi a^2u$. Eliminating $u$ yields the displayed equation. Its [first integral](differential-equation.md#first-integral) is $R^4\dot R^2+KR^2=C$. From rest at radius $R_0$, $C=KR_0^2$; integration gives $t=R_0^2K^{-1/2}(\pi/4-\theta/2+\sin(2\theta)/4)$, where $\theta=\arcsin(R/R_0)$. The ideal emptying time is $\pi R_0^2/(4\sqrt K)$. Independently prescribed initial flow changes $C$ and therefore this time.

#### Inviscid startup in a pressure-driven tube

↑ **Parent:** [Unsteady Bernoulli equation](#unsteady-bernoulli-equation)

For a slender tube of length $L$ supplied from a large reservoir with excess pressure $P$, negligible gravity and entrance inertia, the [Unsteady Bernoulli equation](#unsteady-bernoulli-equation) gives $L\dot U+U^2/2=P/\rho$. A stationary initial liquid column has the displayed speed and [volume flux](#volumetric-flow-rate) $\pi a^2U$ for tube radius $a$. The inertial term controls the early linear acceleration; the kinetic-energy term sets the terminal inviscid speed. This is a leading slender-tube model while the reservoir remains large and the tube full.

#### Linearly elastic balloon discharge

↑ **Parent:** [Unsteady Bernoulli equation](#unsteady-bernoulli-equation)

An inviscid uniform tube plug driven by entrance excess pressure $KV$ obeys $\rho L\dot u=KV$ and $\dot V=-\pi a^2u$. From rest, the first zero of $V$ occurs after a quarter harmonic period, independent of its initial volume. The maximum speed is proportional to that initial volume. Entrance losses, a reservoir kinetic head or independently prescribed initial flow change this ideal model.

### Clebsch-potential variational derivation of incompressible Euler flow

↑ **Parent:** [Euler equations for an inviscid fluid](#euler-equations-for-an-inviscid-fluid)

For $\mathbf u=\nabla\phi+\beta\nabla\alpha$, the density

$$
\mathcal L=-\beta\alpha_t-\frac12|\mathbf u|^2
$$

gives incompressibility and material conservation of $\alpha$ and $\beta$. Differentiating the Clebsch representation then yields the Euler momentum equation with

$$
p=-\frac12|\mathbf u|^2-\phi_t-\beta\alpha_t.
$$

### Bernoulli equation

↑ **Parent:** [Euler equations for an inviscid fluid](#euler-equations-for-an-inviscid-fluid)

For steady inviscid flow, pressure, kinetic energy density, and conservative potential are constant along a streamline.

#### Bernoulli invariant

↑ **Parent:** [Bernoulli equation](#bernoulli-equation)

In a steady adiabatic inviscid fluid with a conservative body force, the [Bernoulli invariant](#bernoulli-invariant) is the displayed specific energy, constant along each [streamline](#streamline). Dotting the [Euler equations](#euler-equations-for-an-inviscid-fluid) with velocity and using the [specific enthalpy](thermodynamics.md#specific-enthalpy) identity gives $\mathbf u\cdot\nabla b=0$. In [ideal magnetohydrodynamics](astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamics), magnetic work need not vanish; the [planar ideal-MHD Bernoulli invariant](astrophysical-fluid-dynamics.md#planar-ideal-mhd-bernoulli-invariant) includes the corresponding electromagnetic correction.

#### Hydraulic control over a smooth hump

↑ **Parent:** [Bernoulli equation](#bernoulli-equation)

A slowly varying, steady, inviscid channel flow has constant discharge $Q=uh$ per unit width and the displayed [Bernoulli equation](#bernoulli-equation). The bed-height function of depth has its maximum at $h_c=(Q^2/g)^{1/3}$, where the [Froude number](reduced-gravity.md#froude-number) is one. At a nondegenerate critical crest, a differentiable profile changes between the [subcritical flow](reduced-gravity.md#subcritical-flow) and [supercritical flow](reduced-gravity.md#supercritical-flow) branches. With subcritical upstream squared Froude number $F<1$ and upstream depth $h_1$, the shock-free supercritical downstream depth is $h_1(F+\sqrt{F^2+8F})/4$.

#### Bernoulli function for planar constant-vorticity flow

↑ **Parent:** [Bernoulli equation](#bernoulli-equation)

With the [streamfunction](#stream-function) convention $(u,v)=(\psi_y,-\psi_x)$, constant scalar [vorticity](#vorticity) gives $\mathbf u\times\boldsymbol\omega=-\omega\nabla\psi$. For steady inviscid constant-density flow without body force, this integrates to

$$
\tfrac12|\mathbf u|^2+\omega\psi+p/\rho=C
$$

throughout a connected fluid region. Reversing the streamfunction convention changes the sign of its term; the declared convention matters.

#### Steady rotating-frame Bernoulli integral

↑ **Parent:** [Bernoulli equation](#bernoulli-equation)

For [steady flow](#steady-flow) of constant-density fluid in a uniformly rotating frame with conservative body forces, the displayed quantity is constant along each relative [streamline](#streamline). The [centrifugal potential](physics.md#centrifugal-potential) contributes the negative quadratic term, and the [Coriolis force](physics.md#coriolis-force) contributes no work because it is perpendicular to the relative velocity. The result follows by dotting the rotating [Euler equations for an inviscid fluid](#euler-equations-for-an-inviscid-fluid) with that velocity.

#### Bernoulli function

↑ **Parent:** [Bernoulli equation](#bernoulli-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bernoulli_function)

The Bernoulli function combines pressure, kinetic energy density, and conservative potential.

#### Bernoulli equation over topography

↑ **Parent:** [Bernoulli equation](#bernoulli-equation)

For steady potential flow over small hills, linearized Bernoulli pressure combines a hydrostatic term $-\rho g\eta$ with a dynamic term $-\rho U\phi_x$.

#### Draining time of a uniform tank through a siphon

↑ **Parent:** [Bernoulli equation](#bernoulli-equation)

If a tank and siphon tube have areas $A$ and $a$, the tube outlet is $H$ below an inlet initially submerged by $h_0$, and both free boundaries are at atmospheric pressure, continuity and Bernoulli's equation give

$$
t=\sqrt{2}\left(\frac{A^2}{a^2}-1\right)^{1/2}
\frac{\sqrt{H+h_0}-\sqrt H}{\sqrt g}
$$

for the free surface to reach the inlet.

### Integral momentum equation

↑ **Parent:** [Euler equations for an inviscid fluid](#euler-equations-for-an-inviscid-fluid)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Integral_momentum_equation)

The integral momentum equation balances momentum flux, pressure, body force, and forces on a control volume.

#### Holding force on a contracting nozzle

↑ **Parent:** [Integral momentum equation](#integral-momentum-equation)

For steady ideal flow through a horizontal contracting nozzle, [Bernoulli equation](#bernoulli-equation) gives inlet gauge pressure $p_0=\rho Q^2(A_1^{-2}-A_0^{-2})/2$. The [integral momentum equation](#integral-momentum-equation) gives the fluid's force on the nozzle as $p_0A_0-\rho Q^2(A_1^{-1}-A_0^{-1})$ in the outlet direction. Simplification yields the displayed nonnegative magnitude. The external holding force has equal magnitude and the opposite direction.

#### Force on a pipe junction

↑ **Parent:** [Integral momentum equation](#integral-momentum-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Force_on_a_pipe_junction)

The force on a pipe junction follows by balancing inlet and outlet momentum fluxes and pressure forces.

## Conservation of mass in a pipe

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conservation_of_mass_in_a_pipe)

For steady incompressible pipe flow, volume flux equals cross-sectional area times mean speed and is conserved through a junction.

## Viscous fluid flow

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](viscous-fluid-flow.md)

## Surface tension

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Surface_tension)

Surface tension is interfacial energy per unit area and produces a normal-stress jump proportional to mean curvature.

### Surface energy

↑ **Parent:** [Surface tension](#surface-tension)

For a liquid interface with constant [surface tension](#surface-tension) $\gamma$, the mechanical [surface energy](#surface-energy) is $E_{\mathrm s}=\gamma A$, up to a fixed additive constant. Increasing area by $dA$ requires work $\gamma\,dA$. At fixed liquid volume, a decrease in area can drive [viscous fluid flow](viscous-fluid-flow.md); the released [surface energy](#surface-energy) supplies [viscous dissipation](stokes-flow.md#viscous-dissipation). If [surface tension](#surface-tension) depends on temperature or composition, the mechanical area-work relation must be distinguished from the complete interfacial thermodynamic energy.

### Wetting

↑ **Parent:** [Surface tension](#surface-tension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wetting)

#### Contact line

↑ **Parent:** [Wetting](#wetting)

The line where the interfaces of three phases meet, for example where a liquid film meets a solid and the surrounding gas. Continuum assumptions at this line can differ from the bulk [lubrication approximation](viscous-fluid-flow.md#lubrication-theory).

### Bond number

↑ **Parent:** [Surface tension](#surface-tension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bond_number)

The Bond number compares hydrostatic stress over a length $\ell$ with capillary stress. For a gas bubble of radius $a$ and negligible density, $\mathrm{Bo}=\rho ga^2/\gamma$. Small Bond number is the usual sufficient criterion for capillarity to resist gravity-scale deformations. For the clean-bubble terminal speed, the [capillary number](#capillary-number) is $\mathrm{Ca}=\mu U/\gamma=\mathrm{Bo}/3$.

### Oil lens capillary balance

↑ **Parent:** [Surface tension](#surface-tension)

For a broad, thin oil lens below a flat ice-water interface, define the effective interfacial energy $\Gamma=\gamma_{io}+\gamma_{ow}-\gamma_{iw}$ from the relevant [surface tensions](#surface-tension). At fixed oil volume $\mathcal V=Ah$, the energy is $E=\Gamma\mathcal V/h+\frac12(\rho_w-\rho_o)g\mathcal Vh$. Setting its [derivative](calculus.md#derivative) to zero gives $h^2=2\Gamma/[(\rho_w-\rho_o)g]$ for $\Gamma>0$, and the positive [second derivative](calculus.md#second-derivative) proves a minimum. A contact angle measured through the oil gives $\Gamma=\gamma_{ow}(1-\cos\vartheta)$. Oil-ice tension alone does not determine this effective quantity. Complete wetting or rough underside pockets invalidate this finite, flat-lens approximation. With densities $1025$ and $850\,\mathrm{kg\,m^{-3}}$, a lens below $1\,\mathrm{cm}$ requires $0<\Gamma<0.08584\,\mathrm{N\,m^{-1}}$.

### Contact angle

↑ **Parent:** [Surface tension](#surface-tension)

The contact angle is measured through a liquid between its interface and a solid substrate at their contact line. In a gently sloping two-dimensional film on a horizontal substrate, its small-angle value is the limiting magnitude of the height slope. A zero contact angle means a tangential approach to the substrate; it does not imply bounded curvature, as the limiting [zero-flux thermocapillary film profiles](viscous-fluid-flow.md#zero-flux-thermocapillary-film-profiles) illustrate.

### Capillary number

↑ **Parent:** [Surface tension](#surface-tension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Capillary_number)

The capillary number compares viscous stresses with [surface tension](#surface-tension). Its velocity and viscosity conventions must be specified; a porous-medium displacement can use the [Darcy velocity](porous-media-flow.md#darcy-velocity) and the viscosity of the displaced fluid.

### Capillary pressure

↑ **Parent:** [Surface tension](#surface-tension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Capillary_pressure)

Capillary pressure is the pressure jump produced by a curved interface. For constant surface tension it is proportional to the interface curvature according to the [Young–Laplace equation](#young-laplace-equation).

### Surfactant

↑ **Parent:** [Surface tension](#surface-tension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Surfactant)

A surfactant is an interfacially active substance that changes surface tension. A concentration gradient therefore generates tangential [Marangoni stress](#marangoni-effect).

#### Surfactant transport with exchange relaxation

↑ **Parent:** [Surfactant](#surfactant)

The [material derivative](continuum-mechanics.md#material-derivative) of surface concentration combines tangential and normal area change, [surface diffusion](#surface-diffusion), and relaxation towards a reservoir concentration $C_0$. The rate $k$ represents exchange; setting $k=0$ recovers transport without exchange. The concentration is measured per interfacial area, so stretching dilutes it.

##### Translating surfactant-coated bubble

↑ **Parent:** [Surfactant transport with exchange relaxation](#surfactant-transport-with-exchange-relaxation)

A spherical inviscid bubble moving slowly through a viscous liquid has a dipolar [surfactant](#surfactant) perturbation. The associated [Marangoni stress](#marangoni-effect) reduces the tangential velocity from its clean-bubble value towards zero. In the linear regime, with $\mathbf u_s=A(I-\mathbf n\mathbf n)\mathbf U$, the consistent [Newtonian fluid stress tensor](viscous-fluid-flow.md#newtonian-fluid-stress-tensor) gives $A=-1/[2(1+2\lambda)]$.

###### Normal stress balance on a translating bubble

↑ **Parent:** [Translating surfactant-coated bubble](#translating-surfactant-coated-bubble)

The dipolar normal [traction](continuum-mechanics.md#traction) is balanced by buoyant [hydrostatic pressure](#hydrostatic-pressure) and the concentration-dependent normal capillary stress, in addition to the constant gas pressure and equilibrium Laplace pressure. A degree-one shape perturbation translates a sphere rather than deforming it; the balance fixes the terminal speed. A uniform gas pressure alone cannot balance this mode.

###### Dipolar surfactant distribution

↑ **Parent:** [Translating surfactant-coated bubble](#translating-surfactant-coated-bubble)

Linear steady transport on a translating sphere gives $B=2AC_0a/(ka^2+2D_s)$. The components of its unit [normal vector](differential-geometry.md#normal-vector) are degree-one [spherical harmonics](analysis.md#spherical-harmonic). The condition $2|A|Ua/(ka^2+2D_s)\ll1$ ensures the concentration perturbation is small relative to $C_0$.

#### Surfactant stabilization of film rupture

↑ **Parent:** [Surfactant](#surfactant)

Outward interfacial flow from a thinning region dilutes surfactant there and raises its [surface tension](#surface-tension). The resulting [Marangoni stress](#marangoni-effect) pulls fluid back toward the thinning region, opposes further stretching, and slows rupture.

##### Strong-surfactant long-wave rupture maximum

↑ **Parent:** [Surfactant stabilization of film rupture](#surfactant-stabilization-of-film-rupture)

For strong [Marangoni stress](#marangoni-effect) and large $\Gamma=\gamma h_0^2/(3V)$, the unstable band has $K\ll1$. Its rate is asymptotically $[3V/(\mu h_0^3)]K^2(1-\Gamma K^2)/3$. Maximizing this quadratic in $K^2$ gives the displayed finite-wavelength maximum. The growth timescale is not alone a bubble lifetime: initial disturbance size and thickness evolution also enter.

#### Insoluble surfactant

↑ **Parent:** [Surfactant](#surfactant)

An insoluble surfactant remains on an interface. Without surface diffusion, its material concentration changes only through the local surface-area dilation rate.

##### Surface diffusion

↑ **Parent:** [Insoluble surfactant](#insoluble-surfactant)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Surface_diffusion)

Surface diffusion transports particles along an interface down a [concentration](physics.md#concentration) gradient. On an isotropic smooth interface with constant diffusivity $D_s$, its flux is $-D_s\nabla_sC$ and its concentration source is $D_s\Delta_sC$, using the [surface gradient](riemannian-geometry.md#surface-gradient) and [surface Laplacian](differential-geometry.md#surface-laplacian).

##### Conservation of insoluble surfactant on a moving interface

↑ **Parent:** [Insoluble surfactant](#insoluble-surfactant)

For concentration $C$ per unit [surface area](differential-geometry.md#surface-area), conservation on a moving material interface gives

$$
\frac{DC}{Dt}=-C\left[\nabla_s\cdot\mathbf u_s+u_n\nabla_s\cdot\mathbf n\right]+D_s\Delta_sC.
$$

The [material derivative](continuum-mechanics.md#material-derivative) follows the surface particles. The two dilution terms are tangential expansion and curvature-induced area change from normal velocity $u_n$; the last term is [surface diffusion](#surface-diffusion).

###### Quadrupolar surfactant distribution on a spherical interface

↑ **Parent:** [Conservation of insoluble surfactant on a moving interface](#conservation-of-insoluble-surfactant-on-a-moving-interface)

For radius $a$ and tangential velocity $\mathbf u_s=\mathbf I_s\mathbf A\mathbf x$ with symmetric traceless $\mathbf A$, the [surface divergence](riemannian-geometry.md#surface-divergence) is $-3\mathbf n\cdot\mathbf A\mathbf n$. At small surface [Péclet number](#peclet-number) $a^2|\mathbf A|/D_s$, neglecting advection of the concentration perturbation gives

$$
C-C_0=\frac{C_0a^2}{2D_s}\mathbf n\cdot\mathbf A\mathbf n.
$$

The result follows because this quadratic is a degree-two [spherical harmonic](analysis.md#spherical-harmonic) with [surface Laplacian](differential-geometry.md#surface-laplacian) $-6/a^2$ times itself and zero spherical mean.

### Marangoni effect

↑ **Parent:** [Surface tension](#surface-tension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Marangoni_effect)

The Marangoni effect is interfacial flow driven by a surface-tension gradient. Tangential stress balances the surface gradient $\nabla_s\gamma$.

#### Thermocapillary migration of an insulating bubble

↑ **Parent:** [Marangoni effect](#marangoni-effect)

For a clean spherical gas bubble with negligible internal [dynamic viscosity](#dynamic-viscosity) and [thermal conductivity](thermodynamics.md#thermal-conductivity), a weak temperature gradient produces the displayed migration [velocity](classical-mechanics.md#velocity), where $\gamma_T=d\gamma/dT$. The exterior [Papkovich–Neuber representation](stokes-flow.md#papkovich-neuber-representation) can use only the scalar potential $\chi=-a^3\mathbf U\cdot\mathbf r/(2r^3)$. Its surface normal velocity equals $\mathbf U\cdot\mathbf n$, and its tangential [traction](continuum-mechanics.md#traction) balances minus the surface [surface tension](#surface-tension) gradient from the [temperature dipole around an insulating sphere](thermodynamics.md#temperature-dipole-around-an-insulating-sphere). For the usual $\gamma_T<0$ the bubble moves toward warmer liquid. Small [Reynolds number](#reynolds-number), [Péclet number](#peclet-number), [capillary number](#capillary-number), and fractional surface-tension variation justify the approximation; [surfactants](#surfactant) can oppose the temperature-driven [Marangoni stress](#marangoni-effect).

#### Interfacial stress balance with variable surface tension

↑ **Parent:** [Marangoni effect](#marangoni-effect)

Across a fluid interface, the jump in normal traction is the surface tension times curvature, while the tangential traction jump is the surface gradient of surface tension. For one common normal convention,

$$
(\boldsymbol\sigma_+-\boldsymbol\sigma_-)\mathbin\cdot\mathbf n
=\gamma\kappa\mathbf n-\nabla_s\gamma.
$$

##### Marangoni immobilization of a bubble in straining flow

↑ **Parent:** [Interfacial stress balance with variable surface tension](#interfacial-stress-balance-with-variable-surface-tension)

For an almost spherical inviscid bubble in exterior [Stokes flow](stokes-flow.md) $\mathbf E\mathbf x$, let $\gamma=\gamma_0-\gamma_1(C-C_0)$ and $K=C_0a^2/(2D_s)$. The [quadrupolar surfactant distribution on a spherical interface](#quadrupolar-surfactant-distribution-on-a-spherical-interface) makes the tangential velocity $\mathbf u_s=\alpha\mathbf I_s\mathbf E\mathbf x$ satisfy

$$
\alpha=\frac5{5+2M},\qquad M=\frac{K\gamma_1}{\mu a}.
$$

The [Marangoni stress](#marangoni-effect) approaches the stress needed to suppress surface motion as $M$ grows. The quadrupolar shape perturbation $r=a(1+\mathbf n\cdot\mathbf D\mathbf n)$ is

$$
\mathbf D=\frac{5\mu a}{\gamma_0}\frac{2+M}{5+2M}\mathbf E.
$$

These expressions require small deformation and small surface [Péclet number](#peclet-number); large $M$ alone does not justify a small concentration perturbation.

#### Chemophoresis

↑ **Parent:** [Marangoni effect](#marangoni-effect)

Chemophoresis is the motion of a particle or droplet driven by a gradient in chemical concentration. For a surfactant-coated bubble, adsorption converts the chemical gradient into a [Marangoni stress](#marangoni-effect).

<h3 id="rayleigh-plateau-instability">Rayleigh–Plateau instability</h3>

↑ **Parent:** [Surface tension](#surface-tension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rayleigh–Plateau_instability)

The Rayleigh–Plateau instability makes a sufficiently long cylindrical fluid thread unstable to axisymmetric radius perturbations. Surface tension lowers area by amplifying wavelengths longer than the circumference-scale threshold.

#### Capillary instability of an annular liquid lining

↑ **Parent:** [Rayleigh–Plateau instability](#rayleigh-plateau-instability)

A thin liquid lining inside a rigid cylindrical tube has [pressure](thermodynamics.md#pressure) perturbation $p_1=-\sigma(a^{-2}h_1+h_{1,xx})$ at leading order in $h_0/a$. [Lubrication theory](viscous-fluid-flow.md#lubrication-theory) gives flux $q=-h_0^3p_x/(3\mu)$, so [mass conservation](continuum-mechanics.md#mass-conservation) gives the displayed growth rate. Long waves with $0<k^2a^2<1$ grow, while short waves are stabilized by [curvature](differential-geometry.md#curvature). The maximum occurs at $k^2a^2=1/2$.

##### Surfactant stabilization of an annular liquid lining

↑ **Parent:** [Capillary instability of an annular liquid lining](#capillary-instability-of-an-annular-liquid-lining)

For [insoluble surfactant](#insoluble-surfactant) with $\sigma=\sigma_0-A\Gamma$ and positive base tension, let $q=k^2a^2$, $\lambda=h_0^3(\sigma_0-A\Gamma_0)/(3\mu a^4)$ and $\alpha=h_0A\Gamma_0/(\mu a^2)$. The coupled film-height and advected-[surfactant](#surfactant) amplitudes give the displayed growth equation. The unstable band remains $0<q<1$. Weak [surfactant](#surfactant) elasticity gives $\beta_{\max}=\lambda/4-3\alpha/8+O(\alpha^2/\lambda)$; strong elasticity gives $\beta_{\max}\sim\lambda/16$. The [Marangoni stress](#marangoni-effect) reduces tangential surface motion; strong elasticity reduces lubrication mobility to the value for an effectively immobile interface.

<h3 id="young-laplace-equation">Young–Laplace equation</h3>

↑ **Parent:** [Surface tension](#surface-tension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Young–Laplace_equation)

The Young–Laplace equation gives the pressure jump across an interface as $\Delta p=\gamma\kappa$, with the sign set by the chosen normal and curvature convention.

<h4 id="gibbs-thomson-relation">Gibbs--Thomson relation</h4>

↑ **Parent:** [Young–Laplace equation](#young-laplace-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gibbs--Thomson_relation)

The Gibbs--Thomson relation shifts the equilibrium chemical potential or composition at a curved interface by an amount proportional to its mean curvature. Small droplets therefore have a larger equilibrium solubility than flat interfaces.

##### Curvature-induced melting-temperature depression

↑ **Parent:** [Gibbs--Thomson relation](#gibbs-thomson-relation)

Curvature depresses the equilibrium [melting](critical-phenomenon.md#melting) [temperature](thermodynamics.md#temperature) of solid convex into liquid. Here $\mathcal K$ is the sum of [principal curvatures](second-fundamental-form.md#principal-curvature), equal to twice a common convention for [mean curvature](second-fundamental-form.md#mean-curvature), and $T_m$ is absolute [temperature](thermodynamics.md#temperature). The coefficient uses [solid-liquid surface energy](geophysics.md#solid-liquid-surface-energy), [mass density](#density) and [latent heat](thermodynamics.md#latent-heat). This stabilizes fine corrugations of a [solidification](critical-phenomenon.md#freezing) front.

### Capillary length

↑ **Parent:** [Surface tension](#surface-tension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Capillary_length)

The capillary length is the scale at which hydrostatic pressure and capillary pressure balance.

### Dynamic meniscus

↑ **Parent:** [Surface tension](#surface-tension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dynamic_meniscus)

A dynamic meniscus is a curved transition region joining a moving thin film to a bulk fluid reservoir.

### Capillary wave

↑ **Parent:** [Surface tension](#surface-tension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Capillary_wave)

A capillary wave is a free-surface wave for which surface tension supplies an essential restoring stress.

#### Deep-water capillary-wave dispersion relation

↑ **Parent:** [Capillary wave](#capillary-wave)

For a capillary wave on deep water with surface tension $T$ and density $\rho$, the dispersion relation is

$$
\omega(k)=S|k|^{3/2},
\qquad
S=\sqrt{T/\rho}.
$$

Its group velocity is $(3S/2)|k|^{1/2}$ in the direction of the wavevector.

##### Surface response to a localized impulsive velocity

↑ **Parent:** [Deep-water capillary-wave dispersion relation](#deep-water-capillary-wave-dispersion-relation)

If an initially flat one-dimensional surface receives velocity $-W$ on $|x|<\epsilon$ and zero velocity elsewhere, its linear capillary-wave response is

$$
\eta(x,t)=-\frac{2W}{\pi S}
\int_0^\infty
\frac{\sin(k\epsilon)\sin(Sk^{3/2}t)\cos(kx)}{k^{5/2}}\,dk.
$$

###### Stationary-phase wake of an impulsive capillary wave

↑ **Parent:** [Surface response to a localized impulsive velocity](#surface-response-to-a-localized-impulsive-velocity)

Along $x=Vt>0$, if $\epsilon V^2/S^2\ll1$, the stationary wavenumber $k_0=4V^2/(9S^2)$ obeys $k_0\epsilon\ll1$. The [one-dimensional stationary-phase formula](analysis.md#one-dimensional-stationary-phase-formula) then gives

$$
\eta(x,t)\sim
\frac{W\epsilon S t^2}{x^{5/2}}
\frac9{2\sqrt\pi}
\sin\left(\frac{4x^3}{27S^2t^2}-\frac\pi4\right).
$$

Only the integrated initial velocity $-2W\epsilon$ survives in this long-wave far field.

#### Diffusion-limited relaxation of an interface

↑ **Parent:** [Capillary wave](#capillary-wave)

For a conserved scalar order parameter, a sinusoidal interface perturbation of wavenumber $q$ creates a harmonic chemical-potential field extending a distance $|q|^{-1}$ into each phase. Surface tension then produces a relaxation rate proportional to $-|q|^3$.

## Body force

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Body_force)

A body force acts throughout a fluid volume. Gravity and electromagnetic forces are standard examples; a body force per unit mass $f$ contributes $\rho f$ to the momentum equation.

### Elastic force dipole

↑ **Parent:** [Body force](#body-force)

Opposite forces separated along the unit direction $\mathbf e$, with fixed force times separation $D$, have this distributional [body force](#body-force) limit. Its net force is zero. A symmetric [seismic moment tensor](wave-equation.md#seismic-moment-tensor) is a sum of such dipoles along its principal directions.

## Hydrostatic pressure

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hydrostatic_pressure)

Hydrostatic pressure has gradient equal to fluid density times gravity.

### Hydrostatic approximation

↑ **Parent:** [Hydrostatic pressure](#hydrostatic-pressure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hydrostatic_approximation)

The hydrostatic approximation neglects vertical acceleration relative to gravity and vertical pressure gradients. It reduces vertical momentum balance to $p_z=-\rho g$.

#### Hydrostatic balance

↑ **Parent:** [Hydrostatic approximation](#hydrostatic-approximation)

Vertical [pressure gradient](#pressure-gradient) balances gravitational force per unit volume. Subtracting the resting hydrostatic state and using [kinematic pressure](thermodynamics.md#kinematic-pressure) gives $p'_z=b'$ for a [Boussinesq approximation](geophysical-fluid-dynamics.md#boussinesq-approximation) buoyancy anomaly. The approximation neglects vertical [acceleration](classical-mechanics.md#acceleration); this diagnostic relation is what couples [buoyancy perturbation](#buoyancy-perturbation) to the vertical pressure profile.

## Volumetric flow rate

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Volumetric_flow_rate)

The volumetric flow rate is the volume of fluid crossing a section per unit time, $Q=\int_A\mathbf u\mathbin\cdot\mathbf n\,dA$.

### Mass flow rate

↑ **Parent:** [Volumetric flow rate](#volumetric-flow-rate)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mass_flow_rate)

The mass flow rate through an oriented cross-section is the integral of [mass density](#density) times normal [velocity](classical-mechanics.md#velocity). For constant density it is density times the [volumetric flow rate](#volumetric-flow-rate). In a steady pipe without leaks, [conservation of mass](continuum-mechanics.md#mass-conservation) makes this rate independent of cross-section.

### Volume flux per unit width

↑ **Parent:** [Volumetric flow rate](#volumetric-flow-rate)

For a flow invariant in one horizontal direction, the [volume flux](#volumetric-flow-rate) per unit width is the [velocity](classical-mechanics.md#velocity) integrated across the flow depth. It has dimensions of area per unit time.

### Discharge coefficient

↑ **Parent:** [Volumetric flow rate](#volumetric-flow-rate)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Discharge_coefficient)

A discharge coefficient multiplies an ideal inviscid opening-flow rate to represent contraction and dissipative losses. Its value depends on the opening geometry and flow regime.

## Potential flow

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Potential_flow)

Potential flow is irrotational flow represented as the gradient of a scalar potential.

### Corner sink in a semi-infinite channel

↑ **Parent:** [Potential flow](#potential-flow)

For unit channel width, [incompressible flow](#incompressible-flow) towards a corner withdrawal point has $\psi=0$ on the lower wall and $\psi=-m$ on the upper and left walls, with $\psi\to-my$ far downstream. For [irrotational flow](#irrotational-flow), [separation of variables](partial-differential-equation.md#separation-of-variables) gives the displayed harmonic correction: the Fourier sine coefficients of $-m(1-y)$ are $-2m/(n\pi)$. Near the corner, $\psi\sim-2m\theta/\pi$ and radial velocity is $-2m/(\pi r)$, whose integrated inward flux across a quarter-circle is $m$.

### Rankine half-body

↑ **Parent:** [Potential flow](#potential-flow)

The region bounded by the dividing [streamlines](#streamline) of a two-dimensional [point source](#point-source) superposed on uniform flow. Its stagnation point is $-Q/(2\pi U)$ upstream and its far downstream width is $Q/U$. The boundary encloses fluid originating at the source rather than a rigid obstacle; the upstream stagnation point is reached only asymptotically by the upstream source trajectory.

### Radial source flow

↑ **Parent:** [Potential flow](#potential-flow)

A two-dimensional incompressible line source with area flux $Q$ has radial [velocity](classical-mechanics.md#velocity) $Q/(2\pi r)$, obtained from flux conservation around a circle. It is irrotational away from the source, with potential $(Q/(2\pi))\ln r$. For a circular expanding interface, $Q=2\pi aa_t$ and $u_r=aa_t/r$, whose radial strain is $-aa_t/r^2$. That strain supplies a normal viscous stress even though the [velocity](classical-mechanics.md#velocity) is a potential flow.

### Potential dipole

↑ **Parent:** [Potential flow](#potential-flow)

A potential dipole in three dimensions is the [potential flow](#potential-flow) $\mathbf u=\nabla\phi$ with $\phi=\mathbf d\cdot\mathbf x/r^3$. Away from the origin its potential is a [harmonic function](partial-differential-equation.md#harmonic-function), so it is also a constant-[pressure](thermodynamics.md#pressure) [Stokes flow](stokes-flow.md). Its [velocity](classical-mechanics.md#velocity) decays as $r^{-3}$ and its [vorticity](#vorticity) is zero. It is distinct from a [stresslet](stokes-flow.md#force-dipole-flow), whose leading [velocity](classical-mechanics.md#velocity) decays as $r^{-2}$.

### Point source

↑ **Parent:** [Potential flow](#potential-flow)

A two-dimensional point source of strength $q$ has velocity potential $\phi=q\log r/(2\pi)$ and outward velocity $q\mathbf e_r/(2\pi r)$. Every closed contour enclosing it has volume flux $q$.

#### Source dipole

↑ **Parent:** [Point source](#point-source)

A source dipole is the limit of an equal source and sink brought together with their source-strength times separation vector fixed at $\mathbf M$. Differentiating the [three-dimensional point source](#three-dimensional-point-source) field gives $\mathbf u=-(\mathbf M\cdot\nabla)[\mathbf r/(4\pi r^3)]$. It has [velocity potential](#velocity-potential) $-\mathbf M\cdot\mathbf r/(4\pi r^3)$, zero total [volume flux](#volumetric-flow-rate), and $r^{-3}$ far-field decay. Unlike a [stresslet](stokes-flow.md#force-dipole-flow), it is an irrotational potential singularity rather than a [force-dipole flow](stokes-flow.md#force-dipole-flow).

#### Three-dimensional point source

↑ **Parent:** [Point source](#point-source)

A point injection of volume at rate $Q$ produces the displayed radial [potential flow](#potential-flow) in three dimensions. Its [velocity potential](#velocity-potential) is $-Q/(4\pi r)$, and every enclosing [sphere](geometry-and-topology.md#sphere) has outward [volume flux](#volumetric-flow-rate) $Q$. The [divergence](calculus.md#divergence) vanishes away from the source and is $Q$ times the three-dimensional [Dirac delta](distribution-theory.md#dirac-delta-function) distribution at it. The field is also a [Stokes flow](stokes-flow.md) with constant [pressure](thermodynamics.md#pressure) away from its singularity.

#### Hydrodynamic attraction of a plane wall to a point source

↑ **Parent:** [Point source](#point-source)

An incompressible [point source](#point-source) of volume [flux](physics.md#flux) $Q$ at height $a$ above an impermeable plane has [velocity potential](#velocity-potential) $\phi=-Q(1/r_++1/r_-)/(4\pi)$, with an equal image source below the plane. On the wall, $u_s=Qs/[2\pi(s^2+a^2)^{3/2}]$. The [Bernoulli equation](#bernoulli-equation) gives $p-p_\infty=-\rho Q^2s^2/[8\pi^2(s^2+a^2)^3]$. Integrating the [pressure](thermodynamics.md#pressure) deficit over the plane gives the displayed attraction force relative to ambient [pressure](thermodynamics.md#pressure). If source strength instead denotes the coefficient $Q/(4\pi)$ of radial inverse-square velocity, the force is $\pi\rho m^2/a^2$.

### Sink flow in a sector

↑ **Parent:** [Potential flow](#potential-flow)

A line sink of strength $\alpha Q$ at the vertex of a sector $0<\theta<\alpha$ produces the irrotational outer flow

$$
u_r=-\frac Qr,
\qquad u_\theta=0,
\qquad \psi=-Q\theta.
$$

It satisfies no penetration at the radial walls but violates no slip there, so viscous boundary layers form along both walls.

#### Similarity solution for a sink-flow boundary layer

↑ **Parent:** [Sink flow in a sector](#sink-flow-in-a-sector)

Near a radial wall, let $x$ measure distance from the sink along the wall and $y$ point into the fluid. With

$$
\delta=x\sqrt{\frac\nu Q},
\qquad
\eta=\frac y\delta,
\qquad
\psi=\sqrt{\nu Q}\,f(\eta),
$$

the [Prandtl boundary-layer equation](viscous-fluid-flow.md#prandtl-boundary-layer-equation) reduces to

$$
f'''=1-(f')^2,
\qquad
f(0)=f'(0)=0,
\qquad
f'(\infty)=-1.
$$

One physical solution has

$$
f'(\eta)=\frac{5-\cosh(\sqrt2\eta+c)}{1+\cosh(\sqrt2\eta+c)},
\qquad
c=\operatorname{arcosh}5.
$$

### Potential flow around a translating sphere

↑ **Parent:** [Potential flow](#potential-flow)

For a sphere of radius $a$ translating at speed $U$ along the polar axis through fluid at rest at infinity, the laboratory-frame potential is

$$
\phi=-\frac{Ua^3}{2r^2}\cos\theta.
$$

It gives $u_r=Ua^3\cos\theta/r^3$ and $u_\theta=Ua^3\sin\theta/(2r^3)$.

### Spherically symmetric incompressible radial flow

↑ **Parent:** [Potential flow](#potential-flow)

For radial flow outside a sphere, [incompressible flow](#incompressible-flow) makes

$$
Q(t)=4\pi r^2u_r(r,t)
$$

independent of radius. Its velocity potential is $\phi=-Q/(4\pi r)$.

#### Rayleigh equation for an inviscid spherical bubble

↑ **Parent:** [Spherically symmetric incompressible radial flow](#spherically-symmetric-incompressible-radial-flow)

In radial [potential flow](#potential-flow) outside a spherical bubble, [incompressibility](#incompressible-flow) and the moving-boundary condition give $u_r=R^2\dot R/r^2$ and $\phi=-R^2\dot R/r$. The [Unsteady Bernoulli equation](#unsteady-bernoulli-equation), with its gauge fixed at infinity, yields the displayed radius equation when surface tension and viscosity are neglected. Pressure continuity at the interface identifies the liquid pressure with the gas pressure $p_g$. The vacuum special case is [Rayleigh collapse of a spherical cavity](#rayleigh-collapse-of-a-spherical-cavity).

##### Pressure-work energy balance for a spherical bubble

↑ **Parent:** [Rayleigh equation for an inviscid spherical bubble](#rayleigh-equation-for-an-inviscid-spherical-bubble)

For spherical expansion in an unbounded [incompressible flow](#incompressible-flow), continuity gives $u_r=R^2\dot R/r^2$. Integrating the [kinetic energy](classical-mechanics.md#kinetic-energy) outside the bubble gives $K=2\pi\rho R^3\dot R^2$. The [Rayleigh equation for an inviscid spherical bubble](#rayleigh-equation-for-an-inviscid-spherical-bubble) then yields $\dot K=(p_b-p_\infty)\dot V$, where $V=4\pi R^3/3$. With $p_b=p_\infty V_0/V$ and constant $p_\infty$, integration gives $K-K_0=p_\infty[V_0\log(V/V_0)-V+V_0]$. This neglects [viscosity](#dynamic-viscosity), [surface tension](#surface-tension) and external body-force differences, which contribute additional terms in other bubble models.

##### First integral of polytropic spherical-bubble motion

↑ **Parent:** [Rayleigh equation for an inviscid spherical bubble](#rayleigh-equation-for-an-inviscid-spherical-bubble)

For gas pressure depending only on radius and initial speed zero, multiplying the [Rayleigh equation for an inviscid spherical bubble](#rayleigh-equation-for-an-inviscid-spherical-bubble) by $2R^2\dot R$ integrates to the displayed identity. A polytropic pressure $p_g=K/R^{3\kappa}$ gives elementary power integrals when $\kappa\ne1$, and a logarithm when $\kappa=1$. Turning radii are the positive zeros of this first integral. At $\kappa=2$ and $p_g(R_0)=p_\infty/2$, they are $R_0$ and $R_0/2^{1/3}$; the inward and outward accelerations at them have opposite signs, giving bounded undamped oscillation in the [ideal](commutative-algebra.md#ideal) model.

#### Rayleigh-Plesset equation

↑ **Parent:** [Spherically symmetric incompressible radial flow](#spherically-symmetric-incompressible-radial-flow)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rayleigh–Plesset_equation)

The [Rayleigh-Plesset equation](#rayleigh-plesset-equation) balances the radial inertia of an incompressible liquid around a spherical bubble against internal and ambient [pressure](thermodynamics.md#pressure), [surface tension](#surface-tension) and [viscous stress](#viscous-stress-tensor). Removing the last two effects and setting the bubble pressure to zero gives the following vacuum-collapse case.

##### Rayleigh collapse of a spherical cavity

↑ **Parent:** [Rayleigh-Plesset equation](#rayleigh-plesset-equation)

A vacuum cavity of radius $a(t)$ in an infinite inviscid incompressible fluid of density $\rho$ and far-field pressure $p_0$ obeys

$$
a\ddot a+\frac32\dot a^2=-\frac{p_0}{\rho}.
$$

If $a(0)=a_0$ and $\dot a(0)=0$, its collapsing branch satisfies

$$
\dot a=-\sqrt{\frac{2p_0}{3\rho}
\left(\frac{a_0^3}{a^3}-1\right)}.
$$

### Squeezing wedge flow

↑ **Parent:** [Potential flow](#potential-flow)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Squeezing_wedge_flow)

Inviscid flow between closing hinged plates is a quadratic potential flow that expels fluid radially.

## Free surface

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Free_surface)

A free surface is a fluid boundary whose position is part of the solution and whose traction is prescribed by the adjoining medium. Its motion obeys a [kinematic boundary condition](#kinematic-boundary-condition), while its pressure or stress supplies a dynamic boundary condition.

### Surface gravity wave

↑ **Parent:** [Free surface](#free-surface)

A surface gravity wave is a free-surface oscillation restored by gravity. In inviscid deep water its angular frequency and horizontal wavenumber satisfy $\omega^2=gk$.

#### Surface-wave breaking

↑ **Parent:** [Surface gravity wave](#surface-gravity-wave)

A [surface gravity wave](#surface-gravity-wave) breaks when its smooth free-surface motion becomes unstable and overturns or forms a strongly dissipative front. In the nondispersive [shallow-water approximation](physics.md#shallow-water-approximation), intersecting compressive [characteristic curves](partial-differential-equation.md#characteristic-curve) signal failure of a smooth [simple wave](compressible-flow.md#simple-wave); a [hydraulic bore](physics.md#hydraulic-bore) replaces it at the integral-model level. Dispersion can instead produce an oscillatory bore, while physical breaking involves turbulence and energy loss beyond the inviscid equations.

#### Normal modes of surface gravity waves in a rectangular tank

↑ **Parent:** [Surface gravity wave](#surface-gravity-wave)

For a tank with side lengths $a,b$, depth $h$, impermeable walls and no surface tension, the small-amplitude surface modes have horizontal factors $\cos(m\pi x/a)\cos(n\pi y/b)$ and $k_{mn}^2=(m\pi/a)^2+(n\pi/b)^2$. The velocity potential has vertical factor $\cosh(k_{mn}(z+h))$. Combining the linearized kinematic and dynamic conditions on the undisturbed surface gives $\omega_{mn}^2=gk_{mn}\tanh(k_{mn}h)$. The uniform $m=n=0$ elevation is excluded when the total water volume is fixed.

#### Power-law near-shore ray asymptotics

↑ **Parent:** [Surface gravity wave](#surface-gravity-wave)

For depth $h=\alpha x^p$ with $p>0$, stationary [surface gravity waves](#surface-gravity-wave) conserve frequency $\omega$ and alongshore wavenumber $K$. Near shore their dispersion becomes $\omega^2\sim g\kappa^2h$, so $\kappa\sim\omega x^{-p/2}/\sqrt{g\alpha}$. The shoreward ray has $y'\sim-K\sqrt{g\alpha}x^{p/2}/\omega$, giving the displayed integrated scaling. Rays approach normally, while equal-phase crests approach parallel to the shore and their shore-normal spacing shrinks as $x^{p/2}$. These are asymptotics within the ray approximation; for $p<2$, its slow-variation assumption eventually fails arbitrarily close to the endpoint.

#### Wave fetch

↑ **Parent:** [Surface gravity wave](#surface-gravity-wave)

Wave fetch is the distance over which wind acts on an uninterrupted water surface to generate waves. Growth also depends on wind speed and duration. A [polynya](geophysics.md#polynya) can provide a local fetch inside otherwise extensive [sea ice](geophysics.md#sea-ice).

#### Radiation stress

↑ **Parent:** [Surface gravity wave](#surface-gravity-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radiation_stress)

The excess depth-integrated, time-averaged [momentum flux](physics.md#momentum-flux) of a [surface gravity wave](#surface-gravity-wave) is its radiation stress. In deep water $c_g/c_p=1/2$, so $S_{xx}=\mathcal E/2=\rho_wga^2/4$. The force per transverse width on a reflecting object is the incident plus reflected minus transmitted radiation stress. Reflection increases force because the reflected wave carries momentum in the opposite direction.

#### Surface-gravity-wave energy

↑ **Parent:** [Surface gravity wave](#surface-gravity-wave)

A linear [deep-water gravity wave](#deep-water-gravity-wave) of surface-displacement amplitude $a$ has equal mean [kinetic energy](classical-mechanics.md#kinetic-energy) and [potential energy](classical-mechanics.md#potential-energy), and total mean [energy](classical-mechanics.md#energy) per horizontal area $\mathcal E=\rho_wga^2/2$. Its energy transport speed is the [group velocity](wave-equation.md#group-velocity). This amplitude is half the crest-to-trough height.

#### Wave steepness

↑ **Parent:** [Surface gravity wave](#surface-gravity-wave)

The dimensionless product of surface-wave amplitude and [wavenumber](wave-equation.md#wavenumber), $ka$, measures orbital displacement relative to the wavelength. Small [wave steepness](#wave-steepness) permits a [Taylor expansion](calculus.md#taylor-expansion) of the velocity sampled by moving parcels. For a [deep-water gravity wave](#deep-water-gravity-wave), orbital amplitudes and the local steepness decrease exponentially with depth.

#### Airy wave theory

↑ **Parent:** [Surface gravity wave](#surface-gravity-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Airy_wave_theory)

[Airy wave theory](#airy-wave-theory) linearizes the motion of small-amplitude [surface gravity waves](#surface-gravity-wave) in an inviscid, incompressible, irrotational fluid. At depth $h$, its dispersion relation is $\omega^2=gk\tanh(kh)$; deep water is the limit $kh\to\infty$.

##### Deep-water gravity wave

↑ **Parent:** [Airy wave theory](#airy-wave-theory)

A small-amplitude deep-water wave with surface elevation $\eta=Ae^{i(kx-\omega t)}$ has dispersion relation $\omega^2=gk$ and a velocity potential that decays as $e^{kz}$ below the surface.

###### Dispersive swell source inversion

↑ **Parent:** [Deep-water gravity wave](#deep-water-gravity-wave)

For an impulsive distant source of [deep-water gravity waves](#deep-water-gravity-wave), a component of period $T$ travels at [group velocity](wave-equation.md#group-velocity) $gT/(4\pi)$. Its arrival at distance $L$ obeys the displayed law, so inverse period increases linearly with arrival time. Two arrivals determine both $L$ and $t_0$. Finite source duration, currents, refraction and passage through [sea ice](geophysics.md#sea-ice) can invalidate the simple inversion.

###### Viscous decay of a deep-water gravity wave

↑ **Parent:** [Deep-water gravity wave](#deep-water-gravity-wave)

For small kinematic viscosity $\nu$, the mean viscous dissipation per unit horizontal area is $2\rho\nu gk^2|A|^2$. Since the mean wave energy is $\rho g|A|^2/2$, the amplitude obeys

$$
\frac{d|A|}{dt}=-2\nu k^2|A|,
\qquad
|A(t)|=|A(0)|e^{-2\nu k^2t}.
$$

###### Linearized free-surface boundary conditions

↑ **Parent:** [Deep-water gravity wave](#deep-water-gravity-wave)

For small-amplitude potential flow beneath a mean surface $z=0$, the linearized kinematic and dynamic conditions are

$$
\eta_t=\phi_z,
\qquad
\phi_t+g\eta=-\frac{p}{\rho}
\qquad(z=0).
$$

###### Rectangular standing surface-gravity mode

↑ **Parent:** [Linearized free-surface boundary conditions](#linearized-free-surface-boundary-conditions)

In a rectangular box with Neumann side walls, a horizontal mode

$$
\cos\frac{m\pi x}{L_x}\cos\frac{n\pi y}{L_y}
$$

has horizontal wavenumber $k=[(m\pi/L_x)^2+(n\pi/L_y)^2]^{1/2}$, depth dependence $e^{kz}$ in infinitely deep fluid, and natural frequency $\Omega=\sqrt{gk}$.

###### Resonance of a pressure-forced rectangular surface-gravity mode

↑ **Parent:** [Rectangular standing surface-gravity mode](#rectangular-standing-surface-gravity-mode)

Pressure forcing of one rectangular free-surface mode reduces its amplitude to

$$
H''+gkH=-\frac{kp_0}{\rho}\cos(\omega t).
$$

At $\omega=\sqrt{gk}$, the inviscid undamped response contains $t\sin(\omega t)$ and grows without bound in the linear model.

## Streamfunction in polar coordinates

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Streamfunction_in_polar_coordinates)

For planar incompressible flow, a streamfunction satisfies

$$
u_r=\frac1r\frac{\partial\psi}{\partial\theta},
\qquad
u_\theta=-\frac{\partial\psi}{\partial r}.
$$

## Stagnation point

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stagnation_point)

A stagnation point of a fluid flow is a point at which the [velocity field](#velocity-field) vanishes. For a two-dimensional [streamfunction](#streamfunction-in-polar-coordinates), it is a critical point satisfying both first spatial derivatives of the streamfunction equal to zero.

## Incompressible flow

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Incompressible_flow)

### Rectilinear flow

↑ **Parent:** [Incompressible flow](#incompressible-flow)

A [rectilinear flow](#rectilinear-flow) has velocity everywhere parallel to a fixed direction and independent of the coordinate in that direction, for example $U(y,z)\widehat x$. Its convective acceleration vanishes. A steady incompressible viscous rectilinear flow obeys the linear transverse Poisson equation $\nu\Delta U=\rho^{-1}dp/dx$, rather than an inertia-viscosity balance. This explains Reynolds-number independence of the spatial equation with fixed scaled forcing and boundary data.

### Streamfunction advection bracket

↑ **Parent:** [Incompressible flow](#incompressible-flow)

For the two-dimensional [streamfunction](#stream-function) convention $u=\psi_z$, $w=-\psi_x$, the advective derivative of $\theta$ is $u\theta_x+w\theta_z=J(\psi,\theta)$. This antisymmetric [Jacobian determinant](calculus.md#jacobian-determinant) bracket organizes nonlinear interactions in convection and vorticity equations.

### Cartesian streamfunction

↑ **Parent:** [Incompressible flow](#incompressible-flow)

For a two-dimensional [incompressible flow](#incompressible-flow), a Cartesian streamfunction $\psi$ defines $u=\partial_y\psi$ and $v=-\partial_x\psi$. The continuity equation $u_x+v_y=0$ then holds identically.

### Divergence-free vector field

↑ **Parent:** [Incompressible flow](#incompressible-flow)

A divergence-free vector field satisfies $\nabla\mathbin\cdot u=0$. It preserves volume under its flow, and its transport operator is skew-symmetric when boundary fluxes vanish.

## Streakline

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Streakline)

A streakline at a given time is the locus of all fluid particles that previously passed through one fixed release point.

## Kinematic boundary condition

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kinematic_boundary_condition)

A material fluid boundary has no relative normal flow; at a fixed impermeable graph $y=\eta(x)$ this is $v=u\eta_x$.

### Kinematic boundary condition for a free-surface graph

↑ **Parent:** [Kinematic boundary condition](#kinematic-boundary-condition)

For a free surface $z=\eta(x,y,t)$ and velocity $(u,v,w)$, material conservation of $z-\eta$ gives

$$
w=\eta_t+u\eta_x+v\eta_y=\frac{D\eta}{Dt}
$$

on the surface.

### Linearized boundary condition

↑ **Parent:** [Kinematic boundary condition](#kinematic-boundary-condition)

For a small boundary displacement and weak disturbance, evaluate boundary data on the undisturbed surface and discard products of small quantities.

## Dynamic boundary condition for an inviscid interface

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

At an interface between two inviscid fluids without surface tension, the pressure is continuous. For potential flows of equal density, the [Unsteady Bernoulli equation](#unsteady-bernoulli-equation) therefore equates

$$
\partial_t\phi+\frac12|\nabla\phi|^2
$$

on the two sides, up to a removable function of time.

### Pressure continuity

↑ **Parent:** [Dynamic boundary condition for an inviscid interface](#dynamic-boundary-condition-for-an-inviscid-interface)

For an inviscid interface with no [surface tension](#surface-tension), continuity of normal [traction](continuum-mechanics.md#traction) reduces to continuity of [pressure](thermodynamics.md#pressure). The same condition is used in a sharp [Darcy law](porous-media-flow.md#darcy-law) interface model that neglects [capillary pressure](#capillary-pressure) and resolved interfacial viscous normal [stress](continuum-mechanics.md#stress). For a general viscous interface, continuity of normal [traction](continuum-mechanics.md#traction) balances the full [stress](continuum-mechanics.md#stress) [tensor](linear-algebra.md#tensor); it does not by itself imply continuity of [pressure](thermodynamics.md#pressure).

## Wake (physics)

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wake_(physics))

A fluid wake is the region downstream of a body or velocity defect in which the flow differs from the surrounding stream.

## Shear layer

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A shear layer is a thin region across which the tangential [velocity](classical-mechanics.md#velocity) changes rapidly. In an inviscid idealization it can collapse to a [vortex sheet](#vortex-sheet).

### Vortex sheet

↑ **Parent:** [Shear layer](#shear-layer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vortex_sheet)

A vortex sheet is a surface across which tangential velocity is discontinuous while normal velocity remains continuous.

#### Cylindrical vortex sheet

↑ **Parent:** [Vortex sheet](#vortex-sheet)

A cylindrical vortex sheet is a vortex sheet supported on a cylindrical surface. Azimuthal Fourier disturbances have harmonic velocity potentials proportional to $r^m$ inside and $r^{-m}$ outside.

#### Kelvin-Helmholtz instability

↑ **Parent:** [Vortex sheet](#vortex-sheet)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kelvin–Helmholtz_instability)

For a planar vortex sheet separating equal-density streams of velocities $U_1$ and $U_2$, a mode of nonzero [wavenumber](wave-equation.md#wavenumber) $k$ has complex growth exponent

$$
\sigma=-ik\frac{U_1+U_2}{2}
\mathbin{\pm}\frac{|k|\,|U_1-U_2|}{2}.
$$

One sign has positive [growth rate](wave-equation.md#growth-rate), so every nonzero wavenumber is unstable in the inviscid zero-thickness model.

##### Bending-membrane Kelvin-Helmholtz dispersion relation

↑ **Parent:** [Kelvin-Helmholtz instability](#kelvin-helmholtz-instability)

For equal fluid density $\rho$ on opposite sides of a massless flat membrane, a velocity jump $U$ and bending pressure jump $\beta\eta_{xxxx}$ with $\beta>0$, a mode $e^{ikx+\sigma t}$ satisfies

$$
(\sigma+ikU/2)^2=U^2k^2/4-\beta|k|^5/(2\rho).
$$

The decaying upper and lower perturbation potentials are $A_+e^{-|k|y}$ and $A_-e^{|k|y}$. Their kinematic conditions are $-|k|A_+=(\sigma+ikU)\eta$ and $|k|A_-=\sigma\eta$. The linearized [Bernoulli equation](#bernoulli-equation) gives $p_- -p_+=-\rho[\sigma^2+(\sigma+ikU)^2]\eta/|k|$. Equating it to the bending pressure yields the relation. Bending stabilizes $|k|^3\ge\rho U^2/(2\beta)$. The maximum positive growth is at $|k|^3=\rho U^2/(5\beta)$ and is $|U|\,|k|\sqrt{3/20}$.

##### Kelvin-Helmholtz dispersion relation with gravity

↑ **Parent:** [Kelvin-Helmholtz instability](#kelvin-helmholtz-instability)

Two deep layers of [incompressible flow](#incompressible-flow) with upper [mass density](#density) $\rho_1$, lower [mass density](#density) $\rho_2$, and tangential [velocities](classical-mechanics.md#velocity) $U_1,U_2$ have this [dispersion relation](wave-equation.md#dispersion-relation) when [surface tension](#surface-tension) is absent. Decaying [velocity potentials](#velocity-potential) and the linearized [kinematic boundary condition](#kinematic-boundary-condition) determine their amplitudes; the [dynamic boundary condition for an inviscid interface](#dynamic-boundary-condition-for-an-inviscid-interface) gives the displayed relation. For $k>0$ the squared departure of the [phase velocity](wave-equation.md#phase-velocity) $c$ from the density-weighted mean [velocity](classical-mechanics.md#velocity) is $g(\rho_2-\rho_1)/[k(\rho_1+\rho_2)]-\rho_1\rho_2(U_1-U_2)^2/(\rho_1+\rho_2)^2$. A negative value gives [Kelvin-Helmholtz instability](#kelvin-helmholtz-instability) despite stable [density stratification](gravity-wave.md#density-stratification).

##### Top-hat planar jet

↑ **Parent:** [Kelvin-Helmholtz instability](#kelvin-helmholtz-instability)

A top-hat planar jet has one constant streamwise velocity in a layer and another constant velocity outside it. In the inviscid model, the two layer boundaries are parallel [vortex sheets](#vortex-sheet).

###### Varicose mode of a planar jet

↑ **Parent:** [Top-hat planar jet](#top-hat-planar-jet)

In a varicose mode, the upper and lower jet interfaces move in opposite directions, so the jet thickness varies while its centreline remains fixed.

###### Sinuous mode of a planar jet

↑ **Parent:** [Top-hat planar jet](#top-hat-planar-jet)

In a sinuous mode, the upper and lower jet interfaces move in the same direction, so the jet centreline bends while its thickness is unchanged to first order.

###### Equal-density top-hat planar-jet dispersion relation

↑ **Parent:** [Top-hat planar jet](#top-hat-planar-jet)

For a jet of velocity $U$ occupying $|y|<h$ in stationary fluid of the same density, disturbances proportional to $e^{ikx+\sigma t}$ satisfy

$$
\sigma^2+\coth(|k|h)(\sigma+ikU)^2=0
$$

for a [varicose mode of a planar jet](#varicose-mode-of-a-planar-jet), and

$$
\sigma^2+\tanh(|k|h)(\sigma+ikU)^2=0
$$

for a [sinuous mode of a planar jet](#sinuous-mode-of-a-planar-jet). Both have unstable growth rate

$$
\operatorname{Re}\sigma
=\frac{|kU|}{2}\sqrt{1-e^{-4|k|h}}.
$$

###### Equality of top-hat jet parity growth rates

↑ **Parent:** [Equal-density top-hat planar-jet dispersion relation](#equal-density-top-hat-planar-jet-dispersion-relation)

For a [top-hat planar jet](#top-hat-planar-jet) in stationary fluid of the same [mass density](#density), odd and even [velocity potentials](#velocity-potential) have the same [temporal growth rate](wave-equation.md#growth-rate). Put $s=\tanh(|k|L)$. Their [dispersion relations](wave-equation.md#dispersion-relation) use $s$ and $1/s$, but $\sqrt{s}/(1+s)=\sqrt{1/s}/(1+1/s)$. Their real [phase velocities](wave-equation.md#phase-velocity) are respectively $Vs/(1+s)$ and $V/(1+s)$. The common [growth rate](wave-equation.md#growth-rate) is strictly below $|kV|/2$ for finite $|k|L>0$, approaching the isolated [vortex sheet](#vortex-sheet) value when the sheets decouple.

##### Finite-depth vortex-sheet dispersion relation

↑ **Parent:** [Kelvin-Helmholtz instability](#kelvin-helmholtz-instability)

For an equal-density vortex sheet a distance $h$ above a rigid wall, with lower and upper base velocities $U$ and zero, a mode $e^{i(kx-\omega t)}$ satisfies

$$
(\omega-kU)^2\coth(|k|h)+\omega^2=0.
$$

The wall changes the inertia of the lower perturbation through the factor $\coth(|k|h)$.

## Compressible flow

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](compressible-flow.md)

## Linear acoustics

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](linear-acoustics.md)

## Astrophysical fluid dynamics

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](astrophysical-fluid-dynamics.md)

## Geophysical fluid dynamics

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](geophysical-fluid-dynamics.md)

## Dispersion of a solute by flow

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

Dispersion of a solute by flow combines molecular diffusion with spatially varying advection, often producing an enhanced large-scale longitudinal diffusivity.

### Irreversible capture of an advecting tracer

↑ **Parent:** [Dispersion of a solute by flow](#dispersion-of-a-solute-by-flow)

A first-order irreversible transfer from fluid concentration $C$ to stored concentration $S$, measured per matching fluid storage volume, obeys the displayed balances. A sustained inlet can produce a stationary decaying fluid profile, but the stored amount then grows rather than becoming stationary. A finite pulse instead has $C\to0$ and a finite final deposit. Decay, desorption or finite adsorption capacity is additional physics, not a consequence of the linear capture term alone.

### Transverse dispersion

↑ **Parent:** [Dispersion of a solute by flow](#dispersion-of-a-solute-by-flow)

Spreading of solute across the mean flow direction through diffusion and pore-scale velocity variations. In a reflecting layer of depth $H$, a constant transverse dispersion coefficient gives mixing time of order $H^2/D_T$. Repeated exchange between different longitudinal speeds produces [Taylor dispersion](#taylor-dispersion) on times long compared with this mixing time.

<h3 id="peclet-number">Péclet number</h3>

↑ **Parent:** [Dispersion of a solute by flow](#dispersion-of-a-solute-by-flow)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Péclet_number)

The Péclet number compares advection over length $L$ at speed $U$ with molecular diffusion of diffusivity $D$.

### Taylor dispersion

↑ **Parent:** [Dispersion of a solute by flow](#dispersion-of-a-solute-by-flow)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Taylor_dispersion)

Taylor dispersion is enhanced longitudinal spreading produced when transverse molecular diffusion repeatedly moves solute between streamlines of different velocity.

#### Longitudinal moment hierarchy for shear transport

↑ **Parent:** [Taylor dispersion](#taylor-dispersion)

For a [passive scalar](#passive-scalar) in a planar [shear flow](#shear-flow) $u(y,t)$, let $m_j(y,t)=\int_{\mathbb R}x^j\chi(x,y,t)\,dx$. Integrating the [advection-diffusion equation](diffusion-equation.md#advection-diffusion-equation) by parts in $x$ gives the displayed hierarchy for $j\geq0$, with negative-index terms omitted. Sufficient decay and finite moments justify the integrations. Insulating walls give [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition) for every moment. Solving the first two equations then determines the long-time growth of the second moment without solving the full scalar field.

##### Oscillating shear dispersion in an insulating channel

↑ **Parent:** [Longitudinal moment hierarchy for shear transport](#longitudinal-moment-hierarchy-for-shear-transport)

For $u=U\cos(\omega t)\sin(\pi y/L)$ on $|y|<L/2$, positive [diffusivity](brownian-motion.md#diffusion-coefficient) $\kappa$, nonzero frequency and insulating walls, a transversely uniform zeroth moment remains constant. Its first moment is proportional to $g(t)\sin(\pi y/L)$, where $g'+ag=U\cos(\omega t)$. The periodic solution is $g=U[a\cos(\omega t)+\omega\sin(\omega t)]/(a^2+\omega^2)$. The [longitudinal moment hierarchy for shear transport](#longitudinal-moment-hierarchy-for-shear-transport) then gives $m_2=2Ktm_0+O(1)$ after both transverse and periodic transients. The spatial average of $\sin^2(\pi y/L)$ is $1/2$ and the time average of $\cos^2(\omega t)$ is $1/2$, producing the factor $1/4$. At exactly zero frequency the steady enhancement is instead $U^2/(2a)$; averaging indefinitely over slow cycles does not commute with setting the frequency to zero.

#### Effective diffusivity of a periodic sinusoidal shear

↑ **Parent:** [Taylor dispersion](#taylor-dispersion)

For a [passive scalar](#passive-scalar) transported by $U(t)\sin(my)$ with transverse period $2\pi/m$, positive [diffusivity](brownian-motion.md#diffusion-coefficient) $\kappa$ and periodic $U$, let $g$ be the unique periodic solution of $g'+\kappa m^2g=U$. A [multiple-scale expansion](differential-equation.md#method-of-multiple-scales) has first corrector $-g(t)\sin(my)\partial_X\overline\chi$. Averaging the next-order equation over the space-time cell gives the displayed longitudinal [diffusion coefficient](brownian-motion.md#diffusion-coefficient). Averaging $gg'+\kappa m^2g^2=Ug$ proves the second form. This is a long-time, long-wavelength effective equation, after transverse and periodic transients have decayed, rather than an exact finite-time closure for arbitrary concentrations.

##### Impulsively kicked sinusoidal shear dispersion

↑ **Parent:** [Effective diffusivity of a periodic sinusoidal shear](#effective-diffusivity-of-a-periodic-sinusoidal-shear)

When velocity consists of impulses $U_1$ spaced by $T$, the periodic corrector jumps by $U_1$ and decays between kicks. With $a=\kappa m^2$, $g(t)=U_1e^{-at}/(1-e^{-aT})$ for $0<t<T$. Integrating $g^2$ in the [effective diffusivity of a periodic sinusoidal shear](#effective-diffusivity-of-a-periodic-sinusoidal-shear) formula yields the displayed result. For $aT\gg1$, independent transverse phases give longitudinal variance $U_1^2/2$ per kick and enhancement $U_1^2/(4T)$. For $aT\ll1$, the enhancement is $U_1^2/(2\kappa m^2T^2)$ to leading order, the steady-shear result for average speed $U_1/T$. The zero-diffusivity limit does not commute with the long-time limit: without transverse diffusion the displacement is ballistic.

#### Taylor dispersion in a parabolic porous-layer velocity profile

↑ **Parent:** [Taylor dispersion](#taylor-dispersion)

For [interstitial velocity](porous-media-flow.md#pore-velocity) $u=6U\xi(1-\xi)$, $\xi=z/h$, reflecting transverse walls and molecular [diffusion](thermodynamics.md#diffusion) $D$, solve $D\chi''=u-U$ with zero mean and zero normal derivative. One solution is $\chi=(Uh^2/D)(\xi^3-\xi^4/2-\xi^2/2+1/60)$. Averaging the [advection-diffusion equation](diffusion-equation.md#advection-diffusion-equation) gives enhancement $-\overline{(u-U)\chi}=D\overline{(\chi')^2}=U^2h^2/(210D)$. The approximation requires transverse equilibration and slowly varying longitudinal concentration.

#### Taylor dispersion in a linear porous-layer velocity profile

↑ **Parent:** [Taylor dispersion](#taylor-dispersion)

For pore velocity $u(y)=2Uy/H$ on $0<y<H$, with reflecting transverse boundaries, solve $D_T\chi''=u-U$, $\chi'(0)=\chi'(H)=0$, $\overline\chi=0$. The [Taylor dispersion](#taylor-dispersion) enhancement is $D_T\overline{(\chi')^2}=U^2H^2/(30D_T)$. Here $U$ is the mean advective pore velocity, not the [Darcy velocity](porous-media-flow.md#darcy-velocity), and $D_L$ is the original longitudinal dispersion. The averaged equation applies after transverse equilibration and on suitably long longitudinal scales.

#### Taylor dispersion in plane Couette flow

↑ **Parent:** [Taylor dispersion](#taylor-dispersion)

For $u(y)=Uy/h$ between reflecting walls at $y=\pm h$, the flow-induced diffusivity is

$$
D_T=\frac{2U^2h^2}{15D}.
$$

## Rheology

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](rheology.md)

## Porous-media flow

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](porous-media-flow.md)

## Reduced gravity

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](reduced-gravity.md)

## Laminar round jet

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A laminar round jet is an axisymmetric momentum-driven flow issuing into otherwise still fluid. Viscous diffusion broadens the jet while its axial momentum flux remains constant.

### Conserved momentum flux of a laminar round jet

↑ **Parent:** [Laminar round jet](#laminar-round-jet)

For axial velocity $w(r,z)$ in the boundary-layer approximation,

$$
M=\int_0^\infty r w^2\,dr
$$

is independent of $z$. If $W$ and $\delta$ are characteristic centre-line speed and width, then $W\delta\sim M^{1/2}$, while the momentum balance gives $W\delta^2\sim\nu z$. Thus

$$
\delta\sim\frac{\nu z}{M^{1/2}},
\qquad
W\sim\frac{M}{\nu z}.
$$

### Similarity solution for a laminar round jet

↑ **Parent:** [Laminar round jet](#laminar-round-jet)

With axisymmetric streamfunction $\psi=\nu z g(r/z)$, the regular normalized similarity profile is

$$
g(\eta)=\frac{12M\eta^2}{32\nu^2+3M\eta^2}.
$$

Its volume flux grows linearly with $z$, expressing [fluid entrainment](#fluid-entrainment).

## Fluid entrainment

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

Fluid entrainment is the incorporation of surrounding fluid into a moving current, jet, or plume. It increases volume flux while diluting transported momentum, buoyancy, or concentration.

### Entrainment velocity

↑ **Parent:** [Fluid entrainment](#fluid-entrainment)

The mean speed, measured normal to a chosen plume or jet boundary, at which ambient fluid enters the turbulent region. The boundary and averaging convention must be specified: this speed is not the plume's axial velocity. In the [Batchelor entrainment hypothesis](turbulent-plume.md#batchelor-entrainment-hypothesis) for a rising [Boussinesq](geophysical-fluid-dynamics.md#boussinesq-approximation) plume, $u_e=\alpha w$, where $\alpha$ is the dimensionless [entrainment coefficient](turbulent-plume.md#entrainment-coefficient) and $w$ the characteristic axial speed. Multiplying by the boundary perimeter gives the entrained [volume flux](#volumetric-flow-rate) per axial length.

### Interfacial power model for entrainment

↑ **Parent:** [Fluid entrainment](#fluid-entrainment)

An interfacial stress $\tau=c_D\rho_lu_I^2$ supplies local stress power $P_I=S\tau u_I$. Assuming a fixed fraction $C_W$ becomes global [potential energy](classical-mechanics.md#potential-energy) gives $\dot E_P=C_WP_I$. Together with [potential energy of two-layer entrainment](#potential-energy-of-two-layer-entrainment), this gives $\dot h=2C_Wc_Du_I^3/(g'h)$. This is an additional local power-transfer closure. The shaft power of a rotating lid is its torque times its prescribed angular speed and need not equal $P_I$. Geometric factors and a constant transfer fraction may be absorbed into the empirical coefficients only when explicitly assumed time-independent.

### Potential energy of two-layer entrainment

↑ **Parent:** [Fluid entrainment](#fluid-entrainment)

In a closed tank of cross-sectional area $S$, entrainment into a uniform upper layer conserves the density deficit $(\rho_l-\rho_u)h$. Thus $B=g'h$ is constant. With depth $z$ increasing downward, gravitational [potential energy](classical-mechanics.md#potential-energy) is $-gS\int_0^H\rho(z)z\,dz=E_*+\rho_lSBh/2$, so its rate of increase is proportional to the rate of deepening. This includes homogenization throughout the upper layer, not merely lifting a thin parcel across the interface.

#### Potential energy of mixed-layer deepening with an initial buoyancy jump

↑ **Parent:** [Potential energy of two-layer entrainment](#potential-energy-of-two-layer-entrainment)

Let an initial upper mixed layer have finite depth $a$, buoyancy $b_1$, and fixed upper boundary; beneath it let $b=b_1-\Delta b+N^2z$ with the initial interface at $z=0$. Homogenization down to $z=-d$ conserves [buoyancy](#buoyancy) and gives mixed buoyancy $b_1-[\Delta b\,d+N^2d^2/2]/(a+d)$. Integrating gravitational [potential energy](classical-mechanics.md#potential-energy) over the initial and final profiles gives the displayed increase per unit area. Its derivative is $\rho_0[\Delta b\,a/2+N^2a d/2+N^2d^2/4]$. Specifying absorbed mixing power is not enough to determine deepening unless the initial depth or an alternative upper-reservoir model is supplied.

### Fixed-energy turbulent mixed layer

↑ **Parent:** [Fluid entrainment](#fluid-entrainment)

In a slowly deepening mixed layer driven by a rotating boundary, a phenomenological balance between energy input, turbulent loss and acceleration of entrained fluid can keep total [kinetic energy](classical-mechanics.md#kinetic-energy) approximately fixed. For a tank of radius $R$ this gives $u^2h=A\Omega^2R^3$, so velocity decreases as $h^{-1/2}$. The closure does not make the speed constant and is an additional physical assumption rather than a direct consequence of [mass conservation](continuum-mechanics.md#mass-conservation).

#### Fixed-energy two-layer entrainment law

↑ **Parent:** [Fixed-energy turbulent mixed layer](#fixed-energy-turbulent-mixed-layer)

For [potential energy of two-layer entrainment](#potential-energy-of-two-layer-entrainment) with constant $B=g'h$, the [fixed-energy turbulent mixed layer](#fixed-energy-turbulent-mixed-layer) assumption gives $u_U^2h=C_K^2\Omega^2R^2h_0$. If $u_I=C_Iu_U$ and the [interfacial power model for entrainment](#interfacial-power-model-for-entrainment) applies with fixed coefficients, integration gives the displayed depth law with $A=5C_Wc_DC_I^3C_K^3\Omega^2R^3/(Bh_0)$. The relation applies only before the layer reaches the tank bottom. Its [interfacial Richardson number](gravity-wave.md#interfacial-richardson-number) $Bd_I/(h u_I^2)$ stays constant for fixed interface thickness, whereas it decreases like $h^{-1}$ in the constant-speed entrainment model.

#### Rotating-disc mixed-layer depth law

↑ **Parent:** [Fixed-energy turbulent mixed layer](#fixed-energy-turbulent-mixed-layer)

With constant interface thickness and the local [entrainment](#fluid-entrainment) exponent $3/2$, the [fixed-energy turbulent mixed layer](#fixed-energy-turbulent-mixed-layer) satisfies $\dot h=C\Omega^4R^6/(N^3\delta^{3/2}h^{7/2})$. Integration gives a linear growth law for $h^{9/2}$. Once an initial-depth offset is negligible, $h/R$ scales as $[\Omega^2R/(N^2\delta)]^{1/3}(\Omega t)^{2/9}$. The law applies before the mixed layer reaches the tank bottom and after the initial forcing transient.

## Turbulent plume

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](turbulent-plume.md)

## Natural ventilation

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Natural_ventilation)

Natural ventilation exchanges indoor and outdoor fluid through openings using pressure differences created by buoyancy or wind.

### Ventilation after a heating reduction

↑ **Parent:** [Natural ventilation](#natural-ventilation)

For an ideal two-layer [natural ventilation](#natural-ventilation) transient following a heating change $Q\mapsto\lambda Q$, let $V_0$ and $\theta_0$ be the initial flow and temperature excess, $s=V_0t/(A_rH)$, $\eta=h/H$, and $x=\eta(1-\theta/\theta_0)$. The integrated buoyancy pressure gives $V/V_0=\sqrt{1-x}$, while [heat](thermodynamics.md#heat) balance gives $x_s=\sqrt{1-x}-\lambda$. A material interface satisfies $\eta_s=\sqrt{1-x}$, so $\eta=x+\lambda s$. For $0<\lambda<1$, $x$ increases toward $1-\lambda^2$ and $\eta_s\geq\lambda$, ensuring finite-time filling of the room. After filling, $y=\theta/\theta_0$ obeys $y_s=\lambda-y^{3/2}$ and tends to $\lambda^{2/3}$. This model assumes well-mixed individual layers, negligible wall heat capacity and a sharp advected interface.

### Well-mixed ventilation temperature balance

↑ **Parent:** [Natural ventilation](#natural-ventilation)

For a distributed [heat](thermodynamics.md#heat) source, a well-mixed interior with [temperature](thermodynamics.md#temperature) excess $\theta$ gains temperature-volume flux $\mathcal H$ and loses $|q|\theta$ by ventilation in either direction. With signed upward throughflow, $q|q|=K_A(G_T\theta\pm W)$, where $G_T=g\alpha_TH_b$ and $W$ is wind [pressure](thermodynamics.md#pressure) divided by [mass density](#density). The plus sign is assisting wind. Steady temperatures satisfy $\theta^2(G_T\theta+W)=\mathcal H^2/K_A$ for assistance, or $\theta^2|G_T\theta-W|=\mathcal H^2/K_A$ for opposition. Direction restrictions must be applied to roots.

#### Opposing-wind ventilation bistability

↑ **Parent:** [Well-mixed ventilation temperature balance](#well-mixed-ventilation-temperature-balance)

For $0<\varepsilon<2/(3\sqrt3)$, the [well-mixed ventilation temperature balance](#well-mixed-ventilation-temperature-balance) has one stable upward-flow [temperature](thermodynamics.md#temperature) and two downward-flow temperatures. The heat-removal curve on the latter interval is $\sqrt{K_A}\theta\sqrt{W-G_T\theta}$, maximal at $2W/(3G_T)$. Its lower-temperature root is stable and its higher-temperature root unstable. The two meet at a [saddle-node bifurcation](dynamical-systems.md#saddle-node-bifurcation). The unstable root separates the basins of the stable wind-dominated and buoyancy-dominated states.

##### Ventilation switching under wind and heating changes

↑ **Parent:** [Opposing-wind ventilation bistability](#opposing-wind-ventilation-bistability)

Increasing wind or reducing heating both reduce the control parameter of [opposing-wind ventilation bistability](#opposing-wind-ventilation-bistability). However, wind moves the reversal threshold $\theta_w=W/G_T$, whereas heating does not. A sufficiently abrupt wind increase can place a hot upward-flow state in the cooler state's basin. Reducing positive heating at fixed wind cannot make an upward-flow state cross $\theta_w$, because its [temperature](thermodynamics.md#temperature) time derivative there is positive. Slow variation follows a persistent stable branch; a fold destroys the cooler branch when wind is weakened or [heat](thermodynamics.md#heat) input increased.

### Effective opening area for pressure-driven ventilation

↑ **Parent:** [Natural ventilation](#natural-ventilation)

An effective opening area may absorb both the discharge coefficient and the factor of two in an orifice law. If $A_e=\sqrt2C_dA_{\rm geom}$, its discharge is $q=A_e\sqrt{\delta p/\rho}$. Two equal openings carrying the same flux share the total [pressure](thermodynamics.md#pressure) drop, so $q^2=A_e^2\Delta p/(2\rho)$. They do not share equal drops when an internal volume source makes their fluxes unequal. State the effective-area convention before comparing numerical factors in [natural ventilation](#natural-ventilation) models.

### Displacement ventilation

↑ **Parent:** [Natural ventilation](#natural-ventilation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Displacement_ventilation)

Displacement ventilation supplies relatively cool air at low level and removes warmer air at high level. In the ideal two-layer model, buoyant plumes feed a warm upper layer above a sharp density interface while the supply occupies the lower layer.

#### Plume-fed doorway ventilation

↑ **Parent:** [Displacement ventilation](#displacement-ventilation)

For a [pure plume](turbulent-plume.md#pure-plume) with $g'_p=\gamma B^{2/3}z^{-5/3}$, a steady sharp interface at $z_i$ has $Q_p=B^{1/3}z_i^{5/3}/\gamma$ and warm-layer [reduced gravity](reduced-gravity.md) $g'=B/Q_p$. A freely discharging upper doorway of height $D$ and width $W$ has available head $D-z_i$. Equating plume supply to the [broad-crested weir](reduced-gravity.md#broad-crested-weir) flux gives the displayed implicit height relation, with $0<z_i<D$. Warm air above the doorway stores heat but adds no available head at its crest in this uniform-layer model.

#### Two-plume three-layer displacement ventilation

↑ **Parent:** [Displacement ventilation](#displacement-ventilation)

Two independent point-source [pure plumes](turbulent-plume.md#pure-plume) with $\psi=B_1/B_2<1$ remove lower-layer volume $Q=C(B_1^{1/3}+B_2^{1/3})h_1^{5/3}$. If plume 1 feeds the middle layer, its reduced gravity is $g_1'=B_1/[CB_1^{1/3}h_1^{5/3}]$. The upper outflow carries both sources, so $g_2'=(B_1+B_2)/Q$, yielding the displayed ratio. Opening flow is driven by the integrated hydrostatic head $g_1'(h_2-h_1)+g_2'(H-h_2)$. A plume crossing the lower interface has altered buoyancy relative to its new ambient and must be continued with nonzero incoming mass and momentum fluxes rather than reset as a zero-flux pure plume.

#### Source-volume blocking of displacement ventilation

↑ **Parent:** [Displacement ventilation](#displacement-ventilation)

A source volume $Q$ makes roof outflow exceed floor inflow by $Q$. At zero floor inflow, an entraining plume cannot support a steady cold lower layer; the warm layer reaches the floor. With [reduced gravity](reduced-gravity.md) $g'=B/Q$, the entire hydrostatic head drives roof discharge $Q=A_e\sqrt{g'H}$. This gives the stated threshold. Equal splitting of [pressure](thermodynamics.md#pressure) head is inappropriate at blocking. The same result in physical-area notation is $Q_c=(2C_d^2A_{\rm geom}^2BH)^{1/3}$.

#### Ventilated filling-box relaxation

↑ **Parent:** [Displacement ventilation](#displacement-ventilation)

For total plume flux $P(h)$, fixed ceiling exhaust $F$, zero ambient [buoyancy](#buoyancy), and uniform upper-layer [reduced gravity](reduced-gravity.md) $b$, the ideal two-layer balances are

$$
A\dot h=F-P(h),\qquad \frac{d}{dt}\bigl[A(H-h)b\bigr]=B-Fb.
$$

At $P(h_*)=F$ and $b_*=B/F$, [linearization](algebra.md#linearization) yields the decay times $\tau_h=A/P'(h_*)$ and $\tau_b=A(H-h_*)/F$. For $P(h)\propto h^{5/3}$, $\tau_h=3Ah_*/(5F)$. Upper-layer [buoyancy](#buoyancy) relaxation usually dominates when $h_*\ll H$. Exact equilibrium is approached asymptotically; a fixed small relative tolerance takes order $\max(\tau_h,\tau_b)\log(1/\varepsilon)$ after the initial transient.

#### No steady displacement layer without ambient supply

↑ **Parent:** [Displacement ventilation](#displacement-ventilation)

Consider entraining plumes supplied with total source [volume flux](#volumetric-flow-rate) $S$, a separate lower-layer ambient inflow $L$, and ceiling exhaust $F=S+L$. Write $P(h)=S+E(h)$, where $E(h)$ is total [fluid entrainment](#fluid-entrainment) from the lower layer. [Volume conservation](physics.md#volume-conservation) gives $A\dot h=L-E(h)$. A steady positive lower layer therefore requires $L=E(h)>0$. If $L=0$ and $E(h)>0$ for every $h>0$, no positive steady [displacement-ventilation interface height](#displacement-ventilation-interface-height) exists. In a shifted [pure plume](turbulent-plume.md#pure-plume) approximation $P_i(h)=\lambda B_i^{1/3}(h+z_i)^{5/3}$ matched to source flux $S_i$ at $h=0$, this follows immediately from $P_i(h)>S_i$ for $h>0$. This is a statement about the ideal two-layer model, not a prohibition of all possible stratification in a real ventilated room.

#### Multiple-plume displacement ventilation

↑ **Parent:** [Displacement ventilation](#displacement-ventilation)

Suppose $n$ independent [axisymmetric pure plumes](turbulent-plume.md#axisymmetric-pure-plume) share total [buoyancy flux](turbulent-plume.md#buoyancy-flux) $B$ equally, have negligible source [volume flux](#volumetric-flow-rate), and are supplied with a separate ambient ventilation flux $F$ at floor level. Their combined flux is $P(h)=\lambda n^{2/3}B^{1/3}h^{5/3}$. [Volume conservation](physics.md#volume-conservation) at a steady [displacement-ventilation interface height](#displacement-ventilation-interface-height) and [buoyancy flux](turbulent-plume.md#buoyancy-flux) conservation give

$$
h_* = \left(\frac{F}{\lambda n^{2/3}B^{1/3}}\right)^{3/5},\qquad b_* = \frac BF.
$$

A positive two-layer state needs $0<h_*<H$, sources small relative to $h_*$, and plumes sufficiently separated to remain independent. Splitting the sources increases total [fluid entrainment](#fluid-entrainment) and reduces the interface height by $n^{-2/5}$. A finite source flux cannot simultaneously be neglected and supply all the replacement air; [no steady displacement layer without ambient supply](#no-steady-displacement-layer-without-ambient-supply) explains this restriction.

#### Displacement-ventilation interface height

↑ **Parent:** [Displacement ventilation](#displacement-ventilation)

At steady state, the displacement-ventilation interface lies where the total plume [volume flux](#volumetric-flow-rate) equals the imposed ventilation flux. For one triangular-profile [wall line plume](turbulent-plume.md#wall-line-plume) with kinematic [buoyancy flux](turbulent-plume.md#buoyancy-flux) $B_0$, entrainment coefficient $\alpha$, and ventilation flux $A$ per unit span,

$$
h=\left(\frac{2}{3\alpha}\right)^{2/3}\frac{A}{B_0^{1/3}}.
$$

### Single-opening exchange flow

↑ **Parent:** [Natural ventilation](#natural-ventilation)

A tall opening between fluids of different densities can support simultaneous inflow below a neutral pressure level and outflow above it. For a symmetric opening with a Boussinesq hydrostatic pressure difference and equal discharge coefficients, the neutral level lies at mid-height.

#### Neutral pressure level

↑ **Parent:** [Single-opening exchange flow](#single-opening-exchange-flow)

The neutral pressure level is the height at which indoor and outdoor hydrostatic pressures agree. Flow through an opening reverses direction across this level.

### Stratified-room plume-exchange model

↑ **Parent:** [Natural ventilation](#natural-ventilation)

A stratified-room plume-exchange model balances the upward volume transported by a warm plume against downward transport by cold wall plumes. A global buoyancy balance relates the source flux to the buoyancy carried out through the vents.

## Homologous spherical flow

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A homologous spherical flow has velocity proportional to radius. Its [velocity gradient](continuum-mechanics.md#velocity-gradient) is $q(t)I$ and its [velocity divergence](continuum-mechanics.md#velocity-divergence) is $3q(t)$.

### Self-similar ansatz

↑ **Parent:** [Homologous spherical flow](#homologous-spherical-flow)

A self-similar ansatz expresses evolving fields through a dimensionless similarity coordinate such as $x=r/R(t)$, reducing a partial differential equation to ordinary differential equations in $x$.

## ↑ Ancestors (3)

1. [Branches of physics](physics.md#branches-of-physics)
2. [Physics](physics.md)
3. [Codex Wiki](README.md)

## ← Incoming links (1)

- [Sonic point of a scalar flux](partial-differential-equation.md#sonic-point-of-a-scalar-flux)
