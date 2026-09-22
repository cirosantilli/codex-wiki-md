# Fluid mechanics

↑ **Parent:** [Branches of physics](physics.md#branches-of-physics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fluid_mechanics)

[Fluid mechanics](fluid-mechanics.md) studies the motion and [forces](force.md) of [liquids](thermodynamics.md#liquid) and [gases](thermodynamics.md#gas). Its central simplification is the [continuum approximation](continuum-mechanics.md#continuum-approximation): replace individual [molecules](molecule.md) by bulk properties defined at every position and time. The averaging region must contain many [molecules](molecule.md) while remaining small compared with the distances over which those properties vary. A [fluid element](continuum-mechanics.md#fluid-element) is such a small material parcel, rather than a single [molecule](molecule.md). This connects [fluid mechanics](fluid-mechanics.md) to [continuum mechanics](continuum-mechanics.md) and makes [calculus](calculus.md) useful for describing flow. [MIT, A. Techet, Hydrodynamics reading 1, pp. 2–3](https://ocw.mit.edu/courses/2-016-hydrodynamics-13-012-fall-2005/dc299d2ff05553b3515dccc23fc0f7d2_2005reading1.pdf)

Three basic fields are the [velocity field](#velocity-field) $\mathbf u(\mathbf x,t)$, the [mass density](#density) $\rho(\mathbf x,t)$ and the [pressure](pressure.md) $p(\mathbf x,t)$. The first gives a parcel's instantaneous [velocity](classical-mechanics.md#velocity); the second gives [mass](classical-mechanics.md#mass) per unit [volume](geometry-and-topology.md#volume). The [pressure](pressure.md) contributes an inward normal [traction](continuum-mechanics.md#traction) $-p\mathbf n$ across a surface with outward unit normal $\mathbf n$. Thus [pressure](pressure.md) is a [stress](continuum-mechanics.md#stress), measured in $\mathrm{Pa}=\mathrm{N\,m^{-2}}$, and may vary with position even in [incompressible flow](#incompressible-flow). Additional [viscous stresses](dynamic-viscosity.md#viscous-stress-tensor) can act tangentially. [MIT, A. Techet, Hydrodynamics reading 1, p. 5](https://ocw.mit.edu/courses/2-016-hydrodynamics-13-012-fall-2005/dc299d2ff05553b3515dccc23fc0f7d2_2005reading1.pdf)

The guiding questions are what must be conserved and which [forces](force.md) matter. [Mass conservation](continuum-mechanics.md#mass-conservation) constrains the [velocity field](#velocity-field); [momentum conservation](momentum.md#momentum-conservation) determines its response to [pressure gradients](#pressure-gradient), [viscosity](dynamic-viscosity.md) and body [forces](force.md). An [incompressible flow](#incompressible-flow) model, a [Reynolds number](dynamic-viscosity.md#reynolds-number) estimate and [Bernoulli's principle](euler-equations-for-an-inviscid-fluid.md#bernoulli-s-principle) answer different parts of a problem. Their appeal is that a few carefully stated assumptions can determine useful quantities before the entire [velocity field](#velocity-field) is known.

**Table of contents**

- [Multiphase flow](#multiphase-flow)
  - [Complex characteristic speeds of a pressure-coupled two-fluid model](#complex-characteristic-speeds-of-a-pressure-coupled-two-fluid-model)
  - [Intrinsic phase averages in a two-fluid pipe model](#intrinsic-phase-averages-in-a-two-fluid-pipe-model)
  - [Interphase mass transfer](#interphase-mass-transfer)
- [Cross-section averaged phase mass balance](#cross-section-averaged-phase-mass-balance)
- [Chézy friction law](#chezy-friction-law)
- [Hydraulic radius](#hydraulic-radius)
  - [Chézy drag law](#chezy-drag-law)
- [Cross-section averaged phase momentum balance](#cross-section-averaged-phase-momentum-balance)
- [Hydrometer](#hydrometer)
  - [Urinometer](#urinometer)
- [Hydrofoil](#hydrofoil)
- [Anelastic approximation](#anelastic-approximation)
- [Air pump](#air-pump)
- [Eddy](#eddy)
- [Wall slip](#wall-slip)
- [Focal length of a rotating liquid mirror](#focal-length-of-a-rotating-liquid-mirror)
- [Pump](#pump)
  - [Centrifugal pump](#centrifugal-pump)
- [Hydraulic diameter](#hydraulic-diameter)
- [Computational fluid dynamics](#computational-fluid-dynamics)
- [Microfluidics](#microfluidics)
  - [Nanopore](#nanopore)
  - [Resistive-pulse sensing](#resistive-pulse-sensing)
- [Magnus effect](#magnus-effect)
- [Laminar flow](#laminar-flow)
  - [Reynolds pipe-and-dye experiment](#reynolds-pipe-and-dye-experiment)
- [Void fraction](#void-fraction)
  - [Terminal-drift density law for compressible bubbles](#terminal-drift-density-law-for-compressible-bubbles)
  - [Kinematic bubble transport in an exponentially narrowing vessel](#kinematic-bubble-transport-in-an-exponentially-narrowing-vessel)
  - [Bubble clearing in a cylindrical vessel](#bubble-clearing-in-a-cylindrical-vessel)
- [Strouhal number](#strouhal-number)
- [Lift (force)](lift-force.md)
  - [Lift coefficient](lift-force.md#lift-coefficient)
  - [Pressure coefficient](lift-force.md#pressure-coefficient)
- [Static pressure](#static-pressure)
  - [Absolute pressure](#absolute-pressure)
  - [Stagnation pressure](#stagnation-pressure)
- [Manometer](#manometer)
  - [U-tube differential manometer](#u-tube-differential-manometer)
  - [McLeod gauge](#mcleod-gauge)
- [Pressure transducer](#pressure-transducer)
  - [Differential-pressure calibration](#differential-pressure-calibration)
- [D'Alembert's paradox](#d-alembert-s-paradox)
- [Wind tunnel](#wind-tunnel)
  - [Supersonic wind tunnel](#supersonic-wind-tunnel)
- [Airfoil](#airfoil)
  - [Angle of attack](#angle-of-attack)
  - [Thin airfoil theory](#thin-airfoil-theory)
  - [Aerodynamic stall](#aerodynamic-stall)
- [Uniform flow](#uniform-flow)
- [Volume viscosity](#volume-viscosity)
- [Hydraulic resistance](#hydraulic-resistance)
  - [Hydraulic ladder network](#hydraulic-ladder-network)
  - [Delta-star transformation](#delta-star-transformation)
- [Physiological fluid dynamics](physiological-fluid-dynamics.md)
  - [Lubrication model of a compliant translating plug](physiological-fluid-dynamics.md#lubrication-model-of-a-compliant-translating-plug)
  - [Annular inviscid-core displacement](physiological-fluid-dynamics.md#annular-inviscid-core-displacement)
  - [Peristaltic pumping](physiological-fluid-dynamics.md#peristaltic-pumping)
  - [Collapsible tube flow](physiological-fluid-dynamics.md#collapsible-tube-flow)
  - [Arterial pressure wave](physiological-fluid-dynamics.md#arterial-pressure-wave)
- [Fluid](#fluid)
- [Buoyant plume](#buoyant-plume)
- [Pathline](#pathline)
- [Control volume](#control-volume)
- [Navier slip boundary condition](#navier-slip-boundary-condition)
  - [Slip length](#slip-length)
  - [Wall friction in the Navier slip boundary condition](#wall-friction-in-the-navier-slip-boundary-condition)
- [Fluid free boundary](#fluid-free-boundary)
- [Material surface](#material-surface)
  - [Material surface element](#material-surface-element)
- [Material curve](#material-curve)
- [Scalar transport](scalar-transport.md)
  - [Active scalar](scalar-transport.md#active-scalar)
  - [Passive scalar](scalar-transport.md#passive-scalar)
  - [Adjoint equations for Boussinesq scalar mixing](scalar-transport.md#adjoint-equations-for-boussinesq-scalar-mixing)
  - [Scalar variance](scalar-transport.md#scalar-variance)
- [Fluid flow](#fluid-flow)
  - [Airflow](#airflow)
  - [Unidirectional flow](#unidirectional-flow)
  - [Steady flow](#steady-flow)
  - [Inviscid flow](#inviscid-flow)
- [Sediment transport](#sediment-transport)
  - [Relaxation-controlled antidune instability](#relaxation-controlled-antidune-instability)
  - [Bedload transport](#bedload-transport)
  - [Suspended sediment](#suspended-sediment)
  - [Dune](#dune)
  - [Antidune](#antidune)
  - [Sediment resuspension](#sediment-resuspension)
  - [Sediment transport saturation](#sediment-transport-saturation)
  - [Exner equation](#exner-equation)
  - [Shields parameter](#shields-parameter)
  - [Bedform](#bedform)
- [Ram pressure](#ram-pressure)
- [Turbulence](turbulence.md)
  - [Reynolds averaging](turbulence.md#reynolds-averaging)
  - [External intermittency](turbulence.md#external-intermittency)
  - [Wave turbulence](turbulence.md#wave-turbulence)
  - [Magnetohydrodynamic turbulence](turbulence.md#magnetohydrodynamic-turbulence)
  - [Turbulence closure](turbulence.md#turbulence-closure)
  - [K-epsilon turbulence model](turbulence.md#k-epsilon-turbulence-model)
  - [Turbulent mixing](turbulence.md#turbulent-mixing)
  - [Turbulent plane jet similarity](turbulence.md#turbulent-plane-jet-similarity)
  - [Mixing length](turbulence.md#mixing-length)
  - [Turbulent kinetic energy](turbulence.md#turbulent-kinetic-energy)
  - [Reynolds stress](turbulence.md#reynolds-stress)
  - [Internal intermittency](turbulence.md#internal-intermittency)
  - [Energy cascade](turbulence.md#energy-cascade)
  - [Homogeneous turbulence](turbulence.md#homogeneous-turbulence)
  - [Eddy diffusion](turbulence.md#eddy-diffusion)
  - [Eddy diffusivity](turbulence.md#eddy-diffusivity)
  - [Turbulent round jet](turbulence.md#turbulent-round-jet)
- [Acoustic wave](#acoustic-wave)
  - [Acoustic modes of a rigid cylindrical cavity](#acoustic-modes-of-a-rigid-cylindrical-cavity)
  - [Nonlinear acoustics](#nonlinear-acoustics)
  - [Ultrasound](#ultrasound)
  - [Burgers reduction of weakly nonlinear rightgoing acoustics](#burgers-reduction-of-weakly-nonlinear-rightgoing-acoustics)
  - [Adiabatic vertical modes of a Gaussian atmosphere](#adiabatic-vertical-modes-of-a-gaussian-atmosphere)
  - [Acoustically rigid boundary](#acoustically-rigid-boundary)
  - [Acoustic cutoff frequency](#acoustic-cutoff-frequency)
  - [Pressure-release boundary](#pressure-release-boundary)
  - [Sonic boom](#sonic-boom)
- [Velocity field](#velocity-field)
  - [Affine velocity field](#affine-velocity-field)
  - [Secondary flow](#secondary-flow)
  - [Velocity gradient tensor](#velocity-gradient-tensor)
  - [Vertical velocity](#vertical-velocity)
  - [Axisymmetric flow](#axisymmetric-flow)
- [Advection](#advection)
  - [Chaotic advection](#chaotic-advection)
  - [Ballistic transport](#ballistic-transport)
- [Convection](convection.md)
  - [Convection cell](convection.md#convection-cell)
  - [Convection zone](convection.md#convection-zone)
  - [Compositional convection](convection.md#compositional-convection)
  - [Long-wave convection equation with broken Boussinesq symmetry](convection.md#long-wave-convection-equation-with-broken-boussinesq-symmetry)
  - [Thermal convection](convection.md#thermal-convection)
- [Buoyancy](#buoyancy)
  - [Convective available potential energy](#convective-available-potential-energy)
  - [Centre of buoyancy](#centre-of-buoyancy)
  - [Buoyancy of an aerated liquid](#buoyancy-of-an-aerated-liquid)
  - [Buoyancy gradient](#buoyancy-gradient)
  - [Magnetic buoyancy](#magnetic-buoyancy)
  - [Archimedes' principle](#archimedes-principle)
  - [Neutral buoyancy](#neutral-buoyancy)
  - [Submerged weight](#submerged-weight)
  - [Buoyancy perturbation](#buoyancy-perturbation)
  - [Isopycnal](#isopycnal)
- [Hydrodynamic stability](hydrodynamic-stability.md)
  - [Shear instability](hydrodynamic-stability.md#shear-instability)
  - [Static stability](hydrodynamic-stability.md#static-stability)
  - [Convective amplification length](hydrodynamic-stability.md#convective-amplification-length)
  - [Global hydrodynamic mode](hydrodynamic-stability.md#global-hydrodynamic-mode)
  - [Global hydrodynamic instability](hydrodynamic-stability.md#global-hydrodynamic-instability)
  - [Critical layer in a shear flow](hydrodynamic-stability.md#critical-layer-in-a-shear-flow)
  - [Critical level of a shear-flow wave](hydrodynamic-stability.md#critical-level-of-a-shear-flow-wave)
  - [Baroclinic instability](hydrodynamic-stability.md#baroclinic-instability)
  - [Three-layer long-wave shear-flow matching](hydrodynamic-stability.md#three-layer-long-wave-shear-flow-matching)
  - [Pressure equation for a shear-flow normal mode](hydrodynamic-stability.md#pressure-equation-for-a-shear-flow-normal-mode)
  - [Adjoint linearized Navier-Stokes evolution](hydrodynamic-stability.md#adjoint-linearized-navier-stokes-evolution)
  - [Kinetic-energy inner product](hydrodynamic-stability.md#kinetic-energy-inner-product)
  - [Stability diagram of the linear complex Ginzburg-Landau equation](hydrodynamic-stability.md#stability-diagram-of-the-linear-complex-ginzburg-landau-equation)
  - [Saddle growth rate along a ray](hydrodynamic-stability.md#saddle-growth-rate-along-a-ray)
  - [Convective hydrodynamic instability](hydrodynamic-stability.md#convective-hydrodynamic-instability)
  - [Absolute hydrodynamic instability](hydrodynamic-stability.md#absolute-hydrodynamic-instability)
  - [Orr-Sommerfeld equation](hydrodynamic-stability.md#orr-sommerfeld-equation)
  - [Inertial instability](hydrodynamic-stability.md#inertial-instability)
  - [Rayleigh equation for inviscid shear flow](hydrodynamic-stability.md#rayleigh-equation-for-inviscid-shear-flow)
  - [Counterpropagating wave instability](hydrodynamic-stability.md#counterpropagating-wave-instability)
  - [Transient growth from non-normal modes](hydrodynamic-stability.md#transient-growth-from-non-normal-modes)
  - [Energy-stability threshold](hydrodynamic-stability.md#energy-stability-threshold)
  - [Symmetric instability](hydrodynamic-stability.md#symmetric-instability)
  - [Eady model](hydrodynamic-stability.md#eady-model)
  - [Dissipation-induced instability](hydrodynamic-stability.md#dissipation-induced-instability)
  - [Rayleigh discriminant](hydrodynamic-stability.md#rayleigh-discriminant)
- [Barotropic fluid](#barotropic-fluid)
  - [Barotropic cylindrical rotation theorem](#barotropic-cylindrical-rotation-theorem)
  - [Barotropic spherical accretion equation](#barotropic-spherical-accretion-equation)
  - [Barotropic enthalpy function](#barotropic-enthalpy-function)
  - [Centrifugal potential of cylindrical rotation](#centrifugal-potential-of-cylindrical-rotation)
  - [Barotropic energy density](#barotropic-energy-density)
  - [Barotropic magnetic energy equation](#barotropic-magnetic-energy-equation)
  - [Barotropic vorticity transport](#barotropic-vorticity-transport)
- [Shear flow](#shear-flow)
  - [Vertical shear](#vertical-shear)
  - [Renovating shear flow](#renovating-shear-flow)
  - [Linear shear flow](#linear-shear-flow)
- [Lagrangian displacement (fluid mechanics)](#lagrangian-displacement-fluid-mechanics)
  - [Eulerian perturbation of a fluid variable](#eulerian-perturbation-of-a-fluid-variable)
  - [Lagrangian perturbation of a fluid variable](#lagrangian-perturbation-of-a-fluid-variable)
- [Eulerian and Lagrangian fluid perturbations](#eulerian-and-lagrangian-fluid-perturbations)
  - [Eulerian fluid perturbation](#eulerian-fluid-perturbation)
  - [Surface density perturbation of a displaced uniform interface](#surface-density-perturbation-of-a-displaced-uniform-interface)
  - [Lagrangian pressure perturbation](#lagrangian-pressure-perturbation)
- [Torricelli's law](#torricelli-s-law)
  - [Draining tank with constant cross-sectional area](#draining-tank-with-constant-cross-sectional-area)
  - [Discharge measurement in a draining tank](#discharge-measurement-in-a-draining-tank)
  - [Drainage time of a conical tank](#drainage-time-of-a-conical-tank)
- [Density](#density)
  - [Relative density](#relative-density)
  - [Integrable power-law density at an axis or center](#integrable-power-law-density-at-an-axis-or-center)
  - [Density profile](#density-profile)
  - [Mass current](#mass-current)
  - [Mean density](#mean-density)
  - [Mass of an exponential spherical atmosphere](#mass-of-an-exponential-spherical-atmosphere)
  - [Gas density](#gas-density)
  - [Linear mass density](#linear-mass-density)
  - [Gas clumping factor](#gas-clumping-factor)
  - [Projected surface mass density](#projected-surface-mass-density)
- [Fluid pressure](#fluid-pressure)
  - [Cavitation](#cavitation)
  - [Pressure gradient](#pressure-gradient)
- [Drag (physics)](#drag-physics)
  - [Air resistance](#air-resistance)
  - [Linear drag](#linear-drag)
  - [Drag coefficient](#drag-coefficient)
  - [Quadratic drag](#quadratic-drag)
  - [Pressure drag](#pressure-drag)
  - [Stokes number](#stokes-number)
  - [Gas drag](#gas-drag)
  - [Aerodynamic stopping time](#aerodynamic-stopping-time)
- [Dynamic viscosity](dynamic-viscosity.md)
  - [Viscous drag coefficient](dynamic-viscosity.md#viscous-drag-coefficient)
  - [Lateral viscosity](dynamic-viscosity.md#lateral-viscosity)
  - [Zero-shear viscosity](dynamic-viscosity.md#zero-shear-viscosity)
  - [Kinematic viscosity](dynamic-viscosity.md#kinematic-viscosity)
  - [Viscous stress tensor](dynamic-viscosity.md#viscous-stress-tensor)
  - [Reynolds number](dynamic-viscosity.md#reynolds-number)
- [Suspension (chemistry)](suspension-chemistry.md)
  - [Sedimentation](suspension-chemistry.md#sedimentation)
  - [Monodisperse](suspension-chemistry.md#monodisperse)
  - [Density inversion in a settling suspension](suspension-chemistry.md#density-inversion-in-a-settling-suspension)
  - [Heated particle-laden layer](suspension-chemistry.md#heated-particle-laden-layer)
  - [Particle volume fraction](suspension-chemistry.md#particle-volume-fraction)
  - [Bidisperse particle suspension](suspension-chemistry.md#bidisperse-particle-suspension)
  - [Settling velocity](suspension-chemistry.md#settling-velocity)
- [Mass diffusivity](#mass-diffusivity)
- [Vorticity](vorticity.md)
  - [Local spin in an azimuthal power-law flow](vorticity.md#local-spin-in-an-azimuthal-power-law-flow)
  - [Vorticity of a linear shear flow](vorticity.md#vorticity-of-a-linear-shear-flow)
  - [Vortex line](vorticity.md#vortex-line)
  - [Vortex (fluid mechanics)](vorticity.md#vortex-fluid-mechanics)
  - [Hydrodynamic Biot-Savart kernel](vorticity.md#hydrodynamic-biot-savart-kernel)
  - [Hydrodynamic impulse](vorticity.md#hydrodynamic-impulse)
  - [Vortex tube](vorticity.md#vortex-tube)
  - [Enstrophy](vorticity.md#enstrophy)
  - [Planar vorticity velocity kernel](vorticity.md#planar-vorticity-velocity-kernel)
  - [Uniform-vorticity circular flow in an annulus](vorticity.md#uniform-vorticity-circular-flow-in-an-annulus)
  - [Vorticity cross-product identity](vorticity.md#vorticity-cross-product-identity)
  - [Hydrodynamical helicity](vorticity.md#hydrodynamical-helicity)
  - [Absolute vorticity](vorticity.md#absolute-vorticity)
  - [Relative vorticity](vorticity.md#relative-vorticity)
  - [Circulation (physics)](vorticity.md#circulation-physics)
  - [Irrotational flow](vorticity.md#irrotational-flow)
- [Circular vortex-sheet mode](#circular-vortex-sheet-mode)
- [Gravity wave](gravity-wave.md)
  - [Internal wave](gravity-wave.md#internal-wave)
- [Stream function](#stream-function)
  - [Sine-cosine cellular Euler flow](#sine-cosine-cellular-euler-flow)
  - [Steady Euler flow with vorticity proportional to its stream function](#steady-euler-flow-with-vorticity-proportional-to-its-stream-function)
  - [Sinusoidal cellular flow](#sinusoidal-cellular-flow)
  - [Linear planar strain and rotation streamlines](#linear-planar-strain-and-rotation-streamlines)
  - [Axisymmetric hydrodynamic mass flux function](#axisymmetric-hydrodynamic-mass-flux-function)
  - [Stokes streamfunction](#stokes-streamfunction)
  - [Streamline classification of a planar linear saddle or centre](#streamline-classification-of-a-planar-linear-saddle-or-centre)
- [Streamline](#streamline)
  - [Free streamline](#free-streamline)
  - [Stream tube](#stream-tube)
- [Velocity potential](#velocity-potential)
  - [Additive freedom of a velocity potential](#additive-freedom-of-a-velocity-potential)
  - [Potential flow around a circular cylinder](#potential-flow-around-a-circular-cylinder)
  - [Radially symmetric incompressible flow in a planar annulus](#radially-symmetric-incompressible-flow-in-a-planar-annulus)
- [Plume (fluid dynamics)](#plume-fluid-dynamics)
  - [Laminar plume](#laminar-plume)
- [Euler equations for an inviscid fluid](euler-equations-for-an-inviscid-fluid.md)
  - [Euler equation in a uniformly rotating frame](euler-equations-for-an-inviscid-fluid.md#euler-equation-in-a-uniformly-rotating-frame)
  - [Density scaling invariance of incompressible Euler flow](euler-equations-for-an-inviscid-fluid.md#density-scaling-invariance-of-incompressible-euler-flow)
  - [Linearized Euler equations](euler-equations-for-an-inviscid-fluid.md#linearized-euler-equations)
  - [Conservative energy flux of a polytropic ideal gas](euler-equations-for-an-inviscid-fluid.md#conservative-energy-flux-of-a-polytropic-ideal-gas)
  - [Crocco form of the unsteady Euler equation](euler-equations-for-an-inviscid-fluid.md#crocco-form-of-the-unsteady-euler-equation)
  - [Yudovich characteristic flow](euler-equations-for-an-inviscid-fluid.md#yudovich-characteristic-flow)
  - [Bernoulli's principle](euler-equations-for-an-inviscid-fluid.md#bernoulli-s-principle)
  - [Axisymmetric inviscid flow between moving parallel plates](euler-equations-for-an-inviscid-fluid.md#axisymmetric-inviscid-flow-between-moving-parallel-plates)
  - [Radial velocity](euler-equations-for-an-inviscid-fluid.md#radial-velocity)
  - [Unsteady Bernoulli equation](euler-equations-for-an-inviscid-fluid.md#unsteady-bernoulli-equation)
  - [Clebsch-potential variational derivation of incompressible Euler flow](euler-equations-for-an-inviscid-fluid.md#clebsch-potential-variational-derivation-of-incompressible-euler-flow)
  - [Bernoulli equation](euler-equations-for-an-inviscid-fluid.md#bernoulli-equation)
  - [Integral momentum equation](euler-equations-for-an-inviscid-fluid.md#integral-momentum-equation)
- [Conservation of mass in a pipe](#conservation-of-mass-in-a-pipe)
- [Surface tension](surface-tension.md)
  - [Meniscus (liquid)](surface-tension.md#meniscus-liquid)
  - [Critical point drying](surface-tension.md#critical-point-drying)
  - [Capillary force](surface-tension.md#capillary-force)
  - [Hamaker estimate of liquid surface tension](surface-tension.md#hamaker-estimate-of-liquid-surface-tension)
  - [Thermodynamics of a liquid film](surface-tension.md#thermodynamics-of-a-liquid-film)
  - [Surface energy](surface-tension.md#surface-energy)
  - [Wetting](surface-tension.md#wetting)
  - [Bond number](surface-tension.md#bond-number)
  - [Oil lens capillary balance](surface-tension.md#oil-lens-capillary-balance)
  - [Contact angle](surface-tension.md#contact-angle)
  - [Capillary number](surface-tension.md#capillary-number)
  - [Capillary pressure](surface-tension.md#capillary-pressure)
  - [Surfactant](surface-tension.md#surfactant)
  - [Marangoni effect](surface-tension.md#marangoni-effect)
  - [Rayleigh–Plateau instability](surface-tension.md#rayleigh-plateau-instability)
  - [Young–Laplace equation](surface-tension.md#young-laplace-equation)
  - [Capillary length](surface-tension.md#capillary-length)
  - [Dynamic meniscus](surface-tension.md#dynamic-meniscus)
  - [Capillary wave](surface-tension.md#capillary-wave)
  - [Capillary action](surface-tension.md#capillary-action)
- [Viscous fluid flow](viscous-fluid-flow.md)
  - [Radial viscous flow in a wedge](viscous-fluid-flow.md#radial-viscous-flow-in-a-wedge)
  - [In-phase oscillating parallel-plate flow](viscous-fluid-flow.md#in-phase-oscillating-parallel-plate-flow)
  - [Equilateral triangular pipe flow](viscous-fluid-flow.md#equilateral-triangular-pipe-flow)
  - [Stokes' second problem](viscous-fluid-flow.md#stokes-second-problem)
  - [Euler limit](viscous-fluid-flow.md#euler-limit)
  - [Pressure-driven channel flow](viscous-fluid-flow.md#pressure-driven-channel-flow)
  - [Plane Poiseuille flow](viscous-fluid-flow.md#plane-poiseuille-flow)
  - [Fully developed flow](viscous-fluid-flow.md#fully-developed-flow)
  - [Velocity profile](viscous-fluid-flow.md#velocity-profile)
  - [Viscous boundary layer](viscous-fluid-flow.md#viscous-boundary-layer)
  - [Viscous diffusion time](viscous-fluid-flow.md#viscous-diffusion-time)
  - [Couette flow](viscous-fluid-flow.md#couette-flow)
  - [Falling film flow](viscous-fluid-flow.md#falling-film-flow)
  - [Stress boundary condition](viscous-fluid-flow.md#stress-boundary-condition)
  - [No-slip boundary condition](viscous-fluid-flow.md#no-slip-boundary-condition)
  - [Newtonian fluid](viscous-fluid-flow.md#newtonian-fluid)
  - [Navier-Stokes equation](viscous-fluid-flow.md#navier-stokes-equation)
  - [Pipe flow](viscous-fluid-flow.md#pipe-flow)
  - [Kinetic-energy balance for an incompressible Newtonian fluid](viscous-fluid-flow.md#kinetic-energy-balance-for-an-incompressible-newtonian-fluid)
  - [Stokes flow](stokes-flow.md)
  - [Viscous sheet](viscous-fluid-flow.md#viscous-sheet)
  - [Lubrication theory](viscous-fluid-flow.md#lubrication-theory)
  - [Viscous shear torque](viscous-fluid-flow.md#viscous-shear-torque)
- [Body force](#body-force)
  - [Elastic force dipole](#elastic-force-dipole)
- [Hydrostatic pressure](#hydrostatic-pressure)
  - [Triangular-channel hydrostatic pressure head](#triangular-channel-hydrostatic-pressure-head)
  - [Gauge pressure](#gauge-pressure)
  - [Hydrostatic approximation](#hydrostatic-approximation)
- [Volumetric flow rate](#volumetric-flow-rate)
  - [Discharge](#discharge)
  - [Sverdrup](#sverdrup)
  - [Mass flow rate](#mass-flow-rate)
  - [Volume flux per unit width](#volume-flux-per-unit-width)
  - [Discharge coefficient](#discharge-coefficient)
- [Potential flow](#potential-flow)
  - [Rankine oval](#rankine-oval)
  - [Kutta condition](#kutta-condition)
  - [Uniform potential flow around an ellipse](#uniform-potential-flow-around-an-ellipse)
  - [Boundary integral for kinetic energy of planar potential flow](#boundary-integral-for-kinetic-energy-of-planar-potential-flow)
  - [Finite-energy condition for planar exterior potential flow](#finite-energy-condition-for-planar-exterior-potential-flow)
  - [Uniform potential flow around a fixed sphere](#uniform-potential-flow-around-a-fixed-sphere)
  - [Potential of a translating sphere](#potential-of-a-translating-sphere)
  - [Complex potential of a two-dimensional potential flow](#complex-potential-of-a-two-dimensional-potential-flow)
  - [Corner sink in a semi-infinite channel](#corner-sink-in-a-semi-infinite-channel)
  - [Rankine half-body](#rankine-half-body)
  - [Radial source flow](#radial-source-flow)
  - [Potential dipole](#potential-dipole)
  - [Point source](#point-source)
  - [Sink flow in a sector](#sink-flow-in-a-sector)
  - [Potential flow around a translating sphere](#potential-flow-around-a-translating-sphere)
  - [Spherically symmetric incompressible radial flow](#spherically-symmetric-incompressible-radial-flow)
  - [Squeezing wedge flow](#squeezing-wedge-flow)
- [Free surface](#free-surface)
  - [Surface elevation](#surface-elevation)
  - [Surface gravity wave](#surface-gravity-wave)
- [Streamfunction in polar coordinates](#streamfunction-in-polar-coordinates)
- [Stagnation point](#stagnation-point)
  - [Axisymmetric stagnation strain](#axisymmetric-stagnation-strain)
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
- [Astrophysical fluid dynamics](astrophysical-fluid-dynamics.md)
  - [Isobaric thermal stability of a heated ideal gas](astrophysical-fluid-dynamics.md#isobaric-thermal-stability-of-a-heated-ideal-gas)
  - [Gravitational instability](astrophysical-fluid-dynamics.md#gravitational-instability)
  - [Critically rotating self-gravitating cylinder](astrophysical-fluid-dynamics.md#critically-rotating-self-gravitating-cylinder)
  - [Uniformly rotating barotropic star](astrophysical-fluid-dynamics.md#uniformly-rotating-barotropic-star)
  - [Self-gravitating incompressible slab](astrophysical-fluid-dynamics.md#self-gravitating-incompressible-slab)
  - [Isothermal pressure support during gravitational collapse](astrophysical-fluid-dynamics.md#isothermal-pressure-support-during-gravitational-collapse)
  - [Adiabatic pressure support during gravitational collapse](astrophysical-fluid-dynamics.md#adiabatic-pressure-support-during-gravitational-collapse)
  - [Differential rotation](astrophysical-fluid-dynamics.md#differential-rotation)
  - [Affine stellar model](astrophysical-fluid-dynamics.md#affine-stellar-model)
  - [Stellar oscillation](astrophysical-fluid-dynamics.md#stellar-oscillation)
  - [Polytrope](astrophysical-fluid-dynamics.md#polytrope)
  - [Magnetohydrodynamics](magnetohydrodynamics.md)
  - [Self-gravitating gaseous filament](astrophysical-fluid-dynamics.md#self-gravitating-gaseous-filament)
  - [Parker wind](astrophysical-fluid-dynamics.md#parker-wind)
- [Compressible flow](compressible-flow.md)
  - [Transonic flow](compressible-flow.md#transonic-flow)
  - [Stagnation temperature](compressible-flow.md#stagnation-temperature)
  - [Choked flow](compressible-flow.md#choked-flow)
  - [Quasi-one-dimensional flow](compressible-flow.md#quasi-one-dimensional-flow)
  - [Isothermal flow through molecular hydrogen formation](compressible-flow.md#isothermal-flow-through-molecular-hydrogen-formation)
  - [Self-similar blast wave](compressible-flow.md#self-similar-blast-wave)
  - [Polytropic flow](compressible-flow.md#polytropic-flow)
  - [Spherically symmetric adiabatic flow](compressible-flow.md#spherically-symmetric-adiabatic-flow)
  - [Isothermal shock](compressible-flow.md#isothermal-shock)
  - [Fluid total-energy equation](compressible-flow.md#fluid-total-energy-equation)
  - [Spherical polytropic flow with adiabatic exponent three halves](compressible-flow.md#spherical-polytropic-flow-with-adiabatic-exponent-three-halves)
  - [Speed of sound](compressible-flow.md#speed-of-sound)
  - [Isentropic flow](compressible-flow.md#isentropic-flow)
  - [Globally isothermal equation of state](compressible-flow.md#globally-isothermal-equation-of-state)
  - [Sonic point](compressible-flow.md#sonic-point)
  - [Mach number](compressible-flow.md#mach-number)
  - [Riemann invariant](compressible-flow.md#riemann-invariant)
  - [Normal shock wave](compressible-flow.md#normal-shock-wave)
- [Geophysical fluid dynamics](geophysical-fluid-dynamics.md)
  - [Zonal flow](geophysical-fluid-dynamics.md#zonal-flow)
  - [Pressure coordinate](geophysical-fluid-dynamics.md#pressure-coordinate)
  - [Weak temperature gradient approximation](geophysical-fluid-dynamics.md#weak-temperature-gradient-approximation)
  - [Ekman number](geophysical-fluid-dynamics.md#ekman-number)
  - [Deacon cell](geophysical-fluid-dynamics.md#deacon-cell)
  - [Deformation radius](geophysical-fluid-dynamics.md#deformation-radius)
  - [Burger number](geophysical-fluid-dynamics.md#burger-number)
  - [General circulation model](geophysical-fluid-dynamics.md#general-circulation-model)
  - [Eulerian mean flow](geophysical-fluid-dynamics.md#eulerian-mean-flow)
  - [Thermal wind](geophysical-fluid-dynamics.md#thermal-wind)
  - [Log-pressure coordinate](geophysical-fluid-dynamics.md#log-pressure-coordinate)
  - [Rossby number](geophysical-fluid-dynamics.md#rossby-number)
  - [Burgers number](geophysical-fluid-dynamics.md#burgers-number)
  - [Boussinesq approximation](geophysical-fluid-dynamics.md#boussinesq-approximation)
  - [Rotating fluid](geophysical-fluid-dynamics.md#rotating-fluid)
  - [Potential vorticity](geophysical-fluid-dynamics.md#potential-vorticity)
  - [Quasi-geostrophic approximation](geophysical-fluid-dynamics.md#quasi-geostrophic-approximation)
  - [Geostrophic adjustment](geophysical-fluid-dynamics.md#geostrophic-adjustment)
  - [Ocean circulation](geophysical-fluid-dynamics.md#ocean-circulation)
  - [Rossby wave](geophysical-fluid-dynamics.md#rossby-wave)
  - [Wave activity](geophysical-fluid-dynamics.md#wave-activity)
  - [Equatorial wave](geophysical-fluid-dynamics.md#equatorial-wave)
  - [Transformed Eulerian mean](geophysical-fluid-dynamics.md#transformed-eulerian-mean)
- [Linear acoustics](linear-acoustics.md)
  - [Radial acoustic spectrum between rigid concentric spheres](linear-acoustics.md#radial-acoustic-spectrum-between-rigid-concentric-spheres)
  - [Compliant-wall acoustic cavity](linear-acoustics.md#compliant-wall-acoustic-cavity)
  - [Convected acoustic wave equation](linear-acoustics.md#convected-acoustic-wave-equation)
  - [Sound pressure](linear-acoustics.md#sound-pressure)
  - [Acoustic particle velocity](linear-acoustics.md#acoustic-particle-velocity)
  - [Kundt's tube](linear-acoustics.md#kundt-s-tube)
  - [Stationary vorticity mode in linear acoustics](linear-acoustics.md#stationary-vorticity-mode-in-linear-acoustics)
  - [Rayleigh integral for baffled acoustic radiation](linear-acoustics.md#rayleigh-integral-for-baffled-acoustic-radiation)
  - [Acoustic far field](linear-acoustics.md#acoustic-far-field)
  - [Moving-surface retarded Jacobian](linear-acoustics.md#moving-surface-retarded-jacobian)
  - [Stratified acoustic pressure equation](linear-acoustics.md#stratified-acoustic-pressure-equation)
  - [Acoustic density perturbation](linear-acoustics.md#acoustic-density-perturbation)
  - [Acoustic compact-source approximation](linear-acoustics.md#acoustic-compact-source-approximation)
  - [Acoustic multipole source](linear-acoustics.md#acoustic-multipole-source)
  - [Lighthill acoustic analogy](linear-acoustics.md#lighthill-acoustic-analogy)
  - [Linear homentropic acoustic equations](linear-acoustics.md#linear-homentropic-acoustic-equations)
  - [Homentropic pressure perturbation](linear-acoustics.md#homentropic-pressure-perturbation)
  - [Acoustic velocity potential](linear-acoustics.md#acoustic-velocity-potential)
  - [Acoustic energy conservation](linear-acoustics.md#acoustic-energy-conservation)
  - [Evanescent acoustic surface wave](linear-acoustics.md#evanescent-acoustic-surface-wave)
  - [Time average of harmonic power](linear-acoustics.md#time-average-of-harmonic-power)
- [Dispersion of a solute by flow](#dispersion-of-a-solute-by-flow)
  - [Irreversible capture of an advecting tracer](#irreversible-capture-of-an-advecting-tracer)
  - [Transverse dispersion](#transverse-dispersion)
  - [Péclet number](#peclet-number)
  - [Taylor dispersion](#taylor-dispersion)
- [Porous-media flow](porous-media-flow.md)
  - [Soil infiltration](porous-media-flow.md#soil-infiltration)
  - [Pore pressure](porous-media-flow.md#pore-pressure)
  - [Aquifer](porous-media-flow.md#aquifer)
  - [Delayed polymer diversion in parallel porous layers](porous-media-flow.md#delayed-polymer-diversion-in-parallel-porous-layers)
  - [Thermal front in a porous medium](porous-media-flow.md#thermal-front-in-a-porous-medium)
  - [Porous medium](porous-media-flow.md#porous-medium)
  - [Resident-weighted transit time in a layered flow](porous-media-flow.md#resident-weighted-transit-time-in-a-layered-flow)
  - [Capillary imbibition](porous-media-flow.md#capillary-imbibition)
  - [Two-phase porous-media flow](porous-media-flow.md#two-phase-porous-media-flow)
  - [Flux-weighted residence time in a porous layer](porous-media-flow.md#flux-weighted-residence-time-in-a-porous-layer)
  - [Vertical imbibition under a draining liquid layer](porous-media-flow.md#vertical-imbibition-under-a-draining-liquid-layer)
  - [Darcy law](porous-media-flow.md#darcy-law)
  - [Reactive infiltration instability](porous-media-flow.md#reactive-infiltration-instability)
  - [Porous gravity current](porous-media-flow.md#porous-gravity-current)
- [Reduced gravity](reduced-gravity.md)
  - [Buoyancy exchange time of a cold-air enclosure](reduced-gravity.md#buoyancy-exchange-time-of-a-cold-air-enclosure)
  - [Entraining shallow-water layer](reduced-gravity.md#entraining-shallow-water-layer)
  - [Gravity current](reduced-gravity.md#gravity-current)
- [Rheology](rheology.md)
  - [Rock strength envelope](rheology.md#rock-strength-envelope)
  - [Rheometry](rheology.md#rheometry)
  - [Yield stress](rheology.md#yield-stress)
  - [Microrheology](rheology.md#microrheology)
  - [Extensional flow](rheology.md#extensional-flow)
  - [Viscous dissipation potential](rheology.md#viscous-dissipation-potential)
  - [Rheometer](rheology.md#rheometer)
  - [Non-Newtonian fluid](rheology.md#non-newtonian-fluid)
- [Laminar round jet](#laminar-round-jet)
  - [Conserved momentum flux of a laminar round jet](#conserved-momentum-flux-of-a-laminar-round-jet)
  - [Similarity solution for a laminar round jet](#similarity-solution-for-a-laminar-round-jet)
- [Fluid entrainment](#fluid-entrainment)
  - [Entrainment velocity](#entrainment-velocity)
  - [Interfacial power model for entrainment](#interfacial-power-model-for-entrainment)
  - [Potential energy of two-layer entrainment](#potential-energy-of-two-layer-entrainment)
  - [Fixed-energy turbulent mixed layer](#fixed-energy-turbulent-mixed-layer)
- [Turbulent plume](turbulent-plume.md)
  - [Lazy plume](turbulent-plume.md#lazy-plume)
  - [Filling box model](turbulent-plume.md#filling-box-model)
  - [Forced plume](turbulent-plume.md#forced-plume)
  - [Buoyancy flux](turbulent-plume.md#buoyancy-flux)
  - [Batchelor entrainment hypothesis](turbulent-plume.md#batchelor-entrainment-hypothesis)
  - [Top-hat plume model](turbulent-plume.md#top-hat-plume-model)
  - [Heated wall plume](turbulent-plume.md#heated-wall-plume)
  - [Buoyant thermal](turbulent-plume.md#buoyant-thermal)
  - [Starting plume](turbulent-plume.md#starting-plume)
  - [Buoyant intrusion](turbulent-plume.md#buoyant-intrusion)
- [Natural ventilation](#natural-ventilation)
  - [Stack effect](#stack-effect)
  - [Cross ventilation](#cross-ventilation)
  - [Ventilation after a heating reduction](#ventilation-after-a-heating-reduction)
  - [Well-mixed ventilation temperature balance](#well-mixed-ventilation-temperature-balance)
  - [Effective opening area for pressure-driven ventilation](#effective-opening-area-for-pressure-driven-ventilation)
  - [Displacement ventilation](#displacement-ventilation)
  - [Single-opening exchange flow](#single-opening-exchange-flow)
  - [Stratified-room plume-exchange model](#stratified-room-plume-exchange-model)
- [Homologous spherical flow](#homologous-spherical-flow)
  - [Self-similar ansatz](#self-similar-ansatz)
- [Orifice](#orifice)
  - [Vena contracta](#vena-contracta)
- [Nozzle](#nozzle)
  - [Isentropic nozzle flow](#isentropic-nozzle-flow)

## Multiphase flow

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A flow containing two or more distinguishable material phases, such as two immiscible liquids or a gas-liquid mixture. Each phase can have its own [volume fraction](continuum-mechanics.md#volume-fraction), [density](#density) and [velocity](classical-mechanics.md#velocity). Cross-sectional or ensemble averaging produces coupled phase balance equations whose mass, momentum and energy exchange terms must be specified consistently. A common [pressure](pressure.md) alone does not automatically make an averaged model well posed.

### Complex characteristic speeds of a pressure-coupled two-fluid model

↑ **Parent:** [Multiphase flow](#multiphase-flow)

Take incompressible phase mass equations for fractions $\alpha,1-\alpha$ and momentum equations $\rho_i[(u_i)_t+u_i(u_i)_x]+p_x=0$ with a common [pressure](pressure.md). At a uniform state with $0<\alpha<1$, elimination of the mass and momentum perturbation amplitudes gives

$$
\rho_1(1-\alpha)(u_1-c)^2+\rho_2\alpha(u_2-c)^2=0.
$$

Its roots are the displayed speeds, whose imaginary parts are $\pm s(u_1-u_2)/(1+s^2)$. A nonzero slip [velocity](classical-mechanics.md#velocity) therefore gives a Fourier branch growing as $e^{|k|\,|\operatorname{Im}c|t}$. No finite-order Sobolev estimate can control all high wavenumbers, showing ill-posedness of this unregularized closure. At zero slip the roots coincide and this nonreal-root argument no longer settles the degenerate case. Phase-fraction endpoints also lie outside the root formula's derivation.

### Intrinsic phase averages in a two-fluid pipe model

↑ **Parent:** [Multiphase flow](#multiphase-flow)

Here $\langle\cdot\rangle$ means integration over a fixed pipe cross-section divided by its area, and $\chi_1$ is the indicator of one immiscible fluid. The [volume fraction](continuum-mechanics.md#volume-fraction) is $\alpha$; intrinsic [density](#density) averages over the phase-occupied area rather than over the whole section. The [velocity](classical-mechanics.md#velocity) must be [density](#density)-weighted for its product with mean phase [density](#density) to represent [mass flux](mathematical-physics.md#mass-flux) exactly.

If there is no interphase mass transfer, integrating $\partial_t(\rho\chi_1)+\nabla\cdot(\rho v\chi_1)=0$ over a section with impermeable outer wall gives $\partial_t(\rho_1\alpha)+\partial_x(\rho_1\alpha u_1)=0$. The second phase uses $1-\alpha$ and its own intrinsic averages. For constant phase [density](#density) the [velocity](classical-mechanics.md#velocity) reduces to the ordinary phase-area average. These definitions apply where the corresponding phase fraction is positive; zero-fraction intrinsic quantities need a separate convention.

#### Phase momentum profile coefficient

↑ **Parent:** [Intrinsic phase averages in a two-fluid pipe model](#intrinsic-phase-averages-in-a-two-fluid-pipe-model)

For an incompressible phase, this coefficient compares its actual axial momentum flux with the uniform-profile flux at the same intrinsic mean [velocity](classical-mechanics.md#velocity). Cauchy-Schwarz gives $D_1\geq1$ where the mean is nonzero. A spatially varying profile can have a larger [second moment](expected-value.md#second-moment) even when its mean speed is unchanged.

With constant $D_1$, expansion of $\partial_t(\alpha u_1)+\partial_x(\alpha D_1u_1^2)$ and use of $\alpha_t+(\alpha u_1)_x=0$ gives $\alpha(u_1)_t+(2D_1-1)\alpha u_1(u_1)_x+(D_1-1)u_1^2\alpha_x$. Thus a profile correction changes both convection and phase-fraction-[gradient](multivariable-calculus.md#gradient) coupling in the averaged momentum equation. If $D_1$ varies, an extra $\alpha u_1^2(D_1)_x$ remains; a zero mean should be treated through the undivided [second moment](expected-value.md#second-moment) rather than an undefined coefficient.

### Interphase mass transfer

↑ **Parent:** [Multiphase flow](#multiphase-flow)

The source $\Gamma_i$ is the mass gained by phase $i$ per mixture volume and time, through processes such as [evaporation](critical-phenomenon.md#evaporation) or condensation. Internal exchange conserves total mass, so its phase sources sum to zero. In an immiscible material-interface model without phase change, every $\Gamma_i$ is zero. The interface may still move: absence of transfer means that mass does not cross it relative to its own motion.

## Cross-section averaged phase mass balance

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

For a pipe of area $A$, let a phase [indicator function](measure-theory.md#indicator-function) be $\chi$. Define $\alpha=A^{-1}\int\chi\,dA$, $\bar\rho=(A\alpha)^{-1}\int\chi\rho\,dA$ and the mass-weighted axial velocity $\bar u=(A\alpha\bar\rho)^{-1}\int\chi\rho u_x\,dA$. Without interfacial mass transfer, integrate $\partial_t(\chi\rho)+\nabla\cdot(\chi\rho\mathbf u)=0$ over a cross-section with impermeable lateral wall. The resulting averaged mass and flux are exactly $\alpha\bar\rho$ and $\alpha\bar\rho\bar u$, proving the displayed law. The complementary phase uses $1-\chi$ and $1-\alpha$. An unweighted phase velocity would not generally factor the mass flux correctly.

<h2 id="chezy-friction-law">Chézy friction law</h2>

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

The [Chézy law](#chezy-friction-law) relates mean open-channel [speed](classical-mechanics.md#speed) to [hydraulic radius](#hydraulic-radius) and [energy](energy.md) slope through a [friction](newtonian-mechanics.md#friction) coefficient. Equivalently one can use bed shear $\tau_b=\rho f u|u|$; for positive uniform flow, balance $\rho gAI=\tau_bP_b$ gives $u=\sqrt{gI/f}\sqrt{A/P_b}$. The absolute value makes drag oppose motion if reverse flows are admitted.

## Hydraulic radius

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

The [hydraulic radius](#hydraulic-radius) is cross-sectional flow [area](differential-geometry.md#surface-area) divided by wetted perimeter. A perimeter-averaged boundary [shear stress](viscous-fluid-flow.md#shear-stress) $\tau$ exerts drag per unit fluid volume $\tau\ell/A=\tau/R$. It differs from both actual depth and the radius of a noncircular channel.

<h3 id="chezy-drag-law">Chézy drag law</h3>

↑ **Parent:** [Hydraulic radius](#hydraulic-radius)

A quadratic boundary-drag model relates [shear stress](viscous-fluid-flow.md#shear-stress) to mean flow [velocity](classical-mechanics.md#velocity), with dimensionless resistance coefficient $c_d>0$. Uniform [steady flow](#steady-flow) down slope $S$ balances $\rho gAS=\tau\ell$, giving $|u|=\sqrt{gRS/c_d}$. Its sign is chosen so drag opposes the motion.

## Cross-section averaged phase momentum balance

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

For a phase occupying area $\alpha A$ of a constant-area pipe, define $\bar\rho=(\alpha A)^{-1}\int\rho\,dA$, $\bar v=\int\rho v\,dA/(\alpha A\bar\rho)$ and $\overline{v^2}=\int\rho v^2\,dA/(\alpha A\bar\rho)$. The [momentum](momentum.md) per length is $A\alpha\bar\rho\bar v$, the advected [momentum flux](mathematical-physics.md#momentum-flux) is $A\alpha\bar\rho\overline{v^2}$, and end pressures contribute $-A\partial_x(\alpha\bar p)$. Applying [Newton's second law](force.md#newton-s-second-law) to a slice proves the displayed balance, with $M$ all other phase forces per length. Interphase pressure terms can cancel the derivative of the area fraction. Equality of the second moment and squared mean requires a separate closure.

## Hydrometer

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hydrometer)

A floating [density](#density) instrument. At equilibrium, [Archimedes' principle](#archimedes-principle) gives $\rho V_{\rm displaced}=m$ for fixed instrument [mass](classical-mechanics.md#mass) $m$, so it displaces more volume in a less dense [liquid](thermodynamics.md#liquid). A graduated narrow stem converts this volume change into a visible immersion reading. Calibration specifies a [temperature](temperature.md) and a reading convention for the [meniscus](surface-tension.md#meniscus-liquid); a sample's other dissolved substances can affect a sugar-calibrated scale.

### Urinometer

↑ **Parent:** [Hydrometer](#hydrometer)

A [hydrometer](#hydrometer) used to measure the [specific gravity](#relative-density) of [urine](physiology.md#urine); readings depend on calibration conditions and dissolved constituents.

## Hydrofoil

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hydrofoil)

A submerged lifting surface that develops [lift](lift-force.md) when water moves relative to it. A thin two-dimensional model relates its motion-induced [lift](lift-force.md) per unit span to bound [circulation](vorticity.md#circulation-physics); [buoyancy](#buoyancy) is a separate contribution to the upward fluid [force](force.md).

## Anelastic approximation

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

An anelastic model filters acoustic density fluctuations while retaining a prescribed stratified reference [mass density](#density). For $\rho_0\propto e^{-z/H}$, continuity is $u_x+v_y+w_z-w/H=0$. Momentum and buoyancy conventions must be consistent: with reduced pressure $\Phi=p'/\rho_0$, a pressure acceleration $-\nabla\Phi$ contains a vertical density-gradient term that is absent from $-\rho_0^{-1}\nabla p'$. The two expressions cannot be interchanged when deriving waves in a stratified atmosphere.

## Air pump

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Air_pump)

A device that transfers air into or out of a vessel. Historical vacuum experiments used a receiver, valves and a mechanical pump; leakage limited the attainable [pressure](pressure.md).

## Eddy

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A coherent or fluctuating swirling region of a [velocity field](#velocity-field). [Eddies](#eddy) transport [momentum](momentum.md), [heat](heat.md) and material constituents, and their averaged fluxes can modify a mean current. They need not be nonlinear: a linear [wave packet](dispersion-relation.md#wave-packet) can also have nonzero averaged quadratic fluxes.

## Wall slip

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

Relative tangential motion between material and its solid boundary. In [rheometry](rheology.md#rheometry) it can produce an apparent shear rate greater than the actual bulk rate and distort inferred [viscosity](dynamic-viscosity.md) or modulus.

## Focal length of a rotating liquid mirror

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A liquid in steady rigid rotation has a free surface $z-z_0=\Omega^2r^2/(2g)$. Comparing with a paraboloid $z-z_0=r^2/(4f)$ gives $f=g/(2\Omega^2)$. The result follows from [hydrostatic equilibrium](statistical-physics.md#hydrostatic-equilibrium) in the rotating frame and is independent of [density](#density).

## Pump

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A device that supplies mechanical energy to a fluid to drive a flow. A specified pump installation does not by itself determine the resulting [mass flow rate](#mass-flow-rate); the connected system's resistance also matters.

### Centrifugal pump

↑ **Parent:** [Pump](#pump)

A rotating-impeller [pump](#pump) that transfers mechanical energy to a fluid. At a fixed speed its head varies with flow; its characteristic curve and the connected system determine the [pump operating point](#pump-operating-point).

#### Pump operating point

↑ **Parent:** [Centrifugal pump](#centrifugal-pump)

The flow and head at which a pump's characteristic curve intersects the hydraulic system's required-head curve. Increasing system resistance at unchanged speed normally reduces flow on a conventional falling pump curve.[Module HT-03, pp.51–53, System Operating Point](engineering.md#thermodynamics-heat-transfer-and-fluid-flow-volume-3-by-the-united-states-department-of-energy)

## Hydraulic diameter

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

Four times a flow passage's cross-sectional area divided by its wetted perimeter. It provides a characteristic length for many internal-flow correlations, with applicability depending on geometry and flow regime.

## Computational fluid dynamics

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

Numerical solution of fluid-flow models. In [fossil](paleontology.md#fossil) functional analysis, reconstructed geometry, material assumptions and boundary conditions constrain the interpretation.

## Microfluidics

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Microfluidics)

[Microfluidics](#microfluidics) controls and studies small fluid volumes in confined channels. In cellular assays it can impose reproducible flow and chemical fields, but channel geometry, wall interactions and flow-induced stresses can themselves alter behaviour.

### Nanopore

↑ **Parent:** [Microfluidics](#microfluidics)

A [nanopore](#nanopore) is a channel or aperture with a nanometre-scale constriction. A solid-state realization can connect conducting liquid reservoirs, permitting ionic current to report particle passage through [resistive-pulse sensing](#resistive-pulse-sensing). A geometrical pore diameter alone does not determine its conductance: axial shape, reservoir access, surface charge, solution conductivity and interfacial effects can all matter. This definition concerns a physical aperture, without a biological application.

#### Ionic resistance of a conical pore

↑ **Parent:** [Nanopore](#nanopore)

In a one-dimensional Ohmic approximation, a linear conical frustum of [length](physics.md#length) $L$, end [radii](topology.md#radius) $a,b>0$ and ionic resistivity $\rho$ has $r(z)=a+(b-a)z/L$. Conservation of [electric current](electric-charge.md#electric-current) gives $d\mathcal R=\rho\,dz/[\pi r(z)^2]$. Integration yields the displayed resistance. Two identical opposed frusta, each of [length](physics.md#length) $l$, have resistance $2\rho l/(\pi ab)$, whether their central junction is the wider or narrower end. Their local field profiles nevertheless differ. The approximation neglects surface conduction and resistance outside the defined pore, and is not an exact three-dimensional field solution for arbitrary wall slope.

##### Electrophoretic transit time in a conical pore

↑ **Parent:** [Ionic resistance of a conical pore](#ionic-resistance-of-a-conical-pore)

For a point-like object with constant [electrophoretic mobility](physical-chemistry.md#electrophoretic-mobility), deterministic traversal is the integral of inverse local drift speed. In a conical frustum of [length](physics.md#length) $L$ at pore voltage $V$, the one-dimensional field is $E(z)=Vab/[Lr(z)^2]$. Integrating gives $t=L^2(b/a+1+a/b)/(3\mu V)$ for positive $\mu V$. For two symmetric frusta of total [length](physics.md#length) $2l$ and the same total pore voltage, replace $L$ by $2l$. The inequality $b/a+a/b\geq2$ shows that this nonuniform field cannot produce a shorter deterministic point-particle transit than a uniform field at fixed total [length](physics.md#length) and voltage. Reservoir [forces](force.md), [diffusion](thermodynamics.md#diffusion), adsorption and finite-object conformation are additional physics.

### Resistive-pulse sensing

↑ **Parent:** [Microfluidics](#microfluidics)

Electrical detection of particles passing through a conducting-liquid aperture. A particle changes the effective pore conductance transiently; pulse amplitude and duration depend on geometry, transport and interfacial charge, so calibration is essential.

#### Position-dependent resistive pulse

↑ **Parent:** [Resistive-pulse sensing](#resistive-pulse-sensing)

A small insulating object of excluded [volume](geometry-and-topology.md#volume) $\Omega$ perturbs an Ohmic pore most strongly where the pore cross-sectional [area](differential-geometry.md#surface-area) $A$ is small. In a local weak-blockage model, replacing a small conducting [volume](geometry-and-topology.md#volume) gives the displayed resistance scaling, with a shape-dependent coefficient. At fixed voltage, $\Delta I\simeq-I_0\Delta\mathcal R/\mathcal R_0$. A symmetric pore with narrow ends and a wide middle can therefore resolve two end features in a passage pulse. This is a conditional volume-exclusion model: charged-particle ion transport, surface interactions and bandwidth can change the observed sign, amplitude and shape.

## Magnus effect

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Magnus_effect)

The [Magnus effect](#magnus-effect) is a transverse [force](force.md) on a spinning body in relative motion through a [fluid](#fluid). Rotation changes the surrounding [circulation](vorticity.md#circulation-physics), [pressure](pressure.md) distribution and wake. In a two-dimensional cylinder model, the [Kutta–Joukowski theorem](#kutta-joukowski-theorem) gives [force](force.md) per unit span $\mathbf F'=\rho\mathbf U\times(\Gamma\hat{\mathbf z})$, with relative [fluid](#fluid) [velocity](classical-mechanics.md#velocity) $\mathbf U$ and [circulation](vorticity.md#circulation-physics) $\Gamma$ positive anticlockwise viewed from $+z$. Real [viscosity](dynamic-viscosity.md) and boundary-layer behavior help determine the [circulation](vorticity.md#circulation-physics); impermeability alone does not determine it from spin rate.

## Laminar flow

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Laminar_flow)

[Laminar flow](#laminar-flow) is a regime of [fluid flow](#fluid-flow) in which the motion remains organized, with neighboring fluid parcels following smooth, coherent paths rather than the irregular interacting fluctuations characteristic of [turbulence](turbulence.md). In a straight pipe, the simplest example consists of coaxial layers sliding past one another. This describes the character of the motion, not a requirement that every parcel have the same [velocity](classical-mechanics.md#velocity). Nor does it require [steady flow](#steady-flow): a smooth profile can evolve in time as [viscosity](dynamic-viscosity.md) transmits motion from a newly moving wall into a resting [fluid](#fluid). The unsteady wall-driven solution provides an explicit example. [Shreyas Mandre, Fluid Dynamics Lecture Notes, section 3.3](https://notes.shreyasmandre.com/fluid-dynamics-notes/Ch3.html)

The [Reynolds pipe-and-dye experiment](#reynolds-pipe-and-dye-experiment) makes this distinction visible. A thin injected dye band can remain coherent in [laminar flow](#laminar-flow), whereas irregular motion can fold it and carry dye across the pipe. However, [molecular diffusion](thermodynamics.md#molecular-diffusion) can spread dye even in [laminar flow](#laminar-flow), and an inlet disturbance can move a coherent band without producing [turbulence](turbulence.md). A dye band is a [streakline](#streakline), not a measurement of the entire [velocity field](#velocity-field); in [steady flow](#steady-flow) an ideal passive tracer's [streakline](#streakline) coincides with a [streamline](#streamline). Reynolds explicitly distinguished a wandering band from one broken into eddies. [Osborne Reynolds, An Experimental Investigation (1883), section 11, pp. 941–943](https://archive.org/stream/philtrans06508925/06508925_djvu.txt)

For a circular pipe of internal diameter $D$, define the mean axial [velocity](classical-mechanics.md#velocity) $U$ using the [volumetric flow rate](#volumetric-flow-rate) $Q$ and cross-sectional [area](differential-geometry.md#surface-area) $A$:

$$
A=\frac{\pi D^2}{4},\qquad U=\frac QA,\qquad
\mathrm{Re}_D=\frac{UD}{\nu}=\frac{\rho UD}{\mu}
=\frac{4Q}{\pi D\nu}.
$$

Here $\rho$ is [mass density](#density), $\mu$ is [dynamic viscosity](dynamic-viscosity.md) and $\nu=\mu/\rho$ is [kinematic viscosity](dynamic-viscosity.md#kinematic-viscosity). This particular [Reynolds number](dynamic-viscosity.md#reynolds-number) uses the diameter and mean [velocity](classical-mechanics.md#velocity), not the radius or centreline [velocity](classical-mechanics.md#velocity). Small [Reynolds number](dynamic-viscosity.md#reynolds-number) generally favors [laminar flow](#laminar-flow), but a single universal critical [Reynolds number](dynamic-viscosity.md#reynolds-number) does not distinguish it from [turbulence](turbulence.md) in all geometries and experiments. Even in a given pipe, inlet conditions and the magnitude of disturbances affect the observed onset. Reynolds demonstrated this dependence by deliberately inserting a wire coil. [Osborne Reynolds (1883), section 23, pp. 955–956](https://archive.org/stream/philtrans06508925/06508925_djvu.txt)

<a id="image-ideal-laminar-pipe-flow-zero-velocity-at-the-wall-and-twice-the-mean-velocity-at-the-centre"></a>
![](laminar-pipe-velocity-profile.png)

**[Figure 1](#image-ideal-laminar-pipe-flow-zero-velocity-at-the-wall-and-twice-the-mean-velocity-at-the-centre). Ideal laminar pipe flow: zero velocity at the wall and twice the mean velocity at the centre**. An illustrative fully developed Poiseuille solution, not measured data. The arrows and curve use a 10 mm diameter pipe with mean axial velocity 0.10 m/s. The dashed line marks the mean over the circular cross-section, not the mean along a diameter.

The quantitative example above assumes [steady flow](#steady-flow), [incompressible flow](#incompressible-flow), a [Newtonian fluid](viscous-fluid-flow.md#newtonian-fluid) with constant [dynamic viscosity](dynamic-viscosity.md), a straight horizontal circular pipe of radius $R=D/2$, stationary walls satisfying the [no-slip boundary condition](viscous-fluid-flow.md#no-slip-boundary-condition), and [fully developed flow](viscous-fluid-flow.md#fully-developed-flow). The last assumption means that the axial [velocity](classical-mechanics.md#velocity) profile no longer changes downstream. A positive [pressure](pressure.md) drop $\Delta p=p_{\rm in}-p_{\rm out}$ over a developed length $L$ gives the [Hagen-Poiseuille equation](viscous-fluid-flow.md#hagen-poiseuille-equation):

$$
u(r)=\frac{\Delta p}{4\mu L}(R^2-r^2)
=2U\left(1-\frac{r^2}{R^2}\right),\qquad
Q=\int_0^R u(r)\,2\pi r\,dr
=\frac{\pi R^4\Delta p}{8\mu L}.
$$

The [velocity](classical-mechanics.md#velocity) is zero at the wall and maximal at the centre. Averaging over the circular [area](differential-geometry.md#surface-area), whose annuli have [area](differential-geometry.md#surface-area) $2\pi r\,dr$, gives $U=u(0)/2$; averaging along one diameter would give a different answer. These assumptions produce a [parabola](euclidean-geometry.md#parabola), rather than every [laminar flow](#laminar-flow) having a parabolic profile. [Shreyas Mandre, Fluid Dynamics Lecture Notes, section 3.2.2, equations (3.9)–(3.11)](https://notes.shreyasmandre.com/fluid-dynamics-notes/Ch3.html)

As a stipulated calculation, take $D=0.010\,\mathrm m$, $U=0.10\,\mathrm{m\,s^{-1}}$, $\rho=1000\,\mathrm{kg\,m^{-3}}$, $\mu=0.0010\,\mathrm{Pa\,s}$ and $L=1.0\,\mathrm m$, and assume the developed [laminar flow](#laminar-flow) above. Then $\nu=10^{-6}\,\mathrm{m^2\,s^{-1}}$, $\mathrm{Re}_D=1000$, $u(0)=0.20\,\mathrm{m\,s^{-1}}$, $Q=7.85\times10^{-6}\,\mathrm{m^3\,s^{-1}}$ (about $0.471\,\mathrm{L\,min^{-1}}$), and $\Delta p=32\mu LU/D^2=32\,\mathrm{Pa}$. These are predictions from chosen parameters, not measurements or a claim that $\mathrm{Re}_D=1000$ guarantees [laminar flow](#laminar-flow) in every apparatus.

The beauty of this example is that a spatially varying [velocity field](#velocity-field) still gives an exact relation between two accessible measurements, [pressure](pressure.md) drop and [volumetric flow rate](#volumetric-flow-rate). It predicts the [hydraulic resistance](#hydraulic-resistance) $\Delta p/Q=8\mu L/(\pi R^4)$. Doubling the radius therefore multiplies $Q$ by sixteen at fixed [pressure](pressure.md) drop, length and [dynamic viscosity](dynamic-viscosity.md), provided the model remains applicable. This makes the [laminar flow](#laminar-flow) model useful for sizing narrow tubes or determining [dynamic viscosity](dynamic-viscosity.md). It also explains why a persistent narrow dye band can be informative without implying that the fluid is moving as a uniform plug.

### Reynolds pipe-and-dye experiment

↑ **Parent:** [Laminar flow](#laminar-flow)

In his 1883 paper, Osborne Reynolds investigated how the character of [pipe flow](viscous-fluid-flow.md#pipe-flow) depends jointly on [velocity](classical-mechanics.md#velocity), pipe diameter and [viscosity](dynamic-viscosity.md). His final dye apparatus drew water from a large glass tank through a horizontal glass tube with a smooth trumpet-shaped entrance. A separate reservoir supplied strongly colored water just upstream of the entrance; a valve below the tank controlled the outflow. The glass tube was immersed in the tank, so its internal dye band could be watched. Reynolds repeated the trials with different tube diameters and water [temperatures](temperature.md). [Osborne Reynolds (1883), sections 11 and 21–22, pp. 941–943 and 951–953](https://archive.org/stream/philtrans06508925/06508925_djvu.txt)

<a id="image-reynolds-pipe-and-dye-experiment-observe-the-dye-while-measuring-discharge-and-temperature"></a>
![](reynolds-pipe-dye-apparatus.png)

**[Figure 2](#image-reynolds-pipe-and-dye-experiment-observe-the-dye-while-measuring-discharge-and-temperature). Reynolds' pipe-and-dye experiment: observe the dye while measuring discharge and temperature**. Original schematic of the historical operating principle, not a scale reconstruction. A falling tank level determines discharged volume; timing it gives flow rate. The lower dye patterns are conceptual sketches of a coherent band and irregular spreading, not measured trajectories or concentration records.

The [volumetric flow rate](#volumetric-flow-rate) was measured independently of the appearance of the dye. Reynolds timed a one-inch fall of the tank's water level, corresponding to a calibrated discharged [volume](geometry-and-topology.md#volume). In modern notation, if this volume is $V$ and the elapsed time is $\Delta t$, then $Q=V/\Delta t$ and $U=4V/(\pi D^2\Delta t)$. He determined the glass tubes' internal diameters by filling them with water. For a uniform bore, a known filled length $\ell$ and measured water [volume](geometry-and-topology.md#volume) $V_{\rm tube}$ determine $D=\sqrt{4V_{\rm tube}/(\pi\ell)}$; checking bore uniformity matters because the same [volume](geometry-and-topology.md#volume) would only give an average cross-section in a tapered tube. Thermometers at different tank levels checked both the [temperature](temperature.md) and its uniformity. Reynolds compared the [viscosity](dynamic-viscosity.md) at different [temperatures](temperature.md) using Poiseuille's results and checked his own water by separate experiments of that type. Thus the [Reynolds number](dynamic-viscosity.md#reynolds-number) estimate did not come from judging the dye band or from assuming that transition occurred at a preset value. [Osborne Reynolds (1883), sections 21–22 and the reductions following Table I, pp. 951–955](https://archive.org/stream/philtrans06508925/06508925_djvu.txt)

A practical repetition can instead collect a known outflow [volume](geometry-and-topology.md#volume) in a measuring vessel and time its collection, or weigh the collected water and divide its [mass](classical-mechanics.md#mass) by [mass density](#density). Measure the internal diameter, rather than the external diameter, and obtain [kinematic viscosity](dynamic-viscosity.md#kinematic-viscosity) at the measured water [temperature](temperature.md) from independently established properties or a separate [viscosity](dynamic-viscosity.md) measurement. Record the dye appearance and observation position alongside $Q$, $D$, [temperature](temperature.md) and the resulting [Reynolds number](dynamic-viscosity.md#reynolds-number). These are alternative measurement procedures following $Q=V/\Delta t$, not additional historical claims about Reynolds' dye apparatus.

Begin with settled water and a small dye supply, then open the outlet valve in small steps. Reynolds saw a thin straight band at sufficiently low speeds. With a tank that had not fully settled, the band could wander while retaining its coherence. At higher discharge it could abruptly spread into the surrounding water downstream of the entrance. Short illumination by an electric spark resolved curls within what otherwise looked like a colored cloud. This connected the visible breakup with internal irregular motion rather than merely the appearance of an opaque pipe. [Osborne Reynolds (1883), sections 11 and 22, pp. 942 and 951–952](https://archive.org/stream/philtrans06508925/06508925_djvu.txt)

The controls are part of the result. Reynolds used a smooth entrance and let the tank rest to reduce inlet disturbances. He found that a heated tank could retain slow circulation as it cooled, so measuring one [temperature](temperature.md) was insufficient: thermal uniformity and residual motion also mattered. His wire-coil trial broke up the band below the previous onset speed, but he explicitly cautioned that once the dye was mixed he could not tell from that dye alone whether the motion became orderly again farther along the tube. In a repetition, keep the dye supply small enough to act approximately as a [passive scalar](scalar-transport.md#passive-scalar), avoid a strong injection jet, and record the inlet condition and downstream observation distance. If also testing the [Hagen-Poiseuille equation](viscous-fluid-flow.md#hagen-poiseuille-equation), allow the profile to develop and measure [pressure](pressure.md) drop between positions within the developed region; do not treat the entrance and outlet losses as part of its uniform [pressure gradient](#pressure-gradient). The dye experiment by itself does not establish [fully developed flow](viscous-fluid-flow.md#fully-developed-flow). [Osborne Reynolds (1883), sections 21–23 and 26, pp. 951–956 and 959](https://archive.org/stream/philtrans06508925/06508925_djvu.txt)

The experiment's usefulness is that it compares a visible change in the motion with independently measured scales. Repeating it with several diameters and [temperatures](temperature.md), while controlling disturbances, tests the organizing role of the [Reynolds number](dynamic-viscosity.md#reynolds-number). Its limitations are equally instructive: dye is a tracer of transport, [diffusion](thermodynamics.md#diffusion) still acts in [laminar flow](#laminar-flow), and a local dye observation cannot by itself prove that [turbulence](turbulence.md) persists throughout an arbitrarily long pipe.

## Void fraction

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

The [void fraction](#void-fraction) is the fraction of a mixture's local volume occupied by gas. For a horizontally uniform bubbly liquid it is the transported concentration in a one-dimensional gas-volume [continuity equation](mathematical-physics.md#continuity-equation). It is distinct from gas mass fraction because gas and liquid have different [mass densities](#density).

### Terminal-drift density law for compressible bubbles

↑ **Parent:** [Void fraction](#void-fraction)

For steady upward bubbles in a stationary liquid, assume fixed bubble [mass](classical-mechanics.md#mass), quadratic [drag force](#drag-physics), negligible gas weight and [inertia](classical-mechanics.md#inertia), and negligible wall force. Then $a\propto\rho_g^{-1/3}$. Hydrostatic mixture support and terminal [drag force](#drag-physics) balance give $v^2\propto a(1-\alpha)$. The gas [mass flux](mathematical-physics.md#mass-flux) $J=\alpha\rho_gv$ is constant, hence $J^2\propto\alpha^2(1-\alpha)\rho_g^{5/3}$. Comparing at a reference point proves the displayed relation. The approximation requires a small gas/liquid [mass density](#density) ratio and macroscopic variation scales; it need not hold near a gas-dominated endpoint or rapid acceleration region.

### Kinematic bubble transport in an exponentially narrowing vessel

↑ **Parent:** [Void fraction](#void-fraction)

If the vessel radius is proportional to $e^{-\beta z}$, its area is proportional to $e^{-2\beta z}$. Gas-volume conservation gives the displayed equation. Along concentration [characteristic curves](transport-equation.md#characteristic-curve), $\dot z=V_s(1-2\phi)$ and $\dot\phi=2\beta V_s\phi(1-\phi)$. Uniform initial concentration stays uniform in the uninterrupted bubbly region and follows this logistic law. Individual bubbles move at $V_s(1-\phi)$ instead: their rise distance there is $\eta=-(2\beta)^{-1}\log[\phi_0+(1-\phi_0)e^{-2\beta V_st}]$. Boundary interactions and dense-mixture backflow can invalidate the simplified closure.

### Bubble clearing in a cylindrical vessel

↑ **Parent:** [Void fraction](#void-fraction)

For initially uniform bubbles with upward speed $V_s(1-\phi)$, no new gas production and free escape at the top, gas conservation gives flux $V_s\phi(1-\phi)$. A clearing [shock](transport-equation.md#shock-wave) rises from the impermeable bottom with speed $V_s(1-\phi_0)$ by the [Rankine-Hugoniot condition](transport-equation.md#rankine-hugoniot-conditions). The displayed mean [void fraction](#void-fraction) averages the remaining uniform region over the whole liquid depth $H$. This assumes the dilute regime and no retained foam layer.

#### Incoming boundary condition in dense bubble clearing

↑ **Parent:** [Bubble clearing in a cylindrical vessel](#bubble-clearing-in-a-cylindrical-vessel)

For $\alpha_t+[V_s\alpha(1-\alpha)]_x=0$ in a finite upward pipe, bubbles move upward at $V_s(1-\alpha)$, but dense-mixture phase-fraction characteristics move downward. Hence an open upper end may be an incoming boundary for the scalar conservation law even though the bubbles themselves leave through it. Atmospheric pressure alone does not prescribe that incoming phase-fraction trace.

The bottom-clearing shock from zero to a uniform initial $\alpha_0$ has speed $V_s(1-\alpha_0)$. Continuing that constant right state to the outlet gives clearance time $L/[V_s(1-\alpha_0)]$, but at $\alpha_0>1/2$ it requires a compatible maintained incoming trace. For $\alpha_0=3/4$, the shock is $x=V_st/4$, and a right-state characteristic traced backward from it has initial position $3V_st/4$. It reaches the upper boundary at time $4L/(3V_s)$, before the formal clearance time $4L/V_s$. Later evolution therefore depends on the top closure. This boundary issue is distinct from the validity of the local slip and conservation derivation.

## Strouhal number

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

The Strouhal number compares the advective time $h/U$ with a prescribed forcing time $1/\omega$. Some conventions use ordinary frequency instead of angular frequency, introducing a factor $2\pi$. For a longitudinal disturbance extending over length $\lambda h$, the relevant ratio is $\lambda St$ rather than $St$ alone.

## Lift (force)

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](lift-force.md)

## Static pressure

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Static_pressure)

The local [fluid pressure](#fluid-pressure), distinguished from [dynamic pressure](lift-force.md#dynamic-pressure) and [stagnation pressure](#stagnation-pressure). "Static" does not require the [fluid](#fluid) to be stationary.

### Absolute pressure

↑ **Parent:** [Static pressure](#static-pressure)

[Pressure](pressure.md) referred to an ideal [vacuum](physics.md#vacuum), rather than to [atmospheric pressure](pressure.md#atmospheric-pressure) or another chosen reference. [Gauge pressure](#gauge-pressure) instead subtracts [atmospheric pressure](pressure.md#atmospheric-pressure).

### Stagnation pressure

↑ **Parent:** [Static pressure](#static-pressure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stagnation_pressure)

The [pressure](pressure.md) obtained by bringing a flow to rest without losses; in [compressible flow](compressible-flow.md) the usual definition specifies an [isentropic process](first-law-of-thermodynamics.md#isentropic-process) for stopping. For the constant-[mass density](#density), same-height [Bernoulli equation](euler-equations-for-an-inviscid-fluid.md#bernoulli-equation) discussed under [dynamic pressure](lift-force.md#dynamic-pressure), $p_0=p+q$.

#### Pitot tube

↑ **Parent:** [Stagnation pressure](#stagnation-pressure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pitot_tube)

An upstream-facing probe that senses [stagnation pressure](#stagnation-pressure). Determining [speed](classical-mechanics.md#speed) also requires a separate [static pressure](#static-pressure) and [mass density](#density).

##### Pitot-static tube

↑ **Parent:** [Pitot tube](#pitot-tube)

A combined [Pitot tube](#pitot-tube) and [static pressure](#static-pressure) probe with separate passages for the two [pressures](pressure.md).

## Manometer

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

An instrument for measuring [pressure](pressure.md) relative to another [pressure](pressure.md). A liquid-column [manometer](#manometer) uses [hydrostatic pressure](#hydrostatic-pressure); a digital [manometer](#manometer) uses a [pressure transducer](#pressure-transducer).

The appeal of a [liquid](thermodynamics.md#liquid)-column [manometer](#manometer) is that a [pressure measurement](pressure.md#pressure-measurement) becomes a visible [length](physics.md#length) measurement: [mass density](#density) and [gravitational acceleration](newton-s-law-of-universal-gravitation.md#gravitational-acceleration) supply the conversion. It can compare two [pressure tappings](lift-force.md#pressure-tapping) in a flowing [fluid](#fluid), even though the measuring [liquid](thermodynamics.md#liquid) itself must settle into [hydrostatic equilibrium](statistical-physics.md#hydrostatic-equilibrium). The reference connection determines which [pressure](pressure.md) difference is being measured.

### U-tube differential manometer

↑ **Parent:** [Manometer](#manometer)

A [U-tube differential manometer](#u-tube-differential-manometer) contains a connected column of [liquid](thermodynamics.md#liquid) with one [gas](thermodynamics.md#gas) connection above each [liquid meniscus](mixture.md#meniscus-liquid-surface). Write $p_L,p_R$ for the left and right [pressures](pressure.md), and $z_L,z_R$ for the meniscus heights on an upward vertical coordinate. Assume constant [mass density](#density) $\rho$ and downward [gravitational acceleration](newton-s-law-of-universal-gravitation.md#gravitational-acceleration) of magnitude $g$; neglect the [gas](thermodynamics.md#gas) column's [mass density](#density) and differences in [capillary pressure](surface-tension.md#capillary-pressure). The signed vertical [length](physics.md#length) difference $\Delta h=z_R-z_L$ then gives

$$
\Delta p=p_L-p_R=\rho g\Delta h.
$$

Larger left [pressure](pressure.md) means a lower left [liquid meniscus](mixture.md#meniscus-liquid-surface): $p_L>p_R$ implies $z_L<z_R$. Equal [pressures](pressure.md) give equal meniscus heights.

<a id="image-a-u-tube-differential-manometer-higher-left-pressure-lowers-the-left-liquid-meniscus"></a>
![](manometer-u-tube-signed-height.png)

**[Figure 3](#image-a-u-tube-differential-manometer-higher-left-pressure-lowers-the-left-liquid-meniscus). A U-tube differential manometer: higher left pressure lowers the left liquid meniscus**. Original schematic of two same-height [pressure tappings](lift-force.md#pressure-tapping) connected to a resting [water](chemical-substance.md#water) column. The constructed example uses $z_L=-30\,\mathrm{mm}$ and $z_R=30\,\mathrm{mm}$, so the vertical difference is $60\,\mathrm{mm}$. Dashed lines mark both meniscus heights and the equal-pressure datum; the dotted bottom line identifies two equal-height [points](geometry-and-topology.md#point-geometry) within the connected [liquid](thermodynamics.md#liquid). The arrow in the pipe indicates [fluid flow](#fluid-flow); the [manometer](#manometer) [liquid](thermodynamics.md#liquid) has no continuing flow at equilibrium.

The balance follows directly from [hydrostatic pressure](#hydrostatic-pressure). At a common height $z_0$ below both surfaces, the two [points](geometry-and-topology.md#point-geometry) in the connected homogeneous [liquid](thermodynamics.md#liquid) have equal [pressure](pressure.md):

$$
p_L+\rho g(z_L-z_0)=p_R+\rho g(z_R-z_0).
$$

Subtracting cancels the common bottom depth and leaves $p_L-p_R=\rho g(z_R-z_L)$. The same-height rule follows from [hydrostatic equilibrium](statistical-physics.md#hydrostatic-equilibrium), $\nabla p=-\rho g\mathbf e_z$: a horizontal displacement changes no [pressure](pressure.md), and for constant $\rho$ the quantity $p+\rho gz$ is constant throughout the connected [liquid](thermodynamics.md#liquid). Equal height alone is insufficient for unrelated vessels or for [fluid flow](#fluid-flow) with significant [acceleration](classical-mechanics.md#acceleration).

For an original constructed example, choose [water](chemical-substance.md#water) of stipulated [mass density](#density) $\rho=1000\,\mathrm{kg\,m^{-3}}$, [gravitational acceleration](newton-s-law-of-universal-gravitation.md#gravitational-acceleration) $g=9.81\,\mathrm{m\,s^{-2}}$, and vertical [length](physics.md#length) difference $\Delta h=0.060\,\mathrm m$. Then

$$
\Delta p=1000\times9.81\times0.060=588.6\,\mathrm{Pa}.
$$

The [SI](physics.md#international-system-of-units) [pressure](pressure.md) unit is the [pascal](physics.md#pascal-unit): the product has units $\mathrm{kg\,m^{-3}}\times\mathrm{m\,s^{-2}}\times\mathrm m=\mathrm{kg\,m^{-1}\,s^{-2}}=\mathrm{Pa}$. Swapping the two connections gives $-588.6\,\mathrm{Pa}$ and reverses which [liquid meniscus](mixture.md#meniscus-liquid-surface) is lower. In equal-bore arms, [volume conservation](mathematical-physics.md#volume-conservation) makes each surface move $30\,\mathrm{mm}$ from its initial equal-height position; using only one surface's displacement would halve the inferred [pressure](pressure.md). With unequal arm [areas](differential-geometry.md#surface-area) $A_L,A_R$, a left fall $a$ and right rise $b$ instead obey $A_La=A_Rb$, while the vertical [length](physics.md#length) difference is still $a+b$.

If the right port is open to the local atmosphere, $p_L-p_R$ is the left [gauge pressure](#gauge-pressure). Only with that reference and known [atmospheric pressure](pressure.md#atmospheric-pressure) can one obtain [absolute pressure](#absolute-pressure) from

$$
p_{L,\mathrm{abs}}=p_{\mathrm{atmosphere}}+p_{L,\mathrm{gauge}}.
$$

For an explicitly stipulated [atmospheric pressure](pressure.md#atmospheric-pressure) of $100000\,\mathrm{Pa}$, the example gives $100588.6\,\mathrm{Pa}$ [absolute pressure](#absolute-pressure). If the right port is connected to another vessel or a [pressure tapping](lift-force.md#pressure-tapping), the same reading is a differential [pressure](pressure.md) and supplies no [absolute pressure](#absolute-pressure) without knowing that reference.[§14.2, Gauge Pressure vs. Absolute Pressure, equation 14.11; Manometers](physics-bibliography.md#university-physics-volume-1-by-william-moebs-and-others)

#### Manometer height-to-pressure calibration

↑ **Parent:** [U-tube differential manometer](#u-tube-differential-manometer)

The ideal [measurement calibration](physics.md#measurement-calibration) is a straight line through the equal-pressure zero. For the stipulated [water](chemical-substance.md#water) [mass density](#density) and [gravitational acceleration](newton-s-law-of-universal-gravitation.md#gravitational-acceleration) above, its slope is $9.81\,\mathrm{Pa}$ per vertical millimetre. A lower [liquid](thermodynamics.md#liquid) [mass density](#density) gives a larger [length](physics.md#length) change for the same [pressure](pressure.md), improving the height-reading contribution to [measurement resolution](physics.md#measurement-resolution) but requiring more vertical space for a given [pressure](pressure.md) range. The [pressure](pressure.md) scale depends on the actual [mass density](#density), which depends on [temperature](temperature.md); $1000\,\mathrm{kg\,m^{-3}}$ here is a chosen model value, not an exact property of all [water](chemical-substance.md#water) samples.

<a id="image-calculated-water-column-pressure-scale-and-a-two-meniscus-rounding-model"></a>
![](manometer-height-pressure-resolution.png)

**[Figure 4](#image-calculated-water-column-pressure-scale-and-a-two-meniscus-rounding-model). Calculated water-column pressure scale and a two-meniscus rounding model**. The left panel is the theoretical [measurement calibration](physics.md#measurement-calibration) for $\rho=1000\,\mathrm{kg\,m^{-3}}$ and $g=9.81\,\mathrm{m\,s^{-2}}$. The right panel models two [liquid meniscus](mixture.md#meniscus-liquid-surface) heights read separately to the nearest millimetre: each rounding [measurement error](probability-and-statistics.md#measurement-error) is assumed independently uniform between $-0.5$ and $0.5\,\mathrm{mm}$. Their difference gives a triangular [probability density function](continuous-probability-distribution.md#probability-density-function) for the inferred [pressure](pressure.md) error. The bounds and [standard uncertainty](physics.md#standard-uncertainty) describe this constructed model, not observed instrument data.

Suppose each [liquid meniscus](mixture.md#meniscus-liquid-surface) height is rounded to the nearest scale division $q=1\,\mathrm{mm}$. Each height [measurement error](probability-and-statistics.md#measurement-error) lies within $q/2$, so the error in their difference lies within $q$. The resulting [pressure](pressure.md) error is bounded by $\rho gq=9.81\,\mathrm{Pa}$. To quantify a [standard uncertainty](physics.md#standard-uncertainty), make the additional model assumption that the two rounding errors are [independent random variables](random-variable.md#independent-random-variables), each having a [continuous uniform distribution](continuous-probability-distribution.md#continuous-uniform-distribution) on $[-q/2,q/2]$. Each then has [variance](variance.md) $q^2/12$; adding the two [variances](variance.md) gives

$$
u(\Delta h)=\frac{q}{\sqrt6},\qquad
u(\Delta p)=\frac{\rho gq}{\sqrt6}=4.0049\,\mathrm{Pa}.
$$

Here $u$ denotes [standard uncertainty](physics.md#standard-uncertainty). The $9.81\,\mathrm{Pa}$ worst-case bound and $4.0049\,\mathrm{Pa}$ [standard uncertainty](physics.md#standard-uncertainty) answer different questions. At $588.6\,\mathrm{Pa}$ they are respectively $1.67\%$ and $0.680\%$ of the reading. Shared reading bias or a different reading method can violate the assumed [independence](random-variable.md#independent-random-variables).

If the [mass density](#density), [gravitational acceleration](newton-s-law-of-universal-gravitation.md#gravitational-acceleration) and height difference also have small independent [standard uncertainties](physics.md#standard-uncertainty), a first-order estimate follows from the [partial derivatives](multivariable-calculus.md#partial-derivative) of $\Delta p=\rho g\Delta h$:

$$
u^2(\Delta p)\simeq(g\Delta h)^2u^2(\rho)+(\rho\Delta h)^2u^2(g)+(\rho g)^2u^2(\Delta h).
$$

This displays why a finer scale does not remove uncertainty in [mass density](#density) or [gravitational acceleration](newton-s-law-of-universal-gravitation.md#gravitational-acceleration). A [pressure transducer](#pressure-transducer) compared against the column needs its own [differential-pressure calibration](#differential-pressure-calibration) to establish an electrical response.

#### Water-column wind-tunnel pressure measurement

↑ **Parent:** [U-tube differential manometer](#u-tube-differential-manometer)

NASA's Wind Tunnel Experiment Details, slide 27, describes a practical [manometer](#manometer) measurement: partially fill a Tygon tube with [water](chemical-substance.md#water) and connect its two ends to [total pressure](#stagnation-pressure) and [static pressure](#static-pressure) ports in a [wind tunnel](#wind-tunnel). The [total pressure](#stagnation-pressure) connection pushes its [liquid meniscus](mixture.md#meniscus-liquid-surface) downward; the vertical [length](physics.md#length) difference supplies the [pressure](pressure.md) difference. The slide predicts increasing separation as the tunnel [speed](classical-mechanics.md#speed) increases. It supplies an apparatus and method, rather than a table of observed readings.[Wind Tunnel Experiment Details, slide 27: water-filled Tygon tube, total/static pressure ports and height readout](physics-bibliography.md#wind-tunnel-experiment-details-slide-27-by-nasa-glenn-research-center)

A control for this practical is to expose both connections to the same [atmospheric pressure](pressure.md#atmospheric-pressure) before the run: settled [liquid meniscus](mixture.md#meniscus-liquid-surface) heights should agree in a symmetric column. Read each [liquid meniscus](mixture.md#meniscus-liquid-surface) at eye level, reconnect sealed tubing to the identified ports, and wait for settling. Recheck the equal-pressure zero afterwards; reverse connections to check the sign. These checks establish neither [mass density](#density) nor ruler accuracy.[§14.2, Manometers, Figure 14.12(a): both arms open to atmosphere](physics-bibliography.md#university-physics-volume-1-by-william-moebs-and-others)

The inference is a differential [pressure](pressure.md) from [hydrostatic pressure](#hydrostatic-pressure), with [stagnation pressure](#stagnation-pressure) on one side and [static pressure](#static-pressure) on the other in NASA's practical. Converting that difference to a flow [speed](classical-mechanics.md#speed) additionally needs the hypotheses discussed under [dynamic pressure](lift-force.md#dynamic-pressure) and [Pitot-static tube](#pitot-static-tube). A changing [pressure](pressure.md) can leave the column oscillating; leaks, blocked [pressure tappings](lift-force.md#pressure-tapping) or trapped [liquid](thermodynamics.md#liquid) in a [gas](thermodynamics.md#gas) connection can alter or delay the readout. The column should be read after settling, and [temperature](temperature.md) should be recorded when choosing the measuring [liquid](thermodynamics.md#liquid)'s [mass density](#density).

Two corrections clarify the limits. If both [gas](thermodynamics.md#gas) ports are at the same height and carry the same [gas](thermodynamics.md#gas) of constant [mass density](#density) $\rho_g$, keeping its [hydrostatic pressure](#hydrostatic-pressure) gives $p_L-p_R=(\rho-\rho_g)g\Delta h$. Different port heights require their separate [gas](thermodynamics.md#gas) column heights. Also, a curved [liquid meniscus](mixture.md#meniscus-liquid-surface) can sustain a [capillary pressure](surface-tension.md#capillary-pressure) jump through [surface tension](surface-tension.md). Write $J_L,J_R$ for [liquid](thermodynamics.md#liquid) [pressure](pressure.md) minus [gas](thermodynamics.md#gas) [pressure](pressure.md) at the two surfaces. Neglecting [gas](thermodynamics.md#gas) weight, the balance becomes $p_L-p_R=\rho g\Delta h+J_R-J_L$. Identical meniscus shapes in matching clean bores cancel those jumps; unequal bores or different wetting conditions need not. Thus the useful simplicity of $\rho g\Delta h$ rests on identifiable physical conditions.

### McLeod gauge

↑ **Parent:** [Manometer](#manometer)

A [McLeod gauge](#mcleod-gauge) infers low [gas pressure](pressure.md#gas-pressure) by compressing a trapped [gas](thermodynamics.md#gas) sample into a calibrated smaller [volume](geometry-and-topology.md#volume).

## Pressure transducer

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

An instrument converting [pressure](pressure.md) or a [pressure](pressure.md) difference into a measurable signal. Its zero and scale must be checked separately, as illustrated by [differential-pressure calibration](#differential-pressure-calibration).

### Differential-pressure calibration

↑ **Parent:** [Pressure transducer](#pressure-transducer)

Checking the zero and scale of a differential [pressure transducer](#pressure-transducer) against equal port [pressures](pressure.md) and independently known [pressure](pressure.md) differences. The [dynamic pressure](lift-force.md#dynamic-pressure) measurement discussion gives a liquid-column check.

<h2 id="d-alembert-s-paradox">D'Alembert's paradox</h2>

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/D'Alembert's_paradox)

Ideal [steady flow](#steady-flow) with [incompressible flow](#incompressible-flow), [inviscid flow](#inviscid-flow) and [irrotational flow](vorticity.md#irrotational-flow) can predict zero [drag](#drag-physics) on a body that has nonzero [drag](#drag-physics) in a real [fluid](#fluid). The zero-[circulation](vorticity.md#circulation-physics) cylinder [pressure coefficient](lift-force.md#pressure-coefficient) distribution gives an explicit cancellation example; [viscosity](dynamic-viscosity.md) and [flow separation](continuum-mechanics.md#flow-separation) are absent from that model.

## Wind tunnel

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

An apparatus that produces controlled [fluid flow](#fluid-flow) past a model for measuring quantities such as [pressure](pressure.md), [lift](lift-force.md) and [drag](#drag-physics).

### Supersonic wind tunnel

↑ **Parent:** [Wind tunnel](#wind-tunnel)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Supersonic_wind_tunnel)

A [supersonic wind tunnel](#supersonic-wind-tunnel) produces controlled [supersonic flow](compressible-flow.md#supersonic-flow) in its test section. Its [nozzle](#nozzle) geometry and imposed [pressure](pressure.md) conditions set the test [Mach number](compressible-flow.md#mach-number).

## Airfoil

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Airfoil)

An [airfoil](#airfoil) (British spelling: [aerofoil](#airfoil)) is the cross-sectional profile of a lifting surface, such as a wing or blade. Its chord is the straight segment from leading edge to trailing edge, with length $c$; its mean camber line runs midway between its upper and lower surfaces, and its thickness measures their separation. Camber is the departure of that mean line from the chord. The [angle of attack](#angle-of-attack) describes the profile's orientation relative to the incoming flow. These independent choices let a designer alter the distribution of [pressure](pressure.md), [lift](lift-force.md) and [drag](#drag-physics), rather than simply enlarging the surface. [NASA Glenn, Wing Geometry, Airfoil Geometry subsection](https://www1.grc.nasa.gov/beginners-guide-to-aeronautics/wing-geometry/)

The distinction between an [airfoil](#airfoil) and a finite wing matters. A two-dimensional section model assumes no variation along span and predicts [lift](lift-force.md) per unit span $L'$. A wing of span $b$ has a spanwise distribution $L'(z)$ and total [lift](lift-force.md) $L=\int_{-b/2}^{b/2}L'(z)\,dz$. Its tip flow and trailing [vortices](critical-phenomenon.md#phase-vortex) generate a downward induced [velocity](classical-mechanics.md#velocity), called downwash, which changes the local flow seen by the sections. Thus one cannot generally multiply the isolated two-dimensional $L'$ by $b$. The wing aspect ratio $b^2/S$ measures its span relative to its reference area and helps characterize these three-dimensional effects. [James F. Marchman III, Aerodynamics and Aircraft Performance, chapter 3.4: finite wings](https://pressbooks.lib.vt.edu/aerodynamics/chapter/chapter-3-additional-aerodynamic-tools/)

For a thin section with small camber slopes and small [angle of attack](#angle-of-attack), [thin airfoil theory](#thin-airfoil-theory) predicts

$$
c_l\simeq2\pi(\alpha-\alpha_{L=0}),\qquad
\frac{dc_l}{d\alpha}\simeq2\pi,
$$

where both [angles](geometry-and-topology.md#angle) are in [radians](geometry-and-topology.md#radian) and $\alpha_{L=0}$ is the zero-lift [angle of attack](#angle-of-attack). The model assumes two-dimensional, [steady flow](#steady-flow), [incompressible flow](#incompressible-flow), [inviscid flow](#inviscid-flow), an attached outer flow, and smooth departure at a sharp trailing edge (the Kutta condition). This last condition selects the [circulation](vorticity.md#circulation-physics) used by the [Kutta–Joukowski theorem](#kutta-joukowski-theorem); with counterclockwise [circulation](vorticity.md#circulation-physics) $\Gamma$ positive and $\mathbf U_\infty=U_\infty\mathbf e_x$, that theorem gives $L'=-\rho_\infty U_\infty\Gamma$ for positive lift towards $+\mathbf e_y$. The beauty is that a detailed [velocity field](#velocity-field) collapses to a simple force law, while the geometry enters through $\alpha_{L=0}$. [MIT Unified Engineering, F3 lecture notes, pp. 2–4: camber and lift slope](https://ocw.mit.edu/courses/16-01-unified-engineering-i-ii-iii-iv-fall-2005-spring-2006/d721171c42af48a056aaccec784a6d10_f03_0304.pdf) [MIT Unified Engineering, F2 questions 7 and 9: symmetric sections and Kutta condition](https://ocw.mit.edu/courses/16-01-unified-engineering-i-ii-iii-iv-fall-2005-spring-2006/cc3f20c40c9451bde6a595fdd96a7e9e_f02_mud_0304.pdf)

A symmetric [airfoil](#airfoil) has $\alpha_{L=0}=0$ in this model: at $\alpha=4\,{}^\circ=\pi/45$ the predicted [lift coefficient](lift-force.md#lift-coefficient) is $c_l\simeq0.439$, and reversing $\alpha$ reverses [lift](lift-force.md). A stipulated cambered section with $\alpha_{L=0}=-2\,{}^\circ$ instead predicts $c_l\simeq0.219$ at zero [angle of attack](#angle-of-attack). These are ideal calculations, not measurements or guarantees for a particular profile. Air parcels on the upper and lower surfaces have no obligation to arrive together at the trailing edge; the [pressure](pressure.md) and [velocity field](#velocity-field) must satisfy the flow problem. A symmetric lifting section already makes an unequal-path-length explanation inadequate. [NASA Glenn, Bernoulli and Newton: the equal-transit explanation is incorrect](https://www1.grc.nasa.gov/beginners-guide-to-aeronautics/bernoulli-and-newton/)

Real [airfoils](#airfoil) have a viscous [boundary layer](continuum-mechanics.md#boundary-layer), even when [inviscid flow](#inviscid-flow) approximates the outer motion. At sufficiently demanding incidence, [flow separation](continuum-mechanics.md#flow-separation) can become extensive and the [lift coefficient](lift-force.md#lift-coefficient) departs from its approximately linear law, reaches a maximum and may fall: this is [aerodynamic stall](#aerodynamic-stall). [Lift](lift-force.md) does not generally vanish at [aerodynamic stall](#aerodynamic-stall). The onset depends on profile, [Reynolds number](dynamic-viscosity.md#reynolds-number), surface condition and motion history; $2\pi(\alpha-\alpha_{L=0})$ predicts neither a universal stall angle nor post-stall behavior. The pressure/balance experiment in [lift](lift-force.md) makes this limit observable by measuring changes in the surface [pressure](pressure.md) distribution alongside the total [force](force.md). [James F. Marchman, chapter 3.3: separation invalidates thin-airfoil assumptions](https://pressbooks.lib.vt.edu/aerodynamics/chapter/chapter-3-additional-aerodynamic-tools/)

### Angle of attack

↑ **Parent:** [Airfoil](#airfoil)

The signed [angle](geometry-and-topology.md#angle) between a lifting surface's chord and its incoming relative flow. Positive incidence in the planar convention used in [airfoil](#airfoil) raises the leading edge relative to the trailing edge in a horizontal left-to-right flow. It is distinct from orientation relative to the ground; an induced [velocity](classical-mechanics.md#velocity) can change the local effective incidence.

### Thin airfoil theory

↑ **Parent:** [Airfoil](#airfoil)

A small-disturbance, two-dimensional [potential flow](#potential-flow) model for a thin [airfoil](#airfoil), using surface tangency and smooth flow departure at its trailing edge to determine [circulation](vorticity.md#circulation-physics). Its [lift coefficient](lift-force.md#lift-coefficient) slope is $2\pi$ per [radian](geometry-and-topology.md#radian), with camber shifting the zero-lift [angle of attack](#angle-of-attack). See [airfoil](#airfoil) for assumptions, examples and the [aerodynamic stall](#aerodynamic-stall) limit.

### Aerodynamic stall

↑ **Parent:** [Airfoil](#airfoil)

A loss of the approximately attached-flow relation between [angle of attack](#angle-of-attack) and [lift coefficient](lift-force.md#lift-coefficient), associated with substantial [flow separation](continuum-mechanics.md#flow-separation). A stalled [airfoil](#airfoil) can still produce [lift](lift-force.md); its behavior must be measured or modeled beyond [thin airfoil theory](#thin-airfoil-theory).

## Uniform flow

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A uniform flow has the same [velocity](classical-mechanics.md#velocity) at every position. A constant velocity field has zero [divergence](multivariable-calculus.md#divergence) and zero [vorticity](vorticity.md); a [velocity potential](#velocity-potential) is $\phi(\mathbf x)=\mathbf U\cdot\mathbf x$. It describes the remote ambient flow in idealized obstacle and [line vortex](vorticity.md#line-vortex) problems.

## Volume viscosity

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Volume_viscosity)

Bulk viscosity is the dissipative response to a fluid's volume expansion or compression, distinct from the shear response. For a Newtonian isotropic fluid its isotropic dissipative stress includes $\zeta_B(\nabla\cdot\mathbf v)I$, and nonnegative $\zeta_B$ gives nonnegative compression-related dissipation. A condensate's relative-density-flow bulk coefficient must be identified from its particular hydrodynamic equation; it is not automatically numerically identical to a dimensional Newtonian viscosity.

## Hydraulic resistance

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[Hydraulic resistance](#hydraulic-resistance) relates the [pressure](pressure.md) drop across a resistive fluid element to its [volumetric flow rate](#volumetric-flow-rate). In a linear model, $\Delta p=RQ$ with $R>0$, so dissipated mechanical power is $\Delta p\,Q=RQ^2$. A peripheral circulatory bed can be represented by such a resistance when its detailed dynamics are not retained. This terminal [pressure](pressure.md)-to-flow resistance differs from the area-dependent friction rate multiplying [velocity](classical-mechanics.md#velocity) in a distributed tube momentum equation.

## Physiological fluid dynamics

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](physiological-fluid-dynamics.md)

### Hydraulic ladder network

↑ **Parent:** [Hydraulic resistance](#hydraulic-resistance)

A network of two resistive rails joined by multiple cross-links. Finite rail resistance makes cross-link flows unequal; maintaining a three-terminal equivalent permits exact recursive reduction.

### Delta-star transformation

↑ **Parent:** [Hydraulic resistance](#hydraulic-resistance)

Replacement of a three-edge triangular linear resistance network by a three-arm star with the same relation between terminal pressures and flows. Each star arm equals the product of its two adjacent triangle edges divided by the sum of all three edges.

## Fluid

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A [fluid](#fluid) is a material that flows under sustained [shear stress](viscous-fluid-flow.md#shear-stress) and cannot maintain a static [shear stress](viscous-fluid-flow.md#shear-stress) in its fluid state. [Liquids](thermodynamics.md#liquid) and [gases](thermodynamics.md#gas) are the usual examples. A [Newtonian fluid](viscous-fluid-flow.md#newtonian-fluid) has [deviatoric stress](continuum-mechanics.md#deviatoric-stress) proportional to its [rate-of-strain tensor](viscous-fluid-flow.md#strain-rate-tensor), whereas more general fluid [constitutive equations](continuum-mechanics.md#constitutive-equation) can be nonlinear or have memory. In a [porous medium](porous-media-flow.md#porous-medium), the [fluid](#fluid) occupies connected voids within a load-bearing [solid](thermodynamics.md#solid) framework. The important distinction is the response to a continuing tangential [force](force.md): an ordinary elastic [solid](thermodynamics.md#solid) can settle into a fixed [deformation](continuum-mechanics.md#deformation-mechanics), while an ordinary [fluid](#fluid) continues to deform. A [fluid](#fluid) can nevertheless be at rest when no unbalanced [shear stress](viscous-fluid-flow.md#shear-stress) drives it. [MIT, Fluid Dynamics of the Atmosphere and Ocean, lecture 3, pp. 4–5](https://ocw.mit.edu/courses/12-800-fluid-dynamics-of-the-atmosphere-and-ocean-fall-2004/7bb9e945405534b36776cbe404a8f839_lecture3.pdf)

For a worked example, place a [Newtonian fluid](viscous-fluid-flow.md#newtonian-fluid) between parallel plates separated by $h=1\,\mathrm{mm}$, keep the lower plate fixed and move the upper one at $U=0.10\,\mathrm{m\,s^{-1}}$. With [no-slip boundary conditions](viscous-fluid-flow.md#no-slip-boundary-condition), [steady flow](#steady-flow), no imposed [pressure gradient](#pressure-gradient) and negligible edge effects, [Couette flow](viscous-fluid-flow.md#couette-flow) has $u(y)=Uy/h$. For [dynamic viscosity](dynamic-viscosity.md) $\mu=0.001\,\mathrm{Pa\,s}$, the [shear stress](viscous-fluid-flow.md#shear-stress) magnitude is

$$
\tau=\mu\frac{du}{dy}=\mu\frac{U}{h}=0.10\,\mathrm{Pa}.
$$

The [velocity gradient](continuum-mechanics.md#velocity-gradient) describes neighbouring layers sliding at different speeds. Doubling $U$ doubles the required [shear stress](viscous-fluid-flow.md#shear-stress); maintaining the same [velocity](classical-mechanics.md#velocity) keeps producing [deformation](continuum-mechanics.md#deformation-mechanics), rather than fixing a final shape. This gives [viscosity](dynamic-viscosity.md) a concrete meaning: resistance to a rate of motion, not a prohibition on motion.

## Buoyant plume

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A buoyant plume rises because its density differs from the surrounding fluid and entrains ambient fluid as it travels.

## Pathline

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A [pathline](#pathline) records the motion of one identified [fluid element](continuum-mechanics.md#fluid-element): keep its starting position $\mathbf a$ and starting time $t_0$ fixed, and let physical time $t$ advance. In a [velocity field](#velocity-field) $\mathbf u(\mathbf x,t)$ its [Lagrangian trajectory](continuum-mechanics.md#lagrangian-trajectory) $\mathbf X(t;t_0,\mathbf a)$ solves the [initial value problem](differential-equation.md#initial-value-problem)

$$
\frac{d\mathbf X}{dt}=\mathbf u(\mathbf X(t),t),\qquad \mathbf X(t_0;t_0,\mathbf a)=\mathbf a.
$$

A [streamline](#streamline) instead freezes the time argument of the [velocity field](#velocity-field); a [streakline](#streakline) fixes the observation time and varies the release time of many [fluid elements](continuum-mechanics.md#fluid-element). A [pathline](#pathline) is useful for answering where a particular parcel goes and how long it takes, rather than merely which way the [fluid](#fluid) is moving now. [MIT Marine Hydrodynamics, lecture 2, sections 1.1–1.2](https://web.mit.edu/13.021/demos/lectures/lecture2.pdf)

For a concrete analytical model, take spatial coordinates $x,y$ in metres, time $t\geq0$ in seconds, and the spatially uniform but time-dependent [velocity field](#velocity-field)

$$
\mathbf u(x,y,t)=(U,at),\qquad U=1\ \mathrm{m\,s^{-1}},\qquad a=1\ \mathrm{m\,s^{-2}}.
$$

Its numerical components in these units are $(1,t)$. A [fluid element](continuum-mechanics.md#fluid-element) starting at the origin at $t_0=0$ has the [pathline](#pathline)

$$
x(t)=Ut,\qquad y(t)=\frac{at^2}{2},\qquad y=\frac{a}{2U^2}x^2.
$$

At $t=1\ \mathrm s$ it is at $(1,0.5)\ \mathrm m$; at $t=2\ \mathrm s$ it is at $(2,2)\ \mathrm m$. The [parabola](euclidean-geometry.md#parabola) records earlier, shallower [velocity](classical-mechanics.md#velocity) directions as well as the final direction. Differentiating gives $(\dot x,\dot y)=(U,at)$ and [acceleration](classical-mechanics.md#acceleration) $(0,a)$, so this curved [pathline](#pathline) needs no spatial variation of the [velocity field](#velocity-field). More generally the [chain rule](calculus.md#chain-rule) along a [pathline](#pathline) gives $d f(\mathbf X(t),t)/dt=\partial_t f+\mathbf u\cdot\nabla f$, the [material derivative](continuum-mechanics.md#material-derivative) of a transported [scalar field](classical-field-theory.md#scalar-field).

A motivating tracer demonstration appears in S. J. Kline's film notes: water passes through a contracting channel, and [hydrogen](chemical-substance.md#hydrogen) bubbles mark a small element at a wire at time $t_0$. The illustrated element is shown again $4.7\ \mathrm s$ later, with its accumulated [pathline](#pathline) superposed. Following that same marked element across successive film frames records a history; the entire bubble pattern in one frame has a different meaning. [S. J. Kline, Flow Visualization film notes, figures 7a–7c](https://web.mit.edu/hml/ncfmf/05FV.pdf)

For a modern version of the readout, use sparse small markers in a transparent water channel, illuminate the viewed plane, and keep an [optical camera](optical-instrument.md#optical-camera) fixed with a ruler in that plane. Record timestamps and track the same isolated marker between frames; successive positions estimate its [pathline](#pathline) and $[\mathbf X(t+\Delta t)-\mathbf X(t)]/\Delta t$ estimates its [velocity](classical-mechanics.md#velocity). A long exposure records a [pathline](#pathline) segment but loses the timing within it, so its total length divided by exposure time gives only mean [speed](classical-mechanics.md#speed). These are proposed measurement steps based on Jean Hertzberg's teaching guidance, rather than additional measurements from Kline's film. Markers leaving the viewed plane, overlapping tracks and perspective can break particle identification; repeat with a thinner viewed slice and a lower marker [concentration](mathematical-physics.md#concentration). [Jean Hertzberg and Flow Vis course students, Particles 4: Dilute Particle Techniques](https://www.flowvis.org/Flow%20Vis%20Guide/particles-4-dilute/)

## Control volume

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A [control volume](#control-volume) is a chosen region over which fluid [mass conservation](continuum-mechanics.md#mass-conservation) and momentum balance are integrated. It may be fixed or move with a prescribed [velocity](classical-mechanics.md#velocity). Boundary fluxes must use [velocity](classical-mechanics.md#velocity) relative to the moving boundary. In [Stokes flow](stokes-flow.md), negligible inertia reduces the momentum balance to the sum of body [forces](force.md) and boundary tractions, making a carefully chosen [control volume](#control-volume) useful for finding drag without integrating directly over a curved body.

## Navier slip boundary condition

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

The [Navier slip boundary condition](#navier-slip-boundary-condition) allows a [fluid](#fluid) to slide tangentially past a solid wall while resisting that motion through [wall friction in the Navier slip boundary condition](#wall-friction-in-the-navier-slip-boundary-condition). For parallel flow past a flat, impermeable wall translating uniformly with tangential [velocity](classical-mechanics.md#velocity) $U_w$, write the fluid's tangential [velocity](classical-mechanics.md#velocity) as $u$ and its relative tangential [velocity](classical-mechanics.md#velocity) as $u_{\mathrm{rel}}=u-U_w$. Then

$$
u_{\mathrm{rel}}=b\partial_nu,\qquad b\ge0,
$$

where $b$ is the [slip length](#slip-length), also written $\ell_s$. The [unit normal](differential-geometry.md#unit-normal) $\mathbf n$ points from the wall into the [fluid](#fluid), and $\partial_nu=\mathbf n\cdot\nabla u$ is the [normal derivative](differential-geometry.md#normal-derivative). The separate [no-penetration boundary condition](viscous-fluid-flow.md#no-penetration-boundary-condition) requires $(\mathbf u-\mathbf U_w)\cdot\mathbf n=0$: tangential sliding does not allow flow through the wall.

The sign convention matters. In a channel $0<z<H$, the lower wall has inward [unit normal](differential-geometry.md#unit-normal) $+\mathbf e_z$ and the upper wall has inward [unit normal](differential-geometry.md#unit-normal) $-\mathbf e_z$. If both walls obey the [Navier slip boundary condition](#navier-slip-boundary-condition), their tangential [velocities](classical-mechanics.md#velocity) satisfy

$$
u(0)-U_0=b_0u'(0),\qquad
u(H)-U_H=-b_Hu'(H).
$$

Here the prime means the [derivative](calculus.md#derivative) with respect to $z$. Using $+b_Hu'(H)$ at the upper wall would reverse the friction law. The examples [Couette flow with a slipping lower wall](#couette-flow-with-a-slipping-lower-wall) and [planar Poiseuille flow with equal wall slip](#planar-poiseuille-flow-with-equal-wall-slip) use different upper-wall [boundary conditions](differential-equation.md#boundary-condition).

This flat-wall formula is a local linear model. On a curved wall the [Newtonian fluid stress tensor](viscous-fluid-flow.md#newtonian-fluid-stress-tensor) must supply the tangential [traction](continuum-mechanics.md#traction); the [normal derivative](differential-geometry.md#normal-derivative) alone generally misses curvature terms. The author-written review by Lauga, Brenner and Stone states the full strain-based condition with the [unit normal](differential-geometry.md#unit-normal) directed into the liquid. [Lauga, Brenner and Stone, Microfluidics: The No-Slip Boundary Condition (2005), §2.1, equation (2)](https://arxiv.org/pdf/cond-mat/0501557)

The same review credits Navier's 1823 treatise with the linear slip law. Its history is a reminder that the [no-slip boundary condition](viscous-fluid-flow.md#no-slip-boundary-condition) is an experimentally successful model, whose validity depends on the interface and scale. The history here follows that review rather than a new reading of Navier's original memoir. [Lauga, Brenner and Stone (2005), §2.1: the nineteenth-century boundary-condition debate](https://arxiv.org/pdf/cond-mat/0501557)

### Slip length

↑ **Parent:** [Navier slip boundary condition](#navier-slip-boundary-condition)

The [slip length](#slip-length) measures tangential wall mobility in the [Navier slip boundary condition](#navier-slip-boundary-condition). Where the wall [shear rate](viscous-fluid-flow.md#shear-rate) is nonzero,

$$
b=\frac{u_{\mathrm{rel}}}{\partial_nu}.
$$

The numerator is a [velocity](classical-mechanics.md#velocity) and the denominator has units $\mathrm{s^{-1}}$, so $b$ has units of length. Geometrically, take a local inward normal coordinate $s$, with the wall at $s=0$. The tangent line to the relative [velocity](classical-mechanics.md#velocity) profile is

$$
u_{\mathrm{rel,lin}}(s)=u_{\mathrm{rel}}(0)+s\partial_nu(0)
=(b+s)\partial_nu(0).
$$

It reaches zero at $s=-b$, a fictitious distance $b$ inside the solid. This extrapolation does not assert that [fluid](#fluid) exists there. At a moving wall, extrapolate to the wall's [velocity](classical-mechanics.md#velocity), rather than to zero laboratory [velocity](classical-mechanics.md#velocity). If both the wall [shear rate](viscous-fluid-flow.md#shear-rate) and relative [velocity](classical-mechanics.md#velocity) vanish, their ratio cannot determine $b$.

The useful comparison is $b/H$, where $H$ is the channel gap. A small absolute [slip length](#slip-length) can noticeably change [volumetric flow rate](#volumetric-flow-rate) in a micrometre-scale channel. Measured effective [slip length](#slip-length) may summarize unresolved interfacial structure; it need not mean literal molecular sliding at every point. The review distinguishes intrinsic, apparent and effective slip and discusses how surface conditions affect measurements. [Lauga, Brenner and Stone (2005), §§2.2 and 3.1: slip terminology and measurement](https://arxiv.org/pdf/cond-mat/0501557)

#### Couette flow with a slipping lower wall

↑ **Parent:** [Slip length](#slip-length)

Consider [steady flow](#steady-flow) of a [Newtonian fluid](viscous-fluid-flow.md#newtonian-fluid) in [incompressible flow](#incompressible-flow) with constant [dynamic viscosity](dynamic-viscosity.md) $\mu>0$ between parallel plates at $z=0$ and $z=H$. The bottom plate is stationary and obeys the [Navier slip boundary condition](#navier-slip-boundary-condition) with [slip length](#slip-length) $b$. The top plate moves at [velocity](classical-mechanics.md#velocity) $U>0$ and obeys the [no-slip boundary condition](viscous-fluid-flow.md#no-slip-boundary-condition). There is no streamwise [pressure gradient](#pressure-gradient) or body [force](force.md). The [Couette flow](viscous-fluid-flow.md#couette-flow) solution is

$$
u(z)=U\frac{z+b}{H+b},\qquad
u(0)=\frac{Ub}{H+b},\qquad
\tau=\mu u'(z)=\frac{\mu U}{H+b}.
$$

Here $\tau$ is the constant [shear stress](viscous-fluid-flow.md#shear-stress) magnitude. The lower wall's [Navier slip boundary condition](#navier-slip-boundary-condition) holds exactly because $bu'(0)=bU/(H+b)=u(0)$. At the top, $u(H)=U$ is exactly the prescribed [no-slip boundary condition](viscous-fluid-flow.md#no-slip-boundary-condition); no finite upper-wall [slip length](#slip-length) is imposed in this example.

For a numerical example, stipulate $H=10\,\mathrm{\mu m}$, $b=2\,\mathrm{\mu m}$, $U=1\,\mathrm{mm\,s^{-1}}$ and $\mu=10^{-3}\,\mathrm{Pa\,s}$. The bottom [velocity](classical-mechanics.md#velocity) is $0.167\,\mathrm{mm\,s^{-1}}$ and the [shear stress](viscous-fluid-flow.md#shear-stress) is $0.0833\,\mathrm{Pa}$, compared with $0.100\,\mathrm{Pa}$ when both plates obey the [no-slip boundary condition](viscous-fluid-flow.md#no-slip-boundary-condition). The extrapolated profile reaches zero at $z=-2\,\mathrm{\mu m}$.

<a id="image-couette-profiles-reveal-slip-length-by-extrapolation-beneath-the-lower-wall"></a>
![](navier-slip-couette.png)

**[Figure 5](#image-couette-profiles-reveal-slip-length-by-extrapolation-beneath-the-lower-wall). Couette profiles reveal slip length by extrapolation beneath the lower wall**. The bottom wall is stationary with [slip length](#slip-length) $b$; the upper wall at $z=H$ moves at [velocity](classical-mechanics.md#velocity) $U$ with a [no-slip boundary condition](viscous-fluid-flow.md#no-slip-boundary-condition). Solid lines show [Couette flow](viscous-fluid-flow.md#couette-flow) for $b/H=0$, $0.25$ and $0.75$. Dashed continuations inside the shaded solid reach zero at $z=-b$. Increasing [slip length](#slip-length) reduces the [shear rate](viscous-fluid-flow.md#shear-rate) required for the same upper-wall [velocity](classical-mechanics.md#velocity).

For fixed $H$, $U$ and $\mu$, $b\to0$ recovers $u=Uz/H$. As $b\to\infty$, $u\to U$ throughout the gap and $\tau\to0$: the moving upper wall selects the limiting uniform [velocity](classical-mechanics.md#velocity), while the lower wall approaches a [stress-free boundary condition](viscous-fluid-flow.md#stress-free-boundary-condition). The [dynamic viscosity](dynamic-viscosity.md) stays positive; the disappearing [shear stress](viscous-fluid-flow.md#shear-stress) comes from the disappearing [velocity gradient](continuum-mechanics.md#velocity-gradient).

A short derivation uses [unidirectional flow](#unidirectional-flow): the [convective acceleration](continuum-mechanics.md#convective-acceleration) vanishes and the [Navier-Stokes equation](viscous-fluid-flow.md#navier-stokes-equation) reduces to $\mu u''=0$. Write $u=Az+B$. The bottom condition gives $B=bA$ and the top condition gives $A(H+b)=U$.

#### Planar Poiseuille flow with equal wall slip

↑ **Parent:** [Slip length](#slip-length)

Now both plates at $z=0$ and $z=H$ are stationary and both obey the [Navier slip boundary condition](#navier-slip-boundary-condition) with the same [slip length](#slip-length) $b$. Drive [steady flow](#steady-flow) of a [Newtonian fluid](viscous-fluid-flow.md#newtonian-fluid) in [incompressible flow](#incompressible-flow) by the constant [pressure gradient](#pressure-gradient) $G=-dp/dx>0$, with constant [dynamic viscosity](dynamic-viscosity.md) $\mu>0$ and no other streamwise body [force](force.md). The planar [Poiseuille flow](viscous-fluid-flow.md#hagen-poiseuille-equation) profile and its [volumetric flow rate](#volumetric-flow-rate) per unit width are

$$
u(z)=\frac{G}{2\mu}\left[z(H-z)+bH\right],\qquad
q=\int_0^H u(z)\,dz
=\frac{GH^3}{12\mu}\left(1+\frac{6b}{H}\right).
$$

The full [volumetric flow rate](#volumetric-flow-rate) for channel width $W$ is $Q=Wq$ when side-wall effects are negligible. Thus $q$ has units $\mathrm{m^2\,s^{-1}}$, while $Q$ has units $\mathrm{m^3\,s^{-1}}$. Denote the value at $b=0$ by $q_0=GH^3/(12\mu)$.

The two wall checks expose the normal signs:

$$
u'(z)=\frac{G}{2\mu}(H-2z),\qquad
u(0)=u(H)=\frac{GbH}{2\mu},
$$



$$
bu'(0)=\frac{GbH}{2\mu}=u(0),\qquad
-bu'(H)=\frac{GbH}{2\mu}=u(H).
$$

Both [Navier slip boundary conditions](#navier-slip-boundary-condition) therefore hold exactly. The two walls exert backward tangential [tractions](continuum-mechanics.md#traction) of magnitude $GH/2$ on the [fluid](#fluid). Increasing $b$ at fixed $G$ adds a uniform [velocity](classical-mechanics.md#velocity) offset, leaving the [velocity gradient](continuum-mechanics.md#velocity-gradient) and wall [shear stress](viscous-fluid-flow.md#shear-stress) unchanged. This differs from [Couette flow with a slipping lower wall](#couette-flow-with-a-slipping-lower-wall), where upper-wall [velocity](classical-mechanics.md#velocity) is fixed and [shear stress](viscous-fluid-flow.md#shear-stress) decreases.

For $H=10\,\mathrm{\mu m}$, $b=2\,\mathrm{\mu m}$, $G=10^3\,\mathrm{Pa\,m^{-1}}$ and $\mu=10^{-3}\,\mathrm{Pa\,s}$, the wall [velocity](classical-mechanics.md#velocity) is $10\,\mathrm{\mu m\,s^{-1}}$, the centre [velocity](classical-mechanics.md#velocity) is $22.5\,\mathrm{\mu m\,s^{-1}}$, and $q=1.83\times10^{-10}\,\mathrm{m^2\,s^{-1}}$. The enhancement is $q/q_0=2.2$. Equivalently, a prescribed [volumetric flow rate](#volumetric-flow-rate) needs only $1/2.2$ of the original [pressure gradient](#pressure-gradient). This makes [slip length](#slip-length) useful for estimating pumping requirements in small channels.

<a id="image-equal-slip-at-both-channel-walls-increases-pressure-driven-flow"></a>
![](navier-slip-channel-flow.png)

**[Figure 6](#image-equal-slip-at-both-channel-walls-increases-pressure-driven-flow). Equal slip at both channel walls increases pressure-driven flow**. Both walls are stationary and obey the [Navier slip boundary condition](#navier-slip-boundary-condition). Left: normalized planar [Poiseuille flow](viscous-fluid-flow.md#hagen-poiseuille-equation) profiles at fixed [pressure gradient](#pressure-gradient) $G$, gap $H$ and [dynamic viscosity](dynamic-viscosity.md) $\mu$ for $b/H=0$, $0.10$ and $0.25$. Arrows show inward [unit normals](differential-geometry.md#unit-normal) in opposite directions at the two walls. Right: [volumetric flow rate](#volumetric-flow-rate) per unit width increases by the factor $1+6b/H$ at fixed $G$.

At fixed $H$, $G>0$ and $\mu$, $b\to0$ recovers ordinary planar [Poiseuille flow](viscous-fluid-flow.md#hagen-poiseuille-equation). As $b\to\infty$, the [velocity](classical-mechanics.md#velocity) and $q$ grow without bound in this model, although the varying part of the profile stays the same. At exactly zero tangential wall [traction](continuum-mechanics.md#traction), no steady solution can balance this nonzero [pressure gradient](#pressure-gradient): $u'(0)=u'(H)=0$ conflicts with $\mu[u'(H)-u'(0)]=-GH$. Unlimited enhancement is consequently not a prediction for a real channel; finite wall friction, finite driving capacity and the validity of the assumed [steady flow](#steady-flow) must be assessed. At fixed finite $q$ instead, $G\to0$ and the profile approaches uniform [velocity](classical-mechanics.md#velocity) $q/H$.

A short derivation integrates the reduced [Navier-Stokes equation](viscous-fluid-flow.md#navier-stokes-equation) $\mu u''=-G$ twice. Equal [slip lengths](#slip-length) and the opposite inward [unit normals](differential-geometry.md#unit-normal) give $u=G[z(H-z)+bH]/(2\mu)$. Its [integral](integral.md) over the gap supplies the enhancement factor $1+6b/H$.

### Wall friction in the Navier slip boundary condition

↑ **Parent:** [Navier slip boundary condition](#navier-slip-boundary-condition)

For a [Newtonian fluid](viscous-fluid-flow.md#newtonian-fluid) and a flat wall with $0<b<\infty$, the [Navier slip boundary condition](#navier-slip-boundary-condition) is equivalent to a tangential wall-on-fluid [traction](continuum-mechanics.md#traction)

$$
t_{w,t}=-\frac{\mu}{b}u_{\mathrm{rel}}.
$$

The sign expresses resisting [friction](newtonian-mechanics.md#friction): $\partial_nu$ uses the inward [unit normal](differential-geometry.md#unit-normal), whereas the wall-on-fluid [traction](continuum-mechanics.md#traction) uses the outward [unit normal](differential-geometry.md#unit-normal) of the fluid domain. The irreversible loss of mechanical [energy](energy.md) per unit wall [area](differential-geometry.md#surface-area) and time is

$$
\mathcal D_w=-t_{w,t}u_{\mathrm{rel}}
=\frac{\mu}{b}u_{\mathrm{rel}}^2\ge0,
\qquad [\mathcal D_w]=\mathrm{W\,m^{-2}}.
$$

For two tangential directions replace $u_{\mathrm{rel}}^2$ by the squared [Euclidean norm](normed-vector-space.md#euclidean-norm) of relative tangential [velocity](classical-mechanics.md#velocity). At a moving wall this relative-[velocity](classical-mechanics.md#velocity) loss must be distinguished from the [power](energy.md#power) supplied by the wall's motion. Bulk [viscous dissipation](stokes-flow.md#viscous-dissipation) also remains present. A finite [slip length](#slip-length) models reduced interfacial resistance, without declaring every boundary ideal or removing [dynamic viscosity](dynamic-viscosity.md).

The limiting loss depends on how the flow is driven. In [Couette flow with a slipping lower wall](#couette-flow-with-a-slipping-lower-wall),

$$
\mathcal D_w=\frac{\mu U^2b}{(H+b)^2}.
$$

It tends to zero for both $b\to0$ and $b\to\infty$ at fixed $H$ and $U$. At $b=0$ impose the [no-slip boundary condition](viscous-fluid-flow.md#no-slip-boundary-condition) directly, rather than dividing by zero. In [planar Poiseuille flow with equal wall slip](#planar-poiseuille-flow-with-equal-wall-slip) at fixed $G$, each wall instead dissipates $G^2bH^2/(4\mu)$, which grows with $b$ because relative [velocity](classical-mechanics.md#velocity) grows. The bulk loss per unit width is $G^2H^3/(12\mu)$; adding both wall losses gives $Gq$, the [pressure](pressure.md) work per unit channel length and width. This [energy](energy.md) balance shows why small friction coefficients do not guarantee small losses under every driving constraint.

## Fluid free boundary

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A [fluid free boundary](#fluid-free-boundary) is an initially unknown material interface separating a fluid from its exterior. For a [polytropic elliptical patch in a shearing sheet](gravitational-instability-of-an-astrophysical-disk.md#polytropic-elliptical-patch-in-a-shearing-sheet) bounded by vacuum, it is the level set $p=\rho=Q=0$, and the velocity is tangent to it in a steady solution.

## Material surface

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A material surface is transported with its [fluid elements](continuum-mechanics.md#fluid-element), including its boundary when open. Its oriented [material surface element](#material-surface-element) evolves by tangent transport. [Magnetic flux freezing](ideal-magnetohydrodynamics.md#magnetic-flux-freezing) conserves the flux through such an open surface.

### Material surface element

↑ **Parent:** [Material surface](#material-surface)

If $\mathbf A=\mathbf t_a\times\mathbf t_b\,da\,db$ and each tangent satisfies $D\mathbf t/Dt=(\nabla\mathbf u)\mathbf t$, differentiation of the cross product gives $D\mathbf A/Dt=(\nabla\cdot\mathbf u)\mathbf A-(\nabla\mathbf u)^T\mathbf A$. Combining this with ideal induction proves pointwise conservation of $\mathbf B\cdot\mathbf A$.

#### Material surface element evolution

↑ **Parent:** [Material surface element](#material-surface-element)

Parameterize a [material surface](#material-surface) by fixed particle labels $a,b$, with tangents $\mathbf a=\partial_a\mathbf x$, $\mathbf b=\partial_b\mathbf x$. The [material derivative](continuum-mechanics.md#material-derivative) gives $D\mathbf a/Dt=(\nabla\mathbf u)\mathbf a$ and similarly for $\mathbf b$. Differentiate $d\mathbf S=(\mathbf a\times\mathbf b)\,da\,db$ and use the [cross product](vector-space.md#cross-product) identity

$$
(A\mathbf a)\times\mathbf b+\mathbf a\times(A\mathbf b)
=[(\operatorname{tr}A)\mathsf I-A^{\mathsf T}](\mathbf a\times\mathbf b).
$$

This proves the displayed oriented-area evolution law, with $(\nabla\mathbf u)_{ij}=\partial_ju_i$. It allows both area change and rotation; even [incompressible flow](#incompressible-flow) need not preserve the magnitude of a material area element.

## Material curve

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A material curve consists of the same [fluid elements](continuum-mechanics.md#fluid-element) at all times. Differentiating their flow map gives $D\boldsymbol\ell/Dt=(\boldsymbol\ell\cdot\nabla)\mathbf u$ for its tangent. In [ideal magnetohydrodynamics](ideal-magnetohydrodynamics.md) a magnetic-field tangent obeys this same transport law after division by [mass density](#density).

## Scalar transport

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](scalar-transport.md)

## Fluid flow

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A [fluid flow](#fluid-flow) is motion described by a [velocity field](#velocity-field) $\mathbf u(\mathbf x,t)$. The trajectories of [fluid elements](continuum-mechanics.md#fluid-element) satisfy $d\mathbf x/dt=\mathbf u(\mathbf x,t)$; the [mass density](#density) and other fields obey their [conservation laws](mathematical-physics.md#conservation-law) and [constitutive equations](continuum-mechanics.md#constitutive-equation). This physical motion differs from a [flow](flow-network.md#flow) on a [flow network](flow-network.md).

### Airflow

↑ **Parent:** [Fluid flow](#fluid-flow)

### Unidirectional flow

↑ **Parent:** [Fluid flow](#fluid-flow)

A unidirectional flow has velocity parallel to a single fixed direction, for example $\boldsymbol u=u(y)\boldsymbol e_x$. If the speed is independent of the coordinate along that direction, the convective acceleration $(\boldsymbol u\cdot\nabla)\boldsymbol u$ vanishes. The steady [Navier-Stokes equation](viscous-fluid-flow.md#navier-stokes-equation) then reduces to a linear balance of the pressure gradient and viscosity, as in [Couette flow](viscous-fluid-flow.md#couette-flow) and [Poiseuille flow](viscous-fluid-flow.md#hagen-poiseuille-equation).

### Steady flow

↑ **Parent:** [Fluid flow](#fluid-flow)

In steady flow, the velocity and other relevant flow fields are independent of time in the chosen reference frame. [Streamlines](#streamline) then coincide with the paths of moving particles, while [convective acceleration](continuum-mechanics.md#convective-acceleration) can still be nonzero.

### Inviscid flow

↑ **Parent:** [Fluid flow](#fluid-flow)

An inviscid flow neglects [viscosity](dynamic-viscosity.md) in the [fluid flow](#fluid-flow). Its [momentum](momentum.md) balance is described by the [Euler equations for an inviscid fluid](euler-equations-for-an-inviscid-fluid.md).

#### Inviscid falling jet and radial impact film

↑ **Parent:** [Inviscid flow](#inviscid-flow)

A steady incompressible jet at atmospheric [pressure](pressure.md) conserves [Bernoulli's equation](euler-equations-for-an-inviscid-fluid.md#bernoulli-equation) and [volume flux](#volumetric-flow-rate). Its radius contracts as $R=a[u/u_0]^{-1/2}$. After impact, a thin nearly horizontal axisymmetric film has $2\pi rhv=\pi a^2u_0$. Evaluating [Bernoulli's equation](euler-equations-for-an-inviscid-fluid.md#bernoulli-equation) on its [free surface](#free-surface) gives $v^2=u_0^2+2g(H-h)$, hence $a^4/(4r^2h^2)=1+2g(H-h)/u_0^2$. This inviscid thin-film description applies away from the impact region and does not describe a dissipative hydraulic jump.

## Sediment transport

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sediment_transport)

### Relaxation-controlled antidune instability

↑ **Parent:** [Sediment transport](#sediment-transport)

In a reduced [sediment](planetary-science.md#sediment)-bed model with normalized discharge one, water momentum gives $s=1-u^{-1}+F^2(1-u^2)/2$, while [concentration](mathematical-physics.md#concentration) adaptation and bed exchange give $c_x=E(u)-c=-s_t$. Linearizing about $u=c=1,s=0$ yields $\widetilde s=(1-F^2)\widetilde u$ and $(1+ik)\widetilde c=E'(1)\widetilde u$. Elimination proves the displayed dispersion relation.

For $E'(1)>0$, the [growth rate](dispersion-relation.md#growth-rate) is $E'(1)k^2/[(F^2-1)(1+k^2)]$, positive exactly on the supercritical side $F>1$ for nonzero $k$. The [phase speed](dispersion-relation.md#phase-speed) is $-E'(1)/[(F^2-1)(1+k^2)]$, so unstable bedforms migrate upstream and are [antidunes](#antidune). At high [wavenumber](wave-equation.md#wavenumber) growth approaches a finite plateau rather than becoming unbounded. This closure selects no finite fastest wavelength; short-scale selection needs additional physics. The critical limit $F=1$ and a vanishing [entrainment](#fluid-entrainment) [derivative](calculus.md#derivative) are degenerate cases outside the displayed conclusion.

### Bedload transport

↑ **Parent:** [Sediment transport](#sediment-transport)

[Bedload transport](#bedload-transport) is motion of sediment grains along or close to the bed, represented in a depth-averaged model by a solid-volume [flux](mathematical-physics.md#flux) per unit width. The [Exner equation](#exner-equation) balances this [flux](mathematical-physics.md#flux) divergence and changes in porous-bed solid storage against exchange with [suspended sediment](#suspended-sediment). Consistent [mass](classical-mechanics.md#mass) units are necessary when adding this [equation](algebra.md#equation) to a suspended mass-concentration balance.

#### Bedload transport model with sediment inertia

↑ **Parent:** [Bedload transport](#bedload-transport)

Keeping sediment acceleration while neglecting water storage and a small gravity-friction residual gives a reduced model for the bed elevation $s$, water speed $u$ and sediment speed $v$. A prescribed water flux $q$ gives $h=q/u$; integrated water momentum gives $s=C-F^2u^2/2-q/u$. Around the normalized uniform state $h=u=q=1$, let $(1-v_0)^2=\kappa v_0$, $0<v_0<1$. A [Fourier mode](fourier-analysis.md#fourier-mode) of wavenumber $k$ has growth-rate real part

$$
-\frac{2(1-v_0)v_0k^2}{(1-F^2)([2(1-v_0)+\kappa]^2+k^2v_0^2)}.
$$

Thus nonuniform modes decay for subcritical [Froude number](reduced-gravity.md#froude-number) and grow for supercritical [Froude number](reduced-gravity.md#froude-number). The spatially constant mode is neutral, and the critical value needs terms neglected in this reduction. In a general uniform state the sign change is at the actual mean-flow [Froude number](reduced-gravity.md#froude-number) equal to one, rather than at a velocity-scale parameter unrelated to that state.

### Suspended sediment

↑ **Parent:** [Sediment transport](#sediment-transport)

[Suspended sediment](#suspended-sediment) is particulate material carried within a fluid rather than solely along the bed. Its [concentration](mathematical-physics.md#concentration) balance includes [advection](#advection), erosion into suspension and deposition from suspension. For [water](chemical-substance.md#water) depth $h$ and suspended [mass](classical-mechanics.md#mass) [concentration](mathematical-physics.md#concentration) $c$, the conservative balance $(hc)_t+(huc)_x=\rho_s(v_E-v_D)$ reduces using [water](chemical-substance.md#water) continuity to $h(c_t+uc_x)=\rho_s(v_E-v_D)$.

### Dune

↑ **Parent:** [Sediment transport](#sediment-transport)

A [dune](#dune) is a sediment bedform. In the elementary [subcritical flow](reduced-gravity.md#subcritical-flow) description of river dunes, bed undulations and free-surface undulations are out of phase. This phase relation identifies a hydraulic response; instability additionally requires a positive real part of the relevant [dispersion relation](dispersion-relation.md). Contrast the in-phase surface of an [antidune](#antidune).

### Antidune

↑ **Parent:** [Sediment transport](#sediment-transport)

An antidune is a bedform associated with supercritical free-surface flow, in which bed and surface undulations are approximately in phase. In the elementary erodible-bed model with suspended sediment, an unstable branch can migrate upstream. Its growth and migration depend on the hydraulic and sediment-response parameters; the [high-wavenumber antidune dispersion](#high-wavenumber-antidune-dispersion) calculation makes the required supercritical regime explicit.

#### High-wavenumber antidune dispersion

↑ **Parent:** [Antidune](#antidune)

In the fast-[water](chemical-substance.md#water) limit of an erodible-bed [shallow water equations](mathematical-physics.md#shallow-water-equations) model, let $e=E'(1)>0$, $q_1=q'(1)>0$ and $\gamma>0$ be the suspended-load relaxation coefficient. [Linearization](algebra.md#linearization) and elimination give the [dispersion relation](dispersion-relation.md) $\lambda=-k^2[q_1+\beta e/(\gamma+ik)]/[3\delta+ik(F^2-1)]$. Its real part tends to the finite constant in the title, and phase [velocity](classical-mechanics.md#velocity) tends to $-q_1/(F^2-1)$. Thus the unstable upstream branch requires [supercritical flow](reduced-gravity.md#supercritical-flow) and enough sediment feedback to overcome [friction](newtonian-mechanics.md#friction); subcritical flow has the opposite propagation sign and decay at leading order. The near-critical limit needs a separate balance.

### Sediment resuspension

↑ **Parent:** [Sediment transport](#sediment-transport)

Sediment resuspension transfers deposited bed particles into a [particle suspension](suspension-chemistry.md). It can supply particle [buoyancy flux](turbulent-plume.md#buoyancy-flux) to a [particle-laden gravity current](reduced-gravity.md#particle-laden-gravity-current) if erosion or upward mixing exceeds settling losses. Ambient fluid without particles dilutes concentration without supplying particle mass.

#### Equilibrium settling-diffusion profile

↑ **Parent:** [Sediment resuspension](#sediment-resuspension)

For downward [settling velocity](suspension-chemistry.md#settling-velocity) magnitude $W_s>0$ and [eddy diffusivity](turbulence.md#eddy-diffusivity) $\kappa_T=Kz$, the total upward particle flux is $J=-W_s\phi-Kz\phi_z$. A stationary profile tending to zero at infinity has $J=0$, giving the displayed power law. The exponent compares settling with turbulent mixing. It describes a region above the bed; entrainment from the bed and viscous near-wall effects determine the reference concentration separately.

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

#### Quasistatic bed stability with suspended sediment

↑ **Parent:** [Exner equation](#exner-equation)

A leading fixed-discharge, level-surface approximation to a shallow erodible-bed flow gives perturbation [equations](algebra.md#equation) $C_x=4U-C$ and $U_t+3\beta U_x=-4U+C$. The displayed Fourier growth rate has negative [real part](complex-analysis.md#real-part) for every nonzero [wave number](wave-equation.md#wavenumber), independently of bedload parameter $\beta$. Bedload changes the propagation [speed](classical-mechanics.md#speed) but not this damping. The zero-wave-number mode is neutral, so absence of growing modes should not be confused with strict asymptotic decay of every spatially uniform perturbation.

### Shields parameter

↑ **Parent:** [Sediment transport](#sediment-transport)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Shields_parameter)

The [Shields parameter](#shields-parameter) is $\Theta=\tau/[(\rho_p-\rho_f)gd]$, comparing bed [shear stress](viscous-fluid-flow.md#shear-stress) with a grain-scale [submerged weight](#submerged-weight) per area. Its critical value depends on the assumed [drag coefficient](#drag-coefficient), [static friction](force.md#static-friction), lift, and contact geometry.

#### Sediment entrainment threshold

↑ **Parent:** [Shields parameter](#shields-parameter)

The [sediment entrainment threshold](#sediment-entrainment-threshold) is the bed [shear stress](viscous-fluid-flow.md#shear-stress) at which resting grains begin moving. An elementary [force balance](force.md#force-balance) using spherical grains, tangential [quadratic drag](#quadratic-drag), and [static friction](force.md#static-friction) gives $\Theta_{\mathrm{th},0}=4\mu_s/(3C_D)$ when the [drag coefficient](#drag-coefficient) is defined relative to the bed [shear velocity](viscous-fluid-flow.md#shear-velocity).

##### Inclined-bed sediment threshold

↑ **Parent:** [Sediment entrainment threshold](#sediment-entrainment-threshold)

For locally bed-tangent [drag force](#drag-physics) and an upslope angle $a$, a spherical-grain [force balance](force.md#force-balance) gives $\tau_{\mathrm{th}}(a)=\tau_{\mathrm{th},0}(\cos a+\sin a/\mu_s)$. The small-slope term is $\delta\tau_{\mathrm{th}}=(\tau_{\mathrm{th},0}/\mu_s)\eta_x$. A horizontal [drag force](#drag-physics) instead changes the normal contact [force](force.md) and gives a different slope correction.

### Bedform

↑ **Parent:** [Sediment transport](#sediment-transport)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bedform)

#### Sediment-bed linear instability

↑ **Parent:** [Bedform](#bedform)

Combining the [Exner equation](#exner-equation), [sediment transport saturation](#sediment-transport-saturation), [bed shear response](#bed-shear-response), and [inclined-bed sediment threshold](#inclined-bed-sediment-threshold) gives a competition between upstream forcing and downstream relaxation. With $a=\tau_0A$, $b=\tau_0B-\tau_{\mathrm{th},0}/\mu_s$, $C=\chi\gamma(\tau_0-\tau_{\mathrm{th},0})^{\gamma-1}$, and positive [wavenumber](wave-equation.md#wavenumber) $k$, the [growth rate](dispersion-relation.md#growth-rate) is $\sigma=Ck^2(b-akL_{\mathrm{sat}})/(1+k^2L_{\mathrm{sat}}^2)$. Thus $b>0$ permits long-wave growth when $a>0$, while a finite [saturation length](#saturation-length) stabilizes shorter waves.

#### Bed shear response

↑ **Parent:** [Bedform](#bedform)

For a small sinusoidal [bedform](#bedform), a fluid-dynamical closure can be written $\hat\tau=\tau_0k(A+iB)\hat\eta$ for $k>0$. The real coefficient $A$ is in phase with the bed height and $B$ describes an upstream phase lead. Neither coefficient follows from the [Exner equation](#exner-equation) or sediment relaxation alone; they require a flow calculation or measurement.

## Ram pressure

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ram_pressure)

The momentum-flux [pressure](pressure.md) associated with a moving fluid. Some energy-density balances use $\rho v^2/2$ instead; the numerical convention must be stated when balancing [magnetic pressure](magnetohydrodynamics.md#magnetic-pressure).

## Turbulence

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](turbulence.md)

## Acoustic wave

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Acoustic_wave)

An acoustic wave is a propagating pressure and density disturbance in a material medium. Linear sound waves oscillate when pressure restores a displaced fluid element.

### Acoustic modes of a rigid cylindrical cavity

↑ **Parent:** [Acoustic wave](#acoustic-wave)

For a rigid cylinder of radius $a$ and height $h$, the velocity potential obeys the [wave equation](wave-equation.md) with [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition). Separation in cylindrical coordinates gives radial factors $J_m(k_{m,n}r/a)$, angular sine and cosine factors of integer order $m$, and axial factors $\cos(\ell\pi z/h)$. The nonzero radial numbers satisfy $J'_m(k_{m,n})=0$, yielding the displayed frequencies.

There is also a constant radial mode, with $m=0$ and radial number zero. A formal zero of $J'_m$ at the origin for higher $m$ must not be counted by substituting $k=0$ into $J_m(kr)$, which would give the zero function. Solving the zero-radial-eigenvalue equation directly leaves only the constant mode under the side-wall condition. The fully constant potential has zero velocity and is a gauge mode; constant radial modes with nonzero axial index are physical longitudinal oscillations.

### Nonlinear acoustics

↑ **Parent:** [Acoustic wave](#acoustic-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nonlinear_acoustics)

[Nonlinear acoustics](#nonlinear-acoustics) retains finite-amplitude effects in [sound waves](#acoustic-wave), including amplitude-dependent propagation [speed](classical-mechanics.md#speed), distortion and possible [shock waves](transport-equation.md#shock-wave). For a one-dimensional [polytropic flow](compressible-flow.md#polytropic-flow) with $p\propto\rho^\gamma$, a rightgoing simple wave has characteristic [speed](classical-mechanics.md#speed) $u+c=c_0+(\gamma+1)u/2$ relative to a quiescent reference. Thus small-amplitude [linear acoustics](linear-acoustics.md) need not be uniform when a background [velocity](classical-mechanics.md#velocity) nearly cancels the [speed of sound](compressible-flow.md#speed-of-sound).

### Ultrasound

↑ **Parent:** [Acoustic wave](#acoustic-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ultrasound)

[Ultrasound](#ultrasound) is sound above the conventional upper limit of human hearing, approximately $20\,\mathrm{kHz}$. In a [crystal](thermodynamics.md#crystal), ultrasonic travel-time measurements determine long-wavelength elastic [wave speeds](wave-equation.md#wave-speed), which are the small-[wavevector](elasticity-physics.md#wavevector) slopes of the corresponding [acoustic phonon branches](quantum-ideal-gas-statistics.md#acoustic-phonon-branch).

#### Doppler ultrasound

↑ **Parent:** [Ultrasound](#ultrasound)

Acoustic measurement of a moving-scatterer [velocity](classical-mechanics.md#velocity) projection using [frequency](wave.md#frequency) or [phase](wave.md#phase-waves) changes. A [speed](classical-mechanics.md#speed) estimate needs the scattering geometry; finite pulsed sampling can alias the measured shift.

#### Pulse-echo ultrasound

↑ **Parent:** [Ultrasound](#ultrasound)

An emitted acoustic pulse is followed by detection of returning echoes. Travel time estimates depth under a declared sound-speed and path model, while echo amplitudes depend on interfaces and propagation losses.

##### M-mode ultrasound scan

↑ **Parent:** [Pulse-echo ultrasound](#pulse-echo-ultrasound)

A depth-versus-time display from repeated acquisition along one pulse-echo beam line.

##### B-mode ultrasound scan

↑ **Parent:** [Pulse-echo ultrasound](#pulse-echo-ultrasound)

A brightness-coded spatial image assembled from pulse-echo beam lines.

##### A-mode ultrasound scan

↑ **Parent:** [Pulse-echo ultrasound](#pulse-echo-ultrasound)

An amplitude-versus-depth representation of a single pulse-echo beam line.

### Burgers reduction of weakly nonlinear rightgoing acoustics

↑ **Parent:** [Acoustic wave](#acoustic-wave)

For a pure rightgoing [acoustic wave](#acoustic-wave), retarded time $\theta=t-x$ and slow distance $X=Mx$ separate fast oscillations from nonlinear steepening. Expanding the [equation of state](pressure.md#equation-of-state) gives $p=\rho+M(\gamma-1)\rho^2/2+O(M^2)$. The leading perturbations satisfy $u_0=\rho_0=p_0$. Adding the first-order [mass conservation](continuum-mechanics.md#mass-conservation) and [momentum conservation](momentum.md#momentum-conservation) equations cancels the unknown first corrections and yields the displayed [viscous Burgers equation](partial-differential-equation.md#viscous-burgers-equation). Inviscid characteristics satisfy $\theta=s-(\gamma+1)F(s)X/2$, $p=F(s)$; loss of invertibility marks [shock](transport-equation.md#shock-wave) formation and the end of the smooth inviscid approximation.

### Adiabatic vertical modes of a Gaussian atmosphere

↑ **Parent:** [Acoustic wave](#acoustic-wave)

A [plane-parallel atmosphere](astrophysics.md#plane-parallel-atmosphere) with [isothermal sound speed](compressible-flow.md#isothermal-sound-speed) $c_s$ in gravity $-\Omega^2z$ has [mass density](#density) $\rho_0e^{-z^2/(2H^2)}$, $H=c_s/\Omega$. Above a rigid base, vertically directed [adiabatic fluid perturbations](#adiabatic-fluid-perturbation) satisfy $w''-zw'/H^2+(\sigma^2/\Omega^2-1)w/(\gamma H^2)=0$ and $w(0)=0$. Set $x=z/H$ and $\lambda=(\sigma^2/\Omega^2-1)/\gamma$. The substitution $y=e^{-x^2/4}w$ converts finite Gaussian-weighted [kinetic energy](energy.md#kinetic-energy) into square integrability for $-y''+x^2y/4=(\lambda+1/2)y$. Odd extension across the base and the oscillator lowering operator force $\lambda$ to be an odd positive integer. Thus $w_n$ is proportional to the [Probabilists' Hermite polynomial](orthogonal-polynomial.md#probabilists-hermite-polynomial) $\mathrm{He}_{2n+1}(z/H)$. These are vertical [acoustic waves](#acoustic-wave); a general stably stratified atmosphere also admits [internal gravity waves](gravity-wave.md#internal-wave) with horizontal structure.

### Acoustically rigid boundary

↑ **Parent:** [Acoustic wave](#acoustic-wave)

An acoustically rigid boundary has zero perturbation [normal velocity](classical-mechanics.md#normal-velocity). For a reflected [acoustic plane wave](physics.md#acoustic-plane-wave), [pressure](pressure.md) amplitudes add in phase and the [reflection coefficient](partial-differential-equation.md#reflection-coefficient) is $+1$. It is the infinite-[surface acoustic impedance](elasticity-physics.md#surface-acoustic-impedance) limit. A [pressure-release boundary](#pressure-release-boundary) instead fixes the [pressure](pressure.md) perturbation to zero and reflects with coefficient $-1$.

### Acoustic cutoff frequency

↑ **Parent:** [Acoustic wave](#acoustic-wave)

A stratified atmosphere can reflect low-frequency [acoustic waves](#acoustic-wave) while permitting sufficiently high-frequency waves to escape. In a plane-parallel isothermal atmosphere, the angular acoustic cutoff is approximately $c_s/(2H_\rho)$, where $H_\rho$ is the density scale height. Its detailed form depends on the atmospheric profile and on the wave-variable approximation.

#### Atmospheric acoustic cutoff transformation

↑ **Parent:** [Acoustic cutoff frequency](#acoustic-cutoff-frequency)

In an [isothermal atmosphere](statistical-physics.md#isothermal-atmosphere) with constant density [scale height](statistical-physics.md#scale-height) $H$, the equation $\delta\rho_{tt}-c^2\delta\rho_{zz}-(c^2/H)\delta\rho_z=0$ loses its first spatial derivative under $\delta\rho=e^{-z/(2H)}\Psi$. Direct differentiation gives $\Psi_{tt}-c^2\Psi_{zz}+c^2\Psi/(4H^2)=0$. Thus a [plane wave](wave-function.md#plane-wave) has [dispersion relation](dispersion-relation.md) $\omega^2=c^2k^2+\omega_c^2$, with real [acoustic cutoff frequency](#acoustic-cutoff-frequency) $\omega_c=c/(2H)$. The cutoff term is positive; a minus sign would instead predict growing sufficiently long spatial modes. Vertical propagation requires $|\omega|\ge\omega_c$ within this ideal constant-coefficient model.

### Pressure-release boundary

↑ **Parent:** [Acoustic wave](#acoustic-wave)

A pressure-release boundary imposes zero acoustic pressure disturbance, $\widetilde p=0$. The incident and reflected pressure amplitudes therefore obey $1+R=0$, so the pressure [reflection coefficient](partial-differential-equation.md#reflection-coefficient) is $R=-1$. It contrasts with a rigid inviscid boundary, where zero normal velocity gives $R=+1$. A much lower normal impedance on the far side approximates the pressure-release condition.

### Sonic boom

↑ **Parent:** [Acoustic wave](#acoustic-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sonic_boom)

A [sonic boom](#sonic-boom) is the sound associated with [shock waves](transport-equation.md#shock-wave) from a body moving at a [supersonic](compressible-flow.md#supersonic-flow) [Mach number](compressible-flow.md#mach-number). The weak-wave [Mach cone](compressible-flow.md#mach-cone) describes a propagation geometry rather than the finite [pressure](pressure.md) signature determining the sound strength.

## Velocity field

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A velocity field assigns a velocity vector to every position and time in a moving continuum. Its spatial derivatives describe local deformation, rotation, and volume change.

### Affine velocity field

↑ **Parent:** [Velocity field](#velocity-field)

A [velocity field](#velocity-field) with spatially constant [velocity gradient](continuum-mechanics.md#velocity-gradient) $K$. Differences of fluid [velocities](classical-mechanics.md#velocity) satisfy $\mathbf u(\mathbf x+\mathbf R)-\mathbf u(\mathbf x)=K\mathbf R$, even when the uniform translation $\mathbf b$ is nonzero. [Incompressibility](#incompressible-flow) requires $\operatorname{tr}K=0$.

#### Linear velocity field

↑ **Parent:** [Affine velocity field](#affine-velocity-field)

An [affine velocity field](#affine-velocity-field) with zero uniform translation. It describes the relative motion about a comoving reference point even when the original [velocity field](#velocity-field) has a nonzero spatially uniform component.

### Secondary flow

↑ **Parent:** [Velocity field](#velocity-field)

A secondary flow is a usually smaller velocity component superposed on a primary flow selected by symmetry or a simplified force balance. Examples include meridional circulation around a rotating sphere, or transverse circulation in a curved channel. Its direction depends on the forcing mechanism: elastic [normal stresses](continuum-mechanics.md#normal-stress) and inertial effects can produce opposite circulations.

### Velocity gradient tensor

↑ **Parent:** [Velocity field](#velocity-field)

The [velocity gradient tensor](#velocity-gradient-tensor) is $A_{ij}=\partial_j u_i$. Its symmetric part is the [rate-of-strain tensor](viscous-fluid-flow.md#strain-rate-tensor) $S$ and its antisymmetric part describes local rotation. For [incompressible flow](#incompressible-flow), $\operatorname{tr}A=\operatorname{tr}S=0$. The sign convention for a cubic invariant must be specified explicitly.

### Vertical velocity

↑ **Parent:** [Velocity field](#velocity-field)

The vertical velocity is the component of a fluid [velocity field](#velocity-field) along the selected upward vertical direction. In [incompressible flow](#incompressible-flow), impermeable horizontal boundaries impose $w=0$. Eliminating [pressure](pressure.md) often yields a closed [hydrodynamic stability](hydrodynamic-stability.md) equation for this component.

### Axisymmetric flow

↑ **Parent:** [Velocity field](#velocity-field)

An axisymmetric flow is invariant under rotations about one fixed axis, so scalar fields and cylindrical-coordinate velocity components do not depend on the azimuthal angle.

#### Near-axis radial velocity in incompressible axisymmetric flow

↑ **Parent:** [Axisymmetric flow](#axisymmetric-flow)

For a smooth [axisymmetric flow](#axisymmetric-flow), write $u_z(r,z)=w(z)+O(r^2)$ near the axis. The [incompressible flow](#incompressible-flow) condition is $r^{-1}\partial_r(ru_r)+\partial_zu_z=0$. Integrating radially and excluding a singular line source at the axis gives $u_r=-rw'(z)/2+O(r^3)$. The signed axial velocity is essential: specifying only its magnitude does not fix the sign of the radial velocity.

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

[This section is present in another page, follow this link to view it.](convection.md)

## Buoyancy

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Buoyancy)

[Buoyancy](#buoyancy) is the resultant upward [force](force.md) exerted by a resting [fluid](#fluid) on an immersed body in a downward [gravitational field](physics.md#gravitational-field). The [fluid](#fluid) pushes inward, perpendicular to each part of the body's surface. Because [hydrostatic pressure](#hydrostatic-pressure) increases with depth, the upward push from below exceeds the downward push from above. Opposite horizontal [forces](force.md) cancel; [buoyancy](#buoyancy) is the remaining vertical [force](force.md). A sinking body still receives this upward support. [OpenStax, University Physics, §14.4: origin of buoyancy](https://openstax.org/books/university-physics-volume-1/pages/14-4-archimedes-principle-and-buoyancy)

More precisely, [pressure](pressure.md) $p$ on a small surface of [area](differential-geometry.md#surface-area) $dA$ with outward unit [normal vector](differential-geometry.md#normal-vector) $\mathbf n$ exerts

$$
d\mathbf F=-p\mathbf n\,dA.
$$

The minus sign says the [force](force.md) points into the body. On a [cube](euclidean-geometry.md#cube), the top [force](force.md) points down, the bottom [force](force.md) points up, and the side [forces](force.md) cancel in pairs because opposite sides have the same [pressure](pressure.md) at each depth. This is a surface [traction](continuum-mechanics.md#traction); [gravity](physics.md#gravity) on the body itself is a separate [body force](#body-force). [MIT, A. Techet, Hydrodynamics reading 1, p. 5: pressure traction](https://ocw.mit.edu/courses/2-016-hydrodynamics-13-012-fall-2005/dc299d2ff05553b3515dccc23fc0f7d2_2005reading1.pdf)

For a computed example, stipulate resting [water](chemical-substance.md#water) with constant [mass density](#density) $\rho_f=1000\ \mathrm{kg\,m^{-3}}$ and uniform [gravitational acceleration](newton-s-law-of-universal-gravitation.md#gravitational-acceleration) $g=9.81\ \mathrm{m\,s^{-2}}$. A fully immersed [cube](euclidean-geometry.md#cube) has side $L=0.10\ \mathrm m$, top depth $h_t=0.20\ \mathrm m$ and bottom depth $h_b=0.30\ \mathrm m$. Each horizontal face has [area](differential-geometry.md#surface-area) $A=L^2=0.010\ \mathrm{m^2}$, and its [volume](geometry-and-topology.md#volume) is $V=L^3=0.001\ \mathrm{m^3}$. Its top and bottom [gauge pressures](#gauge-pressure) are

$$
p_{g,t}=\rho_fgh_t=1962\ \mathrm{Pa},\qquad
p_{g,b}=\rho_fgh_b=2943\ \mathrm{Pa}.
$$

The corresponding [forces](force.md) relative to the common surface [pressure](pressure.md) are $p_{g,t}A=19.62\ \mathrm N$ downward and $p_{g,b}A=29.43\ \mathrm N$ upward. Therefore the net [buoyancy](#buoyancy) is

$$
F_b=(p_{g,b}-p_{g,t})A=9.81\ \mathrm N.
$$

Using absolute [pressures](pressure.md) adds the same $p_{\mathrm{surface}}A$ to both face [forces](force.md), leaving their difference unchanged. Zero [gauge pressure](#gauge-pressure) at the surface does not mean zero absolute [pressure](pressure.md). Increasing both depths by the same amount also leaves [buoyancy](#buoyancy) unchanged in this constant-[mass density](#density) model.

<a id="image-how-a-hydrostatic-pressure-difference-supports-an-immersed-cube"></a>
![](hydrostatic-pressure-and-buoyancy.png)

**[Figure 7](#image-how-a-hydrostatic-pressure-difference-supports-an-immersed-cube). How a hydrostatic pressure difference supports an immersed cube**. Left: a fully immersed [cube](euclidean-geometry.md#cube) of side $0.10\ \mathrm m$ has its top at depth $0.20\ \mathrm m$ and bottom at $0.30\ \mathrm m$. The inward [pressure](pressure.md) [forces](force.md) on its sides cancel; its horizontal faces have [area](differential-geometry.md#surface-area) $0.010\ \mathrm{m^2}$. The displayed face [forces](force.md) use [gauge pressure](#gauge-pressure), whose common surface offset cancels in the net $9.81\ \mathrm N$ upward [buoyancy](#buoyancy). Right: [gauge pressure](#gauge-pressure) increases linearly with depth, marking $1962\ \mathrm{Pa}$ at the top and $2943\ \mathrm{Pa}$ at the bottom.

[Archimedes' principle](#archimedes-principle) turns this calculation into a rule for bodies of any shape. It explains [floating equilibrium](#floating-equilibrium) and lets us infer an immersed body's [volume](geometry-and-topology.md#volume) from the difference between its [force](force.md) from [gravity](physics.md#gravity) and the [force](force.md) needed to support it. In particular, [buoyancy](#buoyancy) depends on the displaced [volume](geometry-and-topology.md#volume) and the surrounding [mass density](#density), whereas the body's own [mass density](#density) decides how its [force](force.md) from [gravity](physics.md#gravity) compares with that support.

### Convective available potential energy

↑ **Parent:** [Buoyancy](#buoyancy)

[Convective available potential energy](#convective-available-potential-energy) is the positive [buoyancy](#buoyancy) work per unit mass available to a rising [air parcel](geophysics.md#air-parcel), $\mathrm{CAPE}=\int B\,dz$ over positive-buoyancy layers above free convection. In the ideal lossless parcel model $w_{\max}=\sqrt{2\,\mathrm{CAPE}}$. Negative-buoyancy work is treated separately as convective inhibition.

### Centre of buoyancy

↑ **Parent:** [Buoyancy](#buoyancy)

The [centre of buoyancy](#centre-of-buoyancy) is the point through which the resultant hydrostatic [buoyant force](#buoyancy) acts. In a uniform [fluid](#fluid) under uniform [gravitational acceleration](newton-s-law-of-universal-gravitation.md#gravitational-acceleration), it is the [volume](thermodynamics.md#volume-thermodynamics) [centroid](euclidean-geometry.md#centroid) of the displaced [fluid](#fluid). For a floating body its position generally changes when the body tilts, because the displaced [volume](thermodynamics.md#volume-thermodynamics) changes shape.

### Buoyancy of an aerated liquid

↑ **Parent:** [Buoyancy](#buoyancy)

For a quasihydrostatic bubbly mixture with gas [void fraction](#void-fraction) $\alpha$, volume averaging gives the displayed [mass density](#density). A body displacing mixture volume $V$ has approximate [buoyant force](#buoyancy) $\rho_{\rm mix}gV$. A floating body of mass $m$ therefore needs $V=m/\rho_{\rm mix}$; gas release can increase its draft until the required displacement exceeds its available watertight volume. This mechanism explains a possible loss of flotation without making sinking inevitable in every gas plume. Upward liquid flow, turbulence and nonuniform bubble distributions require additional hydrodynamic forces beyond this simple mixture model.

### Buoyancy gradient

↑ **Parent:** [Buoyancy](#buoyancy)

The spatial [gradient](multivariable-calculus.md#gradient) of [buoyancy](#buoyancy) determines the buoyancy anomaly produced by a small parcel [displacement](classical-mechanics.md#displacement): $b'=-\boldsymbol\xi\cdot\nabla\bar b$. Its vertical component is the squared [buoyancy frequency](gravity-wave.md#buoyancy-frequency) in a stably stratified [Boussinesq approximation](geophysical-fluid-dynamics.md#boussinesq-approximation). A horizontal component enters [thermal wind](geophysical-fluid-dynamics.md#thermal-wind) and the propagation of a [Boundary Rossby wave](hydrodynamic-stability.md#boundary-rossby-wave).

### Magnetic buoyancy

↑ **Parent:** [Buoyancy](#buoyancy)

[Magnetic buoyancy](#magnetic-buoyancy) is the tendency of magnetized fluid to rise when [magnetic pressure](magnetohydrodynamics.md#magnetic-pressure) support reduces its density relative to its surroundings. For a thin flux concentration in lateral balance, $p_{\rm in}+B^2/(2\mu_0)=p_{\rm out}$. At equal [temperature](temperature.md) and composition an ideal-gas equation of state then gives $\rho_{\rm in}<\rho_{\rm out}$, producing an upward buoyant force. Thermal exchange, [magnetic tension](magnetohydrodynamics.md#magnetic-tension) and stable stratification modify this simple argument. In a [solar dynamo](stellar-astrophysics.md#solar-dynamo), buoyant toroidal flux can emerge as tilted bipolar active regions.

### Archimedes' principle

↑ **Parent:** [Buoyancy](#buoyancy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Archimedes'_principle)

[Archimedes' principle](#archimedes-principle) states that [buoyancy](#buoyancy) equals the downward [gravitational weight](force.md#weight-physics), or weight, of the displaced [fluid](#fluid). In a resting [fluid](#fluid) of constant [mass density](#density) $\rho_f$ under uniform [gravitational acceleration](newton-s-law-of-universal-gravitation.md#gravitational-acceleration) $g$, its magnitude is

$$
F_b=\rho_fgV_{\mathrm{displaced}}.
$$

Here $V_{\mathrm{displaced}}$ is the [volume](geometry-and-topology.md#volume) from which the body excludes the [fluid](#fluid): the whole external [volume](geometry-and-topology.md#volume) for a fully immersed solid body, and just the immersed [volume](geometry-and-topology.md#volume) for a partly immersed one. The body's own [mass](classical-mechanics.md#mass) does not enter this [buoyancy](#buoyancy) formula. [OpenStax, University Physics, §14.4: Archimedes' principle](https://openstax.org/books/university-physics-volume-1/pages/14-4-archimedes-principle-and-buoyancy)

A short proof outline for a fully immersed body is to imagine replacing it by exactly the [fluid](#fluid) it displaces. The surrounding [hydrostatic pressure](#hydrostatic-pressure) is unchanged. That replacement [fluid](#fluid) is at rest, so its upward [pressure](pressure.md) [force](force.md) must balance its downward [force](force.md) from [gravity](physics.md#gravity). The original body receives the same inward [pressure](pressure.md) [forces](force.md) on the same closed surface, hence the same upward [buoyancy](#buoyancy).

Equivalently, let $\Omega$ be the displaced region, $\partial\Omega$ its closed surface and $\mathbf e_z$ the upward unit direction. The [divergence theorem](multivariable-calculus.md#divergence-theorem), applied component by component to the [surface integral](multivariable-calculus.md#surface-integral), and [hydrostatic pressure](#hydrostatic-pressure) give

$$
\mathbf F_b=-\int_{\partial\Omega}p\mathbf n\,dA
=-\int_\Omega\nabla p\,dV
=\rho_fgV_{\mathrm{displaced}}\mathbf e_z.
$$

This also explains why horizontal [forces](force.md) cancel even for an irregular shape. A spatially constant surface [pressure](pressure.md) contributes zero to the closed-surface [integral](integral.md). If the [mass density](#density) varies with depth, replace $\rho_fV_{\mathrm{displaced}}$ by the [mass](classical-mechanics.md#mass) $\int_\Omega\rho_f\,dV$ of the displaced [fluid](#fluid).

The closed-surface argument assumes that the [fluid](#fluid) applies [pressure](pressure.md) over the entire boundary of a fully immersed body. A body sealing against a tank bottom may have no [fluid](#fluid) beneath it; then the lower-face [pressure](pressure.md) [force](force.md) used in the proof is absent, and a supporting contact [force](force.md) must be treated separately. For partial immersion, the usual [buoyancy](#buoyancy) formula assumes the exposed surface receives the common atmospheric [pressure](pressure.md), neglects the much smaller [buoyancy](#buoyancy) from the air, and neglects [surface tension](surface-tension.md).

For the $0.10\ \mathrm m$ [cube](euclidean-geometry.md#cube) in the stipulated [water](chemical-substance.md#water), full immersion displaces $0.001\ \mathrm{m^3}$, so $F_b=1000\times9.81\times0.001=9.81\ \mathrm N$. If its uniform [mass density](#density) is $600\ \mathrm{kg\,m^{-3}}$, its [mass](classical-mechanics.md#mass) is $m=600\times0.001=0.600\ \mathrm{kg}$ and its downward [force](force.md) from [gravity](physics.md#gravity) is $mg=5.886\ \mathrm N$. To hold it fully immersed at rest requires an additional downward [force](force.md)

$$
F_{\mathrm{hold}}=F_b-mg=9.81-5.886=3.924\ \mathrm N.
$$

On release from rest it initially moves upward; its eventual [floating equilibrium](#floating-equilibrium) has a smaller displaced [volume](geometry-and-topology.md#volume). A same-size [cube](euclidean-geometry.md#cube) of uniform [mass density](#density) $1200\ \mathrm{kg\,m^{-3}}$ has [mass](classical-mechanics.md#mass) $1.200\ \mathrm{kg}$ and downward [force](force.md) from [gravity](physics.md#gravity) $11.772\ \mathrm N$. Full immersion still gives $9.81\ \mathrm N$ of [buoyancy](#buoyancy), leaving an initial net downward [force](force.md) of $11.772-9.81=1.962\ \mathrm N$. Subsequent motion also involves [drag](#drag-physics).

#### Floating equilibrium

↑ **Parent:** [Archimedes' principle](#archimedes-principle)

A freely floating body at rest has no supporting contact or applied holding [force](force.md). Neglecting [surface tension](surface-tension.md) and the [buoyancy](#buoyancy) of air, its upward [buoyancy](#buoyancy) balances its downward [force](force.md) from [gravity](physics.md#gravity):

$$
F_b=mg.
$$

For a body of uniform [mass density](#density) $\rho_{\mathrm{body}}$ and total [volume](geometry-and-topology.md#volume) $V_{\mathrm{body}}$, its [mass](classical-mechanics.md#mass) is $m=\rho_{\mathrm{body}}V_{\mathrm{body}}$. Substitution into [Archimedes' principle](#archimedes-principle) gives

$$
\frac{V_{\mathrm{displaced}}}{V_{\mathrm{body}}}
=\frac{\rho_{\mathrm{body}}}{\rho_f}.
$$

Partial immersion is possible when $\rho_{\mathrm{body}}<\rho_f$. A nonuniform body uses its mean [mass density](#density) $m/V_{\mathrm{body}}$ instead; for a hollow body this [volume](geometry-and-topology.md#volume) must count the enclosed space that excludes [water](chemical-substance.md#water). This explains how the amount of displaced [water](chemical-substance.md#water) can support a vessel whose walls alone are denser than [water](chemical-substance.md#water). [OpenStax, College Physics, §11.7: floating fraction and mean density](https://openstax.org/books/college-physics-2e/pages/11-7-archimedes-principle)

For the $600\ \mathrm{kg\,m^{-3}}$ [cube](euclidean-geometry.md#cube) in [water](chemical-substance.md#water) of [mass density](#density) $1000\ \mathrm{kg\,m^{-3}}$, the displaced fraction is $600/1000=0.60$: sixty percent of its [volume](geometry-and-topology.md#volume) lies below the surface. With a horizontal top and bottom, the immersed depth $d$ satisfies $V_{\mathrm{displaced}}=Ad$, so

$$
V_{\mathrm{displaced}}=0.000600\ \mathrm{m^3},\qquad
d=\frac{0.000600}{0.010}=0.060\ \mathrm m.
$$

Its remaining height is $0.040\ \mathrm m$, and the [buoyancy](#buoyancy) is $1000\times9.81\times0.000600=5.886\ \mathrm N$, exactly balancing its downward [force](force.md) from [gravity](physics.md#gravity).

<a id="image-floating-neutral-buoyancy-and-sinking-for-three-equal-size-cubes"></a>
![](buoyancy-floating-and-sinking.png)

**[Figure 8](#image-floating-neutral-buoyancy-and-sinking-for-three-equal-size-cubes). Floating, neutral buoyancy and sinking for three equal-size cubes**. All three [cubes](euclidean-geometry.md#cube) have side $0.10\ \mathrm m$ in [water](chemical-substance.md#water) with stipulated [mass density](#density) $1000\ \mathrm{kg\,m^{-3}}$ and [gravitational acceleration](newton-s-law-of-universal-gravitation.md#gravitational-acceleration) $9.81\ \mathrm{m\,s^{-2}}$. Left: the $600\ \mathrm{kg\,m^{-3}}$ body floats with $0.060\ \mathrm m$ immersed and equal upward and downward [forces](force.md) of $5.886\ \mathrm N$. Middle: a fully immersed $1000\ \mathrm{kg\,m^{-3}}$ body has [neutral buoyancy](#neutral-buoyancy), with both [forces](force.md) equal to $9.81\ \mathrm N$. Right: a fully immersed $1200\ \mathrm{kg\,m^{-3}}$ body has downward [force](force.md) from [gravity](physics.md#gravity) $11.772\ \mathrm N$ against upward [buoyancy](#buoyancy) $9.81\ \mathrm N$, so release from rest gives an initial net downward [force](force.md) $1.962\ \mathrm N$.

##### Metacentric height

↑ **Parent:** [Floating equilibrium](#floating-equilibrium)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Metacentric_height)

For a small heel of a floating body in a uniform [fluid](#fluid), the metacentre is the intersection of the new vertical [buoyancy](#buoyancy) line with the original vertical through the [centre of buoyancy](#centre-of-buoyancy). With the [centre of mass](classical-mechanics.md#center-of-mass) a signed distance $BG$ above the original [centre of buoyancy](#centre-of-buoyancy), the [metacentric height](#metacentric-height) is $GM=I_{\rm wp}/V_d-BG$. Here $I_{\rm wp}$ is the waterplane [second moment of area](elasticity-physics.md#second-moment-of-area) about the heel axis and $V_d$ the displaced [volume](thermodynamics.md#volume-thermodynamics). Positive $GM$ gives a restoring small-angle [torque](momentum.md#torque) and negative $GM$ gives instability. The formula describes local static stability, not all large-angle behaviour or effects of free [liquid](thermodynamics.md#liquid) surfaces inside the body.

##### Vertical oscillations of a floating cylinder

↑ **Parent:** [Floating equilibrium](#floating-equilibrium)

A vertical cylinder of constant cross-sectional [area](differential-geometry.md#surface-area) $A$, partly immersed to depth $h_0$ in a fluid of [mass density](#density) $\rho_f$, satisfies $mg=\rho_f gAh_0$ by [Archimedes' principle](#archimedes-principle). A small extra downward displacement $z$ increases the [buoyant force](#buoyancy) by $\rho_f gAz$, so $m\ddot z=-\rho_f gAz$. This is [simple harmonic motion](classical-mechanics.md#simple-harmonic-motion) with the displayed [angular frequency](lagrangian-mechanics.md#angular-frequency) and [oscillation period](classical-mechanics.md#period-of-an-oscillation) $2\pi\sqrt{h_0/g}$. The ideal model neglects fluid added inertia, [drag](#drag-physics) and surface effects; it requires partial immersion throughout the motion.

### Neutral buoyancy

↑ **Parent:** [Buoyancy](#buoyancy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Neutral_buoyancy)

[Neutral buoyancy](#neutral-buoyancy) means a fully immersed body's upward [buoyancy](#buoyancy) equals its downward [force](force.md) from [gravity](physics.md#gravity). For a body of fixed [volume](geometry-and-topology.md#volume) in a constant-[mass density](#density) [fluid](#fluid) under a uniform [gravitational field](physics.md#gravitational-field), this occurs when its mean [mass density](#density) equals the surrounding [mass density](#density). A $0.10\ \mathrm m$ [cube](euclidean-geometry.md#cube) of [mass density](#density) $1000\ \mathrm{kg\,m^{-3}}$ in the stipulated [water](chemical-substance.md#water) has [mass](classical-mechanics.md#mass) $1.000\ \mathrm{kg}$, so both [forces](force.md) are $9.81\ \mathrm N$.

Ideally it can remain at rest at any depth for which it stays fully immersed and clear of boundaries. Raising or lowering it changes the absolute [pressure](pressure.md), but neither its displaced [volume](geometry-and-topology.md#volume) nor the difference between the vertical [pressure](pressure.md) [forces](force.md). There is therefore no vertical [restoring force](force.md#restoring-force) toward a preferred depth in this model. [Neutral buoyancy](#neutral-buoyancy) is a vertical [force](force.md) balance, not a claim about resistance to tilting or about a compressible body whose [volume](geometry-and-topology.md#volume) changes with [pressure](pressure.md).

### Submerged weight

↑ **Parent:** [Buoyancy](#buoyancy)

For a grain of [mass density](#density) $\rho_p$ and volume $\mathcal V$ in a fluid of [mass density](#density) $\rho_f$, its effective downward [force](force.md) is $(\rho_p-\rho_f)g\mathcal V$, after subtracting [buoyancy](#buoyancy) from weight.

### Buoyancy perturbation

↑ **Parent:** [Buoyancy](#buoyancy)

A buoyancy perturbation is the departure $b'$ from a prescribed basic buoyancy field. In a fluid with constant [buoyancy frequency](gravity-wave.md#buoyancy-frequency) $N$, vertical velocity $w'$ changes it according to $(\partial_t+\mathbf U\cdot\nabla)b'=-N^2w'$.

#### Buoyancy displacement variable

↑ **Parent:** [Buoyancy perturbation](#buoyancy-perturbation)

In a radially stratified [shearing sheet](gravitational-instability-of-an-astrophysical-disk.md#shearing-sheet), one can normalize the scalar [buoyancy perturbation](#buoyancy-perturbation) by writing $b_x=-N^2\theta$ and $D_t\theta=u_x+\xi\nabla^2\theta$. With this convention $\theta$ has dimensions of length, rather than [temperature](temperature.md); $\xi$ is [thermal diffusivity](heat.md#thermal-diffusivity).

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

Steady spherical [continuity equation](mathematical-physics.md#continuity-equation) gives $r^2\rho u=\text{constant}$. Combining this with [Euler equations for an inviscid fluid](euler-equations-for-an-inviscid-fluid.md) and $c_s^2=dp/d\rho$ gives the displayed equation. Smooth transonic passage requires $u^2=c_s^2$ and $\Phi^{\prime}=2c_s^2/r$ simultaneously. The [barotropic enthalpy function](#barotropic-enthalpy-function) gives the integral $u^2/2+h+\Phi=\text{constant}$.

#### Polytropic accretion in a mixed inverse-power potential

↑ **Parent:** [Barotropic spherical accretion equation](#barotropic-spherical-accretion-equation)

For $p=K\rho^{1+1/m}$, the [barotropic enthalpy function](#barotropic-enthalpy-function) is $mc_s^2$. In $\Phi=-\lambda/R^2-\mu/R$, a regular [sonic point](compressible-flow.md#sonic-point) obeys $c_{s,s}^2=\lambda/R_s^2+\mu/(2R_s)$, and its Bernoulli integral yields the displayed quadratic. For $K,\lambda,\mu>0$ and the usual positive polytropic index, its unique positive root exists precisely when $m>1/2$. The [mass accretion rate](astrophysical-black-hole.md#mass-accretion-rate) is $4\pi R_s^2\rho_\infty c_{s,s}(c_{s,s}^2/c_\infty^2)^m$. If indices with $0<1+1/m<1$ are admitted, $m<-1$ also permits a positive sonic root; negative compressibility indices do not.

#### Critical-point slope of barotropic spherical accretion

↑ **Parent:** [Barotropic spherical accretion equation](#barotropic-spherical-accretion-equation)

At a regular [sonic point](compressible-flow.md#sonic-point), differentiating the vanishing coefficient and numerator yields $(2+C/c_s^2)(u^{\prime})^2+4Cu^{\prime}/(ru)+(4C+2c_s^2)/r^2+\Phi^{\prime\prime}=0$. A real slope compatible with the desired branch is needed in addition to the sonic equalities. For constant [sound speed](compressible-flow.md#speed-of-sound) this reduces to $(u^{\prime})^2=-c_s^2/r^2-\Phi^{\prime\prime}/2$.

### Barotropic enthalpy function

↑ **Parent:** [Barotropic fluid](#barotropic-fluid)

This [barotropic pressure potential](#barotropic-enthalpy-function) obeys $\nabla h=\nabla p/\rho$ for a [barotropic fluid](#barotropic-fluid). It gives the [pressure](pressure.md) contribution to a steady [Bernoulli equation](euler-equations-for-an-inviscid-fluid.md#bernoulli-equation). In isentropic thermodynamics it agrees with [specific enthalpy](enthalpy.md#specific-enthalpy) up to a constant; for an externally maintained isothermal ideal gas it is $c_s^2\log\rho$ and is not the constant thermodynamic enthalpy at fixed temperature.

### Centrifugal potential of cylindrical rotation

↑ **Parent:** [Barotropic fluid](#barotropic-fluid)

For [angular velocity](rigid-body-dynamics.md#angular-velocity) depending only on cylindrical radius, the centrifugal acceleration is a [gradient](multivariable-calculus.md#gradient). Steady barotropic balance is $\nabla p/\rho=-\nabla\Psi$, hence [specific enthalpy](enthalpy.md#specific-enthalpy) satisfies $h(\rho)+\Psi=\text{constant}$. On an invertible equation-of-state branch, [mass density](#density) and [pressure](pressure.md) are functions of $\Psi$. Cylindrical rotation is essential to this scalar centrifugal-potential representation.

### Barotropic energy density

↑ **Parent:** [Barotropic fluid](#barotropic-fluid)

For a [barotropic fluid](#barotropic-fluid) with [pressure](pressure.md) $P=P(\rho)$, choose an energy density $U$ satisfying $\rho U'(\rho)-U=P$. The [continuity equation](mathematical-physics.md#continuity-equation) then gives $\partial_tU+\nabla\cdot(U\mathbf u)=-P\nabla\cdot\mathbf u$. For an [isothermal equation of state](compressible-flow.md#globally-isothermal-equation-of-state) $P=c_s^2\rho$, one choice is $U=c_s^2\rho\ln(\rho/\rho_{\rm ref})$. A fixed reference density changes $U$ only by a conserved mass term. The same construction holds with [surface density](astrophysical-disk.md#surface-density-of-a-disk) and vertically integrated [pressure](pressure.md). This closure energy need not equal the microscopic internal energy of a gas maintained at fixed [temperature](temperature.md).

### Barotropic magnetic energy equation

↑ **Parent:** [Barotropic fluid](#barotropic-fluid)

For a [barotropic fluid](#barotropic-fluid), an energy per mass $e$ can be defined by $de/d\rho=p/\rho^2$. For the [isothermal equation of state](compressible-flow.md#globally-isothermal-equation-of-state), $e=c_s^2\ln(\rho/\rho_0)$. Adding kinetic, gravitational and [magnetic energy](electromagnetic-wave.md#magnetic-energy) gives the ideal magnetic energy flux $\mathbf u(E+p+B^2/(2\mu_0))-\mathbf B(\mathbf u\cdot\mathbf B)/\mu_0$. This is a mechanical barotropic energy identity; it does not say that an isothermal gas is thermally isolated.

### Barotropic vorticity transport

↑ **Parent:** [Barotropic fluid](#barotropic-fluid)

For an inviscid [barotropic fluid](#barotropic-fluid) with only potential body forces, the [vorticity](vorticity.md) $\boldsymbol\omega=\nabla\times\mathbf u$ obeys

$$
\partial_t\boldsymbol\omega=\nabla\times(\mathbf u\times\boldsymbol\omega).
$$

The pressure force is a [gradient](multivariable-calculus.md#gradient) because $\rho^{-1}\nabla p=\nabla\int^\rho p'(s)\,ds/s$. A spatially uniform [specific entropy](entropy.md#specific-entropy) makes a fixed-composition fluid barotropic. Merely having $Ds/Dt=0$ does not exclude [baroclinic vorticity generation](mathematical-physics.md#baroclinic-vorticity-generation) from spatial entropy gradients.

#### Conservation of vorticity flux through a material surface

↑ **Parent:** [Barotropic vorticity transport](#barotropic-vorticity-transport)

For smooth inviscid [barotropic fluid](#barotropic-fluid) with potential body forces, [barotropic vorticity transport](#barotropic-vorticity-transport) and $\nabla\cdot\boldsymbol\omega=0$ give $D\boldsymbol\omega/Dt=(\boldsymbol\omega\cdot\nabla)\mathbf u-\boldsymbol\omega\nabla\cdot\mathbf u$. Combine this with [material surface element evolution](#material-surface-element-evolution) to obtain $D(\boldsymbol\omega\cdot d\mathbf S)/Dt=0$. Integrating over a [material surface](#material-surface) proves the flux law. Its boundary must move with the fluid; flux through a fixed open surface is generally not conserved. By [Stokes theorem](multivariable-calculus.md#stokes-theorem) the same statement is [Kelvin's circulation theorem](vorticity.md#kelvin-s-circulation-theorem) around the material boundary.

## Shear flow

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

A shear flow has a [velocity field](#velocity-field) varying across adjacent fluid layers, giving a nonzero [shear rate](viscous-fluid-flow.md#shear-rate). A parallel example is $\mathbf u=U(z)\mathbf e_x$, with vertical shear $U'$. [Linear shear flow](#linear-shear-flow) has constant shear, while a [shear layer](#shear-layer) concentrates the velocity change in a narrow region.

### Vertical shear

↑ **Parent:** [Shear flow](#shear-flow)

Variation of horizontal [velocity](classical-mechanics.md#velocity) with height. In a rotating balanced [stratification](gravity-wave.md#density-stratification), [thermal-wind balance](geophysical-fluid-dynamics.md#thermal-wind) relates this [vertical shear](#vertical-shear) to a horizontal [buoyancy gradient](#buoyancy-gradient). The sign reverses when changing from upward height to downward-increasing [pressure coordinate](geophysical-fluid-dynamics.md#pressure-coordinate).

### Renovating shear flow

↑ **Parent:** [Shear flow](#shear-flow)

A renovating shear flow holds a planar [shear flow](#shear-flow) fixed for an interval $T$, then chooses a fresh orientation independently of preceding intervals. Each interval acts on a [material line](#material-curve) by a rotated copy of the displayed [deformation gradient](continuum-mechanics.md#deformation-gradient). The orientation law must be specified: independent uniformly distributed orientations define the isotropic model, whereas a biased orientation law generally gives another [Lyapunov exponent](dynamical-systems.md#lyapunov-exponent).

#### Mean logarithmic stretching in an isotropic renovating shear

↑ **Parent:** [Renovating shear flow](#renovating-shear-flow)

For independent uniform orientations in a [renovating shear flow](#renovating-shear-flow), the incident angle relative to each new shear is uniform even after earlier deformations. One interval stretches a unit [material line](#material-curve) by $\ell(\theta)^2=1+a\sin2\theta+a^2\sin^2\theta$. Write this as $A+B\cos(2\theta-\delta)$, where $A=1+a^2/2$ and $A^2-B^2=1$. The angular logarithmic integral gives $\langle\log\ell\rangle=\tfrac12\log[(A+1)/2]$. Add these independent logarithmic increments to get the displayed rate. At fixed shear rate, small $T$ gives $\mu\sim\Lambda^2T/8$ and large $T$ gives $\mu\sim\log(|\Lambda|T/2)/T$. The unique positive maximum is at $|\Lambda|T\approx3.9605826$, obtained from $\log z=2(1-z^{-1})$ with $z=1+a^2/4$.

##### Log-stretch fluctuations in an isotropic renovating shear

↑ **Parent:** [Mean logarithmic stretching in an isotropic renovating shear](#mean-logarithmic-stretching-in-an-isotropic-renovating-shear)

The logarithm of the stretch after $N$ independent uniform renovations is a sum of independent identically distributed bounded increments. For singular stretching $e^\gamma$, $\gamma=\operatorname{arsinh}(|a|/2)$, the increment has Fourier expansion $r+\sum_{n\geq1}(-1)^{n+1}q^n\cos(2n\theta)/n$, with $q=\tanh\gamma$ and $r=\tfrac12\log(1+a^2/4)$. Orthogonality proves the displayed variance. The [central limit theorem](convergence-of-random-variables.md#central-limit-theorem) gives an approximate central [log-normal distribution](probability-distribution.md#log-normal-distribution) of $\lambda_N$, not an exact description of extreme tails. For $|a|\ll1$, both the mean and variance of $\log\lambda_N$ are $Na^2/8$ to leading order. Direct expansion of fixed-power moments gives $\langle\lambda_N^p\rangle=\exp[Np(p+2)a^2/16+O(Na^4)]$; in particular mean stretch grows faster than typical stretch.

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

The Lagrangian perturbation compares a variable on the same moving fluid element before and after a displacement. Taylor expansion of the background value at the displaced position gives the displayed relation to an Eulerian perturbation. For an adiabatic [ideal gas](ideal-gas.md), $\Delta(p/\rho^\gamma)=0$ even when the equilibrium [entropy](entropy.md) varies spatially.

#### Adiabatic fluid perturbation

↑ **Parent:** [Lagrangian perturbation of a fluid variable](#lagrangian-perturbation-of-a-fluid-variable)

An adiabatic fluid perturbation preserves the [specific entropy](entropy.md#specific-entropy) of each displaced parcel. For a [perfect gas](ideal-gas.md), [mass conservation](continuum-mechanics.md#mass-conservation) gives $\Delta\rho=-\rho\nabla\cdot\boldsymbol\xi$ and the [adiabatic equation of state](pressure.md#adiabatic-equation-of-state) gives $\Delta p=\gamma p\Delta\rho/\rho$. The corresponding [Eulerian perturbation of a fluid variable](#eulerian-perturbation-of-a-fluid-variable) is $\delta p=-\gamma p\nabla\cdot\boldsymbol\xi-\boldsymbol\xi\cdot\nabla p$. An isothermal equilibrium may still have adiabatic perturbations, because the thermodynamic constraint on displaced parcels differs from the equilibrium temperature profile.

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

Moving a uniform-density boundary produces a delta-function sheet in the Eulerian [mass density](#density) perturbation. For a slab displaced vertically by $\eta_\pm$, $\rho^{\prime}=\rho_0\eta_+\delta(z-H)-\rho_0\eta_-\delta(z+H)$. [Poisson equation](partial-differential-equation.md#poisson-s-equation) then gives a continuous gravitational potential with derivative jumps fixed by those sheets.

### Lagrangian pressure perturbation

↑ **Parent:** [Eulerian and Lagrangian fluid perturbations](#eulerian-and-lagrangian-fluid-perturbations)

The [Lagrangian pressure perturbation](#lagrangian-pressure-perturbation) is the change in [pressure](pressure.md) experienced by a displaced [fluid element](continuum-mechanics.md#fluid-element): $\Delta p=\delta p+\boldsymbol\xi\cdot\nabla p_0$. For a free surface against fixed external [pressure](pressure.md), $\Delta p=0$, rather than $\delta p=0$ at the original surface.

<h2 id="torricelli-s-law">Torricelli's law</h2>

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Torricelli's_law)

An ideal fluid issuing from a small hole a vertical depth $h$ below a free surface has speed

$$
v=\sqrt{2gh}.
$$

Here $h$ is the vertical distance from the [free surface](#free-surface) to the centre of the [orifice](#orifice), and $g$ is the positive magnitude of [gravitational acceleration](newton-s-law-of-universal-gravitation.md#gravitational-acceleration). The ideal prediction assumes [incompressible flow](#incompressible-flow), the same ambient [pressure](pressure.md) at the [free surface](#free-surface) and emerging jet, negligible [velocity](classical-mechanics.md#velocity) of the reservoir's [free surface](#free-surface), and negligible [viscous dissipation](stokes-flow.md#viscous-dissipation) and [surface tension](surface-tension.md) effects. For a falling [free surface](#free-surface), a [quasi-steady approximation](mathematics.md#quasi-steady-approximation) additionally assumes that the local outflow adjusts much faster than $h$ changes. It applies the [Bernoulli equation](euler-equations-for-an-inviscid-fluid.md#bernoulli-equation) at each instant, rather than claiming that the whole drainage is [steady flow](#steady-flow).[Macro Scale Derivation and Common Assumptions: steady, inviscid, incompressible streamline balance and the gravity-height term](physics-bibliography.md#bernoulli’s-equation-by-nasa-glenn-research-center)

A short proof uses a [streamline](#streamline) connecting the reservoir's [free surface](#free-surface) at elevation $z_s$ to the emerging jet at elevation $z_o$. With constant [mass density](#density) $\rho$, negligible surface [speed](classical-mechanics.md#speed) and no mechanical [energy](energy.md) losses, the [Bernoulli equation](euler-equations-for-an-inviscid-fluid.md#bernoulli-equation) gives

$$
\frac{p_{\mathrm{ambient}}}{\rho}+gz_s
=\frac{p_{\mathrm{ambient}}}{\rho}+\frac{v^2}{2}+gz_o,
\qquad h=z_s-z_o.
$$

Equal [pressures](pressure.md) cancel, leaving $v^2/2=gh$: a unit [mass](classical-mechanics.md#mass) gains the same [kinetic energy](energy.md#kinetic-energy) as a body in [free fall](newton-s-law-of-universal-gravitation.md#free-fall) through height $h$. This makes [Torricelli's law](#torricelli-s-law) a useful first estimate before the detailed [velocity field](#velocity-field) is known. At one quarter of the original head, ideal jet [speed](classical-mechanics.md#speed) is one half as large; it is not proportional to head.

<a id="image-torricelli-geometry-equal-boundary-pressures-and-a-vertical-head"></a>
![](torricelli-reservoir-head-and-pressure.png)

**[Figure 9](#image-torricelli-geometry-equal-boundary-pressures-and-a-vertical-head). Torricelli geometry: equal boundary pressures and a vertical head**. Original schematic of ideal outflow, not measured apparatus or a scale drawing. The [free surface](#free-surface) and emerging jet share ambient [pressure](pressure.md). Head $h$ is measured to the [orifice](#orifice) centre. Bulk [hydrostatic pressure](#hydrostatic-pressure) at that elevation is a different quantity from jet [pressure](pressure.md).

Far from the accelerating outlet region, the reservoir has approximately [hydrostatic pressure](#hydrostatic-pressure) $p_{\mathrm{ambient}}+\rho gh$ at the outlet's elevation. The emerging jet instead has approximately ambient [pressure](pressure.md) when [surface tension](surface-tension.md) is negligible. Do not assign that bulk [hydrostatic pressure](#hydrostatic-pressure) to the emerging jet as well as adding the height difference: that would count the available mechanical [energy](energy.md) twice. A sealed reservoir, a submerged outlet or significant [surface tension](surface-tension.md) changes the [pressure](pressure.md) conditions and requires a different balance.

Actual [volumetric flow rate](#volumetric-flow-rate) is commonly represented by a [discharge coefficient](#discharge-coefficient):

$$
Q=C_d a\sqrt{2gh},\qquad C_d=\frac{Q}{a\sqrt{2gh}},
$$

where $a$ is the geometric [area](differential-geometry.md#surface-area) of the [orifice](#orifice). This definition compares [volumetric flow rates](#volumetric-flow-rate), not just [speeds](classical-mechanics.md#speed). If a nearly uniform jet at its [vena contracta](#vena-contracta) has [area](differential-geometry.md#surface-area) $a_j$ and [speed](classical-mechanics.md#speed) $v_j$, define the two separate ratios $C_c=a_j/a$ and $C_v=v_j/\sqrt{2gh}$. Then $Q=a_jv_j$ gives $C_d=C_cC_v$. A contracted jet can consequently have a [speed](classical-mechanics.md#speed) close to $\sqrt{2gh}$ while $C_d$ is appreciably below one. No particular $C_d$ is universal: calibrate it for the opening and operating range.

### Draining tank with constant cross-sectional area

↑ **Parent:** [Torricelli's law](#torricelli-s-law)

Take a reservoir with constant horizontal cross-sectional [area](differential-geometry.md#surface-area) $A$, one small [orifice](#orifice) of [area](differential-geometry.md#surface-area) $a$, no inflow, and constant stipulated [discharge coefficient](#discharge-coefficient) $C_d>0$. Let the initial head be $H>0$. For constant [mass density](#density) $\rho$, the stored [mass](classical-mechanics.md#mass) above the outlet level is $\rho Ah$ and outgoing [mass flow rate](#mass-flow-rate) is $\rho Q$. [Mass conservation](continuum-mechanics.md#mass-conservation) cancels $\rho$ and gives the [initial value problem](differential-equation.md#initial-value-problem)

$$
A\frac{dh}{dt}=-Q,
\qquad \frac{dh}{dt}=-k\sqrt h,
\qquad h(0)=H,
\qquad k=\frac{C_da}{A}\sqrt{2g}.
$$

The downward [speed](classical-mechanics.md#speed) of the [free surface](#free-surface) is $Q/A$, smaller than the ideal jet [speed](classical-mechanics.md#speed) by the factor $C_da/A$. Thus a small opening relative to the reservoir supports the negligible-surface-[velocity](classical-mechanics.md#velocity) assumption.

For $h>0$, [separation of variables](partial-differential-equation.md#separation-of-variables) or the [chain rule](calculus.md#chain-rule) gives $d\sqrt h/dt=-k/2$. Integrating yields

$$
T=\frac{2\sqrt H}{k}=\frac{A}{C_da}\sqrt{\frac{2H}{g}},
\qquad
h(t)=\begin{cases}H(1-t/T)^2,&0\le t\le T,\\0,&t\ge T,\end{cases}
$$



$$
Q(t)=\begin{cases}Q_0(1-t/T),&0\le t\le T,\\0,&t\ge T,\end{cases}
\qquad Q_0=C_da\sqrt{2gH}.
$$

The model reaches zero head in finite time even though [volumetric flow rate](#volumetric-flow-rate) tends to zero. Extending the squared expression beyond $T$ would make head grow again and violate the original [ordinary differential equation](differential-equation.md#ordinary-differential-equation). The zero-head continuation enforces no further outflow. For an elevated side opening, zero head means the surface has reached that opening, leaving [fluid](#fluid) below it; $T$ is not the time to remove every drop from such a tank.

For an original synthetic example, stipulate

$$
A=0.100\ \mathrm{m^2},\quad a=1.00\times10^{-4}\ \mathrm{m^2},\quad
C_d=0.620,\quad H=0.250\ \mathrm m,\quad g=9.81\ \mathrm{m\,s^{-2}}.
$$

The initial [volume](geometry-and-topology.md#volume) above outlet level is $AH=0.0250\ \mathrm{m^3}=25.0\ \mathrm L$. The initial ideal jet [speed](classical-mechanics.md#speed) is $2.215\ \mathrm{m\,s^{-1}}$, the initial [volumetric flow rate](#volumetric-flow-rate) is $Q_0=0.1373\ \mathrm{L\,s^{-1}}$, and the predicted zero-head time is $T=364.1\ \mathrm s$. These are consequences of stipulated parameters, not experimental measurements. At $t=T/2=182.1\ \mathrm s$, head is $H/4=0.0625\ \mathrm m$, stored [volume](geometry-and-topology.md#volume) is $6.25\ \mathrm L$, and [volumetric flow rate](#volumetric-flow-rate) is $Q_0/2=0.06866\ \mathrm{L\,s^{-1}}$. Half the initial [volume](geometry-and-topology.md#volume) has already left at $t=T(1-1/\sqrt2)=106.7\ \mathrm s$.

<a id="image-constant-area-drainage-quadratic-head-and-linearly-declining-discharge"></a>
![](torricelli-draining-tank-height-and-flow.png)

**[Figure 10](#image-constant-area-drainage-quadratic-head-and-linearly-declining-discharge). Constant-area drainage: quadratic head and linearly declining discharge**. Original synthetic trajectories for the stipulated [draining tank with constant cross-sectional area](#draining-tank-with-constant-cross-sectional-area), with $A=0.100\ \mathrm{m^2}$, $a=10^{-4}\ \mathrm{m^2}$, $C_d=0.620$, $H=0.250\ \mathrm m$ and $g=9.81\ \mathrm{m\,s^{-2}}$. The model remains at zero head and zero [volumetric flow rate](#volumetric-flow-rate) after $T$. The shaded [area](differential-geometry.md#surface-area) under the flow curve represents $25.0\ \mathrm L$.

An independent [mass conservation](continuum-mechanics.md#mass-conservation) check integrates the outgoing [volumetric flow rate](#volumetric-flow-rate):

$$
\int_0^tQ(s)\,ds
=Q_0\left(t-\frac{t^2}{2T}\right)
=A[H-h(t)]\quad(0\le t\le T),
\qquad \int_0^TQ(s)\,ds=\frac{Q_0T}{2}=AH.
$$

Multiply both sides by [mass density](#density) to obtain discharged [mass](classical-mechanics.md#mass). A [dimensional analysis](mathematical-physics.md#dimensional-analysis) check gives $[k]=\mathrm{m^{1/2}\,s^{-1}}$, $[Q]=\mathrm{m^3\,s^{-1}}$ and $[T]=\mathrm s$. The triangular [area](differential-geometry.md#surface-area) under $Q(t)$ explains why the initial-rate estimate $AH/Q_0$ is only half the actual model time. Doubling $A$ doubles $T$; doubling $a$ or $C_d$ halves $T$, within the same assumptions.

This finite-time result is an idealized prediction. The constant $C_d$ and [quasi-steady approximation](mathematics.md#quasi-steady-approximation) need not survive very small head or the initial startup. Appreciable [viscosity](dynamic-viscosity.md) in a narrow outlet tube requires a different [pressure](pressure.md) balance, as in [Poiseuille flow](viscous-fluid-flow.md#hagen-poiseuille-equation); appreciable [surface tension](surface-tension.md) can prevent zero head altogether.

### Discharge measurement in a draining tank

↑ **Parent:** [Torricelli's law](#torricelli-s-law)

[James F. Price](physics.md#james-f-price)'s Draining a Tank, an appendix to Dimensional Analysis of Models and Data Sets, describes an actual tabletop experiment in sections 2.1–2.3. Tap [water](chemical-substance.md#water) filled a semitransparent polypropylene beaker with a marked [volume](geometry-and-topology.md#volume) scale and drilled side openings. Some trials added horizontal outlet tubes. [Temperature](temperature.md) was measured, and dye checked that the [water](chemical-substance.md#water) had settled before uncovering the outlet. The readout was elapsed time at successive [volume](geometry-and-topology.md#volume) marks. Opening diameter and tube length varied between trials. Reported repeatability was checked; tube bores were measured with feeler gauges rather than accepted from nominal sizes.[James F. Price, Draining a Tank, §§2.1–2.3, printed pp. 9–12: preparation, volume/time readout and repeatability](physics-bibliography.md#draining-a-tank-by-james-f-price)

For tank [area](differential-geometry.md#surface-area) $A$ and [volume](geometry-and-topology.md#volume) $W_o$ at outlet level, the observations give $h_i=(W_i-W_o)/A$ and interval [volumetric flow rate](#volumetric-flow-rate) $Q_i\simeq(W_i-W_{i+1})/(t_{i+1}-t_i)$. Price compared $Q/(a\sqrt{2gh})$ across heads to infer a [discharge coefficient](#discharge-coefficient) where that ratio was nearly constant. At small head, drainage could stop with a protruding [water](chemical-substance.md#water) cap; [surface tension](surface-tension.md) mattered. Outlet tubes introduced [viscosity](dynamic-viscosity.md) effects. This experiment tests a useful operating range, rather than proving ideal drainage down to zero head.[James F. Price, Draining a Tank, eqs. (1)–(2), Fig. 2, §3.1 eq. (13), §§4 and 5: coefficient inference and departures from ideal flow](physics-bibliography.md#draining-a-tank-by-james-f-price)

A useful independent test of the constant-coefficient model avoids numerical [derivatives](calculus.md#derivative) of noisy head readings. Its exact [square root](algebra.md#square-root) relation predicts

$$
\sqrt{h(t)}=\sqrt H-bt,\qquad
b=\frac{C_da}{A}\sqrt{\frac g2},\qquad
C_d=\frac{A}{a}\sqrt{\frac2g}\,b.
$$

Fit a straight line to $\sqrt{h_i}$ against time over a chosen positive-head interval; the negative slope determines $b$. Repeat from the same initial head and compare slopes, then vary the head interval to test constancy of $C_d$. This is a proposed diagnostic derived from the [draining tank with constant cross-sectional area](#draining-tank-with-constant-cross-sectional-area), not an additional procedure or measured fit attributed to Price. Startup transients, uncertain outlet level, a changing jet shape and terminal low-head data can spoil the straight line. Independent collection of discharged [volume](geometry-and-topology.md#volume) provides a check on the tank-scale readout.

### Drainage time of a conical tank

↑ **Parent:** [Torricelli's law](#torricelli-s-law)

For a cone of half angle $\pi/4$ draining through a small circular aperture of radius $\epsilon$, the horizontal area at height $h$ is $\pi h^2$. [Torricelli's law](#torricelli-s-law) gives speed $\sqrt{2gh}$, so [conservation of mass](continuum-mechanics.md#mass-conservation) gives $h^2\dot h=-\epsilon^2\sqrt{2gh}$. Integration yields the displayed leading drainage time when $h_0\gg\epsilon$. The final layer $h=O(\epsilon)$ is outside the quasi-steady approximation and contributes only order $\sqrt{\epsilon/g}$, compared with the leading time of order $h_0^{5/2}/(\epsilon^2\sqrt g)$. This is an ideal inviscid estimate without a discharge coefficient.

## Density

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Density)

Mass density is mass per unit volume.

### Relative density

↑ **Parent:** [Density](#density)

The [dimensionless](physics.md#dimensionless-quantity) ratio of a material's [density](#density) to a specified reference [density](#density), with reference conditions stated. Gases are commonly compared with dry air and liquids with [water](chemical-substance.md#water).

### Integrable power-law density at an axis or center

↑ **Parent:** [Density](#density)

A nonnegative [mass density](#density) proportional to $r^p$ has finite local mass near a straight axis if $\int_0^\varepsilon r^{p+1}\,dr$ converges, namely $p>-2$. Near a three-dimensional center the corresponding condition is convergence of $\int_0^\varepsilon r^{p+2}\,dr$, namely $p>-3$. These follow from the [cylindrical volume element](multivariable-calculus.md#cylindrical-volume-element) and [spherical volume element](multivariable-calculus.md#spherical-volume-element). At equality the divergence is logarithmic. An unbounded density does not by itself imply infinite [mass](classical-mechanics.md#mass).

### Density profile

↑ **Parent:** [Density](#density)

The spatial dependence of [density](#density), such as $\rho(r)$ for spherical matter. [Hydrostatic equilibrium](statistical-physics.md#hydrostatic-equilibrium) relates a gas profile and [temperature](temperature.md) to its confining gravitational [mass](classical-mechanics.md#mass).

### Mass current

↑ **Parent:** [Density](#density)

The flux of [mass](classical-mechanics.md#mass) carried by a continuum moving with [velocity](classical-mechanics.md#velocity) $\mathbf v$. In the nonrelativistic limit, $\partial_t\rho+\nabla\cdot\mathbf j_m=0$ is local [mass conservation](continuum-mechanics.md#mass-conservation). A stationary mass current can produce a stationary gravitomagnetic field without emitting [gravitational radiation](gravitational-wave.md).

### Mean density

↑ **Parent:** [Density](#density)

The mean [mass density](#density) of a body is its total [mass](classical-mechanics.md#mass) divided by its [volume](geometry-and-topology.md#volume). A nonuniform density distribution can have the same mean as a uniform one; orbital information that determines only $M/V$ does not determine the internal density profile.

### Mass of an exponential spherical atmosphere

↑ **Parent:** [Density](#density)

For a spherical surface of radius $R$ with exterior [mass density](#density) $\rho(r)=\rho_0e^{-(r-R)/h_0}$, integrate the spherical [volume element](integral.md#volume-element) to obtain $M=4\pi\rho_0\int_0^\infty(R+h)^2e^{-h/h_0}\,dh$. The moments $\int_0^\infty h^ne^{-h/h_0}\,dh=n!h_0^{n+1}$ give the displayed expression. Its leading thin-atmosphere approximation is surface area times column mass, $4\pi R^2\rho_0h_0$; the two positive correction terms account for the growth of shell area with altitude.

### Gas density

↑ **Parent:** [Density](#density)

[Gas density](#gas-density) is the [mass density](#density) of a [gas](thermodynamics.md#gas). For an [ideal gas](ideal-gas.md) sample of [amount of substance](physics.md#amount-of-substance) $n$, mean [molar mass](chemistry.md#molar-mass) $\overline M$ and [volume](thermodynamics.md#volume-thermodynamics) $V$, combine $m=n\overline M$ with $pV=nRT$ to obtain

$$
\rho=\frac{m}{V}=\frac{p\overline M}{RT}.
$$

Here $R$ is the [molar gas constant](ideal-gas.md#molar-gas-constant). For a homogeneous [mixture](mixture.md) of [gases](thermodynamics.md#gas), $\overline M=\sum_i x_iM_i$, where $x_i$ is the [mole fraction](mathematical-biology.md#mole-fraction) of component $i$. Equal [pressure](pressure.md) and [temperature](temperature.md) make a [gas density](#gas-density) ratio equal to a mean-[molar mass](chemistry.md#molar-mass) ratio within this model. [Argon detection in a binary gas mixture](chemical-substance.md#argon-detection-in-a-binary-gas-mixture) gives a worked example and a [temperature](temperature.md) confounder.

#### Gas-globe density measurement

↑ **Parent:** [Gas density](#gas-density)

In an idealized rigid-globe weighing, subtract the evacuated assembly's [mass](classical-mechanics.md#mass) from the filled assembly's [mass](classical-mechanics.md#mass), then divide by the internal [volume](thermodynamics.md#volume-thermodynamics). Establish the filled sample's [pressure](pressure.md) and [temperature](temperature.md) before comparing gases. The subtraction removes the container's large contribution, making a small gas contribution accessible. A real measurement also needs corrections or bounds for residual [gas](thermodynamics.md#gas), [adsorption](physical-chemistry.md#adsorption), leaks, changing vessel volume and external [buoyancy](#buoyancy). The [Rayleigh-Ramsay argon density experiment](chemical-substance.md#rayleigh-ramsay-argon-density-experiment) shows why preparation-route comparisons add information beyond repeated weighings of one sample.

### Linear mass density

↑ **Parent:** [Density](#density)

Linear mass density is [mass](classical-mechanics.md#mass) per unit [length](physics.md#length), measured in $\mathrm{kg\,m^{-1}}$. A uniform string of mass $m$ and length $L$ has $\mu=m/L$; with constant [tension](force.md#tension) $T$, its transverse [wave](wave.md) speed is $\sqrt{T/\mu}$. [Mass density](#density) instead measures mass per unit [volume](geometry-and-topology.md#volume).

### Gas clumping factor

↑ **Parent:** [Density](#density)

The [gas clumping factor](#gas-clumping-factor) measures unresolved inhomogeneity in electron [number density](statistical-physics.md#number-density) within a chosen averaging region. Nonnegative [variance](variance.md) gives $C_e\ge1$. At a uniform [temperature](temperature.md), [thermal bremsstrahlung](astrophysics.md#thermal-bremsstrahlung) scales with $\langle n_e^2\rangle$, whereas the [thermal Sunyaev-Zeldovich effect](cosmic-microwave-background.md#thermal-sunyaev-zeldovich-effect) scales with $\langle n_e\rangle$. A homogeneous [cluster distance from Sunyaev-Zeldovich and X-ray signals](cosmic-microwave-background.md#cluster-distance-from-sunyaev-zeldovich-and-x-ray-signals) inference then gives $d_{A,\mathrm{inferred}}=d_{A,\mathrm{true}}/C_e$, for the same geometry and temperature. Correlated temperature variations require additional weighted averages.

### Projected surface mass density

↑ **Parent:** [Density](#density)

Projected surface mass density is mass per unit projected area, obtained by integrating [mass density](#density) along the line of sight. It determines the enclosed cylindrical mass used by a [thin gravitational lens equation](gravitational-lensing.md#thin-gravitational-lens-equation). It need not equal a physical disk's density, and its aperture mass differs from a spherical three-dimensional enclosed mass.

## Fluid pressure

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

Fluid pressure is the isotropic normal compressive stress in a fluid at rest.

### Cavitation

↑ **Parent:** [Fluid pressure](#fluid-pressure)

Cavitation is the formation of gas or vapour cavities when a liquid's [pressure](pressure.md) becomes sufficiently low. A [journal bearing](viscous-fluid-flow.md#journal-bearing) model with [cavitation](#cavitation) must specify how a partly filled film and its boundaries behave, so periodic [pressure](pressure.md) alone cannot determine the flow there.

### Pressure gradient

↑ **Parent:** [Fluid pressure](#fluid-pressure)

The pressure gradient is the vector $\nabla p$ pointing in the direction of fastest pressure increase. The force density exerted by pressure on a continuum is $-\nabla p$.

#### Adverse pressure gradient

↑ **Parent:** [Pressure gradient](#pressure-gradient)

Along a boundary-layer streamline directed by increasing $s$, an adverse pressure gradient is a rise in [pressure](pressure.md) in the direction of flow. The associated [pressure gradient force](#pressure-gradient-force) opposes the [velocity](classical-mechanics.md#velocity). In a steady inviscid outer stream the [Euler equation](euler-equations-for-an-inviscid-fluid.md) gives $U\,dU/ds=-\rho^{-1}dp/ds$, so a positive gradient decelerates a positive outer velocity. Within a viscous [boundary layer](continuum-mechanics.md#boundary-layer) the slower fluid near the wall has less streamwise momentum and can reverse while the outer stream still moves forward. The onset of [flow separation](continuum-mechanics.md#flow-separation) is therefore associated with vanishing and then reversed [wall shear stress](continuum-mechanics.md#wall-shear-stress). A pressure rise does not by itself locate separation: the full boundary-layer solution and upstream history also matter.

#### Pressure gradient force

↑ **Parent:** [Pressure gradient](#pressure-gradient)

A spatially varying [pressure](pressure.md) exerts net [force](force.md) per unit volume $-\nabla p$ on a small fluid element. Its contribution to [acceleration](classical-mechanics.md#acceleration) is $-\nabla p/\rho$. Pressure increases in the direction opposite to this force.

## Drag (physics)

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Drag_(physics))

A drag force opposes an object's motion relative to a surrounding fluid and transfers momentum between them.

### Air resistance

↑ **Parent:** [Drag (physics)](#drag-physics)

The [drag force](#drag-physics) exerted by air on a body moving relative to it. Neglecting it is an approximation whose accuracy depends on the body, its [speed](classical-mechanics.md#speed) and the ambient [gas](thermodynamics.md#gas).

### Linear drag

↑ **Parent:** [Drag (physics)](#drag-physics)

Linear drag opposes the [velocity](classical-mechanics.md#velocity) relative to the surrounding medium with magnitude proportional to its [speed](classical-mechanics.md#speed), where $\alpha>0$. Its [power](energy.md#power) is $\mathbf F_d\cdot\mathbf v=-\alpha|\mathbf v|^2$, so it dissipates [kinetic energy](energy.md#kinetic-energy). Under a constant external [force](force.md), the resulting [linear ordinary differential equation](linear-ordinary-differential-equation.md) relaxes exponentially on the [time](classical-mechanics.md#time-in-physics) scale $m/\alpha$.

#### Projectile motion with linear drag

↑ **Parent:** [Linear drag](#linear-drag)

For constant [acceleration](classical-mechanics.md#acceleration) vector $\mathbf g$ and $\gamma>0$, a projectile initially at $\mathbf r_0$ with [velocity](classical-mechanics.md#velocity) $\mathbf v_0$ has

$$
\mathbf v(t)=\frac{\mathbf g}{\gamma}+\left(\mathbf v_0-\frac{\mathbf g}{\gamma}\right)e^{-\gamma t},\qquad
\mathbf r(t)=\mathbf r_0+\frac{\mathbf g}{\gamma}t+
\frac{\mathbf v_0-\mathbf g/\gamma}{\gamma}(1-e^{-\gamma t}).
$$

The [integrating factor](linear-ordinary-differential-equation.md#integrating-factor) $e^{\gamma t}$ solves the first-order [linear ordinary differential equation](linear-ordinary-differential-equation.md) for the [velocity](classical-mechanics.md#velocity); one more integration proves the position formula. The terminal [velocity](classical-mechanics.md#velocity) is $\mathbf g/\gamma$, and $1/\gamma$ is the relaxation [time](classical-mechanics.md#time-in-physics). For $\mathbf g=(0,-g)$ and $\mathbf r_0=0$, eliminating time when $V_{0x}\ne0$ gives

$$
z(x)=\left(\frac{V_{0z}}{V_{0x}}+\frac{g}{\gamma V_{0x}}\right)x
+\frac{g}{\gamma^2}\ln\left(1-\frac{\gamma x}{V_{0x}}\right).
$$

For finite $t\geq0$, the physical domain is $0\leq\gamma x/V_{0x}<1$. If $V_{0x}=0$, the path is vertical and cannot generally be represented as a single-valued graph $z(x)$. Expanding at fixed $x$ as $\gamma\to0$ recovers $z=(V_{0z}/V_{0x})x-gx^2/(2V_{0x}^2)$.

#### Mechanical mobility

↑ **Parent:** [Linear drag](#linear-drag)

Mechanical mobility relates a steady drift [velocity](classical-mechanics.md#velocity) to a weak applied mechanical [force](force.md). For isotropic [linear drag](#linear-drag) $-\zeta\mathbf v$, terminal force balance gives $\mathbf v_{\mathrm{drift}}=\mu_{\mathrm{mech}}\mathbf F$ with $\mu_{\mathrm{mech}}=1/\zeta$, in units $\mathrm{s\,kg^{-1}}$. For a sphere obeying [Stokes's law](stokes-flow.md#stokes-s-law), it is $1/(6\pi\eta R)$. The corresponding translational [hydrodynamic mobility matrix](stokes-flow.md#hydrodynamic-mobility-matrix) is $\mu_{\mathrm{mech}}I$. The [Stokes–Einstein relation](stokes-flow.md#stokes-einstein-relation) reads $D=k_BT\mu_{\mathrm{mech}}$, and the [velocity relaxation time](stochastic-process.md#velocity-relaxation-time) is $m\mu_{\mathrm{mech}}$. In the bare-force spherical model, a particle with [electric charge](electric-charge.md) $q$ has [electrophoretic mobility](physical-chemistry.md#electrophoretic-mobility) $\mu_{\mathrm{ep}}=q\mu_{\mathrm{mech}}$; ionic-atmosphere effects can modify that simple model.

#### Overdamped particle dynamics

↑ **Parent:** [Linear drag](#linear-drag)

When momentum relaxes much faster than the imposed motion, [force](force.md) balance replaces the inertial equation: $\zeta\dot x=F(x,t)$ in a deterministic one-dimensional model. The [linear friction coefficient](#linear-friction-coefficient) sets the time scale. Thermal forcing, if included, gives [overdamped Langevin dynamics](stochastic-calculus.md#overdamped-langevin-dynamics).

#### Linear friction coefficient

↑ **Parent:** [Linear drag](#linear-drag)

The dimensional linear friction coefficient relates [drag force](#drag-physics) and [velocity](classical-mechanics.md#velocity), $F_d=-\zeta v$, and has units of [force](force.md) divided by speed. It differs from the dimensionless aerodynamic [drag coefficient](#drag-coefficient). For an isolated sphere in [Stokes flow](stokes-flow.md), the [Stokes drag law](stokes-flow.md#stokes-s-law) gives $\zeta=6\pi\eta a$.

#### Vertical ascent under linear drag

↑ **Parent:** [Linear drag](#linear-drag)

For constant downward gravitational [acceleration](classical-mechanics.md#acceleration) $g$ and [linear drag](#linear-drag) $-\alpha v$, the upward [velocity](classical-mechanics.md#velocity) solves $m\dot v=-mg-\alpha v$ with $v(0)=u_0\ge0$. Its first zero occurs at the displayed [time](classical-mechanics.md#time-in-physics). The dimensionless control variable is $\alpha u_0/(mg)$, and the limit $\alpha\to0$ gives $u_0/g$.

### Drag coefficient

↑ **Parent:** [Drag (physics)](#drag-physics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Drag_coefficient)

The [drag coefficient](#drag-coefficient) measures a [drag force](#drag-physics) against a specified scale of [force](force.md). Let $\mathbf U=\mathbf v_{\rm body}-\mathbf u_\infty$ be the body's [velocity](classical-mechanics.md#velocity) relative to the distant, undisturbed [fluid](#fluid), and let $U=|\mathbf U|>0$ be its relative [speed](classical-mechanics.md#speed). For [fluid](#fluid) [density](#density) $\rho$, [drag force](#drag-physics) magnitude $F_D$ and reference [area](differential-geometry.md#surface-area) $A>0$, define

$$
C_D=\frac{F_D}{\tfrac12\rho U^2A},\qquad F_D=\tfrac12\rho U^2AC_D.
$$

The [drag coefficient](#drag-coefficient) is a [dimensionless quantity](physics.md#dimensionless-quantity): the denominator has units of [force](force.md). The reference [area](differential-geometry.md#surface-area) must be reported with it. For a [sphere](euclidean-geometry.md#sphere) of radius $a$, the usual choice is the frontal [area](differential-geometry.md#surface-area) $A=\pi a^2$. Choosing its entire surface [area](differential-geometry.md#surface-area) $4\pi a^2$ instead divides the reported [drag coefficient](#drag-coefficient) by four for the same physical [drag force](#drag-physics). Comparing coefficients without comparing their reference [areas](differential-geometry.md#surface-area) can therefore be misleading. [NASA Glenn Research Center, Drag Coefficient, definition and Determining Value for Drag Coefficient](https://www1.grc.nasa.gov/beginners-guide-to-aeronautics/drag-coefficient/)

For a rigid [sphere](euclidean-geometry.md#sphere) in [steady flow](#steady-flow) through an unbounded [Newtonian fluid](viscous-fluid-flow.md#newtonian-fluid) with constant [dynamic viscosity](dynamic-viscosity.md) $\mu$, [incompressible flow](#incompressible-flow) and the [no-slip boundary condition](viscous-fluid-flow.md#no-slip-boundary-condition), the creeping-flow limit requires the diameter-based [particle Reynolds number](suspension-chemistry.md#particle-reynolds-number) $\mathrm{Re}_d=2a\rho U/\mu\ll1$. The [Stokes drag law](stokes-flow.md#stokes-s-law) gives $F_D=6\pi\mu aU$. Substitution into the definition with $A=\pi a^2$ gives the short derivation

$$
C_D=\frac{6\pi\mu aU}{\tfrac12\rho U^2\pi a^2}=\frac{12\mu}{\rho aU}=\frac{24}{\mathrm{Re}_d}.
$$

Thus the [drag coefficient](#drag-coefficient) is neither necessarily constant nor bounded above by one. The formula containing $U^2$ still describes [linear drag](#linear-drag) here, because the [drag coefficient](#drag-coefficient) varies as $1/U$. The relation $C_D=24/\mathrm{Re}_d$ is the leading small-[Reynolds number](dynamic-viscosity.md#reynolds-number) approximation, not a measured curve valid at every [Reynolds number](dynamic-viscosity.md#reynolds-number). [Richard Fitzpatrick, Axisymmetric Stokes Flow Around a Solid Sphere, equations 10.126 and 10.129](https://farside.ph.utexas.edu/teaching/336L/Fluid/node142.html)

For a worked example, stipulate [dynamic viscosity](dynamic-viscosity.md) $\mu=0.10\,\mathrm{Pa\,s}$, [density](#density) $\rho=1000\,\mathrm{kg\,m^{-3}}$, radius $a=10^{-4}\,\mathrm m$ and relative [speed](classical-mechanics.md#speed) $U=10^{-3}\,\mathrm{m\,s^{-1}}$. Within the stated [Stokes drag law](stokes-flow.md#stokes-s-law) assumptions,

$$
\mathrm{Re}_d=0.002,\qquad C_D=12000,\qquad F_D=6\pi\times10^{-8}\,\mathrm N\approx1.88495559\times10^{-7}\,\mathrm N.
$$

Doubling the relative [speed](classical-mechanics.md#speed) with all other parameters fixed gives $\mathrm{Re}_d=0.004$ and $C_D=6000$: the predicted [drag force](#drag-physics) doubles to $3.76991118\times10^{-7}\,\mathrm N$. Falsely holding the [drag coefficient](#drag-coefficient) at $12000$ would instead quadruple the [drag force](#drag-physics). Both [particle Reynolds numbers](suspension-chemistry.md#particle-reynolds-number) remain small, so the comparison is within the creeping-flow approximation.

<a id="image-sphere-drag-coefficient-in-the-creeping-flow-approximation"></a>
![](sphere-drag-coefficient-stokes-limit.png)

**[Figure 11](#image-sphere-drag-coefficient-in-the-creeping-flow-approximation). Sphere drag coefficient in the creeping-flow approximation**. The mathematical approximation $C_D=24/\mathrm{Re}_d$ is plotted only for small diameter-based [particle Reynolds number](suspension-chemistry.md#particle-reynolds-number), using frontal reference [area](differential-geometry.md#surface-area) $A=\pi a^2$. The two dots mark the worked example and its doubled relative [speed](classical-mechanics.md#speed). This is a creeping-limit curve, not empirical data or an extension of the [Stokes drag law](stokes-flow.md#stokes-s-law) to all [Reynolds numbers](dynamic-viscosity.md#reynolds-number).

The useful idea is to separate the [force](force.md) scale from the dependence on geometry and flow conditions. A [drag coefficient](#drag-coefficient) can help compare experiments, but changing [Reynolds number](dynamic-viscosity.md#reynolds-number) can change the coefficient itself; NASA Glenn explicitly stresses matching the relevant flow conditions. The elegant cancellation above also exposes a common mistake: a [drag coefficient](#drag-coefficient) definition does not by itself impose a [quadratic drag](#quadratic-drag) law.

### Quadratic drag

↑ **Parent:** [Drag (physics)](#drag-physics)

Quadratic drag has magnitude proportional to the square of the relative speed and points opposite to the relative velocity.

For an [isotropic](continuum-mechanics.md#isotropy) model of a body of fixed shape, let $\mathbf U=\mathbf v_{\rm body}-\mathbf u_\infty$ denote its [relative velocity](classical-mechanics.md#relative-velocity) through the distant [fluid](#fluid), with $U=|\mathbf U|$. A constant positive resistance $k$ gives

$$
\mathbf F_D=-k|\mathbf U|\mathbf U,\qquad F_D=kU^2,\qquad k=\tfrac12\rho AC_D.
$$

Here [density](#density) $\rho$, reference [area](differential-geometry.md#surface-area) $A$ and [drag coefficient](#drag-coefficient) $C_D$ are held fixed over the modeled range of relative [speeds](classical-mechanics.md#speed). The vector formula makes the direction explicit: the [drag force](#drag-physics) on the body opposes its motion relative to the [fluid](#fluid), and vanishes at $U=0$. For a general body, orientation and other flow conditions can affect the [drag coefficient](#drag-coefficient); treating it as a constant requires a regime in which that is an adequate approximation. [NASA Glenn Research Center, Drag Coefficient, Air Viscosity and Compressibility Effects](https://www1.grc.nasa.gov/beginners-guide-to-aeronautics/drag-coefficient/)

Compare two distinct models at a chosen relative [speed](classical-mechanics.md#speed) $U_0>0$. A [linear drag](#linear-drag) model has $F_D(U)/F_D(U_0)=U/U_0$, while a constant-coefficient [quadratic drag](#quadratic-drag) model has $F_D(U)/F_D(U_0)=(U/U_0)^2$. At $U=2U_0$ their [drag force](#drag-physics) ratios are two and four respectively.

<a id="image-normalized-linear-and-quadratic-drag-models-doubling-speed-gives-force-ratios-two-and-four"></a>
![](linear-versus-quadratic-drag-scaling.png)

**[Figure 12](#image-normalized-linear-and-quadratic-drag-models-doubling-speed-gives-force-ratios-two-and-four). Normalized linear and quadratic drag models: doubling speed gives force ratios two and four**. Each model is divided by its own [drag force](#drag-physics) at $U_0$. The [linear drag](#linear-drag) curve applies, for example, to a rigid [sphere](euclidean-geometry.md#sphere) under the [Stokes drag law](stokes-flow.md#stokes-s-law) assumptions while its [particle Reynolds number](suspension-chemistry.md#particle-reynolds-number) remains small. The [quadratic drag](#quadratic-drag) curve assumes constant [density](#density), reference [area](differential-geometry.md#surface-area) and [drag coefficient](#drag-coefficient) over its modeled range. The comparison specifies neither an exact transition nor a single set of physical parameters that realizes both laws throughout the plotted range.

This distinction matters when estimating [terminal velocity](classical-mechanics.md#terminal-velocity) or trajectories such as [descent from rest under quadratic drag](#descent-from-rest-under-quadratic-drag): doubling relative [speed](classical-mechanics.md#speed) increases the resistance much more strongly in the [quadratic drag](#quadratic-drag) model. An approximately constant [drag coefficient](#drag-coefficient) can occur in another [Reynolds number](dynamic-viscosity.md#reynolds-number) regime; its use must be justified there. Conversely, substituting the creeping-flow [sphere](euclidean-geometry.md#sphere) coefficient $C_D=24/\mathrm{Re}_d$ into $F_D=\tfrac12\rho U^2AC_D$ recovers [linear drag](#linear-drag), so writing this general formula does not make the resistance quadratic. Neither approximation should be extended across all [Reynolds numbers](dynamic-viscosity.md#reynolds-number).

The distinction already appears in the original investigation underlying the [Stokes drag law](stokes-flow.md#stokes-s-law), read on 9 December 1850: article 42 identifies resistance proportional to relative [speed](classical-mechanics.md#speed) and distinguishes it from a contribution proportional to the square of relative [speed](classical-mechanics.md#speed). [George Gabriel Stokes, On the Effect of the Internal Friction of Fluids on the Motion of Pendulums, article 42, collected-paper reprint](https://mural.uv.es/daroig/documentos/stokes1850.pdf)

#### Superterminal descent under quadratic drag

↑ **Parent:** [Quadratic drag](#quadratic-drag)

Let downward [velocity](classical-mechanics.md#velocity) $v$ obey $\dot v=a-bv^2$, with constants $a,b>0$, [terminal velocity](classical-mechanics.md#terminal-velocity) $v_t=\sqrt{a/b}$ and initial [speed](classical-mechanics.md#speed) $u>v_t$. Gravity minus [buoyancy](#buoyancy) can supply the constant downward [force](force.md) represented by $a$. Since $\dot z=v$, the equation for $v^2$ is linear in depth: $d(v^2)/dz=-2b(v^2-v_t^2)$, giving the displayed decay. Exact [terminal velocity](classical-mechanics.md#terminal-velocity) is approached only asymptotically. A practical tolerance $v\leq(1+\epsilon)v_t$ is attained at $z_\epsilon=(2b)^{-1}\ln[(u^2/v_t^2-1)/(2\epsilon+\epsilon^2)]$, provided the initial excess exceeds that tolerance. Its [time](classical-mechanics.md#time-in-physics)-domain form is $v=v_t\coth(bv_tt+\chi)$ with $\chi=\operatorname{arctanh}(v_t/u)$, in contrast to the [hyperbolic tangent](calculus.md#hyperbolic-tangent) for [descent from rest under quadratic drag](#descent-from-rest-under-quadratic-drag).

#### Descent from rest under quadratic drag

↑ **Parent:** [Quadratic drag](#quadratic-drag)

For positive downward speed, gravity and [quadratic drag](#quadratic-drag) give $m\dot v=mg-\alpha v^2$, $v(0)=0$. Separation and the integral of $(1-s^2)^{-1}$ give the displayed approach to [terminal velocity](classical-mechanics.md#terminal-velocity). The fallen distance is $(m/\alpha)\log\cosh(\sqrt{\alpha g/m}\,t)$. The limit as $\alpha\to0$ recovers $v=gt$ and distance $gt^2/2$.

#### Quadratic-drag turning angle

↑ **Parent:** [Quadratic drag](#quadratic-drag)

For an ice mass in still water, approximate the wind stress by a fixed vector $a\mathbf e_x$ while retaining [quadratic drag](#quadratic-drag) in the water. With mass per water-drag area $\mu=m/A_w$, water coefficient $b=\rho_wC_w$ and $f=2\Omega\sin\phi$, the steady balance is $a\mathbf e_x=bU\mathbf u+\mu f\widehat{\mathbf z}\times\mathbf u$. Resolving along the drift and perpendicular to it gives $a\cos\theta=bU^2$, $a\sin\theta=\mu|f|U$. Thus $b^2U^4+(\mu f)^2U^2=a^2$ and $\tan\theta=\mu|f|/(bU)$. The direction is right of the wind in the northern hemisphere and left in the southern hemisphere. This angle neglects intrinsic boundary-layer turning, ocean currents and contact forces; it is not a universal observed sea-ice turning angle.

##### Mass per drag area

↑ **Parent:** [Quadratic-drag turning angle](#quadratic-drag-turning-angle)

The normalization $\mu=m/A_w$ has units $\mathrm{kg\,m^{-2}}$. It converts the [Coriolis force](mathematical-physics.md#coriolis-force) into a force per water-drag area and allows comparison with wind and water stresses. [Icebergs](geophysics.md#iceberg) generally have much larger $\mu$ than thin [ice floes](geophysics.md#ice-floe), but their effective air-to-water drag-area ratio also matters. A geometric depth becomes a mass per area only after multiplication by density.

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

## Dynamic viscosity

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](dynamic-viscosity.md)

## Suspension (chemistry)

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](suspension-chemistry.md)

## Mass diffusivity

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mass_diffusivity)

Mass diffusivity is the coefficient multiplying the Laplacian in a diffusion law for a concentration or density anomaly.

## Vorticity

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](vorticity.md)

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

### Sine-cosine cellular Euler flow

↑ **Parent:** [Stream function](#stream-function)

With $u=\psi_y$ and $v=-\psi_x$, this steady incompressible solution of the [Euler equations](euler-equations-for-an-inviscid-fluid.md) has velocity $(-\sin x\sin y,-\cos x\cos y)$ and [vorticity](vorticity.md) $2\psi$. Its pressure is $C+\rho(\cos2x-\cos2y)/4$. The Bernoulli function is $C_0-\psi^2$, so it is constant along streamlines but generally varies between them.

### Steady Euler flow with vorticity proportional to its stream function

↑ **Parent:** [Stream function](#stream-function)

For a smooth planar [incompressible flow](#incompressible-flow), use $u=\psi_y$, $v=-\psi_x$, so its scalar [vorticity](vorticity.md) is $\omega=-\Delta\psi$. If $\omega=\lambda\psi$ for a constant $\lambda$, the flow solves the steady constant-density [Euler equations](euler-equations-for-an-inviscid-fluid.md) with a suitable pressure.

Indeed the vector identity for the convective acceleration gives

$$
(\mathbf u\cdot\nabla)\mathbf u=\nabla(|\mathbf u|^2/2)+\omega\nabla\psi.
$$

Therefore the pressure can be chosen so that the [Bernoulli function](euler-equations-for-an-inviscid-fluid.md#bernoulli-function) satisfies $p/\rho+|\mathbf u|^2/2=C-\lambda\psi^2/2$. Its gradient is $-\omega\nabla\psi$, exactly the steady momentum equation. It is constant along each [streamline](#streamline), since the stream function is constant there.

For example $\psi=\sin x\cos y$ satisfies $\omega=2\psi$. Its pressure is $p_0-\rho\sin^2x/2+\rho\sin^2y/2$. Thus a rotational flow can have an explicit pressure and a streamline-dependent Bernoulli constant.

### Sinusoidal cellular flow

↑ **Parent:** [Stream function](#stream-function)

Using $\mathbf u=(-\psi_y,\psi_x)$, the displayed [stream function](#stream-function) gives $\mathbf u_0=(\sin x\cos y,-\cos x\sin y)$. Its [streamlines](#streamline) are level sets of $\psi_0$. At $(n\pi,m\pi)$, the [Jacobian matrix](multivariable-calculus.md#jacobian-matrix) is $\operatorname{diag}((-1)^{n+m},-(-1)^{n+m})$, so the points are [saddle equilibria](dynamical-systems.md#saddle-equilibrium). At $(\pi/2+n\pi,\pi/2+m\pi)$ the eigenvalues are $\pm i$, giving [center equilibria](dynamical-systems.md#center-equilibrium) surrounded by closed [streamlines](#streamline). The grid lines $x=n\pi$ and $y=m\pi$ form [heteroclinic orbits](dynamical-systems.md#heteroclinic-orbit) between adjacent saddles; circulation alternates between cells.

#### Melnikov splitting of a periodically perturbed cellular flow

↑ **Parent:** [Sinusoidal cellular flow](#sinusoidal-cellular-flow)

Perturb the [sinusoidal cellular flow](#sinusoidal-cellular-flow) by $\epsilon\cos x\cos y\sin(\omega t)$ in its [stream function](#stream-function). On $y=0$, parameterizing the unperturbed orbit with $q_0(0)=(X_0,0)$ gives $x(s)=2\arctan e^{s+a}$, $a=\log\tan(X_0/2)$. The [heteroclinic Melnikov function for a periodic planar flow](dynamical-systems.md#heteroclinic-melnikov-function-for-a-periodic-planar-flow) has integrand $\operatorname{sech}^2(t-t_0+a)\sin(\omega t)$. Its odd part vanishes and the Fourier transform of $\operatorname{sech}^2$ gives the displayed result. For each fixed nonzero frequency its simple zeros produce transverse intersections at sufficiently small perturbation, hence exchange of fluid lobes across the former cell boundary. The leading splitting is exponentially small at high frequency; that estimate is not uniform in frequency and perturbation size.

### Linear planar strain and rotation streamlines

↑ **Parent:** [Stream function](#stream-function)

The incompressible planar field $(\alpha x-\beta y,\beta x-\alpha y)$ has the displayed [stream function](#stream-function) under $(u,v)=(\psi_y,-\psi_x)$ and vorticity $2\beta$. In rotated coordinates $s=(x+y)/\sqrt2$, $t=(x-y)/\sqrt2$, $\psi=((\alpha-\beta)s^2-(\alpha+\beta)t^2)/2$. For positive parameters its nonstationary [streamlines](#streamline) are closed ellipses if $\alpha<\beta$, hyperbolas and straight separatrices if $\alpha>\beta$, and parallel straight lines with a stationary diagonal if $\alpha=\beta$.

### Axisymmetric hydrodynamic mass flux function

↑ **Parent:** [Stream function](#stream-function)

For a steady axisymmetric compressible [fluid flow](#fluid-flow), [mass conservation](continuum-mechanics.md#mass-conservation) permits this representation. The mass flow through an annulus between two stream surfaces is $2\pi\Delta\psi$. In a steady adiabatic wind without magnetic forces, the [specific entropy](entropy.md#specific-entropy), [specific angular momentum](celestial-mechanics.md#specific-angular-momentum) and [Bernoulli function](euler-equations-for-an-inviscid-fluid.md#bernoulli-function) are locally functions of $\psi$ on connected regular stream surfaces.

### Stokes streamfunction

↑ **Parent:** [Stream function](#stream-function)

For axisymmetric incompressible flow without swirl, $u_r=-\psi_z/r$ and $u_z=\psi_r/r$. These identities enforce incompressibility, and $2\pi\psi$ measures axial volume flux from the symmetry axis when its additive constant is chosen there.

#### Stokes streamfunction equation for irrotational flow

↑ **Parent:** [Stokes streamfunction](#stokes-streamfunction)

For an [axisymmetric flow](#axisymmetric-flow) without azimuthal [velocity](classical-mechanics.md#velocity), the spherical [Stokes streamfunction](#stokes-streamfunction) gives $u_r=\Psi_\theta/(r^2\sin\theta)$ and $u_\theta=-\Psi_r/(r\sin\theta)$. These formulas enforce [incompressibility](#incompressible-flow). The only possibly nonzero component of [vorticity](vorticity.md) is

$$
(\nabla\times\mathbf u)_\varphi=-\frac{r^2\Psi_{rr}+\Psi_{\theta\theta}-\cot\theta\,\Psi_\theta}{r^3\sin\theta}.
$$

Thus the displayed equation is precisely the condition for [irrotational flow](vorticity.md#irrotational-flow), away from coordinate poles, with limits interpreted through regularity of the physical [velocity field](#velocity-field). It differs from the scalar spherical [Laplace equation](partial-differential-equation.md#laplace-equation): $\Psi$ is a [Stokes streamfunction](#stokes-streamfunction), not a [velocity potential](#velocity-potential).

##### Sphere theorem for a Stokes streamfunction

↑ **Parent:** [Stokes streamfunction equation for irrotational flow](#stokes-streamfunction-equation-for-irrotational-flow)

Suppose the incident [axisymmetric flow](#axisymmetric-flow) is an [incompressible flow](#incompressible-flow) and an [irrotational flow](vorticity.md#irrotational-flow), with [Stokes streamfunction](#stokes-streamfunction) $\Psi$ regular inside $r<a$. The displayed transformation adds an impermeable [sphere](euclidean-geometry.md#sphere) at $r=a$ without new finite exterior singularities. Writing $s=a^2/r$ and $G=(r/a)\Psi(s,\theta)$, direct differentiation shows

$$
\left(r^2\partial_r^2+\partial_\theta^2-\cot\theta\,\partial_\theta\right)G
=\frac r a\left(s^2\Psi_{ss}+\Psi_{\theta\theta}-\cot\theta\,\Psi_\theta\right)=0.
$$

Hence the [Stokes streamfunction equation for irrotational flow](#stokes-streamfunction-equation-for-irrotational-flow) is preserved. At $r=a$, $\widetilde\Psi=0$, making the radial [velocity](classical-mechanics.md#velocity) zero. Exterior points sample only the regular interior under inversion. If $\Psi$ vanishes at the origin and is $O(r)$ there with smooth regular derivatives, the induced [velocity](classical-mechanics.md#velocity) decays at infinity. This is an inversion construction for an axisymmetric streamfunction, distinct from a scalar [Kelvin transform](partial-differential-equation.md#kelvin-transform).

### Streamline classification of a planar linear saddle or centre

↑ **Parent:** [Stream function](#stream-function)

For $(u,v)=(y,ax)$, the stream function $\psi=(y^2-ax^2)/2$ gives hyperbolic streamlines and a saddle when $a>0$, while $a<0$ gives elliptical streamlines and a centre.

#### Linear planar flow with strain and rotation

↑ **Parent:** [Streamline classification of a planar linear saddle or centre](#streamline-classification-of-a-planar-linear-saddle-or-centre)

The incompressible linear flow $(u,v)=(\epsilon x-\gamma y,\gamma x-\epsilon y)$ has [streamfunction](#stream-function) $\psi=\epsilon xy-\gamma(x^2+y^2)/2$. Its velocity matrix squares to $(\epsilon^2-\gamma^2)I$. Thus strain-dominated flow has saddle trajectories, rotation-dominated flow has closed elliptical trajectories, and equal nonzero strain and rotation gives [simple shear flow](viscous-fluid-flow.md#simple-shear-flow) along parallel lines with a stationary line. Pure rotation is counterclockwise for positive $\gamma$.

## Streamline

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Streamline)

A [streamline](#streamline) at a specified instant $T$ is a curve whose [tangent line](calculus.md#tangent-line) follows the [velocity field](#velocity-field) at that same frozen instant everywhere along the curve. One convenient [integral curve](multivariable-calculus.md#integral-curve-of-a-vector-field) parameterization is

$$
\frac{d\boldsymbol\gamma}{ds}=\mathbf u(\boldsymbol\gamma(s),T),\qquad T\text{ fixed}.
$$

Here $s$ is an auxiliary curve parameter, with units of seconds in this convention; advancing $s$ does not advance physical time. Any regular reparameterization preserves the tangent geometry. Where $u_x\ne0$, a planar [streamline](#streamline) satisfies $dy/dx=u_y/u_x$ evaluated at time $T$. At a [stagnation point](#stagnation-point) the [velocity field](#velocity-field) has no direction; under the local [Lipschitz condition](real-analysis.md#lipschitz-continuity) of the [Picard-Lindelöf theorem](differential-equation.md#picard-lindelof-theorem), regular [streamlines](#streamline) at the same time cannot cross. A [streamline](#streamline) answers which directions fit together now, making it useful for describing local flow geometry. [MIT fluid mechanics modules, tutorial on streamlines, streaklines and pathlines](https://web.mit.edu/fluids-modules/www/potential_flows/LecturesHTML/lec02/tutorial/)

In the analytical [velocity field](#velocity-field) $(U,at)$ introduced under [pathline](#pathline), the [streamline](#streamline) through the origin at time $T$ is

$$
y=\frac{aT}{U}x.
$$

At $T=2\ \mathrm s$ this is $y=2x$ when both coordinates are expressed in metres. At $x=1\ \mathrm m$ its height is $2\ \mathrm m$, whereas the earlier [pathline](#pathline) of the origin's first released [fluid element](continuum-mechanics.md#fluid-element) has height $0.5\ \mathrm m$. Its instantaneous [streamline](#streamline) at the final position $(2,2)\ \mathrm m$ is instead $y-2\ \mathrm m=2(x-2\ \mathrm m)$: the [pathline](#pathline) is tangent to that [streamline](#streamline) at its current endpoint, although its recorded history does not lie along it.

<a id="image-analytical-comparison-of-a-frozen-time-streamline-one-pathline-and-a-streakline"></a>
![](stream-path-streak-lines-three-curves.png)

**[Figure 13](#image-analytical-comparison-of-a-frozen-time-streamline-one-pathline-and-a-streakline). Analytical comparison of a frozen-time streamline, one pathline and a streakline**.

The green [streamline](#streamline) uses the [velocity field](#velocity-field) at $T=2\ \mathrm s$ throughout; the orange [pathline](#pathline) uses times $0\leq t\leq2\ \mathrm s$; the purple [streakline](#streakline) uses different release times at the single observation time $T=2\ \mathrm s$. The grey arrows all show the instantaneous [velocity](classical-mechanics.md#velocity) direction at $T$. These are exact analytical curves with chosen units, not measured dye shapes.

In a [steady flow](#steady-flow) in a fixed [reference frame](mathematical-physics.md#reference-frame), a [pathline](#pathline) and a [streamline](#streamline) solve the same autonomous [ordinary differential equation](differential-equation.md#ordinary-differential-equation). Uniqueness makes each particle released from a fixed point follow the same [integral curve](multivariable-calculus.md#integral-curve-of-a-vector-field), so its [pathline](#pathline), the [streakline](#streakline) from that point and the [streamline](#streamline) share one geometrical curve. Finite recording or release intervals usually show different segments of that curve; the comparison assumes particles stay in the domain and treats stationary [fluid elements](continuum-mechanics.md#fluid-element) separately. Neither two-dimensionality nor [incompressibility](#incompressible-flow) is needed for this coincidence. Steadiness is sufficient, but is not necessary: $\mathbf u(\mathbf x,t)=g(t)\mathbf v(\mathbf x)$ with smooth $g(t)>0$ changes [speed](classical-mechanics.md#speed) while preserving the same [integral curves](multivariable-calculus.md#integral-curve-of-a-vector-field). In a general time-dependent [velocity field](#velocity-field), however, the three curves differ. Kline explains why continuous dye release in [steady flow](#steady-flow) can therefore display [streamlines](#streamline). [S. J. Kline, Flow Visualization film notes, section II](https://web.mit.edu/hml/ncfmf/05FV.pdf)

For two-dimensional [incompressible flow](#incompressible-flow), the convention $\mathbf u=(\partial_y\psi,-\partial_x\psi)$ gives $\mathbf u\cdot\nabla\psi=0$, so regular [streamlines](#streamline) are [level sets](topology.md#level-set) of the [stream function](#stream-function) at each frozen time. In time-dependent [incompressible flow](#incompressible-flow), that does not force a [pathline](#pathline) to stay on one numerical value of $\psi$: its [material derivative](continuum-mechanics.md#material-derivative) is $D\psi/Dt=\partial_t\psi$. The distinction is the difference between a geometric snapshot and a parcel's history.

### Free streamline

↑ **Parent:** [Streamline](#streamline)

A [free streamline](#free-streamline) is a [streamline](#streamline) that forms an unknown [boundary](topology.md#boundary-of-a-set) of a [fluid](#fluid) region, typically against a region of prescribed pressure. In steady inviscid [potential flow](#potential-flow) with gravity and surface tension neglected, the [Bernoulli equation](euler-equations-for-an-inviscid-fluid.md#bernoulli-equation) makes its [speed](classical-mechanics.md#speed) constant when its pressure is constant. It is simultaneously a level set of the [stream function](#stream-function). These two [boundary conditions](differential-equation.md#boundary-condition) take particularly simple forms in the [complex potential of a two-dimensional potential flow](#complex-potential-of-a-two-dimensional-potential-flow) and the [hodograph plane](#hodograph-plane).

### Stream tube

↑ **Parent:** [Streamline](#streamline)

A [stream tube](#stream-tube) is a narrow tube whose side boundary consists of [streamlines](#streamline). In steady flow no fluid crosses its sides, so continuity makes its [mass flux](mathematical-physics.md#mass-flux) $A\rho u$ constant. If flow follows a [magnetic field](magnetic-field.md) with constant [magnetohydrodynamic mass loading](ideal-magnetohydrodynamics.md#magnetohydrodynamic-mass-loading), its normal area obeys $A|\mathbf B|=\mathrm{constant}$.

## Velocity potential

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Velocity_potential)

Use a [velocity potential](#velocity-potential) to reconstruct an [irrotational flow](vorticity.md#irrotational-flow) from one [scalar field](classical-field-theory.md#scalar-field). A [velocity potential](#velocity-potential) $\phi(\mathbf x,t)$ satisfies

$$
\mathbf u=\nabla\phi.
$$

It has units $\mathrm{m^2\,s^{-1}}$ and is unchanged as a description of the [velocity field](#velocity-field) when any function of time alone is added. For twice continuously differentiable $\phi$, the identity [curl of a gradient](multivariable-calculus.md#curl-of-a-gradient) proves zero [vorticity](vorticity.md). In [incompressible flow](#incompressible-flow), taking the [divergence](multivariable-calculus.md#divergence) also gives $\nabla^2\phi=0$, the [Laplace equation](partial-differential-equation.md#laplace-equation). This turns a three-component [velocity field](#velocity-field) into a single [harmonic function](partial-differential-equation.md#harmonic-function) with appropriate [boundary conditions](differential-equation.md#boundary-condition). [A. H. Techet, MIT Hydrodynamics reading 4, pp. 1–3](https://ocw.mit.edu/courses/2-016-hydrodynamics-13-012-fall-2005/c472432debcf6ee250209b68cf18cc12_2005reading4.pdf)

For [uniform flow](#uniform-flow) $\mathbf u=(U,0,0)$, take $\phi=Ux$. With $U=2\ \mathrm{m\,s^{-1}}$, the change from $x=0$ to $x=3\ \mathrm m$ is $\Delta\phi=6\ \mathrm{m^2\,s^{-1}}$. By the [fundamental theorem for line integrals](multivariable-calculus.md#fundamental-theorem-for-line-integrals), the [line integral](multivariable-calculus.md#line-integral) of [velocity](classical-mechanics.md#velocity) between these points equals that change along any path in the domain; a [closed curve](topology.md#closed-curve) gives zero [circulation](vorticity.md#circulation-physics).

For the potential [line vortex](vorticity.md#line-vortex), choose a local angle branch in [polar coordinates](multivariable-calculus.md#polar-coordinates) and set $\phi=K\theta$. Then $u_r=\partial_r\phi=0$ and $u_\theta=r^{-1}\partial_\theta\phi=K/r$. One counterclockwise turn changes the continued [velocity potential](#velocity-potential) by $2\pi K$, although the [velocity field](#velocity-field) returns to its original value. With $K=1\ \mathrm{m^2\,s^{-1}}$, this change is $2\pi\ \mathrm{m^2\,s^{-1}}$, exactly the [circulation](vorticity.md#circulation-physics). A full [annulus](topology.md#annulus-mathematics) therefore admits local angle branches and a multivalued [velocity potential](#velocity-potential), but no global single-valued [velocity potential](#velocity-potential) when $K\ne0$. Cutting the [annulus](topology.md#annulus-mathematics) along a radial line allows a single-valued angle branch on the remaining domain. The obstruction is [path independence](multivariable-calculus.md#path-independence), not a failure of the local [gradient](multivariable-calculus.md#gradient) formula.

### Additive freedom of a velocity potential

↑ **Parent:** [Velocity potential](#velocity-potential)

Adding a spatially constant function of time to a [velocity potential](#velocity-potential) leaves its [velocity](classical-mechanics.md#velocity) $\mathbf u=\nabla\phi$ unchanged. When integrating the [Euler equations](euler-equations-for-an-inviscid-fluid.md) in space, this freedom can absorb the time-only integration term in the potential form of momentum balance. A spatially constant zero-frequency potential represents no acoustic velocity and must not be counted as a propagating [normal mode](wave-equation.md#normal-mode) merely because a frequency determinant vanishes at zero. Pressure conventions and time dependence must still be fixed consistently when the potential is used to recover physical fields.

### Potential flow around a circular cylinder

↑ **Parent:** [Velocity potential](#velocity-potential)

Uniform irrotational flow of speed $U$ past a circular cylinder of radius $a$, with zero circulation, has [velocity potential](#velocity-potential)

$$
\phi=U\left(r+\frac{a^2}{r}\right)\cos\theta.
$$

On the cylinder, the tangential speed is $-2U\sin\theta$, so the [Bernoulli equation](euler-equations-for-an-inviscid-fluid.md#bernoulli-equation) gives

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

##### Surface stagnation points of a circulating cylinder flow

↑ **Parent:** [Potential flow around a circular cylinder with circulation](#potential-flow-around-a-circular-cylinder-with-circulation)

For [complex potential of a two-dimensional potential flow](#complex-potential-of-a-two-dimensional-potential-flow) $w=U(z+a^2/z)-i\Gamma\log z/(2\pi)$, zeros of the [complex velocity](#complex-velocity) solve a quadratic. If $0<\gamma<1$, the displayed two roots are distinct and both have modulus $a$; positive [circulation](vorticity.md#circulation-physics) places them above the centreline. Their polar angles satisfy $\sin\theta=\gamma$. At the threshold $\gamma=1$ they merge at the top of the cylinder. This follows also from the surface tangential velocity $-2U\sin\theta+\Gamma/(2\pi a)$. The shifted [stream function](#stream-function) $U(r-a^2/r)\sin\theta-\Gamma\log(r/a)/(2\pi)$ is constant on the cylinder.

<h5 id="kutta-joukowski-theorem">Kutta–Joukowski theorem</h5>

↑ **Parent:** [Potential flow around a circular cylinder with circulation](#potential-flow-around-a-circular-cylinder-with-circulation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kutta–Joukowski_theorem)

For steady two-dimensional inviscid flow of density $\rho$, far-field velocity $\mathbf U$, and circulation $\kappa$, the force per unit span is perpendicular to the flow. With counterclockwise circulation taken positive and $\mathbf U=U\mathbf e_x$, it is $-\rho\kappa U\mathbf e_y$.

###### Advective and pressure contributions to circulatory lift

↑ **Parent:** [Kutta–Joukowski theorem](#kutta-joukowski-theorem)

For [uniform flow](#uniform-flow) $\mathbf U$ plus a [line vortex](vorticity.md#line-vortex) of counterclockwise [circulation](vorticity.md#circulation-physics) $\Gamma$, the outward advective [momentum flux](mathematical-physics.md#momentum-flux) around a large circle is $\rho\boldsymbol\Gamma\times\mathbf U/2$. The [Bernoulli equation](euler-equations-for-an-inviscid-fluid.md#bernoulli-equation) supplies an equal [pressure](pressure.md) contribution. Their sum is the force on the fluid; the force on an obstacle per unit span is its negative, $\rho\mathbf U\times\boldsymbol\Gamma$. Retaining only the advective term loses half the lift and obscures its sign.

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

If the pressure at $r=b(t)$ is $p_\infty$, the [Unsteady Bernoulli equation](euler-equations-for-an-inviscid-fluid.md#unsteady-bernoulli-equation) gives

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

[This section is present in another page, follow this link to view it.](euler-equations-for-an-inviscid-fluid.md)

## Conservation of mass in a pipe

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conservation_of_mass_in_a_pipe)

For steady incompressible pipe flow, volume flux equals cross-sectional area times mean speed and is conserved through a junction.

## Surface tension

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](surface-tension.md)

## Viscous fluid flow

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](viscous-fluid-flow.md)

## Body force

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Body_force)

A [body force](#body-force) acts throughout a body's or [fluid](#fluid)'s [volume](geometry-and-topology.md#volume), rather than only through its surface. [Gravity](physics.md#gravity) is the example used in [hydrostatic pressure](#hydrostatic-pressure): a [gravitational field](physics.md#gravitational-field) $\mathbf g$ gives [force](force.md) per unit [volume](geometry-and-topology.md#volume) $\rho\mathbf g$, where $\rho$ is the [mass density](#density). More generally, a [body force](#body-force) per unit [mass](classical-mechanics.md#mass) $\mathbf f$ contributes $\rho\mathbf f$ to [momentum conservation](momentum.md#momentum-conservation). [Forces](force.md) from [electromagnetism](electromagnetism.md) are another example. Surface [pressure](pressure.md) [forces](force.md) produce [buoyancy](#buoyancy) on an immersed body, while its [body force](#body-force) from [gravity](physics.md#gravity) acts downward.

### Elastic force dipole

↑ **Parent:** [Body force](#body-force)

Opposite forces separated along the unit direction $\mathbf e$, with fixed force times separation $D$, have this distributional [body force](#body-force) limit. Its net force is zero. A symmetric [seismic moment tensor](wave-equation.md#seismic-moment-tensor) is a sum of such dipoles along its principal directions.

## Hydrostatic pressure

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hydrostatic_pressure)

[Hydrostatic pressure](#hydrostatic-pressure) is the [pressure](pressure.md) distribution in a resting [fluid](#fluid), balancing its [body force](#body-force) from [gravity](physics.md#gravity). Take $z$ upward and a uniform downward [gravitational field](physics.md#gravitational-field) $\mathbf g=-g\mathbf e_z$, where $g>0$. The vertical [pressure gradient](#pressure-gradient) satisfies

$$
\frac{dp}{dz}=-\rho_f g.
$$

A short derivation balances the vertical [forces](force.md) on a thin horizontal layer of [area](differential-geometry.md#surface-area) $A$ and thickness $\Delta z$: $p(z)A-p(z+\Delta z)A-\rho_fgA\Delta z=0$. Dividing by $A\Delta z$ and taking the [derivative](calculus.md#derivative) gives the equation above. For constant [mass density](#density) $\rho_f$, [integration](integral.md) from the surface at $z_s$ gives

$$
p(z)=p_{\mathrm{surface}}+\rho_fg(z_s-z)
=p_{\mathrm{surface}}+\rho_fgh,\qquad h=z_s-z.
$$

Thus [pressure](pressure.md) increases with depth $h$. For the stipulated [water](chemical-substance.md#water) with [mass density](#density) $1000\ \mathrm{kg\,m^{-3}}$ and [gravitational acceleration](newton-s-law-of-universal-gravitation.md#gravitational-acceleration) $9.81\ \mathrm{m\,s^{-2}}$, depths $0.20\ \mathrm m$ and $0.30\ \mathrm m$ give [gauge pressures](#gauge-pressure) $1962\ \mathrm{Pa}$ and $2943\ \mathrm{Pa}$. Their difference produces the [buoyancy](#buoyancy) of the example [cube](euclidean-geometry.md#cube). [Feynman Lectures, II §40-1: hydrostatics](https://www.feynmanlectures.caltech.edu/II_40.html#Ch40-S1)

### Triangular-channel hydrostatic pressure head

↑ **Parent:** [Hydrostatic pressure](#hydrostatic-pressure)

For a fixed symmetric triangular channel with depth $H$ and [area](differential-geometry.md#surface-area) $A=kH^2$, the hydrostatic first moment is $I=\int_A(H-z)\,dA=kH^3/3=AH/3$. Since $dI/dH=A$, the depth-averaged [pressure gradient](#pressure-gradient) is $gI_x/A=gH_x$. A mean geometric depth $H/2$ cannot replace $H$ in that gradient without an extra factor two. This distinction prevents confusion between [pressure](pressure.md) head, centroid depth, and [hydraulic radius](#hydraulic-radius).

### Gauge pressure

↑ **Parent:** [Hydrostatic pressure](#hydrostatic-pressure)

[Gauge pressure](#gauge-pressure) is [pressure](pressure.md) measured relative to the surrounding [atmospheric pressure](pressure.md#atmospheric-pressure); absolute [pressure](pressure.md) is instead measured relative to an ideal [vacuum](physics.md#vacuum). At an open surface $p_{\mathrm{surface}}=p_{\mathrm{atmosphere}}$, so the constant-[mass density](#density) [hydrostatic pressure](#hydrostatic-pressure) law becomes $p_g=\rho_fgh$. Here $p_g=0$ at the surface denotes equality with [atmospheric pressure](pressure.md#atmospheric-pressure). It does not denote zero absolute [pressure](pressure.md). [OpenStax, University Physics, §14.2: gauge and absolute pressure](physics-bibliography.md#university-physics-volume-1-by-william-moebs-and-others)

### Hydrostatic approximation

↑ **Parent:** [Hydrostatic pressure](#hydrostatic-pressure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hydrostatic_approximation)

The hydrostatic approximation neglects vertical acceleration relative to gravity and vertical pressure gradients. It reduces vertical momentum balance to $p_z=-\rho g$.

#### Hydrostatic balance

↑ **Parent:** [Hydrostatic approximation](#hydrostatic-approximation)

Vertical [pressure gradient](#pressure-gradient) balances gravitational force per unit volume. Subtracting the resting hydrostatic state and using [kinematic pressure](pressure.md#kinematic-pressure) gives $p'_z=b'$ for a [Boussinesq approximation](geophysical-fluid-dynamics.md#boussinesq-approximation) buoyancy anomaly. The approximation neglects vertical [acceleration](classical-mechanics.md#acceleration); this diagnostic relation is what couples [buoyancy perturbation](#buoyancy-perturbation) to the vertical pressure profile.

##### Hydrostatic atmosphere with a constant temperature lapse rate

↑ **Parent:** [Hydrostatic balance](#hydrostatic-balance)

For an [ideal gas](ideal-gas.md) with constant composition, set $\mathcal R=k_B/\bar m$, where $\bar m$ is the mean particle [mass](classical-mechanics.md#mass). Constant downward [gravitational acceleration](newton-s-law-of-universal-gravitation.md#gravitational-acceleration) $g$ and $T=T_0-\alpha z>0$ give $p'=-(g/\mathcal R T)p$ by [hydrostatic equilibrium](statistical-physics.md#hydrostatic-equilibrium). Integration gives $p/p_0=(T/T_0)^{g/(\mathcal R\alpha)}$, and the [ideal gas law](ideal-gas.md#ideal-gas-law) gives the displayed [mass density](#density) ratio. The isothermal limit $\alpha\to0$ is $\rho/\rho_0=\exp[-gz/(\mathcal R T_0)]$.

## Volumetric flow rate

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Volumetric_flow_rate)

The volumetric flow rate is the volume of fluid crossing a section per unit time, $Q=\int_A\mathbf u\mathbin\cdot\mathbf n\,dA$.

### Discharge

↑ **Parent:** [Volumetric flow rate](#volumetric-flow-rate)

River [discharge](#discharge) is [volume flux](#volumetric-flow-rate) across a channel section. For approximately uniform cross-sectional [velocity](classical-mechanics.md#velocity) it equals flow [area](differential-geometry.md#surface-area) times mean [velocity](classical-mechanics.md#velocity). Its time dependence at a fixed station is a [hydrograph](#hydrograph).

#### Hydrograph

↑ **Parent:** [Discharge](#discharge)

A [hydrograph](#hydrograph) records [discharge](#discharge) against time at a fixed location. A nonlinear [kinematic wave](transport-equation.md#kinematic-wave) can steepen an upstream increase into a sharp front; longitudinal [diffusion](thermodynamics.md#diffusion) or additional storage rounds the resulting rise.

### Sverdrup

↑ **Parent:** [Volumetric flow rate](#volumetric-flow-rate)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sverdrup)

A unit of [volume flux](#volumetric-flow-rate) used for [ocean circulation](geophysical-fluid-dynamics.md#ocean-circulation). Its symbol is $\mathrm{Sv}$; this denotes a volume transported per time, not a [velocity](classical-mechanics.md#velocity).

### Mass flow rate

↑ **Parent:** [Volumetric flow rate](#volumetric-flow-rate)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mass_flow_rate)

The mass flow rate through an oriented cross-section is the integral of [mass density](#density) times normal [velocity](classical-mechanics.md#velocity). For constant density it is density times the [volumetric flow rate](#volumetric-flow-rate). In a steady pipe without leaks, [conservation of mass](continuum-mechanics.md#mass-conservation) makes this rate independent of cross-section.

#### Coolant mass flux

↑ **Parent:** [Mass flow rate](#mass-flow-rate)

[Coolant](engineering.md#coolant) [mass flow rate](#mass-flow-rate) per open flow area, measured in $\mathrm{kg\,m^{-2}\,s^{-1}}$. A decrease in total flow does not establish a decrease in mass flux when the open area also changes.

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

### Rankine oval

↑ **Parent:** [Potential flow](#potential-flow)

A uniform planar stream combined with an equal source and sink produces a closed dividing [streamline](#streamline) enclosing them. Outside it the flow approaches the uniform stream; inside it streamlines connect the source and sink. For positive $U,m$ and separation one, the [complex velocity](#complex-velocity) is $U-m/[2\pi z(z-1)]$ and the stagnation points are $[1\pm\sqrt{1+2m/(\pi U)}]/2$. Both lie on the dividing streamline, which has zero streamfunction with consistent logarithm branches.

### Kutta condition

↑ **Parent:** [Potential flow](#potential-flow)

The [Kutta condition](#kutta-condition) selects the circulation of an idealized [potential flow](#potential-flow) past a body with a sharp trailing edge by requiring finite limiting velocity at that edge. For the [Joukowski map](geometry-and-topology.md#joukowski-map) $z=\zeta+a^2/\zeta$, the trailing edge $z=2a$ corresponds to a simple zero of $dz/d\zeta$ at $\zeta=a$. If $W$ is the [complex potential](#complex-potential-of-a-two-dimensional-potential-flow) in the circle plane, then $dw/dz=W'(\zeta)/(1-a^2/\zeta^2)$ is finite there only if $W'(a)=0$. For a [uniform flow](#uniform-flow) of speed $U$ at angle $\alpha$ and a [point vortex](vorticity.md#line-vortex) of circulation $\Gamma$, this gives $\Gamma=-4\pi Ua\sin\alpha$, and cancellation of the simple zeros gives the tangential trailing-edge velocity $U\cos\alpha$. The opposite endpoint can retain a leading-edge singularity.

### Uniform potential flow around an ellipse

↑ **Parent:** [Potential flow](#potential-flow)

For $0<a<1$, the [Joukowski map](geometry-and-topology.md#joukowski-map) $z=\zeta+a^2/\zeta$ maps the exterior [unit circle](complex-analysis.md#complex-unit-circle) to an [ellipse](euclidean-geometry.md#ellipse) of horizontal and vertical semiaxes $1+a^2$ and $1-a^2$. The [Milne-Thomson circle theorem](#milne-thomson-circle-theorem) gives $W(\zeta)=U(e^{-i\alpha}\zeta+e^{i\alpha}/\zeta)$ for a [uniform flow](#uniform-flow) inclined by $\alpha$. The [chain rule](calculus.md#chain-rule) produces the displayed [complex velocity](#complex-velocity) in the physical plane. Since $z\sim\zeta$, the far-field flow retains its speed and direction. Its two [stagnation points](#stagnation-point) are

$$
z=\pm[(1+a^2)\cos\alpha+i(1-a^2)\sin\alpha],
$$

obtained from $\zeta=\pm e^{i\alpha}$. The map derivative is nonzero on and outside the [unit circle](complex-analysis.md#complex-unit-circle), so these zeros are preserved without introducing a boundary singularity.

### Boundary integral for kinetic energy of planar potential flow

↑ **Parent:** [Potential flow](#potential-flow)

For a smooth constant-density exterior [potential flow](#potential-flow) satisfying the [finite-energy condition for planar exterior potential flow](#finite-energy-condition-for-planar-exterior-potential-flow), use $\mathbf u=\nabla\phi$ and the planar [streamfunction](#stream-function) convention $u=\psi_y$, $v=-\psi_x$. Since $\nabla^2\phi=0$, $\nabla\cdot(\phi\nabla\phi)=|\mathbf u|^2$. Apply the [divergence theorem](multivariable-calculus.md#divergence-theorem) to a truncated exterior region. The outer term vanishes; on a counterclockwise body boundary the body's outward normal satisfies $\partial_n\phi\,ds=d\psi$, while the fluid's outward normal points the opposite way. This gives the displayed [kinetic energy](energy.md#kinetic-energy) per unit span. The formula yields the [added mass of a circular cylinder](mathematical-physics.md#added-mass-of-a-circular-cylinder) directly from its surface values of $\phi$ and $\psi$.

### Finite-energy condition for planar exterior potential flow

↑ **Parent:** [Potential flow](#potential-flow)

For a planar [potential flow](#potential-flow) outside a bounded body, suppose its single-valued [complex velocity](#complex-velocity) $q=u-iv$ is holomorphic near infinity and tends to zero. Its exterior [Laurent series](analysis.md#laurent-series) begins $q=b_1/z+O(z^{-2})$. The outward [volume flux](#volumetric-flow-rate) $Q$ and counterclockwise [circulation](vorticity.md#circulation-physics) $\Gamma$ satisfy $\Gamma+iQ=2\pi i b_1$. Thus both vanish precisely when the leading term is absent. A nonzero $b_1$ gives $|q|^2\sim|b_1|^2/r^2$ and logarithmically divergent exterior [kinetic energy](energy.md#kinetic-energy). When $b_1=0$, $q=O(r^{-2})$ and the far-field energy integral converges. Zero [circulation](vorticity.md#circulation-physics) alone does not exclude the radial source field $\nabla\log r$.

### Uniform potential flow around a fixed sphere

↑ **Parent:** [Potential flow](#potential-flow)

For a fixed impermeable [sphere](euclidean-geometry.md#sphere) of radius $a$ and incident [uniform flow](#uniform-flow) $U\mathbf e_z$, the [velocity potential](#velocity-potential) is the displayed expression and the [Stokes streamfunction](#stokes-streamfunction) is $\Psi=(U/2)(r^2-a^3/r)\sin^2\theta$. Differentiation gives $u_r=U(1-a^3/r^3)\cos\theta$ and $u_\theta=-U(1+a^3/(2r^3))\sin\theta$. Thus the [no-penetration boundary condition](viscous-fluid-flow.md#no-penetration-boundary-condition) holds, the poles are [stagnation points](#stagnation-point), and the equatorial surface speed is $3U/2$. The disturbance is a [potential dipole](#potential-dipole) decaying as $r^{-3}$ in [velocity](classical-mechanics.md#velocity). The [sphere theorem for a Stokes streamfunction](#sphere-theorem-for-a-stokes-streamfunction) constructs this solution from $\Psi_0=Ur^2\sin^2\theta/2$.

### Potential of a translating sphere

↑ **Parent:** [Potential flow](#potential-flow)

For a sphere translating through an unbounded inviscid incompressible fluid at rest far away, the laboratory fluid [velocity](classical-mechanics.md#velocity) written in coordinates centred on the moving sphere is the gradient of the displayed dipole potential. Its radial [velocity](classical-mechanics.md#velocity) at the surface equals $U\cos\theta$. The sphere-rest-frame [velocity](classical-mechanics.md#velocity) instead needs the additional uniform potential $-Ur\cos\theta$.

### Complex potential of a two-dimensional potential flow

↑ **Parent:** [Potential flow](#potential-flow)

For an incompressible irrotational two-dimensional [potential flow](#potential-flow), an analytic [complex potential of a two-dimensional potential flow](#complex-potential-of-a-two-dimensional-potential-flow) combines the velocity potential $\Phi$ and [streamfunction](#stream-function) $\Psi$. The [Cauchy-Riemann equations](analysis.md#cauchy-riemann-equations) give $u=\Phi_x=\Psi_y$ and $v=\Phi_y=-\Psi_x$, hence $W'(z)=u-iv$. Curves of constant $\Psi$ are [streamlines](#streamline). An analytic coordinate change $z=f(\zeta)$ transforms the complex velocity by $dW/dz=(dW/d\zeta)/f'(\zeta)$ wherever $f'\neq0$.

#### Planar potential dipole

↑ **Parent:** [Complex potential of a two-dimensional potential flow](#complex-potential-of-a-two-dimensional-potential-flow)

A [planar potential dipole](#planar-potential-dipole) at $a$ with complex moment $m$ has [complex potential of a two-dimensional potential flow](#complex-potential-of-a-two-dimensional-potential-flow) $w(z)=m/(z-a)$. Its [complex velocity](#complex-velocity) is $w'(z)=-m/(z-a)^2$, interpreted as $v_x-iv_y$. Unlike the three-dimensional [potential dipole](#potential-dipole), this is a two-dimensional singularity of the logarithmic-source potential. For example, two opposite source coefficients $s$ at $a\pm\delta/2$ have potential $s[\log(z-a-\delta/2)-\log(z-a+\delta/2)]$, whose leading term is $-s\delta/(z-a)$ as the separation tends to zero with $s\delta$ fixed. This gives the [dipole](#planar-potential-dipole) as a limiting source–sink pair, with the complex sign and orientation included in $m$.

##### Wall-induced motion of a planar potential dipole

↑ **Parent:** [Planar potential dipole](#planar-potential-dipole)

A transported [planar potential dipole](#planar-potential-dipole) follows the surrounding regular [velocity](classical-mechanics.md#velocity), so its position satisfies the displayed equation after its own singular term is removed. The [conjugation](group-action.md#conjugation) comes from the convention $w'=v_x-iv_y$. Reflected image parameters are held fixed when taking the spatial [derivative](calculus.md#derivative), then evaluated at the instantaneous [dipole](#planar-potential-dipole) position.

For a unit circular wall, the [Milne-Thomson circle theorem](#milne-thomson-circle-theorem) gives image potential $\bar m z/(1-\bar a z)$ and therefore $\dot{\bar a}=\bar m/(1-|a|^2)^2$. For a horizontal straight wall the image is $\bar m/(z-\bar a)$, giving $\dot{\bar a}=-\bar m/(a-\bar a)^2$. For the line $y=-x$, reflected [conjugation](group-action.md#conjugation) gives image $-i\bar m/(z+i\bar a)$ and hence $\dot{\bar a}=i\bar m/(a+i\bar a)^2$. In each case the image lies outside the fluid region and makes the wall a [streamline](#streamline); differentiation of the regular image proves the motion formula. Several compatible straight-wall reflections can be summed before the same operation is applied.

#### Reflection image of a planar hydrodynamic dipole

↑ **Parent:** [Complex potential of a two-dimensional potential flow](#complex-potential-of-a-two-dimensional-potential-flow)

For a [complex potential](#complex-potential-of-a-two-dimensional-potential-flow) $w(z)=m/(z-a)$, reflection in the straight wall through zero at angle $\theta$ is $Rz=e^{2i\theta}\bar z$. The image construction $W(z)=w(z)+\overline{w(Rz)}$ gives

$$
W(z)=\frac{m}{z-a}+\frac{e^{2i\theta}\bar m}{z-e^{2i\theta}\bar a}.
$$

On the wall $Rz=z$, this is real, so its [stream function](#stream-function) is constant there. This proves the [impermeability condition](viscous-fluid-flow.md#no-penetration-boundary-condition). Thus the image position is $a'=e^{2i\theta}\bar a$ and its moment is $m'=e^{2i\theta}\bar m$. If the point dipole is advected by the regular image flow, the [complex velocity](#complex-velocity) convention $W'=u-iv$ gives

$$
\frac{d\bar a}{dt}=-\frac{m'}{(a-a')^2}=\frac{\bar m}{4d^2},
$$

where $d=\operatorname{Im}(e^{-i\theta}a)$ is its signed distance from the wall. The last equality follows from $a-a'=2ie^{i\theta}d$. It applies when $d\ne0$.

#### Two-dimensional point sink

↑ **Parent:** [Complex potential of a two-dimensional potential flow](#complex-potential-of-a-two-dimensional-potential-flow)

A [two-dimensional point sink](#two-dimensional-point-sink) of strength $Q>0$ removes [volume flux](#volumetric-flow-rate) $Q$ per unit depth at $z_0$. Its [complex potential of a two-dimensional potential flow](#complex-potential-of-a-two-dimensional-potential-flow) is the displayed expression, so $u-iv=-Q/[2\pi(z-z_0)]$. The radial [velocity](classical-mechanics.md#velocity) is $u_r=-Q/(2\pi r)$: integrating over a circle gives outward flux $2\pi r u_r=-Q$. This is the planar cross-section of a [line sink](#line-sink). A passive particle satisfies $d(r^2)/dt=-Q/\pi$ and reaches the ideal point singularity in finite time. This is a flow singularity, distinct from a stable [sink equilibrium](dynamical-systems.md#sink-equilibrium) of a regular dynamical system.

#### Image-induced motion of a planar doublet

↑ **Parent:** [Complex potential of a two-dimensional potential flow](#complex-potential-of-a-two-dimensional-potential-flow)

For a [two-dimensional potential doublet](#two-dimensional-potential-doublet) of fixed complex strength $M$ outside a stationary circle of radius $a$, the [Milne-Thomson circle theorem](#milne-thomson-circle-theorem) gives the image contribution $\bar M z/(a^2-\bar b z)$. If the singularity is stipulated to follow the regular fluid [velocity](classical-mechanics.md#velocity) at its position, differentiating this term and using the [complex velocity](#complex-velocity) convention gives the displayed motion law. Thus $\operatorname{Im}(b\bar M)$ is constant: the trajectory is a straight line parallel to $M$. With $M=me^{i\alpha}$ and initial location $b_0>a$ real, its [polar coordinates](multivariable-calculus.md#polar-coordinates) satisfy $r\sin(\theta-\alpha)=-b_0\sin\alpha$. This statement assumes fixed orientation; the translational rule alone supplies no equation for orientation evolution.

#### Blasius force theorem

↑ **Parent:** [Complex potential of a two-dimensional potential flow](#complex-potential-of-a-two-dimensional-potential-flow)

For a steady two-dimensional [incompressible flow](#incompressible-flow) and [irrotational flow](vorticity.md#irrotational-flow) around an impermeable body, the displayed contour formula gives the [force](force.md) on the body per unit span. Here $W'=u-iv$ is the [complex velocity](#complex-velocity), $\rho$ is the constant [mass density](#density), and $C$ runs counterclockwise around the body, excluding other fluid singularities. To verify the sign, [Bernoulli's principle](euler-equations-for-an-inviscid-fluid.md#bernoulli-s-principle) gives $p=p_0-\rho|q|^2/2$. On a counterclockwise boundary, the complex pressure force is $d(X-iY)=-ip\,d\bar z$. Tangency gives $q\,dz=\bar q\,d\bar z$, and therefore $|q|^2d\bar z=q^2dz$. Integrating removes the constant $p_0$ term and gives the formula. The theorem is named after [Heinrich Blasius](physicist.md#paul-richard-heinrich-blasius).

##### Force on a cylinder from an external dipole

↑ **Parent:** [Blasius force theorem](#blasius-force-theorem)

The [Milne-Thomson circle theorem](#milne-thomson-circle-theorem) places an image dipole inside a [cylinder](geometry-and-topology.md#cylinder-geometry) at the inverse point of an external dipole. In the [residue](analysis.md#residue) of the squared [complex velocity](#complex-velocity), only the cross term between the analytic external [velocity](classical-mechanics.md#velocity) and the image [double pole](isolated-singularity.md#double-pole) contributes. The product of their conjugate dipole strengths is independent of orientation, so the [cylinder](geometry-and-topology.md#cylinder-geometry) force is radial toward the external dipole.

##### Blasius force from a Laurent coefficient at infinity

↑ **Parent:** [Blasius force theorem](#blasius-force-theorem)

For a two-dimensional steady ideal flow outside a body, let $q=w'$ be the [complex velocity](#complex-velocity). Suppose $q$ is holomorphic in the exterior and $q^2$ has a [Laurent series](analysis.md#laurent-series) near infinity, with coefficient $a_{-1}$ of $z^{-1}$. Orient the body contour counterclockwise and assume the usual impermeability and Bernoulli hypotheses of the [Blasius force theorem](#blasius-force-theorem). Deforming the contour to a large circle gives $\oint q^2dz=2\pi i a_{-1}$. Substitution in Blasius' formula proves $F_x-iF_y=-\pi\rho a_{-1}$.

In particular, $q(z)=q_\infty+O(z^{-2})$ makes the force zero: its square has no reciprocal term. This criterion handles branch-cut obstacles by applying the contour in their analytic exterior, rather than separately assigning forces to endpoint singularities.

##### Force on a circular cylinder from a held exterior vortex

↑ **Parent:** [Blasius force theorem](#blasius-force-theorem)

Place a held [point vortex](vorticity.md#line-vortex) of circulation $\Gamma$ at real position $b>a$ outside a circular cylinder $|z|=a$, and prescribe circulation $-\Gamma$ about the cylinder. An opposite image at $c=a^2/b$ gives [complex velocity](#complex-velocity) $q(z)=-i\Gamma(1/(z-b)-1/(z-c))/(2\pi)$. On the positively oriented cylinder contour, the only pole of $q^2$ inside is at $c$, with residue $-\Gamma^2/(2\pi^2(b-c))$. The [residue theorem](analysis.md#residue-theorem) and [Blasius force theorem](#blasius-force-theorem) give $F_x-iF_y=\rho\Gamma^2/(2\pi(b-c))$. Thus $F_y=0$ and $F_x=\rho\Gamma^2b/(2\pi(b^2-a^2))>0$: the force on the cylinder points toward the vortex. The specified cylinder circulation is part of the hypothesis; a zero-circulation cylinder has an additional central image term.

##### Blasius moment theorem

↑ **Parent:** [Blasius force theorem](#blasius-force-theorem)

For steady [incompressible flow](#incompressible-flow) and [irrotational flow](vorticity.md#irrotational-flow) of constant [mass density](#density), with no [body force](#body-force), this formula gives the [hydrodynamic torque](continuum-mechanics.md#hydrodynamic-torque) about the origin per unit span on an impermeable body. Orient its boundary counterclockwise, and let positive [torque](momentum.md#torque) be counterclockwise. The proof uses $M=\operatorname{Re}\oint_Cpz\,d\bar z$, the [Bernoulli equation](euler-equations-for-an-inviscid-fluid.md#bernoulli-equation) $p=P_*-\rho|w'|^2/2$, and the tangency identity $|w'|^2d\bar z=(w')^2dz$. The real part of the constant-pressure term vanishes because $\operatorname{Re}(z\,d\bar z)=d|z|^2/2$. The full complex integral of $z\,d\bar z$ need not vanish.

##### Force on a unit cylinder due to a uniform flow and an external source

↑ **Parent:** [Blasius force theorem](#blasius-force-theorem)

In a planar [potential flow](#potential-flow), superpose a positive-$x$ [uniform flow](#uniform-flow) of speed $U$ and a [line source](#line-source) of strength $Q=2\pi m$ at the real point $b>1$. Introduce an impermeable unit circular [cylinder](geometry-and-topology.md#cylinder-geometry) with zero [circulation](vorticity.md#circulation-physics). The [Milne-Thomson circle theorem](#milne-thomson-circle-theorem) gives the [complex potential of a two-dimensional potential flow](#complex-potential-of-a-two-dimensional-potential-flow)

$$
w=U(z+z^{-1})+m[\log(z-b)+\log(z-b^{-1})-\log z].
$$

The displayed horizontal [force per unit length](force.md#force-per-unit-length) acts on the [cylinder](geometry-and-topology.md#cylinder-geometry), and $F_y=0$ by [reflection symmetry](physics.md#reflection-symmetry). To prove it, let $q=w'$ be the [complex velocity](#complex-velocity). At infinity, $q=U+m/z+O(z^{-2})$, so the sum of all finite [residues](analysis.md#residue) of $q^2$ is $2Um$. At the external [pole](isolated-singularity.md#pole) $b$, write $q=m/(z-b)+H(z)$; then

$$
\operatorname{Res}_{b}q^2=2mH(b),\qquad
H(b)=U-\frac U{b^2}+\frac{m}{b(b^2-1)}.
$$

The [residue theorem](analysis.md#residue-theorem) and the counterclockwise [Blasius force theorem](#blasius-force-theorem) give $F_x-iF_y=2\pi\rho m[H(b)-U]$, proving the formula. With $m>0$ and $U>0$, its sign changes at $b=(m+\sqrt{m^2+4U^2})/(2U)$.

#### Milne-Thomson circle theorem

↑ **Parent:** [Complex potential of a two-dimensional potential flow](#complex-potential-of-a-two-dimensional-potential-flow)

The [Milne-Thomson circle theorem](#milne-thomson-circle-theorem) constructs a circular impermeable boundary in a two-dimensional [potential flow](#potential-flow). Suppose an incident [complex potential of a two-dimensional potential flow](#complex-potential-of-a-two-dimensional-potential-flow) $f$ is analytic on and inside $|z|=a$, with its physical singularities outside that disk. Then the displayed $W$ has constant [stream function](#stream-function) on $|z|=a$. The proof is the identity $a^2/\bar z=z$ on the circle: there $W=f(z)+\overline{f(z)}$ is real. Hence the circle is a [streamline](#streamline) and satisfies the [no-penetration boundary condition](viscous-fluid-flow.md#no-penetration-boundary-condition). The reflected term has its image singularities inside the obstacle. Additional imposed [circulation](vorticity.md#circulation-physics) must be specified separately. The theorem is named after [Louis Melville Milne-Thomson](mathematics.md#l-m-milne-thomson).

#### Two-dimensional potential doublet

↑ **Parent:** [Complex potential of a two-dimensional potential flow](#complex-potential-of-a-two-dimensional-potential-flow)

A [two-dimensional potential doublet](#two-dimensional-potential-doublet) is a localized [potential flow](#potential-flow) singularity with [complex potential of a two-dimensional potential flow](#complex-potential-of-a-two-dimensional-potential-flow) $W=M/(z-b)$, where $M=me^{i\alpha}$ specifies strength and orientation. It is the limiting field of an equal [point source](#point-source) and sink as their separation tends to zero with strength times separation fixed, with the sign absorbed in $M$. Its [complex velocity](#complex-velocity) is $-M/(z-b)^2$, so the [velocity](classical-mechanics.md#velocity) decays as inverse distance squared. The total [volumetric flow rate](#volumetric-flow-rate) around the singularity is zero. Its two-dimensional decay differs from that of the three-dimensional [source dipole](#source-dipole).

#### Complex velocity

↑ **Parent:** [Complex potential of a two-dimensional potential flow](#complex-potential-of-a-two-dimensional-potential-flow)

For a [complex potential of a two-dimensional potential flow](#complex-potential-of-a-two-dimensional-potential-flow) $W=\phi+i\psi$ in the coordinate $z=x+iy$, the [Cauchy-Riemann equations](analysis.md#cauchy-riemann-equations) give $W'=\phi_x-i\phi_y=u-iv$. A material point with physical [velocity](classical-mechanics.md#velocity) $(u,v)$ therefore satisfies $\dot z=\overline{W'(z)}$. Complex conjugation matters when deriving a [pathline](#pathline) from a [complex potential of a two-dimensional potential flow](#complex-potential-of-a-two-dimensional-potential-flow).

##### Hodograph plane

↑ **Parent:** [Complex velocity](#complex-velocity)

The hodograph plane records [velocity](classical-mechanics.md#velocity) rather than position. For a two-dimensional [potential flow](#potential-flow), the complex coordinate $q=u-iv$ is the [complex velocity](#complex-velocity). A straight impermeable wall fixes the [velocity](classical-mechanics.md#velocity) direction and hence maps to a radial line in this plane. A constant-[speed](classical-mechanics.md#speed) [free streamline](#free-streamline) maps to a circle centered at zero. Thus a free-[boundary](topology.md#boundary-of-a-set) problem in physical space can become a fixed geometric domain in [velocity](classical-mechanics.md#velocity) space. Recovering the physical map then uses $dz/dw=1/q(w)$, wherever $q$ is nonzero.

###### Exterior quarter-disc hodograph for a downward right-angle turn

↑ **Parent:** [Hodograph plane](#hodograph-plane)

A unit-speed free layer turning downward around a reentrant wall corner has [complex velocity](#complex-velocity) $q=u-iv$ in the first-quadrant exterior of the [unit disc](topology.md#unit-disc). Upstream $q=1$, downstream $q=i$, and the corner has infinite speed because its fluid angle is $3\pi/2$. Squaring $q$, applying $(s-1)/(s+1)$, and squaring again maps this domain to the [upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) with upstream, corner and downstream at $0,1,\infty$. The potential strip map $e^{\pi w}$ has the same normalization, proving the formula. The sign of the turn and the fluid corner angle determine whether the relevant hodograph is an exterior or interior quarter disc.

###### Half-contraction free streamline at a horizontal canal lip

↑ **Parent:** [Hodograph plane](#hodograph-plane)

A semi-infinite horizontal plate at unit height and a floor at zero give a [velocity potential](#velocity-potential) strip of height $a$ and an upper unit [semicircle](topology.md#semicircle) in the [complex velocity](#complex-velocity) $q$. Their matching [half-plane](geometry-and-topology.md#half-plane) maps give $(1+e^{\pi w/a})^{-1}=((q-1)/(q+1))^2$. Along the [fluid free boundary](#fluid-free-boundary) put $q=e^{-i\theta}$, $-\pi<\theta<0$. Then $dz/d\theta=-(a/\pi)e^{i\theta}\cot(\theta/2)$ and $y=1-(a/\pi)(\theta+\pi+\sin\theta)$. Its downstream limit is $1-a$, which must equal the downstream depth $a$. Thus the contraction is exactly one half.

###### Finite-reservoir-head draining free streamline

↑ **Parent:** [Hodograph plane](#hodograph-plane)

For a planar reservoir draining below a vertical lip of height one into a unit-speed stream, the potential strip $0<\operatorname{Im}w<a$ and first-quadrant unit velocity disk satisfy

$$
\frac1{1+e^{\pi w/a}}=\left(\frac{q^2-1}{q^2+1}\right)^2.
$$

On the [fluid free boundary](#fluid-free-boundary) put $q=e^{-i\theta}$, $-\pi/2\leq\theta<0$. Then $dz/d\theta=-2ae^{i\theta}\cot\theta/\pi$, so the downstream height is $1-2a/\pi$. Equating it to $a$ gives $a=\pi/(\pi+2)$.

###### Right-angle free-streamline hodograph map

↑ **Parent:** [Hodograph plane](#hodograph-plane)

For an inviscid irrotational unit-speed layer turning through a right angle, the [complex potential of a two-dimensional potential flow](#complex-potential-of-a-two-dimensional-potential-flow) occupies the strip $0<\operatorname{Im}w<1$ and its complex velocity $q$ occupies a fourth-quadrant quarter disk. The maps $r=q^2$, $s=(r-1)/(r+1)$ and $s^2$ take this disk to the upper half-plane, sending upstream velocity one, corner stagnation zero, and downstream velocity $-i$ to $0,1,\infty$. The map $e^{\pi w}$ has the same normalization, proving the displayed relation.

#### Logarithmic flow in a sine-mapped half-strip

↑ **Parent:** [Complex potential of a two-dimensional potential flow](#complex-potential-of-a-two-dimensional-potential-flow)

The [conformal map of a vertical half-strip by sine](geometry-and-topology.md#conformal-map-of-a-vertical-half-strip-by-sine) sends $-\pi/2<\operatorname{Re}z<\pi/2$, $\operatorname{Im}z>0$ to the [upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis). The [complex potential of a two-dimensional potential flow](#complex-potential-of-a-two-dimensional-potential-flow) $W(z)=\log(a+\sin z)$ therefore pulls back the radial logarithmic flow originating at $\zeta=-a$. Its complex velocity is $W'=\cos z/(a+\sin z)$, with a boundary singularity at $z=-\pi/2+i\operatorname{arcosh}a$. For $z=x+iy$, define $D=(a+\sin x\cosh y)^2+\cos^2x\sinh^2y$. Then

$$
u=\frac{\cos x(a\cosh y+\sin x)}D,\qquad v=\frac{\sinh y(\cosh y+a\sin x)}D.
$$

The bottom boundary carries rightward flow, the right boundary upward flow, and the left boundary flow away from the singular point. The velocity tends to $(0,1)$ at large height. The finite bottom corners are stagnation points, not singularities of $W$.

### Corner sink in a semi-infinite channel

↑ **Parent:** [Potential flow](#potential-flow)

For unit channel width, [incompressible flow](#incompressible-flow) towards a corner withdrawal point has $\psi=0$ on the lower wall and $\psi=-m$ on the upper and left walls, with $\psi\to-my$ far downstream. For [irrotational flow](vorticity.md#irrotational-flow), [separation of variables](partial-differential-equation.md#separation-of-variables) gives the displayed harmonic correction: the Fourier sine coefficients of $-m(1-y)$ are $-2m/(n\pi)$. Near the corner, $\psi\sim-2m\theta/\pi$ and radial velocity is $-2m/(\pi r)$, whose integrated inward flux across a quarter-circle is $m$.

### Rankine half-body

↑ **Parent:** [Potential flow](#potential-flow)

The region bounded by the dividing [streamlines](#streamline) of a two-dimensional [point source](#point-source) superposed on uniform flow. Its stagnation point is $-Q/(2\pi U)$ upstream and its far downstream width is $Q/U$. The boundary encloses fluid originating at the source rather than a rigid obstacle; the upstream stagnation point is reached only asymptotically by the upstream source trajectory.

### Radial source flow

↑ **Parent:** [Potential flow](#potential-flow)

A two-dimensional incompressible line source with area flux $Q$ has radial [velocity](classical-mechanics.md#velocity) $Q/(2\pi r)$, obtained from flux conservation around a circle. It is irrotational away from the source, with potential $(Q/(2\pi))\ln r$. For a circular expanding interface, $Q=2\pi aa_t$ and $u_r=aa_t/r$, whose radial strain is $-aa_t/r^2$. That strain supplies a normal viscous stress even though the [velocity](classical-mechanics.md#velocity) is a potential flow.

### Potential dipole

↑ **Parent:** [Potential flow](#potential-flow)

A potential dipole in three dimensions is the [potential flow](#potential-flow) $\mathbf u=\nabla\phi$ with $\phi=\mathbf d\cdot\mathbf x/r^3$. Away from the origin its potential is a [harmonic function](partial-differential-equation.md#harmonic-function), so it is also a constant-[pressure](pressure.md) [Stokes flow](stokes-flow.md). Its [velocity](classical-mechanics.md#velocity) decays as $r^{-3}$ and its [vorticity](vorticity.md) is zero. It is distinct from a [stresslet](stokes-flow.md#force-dipole-flow), whose leading [velocity](classical-mechanics.md#velocity) decays as $r^{-2}$.

### Point source

↑ **Parent:** [Potential flow](#potential-flow)

A two-dimensional point source of strength $q$ has velocity potential $\phi=q\log r/(2\pi)$ and outward velocity $q\mathbf e_r/(2\pi r)$. Every closed contour enclosing it has volume flux $q$.

#### Line sink

↑ **Parent:** [Point source](#point-source)

A [line sink](#line-sink) is a planar [line source](#line-source) with negative [volume flux](#volumetric-flow-rate): fluid moves radially inward towards its location. For withdrawal rate $S>0$, its [complex potential of a two-dimensional potential flow](#complex-potential-of-a-two-dimensional-potential-flow) is $-S\log(z-b)/(2\pi)$.

#### Line source

↑ **Parent:** [Point source](#point-source)

In a planar [incompressible flow](#incompressible-flow), a [line source](#line-source) injects [volume flux](#volumetric-flow-rate) $Q$ per unit length perpendicular to the plane. Its radial [velocity](classical-mechanics.md#velocity) is $u_r=Q/(2\pi r)$, since integrating the outward [velocity](classical-mechanics.md#velocity) around a [circle](topology.md#circle) gives $2\pi r u_r=Q$. Its [complex potential of a two-dimensional potential flow](#complex-potential-of-a-two-dimensional-potential-flow) is $w=Q\log(z-b)/(2\pi)$ and its [complex velocity](#complex-velocity) is $w'=Q/[2\pi(z-b)]$. Here $Q>0$ means outward flow; a [line sink](#line-sink) has negative $Q$. Away from $b$, this is an [irrotational flow](vorticity.md#irrotational-flow) as well as an [incompressible flow](#incompressible-flow).

##### Hydrodynamic attraction of a wall to a line source

↑ **Parent:** [Line source](#line-source)

In the upper [half-plane](geometry-and-topology.md#half-plane), a [line source](#line-source) of outward [volume flux](#volumetric-flow-rate) $Q$ at height $a$ above an impermeable wall has an equal image source below it. On the wall $u=Qx/[\pi(x^2+a^2)]$ and the normal [velocity](classical-mechanics.md#velocity) vanishes. The steady [Bernoulli equation](euler-equations-for-an-inviscid-fluid.md#bernoulli-equation) gives $p-p_\infty=-\rho Q^2x^2/[2\pi^2(x^2+a^2)^2]$. Since

$$
\int_{-\infty}^{\infty}\frac{x^2}{(x^2+a^2)^2}\,dx=\frac\pi{2a},
$$

the ambient-relative [force per unit length](force.md#force-per-unit-length) pulls the wall toward the source with the displayed magnitude. The [torque](momentum.md#torque) about the source's projection onto the wall is zero in the symmetric [Cauchy principal value](complex-analysis.md#cauchy-principal-value) sense. Individual one-sided moments diverge logarithmically. This planar result differs from the three-dimensional [hydrodynamic attraction of a plane wall to a point source](#hydrodynamic-attraction-of-a-plane-wall-to-a-point-source).

##### Line source in a closed-end semi-infinite strip

↑ **Parent:** [Line source](#line-source)

In the impermeable strip $x>0$, $0<y<a$, a [line source](#line-source) of strength $Q$ at an interior point $c$ has the displayed [complex potential of a two-dimensional potential flow](#complex-potential-of-a-two-dimensional-potential-flow), with locally consistent [complex logarithm](analysis.md#complex-logarithm) and $f(z)=\cosh(\pi z/a)$. The [hyperbolic-cosine map of a half-strip](geometry-and-topology.md#hyperbolic-cosine-map-of-a-half-strip) sends the walls to the [real axis](complex-analysis.md#real-axis). An equal image [line source](#line-source) at $\overline{f(c)}$ makes that axis a [streamline](#streamline). Since $f'(c)\ne0$, the local singular part remains $Q\log(z-c)/(2\pi)$, proving preservation of strength. With no extra imposed flow, the [complex velocity](#complex-velocity) tends to $Q/a$ as $x\to\infty$, so the outgoing [volume flux](#volumetric-flow-rate) is $Q$. The source position $c$ has positive imaginary part; assuming it real would place it on a wall.

#### Source dipole

↑ **Parent:** [Point source](#point-source)

A source dipole is the limit of an equal source and sink brought together with their source-strength times separation vector fixed at $\mathbf M$. Differentiating the [three-dimensional point source](#three-dimensional-point-source) field gives $\mathbf u=-(\mathbf M\cdot\nabla)[\mathbf r/(4\pi r^3)]$. It has [velocity potential](#velocity-potential) $-\mathbf M\cdot\mathbf r/(4\pi r^3)$, zero total [volume flux](#volumetric-flow-rate), and $r^{-3}$ far-field decay. Unlike a [stresslet](stokes-flow.md#force-dipole-flow), it is an irrotational potential singularity rather than a [force-dipole flow](stokes-flow.md#force-dipole-flow).

#### Three-dimensional point source

↑ **Parent:** [Point source](#point-source)

A point injection of volume at rate $Q$ produces the displayed radial [potential flow](#potential-flow) in three dimensions. Its [velocity potential](#velocity-potential) is $-Q/(4\pi r)$, and every enclosing [sphere](euclidean-geometry.md#sphere) has outward [volume flux](#volumetric-flow-rate) $Q$. The [divergence](multivariable-calculus.md#divergence) vanishes away from the source and is $Q$ times the three-dimensional [Dirac delta](distribution-theory.md#dirac-delta-function) distribution at it. The field is also a [Stokes flow](stokes-flow.md) with constant [pressure](pressure.md) away from its singularity.

#### Hydrodynamic attraction of a plane wall to a point source

↑ **Parent:** [Point source](#point-source)

An incompressible [point source](#point-source) of volume [flux](mathematical-physics.md#flux) $Q$ at height $a$ above an impermeable plane has [velocity potential](#velocity-potential) $\phi=-Q(1/r_++1/r_-)/(4\pi)$, with an equal image source below the plane. On the wall, $u_s=Qs/[2\pi(s^2+a^2)^{3/2}]$. The [Bernoulli equation](euler-equations-for-an-inviscid-fluid.md#bernoulli-equation) gives $p-p_\infty=-\rho Q^2s^2/[8\pi^2(s^2+a^2)^3]$. Integrating the [pressure](pressure.md) deficit over the plane gives the displayed attraction force relative to ambient [pressure](pressure.md). If source strength instead denotes the coefficient $Q/(4\pi)$ of radial inverse-square velocity, the force is $\pi\rho m^2/a^2$.

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

#### Pressure field of a pulsating sphere

↑ **Parent:** [Spherically symmetric incompressible radial flow](#spherically-symmetric-incompressible-radial-flow)

In an unbounded [incompressible flow](#incompressible-flow) with [spherical symmetry](geometry-and-topology.md#spherical-symmetry), the [kinematic boundary condition](#kinematic-boundary-condition) on a sphere of radius $R(t)$ gives $u_r=R^2\dot R/r^2$ and [velocity potential](#velocity-potential) $\phi=G(t)-R^2\dot R/r$. The [Unsteady Bernoulli equation](euler-equations-for-an-inviscid-fluid.md#unsteady-bernoulli-equation) at infinity has $F(t)=\dot G+p_\infty/\rho$. Subtracting it from the finite-radius equation gives the displayed [pressure](pressure.md), independently of $G$. Time differentiation is at fixed $r$. Evaluating at $r=R(t)$ yields the [Rayleigh equation for an inviscid spherical bubble](#rayleigh-equation-for-an-inviscid-spherical-bubble) when the boundary [pressure](pressure.md) is prescribed.

#### Rayleigh equation for an inviscid spherical bubble

↑ **Parent:** [Spherically symmetric incompressible radial flow](#spherically-symmetric-incompressible-radial-flow)

In radial [potential flow](#potential-flow) outside a spherical bubble, [incompressibility](#incompressible-flow) and the moving-boundary condition give $u_r=R^2\dot R/r^2$ and $\phi=-R^2\dot R/r$. The [Unsteady Bernoulli equation](euler-equations-for-an-inviscid-fluid.md#unsteady-bernoulli-equation), with its gauge fixed at infinity, yields the displayed radius equation when surface tension and viscosity are neglected. Pressure continuity at the interface identifies the liquid pressure with the gas pressure $p_g$. The vacuum special case is [Rayleigh collapse of a spherical cavity](#rayleigh-collapse-of-a-spherical-cavity).

##### Pressure-work energy balance for a spherical bubble

↑ **Parent:** [Rayleigh equation for an inviscid spherical bubble](#rayleigh-equation-for-an-inviscid-spherical-bubble)

For spherical expansion in an unbounded [incompressible flow](#incompressible-flow), continuity gives $u_r=R^2\dot R/r^2$. Integrating the [kinetic energy](energy.md#kinetic-energy) outside the bubble gives $K=2\pi\rho R^3\dot R^2$. The [Rayleigh equation for an inviscid spherical bubble](#rayleigh-equation-for-an-inviscid-spherical-bubble) then yields $\dot K=(p_b-p_\infty)\dot V$, where $V=4\pi R^3/3$. With $p_b=p_\infty V_0/V$ and constant $p_\infty$, integration gives $K-K_0=p_\infty[V_0\log(V/V_0)-V+V_0]$. This neglects [viscosity](dynamic-viscosity.md), [surface tension](surface-tension.md) and external body-force differences, which contribute additional terms in other bubble models.

##### First integral of polytropic spherical-bubble motion

↑ **Parent:** [Rayleigh equation for an inviscid spherical bubble](#rayleigh-equation-for-an-inviscid-spherical-bubble)

For gas pressure depending only on radius and initial speed zero, multiplying the [Rayleigh equation for an inviscid spherical bubble](#rayleigh-equation-for-an-inviscid-spherical-bubble) by $2R^2\dot R$ integrates to the displayed identity. A polytropic pressure $p_g=K/R^{3\kappa}$ gives elementary power integrals when $\kappa\ne1$, and a logarithm when $\kappa=1$. Turning radii are the positive zeros of this first integral. At $\kappa=2$ and $p_g(R_0)=p_\infty/2$, they are $R_0$ and $R_0/2^{1/3}$; the inward and outward accelerations at them have opposite signs, giving bounded undamped oscillation in the [ideal](commutative-algebra.md#ideal) model.

#### Rayleigh-Plesset equation

↑ **Parent:** [Spherically symmetric incompressible radial flow](#spherically-symmetric-incompressible-radial-flow)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rayleigh–Plesset_equation)

The [Rayleigh-Plesset equation](#rayleigh-plesset-equation) balances the radial inertia of an incompressible liquid around a spherical bubble against internal and ambient [pressure](pressure.md), [surface tension](surface-tension.md) and [viscous stress](dynamic-viscosity.md#viscous-stress-tensor). Removing the last two effects and setting the bubble pressure to zero gives the following vacuum-collapse case.

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

###### Collapse time of a spherical cavity

↑ **Parent:** [Rayleigh collapse of a spherical cavity](#rayleigh-collapse-of-a-spherical-cavity)

For a spherical vacuum cavity initially at rest with radius $a$, in an inviscid liquid of constant [mass density](#density) $\rho$ and positive constant far-field [pressure](pressure.md) $p_\infty$, the [Rayleigh equation for an inviscid spherical bubble](#rayleigh-equation-for-an-inviscid-spherical-bubble) has the [first integral](differential-equation.md#first-integral) $R^3\dot R^2=2p_\infty(a^3-R^3)/(3\rho)$. To obtain it, multiply the radius equation by $2R^2\dot R$ and integrate the resulting exact derivative. Choosing the negative square root and integrating $dt=dR/\dot R$ gives

$$
k=\sqrt{\frac32}\int_0^1\frac{s^{3/2}}{\sqrt{1-s^3}}\,ds.
$$

This [improper integral](real-analysis.md#improper-integral) converges at both endpoints, proving finite-time [Rayleigh collapse of a spherical cavity](#rayleigh-collapse-of-a-spherical-cavity) in the ideal model. It has numerical value approximately $0.914681$. The prediction neglects [viscosity](dynamic-viscosity.md), [surface tension](surface-tension.md) and liquid compressibility.

### Squeezing wedge flow

↑ **Parent:** [Potential flow](#potential-flow)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Squeezing_wedge_flow)

Inviscid flow between closing hinged plates is a quadratic potential flow that expels fluid radially.

## Free surface

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Free_surface)

A free surface is a fluid boundary whose position is part of the solution and whose traction is prescribed by the adjoining medium. Its motion obeys a [kinematic boundary condition](#kinematic-boundary-condition), while its pressure or stress supplies a dynamic boundary condition.

### Surface elevation

↑ **Parent:** [Free surface](#free-surface)

The [surface elevation](#surface-elevation) is the signed height of a [free surface](#free-surface) relative to a chosen reference level, commonly its undisturbed position. With upward coordinate $z$, the surface is the graph $z=\eta(x,y,t)$. Its evolution obeys the [kinematic boundary condition for a free-surface graph](#kinematic-boundary-condition-for-a-free-surface-graph).

### Surface gravity wave

↑ **Parent:** [Free surface](#free-surface)

A surface gravity wave is a free-surface oscillation restored by gravity. In inviscid deep water its angular frequency and horizontal wavenumber satisfy $\omega^2=gk$.

#### Hydrostatic lower bound for a travelling-pressure response

↑ **Parent:** [Surface gravity wave](#surface-gravity-wave)

For the subcritical [travelling-pressure response of finite-depth surface gravity waves](#travelling-pressure-response-of-finite-depth-surface-gravity-waves), put $c_*^2=g\tanh(kh)/k$. When $0\leq c<c_*$, the [amplitude](wave.md#wave-amplitude) is

$$
a(c)=\frac{p_1}{\rho g}\frac1{1-(c/c_*)^2}\geq\frac{p_1}{\rho g}.
$$

The inequality follows immediately because the denominator belongs to $(0,1]$. Equality holds precisely at $c=0$, where [hydrostatic equilibrium](statistical-physics.md#hydrostatic-equilibrium) gives $\rho g\eta=-p_1\cos(kx)$. If only strictly positive $c$ is allowed, $p_1/(\rho g)$ is the [infimum](real-analysis.md#infimum), approached as $c\downarrow0$, and is not an attained [minimum](set.md#minimum-of-a-subset-of-a-total-order). This bound applies to the travelling forced component, rather than an arbitrary superposition with free [surface gravity waves](#surface-gravity-wave).

#### Travelling-pressure response of finite-depth surface gravity waves

↑ **Parent:** [Surface gravity wave](#surface-gravity-wave)

For an [inviscid flow](#inviscid-flow) of constant [mass density](#density) $\rho$ and depth $h$, impose excess [pressure](pressure.md) $p_1\cos(k(x-ct))$ with $k>0$ on a [free surface](#free-surface). Neglect [surface tension](surface-tension.md). A travelling solution of the [linearized free-surface boundary conditions](#linearized-free-surface-boundary-conditions) is

$$
\eta=A\cos(k(x-ct)),\qquad
\phi=\frac{Ac}{\sinh(kh)}\cosh(k(y+h))\sin(k(x-ct)).
$$

The [velocity potential](#velocity-potential) satisfies the [Laplace equation](partial-differential-equation.md#laplace-equation) and the bed [no-penetration boundary condition](viscous-fluid-flow.md#no-penetration-boundary-condition). Its surface [time derivative](multivariable-calculus.md#time-derivative) is $-Ac^2k\coth(kh)\cos(k(x-ct))$, so the dynamic condition gives the displayed signed response. The nonnegative [amplitude](wave.md#wave-amplitude) is $|A|$. It is finite except at

$$
c_*^2=\frac{g\tanh(kh)}k,
$$

the squared [phase speed](dispersion-relation.md#phase-speed) of a free [surface gravity wave](#surface-gravity-wave) at that [wavenumber](wave-equation.md#wavenumber). Equality produces [resonance](dynamical-systems.md#resonance). This describes a travelling forced component; free [surface gravity waves](#surface-gravity-wave) must be added to meet general [initial conditions](differential-equation.md#initial-condition). At exact [resonance](dynamical-systems.md#resonance), a solution of the [initial value problem](differential-equation.md#initial-value-problem) generally grows with time rather than having a bounded periodic [amplitude](wave.md#wave-amplitude).

#### Surface-wave breaking

↑ **Parent:** [Surface gravity wave](#surface-gravity-wave)

A [surface gravity wave](#surface-gravity-wave) breaks when its smooth free-surface motion becomes unstable and overturns or forms a strongly dissipative front. In the nondispersive [shallow-water approximation](mathematical-physics.md#shallow-water-approximation), intersecting compressive [characteristic curves](transport-equation.md#characteristic-curve) signal failure of a smooth [simple wave](compressible-flow.md#simple-wave); a [hydraulic bore](mathematical-physics.md#hydraulic-bore) replaces it at the integral-model level. Dispersion can instead produce an oscillatory bore, while physical breaking involves turbulence and energy loss beyond the inviscid equations.

#### Normal modes of surface gravity waves in a rectangular tank

↑ **Parent:** [Surface gravity wave](#surface-gravity-wave)

For a tank with side lengths $a,b$, depth $h$, impermeable walls and negligible [surface tension](surface-tension.md), the small-amplitude [surface gravity wave](#surface-gravity-wave) [normal modes](wave-equation.md#normal-mode) have horizontal factors $\cos(m\pi x/a)\cos(n\pi y/b)$ and $k_{mn}^2=(m\pi/a)^2+(n\pi/b)^2$. The [velocity potential](#velocity-potential) has vertical factor $\cosh(k_{mn}(z+h))$, satisfying the bottom [Neumann boundary condition](differential-equation.md#neumann-boundary-condition). Combining the [linearized free-surface boundary conditions](#linearized-free-surface-boundary-conditions) gives $\omega_{mn}^2=gk_{mn}\tanh(k_{mn}h)$. The uniform $m=n=0$ [surface elevation](#surface-elevation) is excluded when the total water volume is fixed. Taking one horizontal index zero gives the two-dimensional tank modes.

For $k_{mn}h\ll1$, the [shallow-water approximation](mathematical-physics.md#shallow-water-approximation) gives $\omega_{mn}\sim\sqrt{gh}\,k_{mn}$; for $k_{mn}h\gg1$, the [deep-water gravity wave](#deep-water-gravity-wave) relation $\omega_{mn}^2\sim gk_{mn}$ follows. An [oscillating-wall forcing of a rectangular tank](#oscillating-wall-forcing-of-a-rectangular-tank) couples to these same [normal modes](wave-equation.md#normal-mode) and becomes resonant at their natural frequencies.

##### Oscillating-wall forcing of a rectangular tank

↑ **Parent:** [Normal modes of surface gravity waves in a rectangular tank](#normal-modes-of-surface-gravity-waves-in-a-rectangular-tank)

For a tank $0<x<L$, $-h<z<0$, let the left wall move by $\operatorname{Re}(ce^{-i\omega t})$ with small [amplitude](wave.md#wave-amplitude), while the right wall and bottom remain fixed. A periodic [velocity potential](#velocity-potential) $\operatorname{Re}(f e^{-i\omega t})$ has $f_x(0,z)=-i\omega c$. Add the [harmonic function](partial-differential-equation.md#harmonic-function)

$$
Q(x,z)=\frac{i\omega c}{2L}[(z+h)^2-(L-x)^2]
$$

to obtain $G=f+Q$ with homogeneous wall and bottom [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition). Thus $G=a_0/2+\sum_{n\geq1}a_n\cos(k_nx)\cosh(k_n(z+h))$, where $k_n=n\pi/L$. The [linearized free-surface boundary conditions](#linearized-free-surface-boundary-conditions) give $G_z-\lambda G=H$ at $z=0$, with $\lambda=\omega^2/g$ and

$$
H(x)=\frac{i\omega c}{L}\left[h-\frac\lambda2(h^2-(L-x)^2)\right].
$$

Its [Fourier cosine coefficients](fourier-series.md#fourier-cosine-coefficient) $H_n=(2/L)\int_0^L H(x)\cos(k_nx)dx$ give the title expression for $n\geq1$ and $a_0=-H_0/\lambda$. In particular $H_n=2i\omega c\lambda/(Lk_n^2)$ for $n\geq1$. The denominator vanishes at the corresponding [normal modes of surface gravity waves in a rectangular tank](#normal-modes-of-surface-gravity-waves-in-a-rectangular-tank), giving [resonance](dynamical-systems.md#resonance). Exact undamped resonance produces secular growth instead of a bounded periodic response. Free transients do not generally decay in this inviscid model.

#### Power-law near-shore ray asymptotics

↑ **Parent:** [Surface gravity wave](#surface-gravity-wave)

For depth $h=\alpha x^p$ with $p>0$, stationary [surface gravity waves](#surface-gravity-wave) conserve frequency $\omega$ and alongshore wavenumber $K$. Near shore their dispersion becomes $\omega^2\sim g\kappa^2h$, so $\kappa\sim\omega x^{-p/2}/\sqrt{g\alpha}$. The shoreward ray has $y'\sim-K\sqrt{g\alpha}x^{p/2}/\omega$, giving the displayed integrated scaling. Rays approach normally, while equal-phase crests approach parallel to the shore and their shore-normal spacing shrinks as $x^{p/2}$. These are asymptotics within the ray approximation; for $p<2$, its slow-variation assumption eventually fails arbitrarily close to the endpoint.

#### Wave fetch

↑ **Parent:** [Surface gravity wave](#surface-gravity-wave)

Wave fetch is the distance over which wind acts on an uninterrupted water surface to generate waves. Growth also depends on wind speed and duration. A [polynya](geophysics.md#polynya) can provide a local fetch inside otherwise extensive [sea ice](geophysics.md#sea-ice).

#### Radiation stress

↑ **Parent:** [Surface gravity wave](#surface-gravity-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radiation_stress)

The excess depth-integrated, time-averaged [momentum flux](mathematical-physics.md#momentum-flux) of a [surface gravity wave](#surface-gravity-wave) is its radiation stress. In deep water $c_g/c_p=1/2$, so $S_{xx}=\mathcal E/2=\rho_wga^2/4$. The force per transverse width on a reflecting object is the incident plus reflected minus transmitted radiation stress. Reflection increases force because the reflected wave carries momentum in the opposite direction.

#### Surface-gravity-wave energy

↑ **Parent:** [Surface gravity wave](#surface-gravity-wave)

A linear [deep-water gravity wave](#deep-water-gravity-wave) of surface-displacement amplitude $a$ has equal mean [kinetic energy](energy.md#kinetic-energy) and [potential energy](energy.md#potential-energy), and total mean [energy](energy.md) per horizontal area $\mathcal E=\rho_wga^2/2$. Its energy transport speed is the [group velocity](dispersion-relation.md#group-velocity). This amplitude is half the crest-to-trough height.

#### Wave steepness

↑ **Parent:** [Surface gravity wave](#surface-gravity-wave)

The dimensionless product of surface-wave amplitude and [wavenumber](wave-equation.md#wavenumber), $ka$, measures orbital displacement relative to the wavelength. Small [wave steepness](#wave-steepness) permits a [Taylor expansion](calculus.md#taylor-expansion) of the velocity sampled by moving parcels. For a [deep-water gravity wave](#deep-water-gravity-wave), orbital amplitudes and the local steepness decrease exponentially with depth.

#### Airy wave theory

↑ **Parent:** [Surface gravity wave](#surface-gravity-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Airy_wave_theory)

[Airy wave theory](#airy-wave-theory) linearizes the motion of small-amplitude [surface gravity waves](#surface-gravity-wave) in an inviscid, incompressible, irrotational fluid. At depth $h$, its dispersion relation is $\omega^2=gk\tanh(kh)$; deep water is the limit $kh\to\infty$.

##### Surface gravity wave forced by a traveling bottom

↑ **Parent:** [Airy wave theory](#airy-wave-theory)

Consider fluid at rest with mean depth $d$ and a bottom displacement $a\sin(k(x-ct))$. The [linearized free-surface boundary conditions](#linearized-free-surface-boundary-conditions) at $y=0$ and moving-bottom [kinematic boundary condition](#kinematic-boundary-condition) at $y=-d$ give a periodic particular response $\eta=b\sin(k(x-ct))$ and [velocity potential](#velocity-potential)

$$
\phi=-\frac b{kc}[g\cosh(ky)+kc^2\sinh(ky)]\cos(k(x-ct)).
$$

The bottom derivative fixes the signed response coefficient to the title formula. Here $k>0$, $c\ne0$, and the forcing must avoid $k^2c^2=gk\tanh(kd)$. This equality is [resonance](dynamical-systems.md#resonance) with the natural finite-depth [surface gravity wave](#surface-gravity-wave); nonzero undamped resonant forcing has no bounded periodic solution. The response reverses phase below resonance. General initial data can add free [surface gravity waves](#surface-gravity-wave), which do not decay in this inviscid model. Near resonance the resulting [wave steepness](#wave-steepness) and particle excursions, rather than the bottom displacement alone, determine whether the [linearization](algebra.md#linearization) remains valid.

###### Linearized particle orbits of a bottom-forced gravity wave

↑ **Parent:** [Surface gravity wave forced by a traveling bottom](#surface-gravity-wave-forced-by-a-traveling-bottom)

For a [bottom-forced gravity wave](#surface-gravity-wave-forced-by-a-traveling-bottom) with signed surface coefficient $b$, evaluate the first-order [velocity field](#velocity-field) at a parcel's mean position $(\bar x,\bar y)$ and integrate, with $\Theta=k(\bar x-ct)$. The horizontal and vertical displacement coefficients are

$$
A=b\left[\frac g{kc^2}\cosh(k\bar y)+\sinh(k\bar y)\right],\qquad
B=b\left[\frac g{kc^2}\sinh(k\bar y)+\cosh(k\bar y)\right].
$$

Thus the [pathline](#pathline) is an [ellipse](euclidean-geometry.md#ellipse) with horizontal and vertical semiaxes $|A|,|B|$ whenever both are nonzero, and a line segment if one vanishes. The identity $A^2-B^2=b^2[(g/(kc^2))^2-1]$ determines which axis is longer. Also $B(0)=b$ and $B(-d)=a$, verifying the surface and bottom displacements. Closed first-order orbits do not rule out a higher-order mean drift.

##### Deep-water gravity wave

↑ **Parent:** [Airy wave theory](#airy-wave-theory)

A small-amplitude deep-water wave with surface elevation $\eta=Ae^{i(kx-\omega t)}$ has dispersion relation $\omega^2=gk$ and a velocity potential that decays as $e^{kz}$ below the surface.

###### Wavenumber selection by a moving observer of deep-water waves

↑ **Parent:** [Deep-water gravity wave](#deep-water-gravity-wave)

A deep-water [gravity wave](gravity-wave.md) has dispersion $\omega(k)=\sqrt{g|k|}$. An observer moving with nonzero speed $V$ samples Fourier phases $kV\pm\omega(k)$. The [stationary phase method](analysis.md#stationary-phase-method) selects the points where their [derivatives](calculus.md#derivative) vanish, which gives the displayed wavenumbers. Their [group velocity](dispersion-relation.md#group-velocity) matches the observer's [velocity](classical-mechanics.md#velocity). For real even initial displacement with a nonzero Fourier coefficient there, the resulting signal has leading size $t^{-1/2}$ and phase $gt/(4|V|)-\pi/4$. If the initial coefficient vanishes, that leading term is absent; a stationary observer does not select a finite nonzero [wavenumber](wave-equation.md#wavenumber) by this rule.

###### Deep-water swell distance from period-dependent arrival times

↑ **Parent:** [Deep-water gravity wave](#deep-water-gravity-wave)

For two wave periods emitted together at one location, deep-water [group velocity](dispersion-relation.md#group-velocity) is $gT/(4\pi)$. A distant observer sees the shorter period $T_2<T_1$ later, with $\Delta t=(4\pi D/g)(1/T_2-1/T_1)$. This yields the displayed range estimate. Different emission times, a moving storm, finite-depth dispersion, currents and refraction are possible confounders; the propagation calculation alone does not establish a unique source range without these assumptions.

###### Energy of a deep-water standing gravity wave

↑ **Parent:** [Deep-water gravity wave](#deep-water-gravity-wave)

For elevation $h_0\sin(\omega t)\sin(kx)$, depth-integrated [kinetic energy](energy.md#kinetic-energy) per surface [area](differential-geometry.md#surface-area) is $\rho h_0^2\omega^2\cos^2(\omega t)/(4k)$. Wavelength-averaged excess gravitational [energy](energy.md) is $\rho gh_0^2\sin^2(\omega t)/4$. Conservation gives $\omega^2=gk$ in the inviscid gravity-only model.

###### Dispersive swell source inversion

↑ **Parent:** [Deep-water gravity wave](#deep-water-gravity-wave)

For an impulsive distant source of [deep-water gravity waves](#deep-water-gravity-wave), a component of period $T$ travels at [group velocity](dispersion-relation.md#group-velocity) $gT/(4\pi)$. Its arrival at distance $L$ obeys the displayed law, so inverse period increases linearly with arrival time. Two arrivals determine both $L$ and $t_0$. Finite source duration, currents, refraction and passage through [sea ice](geophysics.md#sea-ice) can invalidate the simple inversion.

###### Viscous decay of a deep-water gravity wave

↑ **Parent:** [Deep-water gravity wave](#deep-water-gravity-wave)

For small kinematic viscosity $\nu$, the mean viscous dissipation per unit horizontal area is $2\rho\nu gk^2|A|^2$. Since the mean wave energy is $\rho g|A|^2/2$, the amplitude obeys

$$
\frac{d|A|}{dt}=-2\nu k^2|A|,
\qquad
|A(t)|=|A(0)|e^{-2\nu k^2t}.
$$

#### Linearized free-surface boundary conditions

↑ **Parent:** [Surface gravity wave](#surface-gravity-wave)

For a small-amplitude [surface gravity wave](#surface-gravity-wave) described by [velocity potential](#velocity-potential) $\phi$ and [surface elevation](#surface-elevation) $\eta$, linearizing the [kinematic boundary condition for a free-surface graph](#kinematic-boundary-condition-for-a-free-surface-graph) and the [Bernoulli equation](euler-equations-for-an-inviscid-fluid.md#bernoulli-equation) at the mean surface $z=0$ gives

$$
\eta_t=\phi_z,
\qquad
\phi_t+g\eta=-\frac{p}{\rho}
\qquad(z=0).
$$

Here $p$ is the applied excess [pressure](pressure.md) above constant atmospheric pressure. With $p=0$, differentiate the second equation in time and use the first to obtain $\phi_{tt}+g\phi_z=0$. These surface conditions apply at finite depth as well as in the [deep-water gravity wave](#deep-water-gravity-wave) limit; depth enters through the bottom condition. The quadratic [kinetic energy](energy.md#kinetic-energy) term is omitted at this order, and [surface tension](surface-tension.md) is neglected.

##### Rectangular standing surface-gravity mode

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

### Axisymmetric stagnation strain

↑ **Parent:** [Stagnation point](#stagnation-point)

A regular axisymmetric [irrotational flow](vorticity.md#irrotational-flow) near a stagnation point on an impermeable tangent plane has equal tangential strain rates. The [incompressibility condition](#incompressible-flow) forces the normal rate to be their negative double. Thus the leading [velocity potential](#velocity-potential) has the displayed quadratic form. Its streamline invariants are the azimuth and $z(x^2+y^2)$; for incoming flow from positive $z$, $W>0$.

## Incompressible flow

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Incompressible_flow)

An [incompressible flow](#incompressible-flow) preserves the [volume](geometry-and-topology.md#volume) of each moving [fluid element](continuum-mechanics.md#fluid-element). Its local condition is zero [velocity divergence](continuum-mechanics.md#velocity-divergence), $\nabla\cdot\mathbf u=0$. Combined with [mass conservation](continuum-mechanics.md#mass-conservation), it says that each parcel's [mass density](#density) stays unchanged as it moves. This does not require every parcel to have the same [mass density](#density): an initially nonuniform distribution can be transported without compression. Nor does [incompressibility](#incompressible-flow) require a constant [velocity](classical-mechanics.md#velocity) or constant [pressure](pressure.md).

For positive [mass density](#density), the [continuity equation](mathematical-physics.md#continuity-equation) makes the equivalence precise:

$$
\frac{\partial\rho}{\partial t}+\nabla\cdot(\rho\mathbf u)=0,
\qquad
\frac{D\rho}{Dt}+\rho\nabla\cdot\mathbf u=0,
\qquad
\frac{D}{Dt}=\frac{\partial}{\partial t}+\mathbf u\cdot\nabla.
$$

The [material derivative](continuum-mechanics.md#material-derivative) follows a [fluid element](continuum-mechanics.md#fluid-element). Thus $D\rho/Dt=0$ if and only if the [velocity field](#velocity-field) is a [divergence-free vector field](#divergence-free-vector-field). The distinction between following a parcel and observing a fixed position prevents confusing [incompressibility](#incompressible-flow) with an unchanging [density](#density) field. [UCL, Conservation law derivations, sections 30.1–30.2](https://uclnatsci.github.io/2021/Electromagnetism-Fluids-and-Waves/fluids/conservation.html)

For a rigid pipe with impermeable walls, no leaks and [steady flow](#steady-flow), [mass conservation](continuum-mechanics.md#mass-conservation) at constant [mass density](#density) implies a constant [volumetric flow rate](#volumetric-flow-rate):

$$
Q=\int_A\mathbf u\cdot\mathbf n\,dA=A\overline U,
\qquad A_1\overline U_1=A_2\overline U_2.
$$

Here $\mathbf n$ points downstream, $A$ is the section's [area](differential-geometry.md#surface-area) and $\overline U$ is the mean normal [velocity](classical-mechanics.md#velocity), not necessarily the centreline speed. No assumption of [inviscid flow](#inviscid-flow) or a uniform [velocity profile](viscous-fluid-flow.md#velocity-profile) is needed. If unequal amounts entered and left a fixed segment, its [mass](classical-mechanics.md#mass) would accumulate, contradicting [steady flow](#steady-flow).

For a worked example, take horizontal water flow with stipulated [mass density](#density) $1000\,\mathrm{kg\,m^{-3}}$, inlet radius $R_1=0.010\,\mathrm m$, outlet radius $R_2=0.005\,\mathrm m$ and inlet mean [velocity](classical-mechanics.md#velocity) $\overline U_1=0.20\,\mathrm{m\,s^{-1}}$. The circular [areas](differential-geometry.md#surface-area) give

$$
Q=\pi R_1^2\overline U_1=2\pi\times10^{-5}\,\mathrm{m^3\,s^{-1}},
\qquad
\overline U_2=\frac{Q}{\pi R_2^2}=0.80\,\mathrm{m\,s^{-1}}.
$$

The radius halves, the [area](differential-geometry.md#surface-area) falls to one quarter, and the mean [velocity](classical-mechanics.md#velocity) quadruples. The [mass flow rate](#mass-flow-rate) is $\rho Q=0.02\pi\,\mathrm{kg\,s^{-1}}$. The same amount of water passes both sections each second; narrowing changes its speed rather than compressing it. The [Reynolds number](dynamic-viscosity.md#reynolds-number) and [Bernoulli's principle](euler-equations-for-an-inviscid-fluid.md#bernoulli-s-principle) discussions use this same example to examine viscous effects and the additional assumptions needed to calculate [pressure](pressure.md).

<a id="image-continuity-fixes-the-mean-speeds-bernoulli-s-principle-gives-a-conditional-ideal-pressure-drop"></a>
![](fluid-flow-constriction.png)

**[Figure 14](#image-continuity-fixes-the-mean-speeds-bernoulli-s-principle-gives-a-conditional-ideal-pressure-drop). Continuity fixes the mean speeds; Bernoulli's principle gives a conditional ideal pressure drop**. The pipe outline shows the radius ratio. Arrows represent section means, not a computed velocity field. The bars show the constant $Q$ and the ideal exchange between pressure and kinetic energy density at equal height; $p_2$ is the arbitrary pressure reference.

### Rectilinear flow

↑ **Parent:** [Incompressible flow](#incompressible-flow)

A [rectilinear flow](#rectilinear-flow) has velocity everywhere parallel to a fixed direction and independent of the coordinate in that direction, for example $U(y,z)\widehat x$. Its convective acceleration vanishes. A steady incompressible viscous rectilinear flow obeys the linear transverse Poisson equation $\nu\Delta U=\rho^{-1}dp/dx$, rather than an inertia-viscosity balance. This explains Reynolds-number independence of the spatial equation with fixed scaled forcing and boundary data.

### Streamfunction advection bracket

↑ **Parent:** [Incompressible flow](#incompressible-flow)

For the two-dimensional [streamfunction](#stream-function) convention $u=\psi_z$, $w=-\psi_x$, the advective derivative of $\theta$ is $u\theta_x+w\theta_z=J(\psi,\theta)$. This antisymmetric [Jacobian determinant](multivariable-calculus.md#jacobian-determinant) bracket organizes nonlinear interactions in convection and vorticity equations.

### Cartesian streamfunction

↑ **Parent:** [Incompressible flow](#incompressible-flow)

For a two-dimensional [incompressible flow](#incompressible-flow), a Cartesian streamfunction $\psi$ defines $u=\partial_y\psi$ and $v=-\partial_x\psi$. The continuity equation $u_x+v_y=0$ then holds identically.

### Divergence-free vector field

↑ **Parent:** [Incompressible flow](#incompressible-flow)

A divergence-free vector field satisfies $\nabla\mathbin\cdot u=0$. It preserves volume under its flow, and its transport operator is skew-symmetric when boundary fluxes vanish.

## Streakline

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Streakline)

A [streakline](#streakline) at observation time $T$ is the set of present positions of all [fluid elements](continuum-mechanics.md#fluid-element) that passed through one fixed release point $\mathbf a$ during a specified history of injection. For continuous release over $\tau_0\leq\tau\leq T$, solve a different [initial value problem](differential-equation.md#initial-value-problem) for each release time $\tau$:

$$
\frac{\partial\mathbf X}{\partial t}(t;\tau,\mathbf a)=\mathbf u(\mathbf X(t;\tau,\mathbf a),t),\qquad \mathbf X(\tau;\tau,\mathbf a)=\mathbf a,\qquad \mathcal S_T=\{\mathbf X(T;\tau,\mathbf a):\tau_0\leq\tau\leq T\}.
$$

Thus a [pathline](#pathline) varies $t$ for one particle; a [streakline](#streakline) varies $\tau$ while holding $T$ fixed. Interrupted release gives only the corresponding subsets of the [streakline](#streakline). A moving nozzle requires a time-dependent release position instead, so the standard fixed-point definition should not silently be applied to it. Continuous release makes [streaklines](#streakline) easy to observe and useful for showing where material from one source has reached. [MIT Marine Hydrodynamics, lecture 2, section 1.2](https://web.mit.edu/13.021/demos/lectures/lecture2.pdf)

In the analytical [velocity field](#velocity-field) $(U,at)$ of [pathline](#pathline), a particle released at the origin at time $\tau$ follows

$$
x(t;\tau)=U(t-\tau),\qquad y(t;\tau)=\frac a2(t^2-\tau^2),\qquad t\geq\tau.
$$

Observe all particles together at time $T$, after continuous release from $\tau=0$:

$$
x=U(T-\tau),\qquad y=\frac a2(T^2-\tau^2),\qquad y=\frac{aT}{U}x-\frac{a}{2U^2}x^2,\qquad 0\leq x\leq UT.
$$

For $U=1\ \mathrm{m\,s^{-1}}$, $a=1\ \mathrm{m\,s^{-2}}$ and $T=2\ \mathrm s$, the [streakline](#streakline) is the downward-curving [parabola](euclidean-geometry.md#parabola) $y=2x-x^2/2$ in metre coordinates. Releases at $\tau=0,1,2\ \mathrm s$ occupy $(2,2)$, $(1,1.5)$ and $(0,0)\ \mathrm m$, respectively. At $x=1\ \mathrm m$, the [streakline](#streakline) lies above the [pathline](#pathline) $y=x^2/2$ and below the origin's [streamline](#streamline) $y=2x$. All particles nevertheless have the same present [velocity](classical-mechanics.md#velocity) $(1,2)\ \mathrm{m\,s^{-1}}$. The [streakline](#streakline) slope $dy/dx=a\tau/U$ generally differs from the present [velocity](classical-mechanics.md#velocity) slope $aT/U$; they agree at the nozzle. The oldest particle is the downstream endpoint, which explains why the [pathline](#pathline) and [streakline](#streakline) meet there without being the same curve.

<a id="image-analytical-release-families-observed-at-one-and-two-seconds"></a>
![](stream-path-streak-lines-release-family.png)

**[Figure 15](#image-analytical-release-families-observed-at-one-and-two-seconds). Analytical release families observed at one and two seconds**.

Each panel fixes one observation time. Coloured dots are the present positions of particles with the indicated release times; dashed [pathlines](#pathline) show those particles' earlier histories. The black [streakline](#streakline) connects present positions of the continuously released family, including release times between the sampled dots. After $T=1\ \mathrm s$, particles already present keep moving and new ones enter at the origin, so the later [streakline](#streakline) is not a frozen record of the earlier one. Injection beginning only at $\tau=1\ \mathrm s$ would show just $0\leq x\leq1\ \mathrm m$ of the $T=2\ \mathrm s$ curve. Both panels are diffusion-free analytical models, not experimental photographs.

Kline's contracting-channel demonstration switches from marking an element to continuous bubble production at a marking wire: the resulting trace is a [streakline](#streakline). The apparatus therefore changes the curve being displayed by changing the marking history, even with the same channel. A wire produces a family of traces; conceptually each fixed emitting location supplies its own [streakline](#streakline). Individual bubbles are markers rather than perfect [fluid elements](continuum-mechanics.md#fluid-element): Jean Hertzberg's teaching notes describe [hydrogen](chemical-substance.md#hydrogen) production by [electrolysis](electrochemistry.md#electrolysis) at a thin [cathode](electrochemistry.md#cathode) wire and warn that larger bubbles have more [buoyancy](#buoyancy). [S. J. Kline, Flow Visualization film notes, figure 8](https://web.mit.edu/hml/ncfmf/05FV.pdf) [Jean Hertzberg and Flow Vis course students, Particles 3: In Water](https://www.flowvis.org/Flow%20Vis%20Guide/particles-3-in-water/)

A dye version uses a small fixed injection port upstream in a transparent water channel, a dilute premix of dye with the channel water, illumination and a fixed [optical camera](optical-instrument.md#optical-camera). Start continuous injection at a recorded time $\tau_0$ and take a short exposure at $T$: the visible filament approximates a [streakline](#streakline), not the accumulated [pathline](#pathline) of one particle. Repeat with the same port and imaging geometry after changing the flow with time; compare the filament against local directions estimated from short displacements of sparse markers at $T$. Agreement in a [steady flow](#steady-flow) and possible disagreement when the flow changes are the predictions being tested; no measured curves are claimed here. The protocol follows Hertzberg's advice to use small ports, little injected volume and a dilute premix with matched [density](#density) and [viscosity](dynamic-viscosity.md). Check for nozzle disturbance by reducing injection rate, for [buoyancy](#buoyancy) by watching the premix in still water, and for [diffusion](thermodynamics.md#diffusion) by comparing filament widths at different ages. Keep exposure short enough to suppress motion blur. Dye [concentration](mathematical-physics.md#concentration) approximates a [passive scalar](scalar-transport.md#passive-scalar) only when it has negligible feedback on the [velocity field](#velocity-field); finite port width, [diffusion](thermodynamics.md#diffusion) and out-of-plane motion limit how literally a visible filament can be read as a geometrical [streakline](#streakline). [Jean Hertzberg and Flow Vis course students, Dye Techniques 1: Do Not Disturb](https://www.flowvis.org/Flow%20Vis%20Guide/do-not-disturb-dyes-in-liquids/)

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

At an interface between two inviscid fluids without surface tension, the pressure is continuous. For potential flows of equal density, the [Unsteady Bernoulli equation](euler-equations-for-an-inviscid-fluid.md#unsteady-bernoulli-equation) therefore equates

$$
\partial_t\phi+\frac12|\nabla\phi|^2
$$

on the two sides, up to a removable function of time.

### Pressure continuity

↑ **Parent:** [Dynamic boundary condition for an inviscid interface](#dynamic-boundary-condition-for-an-inviscid-interface)

For an inviscid interface with no [surface tension](surface-tension.md), continuity of normal [traction](continuum-mechanics.md#traction) reduces to continuity of [pressure](pressure.md). The same condition is used in a sharp [Darcy law](porous-media-flow.md#darcy-law) interface model that neglects [capillary pressure](surface-tension.md#capillary-pressure) and resolved interfacial viscous normal [stress](continuum-mechanics.md#stress). For a general viscous interface, continuity of normal [traction](continuum-mechanics.md#traction) balances the full [stress](continuum-mechanics.md#stress) [tensor](multilinear-algebra.md#tensor); it does not by itself imply continuity of [pressure](pressure.md).

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

One sign has positive [growth rate](dispersion-relation.md#growth-rate), so every nonzero wavenumber is unstable in the inviscid zero-thickness model.

##### Minimum shear for capillary Kelvin-Helmholtz instability

↑ **Parent:** [Kelvin-Helmholtz instability](#kelvin-helmholtz-instability)

For two infinitely deep inviscid layers with stable density ordering $\rho_2>\rho_1$ and positive [surface tension](surface-tension.md) $\gamma$, the velocity jump destabilizes wavenumber $k$ precisely when

$$
U^2>\frac{\rho_1+\rho_2}{\rho_1\rho_2}
\left(\frac{(\rho_2-\rho_1)g}{|k|}+\gamma|k|\right).
$$

The threshold diverges at both small and large wavenumber. Minimizing the bracket gives $|k|=\sqrt{(\rho_2-\rho_1)g/\gamma}$ and the stated minimum velocity jump. A larger jump opens a bounded band of unstable wavenumbers, obtained from the two positive roots of $\gamma q^2-[\rho_1\rho_2U^2/(\rho_1+\rho_2)]q+(\rho_2-\rho_1)g=0$. Equality at threshold is marginal rather than exponential growth.

##### Vortex sheet in a symmetric rigid channel

↑ **Parent:** [Kelvin-Helmholtz instability](#kelvin-helmholtz-instability)

Consider an equal-density [vortex sheet](#vortex-sheet) halfway between rigid walls, with equal layer depths $h$, base [velocities](classical-mechanics.md#velocity) $U_1,U_2$ and no restoring interfacial force. The irrotational perturbations have vertical factors $\cosh(k(y-h))$ above and $\cosh(k(y+h))$ below. Their [kinematic boundary conditions](#kinematic-boundary-condition) and [pressure continuity](#pressure-continuity) give

$$
\coth(|k|h)\left[(\omega-kU_1)^2+(\omega-kU_2)^2\right]=0.
$$

The common depth factor cancels, yielding the displayed [dispersion relation](dispersion-relation.md) roots and [Kelvin-Helmholtz instability](#kelvin-helmholtz-instability) for nonzero shear. The real [phase velocity](dispersion-relation.md#phase-velocity) of the pattern is $(U_1+U_2)/2$ and the growing branch has [temporal growth rate](dispersion-relation.md#growth-rate) $|k(U_1-U_2)|/2$. This exact depth cancellation depends on equal depths and equal [mass densities](#density); a single nearby wall or unequal layers changes the inertia factors.

##### Two-fluid interfacial gravity-shear dispersion relation

↑ **Parent:** [Kelvin-Helmholtz instability](#kelvin-helmholtz-instability)

For two inviscid incompressible half-spaces, lower density/[velocity](classical-mechanics.md#velocity) $\rho_1,U_1$, upper density/[velocity](classical-mechanics.md#velocity) $\rho_2,U_2$, downward [gravity](physics.md#gravity) $g$ and [surface tension](surface-tension.md) $\sigma$, a mode $e^{i(kx-\omega t)}$ with $k>0$ obeys

$$
(\omega-k\overline U)^2=\frac{gk(\rho_1-\rho_2)+\sigma k^3}{\rho_1+\rho_2}-\frac{\rho_1\rho_2}{(\rho_1+\rho_2)^2}k^2(U_1-U_2)^2,\qquad\overline U=\frac{\rho_1U_1+\rho_2U_2}{\rho_1+\rho_2}.
$$

A negative right-hand side produces exponential growth. The gravitational term recovers [Rayleigh-Taylor instability](continuum-mechanics.md#rayleigh-taylor-instability) for heavy-over-light ordering; the shear term can destabilize otherwise stable stratification. Finite layer thickness, [viscosity](dynamic-viscosity.md), compressibility and [magnetic tension](magnetohydrodynamics.md#magnetic-tension) lie outside this interface model.

##### Bending-membrane Kelvin-Helmholtz dispersion relation

↑ **Parent:** [Kelvin-Helmholtz instability](#kelvin-helmholtz-instability)

For equal fluid density $\rho$ on opposite sides of a massless flat membrane, a velocity jump $U$ and bending pressure jump $\beta\eta_{xxxx}$ with $\beta>0$, a mode $e^{ikx+\sigma t}$ satisfies

$$
(\sigma+ikU/2)^2=U^2k^2/4-\beta|k|^5/(2\rho).
$$

The decaying upper and lower perturbation potentials are $A_+e^{-|k|y}$ and $A_-e^{|k|y}$. Their kinematic conditions are $-|k|A_+=(\sigma+ikU)\eta$ and $|k|A_-=\sigma\eta$. The linearized [Bernoulli equation](euler-equations-for-an-inviscid-fluid.md#bernoulli-equation) gives $p_- -p_+=-\rho[\sigma^2+(\sigma+ikU)^2]\eta/|k|$. Equating it to the bending pressure yields the relation. Bending stabilizes $|k|^3\ge\rho U^2/(2\beta)$. The maximum positive growth is at $|k|^3=\rho U^2/(5\beta)$ and is $|U|\,|k|\sqrt{3/20}$.

##### Kelvin-Helmholtz dispersion relation with gravity

↑ **Parent:** [Kelvin-Helmholtz instability](#kelvin-helmholtz-instability)

Two deep layers of [incompressible flow](#incompressible-flow) with upper [mass density](#density) $\rho_1$, lower [mass density](#density) $\rho_2$, and tangential [velocities](classical-mechanics.md#velocity) $U_1,U_2$ have this [dispersion relation](dispersion-relation.md) when [surface tension](surface-tension.md) is absent. Decaying [velocity potentials](#velocity-potential) and the linearized [kinematic boundary condition](#kinematic-boundary-condition) determine their amplitudes; the [dynamic boundary condition for an inviscid interface](#dynamic-boundary-condition-for-an-inviscid-interface) gives the displayed relation. For $k>0$ the squared departure of the [phase velocity](dispersion-relation.md#phase-velocity) $c$ from the density-weighted mean [velocity](classical-mechanics.md#velocity) is $g(\rho_2-\rho_1)/[k(\rho_1+\rho_2)]-\rho_1\rho_2(U_1-U_2)^2/(\rho_1+\rho_2)^2$. A negative value gives [Kelvin-Helmholtz instability](#kelvin-helmholtz-instability) despite stable [density stratification](gravity-wave.md#density-stratification).

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

For a [top-hat planar jet](#top-hat-planar-jet) in stationary fluid of the same [mass density](#density), odd and even [velocity potentials](#velocity-potential) have the same [temporal growth rate](dispersion-relation.md#growth-rate). Put $s=\tanh(|k|L)$. Their [dispersion relations](dispersion-relation.md) use $s$ and $1/s$, but $\sqrt{s}/(1+s)=\sqrt{1/s}/(1+1/s)$. Their real [phase velocities](dispersion-relation.md#phase-velocity) are respectively $Vs/(1+s)$ and $V/(1+s)$. The common [growth rate](dispersion-relation.md#growth-rate) is strictly below $|kV|/2$ for finite $|k|L>0$, approaching the isolated [vortex sheet](#vortex-sheet) value when the sheets decouple.

##### Finite-depth vortex-sheet dispersion relation

↑ **Parent:** [Kelvin-Helmholtz instability](#kelvin-helmholtz-instability)

For an equal-density vortex sheet a distance $h$ above a rigid wall, with lower and upper base velocities $U$ and zero, a mode $e^{i(kx-\omega t)}$ satisfies

$$
(\omega-kU)^2\coth(|k|h)+\omega^2=0.
$$

The wall changes the inertia of the lower perturbation through the factor $\coth(|k|h)$.

## Astrophysical fluid dynamics

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](astrophysical-fluid-dynamics.md)

## Compressible flow

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](compressible-flow.md)

## Geophysical fluid dynamics

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](geophysical-fluid-dynamics.md)

## Linear acoustics

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](linear-acoustics.md)

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

For a [passive scalar](scalar-transport.md#passive-scalar) in a planar [shear flow](#shear-flow) $u(y,t)$, let $m_j(y,t)=\int_{\mathbb R}x^j\chi(x,y,t)\,dx$. Integrating the [advection-diffusion equation](diffusion-equation.md#advection-diffusion-equation) by parts in $x$ gives the displayed hierarchy for $j\geq0$, with negative-index terms omitted. Sufficient decay and finite moments justify the integrations. Insulating walls give [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition) for every moment. Solving the first two equations then determines the long-time growth of the second moment without solving the full scalar field.

##### Oscillating shear dispersion in an insulating channel

↑ **Parent:** [Longitudinal moment hierarchy for shear transport](#longitudinal-moment-hierarchy-for-shear-transport)

For $u=U\cos(\omega t)\sin(\pi y/L)$ on $|y|<L/2$, positive [diffusivity](brownian-motion.md#diffusion-coefficient) $\kappa$, nonzero frequency and insulating walls, a transversely uniform zeroth moment remains constant. Its first moment is proportional to $g(t)\sin(\pi y/L)$, where $g'+ag=U\cos(\omega t)$. The periodic solution is $g=U[a\cos(\omega t)+\omega\sin(\omega t)]/(a^2+\omega^2)$. The [longitudinal moment hierarchy for shear transport](#longitudinal-moment-hierarchy-for-shear-transport) then gives $m_2=2Ktm_0+O(1)$ after both transverse and periodic transients. The spatial average of $\sin^2(\pi y/L)$ is $1/2$ and the time average of $\cos^2(\omega t)$ is $1/2$, producing the factor $1/4$. At exactly zero frequency the steady enhancement is instead $U^2/(2a)$; averaging indefinitely over slow cycles does not commute with setting the frequency to zero.

#### Effective diffusivity of a periodic sinusoidal shear

↑ **Parent:** [Taylor dispersion](#taylor-dispersion)

For a [passive scalar](scalar-transport.md#passive-scalar) transported by $U(t)\sin(my)$ with transverse period $2\pi/m$, positive [diffusivity](brownian-motion.md#diffusion-coefficient) $\kappa$ and periodic $U$, let $g$ be the unique periodic solution of $g'+\kappa m^2g=U$. A [multiple-scale expansion](singular-perturbation.md#method-of-multiple-scales) has first corrector $-g(t)\sin(my)\partial_X\overline\chi$. Averaging the next-order equation over the space-time cell gives the displayed longitudinal [diffusion coefficient](brownian-motion.md#diffusion-coefficient). Averaging $gg'+\kappa m^2g^2=Ug$ proves the second form. This is a long-time, long-wavelength effective equation, after transverse and periodic transients have decayed, rather than an exact finite-time closure for arbitrary concentrations.

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

## Porous-media flow

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](porous-media-flow.md)

## Reduced gravity

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](reduced-gravity.md)

## Rheology

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

[This section is present in another page, follow this link to view it.](rheology.md)

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

An interfacial stress $\tau=c_D\rho_lu_I^2$ supplies local stress power $P_I=S\tau u_I$. Assuming a fixed fraction $C_W$ becomes global [potential energy](energy.md#potential-energy) gives $\dot E_P=C_WP_I$. Together with [potential energy of two-layer entrainment](#potential-energy-of-two-layer-entrainment), this gives $\dot h=2C_Wc_Du_I^3/(g'h)$. This is an additional local power-transfer closure. The shaft power of a rotating lid is its torque times its prescribed angular speed and need not equal $P_I$. Geometric factors and a constant transfer fraction may be absorbed into the empirical coefficients only when explicitly assumed time-independent.

### Potential energy of two-layer entrainment

↑ **Parent:** [Fluid entrainment](#fluid-entrainment)

In a closed tank of cross-sectional area $S$, entrainment into a uniform upper layer conserves the density deficit $(\rho_l-\rho_u)h$. Thus $B=g'h$ is constant. With depth $z$ increasing downward, gravitational [potential energy](energy.md#potential-energy) is $-gS\int_0^H\rho(z)z\,dz=E_*+\rho_lSBh/2$, so its rate of increase is proportional to the rate of deepening. This includes homogenization throughout the upper layer, not merely lifting a thin parcel across the interface.

#### Potential energy of mixed-layer deepening with an initial buoyancy jump

↑ **Parent:** [Potential energy of two-layer entrainment](#potential-energy-of-two-layer-entrainment)

Let an initial upper mixed layer have finite depth $a$, buoyancy $b_1$, and fixed upper boundary; beneath it let $b=b_1-\Delta b+N^2z$ with the initial interface at $z=0$. Homogenization down to $z=-d$ conserves [buoyancy](#buoyancy) and gives mixed buoyancy $b_1-[\Delta b\,d+N^2d^2/2]/(a+d)$. Integrating gravitational [potential energy](energy.md#potential-energy) over the initial and final profiles gives the displayed increase per unit area. Its derivative is $\rho_0[\Delta b\,a/2+N^2a d/2+N^2d^2/4]$. Specifying absorbed mixing power is not enough to determine deepening unless the initial depth or an alternative upper-reservoir model is supplied.

### Fixed-energy turbulent mixed layer

↑ **Parent:** [Fluid entrainment](#fluid-entrainment)

In a slowly deepening mixed layer driven by a rotating boundary, a phenomenological balance between energy input, turbulent loss and acceleration of entrained fluid can keep total [kinetic energy](energy.md#kinetic-energy) approximately fixed. For a tank of radius $R$ this gives $u^2h=A\Omega^2R^3$, so velocity decreases as $h^{-1/2}$. The closure does not make the speed constant and is an additional physical assumption rather than a direct consequence of [mass conservation](continuum-mechanics.md#mass-conservation).

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

### Stack effect

↑ **Parent:** [Natural ventilation](#natural-ventilation)

Buoyancy-driven flow associated with differences in [air](mixture.md#air) density and the vertical separation of openings; heating can drive outflow above and replacement inflow below.

### Cross ventilation

↑ **Parent:** [Natural ventilation](#natural-ventilation)

Exchange through openings on different sides of a space, driven by suitable external [pressure differences](pressure.md#pressure-difference).

### Ventilation after a heating reduction

↑ **Parent:** [Natural ventilation](#natural-ventilation)

For an ideal two-layer [natural ventilation](#natural-ventilation) transient following a heating change $Q\mapsto\lambda Q$, let $V_0$ and $\theta_0$ be the initial flow and temperature excess, $s=V_0t/(A_rH)$, $\eta=h/H$, and $x=\eta(1-\theta/\theta_0)$. The integrated buoyancy pressure gives $V/V_0=\sqrt{1-x}$, while [heat](heat.md) balance gives $x_s=\sqrt{1-x}-\lambda$. A material interface satisfies $\eta_s=\sqrt{1-x}$, so $\eta=x+\lambda s$. For $0<\lambda<1$, $x$ increases toward $1-\lambda^2$ and $\eta_s\geq\lambda$, ensuring finite-time filling of the room. After filling, $y=\theta/\theta_0$ obeys $y_s=\lambda-y^{3/2}$ and tends to $\lambda^{2/3}$. This model assumes well-mixed individual layers, negligible wall heat capacity and a sharp advected interface.

### Well-mixed ventilation temperature balance

↑ **Parent:** [Natural ventilation](#natural-ventilation)

For a distributed [heat](heat.md) source, a well-mixed interior with [temperature](temperature.md) excess $\theta$ gains temperature-volume flux $\mathcal H$ and loses $|q|\theta$ by ventilation in either direction. With signed upward throughflow, $q|q|=K_A(G_T\theta\pm W)$, where $G_T=g\alpha_TH_b$ and $W$ is wind [pressure](pressure.md) divided by [mass density](#density). The plus sign is assisting wind. Steady temperatures satisfy $\theta^2(G_T\theta+W)=\mathcal H^2/K_A$ for assistance, or $\theta^2|G_T\theta-W|=\mathcal H^2/K_A$ for opposition. Direction restrictions must be applied to roots.

#### Opposing-wind ventilation bistability

↑ **Parent:** [Well-mixed ventilation temperature balance](#well-mixed-ventilation-temperature-balance)

For $0<\varepsilon<2/(3\sqrt3)$, the [well-mixed ventilation temperature balance](#well-mixed-ventilation-temperature-balance) has one stable upward-flow [temperature](temperature.md) and two downward-flow temperatures. The heat-removal curve on the latter interval is $\sqrt{K_A}\theta\sqrt{W-G_T\theta}$, maximal at $2W/(3G_T)$. Its lower-temperature root is stable and its higher-temperature root unstable. The two meet at a [saddle-node bifurcation](bifurcation-theory.md#saddle-node-bifurcation). The unstable root separates the basins of the stable wind-dominated and buoyancy-dominated states.

##### Ventilation switching under wind and heating changes

↑ **Parent:** [Opposing-wind ventilation bistability](#opposing-wind-ventilation-bistability)

Increasing wind or reducing heating both reduce the control parameter of [opposing-wind ventilation bistability](#opposing-wind-ventilation-bistability). However, wind moves the reversal threshold $\theta_w=W/G_T$, whereas heating does not. A sufficiently abrupt wind increase can place a hot upward-flow state in the cooler state's basin. Reducing positive heating at fixed wind cannot make an upward-flow state cross $\theta_w$, because its [temperature](temperature.md) time derivative there is positive. Slow variation follows a persistent stable branch; a fold destroys the cooler branch when wind is weakened or [heat](heat.md) input increased.

### Effective opening area for pressure-driven ventilation

↑ **Parent:** [Natural ventilation](#natural-ventilation)

An effective opening area may absorb both the discharge coefficient and the factor of two in an orifice law. If $A_e=\sqrt2C_dA_{\rm geom}$, its discharge is $q=A_e\sqrt{\delta p/\rho}$. Two equal openings carrying the same flux share the total [pressure](pressure.md) drop, so $q^2=A_e^2\Delta p/(2\rho)$. They do not share equal drops when an internal volume source makes their fluxes unequal. State the effective-area convention before comparing numerical factors in [natural ventilation](#natural-ventilation) models.

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

A source volume $Q$ makes roof outflow exceed floor inflow by $Q$. At zero floor inflow, an entraining plume cannot support a steady cold lower layer; the warm layer reaches the floor. With [reduced gravity](reduced-gravity.md) $g'=B/Q$, the entire hydrostatic head drives roof discharge $Q=A_e\sqrt{g'H}$. This gives the stated threshold. Equal splitting of [pressure](pressure.md) head is inappropriate at blocking. The same result in physical-area notation is $Q_c=(2C_d^2A_{\rm geom}^2BH)^{1/3}$.

#### Ventilated filling-box relaxation

↑ **Parent:** [Displacement ventilation](#displacement-ventilation)

For total plume flux $P(h)$, fixed ceiling exhaust $F$, zero ambient [buoyancy](#buoyancy), and uniform upper-layer [reduced gravity](reduced-gravity.md) $b$, the ideal two-layer balances are

$$
A\dot h=F-P(h),\qquad \frac{d}{dt}\bigl[A(H-h)b\bigr]=B-Fb.
$$

At $P(h_*)=F$ and $b_*=B/F$, [linearization](algebra.md#linearization) yields the decay times $\tau_h=A/P'(h_*)$ and $\tau_b=A(H-h_*)/F$. For $P(h)\propto h^{5/3}$, $\tau_h=3Ah_*/(5F)$. Upper-layer [buoyancy](#buoyancy) relaxation usually dominates when $h_*\ll H$. Exact equilibrium is approached asymptotically; a fixed small relative tolerance takes order $\max(\tau_h,\tau_b)\log(1/\varepsilon)$ after the initial transient.

#### No steady displacement layer without ambient supply

↑ **Parent:** [Displacement ventilation](#displacement-ventilation)

Consider entraining plumes supplied with total source [volume flux](#volumetric-flow-rate) $S$, a separate lower-layer ambient inflow $L$, and ceiling exhaust $F=S+L$. Write $P(h)=S+E(h)$, where $E(h)$ is total [fluid entrainment](#fluid-entrainment) from the lower layer. [Volume conservation](mathematical-physics.md#volume-conservation) gives $A\dot h=L-E(h)$. A steady positive lower layer therefore requires $L=E(h)>0$. If $L=0$ and $E(h)>0$ for every $h>0$, no positive steady [displacement-ventilation interface height](#displacement-ventilation-interface-height) exists. In a shifted [pure plume](turbulent-plume.md#pure-plume) approximation $P_i(h)=\lambda B_i^{1/3}(h+z_i)^{5/3}$ matched to source flux $S_i$ at $h=0$, this follows immediately from $P_i(h)>S_i$ for $h>0$. This is a statement about the ideal two-layer model, not a prohibition of all possible stratification in a real ventilated room.

#### Multiple-plume displacement ventilation

↑ **Parent:** [Displacement ventilation](#displacement-ventilation)

Suppose $n$ independent [axisymmetric pure plumes](turbulent-plume.md#axisymmetric-pure-plume) share total [buoyancy flux](turbulent-plume.md#buoyancy-flux) $B$ equally, have negligible source [volume flux](#volumetric-flow-rate), and are supplied with a separate ambient ventilation flux $F$ at floor level. Their combined flux is $P(h)=\lambda n^{2/3}B^{1/3}h^{5/3}$. [Volume conservation](mathematical-physics.md#volume-conservation) at a steady [displacement-ventilation interface height](#displacement-ventilation-interface-height) and [buoyancy flux](turbulent-plume.md#buoyancy-flux) conservation give

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

## Orifice

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)

An [orifice](#orifice) is a small opening through which a [fluid](#fluid) can flow.

### Vena contracta

↑ **Parent:** [Orifice](#orifice)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vena_contracta)

The [vena contracta](#vena-contracta) is the narrowest jet section after an opening. Its [area](differential-geometry.md#surface-area) may be smaller than the opening area, so the jet [speed](classical-mechanics.md#speed) and [volumetric flow rate](#volumetric-flow-rate) require separate comparisons with ideal flow.

## Nozzle

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nozzle)

A [nozzle](#nozzle) shapes a passage to control the speed and direction of a [fluid flow](#fluid-flow). In [compressible flow](compressible-flow.md), converging-diverging passages can accelerate a [gas](thermodynamics.md#gas) through a [sonic flow](compressible-flow.md#sonic-flow) throat into [supersonic flow](compressible-flow.md#supersonic-flow).

### Isentropic nozzle flow

↑ **Parent:** [Nozzle](#nozzle)

Smooth adiabatic [nozzle](#nozzle) flow without [entropy](entropy.md) production. In a steady quasi-one-dimensional ideal-gas model, $\rho uA$ and $u^2/2+c_pT$ are constant along the passage. A converging-diverging passage can connect subsonic and supersonic branches through a sonic throat when reservoir and back-pressure conditions select that branch.

#### Adiabatic nozzle terminal speed

↑ **Parent:** [Isentropic nozzle flow](#isentropic-nozzle-flow)

For a lossless [polytropic flow](compressible-flow.md#polytropic-flow) with $\gamma>1$, negligible [gravity](physics.md#gravity) and a sonic throat, the [Bernoulli function](euler-equations-for-an-inviscid-fluid.md#bernoulli-function) is $u^2/2+c_s^2/(\gamma-1)=(\gamma+1)c_*^2/[2(\gamma-1)]$. On an expanding supersonic branch for which $\rho\to0$, the [specific enthalpy](enthalpy.md#specific-enthalpy) vanishes and the limiting [velocity](classical-mechanics.md#velocity) is the displayed value. If area grows as $Cr^2$, [mass conservation](continuum-mechanics.md#mass-conservation) further gives $\rho\sim\dot M/(Cu_\infty r^2)$. A subsonic pressure-confined branch need not have this asymptotic behavior.

#### Sonic density of a polytropic nozzle

↑ **Parent:** [Isentropic nozzle flow](#isentropic-nozzle-flow)

For steady [polytropic flow](compressible-flow.md#polytropic-flow) with $p=K\rho^\gamma$, $K>0$, $\gamma>1$, a sonic section has $u_*=c_*=(\gamma K\rho_*^{\gamma-1})^{1/2}$. Substitution in [mass conservation](continuum-mechanics.md#mass-conservation) $\dot M=A_*\rho_*u_*$ gives the displayed density. These conditions fix the sonic state for a prescribed flux and throat area, subject to compatible reservoir and downstream [boundary conditions](differential-equation.md#boundary-condition).

#### de Laval nozzle

↑ **Parent:** [Isentropic nozzle flow](#isentropic-nozzle-flow)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/de_Laval_nozzle)

A converging-diverging [nozzle](#nozzle) that can accelerate a [compressible flow](compressible-flow.md) from subsonic to supersonic speed through a sonic throat. The [nozzle area-velocity relation](#nozzle-area-velocity-relation) requires acceleration in a converging subsonic section and a diverging supersonic section. Reservoir and downstream [pressures](pressure.md) determine whether this [transonic branch](compressible-flow.md#transonic-branch) operates; the shape alone does not ensure [choked flow](compressible-flow.md#choked-flow).

#### Nozzle area-Mach number relation

↑ **Parent:** [Isentropic nozzle flow](#isentropic-nozzle-flow)

For a calorically [perfect gas](ideal-gas.md) on a steady isentropic [nozzle](#nozzle) branch,

$$
\frac A{A_*}=\frac1M\left[\frac2{\gamma+1}\left(1+\frac{\gamma-1}{2}M^2\right)\right]^{(\gamma+1)/(2(\gamma-1))}.
$$

Here $A_*$ is the sonic area. An area ratio greater than one generally admits a subsonic and a supersonic root; [boundary conditions](differential-equation.md#boundary-condition) choose the physical branch. Numerical inversion must retain that branch information.

#### Nozzle area-velocity relation

↑ **Parent:** [Isentropic nozzle flow](#isentropic-nozzle-flow)

Steady [mass conservation](continuum-mechanics.md#mass-conservation), inviscid momentum balance and $dp=c_s^2d\rho$ give $d\ln A=(M^2-1)d\ln u$, where $M=u/c_s$. A smooth sonic crossing needs an area extremum; a minimum-area throat supports an accelerating subsonic-to-supersonic branch. A throat is a necessary geometric condition, not a sufficient specification of operating [pressures](pressure.md).

## ↑ Ancestors (3)

1. [Branches of physics](physics.md#branches-of-physics)
2. [Physics](physics.md)
3. [Codex Wiki](README.md)

## ← Incoming links (9)

- [Climate model](geophysics.md#climate-model)
- [Continuum approximation](continuum-mechanics.md#continuum-approximation)
- [Fluid mechanics](fluid-mechanics.md)
- [Leon van Dommelen](engineering.md#leon-van-dommelen)
- [Reactor thermal hydraulics](engineering.md#reactor-thermal-hydraulics)
- [Sonic point of a scalar flux](transport-equation.md#sonic-point-of-a-scalar-flux)
- [Stokes flow](stokes-flow.md)
- [Thermodynamics, Heat Transfer, and Fluid Flow, Volume 3 by the United States Department of Energy](engineering.md#thermodynamics-heat-transfer-and-fluid-flow-volume-3-by-the-united-states-department-of-energy)
- [Weather forecasting](geophysics.md#weather-forecasting)
