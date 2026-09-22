# Critical phenomenon

↑ **Parent:** [Statistical physics](statistical-physics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Critical_phenomenon)

A critical phenomenon is scale-invariant behavior near a continuous phase transition, described by universal critical exponents.

**Table of contents**

- [Universality of critical phenomena](#universality-of-critical-phenomena)
- [Thermodynamic critical point](#thermodynamic-critical-point)
  - [Critical point of a cubic density equation of state](#critical-point-of-a-cubic-density-equation-of-state)
    - [Spinodal densities of a cubic gas](#spinodal-densities-of-a-cubic-gas)
  - [Critical concentration](#critical-concentration)
- [Lifshitz point](#lifshitz-point)
  - [Uniaxial Lifshitz Gaussian renormalization](#uniaxial-lifshitz-gaussian-renormalization)
- [Liquid-gas critical point](#liquid-gas-critical-point)
  - [Supercritical fluid](#supercritical-fluid)
- [Quantum critical point](#quantum-critical-point)
  - [Quantum-critical regime](#quantum-critical-regime)
  - [Quantum critical scaling](#quantum-critical-scaling)
    - [Dynamical critical exponent](#dynamical-critical-exponent)
- [Phase transition](#phase-transition)
  - [Crystallization](#crystallization)
  - [Reconstructive transformation](#reconstructive-transformation)
  - [Hexatic phase](#hexatic-phase)
  - [Displacive transformation](#displacive-transformation)
  - [Vitrification](#vitrification)
  - [Metal-insulator transition](#metal-insulator-transition)
    - [Mott criterion](#mott-criterion)
  - [Liquefaction of gases](#liquefaction-of-gases)
  - [Condensation](#condensation)
  - [Melting](#melting)
  - [Freezing](#freezing)
    - [Morphological instability of a solidification front](#morphological-instability-of-a-solidification-front)
  - [Quantum phase transition](#quantum-phase-transition)
  - [Sublimation](#sublimation)
    - [Sublimation-front capillary instability](#sublimation-front-capillary-instability)
    - [Radiatively heated sublimation profile](#radiatively-heated-sublimation-profile)
    - [Dust sublimation](#dust-sublimation)
      - [Blackbody dust sublimation radius](#blackbody-dust-sublimation-radius)
        - [Thermal stability of externally heated blackbody dust](#thermal-stability-of-externally-heated-blackbody-dust)
          - [Dust-destruction feedback at a sublimation front](#dust-destruction-feedback-at-a-sublimation-front)
  - [Phase coexistence](#phase-coexistence)
    - [Ehrenfest entropy-continuity relation](#ehrenfest-entropy-continuity-relation)
    - [Phase separation](#phase-separation)
      - [Microphase separation](#microphase-separation)
        - [Lamellar microphase](#lamellar-microphase)
        - [Hexagonal cylinder block-copolymer phase](#hexagonal-cylinder-block-copolymer-phase)
        - [Block-copolymer sphere phase](#block-copolymer-sphere-phase)
        - [Order-disorder transition in block copolymers](#order-disorder-transition-in-block-copolymers)
        - [Hexagonally perforated layer phase](#hexagonally-perforated-layer-phase)
        - [Double gyroid](#double-gyroid)
      - [Biomolecular phase separation](#biomolecular-phase-separation)
    - [Pure thermodynamic phase](#pure-thermodynamic-phase)
    - [Common-tangent construction for phase coexistence](#common-tangent-construction-for-phase-coexistence)
      - [Linear composition bias leaves coexistence compositions unchanged](#linear-composition-bias-leaves-coexistence-compositions-unchanged)
    - [Vapor-liquid equilibrium](#vapor-liquid-equilibrium)
  - [Continuous phase transition](#continuous-phase-transition)
  - [Vaporization](#vaporization)
    - [Enthalpy of vaporization](#enthalpy-of-vaporization)
    - [Evaporation](#evaporation)
      - [Coffee-ring effect](#coffee-ring-effect)
    - [Boiling](#boiling)
      - [Critical heat flux](#critical-heat-flux)
        - [Departure from nucleate boiling](#departure-from-nucleate-boiling)
          - [Departure from nucleate boiling ratio](#departure-from-nucleate-boiling-ratio)
            - [Minimum departure from nucleate boiling ratio](#minimum-departure-from-nucleate-boiling-ratio)
      - [Boiling chip](#boiling-chip)
- [Critical exponent](#critical-exponent)
  - [Field crossover exponent](#field-crossover-exponent)
  - [Percolation critical exponents](#percolation-critical-exponents)
    - [Mean-field percolation exponents](#mean-field-percolation-exponents)
    - [Percolation cluster fractal dimension](#percolation-cluster-fractal-dimension)
    - [Percolation cluster-size tail exponent](#percolation-cluster-size-tail-exponent)
    - [Percolation order-parameter exponent](#percolation-order-parameter-exponent)
  - [Reduced temperature](#reduced-temperature)
  - [Heat-capacity critical exponent](#heat-capacity-critical-exponent)
  - [Order-parameter critical exponent](#order-parameter-critical-exponent)
  - [Magnetic-susceptibility critical exponent](#magnetic-susceptibility-critical-exponent)
  - [Critical-isotherm exponent](#critical-isotherm-exponent)
  - [Correlation-length critical exponent](#correlation-length-critical-exponent)
- [Critical dimension (phase transition)](#critical-dimension-phase-transition)
- [Lower critical dimension](#lower-critical-dimension)
  - [Berezinskii–Kosterlitz–Thouless transition](#berezinskii-kosterlitz-thouless-transition)
    - [Single-vortex energy-entropy balance](#single-vortex-energy-entropy-balance)
    - [Vortex-pair renormalization flow](#vortex-pair-renormalization-flow)
      - [Finite-scale vortex renormalization](#finite-scale-vortex-renormalization)
    - [Universal stiffness jump](#universal-stiffness-jump)
    - [Vortex-antivortex binding](#vortex-antivortex-binding)
    - [Quasi-long-range order](#quasi-long-range-order)
    - [Vortex-unbinding crossover in a trapped atomic gas](#vortex-unbinding-crossover-in-a-trapped-atomic-gas)
- [Correlation function](#correlation-function)
  - [Four-point correlation function](#four-point-correlation-function)
  - [One-point correlation function](#one-point-correlation-function)
  - [Connected correlation function](#connected-correlation-function)
    - [Correlation-function susceptibility sum rule](#correlation-function-susceptibility-sum-rule)
      - [Spin-mixture contribution to zero-field susceptibility](#spin-mixture-contribution-to-zero-field-susceptibility)
    - [Inverse Hessian relation for a connected two-point function](#inverse-hessian-relation-for-a-connected-two-point-function)
    - [Amputated connected correlation function](#amputated-connected-correlation-function)
  - [Two-point correlation function](#two-point-correlation-function)
  - [Dynamic structure factor](#dynamic-structure-factor)
    - [Static structure factor](#static-structure-factor)
      - [Polymer scattering function](#polymer-scattering-function)
        - [Guinier expansion of a polymer scattering function](#guinier-expansion-of-a-polymer-scattering-function)
  - [Correlation length](#correlation-length)
    - [Correlation volume](#correlation-volume)
    - [Landau scalar correlation length](#landau-scalar-correlation-length)
- [Order parameter](#order-parameter)
  - [Order-parameter phase](#order-parameter-phase)
  - [Off-diagonal long-range order](#off-diagonal-long-range-order)
  - [Field conjugate to an order parameter](#field-conjugate-to-an-order-parameter)
  - [Vector order parameter](#vector-order-parameter)
  - [Conserved order parameter](#conserved-order-parameter)
  - [Topological defect](#topological-defect)
    - [Homotopy classification of cosmological defects](#homotopy-classification-of-cosmological-defects)
    - [Cosmological texture](#cosmological-texture)
    - [Nematic hedgehog defect](#nematic-hedgehog-defect)
      - [Hyperbolic hedgehog defect](#hyperbolic-hedgehog-defect)
    - [Boojum](#boojum)
    - [Kibble mechanism](#kibble-mechanism)
    - [Domain wall](#domain-wall)
      - [Horizon-scaling domain wall network](#horizon-scaling-domain-wall-network)
      - [Scalar quartic domain wall](#scalar-quartic-domain-wall)
    - [Phase vortex](#phase-vortex)
      - [Compact phase sectors](#compact-phase-sectors)
      - [Quantum vortex](#quantum-vortex)
        - [Stirred-condensate vortex experiment](#stirred-condensate-vortex-experiment)
        - [Inverse-square tail of a Gross–Pitaevskii vortex](#inverse-square-tail-of-a-gross-pitaevskii-vortex)
        - [Matched vortex energy in a parabolic condensate](#matched-vortex-energy-in-a-parabolic-condensate)
        - [Cubic-quintic quantum vortex tail](#cubic-quintic-quantum-vortex-tail)
        - [Constant far-field phase excludes net vortex winding](#constant-far-field-phase-excludes-net-vortex-winding)
        - [Thermodynamic vortex-nucleation frequency](#thermodynamic-vortex-nucleation-frequency)
        - [Quantized circulation](#quantized-circulation)
          - [Phase winding of a condensate](#phase-winding-of-a-condensate)
            - [Superfluid phase slip](#superfluid-phase-slip)
  - [Quench (statistical physics)](#quench-statistical-physics)
  - [Liquid crystal](#liquid-crystal)
    - [Blue phase](#blue-phase)
    - [Columnar liquid crystal](#columnar-liquid-crystal)
    - [Isotropic phase](#isotropic-phase)
    - [Polar liquid crystal](#polar-liquid-crystal)
    - [Nematic liquid crystal](#nematic-liquid-crystal)
      - [Planar anchoring](#planar-anchoring)
      - [Homeotropic anchoring](#homeotropic-anchoring)
      - [Cholesteric liquid crystal](#cholesteric-liquid-crystal)
      - [Onsager excluded-volume mechanism](#onsager-excluded-volume-mechanism)
      - [Twisted nematic field effect](#twisted-nematic-field-effect)
        - [Adiabatic optical following in a twisted nematic](#adiabatic-optical-following-in-a-twisted-nematic)
      - [Fréedericksz transition](#freedericksz-transition)
        - [Quarter-turn nematic instability threshold](#quarter-turn-nematic-instability-threshold)
      - [Dielectric anisotropy of a nematic](#dielectric-anisotropy-of-a-nematic)
      - [Nematic director](#nematic-director)
        - [Independent head-tail reversal symmetry](#independent-head-tail-reversal-symmetry)
        - [Distortion free energy density](#distortion-free-energy-density)
          - [One-dimensional twisted nematic energy](#one-dimensional-twisted-nematic-energy)
          - [Nematic bend](#nematic-bend)
          - [Nematic twist](#nematic-twist)
          - [Nematic splay](#nematic-splay)
        - [Nematic disclination](#nematic-disclination)
          - [Saturn-ring defect](#saturn-ring-defect)
          - [Nematic defect-antidefect annihilation](#nematic-defect-antidefect-annihilation)
          - [Logarithmic energy of a planar nematic disclination](#logarithmic-energy-of-a-planar-nematic-disclination)
            - [Energetic fission of an integer nematic disclination](#energetic-fission-of-an-integer-nematic-disclination)
          - [Tangential integer nematic defect core](#tangential-integer-nematic-defect-core)
          - [Topological charge of a two-dimensional nematic disclination](#topological-charge-of-a-two-dimensional-nematic-disclination)
          - [Escape into the third dimension](#escape-into-the-third-dimension)
        - [One-elastic-constant nematic free energy](#one-elastic-constant-nematic-free-energy)
          - [Planar nematic divergence-elasticity identity](#planar-nematic-divergence-elasticity-identity)
      - [Nematic order parameter](#nematic-order-parameter)
        - [Small-angle width of nematic orientation](#small-angle-width-of-nematic-orientation)
        - [Effective orientation angle from nematic order](#effective-orientation-angle-from-nematic-order)
        - [Uniaxial nematic order](#uniaxial-nematic-order)
          - [Physical range of a uniaxial nematic order parameter](#physical-range-of-a-uniaxial-nematic-order-parameter)
        - [Rotational invariant of a symmetric traceless tensor](#rotational-invariant-of-a-symmetric-traceless-tensor)
        - [Landau-de Gennes free energy](#landau-de-gennes-free-energy)
          - [Electric-field coupling to nematic order](#electric-field-coupling-to-nematic-order)
            - [Field-induced critical endpoint of the isotropic-nematic transition](#field-induced-critical-endpoint-of-the-isotropic-nematic-transition)
    - [Director (liquid crystals)](#director-liquid-crystals)
  - [Nonconserved order-parameter dynamics](#nonconserved-order-parameter-dynamics)
    - [Gaussian Model A impulse response](#gaussian-model-a-impulse-response)
    - [Kinetic coefficient](#kinetic-coefficient)
    - [Onsager--Machlup path probability for Model A dynamics](#onsager-machlup-path-probability-for-model-a-dynamics)
    - [Onsager--Machlup path probability](#onsager-machlup-path-probability)
      - [Onsager–Machlup functional](#onsager-machlup-functional)
      - [Time-reversal invariance of a path Jacobian](#time-reversal-invariance-of-a-path-jacobian)
    - [Model A fluctuation-dissipation relation](#model-a-fluctuation-dissipation-relation)
    - [Gaussian Model A quench](#gaussian-model-a-quench)
  - [Conserved order-parameter dynamics](#conserved-order-parameter-dynamics)
    - [Order-parameter mobility](#order-parameter-mobility)
    - [Fluctuation-dissipation relation for a conserved flux](#fluctuation-dissipation-relation-for-a-conserved-flux)
    - [Hydrodynamic mode](#hydrodynamic-mode)
  - [Mixed conserved and nonconserved order-parameter dynamics](#mixed-conserved-and-nonconserved-order-parameter-dynamics)
    - [Joint path probability of an order parameter and its flux](#joint-path-probability-of-an-order-parameter-and-its-flux)
  - [Compositional order parameter](#compositional-order-parameter)
    - [Binary fluid mixture](#binary-fluid-mixture)
      - [Surfactant renormalization of the square-gradient coefficient](#surfactant-renormalization-of-the-square-gradient-coefficient)
      - [Microemulsion](#microemulsion)
      - [Cahn--Hilliard equation](#cahn-hilliard-equation)
      - [Ostwald ripening](#ostwald-ripening)
        - [Diffusion-controlled droplet growth](#diffusion-controlled-droplet-growth)
          - [Constant-reservoir diffusion-controlled particle growth](#constant-reservoir-diffusion-controlled-particle-growth)
            - [Surface-reaction-controlled particle growth](#surface-reaction-controlled-particle-growth)
          - [Diffusion-capacitance analogy](#diffusion-capacitance-analogy)
          - [Droplet evaporation near a planar reservoir](#droplet-evaporation-near-a-planar-reservoir)
      - [Model H dynamics](#model-h-dynamics)
        - [Energy dissipation identity for Model H](#energy-dissipation-identity-for-model-h)
        - [Korteweg force](#korteweg-force)
        - [Bicontinuous phase separation](#bicontinuous-phase-separation)
          - [Dynamical scaling of binary-fluid coarsening](#dynamical-scaling-of-binary-fluid-coarsening)
            - [Drag-limited hydrodynamic coarsening](#drag-limited-hydrodynamic-coarsening)
            - [Hydrodynamic coarsening crossover scales](#hydrodynamic-coarsening-crossover-scales)
            - [Viscous hydrodynamic coarsening](#viscous-hydrodynamic-coarsening)
            - [Inertial hydrodynamic coarsening](#inertial-hydrodynamic-coarsening)
            - [Stirring-arrested binary-fluid domain size](#stirring-arrested-binary-fluid-domain-size)
  - [Polar order parameter](#polar-order-parameter)
    - [Polar molecular field](#polar-molecular-field)
    - [Flow alignment of a polar order parameter](#flow-alignment-of-a-polar-order-parameter)
      - [Tumbling of a polar order parameter](#tumbling-of-a-polar-order-parameter)
      - [Flow-alignment angle in planar shear](#flow-alignment-angle-in-planar-shear)
      - [Order-parameter stress](#order-parameter-stress)
        - [Reversible stress of a polar liquid crystal](#reversible-stress-of-a-polar-liquid-crystal)
- [Landau theory](#landau-theory)
  - [Arrott plot](#arrott-plot)
    - [Extracting magnetic Landau coefficients from an Arrott plot](#extracting-magnetic-landau-coefficients-from-an-arrott-plot)
  - [Ginzburg-Landau theory](#ginzburg-landau-theory)
    - [Ginzburg-Landau functional of a dilute Bose gas](#ginzburg-landau-functional-of-a-dilute-bose-gas)
  - [Quartic Landau equilibrium branches](#quartic-landau-equilibrium-branches)
  - [Sign-reversal symmetry in Landau theory](#sign-reversal-symmetry-in-landau-theory)
  - [Analytic vector Landau expansion](#analytic-vector-landau-expansion)
  - [Heat-capacity jump in quartic Landau theory](#heat-capacity-jump-in-quartic-landau-theory)
    - [Curie heat-capacity density from an Arrott plot](#curie-heat-capacity-density-from-an-arrott-plot)
  - [Mean-field approximation](#mean-field-approximation)
    - [Self-consistency equation](#self-consistency-equation)
  - [Landau free energy](#landau-free-energy)
    - [Helical minimum of a complex Landau functional](#helical-minimum-of-a-complex-landau-functional)
    - [Constrained order-parameter boundary stability](#constrained-order-parameter-boundary-stability)
    - [Temperature-dependent cubic-quartic Landau free energy](#temperature-dependent-cubic-quartic-landau-free-energy)
      - [Thermal symmetry nonrestoration in a cubic-quartic model](#thermal-symmetry-nonrestoration-in-a-cubic-quartic-model)
      - [Latent heat of a temperature-dependent cubic-quartic Landau transition](#latent-heat-of-a-temperature-dependent-cubic-quartic-landau-transition)
    - [O(3) quartic Landau minima](#o-3-quartic-landau-minima)
    - [Constrained order-parameter free energy](#constrained-order-parameter-free-energy)
      - [Zero-cutoff identification of constrained free energy](#zero-cutoff-identification-of-constrained-free-energy)
    - [First-order transition in a cubic-quartic Landau potential](#first-order-transition-in-a-cubic-quartic-landau-potential)
      - [Coexistence barrier of a cubic-quartic Landau transition](#coexistence-barrier-of-a-cubic-quartic-landau-transition)
      - [Bounded quartic nematic coexistence](#bounded-quartic-nematic-coexistence)
    - [Critical endpoint of a quartic Landau free energy](#critical-endpoint-of-a-quartic-landau-free-energy)
    - [Cubic-term removal in a conserved quartic Landau free energy](#cubic-term-removal-in-a-conserved-quartic-landau-free-energy)
    - [Multicritical even Landau potential](#multicritical-even-landau-potential)
    - [Sextic even Landau potential](#sextic-even-landau-potential)
    - [Equilibrium magnetization](#equilibrium-magnetization)
    - [Spinodal](#spinodal)
      - [Spinodal decomposition](#spinodal-decomposition)
      - [Spinodal point](#spinodal-point)
        - [Hysteresis spinodals of a scalar quartic potential](#hysteresis-spinodals-of-a-scalar-quartic-potential)
    - [Metastability](#metastability)
      - [Supersaturated vapor](#supersaturated-vapor)
        - [Atmospheric supersaturation](#atmospheric-supersaturation)
      - [Nucleation](#nucleation)
        - [Burst nucleation](#burst-nucleation)
        - [La Mer diagram](#la-mer-diagram)
        - [Heterogeneous nucleation](#heterogeneous-nucleation)
          - [Deposition nucleation](#deposition-nucleation)
          - [Contact freezing](#contact-freezing)
          - [Immersion freezing](#immersion-freezing)
        - [Homogeneous nucleation](#homogeneous-nucleation)
          - [Homogeneous ice nucleation](#homogeneous-ice-nucleation)
      - [Hysteresis](#hysteresis)
        - [Magnetic hysteresis](#magnetic-hysteresis)
        - [Magnetic coercivity](#magnetic-coercivity)
      - [Superheating](#superheating)
        - [Superheated liquid](#superheated-liquid)
        - [Constitutional superheating](#constitutional-superheating)
      - [Supercooling](#supercooling)
    - [Common-tangent construction](#common-tangent-construction)
      - [Binodal](#binodal)
        - [Saturation concentration](#saturation-concentration)
  - [Landau-Ginzburg theory](#landau-ginzburg-theory)
    - [Square-gradient theory of a liquid interface](#square-gradient-theory-of-a-liquid-interface)
    - [Scalar-field source Legendre transform](#scalar-field-source-legendre-transform)
    - [Landau approximation](#landau-approximation)
    - [Two-component radial quartic Landau potential](#two-component-radial-quartic-landau-potential)
    - [Local derivative expansion](#local-derivative-expansion)
      - [Canonical normalization of a scalar gradient term](#canonical-normalization-of-a-scalar-gradient-term)
    - [Gradient energy](#gradient-energy)
    - [Gradient expansion](#gradient-expansion)
    - [Interfacial tension](#interfacial-tension)
    - [Phi-four diffuse interface](#phi-four-diffuse-interface)
      - [Interfacial tension of a phi-four diffuse interface](#interfacial-tension-of-a-phi-four-diffuse-interface)
    - [Gaussian field theory](#gaussian-field-theory)
      - [Ordered-phase obstruction in a Gaussian scalar model](#ordered-phase-obstruction-in-a-gaussian-scalar-model)
      - [Massive Gaussian field correlation tail](#massive-gaussian-field-correlation-tail)
      - [Positive-wavevector sum for a real field](#positive-wavevector-sum-for-a-real-field)
      - [Gaussian variational approximation](#gaussian-variational-approximation)
        - [Gaussian variational kernel for a gradient quartic interaction](#gaussian-variational-kernel-for-a-gradient-quartic-interaction)
        - [Gibbs--Bogoliubov--Feynman inequality](#gibbs-bogoliubov-feynman-inequality)
    - [Brazovskii model](#brazovskii-model)
      - [Gradient-quartic Brazovskii model](#gradient-quartic-brazovskii-model)
        - [Single-mode smectic mean-field free energy](#single-mode-smectic-mean-field-free-energy)
      - [Nonzero-wavevector soft-mode sphere](#nonzero-wavevector-soft-mode-sphere)
        - [Soft-mode shell integral](#soft-mode-shell-integral)
      - [Brazovskii fluctuation-induced first-order transition](#brazovskii-fluctuation-induced-first-order-transition)
    - [Smectic phase](#smectic-phase)
      - [Smectic C phase](#smectic-c-phase)
      - [Smectic A phase](#smectic-a-phase)
      - [Polar helical smectic](#polar-helical-smectic)
    - [Ginzburg criterion](#ginzburg-criterion)
      - [Ginzburg reduced-temperature window](#ginzburg-reduced-temperature-window)
      - [Correlation-volume derivation of the scalar Ginzburg ratio](#correlation-volume-derivation-of-the-scalar-ginzburg-ratio)
      - [Critical region of a phase transition](#critical-region-of-a-phase-transition)
      - [One-loop critical-mass subtraction](#one-loop-critical-mass-subtraction)
        - [Infrared asymptotics of the critical-mass subtraction](#infrared-asymptotics-of-the-critical-mass-subtraction)
          - [Radial critical-mass subtraction in dimensions three to five](#radial-critical-mass-subtraction-in-dimensions-three-to-five)
      - [Marginal Ginzburg criterion](#marginal-ginzburg-criterion)
      - [Multicritical Ginzburg ratio](#multicritical-ginzburg-ratio)
    - [Gaussian fluctuation correction near a critical point](#gaussian-fluctuation-correction-near-a-critical-point)
      - [Ornstein--Zernike correlation function](#ornstein-zernike-correlation-function)
  - [Mean-field critical exponent](#mean-field-critical-exponent)
  - [Tricritical point](#tricritical-point)
    - [Mean-field tricritical exponent calculation](#mean-field-tricritical-exponent-calculation)
      - [Tricritical heat-capacity amplitude in a sextic Landau expansion](#tricritical-heat-capacity-amplitude-in-a-sextic-landau-expansion)
    - [Tricritical wing](#tricritical-wing)
      - [Tricritical three-phase line](#tricritical-three-phase-line)
      - [Tricritical wing coexistence factorization](#tricritical-wing-coexistence-factorization)
      - [Tricritical wing critical edge](#tricritical-wing-critical-edge)
    - [Tricritical crossover scaling](#tricritical-crossover-scaling)
      - [Large-quartic asymptotic of tricritical scaling](#large-quartic-asymptotic-of-tricritical-scaling)
    - [Tricritical sextic beta function](#tricritical-sextic-beta-function)
- [Upper critical dimension](#upper-critical-dimension)
  - [Upper critical dimension of percolation](#upper-critical-dimension-of-percolation)
  - [Upper critical dimension of an even scalar interaction](#upper-critical-dimension-of-an-even-scalar-interaction)
- [Renormalization group](#renormalization-group)
  - [Block-spin coarse-graining](#block-spin-coarse-graining)
  - [Integrating and rescaling a statistical model](#integrating-and-rescaling-a-statistical-model)
  - [A solvable infrared renormalization flow](#a-solvable-infrared-renormalization-flow)
  - [Correlation-length scaling from a thermal direction](#correlation-length-scaling-from-a-thermal-direction)
  - [Why microscopic differences fade near criticality](#why-microscopic-differences-fade-near-criticality)
  - [Ultraviolet fixed point](#ultraviolet-fixed-point)
    - [Two-point scaling at an ultraviolet fixed point](#two-point-scaling-at-an-ultraviolet-fixed-point)
  - [Anisotropic renormalization group](#anisotropic-renormalization-group)
    - [Anisotropic Gaussian smectic scaling](#anisotropic-gaussian-smectic-scaling)
    - [Anisotropic effective dimension](#anisotropic-effective-dimension)
  - [Renormalization-group transformation](#renormalization-group-transformation)
    - [Additive free-energy recursion under blocking](#additive-free-energy-recursion-under-blocking)
    - [Blocking kernel](#blocking-kernel)
  - [Real-space renormalization group](#real-space-renormalization-group)
    - [Migdal-Kadanoff approximation](#migdal-kadanoff-approximation)
      - [Bond moving](#bond-moving)
    - [Normalized blocking kernel](#normalized-blocking-kernel)
      - [Identity-operator contribution to renormalization-group free energy](#identity-operator-contribution-to-renormalization-group-free-energy)
        - [Analytic subtraction of an inhomogeneous renormalization recursion](#analytic-subtraction-of-an-inhomogeneous-renormalization-recursion)
          - [Renormalization-group free-energy resonance](#renormalization-group-free-energy-resonance)
    - [Reciprocal coordinate at infinite coupling](#reciprocal-coordinate-at-infinite-coupling)
    - [Spin decimation](#spin-decimation)
      - [Exact zero-field Ising-chain decimation](#exact-zero-field-ising-chain-decimation)
        - [Finite-field Ising-chain decimation](#finite-field-ising-chain-decimation)
        - [Domain-wall scaling coordinate of an Ising chain](#domain-wall-scaling-coordinate-of-an-ising-chain)
        - [Ising-chain decimation constant](#ising-chain-decimation-constant)
      - [Checkerboard decimation of the square-lattice Ising model](#checkerboard-decimation-of-the-square-lattice-ising-model)
        - [Leading checkerboard Ising decimation recursion](#leading-checkerboard-ising-decimation-recursion)
      - [Spin-1 chain decimation recursion](#spin-1-chain-decimation-recursion)
  - [Momentum-shell renormalization group](#momentum-shell-renormalization-group)
    - [Wilsonian coarse-grained statistical Hamiltonian](#wilsonian-coarse-grained-statistical-hamiltonian)
    - [One-loop shell quartic renormalization](#one-loop-shell-quartic-renormalization)
    - [One-loop shell mass renormalization in scalar quartic theory](#one-loop-shell-mass-renormalization-in-scalar-quartic-theory)
    - [Gaussian shell covariance](#gaussian-shell-covariance)
    - [Quartic interaction generated by a sextic interaction](#quartic-interaction-generated-by-a-sextic-interaction)
    - [Cumulant expansion of a coarse-grained free energy](#cumulant-expansion-of-a-coarse-grained-free-energy)
  - [Engineering dimension](#engineering-dimension)
    - [Anomalous dimension](#anomalous-dimension)
      - [Field-renormalization anomalous dimension](#field-renormalization-anomalous-dimension)
      - [Field scaling and anomalous dimension](#field-scaling-and-anomalous-dimension)
  - [Renormalization-group flow](#renormalization-group-flow)
    - [Repulsive renormalization-group trajectory](#repulsive-renormalization-group-trajectory)
    - [Renormalization-group fixed point](#renormalization-group-fixed-point)
      - [Infrared fixed point](#infrared-fixed-point)
      - [Stability matrix of a renormalization-group fixed point](#stability-matrix-of-a-renormalization-group-fixed-point)
      - [Critical surface](#critical-surface)
  - [Gaussian fixed point](#gaussian-fixed-point)
    - [Gaussian critical exponent](#gaussian-critical-exponent)
      - [Gaussian free-energy logarithms at integer singular powers](#gaussian-free-energy-logarithms-at-integer-singular-powers)
      - [Gaussian order-parameter scaling index](#gaussian-order-parameter-scaling-index)
      - [Gaussian specific-heat infrared threshold](#gaussian-specific-heat-infrared-threshold)
    - [Gaussian momentum-shell scaling](#gaussian-momentum-shell-scaling)
      - [Gaussian free-energy scaling relation](#gaussian-free-energy-scaling-relation)
        - [Gaussian free-energy logarithm at effective dimension two](#gaussian-free-energy-logarithm-at-effective-dimension-two)
  - [Wilson-Fisher fixed point](#wilson-fisher-fixed-point)
    - [Thermal relevant direction at the Wilson-Fisher fixed point](#thermal-relevant-direction-at-the-wilson-fisher-fixed-point)
    - [O(N) model](#o-n-model)
    - [Epsilon expansion](#epsilon-expansion)
      - [Coupled Ising fixed points near four dimensions](#coupled-ising-fixed-points-near-four-dimensions)
        - [Field-rotation equivalence of decoupled Ising theories](#field-rotation-equivalence-of-decoupled-ising-theories)
  - [Renormalization-group relevance](#renormalization-group-relevance)
    - [Relevant operator](#relevant-operator)
      - [Relevant direction of a fixed point](#relevant-direction-of-a-fixed-point)
        - [Thermal exponent from a discrete renormalization map](#thermal-exponent-from-a-discrete-renormalization-map)
    - [Irrelevant operator](#irrelevant-operator)
    - [Marginal operator](#marginal-operator)
      - [Marginally irrelevant operator](#marginally-irrelevant-operator)
  - [Universality class](#universality-class)
    - [Universal singular free-energy amplitude ratio](#universal-singular-free-energy-amplitude-ratio)
    - [Universal specific-heat amplitude ratio](#universal-specific-heat-amplitude-ratio)
    - [Percolation universality hypothesis](#percolation-universality-hypothesis)
  - [Dangerously irrelevant coupling](#dangerously-irrelevant-coupling)
- [Scaling relation for critical exponents](#scaling-relation-for-critical-exponents)
  - [Exponent inference from a magnetic data collapse](#exponent-inference-from-a-magnetic-data-collapse)
  - [Fisher scaling relation](#fisher-scaling-relation)
    - [Matching the amplitude of a massive critical correlation tail](#matching-the-amplitude-of-a-massive-critical-correlation-tail)
  - [Scaling hypothesis for critical phenomena](#scaling-hypothesis-for-critical-phenomena)
    - [Magnetization scaling-function matching](#magnetization-scaling-function-matching)
    - [Mean-field scalar free-energy scaling](#mean-field-scalar-free-energy-scaling)
  - [Widom scaling relation](#widom-scaling-relation)
  - [Rushbrooke scaling relation](#rushbrooke-scaling-relation)
  - [Hyperscaling relation](#hyperscaling-relation)
- [Goldstone boson](#goldstone-boson)
  - [Type-B Goldstone boson](#type-b-goldstone-boson)
  - [Goldstone-mode effective free energy](#goldstone-mode-effective-free-energy)
    - [Phase stiffness](#phase-stiffness)
    - [Phase-difference variance](#phase-difference-variance)
      - [Infrared-regulated phase covariance](#infrared-regulated-phase-covariance)
      - [Infrared spin-wave correlations of the XY model](#infrared-spin-wave-correlations-of-the-xy-model)
    - [Spin wave](#spin-wave)
      - [Magnon](#magnon)
        - [Triplon](#triplon)
      - [Linear spin-wave approximation](#linear-spin-wave-approximation)
        - [Isotropic spin-wave vacuum energy comparison](#isotropic-spin-wave-vacuum-energy-comparison)
        - [Full-zone antiferromagnetic Nambu counting](#full-zone-antiferromagnetic-nambu-counting)
        - [Heisenberg-chain spin-wave comparison](#heisenberg-chain-spin-wave-comparison)
        - [Easy-plane XXZ antiferromagnetic spin-wave spectrum](#easy-plane-xxz-antiferromagnetic-spin-wave-spectrum)
        - [Easy-axis XXZ antiferromagnetic spin-wave spectrum](#easy-axis-xxz-antiferromagnetic-spin-wave-spectrum)
  - [Mermin-Wagner theorem](#mermin-wagner-theorem)

## Universality of critical phenomena

↑ **Parent:** [Critical phenomenon](critical-phenomenon.md)

[Universality](#universality-of-critical-phenomena) of critical phenomena is the agreement of critical exponents or normalized scaling forms between microscopically different systems. Dimension, symmetry and interaction range help determine the universality class. A [renormalization-group flow](#renormalization-group-flow) can explain this agreement by showing that different microscopic models approach the same fixed-point description, while irrelevant differences fade at large scales.

## Thermodynamic critical point

↑ **Parent:** [Critical phenomenon](critical-phenomenon.md)

At an ordinary thermodynamic critical point, two coexisting phases become indistinguishable: their [order parameter](#order-parameter) difference vanishes, and the [correlation length](#correlation-length) and appropriate response functions typically diverge. A [continuous phase transition](#continuous-phase-transition) can be approached there by tuning the thermal and conjugate-field variables. A [renormalization-group fixed point](#renormalization-group-fixed-point) controls its singular long-distance behavior. A triple point with three separated minima is not an ordinary thermodynamic critical point, and a [tricritical point](#tricritical-point) requires an additional tuning and has a different scaling theory.

### Critical point of a cubic density equation of state

↑ **Parent:** [Thermodynamic critical point](#thermodynamic-critical-point)

For $p=nk_BT-bn^2/2+cn^3/6$ with $b,c>0$, the first two density derivatives vanish at $n_c=b/c$, $k_BT_c=b^2/(2c)$ and $p_c=b^3/(6c^2)$. The scaled equation is $p/p_c=x^3-3x^2+3tx$, with $x=n/n_c$ and $t=T/T_c$.

#### Spinodal densities of a cubic gas

↑ **Parent:** [Critical point of a cubic density equation of state](#critical-point-of-a-cubic-density-equation-of-state)

### Critical concentration

↑ **Parent:** [Thermodynamic critical point](#thermodynamic-critical-point)

The composition coordinate at the critical endpoint where coexisting phases become identical. Its value depends on the system and control parameters.

## Lifshitz point

↑ **Parent:** [Critical phenomenon](critical-phenomenon.md)

A multicritical point where disordered, spatially uniform ordered and spatially modulated phases meet. The quadratic stiffness in one or more directions vanishes, so a positive higher-derivative term stabilises the [Landau-Ginzburg theory](#landau-ginzburg-theory). For a uniaxial case the kernel at the point has $p_\perp^2+p_\parallel^4$, with the coefficient of $p_\parallel^2$ tuned to zero.

### Uniaxial Lifshitz Gaussian renormalization

↑ **Parent:** [Lifshitz point](#lifshitz-point)

For kernel $\kappa^{-1}p_\perp^2+\mu^{-1}p_\parallel^4+m^2$ with positive stiffnesses, preserve both derivative coefficients by $q_\perp=bp_\perp$ and $q_\parallel=b^{1/2}p_\parallel$. The Fourier field multiplier is $\widetilde Z=b^{(2D+3)/4}$, the mass becomes $bm$, and a uniform source becomes $b^{(2D+3)/4}h$. The [anisotropic effective dimension](#anisotropic-effective-dimension) is $D-1/2$ and the Gaussian exponents are $\alpha=9/4-D/2$, $\Delta=(2D+3)/8$.

## Liquid-gas critical point

↑ **Parent:** [Critical phenomenon](critical-phenomenon.md)

The endpoint of a gas-liquid [phase coexistence curve](thermodynamic-potential.md#phase-coexistence-curve), where the distinct liquid and gas states merge. For a smooth fluid [equation of state](pressure.md#equation-of-state), the critical isotherm has $p_v=p_{vv}=0$ at this point; this thermodynamic meaning differs from a stationary [critical point](analysis.md#critical-point) of an arbitrary function.

### Supercritical fluid

↑ **Parent:** [Liquid-gas critical point](#liquid-gas-critical-point)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Supercritical_fluid)

## Quantum critical point

↑ **Parent:** [Critical phenomenon](critical-phenomenon.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_critical_point)

A quantum critical point is a continuous zero-temperature phase transition driven by a nonthermal control parameter. Quantum and thermal fluctuations near it are organized by a dynamical critical exponent.

### Quantum-critical regime

↑ **Parent:** [Quantum critical point](#quantum-critical-point)

The quantum-critical regime is the finite-temperature region in which temperature exceeds the energy scale generated by detuning from a quantum critical point. Temperature then controls leading masses, relaxation rates, and correlation lengths.

### Quantum critical scaling

↑ **Parent:** [Quantum critical point](#quantum-critical-point)

Quantum critical scaling expresses observables as powers of temperature or detuning times universal functions of dimensionless ratios such as $\omega/T$, $vk/T$, and $\Delta/T$.

#### Dynamical critical exponent

↑ **Parent:** [Quantum critical scaling](#quantum-critical-scaling)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dynamical_critical_exponent)

The dynamical critical exponent relates critical frequency and wavenumber scales by $\omega\sim k^z$. Relativistic critical theories have $z=1$.

## Phase transition

↑ **Parent:** [Critical phenomenon](critical-phenomenon.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Phase_transition)

A phase transition is a nonanalytic change in equilibrium behavior as a thermodynamic control parameter varies. A continuous phase transition has a diverging [correlation length](#correlation-length) and no latent heat.

### Crystallization

↑ **Parent:** [Phase transition](#phase-transition)

Formation of a [crystal](thermodynamics.md#crystal) from a disordered phase. In a cooling [white dwarf](stellar-astrophysics.md#white-dwarf), [crystallization](#crystallization) of the ionic interior releases latent heat and can redistribute chemical species, affecting the relation between [luminosity](astrophysics.md#luminosity) and [white-dwarf cooling age](stellar-astrophysics.md#white-dwarf-cooling-age).

### Reconstructive transformation

↑ **Parent:** [Phase transition](#phase-transition)

A structural phase change requiring substantial rearrangement of near-neighbor bonding or connectivity. Its activation barriers can make equilibrium transitions kinetically sluggish. It is distinguished from a cooperative [displacive transformation](#displacive-transformation), rather than defined solely by the presence of a different final symmetry.

### Hexatic phase

↑ **Parent:** [Phase transition](#phase-transition)

A two-dimensional phase with quasi-long-range sixfold bond-orientational order but short-range translational order. A cell model of independent particle cages does not capture its full physics.

### Displacive transformation

↑ **Parent:** [Phase transition](#phase-transition)

A cooperative change of atomic positions and lattice shape without the long-range compositional [diffusion](thermodynamics.md#diffusion) required by a diffusional transformation. Tetragonal-to-monoclinic transformation in [zirconia](chemical-substance.md#zirconia) is a nonmetallic example.

### Vitrification

↑ **Parent:** [Phase transition](#phase-transition)

[vitrification](#vitrification) produces a noncrystalline glassy state. Rapid freezing of thin aqueous specimens is used to preserve hydrated biological structures for [cryo-electron microscopy](optics.md#cryo-electron-microscopy); vitrification does not prevent all subsequent [radiation damage](biology.md#radiation-damage).

### Metal-insulator transition

↑ **Parent:** [Phase transition](#phase-transition)

A change between a material behaving as an [electrical conductor](electric-charge.md#electrical-conductor) and as an [electrical insulator](permittivity.md#electrical-insulator). The distinction concerns the limiting electronic response as [temperature](temperature.md) tends to zero; finite thermally activated [electrical conductivity](electric-charge.md#electrical-conductivity) alone does not establish a metallic state. A [Peierls transition](quantum-ideal-gas-statistics.md#peierls-transition) opens a [band gap](bloch-s-theorem.md#band-gap) through a change in the [crystal structure](physical-chemistry.md#crystal-structure).

#### Mott criterion

↑ **Parent:** [Metal-insulator transition](#metal-insulator-transition)

The approximate donor metal-insulator threshold is often written $n_c^{1/3}a_B^*\simeq0.25$. It estimates when overlap and screening destroy isolated donor [localization](commutative-algebra.md#localization-of-a-ring). The numerical coefficient is empirical and not a universal exact result; disorder, compensation and anisotropy can shift the threshold.[Abstract and effective-radius scaling](physics-bibliography.md#the-mott-criterion-so-simple-and-yet-so-complex-by-alexander-pergament-and-others)

### Liquefaction of gases

↑ **Parent:** [Phase transition](#phase-transition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Liquefaction_of_gases)

Conversion of a [gas](thermodynamics.md#gas) to a [liquid](thermodynamics.md#liquid).

### Condensation

↑ **Parent:** [Phase transition](#phase-transition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Condensation)

Conversion of [vapor](thermodynamics.md#vapor) into [liquid](thermodynamics.md#liquid).

### Melting

↑ **Parent:** [Phase transition](#phase-transition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Melting)

[Melting](#melting) is a solid-to-liquid [phase transition](#phase-transition) that absorbs [latent heat](thermodynamic-potential.md#latent-heat). It can be driven by heating, changing phase pressures, or adding solute that causes [freezing-point depression](thermodynamic-potential.md#freezing-point-depression). The [ice layer between freshwater and cold brine](geophysics.md#ice-layer-between-freshwater-and-cold-brine) illustrates [melting](#melting) into a cold liquid through dilution and a composition-dependent [liquidus](thermodynamic-potential.md#liquidus).

### Freezing

↑ **Parent:** [Phase transition](#phase-transition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Freezing)

[Freezing](#freezing) is a liquid-to-solid [phase transition](#phase-transition). A moving [phase boundary](geophysics.md#phase-boundary) releases [latent heat](thermodynamic-potential.md#latent-heat); its rate is constrained by heat transport and the [Stefan condition](geophysics.md#stefan-condition). In a solution the [liquidus](thermodynamic-potential.md#liquidus) depends on composition, so being below the pure solvent's [melting](#melting) [temperature](temperature.md) does not imply that the solution must freeze.

#### Morphological instability of a solidification front

↑ **Parent:** [Freezing](#freezing)

A morphological instability amplifies shape perturbations of a [solidification](#freezing) interface. Protrusions may receive a larger diffusive supply or encounter larger undercooling, while [curvature-induced melting-temperature depression](surface-tension.md#curvature-induced-melting-temperature-depression) suppresses fine corrugations. Solute rejection can produce [constitutional supercooling](geophysics.md#constitutional-supercooling), destabilizing a planar front and leading to cells or [crystal dendrites](geophysics.md#dendrite-crystal).

### Quantum phase transition

↑ **Parent:** [Phase transition](#phase-transition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_phase_transition)

### Sublimation

↑ **Parent:** [Phase transition](#phase-transition)

A direct transition from a solid phase to a gaseous phase. Heated [interplanetary dust](planetary-science.md#interplanetary-dust) or a [comet](planetary-science.md#comet) can lose material through this process, changing its size and [radiation-pressure coefficient](planetary-science.md#radiation-pressure-coefficient) or destroying it before gravitational or drag-driven evolution is complete.

#### Sublimation-front capillary instability

↑ **Parent:** [Sublimation](#sublimation)

For a locally linear ice temperature with positive gradient $G$ into the solid, a corrugated [sublimation](#sublimation) front receives a perturbation in [heat flux](heat.md#heat-flux-density) proportional to its horizontal wavenumber $\alpha$. The [Gibbs-Thomson effect](surface-tension.md#gibbs-thomson-relation) suppresses short waves, giving the displayed quasi-static growth rate. It requires $V/(\kappa\alpha)\ll1$ and $|\sigma|/(\kappa\alpha^2)\ll1$, as well as a perturbation depth short enough for the linear background approximation. Unstable modes have $0<\alpha<\sqrt{G/\Gamma}$.

#### Radiatively heated sublimation profile

↑ **Parent:** [Sublimation](#sublimation)

For a sublimating surface with exponentially absorbed volumetric heating, use a frame moving into the solid at speed $V$. Its steady [heat equation](diffusion-equation.md#heat-equation) is $kT''+\rho c_pVT'+q_0e^{-\lambda z}=0$. The surface [Stefan condition](geophysics.md#stefan-condition) is $kT'(0)=\rho LV$. Integrating over the half-space gives the displayed energy-limited speed. The surface gradient is positive, but the far field is colder, so the temperature has a subsurface maximum where [melting](#melting) can begin.

#### Dust sublimation

↑ **Parent:** [Sublimation](#sublimation)

An irradiated grain loses solid material by [sublimation](#sublimation). Its lifetime depends strongly on temperature and composition. In a planetary [dust tail](planetary-science.md#dust-tail), a short lifetime can truncate the distribution well before a relative orbital wrap.

##### Blackbody dust sublimation radius

↑ **Parent:** [Dust sublimation](#dust-sublimation)

A spherical black grain of [radius](topology.md#radius) $a$ absorbs luminosity $L$ through projected area $\pi a^2$ and emits over $4\pi a^2$. Radiative balance at sublimation [temperature](temperature.md) gives $r_{\rm sub}=[L/(16\pi\sigma_{\rm SB}T_{\rm sub}^4)]^{1/2}$. Grain size cancels only under the stated unit-efficiency approximation; shielding and wavelength-dependent emissivity change the result.

###### Thermal stability of externally heated blackbody dust

↑ **Parent:** [Blackbody dust sublimation radius](#blackbody-dust-sublimation-radius)

At fixed irradiation, heating per grain is independent of [temperature](temperature.md) while cooling is proportional to $T^4$. With positive heat capacity and intact grains, a positive [temperature](temperature.md) perturbation increases net cooling, and a negative one increases net heating. Fixed dust properties and sufficient dust-[gas](thermodynamics.md#gas) thermal coupling are necessary assumptions.

###### Dust-destruction feedback at a sublimation front

↑ **Parent:** [Thermal stability of externally heated blackbody dust](#thermal-stability-of-externally-heated-blackbody-dust)

### Phase coexistence

↑ **Parent:** [Phase transition](#phase-transition)

Phase coexistence occurs when two or more thermodynamic phases have equal free energy under the same external conditions. A first-order transition crosses a coexistence locus, where the competing phases are simultaneously stable.

#### Ehrenfest entropy-continuity relation

↑ **Parent:** [Phase coexistence](#phase-coexistence)

If two equilibrium [phases](wave.md#phase-waves) have continuous [entropy](entropy.md) and [volume](geometry-and-topology.md#volume) but jumps in second derivatives of [Gibbs free energy](thermodynamic-potential.md#gibbs-free-energy), differentiate their [entropy](entropy.md) equality along the transition line. Since $dS=(C_P/T)dT-V\alpha_TdP$, one obtains the title slope, for nonzero $\Delta C_P$. Before imposing equal [volume](geometry-and-topology.md#volume), the numerator is $T\Delta(V\alpha_T)$. Equality of [Gibbs free energies](thermodynamic-potential.md#gibbs-free-energy) with equal [entropy](entropy.md) implies equal [volume](geometry-and-topology.md#volume) along a differentiable coexistence curve on which pressure varies. A constant-pressure curve or zero numerator and denominator needs separate analysis. This entropy-continuity condition is one Ehrenfest relation; [volume](geometry-and-topology.md#volume) continuity gives another independent relation.

#### Phase separation

↑ **Parent:** [Phase coexistence](#phase-coexistence)

A system can split into macroscopic regions with distinct local [order parameters](#order-parameter), densities or compositions. In a short-range system at [phase coexistence](#phase-coexistence), regions of two phases with means $M_1,M_2$ and volume fractions $q,1-q$ have spatial mean $M=qM_1+(1-q)M_2$. Their interface contribution is subextensive, so their thermodynamic [free-energy density](statistical-physics.md#free-energy-density) is the corresponding convex combination of the phase densities. This can lie below the homogeneous-branch [Landau free energy](#landau-free-energy) at the same $M$. The equilibrium [constrained order-parameter free energy](#constrained-order-parameter-free-energy) is consequently convexified, with a straight coexistence segment described by the [Maxwell construction](thermodynamic-potential.md#maxwell-construction). A nonconvex local potential remains useful for homogeneous branches, metastability and interfaces, but must not be identified with the full equilibrium constrained density throughout a coexistence interval.

##### Microphase separation

↑ **Parent:** [Phase separation](#phase-separation)

Formation of finite-scale composition domains when complete macroscopic separation is frustrated, for example by the covalent connection of incompatible blocks in a [diblock copolymer](polymer.md#diblock-copolymer). Interfacial cost and chain entropy jointly select the domain scale.

###### Lamellar microphase

↑ **Parent:** [Microphase separation](#microphase-separation)

Alternating sheet-like domains of the components of a microphase-separated material. In diblock systems the two layer thicknesses can be unequal and reflect unequal block fractions. Confinement, surface [wetting](surface-tension.md#wetting) and kinetic trapping can produce layered films outside the [thermodynamic equilibrium](thermodynamics.md#thermodynamic-equilibrium) bulk lamellar region.

###### Hexagonal cylinder block-copolymer phase

↑ **Parent:** [Microphase separation](#microphase-separation)

A microdomain pattern of approximately parallel cylinders arranged on a two-dimensional hexagonal lattice in the other block's matrix. It is conventionally labelled H in many diblock [phase diagrams](thermodynamic-potential.md#phase-diagram). Cylinder orientation and defects are additional properties beyond the local morphology.

###### Block-copolymer sphere phase

↑ **Parent:** [Microphase separation](#microphase-separation)

An ordered morphology in which a minority block forms approximately spherical domains in a continuous majority-block matrix. The lattice packing and phase stability depend on segregation strength, composition and chain statistics. The label S in a [phase diagram](thermodynamic-potential.md#phase-diagram) denotes a morphology, not a spherical shape of the entire specimen.

###### Order-disorder transition in block copolymers

↑ **Parent:** [Microphase separation](#microphase-separation)

The transition between a compositionally disordered state and an ordered microdomain state as effective segregation strength increases. The parameter $\chi N$ combines unlike-segment interaction preference and chain length; its transition value depends on composition and model assumptions. A bulk [thermodynamic equilibrium](thermodynamics.md#thermodynamic-equilibrium) boundary is not by itself an evaporation or [vitrification](#vitrification) kinetic model.

###### Hexagonally perforated layer phase

↑ **Parent:** [Microphase separation](#microphase-separation)

A domain structure resembling lamellae pierced by an ordered array of perforations. It is distinct from an unperforated lamellar phase and from a [double gyroid](#double-gyroid).

###### Double gyroid

↑ **Parent:** [Microphase separation](#microphase-separation)

A bicontinuous domain morphology containing two interpenetrating, nonintersecting networks of one component within the other. In [diblock copolymers](polymer.md#diblock-copolymer) it can appear between lamellar and cylindrical morphologies in part of the phase diagram.

##### Biomolecular phase separation

↑ **Parent:** [Phase separation](#phase-separation)

Separation of a biomolecular mixture into compositionally distinct phases. Concentration dependence, partitioning and reversibility should be tested; a fluorescent punctum or recovery after bleaching alone does not establish the mechanism.

#### Pure thermodynamic phase

↑ **Parent:** [Phase coexistence](#phase-coexistence)

A [pure thermodynamic phase](#pure-thermodynamic-phase) is an extremal equilibrium Gibbs state rather than a probabilistic mixture of distinct macroscopic phases. On an ordered Ising branch, taking the [thermodynamic limit](statistical-physics.md#thermodynamic-limit) before removing a selecting [conjugate field](#field-conjugate-to-an-order-parameter) gives a nonzero [magnetization](electromagnetism.md#magnetization). A symmetric mixture can instead have zero mean but a nondecaying two-point contribution. The [connected correlation function](#connected-correlation-function) and [correlation length](#correlation-length) describing ordinary critical fluctuations should be evaluated in a chosen pure phase when this distinction matters.

#### Common-tangent construction for phase coexistence

↑ **Parent:** [Phase coexistence](#phase-coexistence)

For a bulk [free-energy density](statistical-physics.md#free-energy-density) $f(\phi)$, two compositions coexist across a flat interface when

$$
f'(\phi_1)=f'(\phi_2)=\mu,
\qquad \mu\phi_1-f(\phi_1)=\mu\phi_2-f(\phi_2).
$$

The first condition equates the [chemical potentials](chemical-potential.md), and the second equates the [pressure](pressure.md). Equivalently the same straight line of slope $\mu$ is tangent to the graph of $f$ at both compositions. A stable coexistence pair uses a supporting tangent, so the resulting mixture lowers the bulk free energy.

##### Linear composition bias leaves coexistence compositions unchanged

↑ **Parent:** [Common-tangent construction for phase coexistence](#common-tangent-construction-for-phase-coexistence)

Adding $d\phi$ to a [free-energy density](statistical-physics.md#free-energy-density) adds a constant at fixed total [compositional order parameter](#compositional-order-parameter). In the [common-tangent construction for phase coexistence](#common-tangent-construction-for-phase-coexistence), it shifts the tangent slope by $d$ while preserving its points of contact. Thus coexistence compositions are unchanged, whereas their [chemical potential](chemical-potential.md) shifts. This does not assert unchanged equilibrium composition at a fixed externally imposed [chemical potential](chemical-potential.md).

#### Vapor-liquid equilibrium

↑ **Parent:** [Phase coexistence](#phase-coexistence)

### Continuous phase transition

↑ **Parent:** [Phase transition](#phase-transition)

A continuous phase transition has no latent heat and develops fluctuations on a diverging correlation length. Its singular observables are characterized by critical exponents.

### Vaporization

↑ **Parent:** [Phase transition](#phase-transition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vaporization)

[Vaporization](#vaporization) changes a [liquid](thermodynamics.md#liquid) into a [gas](thermodynamics.md#gas). It includes [evaporation](#evaporation) at a surface and [boiling](#boiling) within the liquid. Below the [liquid-gas critical point](#liquid-gas-critical-point), equilibrium conversion along the liquid-vapour [phase coexistence curve](thermodynamic-potential.md#phase-coexistence-curve) involves [latent heat](thermodynamic-potential.md#latent-heat); the liquid and vapour have equal [chemical potential](chemical-potential.md) there.

#### Enthalpy of vaporization

↑ **Parent:** [Vaporization](#vaporization)

The molar [enthalpy](enthalpy.md) difference between [vapor](thermodynamics.md#vapor) and [liquid](thermodynamics.md#liquid) at specified conditions, evaluated on coexistence when it is a [latent heat](thermodynamic-potential.md#latent-heat). Treating it as constant and treating the [vapor](thermodynamics.md#vapor) as ideal gives $\ln(P_2/P_1)=(\Delta H_{\rm vap}/R)(1/T_1-1/T_2)$.

#### Evaporation

↑ **Parent:** [Vaporization](#vaporization)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Evaporation)

[Evaporation](#evaporation) transfers molecules from a [liquid](thermodynamics.md#liquid) surface into the surrounding vapour. It can occur below the [boiling](#boiling) temperature, and competes with condensation from the vapour. Its net rate depends on the surrounding [vapor pressure](thermodynamic-potential.md#vapor-pressure) and transport conditions. Removing [latent heat](thermodynamic-potential.md#latent-heat) through evaporation can cool the remaining liquid.

##### Coffee-ring effect

↑ **Parent:** [Evaporation](#evaporation)

Nonuniform accumulation of suspended material toward the edge of a drying drop, commonly when a pinned contact line and nonuniform evaporation drive outward liquid flow. Contact-line motion, [solvent](mixture.md#solvent) choice, drying conditions and ink formulation can alter or suppress the resulting deposit.

#### Boiling

↑ **Parent:** [Vaporization](#vaporization)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boiling)

##### Critical heat flux

↑ **Parent:** [Boiling](#boiling)

A limiting heat flux associated with a transition to a less effective boiling heat-transfer regime under specified conditions. Its value depends on fluid properties, pressure, flow, heating and geometry; a single number cannot be transferred indiscriminately between different flow passages.

###### Departure from nucleate boiling

↑ **Parent:** [Critical heat flux](#critical-heat-flux)

A transition from effective nucleate boiling toward impaired surface wetting and substantially poorer heat removal in the relevant boiling regime. It is a concern when a heated fuel surface can become much hotter at an otherwise similar imposed heat load.

###### Departure from nucleate boiling ratio

↑ **Parent:** [Departure from nucleate boiling](#departure-from-nucleate-boiling)

The ratio of the heat flux needed to reach [departure from nucleate boiling](#departure-from-nucleate-boiling) to the actual local heat flux. Greater values indicate more margin under the model and correlation used.[Departure from nucleate boiling ratio entry](engineering.md#reactor-glossary-by-the-united-states-nuclear-regulatory-commission)

###### Minimum departure from nucleate boiling ratio

↑ **Parent:** [Departure from nucleate boiling ratio](#departure-from-nucleate-boiling-ratio)

The minimum local [departure from nucleate boiling ratio](#departure-from-nucleate-boiling-ratio) over the specified core region or assessment. It depends on local heat loading and coolant conditions, not only on average core power.

##### Boiling chip

↑ **Parent:** [Boiling](#boiling)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boiling_chip)

## Critical exponent

↑ **Parent:** [Critical phenomenon](critical-phenomenon.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Critical_exponent)

A critical exponent describes a power-law singularity near a continuous [phase transition](#phase-transition), such as $\xi\sim|t|^{-\nu}$ or $\chi\sim|t|^{-\gamma}$.

### Field crossover exponent

↑ **Parent:** [Critical exponent](#critical-exponent)

The [field crossover exponent](#field-crossover-exponent) describes the field scale $h\sim|t|^\Delta$ at which the zero-field critical regime changes. In the two-variable [scaling hypothesis for critical phenomena](#scaling-hypothesis-for-critical-phenomena), its value is the ratio $y_h/y_t$ of magnetic and thermal [scaling dimensions](string-theory.md#scaling-dimension). It is distinct from either $y_h$ or the [scaling dimension](string-theory.md#scaling-dimension) of the [order parameter](#order-parameter). The [Widom scaling relation](#widom-scaling-relation) and differentiation of the homogeneous [free-energy density](statistical-physics.md#free-energy-density) give the displayed identities when ordinary scaling applies.

### Percolation critical exponents

↑ **Parent:** [Critical exponent](#critical-exponent)

These [critical exponents](#critical-exponent) describe the leading singular powers of [percolation probability](percolation-theory.md#percolation-probability), [percolation susceptibility](bond-percolation.md#percolation-susceptibility), [correlation length](#correlation-length) and critical cluster distributions near the [percolation critical probability](percolation-theory.md#percolation-critical-probability). Their existence and exact values require theorems or scaling hypotheses for the particular model; they are not consequences of the definition of the threshold. For $\theta(p)=P_p(0\leftrightarrow\infty)$ and $\chi(p)=\mathbb E_p|C(0)|$, the definitions are $\theta(p)=(p-p_c)^{\beta+o(1)}$ above $p_c$ and $\chi(p)=(p_c-p)^{-\gamma+o(1)}$ below $p_c$. The [correlation length](#correlation-length) has $\xi(p)=|p-p_c|^{-\nu+o(1)}$. At criticality, the root-cluster tail is $P(|C(0)|\geq s)=s^{-1/\delta+o(1)}$; two-point connectivity has leading power $|x|^{-(d-2+\eta)}$; and the expected number per site of size-$s$ clusters has leading power $s^{-\tau}$. The last distribution differs from the size-weighted distribution seen at a specified site. Relations such as $\gamma=(2-\eta)\nu$ and $2\beta+\gamma=d\nu$ have specific scaling regimes, and the latter [hyperscaling relation](#hyperscaling-relation) fails in ordinary mean-field regimes above the [upper critical dimension of percolation](#upper-critical-dimension-of-percolation).

#### Mean-field percolation exponents

↑ **Parent:** [Percolation critical exponents](#percolation-critical-exponents)

The mean-field predictions model large clusters by [branching processes](stochastic-process.md#branching-process). Rigorous results apply in specified high-dimensional or sufficiently spread-out regimes, using tools such as [lace expansion](percolation-theory.md#lace-expansion) and the [percolation triangle condition](bond-percolation.md#percolation-triangle-condition). The full list involves different observables; the triangle condition alone should not be presented as proving every spatial exponent. With these exponents $2\beta+\gamma=3$, whereas $d\nu=d/2$, explaining the failure of naive [hyperscaling relation](#hyperscaling-relation) above six.

#### Percolation cluster fractal dimension

↑ **Parent:** [Percolation critical exponents](#percolation-critical-exponents)

The critical cluster mass-radius scaling exponent $D_f$ describes clusters of mass roughly $r^{D_f}$ at radius $r$. The displayed relation is the below-upper-critical-dimension scaling prediction, not an identity from the definition. In the planar scaling description $D_f=91/48$.

#### Percolation cluster-size tail exponent

↑ **Parent:** [Percolation critical exponents](#percolation-critical-exponents)

The exponent $\delta$ describes the tail of the critical cluster seen from a specified [vertex of a graph](graph.md#vertex-graph-theory). If the expected number of size-$s$ clusters per site scales as $s^{-\tau}$, weighting by cluster size gives $1/\delta=\tau-2$ when these scaling laws hold.

#### Percolation order-parameter exponent

↑ **Parent:** [Percolation critical exponents](#percolation-critical-exponents)

The leading power $\beta$ of the [percolation probability](percolation-theory.md#percolation-probability) approached from above the [percolation critical probability](percolation-theory.md#percolation-critical-probability). It quantifies how the density of the [infinite percolation cluster](bond-percolation.md#infinite-percolation-cluster) first becomes positive.

### Reduced temperature

↑ **Parent:** [Critical exponent](#critical-exponent)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reduced_temperature)

The reduced temperature is a dimensionless distance from a critical temperature. Multiplying it by a nonzero constant does not change any [critical exponent](#critical-exponent).

### Heat-capacity critical exponent

↑ **Parent:** [Critical exponent](#critical-exponent)

The heat-capacity critical exponent is defined by the singular part $c_{\mathrm s}\sim|t|^{-\alpha}$ as the [reduced temperature](#reduced-temperature) tends to zero.

### Order-parameter critical exponent

↑ **Parent:** [Critical exponent](#critical-exponent)

The order-parameter critical exponent is defined in the ordered phase by $m\sim(-t)^\beta$ at zero conjugate field.

### Magnetic-susceptibility critical exponent

↑ **Parent:** [Critical exponent](#critical-exponent)

The magnetic-susceptibility critical exponent is defined by the zero-field [magnetic susceptibility](statistical-physics.md#magnetic-susceptibility) $\chi\sim|t|^{-\gamma}$. Separate amplitudes, and occasionally separate exponents, may occur on the two sides of the transition.

### Critical-isotherm exponent

↑ **Parent:** [Critical exponent](#critical-exponent)

The critical-isotherm exponent is defined at the critical temperature by $m\sim|B|^{1/\delta}$ as the conjugate field $B$ tends to zero.

### Correlation-length critical exponent

↑ **Parent:** [Critical exponent](#critical-exponent)

The correlation-length critical exponent is defined by $\xi\sim|t|^{-\nu}$. At a [renormalization-group fixed point](#renormalization-group-fixed-point), its reciprocal is the positive eigenvalue of the temperature-like scaling direction.

## Critical dimension (phase transition)

↑ **Parent:** [Critical phenomenon](critical-phenomenon.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Critical_dimension)

In the analysis of a [phase transition](#phase-transition), a critical dimension is a spatial dimension at which the character of fluctuations and critical behavior changes. Below a lower critical dimension the relevant ordered phase cannot persist; above an upper critical dimension mean-field critical exponents apply. This is distinct from the [critical dimension of string theory](bosonic-string-theory.md#critical-dimension-of-string-theory), where cancellation of quantum anomalies selects a target-spacetime dimension.

## Lower critical dimension

↑ **Parent:** [Critical phenomenon](critical-phenomenon.md)

The lower critical dimension is the spatial dimension at or below which fluctuations prevent the ordered phase associated with a proposed finite-temperature transition. A short-range model with discrete symmetry normally has $d_{\mathrm l}=1$, whereas continuous $O(2)$ symmetry has $d_{\mathrm l}=2$.

<h3 id="berezinskii-kosterlitz-thouless-transition">Berezinskii–Kosterlitz–Thouless transition</h3>

↑ **Parent:** [Lower critical dimension](#lower-critical-dimension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Berezinskii–Kosterlitz–Thouless_transition)

The Berezinskii–Kosterlitz–Thouless transition in the two-dimensional [XY model](statistical-physics.md#xy-model) separates a low-temperature phase with algebraically decaying correlations from a high-temperature phase with unbound vortices and exponentially decaying correlations. It does not produce conventional long-range order.

How can something resist a twist when its orientation never settles down? The distinction is between [long-range order](statistical-physics.md#long-range-order), a nonzero limiting [correlation function](#correlation-function), and [phase stiffness](#phase-stiffness), a [free energy](thermodynamic-potential.md#thermodynamic-free-energy) cost for a slow spatial twist. In a uniform two-dimensional [XY model](statistical-physics.md#xy-model) at positive [temperature](temperature.md), smooth [spin waves](#spin-wave) can erase the first while leaving the second finite. [Vortex-antivortex binding](#vortex-antivortex-binding) then decides whether that resistance survives on arbitrarily large scales.

[Vadim Lvovich Berezinskii](physicist.md#vadim-lvovich-berezinskii) developed an earlier description of two-dimensional order. [John Michael Kosterlitz](physicist.md#john-michael-kosterlitz) and [D. J. Thouless](physicist.md#david-james-thouless) independently developed the defect mechanism; Kosterlitz's 2016 lecture explicitly acknowledges their initial ignorance of Berezinskii's work. The central step was to include rare [vortices](#phase-vortex) alongside smooth [spin waves](#spin-wave).[2016 Nobel lecture, pp. 89–94, sections 2–3; independent Berezinskii work, winding sectors and vortex renormalization](physics-bibliography.md#topological-defects-and-phase-transitions-by-john-michael-kosterlitz)

The [Mermin-Wagner theorem](#mermin-wagner-theorem) concerns [continuous symmetry](physics.md#continuous-symmetry) and sufficiently short-range interactions in the [thermodynamic limit](statistical-physics.md#thermodynamic-limit). It does not say that every two-dimensional system is disordered in every sense, nor that every [continuous symmetry](physics.md#continuous-symmetry) gives a [Berezinskii–Kosterlitz–Thouless transition](#berezinskii-kosterlitz-thouless-transition). Here the [order parameter](#order-parameter) has a circular phase, permitting integer [winding numbers](complex-analysis.md#winding-number). [Finite-scale vortex renormalization](#finite-scale-vortex-renormalization) explains why a finite sample can look coherent even when its infinite counterpart lacks [long-range order](statistical-physics.md#long-range-order).

#### Single-vortex energy-entropy balance

↑ **Parent:** [Berezinskii–Kosterlitz–Thouless transition](#berezinskii-kosterlitz-thouless-transition)

Consider an original counting example: a square two-dimensional [XY model](statistical-physics.md#xy-model) of side $L$, a microscopic core radius $a$, and a fixed [phase stiffness](#phase-stiffness) $\rho_s$. This deliberately neglects screening by other [vortices](#phase-vortex). Away from a unit [phase vortex](#phase-vortex), $\theta=\arg(x+iy)$ and $|\nabla\theta|=1/r$. Integrating the [Goldstone-mode effective free energy](#goldstone-mode-effective-free-energy) over an annulus gives

$$
E_{\rm v}=E_c+\frac{\rho_s}{2}\int_a^L\frac{2\pi r\,dr}{r^2}
=E_c+\pi\rho_s\log(L/a).
$$

Boundary shape changes finite terms. There are order $(L/a)^2$ core positions, so the positional [entropy](entropy.md) is $S_{\rm v}=2k_B\log(L/a)+O(k_B)$, where $k_B$ is the [Boltzmann constant](thermodynamics.md#boltzmann-constant). With $K=\rho_s/(k_BT)$, subtracting $TS_{\rm v}$ gives the displayed [free energy](thermodynamic-potential.md#thermodynamic-free-energy).

For $L/a=1000$ and $E_c/(k_BT)=2$, the dimensionless [free energy](thermodynamic-potential.md#thermodynamic-free-energy) cost is about $5.546$ at $K=0.8$ and $-0.965$ at $K=0.5$. The same logarithm appears in the cost and the positional reward: increasing the system size strengthens whichever has the larger coefficient. The corresponding one-defect [Boltzmann factors](canonical-ensemble.md#boltzmann-factor), about $0.00390$ and $2.62$, are relative statistical weights, not normalized probabilities. The latter signals failure of a dilute single-defect estimate.

A single net [phase vortex](#phase-vortex) requires compatible boundaries: on a periodic sample use neutral pairs, as required by [vortex charge neutrality](statistical-physics.md#vortex-charge-neutrality). This argument identifies a possible threshold, but predicting the [universal stiffness jump](#universal-stiffness-jump) requires the renormalized [phase stiffness](#phase-stiffness), after smaller pairs have responded. It does not justify setting the transition [temperature](temperature.md) equal to a bare lattice coupling divided by a universal constant.

#### Vortex-pair renormalization flow

↑ **Parent:** [Berezinskii–Kosterlitz–Thouless transition](#berezinskii-kosterlitz-thouless-transition)

In the dilute-vortex description of the two-dimensional XY model, $K=\rho_s/(k_BT)$ is dimensionless stiffness and $y$ is [phase vortex](#phase-vortex) fugacity. A [phase vortex](#phase-vortex) has logarithmic energy $\pi\rho_s\log(L/a)$, while its placement entropy is $2k_B\log(L/a)$. Small [phase vortex](#phase-vortex) pairs screen the logarithmic interaction, lowering the stiffness. Near $K=2/\pi$, the rescaled variables $X=2-\pi K$, $Y=4\pi y$ obey $X'=Y^2$, $Y'=XY$ to leading order. The invariant $X^2-Y^2$ leads to an essential correlation-length singularity $\xi\sim a\exp(C/\sqrt{T-T_c})$, not a finite power-law exponent.

Here $\ell=\log(r/a)$ increases toward larger observation distances, and the [vortex fugacity](statistical-physics.md#vortex-fugacity) $y$ is a dimensionless weight per unit core, conventionally initialized as $y_0\simeq e^{-E_c/(k_BT)}$ with the microscopic measure fixed. Numerical coefficients depend on this normalization. In the displayed convention, differentiating $X=2-\pi K$ using the original flow gives

$$
X'=4\pi^4K^2y^2=\frac{(2-X)^2}{4}Y^2,
\qquad Y'=XY.
$$

Only replacing the prefactor $(2-X)^2/4$ by one near $X=0$ gives the scaled leading model. Its [first integral](differential-equation.md#first-integral) follows directly:

$$
\frac{d}{d\ell}(X^2-Y^2)=2XY^2-2Y(XY)=0.
$$

Thus this [first integral](differential-equation.md#first-integral) belongs to the stated scaled model, not exactly to the original $K,y$ equations. For $Y\geq0$, the critical [separatrix](dynamical-systems.md#separatrix) is $X=-Y$. The bound side has $X<-Y$ and flows to $Y=0$, $X<0$; the unbinding side ultimately runs to large [vortex fugacity](statistical-physics.md#vortex-fugacity), where the dilute approximation ceases to be quantitative.

To derive the unusual [correlation length](#correlation-length) scaling without fitting an exponent, write the invariant on a nearby unbinding trajectory as $X^2-Y^2=-c^2$. Then $X'=X^2+c^2$ and the time to cross fixed small limits $-b$ to $b$ is $2\arctan(b/c)/c\sim\pi/c$. If a physical one-parameter path crosses the [separatrix](dynamical-systems.md#separatrix) transversely, its $c^2$ is proportional to the positive [reduced temperature](#reduced-temperature). Since distance grows as $e^\ell$, this gives $\xi\sim a\exp(b_0/\sqrt{t})$, with a nonuniversal $b_0>0$. This is the dimensionless-temperature form of the singularity above.

##### Finite-scale vortex renormalization

↑ **Parent:** [Vortex-pair renormalization flow](#vortex-pair-renormalization-flow)

An experiment of size $L$ stops the [renormalization-group flow](#renormalization-group-flow) at a finite $\ell_{\max}$. In the leading scaled model take the original initial conditions $Y_0=0.06$ and $X_0=-0.10,-0.06,-0.03$. The invariant is respectively $0.0064,0,-0.0027$. The first approaches $X=-0.08$, hence $K=(2.08)/\pi$; the second follows the critical [separatrix](dynamical-systems.md#separatrix); the third eventually leaves the small-[vortex fugacity](statistical-physics.md#vortex-fugacity) regime. These are chosen model trajectories, with no fitted experimental parameters.

On the critical [separatrix](dynamical-systems.md#separatrix), $X=-Y$ implies $Y'=-Y^2$, hence

$$
Y(\ell)=\frac{Y_0}{1+Y_0\ell},\qquad
K(\ell)=\frac2\pi+\frac{Y_0}{\pi(1+Y_0\ell)}.
$$

Even a critical finite sample therefore has a [phase stiffness](#phase-stiffness) above its asymptotic jump value, with a slow logarithmic correction in $L$. Slightly above the transition, a sample with $L\ll\xi$ can resemble the algebraic phase before the flow reaches unbound [vortices](#phase-vortex). A trap additionally varies the local density and [phase stiffness](#phase-stiffness); neither its whole-cloud coherence nor a finite observation window automatically measures the homogeneous [thermodynamic limit](statistical-physics.md#thermodynamic-limit).

<a id="image-original-scaled-vortex-flow-and-finite-scale-stiffness"></a>
![](bkt-scaled-vortex-renormalization-flow.png)

**[Figure 1](#image-original-scaled-vortex-flow-and-finite-scale-stiffness). Original scaled vortex flow and finite-scale stiffness**. The arrows increase observation distance in the leading near-critical model $X'=Y^2$, $Y'=XY$. All three colored trajectories start at $Y_0=0.06$. The right panel uses $K=(2-X)/\pi$ along the same trajectories. The plot is a mathematical illustration, not historical data; the dilute model must be abandoned when the vortex fugacity grows large.

#### Universal stiffness jump

↑ **Parent:** [Berezinskii–Kosterlitz–Thouless transition](#berezinskii-kosterlitz-thouless-transition)

The renormalized [phase stiffness](#phase-stiffness) has this discontinuity at the [Berezinskii–Kosterlitz–Thouless transition](#berezinskii-kosterlitz-thouless-transition). The algebraic [correlation function](#correlation-function) has exponent $1/4$ at the transition from the ordered side.

The stiffness here is an energy in two dimensions, not an areal mass density. For a neutral [superfluid](statistical-physics.md#superfluid) of particles of mass $m$, let $n_s$ be the [superfluid number density](statistical-physics.md#superfluid-number-density) per unit area. Substituting the [superfluid velocity](statistical-physics.md#superfluid-velocity) $\mathbf v_s=(\hbar/m)\nabla\theta$ into the kinetic energy gives $\rho_s=\hbar^2n_s/m$. Consequently the jump can also be written

$$
n_s(T_{\rm BKT}^-)\lambda_T^2=4,
\qquad \lambda_T^2=\frac{2\pi\hbar^2}{mk_BT},
$$

where $\lambda_T$ is the [thermal wavelength](canonical-ensemble.md#thermal-de-broglie-wavelength). It is the large-distance [superfluid number density](statistical-physics.md#superfluid-number-density), rather than the total density or a locally inferred condensate density, that enters this relation.

Within the [vortex-pair renormalization flow](#vortex-pair-renormalization-flow), $y$ changes from irrelevant to relevant at $\pi K_R=2$, with $K_R$ the large-distance dimensionless [phase stiffness](#phase-stiffness). Combining this with the [spin wave](#spin-wave) result $\eta=1/(2\pi K_R)$ gives $\eta=1/4$. Above the transition the homogeneous equilibrium [phase stiffness](#phase-stiffness) vanishes at infinite observation scale. A discontinuous response coefficient is compatible with a diverging [correlation length](#correlation-length); it does not imply a [latent heat](thermodynamic-potential.md#latent-heat).[Section 3, pp. 92–94: fugacity flow and renormalized superfluid-density jump](physics-bibliography.md#topological-defects-and-phase-transitions-by-john-michael-kosterlitz)

#### Vortex-antivortex binding

↑ **Parent:** [Berezinskii–Kosterlitz–Thouless transition](#berezinskii-kosterlitz-thouless-transition)

In the phase with [quasi-long-range order](#quasi-long-range-order), [vortex](#phase-vortex) defects of opposite winding remain bound in pairs. Their unbinding produces the disordered phase with a finite [correlation length](#correlation-length).

For two unit [vortices](#phase-vortex) of opposite charge separated by $R$, the [vortex Coulomb gas](statistical-physics.md#vortex-coulomb-gas) gives $E_{+-}(R)\simeq2E_c+2\pi\rho_s\log(R/a)$ before screening. At distances much greater than $R$, their phase gradients cancel at leading order: the pair field decays as $R/r^2$, whereas a lone [phase vortex](#phase-vortex) has a $1/r$ gradient. A neutral pair therefore has finite energy as $L\to\infty$ at fixed $R$. Bound does not mean absent: small pairs remain thermally excited and reduce the [phase stiffness](#phase-stiffness) through their response to a twist.

<a id="image-opposite-phase-windings-and-the-geometry-of-a-neutral-vortex-pair"></a>
![](bkt-vortex-pair-phase-geometry.png)

**[Figure 2](#image-opposite-phase-windings-and-the-geometry-of-a-neutral-vortex-pair). Opposite phase windings and the geometry of a neutral vortex pair**. Original phase field $\theta=\arg(x+1+iy)-\arg(x-1+iy)$. Each arrow is the unit vector $(\cos\theta,\sin\theta)$, not the superfluid velocity. Counterclockwise loops around the left and right cores have winding $+1$ and $-1$; a loop enclosing both has zero winding. The circles on the right show the corresponding motion in phase space.

#### Quasi-long-range order

↑ **Parent:** [Berezinskii–Kosterlitz–Thouless transition](#berezinskii-kosterlitz-thouless-transition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quasi-long-range_order)

Quasi-long-range order means that correlations decay algebraically rather than approaching a nonzero constant. It occurs in the low-temperature phase of the two-dimensional [XY model](statistical-physics.md#xy-model), where [spin waves](#spin-wave) destroy true long-range order but bound vortex pairs preserve power-law correlations.

For a dimensionless [Gaussian](probability-distribution.md#normal-distribution) action $F/(k_BT)=(K_R/2)\int d^2r\,|\nabla\theta|^2$, the [phase-difference variance](#phase-difference-variance) at $a\ll r\ll L$ is $\log(r/a)/(\pi K_R)$ up to bounded cutoff terms. [Gaussian phase averaging](partial-differential-equation.md#gaussian-phase-averaging) then gives

$$
g(r)=\left\langle e^{i[\theta(\mathbf r)-\theta(0)]}\right\rangle
\propto(r/a)^{-\eta},\qquad \eta=\frac{1}{2\pi K_R}.
$$

Every positive $\eta$ makes $g(r)\to0$, so there is no conventional [long-range order](statistical-physics.md#long-range-order), even when the [phase stiffness](#phase-stiffness) is finite. This is how an accumulation of gentle, cheap twists destroys global alignment without making every local twist free.

#### Vortex-unbinding crossover in a trapped atomic gas

↑ **Parent:** [Berezinskii–Kosterlitz–Thouless transition](#berezinskii-kosterlitz-thouless-transition)

In 2006, [Zoran Hadzibabic](physicist.md#zoran-hadzibabic), [Peter Krüger](physicist.md#peter-kruger), [Marc Cheneau](physicist.md#marc-cheneau), [Baptiste Battelier](physicist.md#baptiste-battelier) and [Jean Dalibard](physicist.md#jean-dalibard) split a cooled [rubidium](chemical-substance.md#rubidium)-87 cloud into two independent planar gases using an [optical lattice](optics.md#optical-lattice). After release, the expanding sheets overlapped; [absorption imaging](atomic-physics.md#absorption-imaging) recorded their [matter-wave interference](wave-function.md#matter-wave-interference). Smooth fringe waviness revealed [thermal phase fluctuations](statistical-physics.md#thermal-phase-fluctuation), while sharp dislocations indicated isolated [vortices](#phase-vortex). The initial evaporative-cooling endpoint controlled the preparation; central fringe contrast served as a degeneracy proxy because direct thermometry in the lattice was difficult.[Pages 1–2, preparation and readout; Fig. 1; temperature control and Fig. 2](physics-bibliography.md#berezinskii-kosterlitz-thouless-crossover-in-a-trapped-atomic-gas-by-zoran-hadzibabic-and-others)

Loss of extended coherence coincided with increased vortex signatures. The [optical trap](optics.md#optical-tweezers) and finite cloud produced a crossover; tightly bound pairs were unresolved, and short-wavelength modes could contaminate high-temperature counts. These were observations of the [vortex](#phase-vortex)-unbinding mechanism, not a direct measurement of [phase stiffness](#phase-stiffness) or a sharp homogeneous [universal stiffness jump](#universal-stiffness-jump). The authors left the sample's [superfluidity](statistical-physics.md#superfluidity) open.[Pages 3–4, Figs. 3–4; geometry, invisible pairs, detection limits and final paragraph on unmeasured superfluidity](physics-bibliography.md#berezinskii-kosterlitz-thouless-crossover-in-a-trapped-atomic-gas-by-zoran-hadzibabic-and-others)

## Correlation function

↑ **Parent:** [Critical phenomenon](critical-phenomenon.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Correlation_function)

A correlation function measures the joint fluctuation of observables at separated points. For a scalar field, the connected two-point function is $G(x-y)=\langle\phi(x)\phi(y)\rangle-\langle\phi(x)\rangle\langle\phi(y)\rangle$.

### Four-point correlation function

↑ **Parent:** [Correlation function](#correlation-function)

The [four-point correlation function](#four-point-correlation-function) measures a time-ordered product of four field insertions. For a centered scalar field its disconnected terms are the three products of two-point functions, and subtracting those products leaves the [connected correlation function](#connected-correlation-function). In a free Gaussian scalar vacuum the connected four-point function vanishes, by [Wick's theorem](perturbative-quantum-field-theory.md#wick-s-theorem), so only the three paired products remain. The connected four-point function of [phi-fourth theory](scalar-field-theory.md#quartic-interaction) starts with one quartic vertex; amputation removes its external propagators. The full correlator, its connected part and the [four-point one-particle-irreducible correlation function](perturbative-quantum-field-theory.md#four-point-one-particle-irreducible-correlation-function) should therefore be distinguished.

### One-point correlation function

↑ **Parent:** [Correlation function](#correlation-function)

The [correlation function](#correlation-function) with a single field insertion is its [expectation value](quantum-system.md#expectation-value). In a translation-invariant vacuum it is independent of position. A [tadpole subtraction](perturbative-quantum-field-theory.md#tadpole-subtraction) chooses a linear [counterterm](perturbative-quantum-field-theory.md#counterterm), or shifts the expansion point of the field, so that this expectation is zero. This removes attached [tadpole diagrams](perturbative-quantum-field-theory.md#tadpole-diagram) from higher connected [correlation functions](#correlation-function) without discarding the physical need to renormalize the chosen vacuum.

### Connected correlation function

↑ **Parent:** [Correlation function](#correlation-function)

The connected correlation of two observables is $\langle AB\rangle_c=\langle AB\rangle-\langle A\rangle\langle B\rangle$. It vanishes in a [product state](bell-state.md#product-state) when $A$ and $B$ act on disjoint factors.

#### Correlation-function susceptibility sum rule

↑ **Parent:** [Connected correlation function](#connected-correlation-function)

When an energy Hamiltonian contains $-h\sum_n\sigma_n$, differentiating its [partition function](canonical-ensemble.md#canonical-partition-function) gives $\chi=(\beta_{\rm th}/N)\operatorname{Var}(\sum_n\sigma_n)$. Translation invariance converts this to the connected-correlation sum. A dimensionless source $\beta_{\rm th}h$ removes the explicit inverse-temperature factor. In continuum physical coordinates the lattice sum includes the site-density factor $a^{-D}$. A selected [pure thermodynamic phase](#pure-thermodynamic-phase) is needed below an ordered transition to avoid a macroscopic mixture contribution.

##### Spin-mixture contribution to zero-field susceptibility

↑ **Parent:** [Correlation-function susceptibility sum rule](#correlation-function-susceptibility-sum-rule)

In a symmetric equal mixture of two ordered [pure thermodynamic phases](#pure-thermodynamic-phase) with magnetizations $\pm M_0$, the mean spin vanishes but the large-distance two-spin expectation tends to $M_0^2$. Thus the [connected correlation function](#connected-correlation-function) of the mixture has a nondecaying part. The [correlation-function susceptibility sum rule](#correlation-function-susceptibility-sum-rule) gives an extensive contribution $\beta_{\rm th}N M_0^2$ to susceptibility per spin. This is phase-switching response, not the connected susceptibility within one pure phase. The latter uses the thermodynamic limit followed by a one-sided zero-field limit, and subtracts the nonzero pure-phase mean before defining the [correlation length](#correlation-length).

#### Inverse Hessian relation for a connected two-point function

↑ **Parent:** [Connected correlation function](#connected-correlation-function)

In the [scalar-field source Legendre transform](#scalar-field-source-legendre-transform), differentiating $h=\delta\Gamma/\delta m$ with respect to the source and using $G=\delta m/\delta h$ yields this inverse-kernel relation. For a scalar quartic [Landau-Ginzburg theory](#landau-ginzburg-theory), $\Gamma_{\rm L}^{(2)}=-\nabla^2+r_0+u_0m^2/2$, so the connected response is the Green kernel of that operator. A one-momentum representation requires a translationally invariant background.

#### Amputated connected correlation function

↑ **Parent:** [Connected correlation function](#connected-correlation-function)

An amputated [connected correlation function](#connected-correlation-function) is obtained by removing external propagators. Amputation using full propagators eliminates external [self-energy](perturbative-quantum-field-theory.md#self-energy) decorations; internal exchange diagrams remain. It is distinct from a [one-particle-irreducible correlation function](perturbative-quantum-field-theory.md#one-particle-irreducible-correlation-function). In a scalar theory with vanishing one-point function, at zero momentum the four-point quantity satisfies $\mathcal A_4=-\Gamma^{(4)}+3[\Gamma^{(3)}]^2/\Gamma^{(2)}$ with a convention in which connected diagram vertices are minus effective-action derivatives. For a constant scalar source, the Legendre relation $J=\Gamma'(\phi)$ gives $G''=1/\Gamma''$ and $G''''=-\Gamma''''/(\Gamma'')^4+3(\Gamma''')^2/(\Gamma'')^5$. Dividing by the four full external propagators proves the formula.

### Two-point correlation function

↑ **Parent:** [Correlation function](#correlation-function)

A two-point correlation function is the expectation of a product of fields or observables at two points. Its connected version subtracts the product of the one-point expectations.

### Dynamic structure factor

↑ **Parent:** [Correlation function](#correlation-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dynamic_structure_factor)

The dynamic structure factor is the space-time [Fourier transform](fourier-transform.md) of an equilibrium [two-point correlation function](#two-point-correlation-function). It resolves fluctuations by [angular frequency](lagrangian-mechanics.md#angular-frequency) and [wavevector](elasticity-physics.md#wavevector) and is related to the dissipative part of a [retarded Green function](quantum-field-theory.md#retarded-green-function) by the [fluctuation-dissipation theorem](quantum-field-theory.md#fluctuation-dissipation-theorem).

#### Static structure factor

↑ **Parent:** [Dynamic structure factor](#dynamic-structure-factor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Static_structure_factor)

The static structure factor is the equal-time spatial [Fourier transform](fourier-transform.md) of a [two-point correlation function](#two-point-correlation-function). Depending on convention it is obtained either by integrating the [dynamic structure factor](#dynamic-structure-factor) over frequency or by taking an appropriate zero-frequency limit.

##### Polymer scattering function

↑ **Parent:** [Static structure factor](#static-structure-factor)

For $N$ equal scattering sites on one [polymer](polymer.md), define $g(\mathbf k)=N^{-1}\sum_{m,n}\langle e^{i\mathbf k\cdot(\mathbf R_n-\mathbf R_m)}\rangle$. It has $g(0)=N$; its normalized form factor is $g/N$. Under a rotationally invariant joint distribution, each separation vector has a uniform direction at fixed magnitude $r$. The angular average is $\tfrac12\int_{-1}^{1}e^{ikr\mu}\,d\mu=\sin(kr)/(kr)$, with value one at $r=0$. Thus $g$ depends only on $k=|\mathbf k|$, and $g(k)=N^{-1}\sum_{m,n}\langle\sin(k|\mathbf R_n-\mathbf R_m|)/(k|\mathbf R_n-\mathbf R_m|)\rangle$. The diagonal self terms are essential in a finite chain and give the large-$k$ limit one for a discrete [Gaussian chain](mathematical-biology.md#gaussian-chain).

###### Guinier expansion of a polymer scattering function

↑ **Parent:** [Polymer scattering function](#polymer-scattering-function)

Expand the isotropic angular factor as $\sin(kr)/(kr)=1-k^2r^2/6+O(k^4r^4)$. For a [polymer scattering function](#polymer-scattering-function) and finite fourth pair moments, the constant double sum gives $g(0)=N$, and the quadratic sum is determined by the [radius of gyration](polymer.md#radius-of-gyration):

$$
\frac{g(k)}N=1-\frac{k^2R_g^2}{3}+O(k^4).
$$

In the range $kR_g\ll1$, this is also approximated by $e^{-k^2R_g^2/3}$. The coefficient follows from isotropy and the definition of $R_g$ and does not require a [Gaussian chain](mathematical-biology.md#gaussian-chain).

### Correlation length

↑ **Parent:** [Correlation function](#correlation-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Correlation_length)

The correlation length is the characteristic distance over which a connected [correlation function](#correlation-function) decays. It diverges at an ordinary continuous critical point as $\xi\sim|t|^{-\nu}$.

#### Correlation volume

↑ **Parent:** [Correlation length](#correlation-length)

A volume over which order-parameter fluctuations are correlated. For one isotropic [correlation length](#correlation-length) $\xi$, its scale is $\xi^D$; with anisotropic lengths it is the product of the appropriate directional lengths. A [Ginzburg criterion](#ginzburg-criterion) compares fluctuations averaged over this volume with the squared mean [order parameter](#order-parameter).

#### Landau scalar correlation length

↑ **Parent:** [Correlation length](#correlation-length)

For a stable homogeneous scalar quartic saddle with [gradient](multivariable-calculus.md#gradient) coefficient one, the [Ornstein--Zernike correlation function](#ornstein-zernike-correlation-function) has denominator $q^2+r_0+u_0m_0^2/2$. At zero source and $u_0>0$, the [correlation length](#correlation-length) is $r_0^{-1/2}$ in the disordered phase and $(-2r_0)^{-1/2}$ on either selected ordered branch. Linear thermal tuning of $r_0$ gives [correlation-length critical exponent](#correlation-length-critical-exponent) $\nu=1/2$ with different amplitudes on the two sides.

## Order parameter

↑ **Parent:** [Critical phenomenon](critical-phenomenon.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Order_parameter)

An order parameter vanishes in a symmetric phase and becomes nonzero when that symmetry is spontaneously broken.

### Order-parameter phase

↑ **Parent:** [Order parameter](#order-parameter)

For a two-component [order parameter](#order-parameter) of nonzero magnitude, write $m_x+im_y=\bar m e^{i\theta}$. Its phase is the orientation angle modulo $2\pi$, not a [thermodynamic phase](thermodynamics.md#thermodynamic-phase) such as an ordered or disordered state. A global continuous [symmetry](physics.md#symmetry-physics) rotates this angle uniformly; [spin waves](#spin-wave) are smooth spatial changes, while a [phase vortex](#phase-vortex) has nonzero winding around an excluded core. At a zero of the magnitude the angle is undefined, allowing the topology of an orientation field to change.

### Off-diagonal long-range order

↑ **Parent:** [Order parameter](#order-parameter)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Off-diagonal_long-range_order)

For a homogeneous bosonic condensate, the one-body [density matrix](density-matrix.md) retains a nonzero long-distance component. More generally, macroscopic occupation is identified by an eigenvalue of that [density matrix](density-matrix.md) proportional to particle number. This gives a number-conserving description even when the one-point annihilation-field expectation vanishes. In a paired fermionic system the corresponding macroscopic order belongs to the two-particle [density matrix](density-matrix.md), rather than an [electron](physics.md#electron) single-particle condensate.

### Field conjugate to an order parameter

↑ **Parent:** [Order parameter](#order-parameter)

A field conjugate to a scalar [order parameter](#order-parameter) $m$ contributes $-hm$ to its [free-energy density](statistical-physics.md#free-energy-density). Differentiating the equilibrium [free energy](thermodynamic-potential.md#thermodynamic-free-energy) with respect to $h$ gives $-m$, with density or extensive normalization stated consistently. In a ferromagnet the [conjugate field](#field-conjugate-to-an-order-parameter) is magnetic; for a fluid-density [order parameter](#order-parameter) it is related to a chemical-potential difference. It can explicitly break the symmetry whose spontaneous breaking defines the ordered phase.

### Vector order parameter

↑ **Parent:** [Order parameter](#order-parameter)

A vector order parameter has several components transforming together as a [vector](vector-space.md#vector) under spatial rotations. A [polar order parameter](#polar-order-parameter) is an example. Its [functional derivative](calculus-of-variations.md#functional-derivative) $\delta F/\delta\mathbf p$ has one component for each component of the [order parameter](#order-parameter).

### Conserved order parameter

↑ **Parent:** [Order parameter](#order-parameter)

A conserved order parameter is a field whose spatial integral remains fixed under the dynamics. A local composition difference in a closed mixture is a standard example.

### Topological defect

↑ **Parent:** [Order parameter](#order-parameter)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Topological_defect)

A topological defect is a localized obstruction to extending an ordered field smoothly and nonvanishingly through space. Its charge is determined by the homotopy class of the order parameter around the defect.

#### Homotopy classification of cosmological defects

↑ **Parent:** [Topological defect](#topological-defect)

Disconnected vacuum components support walls, noncontractible vacuum loops support line defects, and nontrivial vacuum two-spheres support monopoles in three spatial dimensions. Allowed [topology](topology.md) does not alone predict the number formed or their subsequent survival.

#### Cosmological texture

↑ **Parent:** [Topological defect](#topological-defect)

An extended order-parameter winding associated with a nontrivial third [homotopy group](homotopy.md#homotopy-group) of a [vacuum manifold](quantum-field-theory.md#vacuum-manifold) in three spatial dimensions. A texture can collapse and unwind when its field leaves the [vacuum manifold](quantum-field-theory.md#vacuum-manifold); it differs from a permanent monopole or string core.

#### Nematic hedgehog defect

↑ **Parent:** [Topological defect](#topological-defect)

A three-dimensional point defect characterized by how the surrounding [nematic director](#nematic-director) covers orientation space. Its hedgehog charge is not the same quantity as a planar disclination winding strength.

##### Hyperbolic hedgehog defect

↑ **Parent:** [Nematic hedgehog defect](#nematic-hedgehog-defect)

A point-defect texture that can compensate the radial boundary condition of a sphere with [homeotropic anchoring](#homeotropic-anchoring), giving a dipolar particle–defect configuration in a uniform far field. It carries the opposite hedgehog charge to the radial particle boundary under a consistent convention.

#### Boojum

↑ **Parent:** [Topological defect](#topological-defect)

A defect localized at a boundary of an ordered medium. A spherical inclusion with degenerate [planar anchoring](#planar-anchoring) in a [nematic liquid crystal](#nematic-liquid-crystal) can have a bipolar texture with two surface boojums, unlike a bulk point-defect pair.

#### Kibble mechanism

↑ **Parent:** [Topological defect](#topological-defect)

A [spontaneous symmetry breaking](quantum-field-theory.md#spontaneous-symmetry-breaking) chooses order-parameter directions independently in regions that have not been in causal contact. Mismatches around disconnected components, loops or enclosing spheres can trap [domain walls](#domain-wall), [cosmic strings](cosmology.md#cosmic-string) or [magnetic monopoles](mathematical-physics.md#magnetic-monopole). The correlation length cannot exceed the causal horizon, so one monopole per horizon volume estimates the smallest causal initial abundance up to geometrical and efficiency factors.

// Target: classical-field-theory-soliton.bigb

#### Domain wall

↑ **Parent:** [Topological defect](#topological-defect)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Domain_wall)

A domain wall is a codimension-one configuration interpolating between disconnected components of a [vacuum manifold](quantum-field-theory.md#vacuum-manifold). In a one-dimensional system with broken discrete symmetry it is a point defect of finite energy, so positional entropy produces a nonzero density at every positive temperature.

##### Horizon-scaling domain wall network

↑ **Parent:** [Domain wall](#domain-wall)

If the typical wall separation grows as cosmic time, surface [energy](energy.md) per volume is of order wall tension divided by time. This decreases more slowly than the usual radiation-era total density and can lead to a wall-domination problem.

##### Scalar quartic domain wall

↑ **Parent:** [Domain wall](#domain-wall)

For a [Landau-Ginzburg theory](#landau-ginzburg-theory) with positive gradient stiffness $\kappa$, $r<0$ and quartic coupling $u>0$, the degenerate minima are $\pm M_0$, $M_0^2=|r|/u$. A planar [domain wall](#domain-wall) solves $\kappa\phi''=r\phi+u\phi^3$. Multiplying by $\phi'$ and using the limiting minima gives $\kappa(\phi')^2/2=u(\phi^2-M_0^2)^2/4$. Separating this equation yields the displayed profile, and integrating its excess energy gives the positive surface tension $2\sqrt{2\kappa}|r|^{3/2}/(3u)$. Its area cost is subextensive compared with bulk volume, permitting phase-separated [common-tangent construction](#common-tangent-construction) states when the average [order parameter](#order-parameter) is constrained.

#### Phase vortex

↑ **Parent:** [Topological defect](#topological-defect)

A vortex is a topological defect around which the phase of a complex [order parameter](#order-parameter) has nonzero integer winding. In two dimensions an isolated vortex in a phase-only model has energy proportional to the logarithm of the system size.

The integer $q$ is a [winding number](complex-analysis.md#winding-number): a counterclockwise circuit returns the same complex [order parameter](#order-parameter) after its angle changes by $2\pi q$. Smooth changes that keep the [order parameter](#order-parameter) nonzero on that circuit cannot change $q$. In a continuum [superfluid](statistical-physics.md#superfluid), the core suppresses the magnitude, allowing the winding obstruction to end there; in an [XY model](statistical-physics.md#xy-model) the microscopic core instead lies beyond the smooth-field approximation. The [vortex-antivortex binding](#vortex-antivortex-binding) figure illustrates a locally nonzero charge with zero charge on a surrounding large circuit.

##### Compact phase sectors

↑ **Parent:** [Phase vortex](#phase-vortex)

An [XY model](statistical-physics.md#xy-model) orientation takes values on a circle, so a circuit around an excluded defect core can carry integer [winding number](complex-analysis.md#winding-number). Smooth single-valued [spin waves](#spin-wave) cannot change that integer without a core event or boundary crossing. The locally quadratic [order-parameter phase](#order-parameter-phase) action therefore describes a sector, rather than automatically summing every compact-field configuration. Vortex-antivortex unbinding changes the large-distance [correlation function](#correlation-function) and renormalized [phase stiffness](#phase-stiffness), even though ordinary [long-range order](statistical-physics.md#long-range-order) is already absent in two dimensions at positive [temperature](temperature.md).

##### Quantum vortex

↑ **Parent:** [Phase vortex](#phase-vortex)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_vortex)

A [quantum vortex](#quantum-vortex) has integer [winding number](complex-analysis.md#winding-number) of a condensate's [complex argument](complex-analysis.md#argument-complex-analysis). For atomic mass $m$, its [superfluid velocity](statistical-physics.md#superfluid-velocity) gives [circulation](vorticity.md#circulation-physics) $2\pi\hbar q/m$ for integer $q$. A straight vortex has a density-depleted core and, outside it, tangential [velocity](classical-mechanics.md#velocity) $q\hbar/(mr)$. Its long-range flow [energy](energy.md) is proportional to $q^2\log(R/a)$, while its [angular momentum](momentum.md#angular-momentum) has the sign of $q$.

###### Stirred-condensate vortex experiment

↑ **Parent:** [Quantum vortex](#quantum-vortex)

Rotating a trap anisotropy can nucleate vortices in an atomic condensate. Expansion followed by [absorption imaging](atomic-physics.md#absorption-imaging) resolves depleted cores, while varying rotation and waiting after removing the stirrer tests their preparation and persistence. The interpretation is quantized rotational response, rather than only the appearance of a condensed density profile.

<h6 id="inverse-square-tail-of-a-gross-pitaevskii-vortex">Inverse-square tail of a Gross–Pitaevskii vortex</h6>

↑ **Parent:** [Quantum vortex](#quantum-vortex)

In healing-length units a straight [quantum vortex](#quantum-vortex) obeys $f''+f'/r-\mathcal N^2f/r^2+(1-f^2)f=0$ and $f\to1$. Inserting $f=1-a/r^2+\cdots$ makes its order-$r^{-2}$ balance $-\mathcal N^2+2a=0$, proving the tail. The physical [healing length](quantum-ideal-gas-statistics.md#healing-length) convention must be stated; the deficit of density $1-f^2$ has twice the leading coefficient of the amplitude deficit $1-f$.

###### Matched vortex energy in a parabolic condensate

↑ **Parent:** [Quantum vortex](#quantum-vortex)

For a centered [quantum vortex](#quantum-vortex) in a [two-dimensional Thomas–Fermi condensate](quantum-ideal-gas-statistics.md#two-dimensional-thomas-fermi-condensate), use an intermediate radius $\xi_{\rm core}\ll L\ll R$. The approximately uniform core contributes $\pi n_c\hbar^2\mathcal N^2[\log(L/\xi)+L_{0|\mathcal N|}]/m$. The outer [superfluid velocity](statistical-physics.md#superfluid-velocity) is $\hbar\mathcal N/(mr)$, so its kinetic contribution is $(\pi\hbar^2\mathcal N^2/m)\int_L^R n_c(1-r^2/R^2)dr/r$. Integration cancels $L$ and produces the constant $-1/2$. The displayed result is the matched small-core approximation at fixed particle number, not a formula for arbitrarily large winding at fixed cloud size. The angular momentum is exactly $L_z=N\hbar\mathcal N$ for a normalized axisymmetric single-winding state.

###### Cubic-quintic quantum vortex tail

↑ **Parent:** [Quantum vortex](#quantum-vortex)

For a [cubic-quintic Gross–Pitaevskii equation](quantum-ideal-gas-statistics.md#cubic-quintic-gross-pitaevskii-equation) with normalized bulk amplitude one, a straight [quantum vortex](#quantum-vortex) of integer [winding number](complex-analysis.md#winding-number) $\mathcal N$ has radial equation $R''+R'/r-\mathcal N^2R/r^2+(1-\alpha R^2-\beta R^4)R=0$. With $\alpha+\beta=1$, the derivative of the nonlinear term at $R=1$ is $-2(1+\beta)$. Balancing the order-$r^{-2}$ centrifugal term with the bulk amplitude restoring term proves the displayed tail for a stable nondegenerate bulk state, $1+\beta>0$. A vortex's amplitude tends to one; its full complex field tends to $e^{i\mathcal N\theta}$, not a direction-independent constant. At $\beta=-1$ the stated inverse-square expansion cannot cancel the centrifugal term.

###### Constant far-field phase excludes net vortex winding

↑ **Parent:** [Quantum vortex](#quantum-vortex)

If a continuous nonzero complex field tends uniformly to one on large circles, its values on a sufficiently large circle lie in a disk about one that excludes zero. That disk is contractible, so the field's [winding number](complex-analysis.md#winding-number) on that circle is zero. A lone unit-charge [quantum vortex](#quantum-vortex) therefore cannot satisfy the literal boundary $\psi\to1$. For a vortex it is the [wave amplitude](wave.md#wave-amplitude), rather than the entire complex field, that can approach one; $f(r)e^{i\theta}$ gives a simple illustration of direction-dependent far-field [complex argument](complex-analysis.md#argument-complex-analysis).

###### Thermodynamic vortex-nucleation frequency

↑ **Parent:** [Quantum vortex](#quantum-vortex)

A [quantum vortex](#quantum-vortex) becomes energetically favourable in a [rotating reference frame](mathematical-physics.md#rotating-reference-frame) when $\Delta E-\Omega\Delta L_z<0$. For a singly [quantized vortex](#quantum-vortex) in a long radially Thomas–Fermi condensate, the cutoff-shell estimate is

$$
\Omega_c\simeq\frac{2\hbar}{mR_r^2}\left[\log\frac{R_r}{a_0}-\frac12\right].
$$

Integrating the trapped [number density](statistical-physics.md#number-density) against $u_\theta^2$ produces the [logarithm](calculus.md#logarithm) and constant; integrating it against [angular momentum](momentum.md#angular-momentum) per particle gives $\Delta L_z\simeq\pi Hn_0\hbar R_r^2/2$. Resolved-core corrections can alter the nonlogarithmic constant. This criterion compares equilibrium rotating-frame energies and does not remove a dynamical vortex-entry barrier.

###### Quantized circulation

↑ **Parent:** [Quantum vortex](#quantum-vortex)

Single-valuedness of the condensate field gives total [complex argument](complex-analysis.md#argument-complex-analysis) change $2\pi q$ on a closed loop avoiding zeros, where $q$ is an integer [winding number](complex-analysis.md#winding-number). Integrating the [superfluid velocity](statistical-physics.md#superfluid-velocity) around that loop gives the displayed [circulation](vorticity.md#circulation-physics). It is unchanged by smooth deformations of the loop that do not cross a [quantum vortex](#quantum-vortex).

###### Phase winding of a condensate

↑ **Parent:** [Quantized circulation](#quantized-circulation)

If a condensate order parameter stays nonzero along a closed loop, its phase changes by an integer multiple of $2\pi$. Broken [rotational symmetry](linear-algebra.md#rotational-symmetry) does not destroy this single-valuedness constraint. In an inhomogeneous ring the winding integer need not label an angular-momentum [eigenstate](energy-eigenvalue.md#eigenstate).

###### Superfluid phase slip

↑ **Parent:** [Phase winding of a condensate](#phase-winding-of-a-condensate)

An event changing the [phase winding of a condensate](#phase-winding-of-a-condensate) around a loop. A continuous nonzero order parameter cannot change its winding integer; a phase-slip path must pass through a locally vanishing amplitude or an equivalent vortex-crossing process. This use concerns a superfluid field, rather than only the relative phase of two classical oscillators.

### Quench (statistical physics)

↑ **Parent:** [Order parameter](#order-parameter)

A quench is a change of control parameters faster than the system can equilibrate. The subsequent relaxation can trap domains and [topological defects](#topological-defect).

A quench abruptly changes temperature or another control parameter and then studies the subsequent nonequilibrium relaxation of the [order parameter](#order-parameter).

### Liquid crystal

↑ **Parent:** [Order parameter](#order-parameter)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Liquid_crystal)

A liquid crystal has orientational or partial translational order while retaining some fluid mobility.

#### Blue phase

↑ **Parent:** [Liquid crystal](#liquid-crystal)

A strongly chiral liquid-crystal phase containing local double-twist order and frustrated regions. Ordered blue phases I and II have body-centered cubic and simple-cubic director/defect structures respectively, while blue phase III is disordered. The periodicity is orientational/defect order, not a molecular positional crystal lattice.

#### Columnar liquid crystal

↑ **Parent:** [Liquid crystal](#liquid-crystal)

A columnar liquid crystal has columns arranged with two-dimensional positional order transverse to the column axes and relatively fluid positional order along them. Orientational order alone, as in a [nematic liquid crystal](#nematic-liquid-crystal), does not specify this structure.

#### Isotropic phase

↑ **Parent:** [Liquid crystal](#liquid-crystal)

An isotropic phase has no preferred spatial direction. In a [liquid crystal](#liquid-crystal), its orientational [nematic order parameter](#nematic-order-parameter) vanishes, although the molecules themselves may be anisotropic.

#### Polar liquid crystal

↑ **Parent:** [Liquid crystal](#liquid-crystal)

A polar liquid crystal distinguishes head from tail and is described at leading order by a vector [polar order parameter](#polar-order-parameter) $\mathbf p$.

#### Nematic liquid crystal

↑ **Parent:** [Liquid crystal](#liquid-crystal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nematic_liquid_crystal)

A nematic liquid crystal identifies the director $\mathbf n$ with $-\mathbf n$. Its rotational order is described by a symmetric traceless tensor such as $Q_{ij}=S(n_in_j-\delta_{ij}/3)$.

##### Planar anchoring

↑ **Parent:** [Nematic liquid crystal](#nematic-liquid-crystal)

A surface preference for the [nematic director](#nematic-director) to lie tangent to the local boundary. Degenerate planar anchoring leaves the in-plane direction unselected; a directionally treated surface can instead select an azimuth. Uniform axial alignment satisfies degenerate planar anchoring on every side point of a cylindrical channel.

##### Homeotropic anchoring

↑ **Parent:** [Nematic liquid crystal](#nematic-liquid-crystal)

A surface boundary preference for the [nematic director](#nematic-director) to align normal to the local surface. Around a sphere it favors radial orientation near the surface, which must match the far-field texture.

##### Cholesteric liquid crystal

↑ **Parent:** [Nematic liquid crystal](#nematic-liquid-crystal)

A cholesteric liquid crystal is a chiral [nematic liquid crystal](#nematic-liquid-crystal) whose local [nematic director](#nematic-director) rotates helically in space. The pitch is the distance over which the director completes a full turn. It retains locally nematic orientational order without smectic density layering; the helical modulation should not be mistaken for a layer lattice.

##### Onsager excluded-volume mechanism

↑ **Parent:** [Nematic liquid crystal](#nematic-liquid-crystal)

For slender hard rods of length $L$ and diameter $D\ll L$, the leading pair [excluded volume](statistical-physics.md#excluded-volume) is the displayed function of their mutual angle $\gamma$. Alignment lowers mutual obstruction and increases positional [entropy](entropy.md), while narrowing the orientation distribution lowers orientational [entropy](entropy.md). Their competition can drive an isotropic-to-nematic transition without attractive forces. The natural concentration scale is $cL^2D$ of order one. Finite rod diameter, flexibility and interactions beyond the hard-core second-virial approximation change quantitative predictions.

##### Twisted nematic field effect

↑ **Parent:** [Nematic liquid crystal](#nematic-liquid-crystal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Twisted_nematic_field_effect)

The [twisted nematic field effect](#twisted-nematic-field-effect) switches a [nematic liquid crystal](#nematic-liquid-crystal) between a twisted optically rotating state and a largely field-aligned state. With [adiabatic optical following in a twisted nematic](#adiabatic-optical-following-in-a-twisted-nematic) and crossed [polarizers](electromagnetic-wave.md#polarizer) aligned to the two planar surface directors, a quarter-turn cell passes light at low voltage and suppresses it at high voltage. A rear reflector permits reflective operation with little power expended on light generation.

###### Adiabatic optical following in a twisted nematic

↑ **Parent:** [Twisted nematic field effect](#twisted-nematic-field-effect)

When the [birefringence](maxwell-equations.md#birefringence) separation of optical propagation constants $\Delta k=2\pi\Delta n/\lambda$ is large compared with the spatial rate of rotation of the optical axes, light with [linear polarization](electromagnetic-wave.md#linear-polarization) in a local eigenpolarization follows the twisting [nematic director](#nematic-director). Thickness alone is insufficient if [birefringence](maxwell-equations.md#birefringence) vanishes. Strong field alignment along the propagation direction suppresses the transverse optical anisotropy and hence the quarter-turn polarization rotation.

<h5 id="freedericksz-transition">Fréedericksz transition</h5>

↑ **Parent:** [Nematic liquid crystal](#nematic-liquid-crystal)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fréedericksz_transition)

The [Fréedericksz transition](#freedericksz-transition) is a field-driven orientational instability of a confined [nematic liquid crystal](#nematic-liquid-crystal). Elasticity and surface anchoring resist the [electric field](electric-field.md) or magnetic torque; a lowest allowed distortion mode becomes unstable at a finite threshold. Positive [dielectric anisotropy of a nematic](#dielectric-anisotropy-of-a-nematic) permits a normal electric field to tilt a planar anchored director.

###### Quarter-turn nematic instability threshold

↑ **Parent:** [Fréedericksz transition](#freedericksz-transition)

For planar strong anchoring and a quarter-turn base profile, $\phi'=\pi/(2L)$ and $\theta=0$. Expanding the [one-dimensional twisted nematic energy](#one-dimensional-twisted-nematic-energy) through quadratic order gives $\Delta F=\frac12\int[K_1\theta'^2+\{(K_3-2K_2)(\pi/(2L))^2-\Delta\epsilon E^2/(4\pi)\}\theta^2]dz$. The lowest zero-endpoint mode is $\sin(\pi z/L)$. Its coefficient vanishes at the displayed threshold, with $V=EL$, provided the bracket and anisotropy are positive. Halving the electric coupling doubles $V_c^2$.

##### Dielectric anisotropy of a nematic

↑ **Parent:** [Nematic liquid crystal](#nematic-liquid-crystal)

The dielectric response differs along and perpendicular to the [nematic director](#nematic-director). In Gaussian units the orientational electric contribution at prescribed field is $-\Delta\epsilon(\mathbf E\cdot\mathbf n)^2/(8\pi)$; positive anisotropy favors alignment with the [electric field](electric-field.md). The electric term does not receive the additional one-half convention used in writing the Frank elastic terms.

##### Nematic director

↑ **Parent:** [Nematic liquid crystal](#nematic-liquid-crystal)

A nematic director is a unit vector specifying the local unoriented axis of a [nematic liquid crystal](#nematic-liquid-crystal). Head-tail symmetry identifies $\mathbf n$ with $-\mathbf n$, so the order-parameter space is a [Real projective space](algebraic-topology.md#real-projective-space) rather than a sphere.

###### Independent head-tail reversal symmetry

↑ **Parent:** [Nematic director](#nematic-director)

An apolar axis model with pair [energy](energy.md) $-(\mathbf s_i\cdot\mathbf s_j)^2$ is invariant when each molecular representative is independently reversed. The [vector](vector-space.md#vector) average changes under these replacements, but the [nematic order parameter](#nematic-order-parameter) made from second moments does not. In an unbiased [statistical ensemble](thermodynamics.md#statistical-ensemble) the [vector](vector-space.md#vector) average vanishes; an individual finite representative need not have zero average. For independently chosen signs of a perfectly aligned axis, $\langle|N^{-1}\sum_i\mathbf s_i|^2\rangle=1/N$. This distinguishes exact head-tail invariance of an observable from vanishing only after an average.[§4.3, printed pp.10–11, molecular head-tail equivalence](physics-bibliography.md#lectures-on-landau-theory-of-phase-transitions-by-peter-d-olmsted)

###### Distortion free energy density

↑ **Parent:** [Nematic director](#nematic-director)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Distortion_free_energy_density)

For a unit [nematic director](#nematic-director), the bulk elastic density is $[K_1(\nabla\cdot\mathbf n)^2+K_2(\mathbf n\cdot\nabla\times\mathbf n)^2+K_3|\mathbf n\times\nabla\times\mathbf n|^2]/2$. The three positive moduli penalize [nematic splay](#nematic-splay), [nematic twist](#nematic-twist), and [nematic bend](#nematic-bend). Boundary elastic terms, chirality, or varying nematic order require additional contributions.

###### One-dimensional twisted nematic energy

↑ **Parent:** [Distortion free energy density](#distortion-free-energy-density)

For a laterally uniform [nematic director](#nematic-director) $(\cos\theta\cos\phi,\cos\theta\sin\phi,\sin\theta)$, its [divergence](multivariable-calculus.md#divergence) is $\cos\theta\,\theta'$ and its twist invariant is $-\cos^2\theta\,\phi'$. Thus $f=K_1\cos^2\theta+K_3\sin^2\theta$ and $g=K_2\cos^4\theta+K_3\sin^2\theta\cos^2\theta$. A normal [electric field](electric-field.md) contributes $-c\sin^2\theta$. The [Euler-Lagrange equations for two fields](analysis.md#euler-lagrange-equations-for-two-fields) are $(g\phi')'=0$ and $f\theta''+f_\theta\theta'^2/2-g_\theta\phi'^2/2+2c\sin\theta\cos\theta=0$.

###### Nematic bend

↑ **Parent:** [Distortion free energy density](#distortion-free-energy-density)

[Nematic bend](#nematic-bend) curves the integral lines of the [nematic director](#nematic-director). For a unit field, $(\mathbf n\cdot\nabla)\mathbf n=-\mathbf n\times(\nabla\times\mathbf n)$, so the bend energy measures curvature along those lines.

###### Nematic twist

↑ **Parent:** [Distortion free energy density](#distortion-free-energy-density)

[Nematic twist](#nematic-twist) rotates the [nematic director](#nematic-director) around an axis perpendicular to it. The helix $\mathbf n=(\cos qz,\sin qz,0)$ has zero [nematic splay](#nematic-splay) and [nematic bend](#nematic-bend), and twist density $K_2q^2/2$.

###### Nematic splay

↑ **Parent:** [Distortion free energy density](#distortion-free-energy-density)

[Nematic splay](#nematic-splay) describes local spreading or convergence of the [nematic director](#nematic-director) field. Its leading elastic cost is quadratic in the [divergence](multivariable-calculus.md#divergence) and invariant under the head-tail identification $\mathbf n\sim-\mathbf n$.

###### Nematic disclination

↑ **Parent:** [Nematic director](#nematic-director)

A nematic disclination is a topological line defect of the unoriented director field. In a two-dimensional sample its point cross-section can have half-integer winding because $\mathbf n$ and $-\mathbf n$ represent the same state.

###### Saturn-ring defect

↑ **Parent:** [Nematic disclination](#nematic-disclination)

An equatorial disclination loop surrounding a roughly spherical inclusion with [homeotropic anchoring](#homeotropic-anchoring). A meridional section cuts the loop twice. It can match a radial near-surface director to a uniform far field.

###### Nematic defect-antidefect annihilation

↑ **Parent:** [Nematic disclination](#nematic-disclination)

A neutral pair of opposite [nematic disclinations](#nematic-disclination) can annihilate under dissipative relaxation, because the total [topological charge of a two-dimensional nematic disclination](#topological-charge-of-a-two-dimensional-nematic-disclination) is zero. Its far-field elastic energy increases as $2\pi K\lambda_0^2q^2\log(R/r_0)$ with separation $R$, so the pair has an attractive elastic force proportional to $-1/R$. As opposite cores meet, the [nematic order parameter](#nematic-order-parameter) may vanish locally and the two windings disappear. Integer defects may first undergo [energetic fission of an integer nematic disclination](#energetic-fission-of-an-integer-nematic-disclination), leading to encounters of elementary half-charge defects. The actual paths and annihilation time require a dynamical law; the [free energy](thermodynamic-potential.md#thermodynamic-free-energy) alone does not specify core mobility. Pinning, imposed boundary winding or thermal defect production can obstruct a defect-free final state.

###### Logarithmic energy of a planar nematic disclination

↑ **Parent:** [Nematic disclination](#nematic-disclination)

With constant amplitude outside a core, the [planar nematic divergence-elasticity identity](#planar-nematic-divergence-elasticity-identity) reduces the elastic density to $K\lambda_0^2|\nabla\chi|^2/2$. A [topological charge of a two-dimensional nematic disclination](#topological-charge-of-a-two-dimensional-nematic-disclination) $q$ has $\chi=q\theta+\chi_0$ and $|\nabla\chi|^2=q^2/r^2$. Integrating over an annulus gives the displayed energy, plus finite core and boundary terms. The outer cutoff is the sample size, compensating-defect separation, or another screening length. An isolated defect in an infinite ordered plane has divergent energy. A neutral pair $q,-q$ separated by $R$ instead has $E_{\rm pair}=2\pi K\lambda_0^2q^2\log(R/r_0)$ plus core terms, since its far-field [gradients](multivariable-calculus.md#gradient) cancel.

###### Energetic fission of an integer nematic disclination

↑ **Parent:** [Logarithmic energy of a planar nematic disclination](#logarithmic-energy-of-a-planar-nematic-disclination)

In a strictly planar [nematic liquid crystal](#nematic-liquid-crystal), a charge-one [nematic disclination](#nematic-disclination) is a winding-two map into the circle $\mathbb{RP}^1$. Its nonzero [fundamental group](algebraic-topology.md#fundamental-group) class prevents complete unwinding while the surrounding loop stays fixed, but permits splitting into two charge-$1/2$ defects. For separation $r_0\ll d\ll L$, the two near fields contribute $\pi K\lambda_0^2(1/4+1/4)\log(d/r_0)$ while their common charge-one far field contributes $\pi K\lambda_0^2\log(L/d)$. Compared with the unsplit defect, the change is

$$
-\frac{\pi K\lambda_0^2}{2}\log(d/r_0)+\text{finite core-energy difference}.
$$

It is negative at sufficiently large scale separation. Thus integer-defect fission is energetically favorable despite conservation of total topological charge. This leading-log argument proves failure of global energetic stability, not absence of kinetic barriers or pinning. If [escape into the third dimension](#escape-into-the-third-dimension) is allowed, an integer winding can also become topologically trivial in $\mathbb{RP}^2$.

###### Tangential integer nematic defect core

↑ **Parent:** [Nematic disclination](#nematic-disclination)

For a planar tangential charge-one [nematic disclination](#nematic-disclination), $\nabla\cdot Q=-(\lambda'/2+\lambda/r)\mathbf e_r$. This follows by differentiating the tensor dyad, using $\nabla\cdot\mathbf e_\theta=0$ and $(\mathbf e_\theta\cdot\nabla)\mathbf e_\theta=-\mathbf e_r/r$. With bulk density $a\lambda^2/2+b\lambda^4/4$ and divergence elastic density $K(\lambda'/2+\lambda/r)^2/2$, radial variation of $2\pi\int rf\,dr$ gives

$$
a\lambda+b\lambda^3-\frac K4(\lambda''+\lambda'/r-4\lambda/r^2)=0.
$$

For $a<0$, a regular melted core has $\lambda=O(r^2)$ and an ordered far field has $\lambda_0=\sqrt{-a/b}$. Linearizing the bulk [derivative](calculus.md#derivative) gives $\lambda/\lambda_0=1-K/(2|a|r^2)+O(r^{-4})$. The core scale is of order $\sqrt{K/|a|}$; the amplitude disturbance has an integrable algebraic tail, rather than exactly compact support.

###### Topological charge of a two-dimensional nematic disclination

↑ **Parent:** [Nematic disclination](#nematic-disclination)

For a continuous director angle around a closed counterclockwise circuit, the enclosed topological charge is $q=\Delta\theta/(2\pi)$. Since $\theta$ is defined modulo $\pi$, elementary nematic disclinations can have $q=\pm1/2$.

###### Escape into the third dimension

↑ **Parent:** [Nematic disclination](#nematic-disclination)

A two-dimensional director winding can sometimes unwind when the director may tilt out of the plane. For a three-dimensional nematic the fundamental group of the order-parameter space is $\pi_1(\mathbb{RP}^2)=\mathbb Z/2\mathbb Z$, so two disclination lines are topologically equivalent to none.

###### One-elastic-constant nematic free energy

↑ **Parent:** [Nematic director](#nematic-director)

In the one-elastic-constant approximation, slow director distortions have a quadratic gradient energy with one modulus. For a planar angle field it reduces to $F=(K/2)\int|\nabla\theta|^2$ up to the convention-dependent effective modulus.

###### Planar nematic divergence-elasticity identity

↑ **Parent:** [One-elastic-constant nematic free energy](#one-elastic-constant-nematic-free-energy)

For a planar [nematic director](#nematic-director) $\mathbf n=(\cos\chi,\sin\chi)$ and constant amplitude $\lambda_0$, the [nematic order parameter](#nematic-order-parameter) is

$$
Q=\frac{\lambda_0}2\begin{pmatrix}\cos2\chi&\sin2\chi\\\sin2\chi&-\cos2\chi\end{pmatrix}.
$$

Differentiation gives $\nabla\cdot Q=\lambda_0(-\sin2\chi\,\chi_x+\cos2\chi\,\chi_y,\cos2\chi\,\chi_x+\sin2\chi\,\chi_y)$. The coefficient matrix is orthogonal, proving the identity. Hence $K|\nabla\cdot Q|^2/2$ is the angle-gradient energy with effective modulus $K\lambda_0^2$. The full tensor-gradient norm instead obeys $\sum_{ijk}(\partial_kQ_{ij})^2=2\lambda_0^2|\nabla\chi|^2$ in this normalization; the two local densities must not be confused.

##### Nematic order parameter

↑ **Parent:** [Nematic liquid crystal](#nematic-liquid-crystal)

###### Small-angle width of nematic orientation

↑ **Parent:** [Nematic order parameter](#nematic-order-parameter)

For a narrow [nematic liquid crystal](#nematic-liquid-crystal) orientation distribution about its unoriented [nematic director](#nematic-director), expand $S=\langle(3\cos^2\theta-1)/2\rangle=1-3\langle\theta^2\rangle/2+O(\langle\theta^4\rangle)$. This proves the displayed root-mean-square width. It does not determine the full distribution or a full width at half maximum. If the two small transverse tilt components are independent equal-variance Gaussians with variance $\sigma^2$, then $\langle\theta^2\rangle\simeq2\sigma^2$, so $\sigma\simeq\sqrt{(1-S)/3}$.

###### Effective orientation angle from nematic order

↑ **Parent:** [Nematic order parameter](#nematic-order-parameter)

For scalar [nematic order parameter](#nematic-order-parameter) $S=\langle(3\cos^2\theta-1)/2\rangle$, the displayed angle has $\cos^2\theta_{\rm eff}=\langle\cos^2\theta\rangle$. It summarizes a second moment, not the literal mean angle. For example an isotropic orientation distribution has $S=0$, giving $\theta_{\rm eff}=\arccos(1/\sqrt3)$; the average acute angle to its unoriented axis is instead one radian, obtained by integrating $\theta\sin\theta$ over $[0,\pi/2]$.

###### Uniaxial nematic order

↑ **Parent:** [Nematic order parameter](#nematic-order-parameter)

A uniaxial [nematic order parameter](#nematic-order-parameter) has one distinguished [nematic director](#nematic-director) and equal [eigenvalues](linear-operator-theory.md#eigenvalue) in its perpendicular plane. In the displayed normalization the [eigenvalues](linear-operator-theory.md#eigenvalue) are $\lambda,-\lambda/2,-\lambda/2$, giving $\operatorname{Tr}Q^2=3\lambda^2/2$ and $\operatorname{Tr}Q^3=3\lambda^3/4$. Positive and negative $\lambda$ describe prolate and oblate orientational anisotropy, respectively; reversing the [nematic director](#nematic-director) leaves the tensor unchanged.

###### Physical range of a uniaxial nematic order parameter

↑ **Parent:** [Uniaxial nematic order](#uniaxial-nematic-order)

For $S=\langle3\mathbf s\mathbf s^{\mathsf T}-I\rangle=Q(3\mathbf n\mathbf n^{\mathsf T}-I)$ and unit molecular orientations $\mathbf s$, contraction with $\mathbf n$ gives $2Q=3\langle(\mathbf s\cdot\mathbf n)^2\rangle-1$. Since the squared projection is between zero and one, the displayed bounds follow. The [eigenvalues](linear-operator-theory.md#eigenvalue) in this normalization are $2Q,-Q,-Q$. A differently normalized [nematic order parameter](#nematic-order-parameter) has correspondingly rescaled bounds; its numerical coefficients cannot be transferred unchanged.

###### Rotational invariant of a symmetric traceless tensor

↑ **Parent:** [Nematic order parameter](#nematic-order-parameter)

Under rotation by a [rotation matrix](linear-algebra.md#rotation-matrix), a [symmetric second-rank tensor](multilinear-algebra.md#symmetric-second-rank-tensor) transforms by conjugation, so its traces of powers are invariant. For a three-dimensional [traceless second-rank tensor](multilinear-algebra.md#traceless-second-rank-tensor), the [Cayley-Hamilton theorem](cayley-hamilton-theorem.md) implies $\operatorname{Tr}Q^4=(\operatorname{Tr}Q^2)^2/2$. In two dimensions its [eigenvalues](linear-operator-theory.md#eigenvalue) are $s,-s$, so $\operatorname{Tr}Q^3=0$. These identities organize the [Landau-de Gennes free energy](#landau-de-gennes-free-energy).

###### Landau-de Gennes free energy

↑ **Parent:** [Nematic order parameter](#nematic-order-parameter)

The Landau-de Gennes free energy is a [rotational symmetry](linear-algebra.md#rotational-symmetry) preserving [Landau free energy](#landau-free-energy) of the [nematic order parameter](#nematic-order-parameter). One three-dimensional normalization through fourth order is

$$
f(Q)=\frac a2\operatorname{Tr}Q^2+\frac c3\operatorname{Tr}Q^3+\frac b4(\operatorname{Tr}Q^2)^2,
\qquad b>0.
$$

The cubic invariant generically produces a [first-order phase transition](thermodynamic-potential.md#first-order-phase-transition). Its absence in two dimensions is an algebraic identity, not a guarantee that a [mean-field approximation](#mean-field-approximation) captures all fluctuations.

###### Electric-field coupling to nematic order

↑ **Parent:** [Landau-de Gennes free energy](#landau-de-gennes-free-energy)

The leading scalar coupling of an [electric field](electric-field.md) to the [nematic order parameter](#nematic-order-parameter) is quadratic in the field and linear in the tensor. For [uniaxial nematic order](#uniaxial-nematic-order), it is $-3\chi\lambda E^2(\cos^2\vartheta-1/3)/2$. When $\chi\lambda>0$, minimization aligns the [nematic director](#nematic-director) with the field axis and adds $-\chi E^2\lambda$ to the scalar [Landau free energy](#landau-free-energy).

###### Field-induced critical endpoint of the isotropic-nematic transition

↑ **Parent:** [Electric-field coupling to nematic order](#electric-field-coupling-to-nematic-order)

For a scalar [Landau-de Gennes free energy](#landau-de-gennes-free-energy) with $\bar b>0$, $\bar c<0$, and coupling $-\chi E^2\lambda$ with $\chi>0$, the [critical endpoint of a quartic Landau free energy](#critical-endpoint-of-a-quartic-landau-free-energy) is reached at the displayed field strength and $\bar a_c=3\bar c^2/(8\bar b)$, $\lambda_c=-\bar c/(4\bar b)$. It terminates the field-biased [first-order phase transition](thermodynamic-potential.md#first-order-phase-transition) when both field and quadratic coefficient can be tuned. This is a quartic small-field [mean-field approximation](#mean-field-approximation); higher terms may alter its location.

#### Director (liquid crystals)

↑ **Parent:** [Liquid crystal](#liquid-crystal)

An unoriented local axis: $\mathbf n$ and $-\mathbf n$ describe the same orientation.

### Nonconserved order-parameter dynamics

↑ **Parent:** [Order parameter](#order-parameter)

Nonconserved relaxational order-parameter dynamics has $\partial_t\psi=-\Gamma\,\delta F/\delta\psi$ plus thermal noise. Its zero-wavenumber mode may decay.

#### Gaussian Model A impulse response

↑ **Parent:** [Nonconserved order-parameter dynamics](#nonconserved-order-parameter-dynamics)

For quadratic [free energy](thermodynamic-potential.md#thermodynamic-free-energy) with positive $a,\kappa$ and [kinetic coefficient](#kinetic-coefficient) $\Gamma$, a deterministic initial [Dirac delta distribution](distribution-theory.md#dirac-delta-function) evolves under [nonconserved order-parameter dynamics](#nonconserved-order-parameter-dynamics) to the mean

$$
\langle\phi(\mathbf r,t)\rangle=\frac{Ae^{-\Gamma at}}{(4\pi\Gamma\kappa t)^{d/2}}e^{-|\mathbf r-\mathbf r'|^2/(4\Gamma\kappa t)}.
$$

Taking the expectation removes the centered [Gaussian white noise](gaussian-process.md#gaussian-white-noise); the resulting diffusion-reaction equation is solved by the [heat kernel](diffusion-equation.md#heat-kernel). The integrated mean is $Ae^{-\Gamma at}$, so spreading does not conserve the initial excess. The connected [Fourier mode](fourier-analysis.md#fourier-mode) covariance grows from zero to $k_BT/(a+\kappa q^2)$ as $1-e^{-2\Gamma(a+\kappa q^2)t}$ by the [Itô isometry](stochastic-calculus.md#ito-isometry). A realization retains equilibrium fluctuations after its mean has decayed. Pointwise continuum white-noise quantities require a coarse-graining cutoff.

#### Kinetic coefficient

↑ **Parent:** [Nonconserved order-parameter dynamics](#nonconserved-order-parameter-dynamics)

For [nonconserved order-parameter dynamics](#nonconserved-order-parameter-dynamics), the positive kinetic coefficient $\Gamma$ converts the [functional derivative](calculus-of-variations.md#functional-derivative) of the [free energy](thermodynamic-potential.md#thermodynamic-free-energy) into a relaxation rate through $\dot p=-\Gamma\,\delta F/\delta p$. [Microscopic reversibility](stochastic-thermodynamics.md#microscopic-reversibility) fixes the accompanying [Gaussian white noise](gaussian-process.md#gaussian-white-noise) variance by the [Model A fluctuation-dissipation relation](#model-a-fluctuation-dissipation-relation).

<h4 id="onsager-machlup-path-probability-for-model-a-dynamics">Onsager--Machlup path probability for Model A dynamics</h4>

↑ **Parent:** [Nonconserved order-parameter dynamics](#nonconserved-order-parameter-dynamics)

For additive Gaussian white noise of variance $\sigma^2$, a Model A trajectory has path weight proportional to

$$
\exp\left[-\frac1{2\sigma^2}\int dt\,d^dr\,
\left|\dot\phi+\Gamma\frac{\delta F}{\delta\phi}\right|^2\right].
$$

Comparing a path with its time reverse yields the free-energy change and hence the thermal fluctuation-dissipation relation.

<h4 id="onsager-machlup-path-probability">Onsager--Machlup path probability</h4>

↑ **Parent:** [Nonconserved order-parameter dynamics](#nonconserved-order-parameter-dynamics)

For additive Gaussian noise, a stochastic trajectory has probability proportional to the exponential of minus the squared noise history required to generate it. Rewriting that history in terms of the trajectory gives an Onsager--Machlup action; comparing it with the time-reversed action yields a path-probability ratio.

<h5 id="onsager-machlup-functional">Onsager–Machlup functional</h5>

↑ **Parent:** [Onsager--Machlup path probability](#onsager-machlup-path-probability)

The Onsager–Machlup functional is the action in the exponential of an additive Gaussian stochastic path probability. For $\dot x=b(x)+\sigma\Lambda$, its elementary discretization contains $\int|\dot x-b(x)|^2/(2\sigma^2)\,dt$, with convention-dependent Jacobian terms for multiplicative or state-dependent drift.

##### Time-reversal invariance of a path Jacobian

↑ **Parent:** [Onsager--Machlup path probability](#onsager-machlup-path-probability)

For additive [Gaussian white noise](gaussian-process.md#gaussian-white-noise) and a time-even [order parameter](#order-parameter), a midpoint discretization of the [Onsager–Machlup functional](#onsager-machlup-functional) evaluates drift derivatives at the midpoint configurations. Reversing a trajectory visits the same midpoints in reverse order, so the noise-to-path [Jacobian determinant](multivariable-calculus.md#jacobian-determinant) is invariant under reversal. It may depend on the trajectory, and must be distinguished from the constant normalization of the noise measure.

For [nonconserved order-parameter dynamics](#nonconserved-order-parameter-dynamics) with $\dot p=-\Gamma\mu[p]+f$, the factor at one time step, apart from a path-independent power of the step size, is

$$
\mathcal J_n=\left|\det\left[I+\frac{\Gamma\Delta t}{2}\mathcal H_n\right]\right|,
\qquad \mathcal H_n=\frac{\partial\mu}{\partial p}\bigg|_{(p_n+p_{n+1})/2}.
$$

Here the fields have first been restricted to a finite spatial grid, and $\mathcal H_n$ is the [Hessian matrix](multivariable-calculus.md#hessian-matrix) of the [free energy](thermodynamic-potential.md#thermodynamic-free-energy).

For [mixed conserved and nonconserved order-parameter dynamics](#mixed-conserved-and-nonconserved-order-parameter-dynamics), the required noises for a joint configuration and flux trajectory are

$$
f_n=\frac{p_{n+1}-p_n}{\Delta t}+\mathsf D W_n+\Gamma\mu_n,
\qquad N_n=W_n+M\mathsf G\mu_n,
$$

where $\mathsf D,\mathsf G$ represent the [divergence](multivariable-calculus.md#divergence) and [gradient](multivariable-calculus.md#gradient), and $\Delta=\mathsf D\mathsf G$ represents the [Laplacian](multivariable-calculus.md#laplacian). The [Jacobian matrix](multivariable-calculus.md#jacobian-matrix) is

$$
\frac{\partial(f_n,N_n)}{\partial(p_{n+1},W_n)}=
\begin{pmatrix}
\frac{I}{\Delta t}+\Gamma\mathcal H_n/2&\mathsf D\\
M\mathsf G\mathcal H_n/2&I
\end{pmatrix}.
$$

Taking its [Schur complement](linear-algebra.md#schur-complement) gives the joint factor

$$
\boxed{\mathcal J_n=\left|\det\left[I+\frac{\Delta t}{2}(\Gamma I-M\Delta)\mathcal H_n\right]\right|.}
$$

For [periodic boundary conditions](differential-equation.md#periodic-boundary-conditions), discretizing the two spatial operators compatibly gives $\mathsf D=-\mathsf G^{\mathsf T}$, so $\Gamma I-M\Delta$ is the positive relaxation operator when $\Gamma,M>0$. Reversal leaves $\mathcal H_n$ unchanged and reverses the sign of the flux. The product of the joint factors is consequently the same for both histories, justifying its cancellation from the [joint path probability of an order parameter and its flux](#joint-path-probability-of-an-order-parameter-and-its-flux). The [functional chain rule](calculus-of-variations.md#functional-chain-rule) used in the action ratio holds in the continuum limit of this midpoint convention.

#### Model A fluctuation-dissipation relation

↑ **Parent:** [Nonconserved order-parameter dynamics](#nonconserved-order-parameter-dynamics)

For [nonconserved order-parameter dynamics](#nonconserved-order-parameter-dynamics), [microscopic reversibility](stochastic-thermodynamics.md#microscopic-reversibility) with equilibrium weight proportional to $e^{-F/(k_BT)}$ requires

$$
\sigma^2=2\Gamma k_BT.
$$

Indeed the [Onsager--Machlup path probability](#onsager-machlup-path-probability) gives $\log(P_F/P_B)=-2\Gamma\int\dot p\,\delta F/\delta p\,dt/\sigma^2=-2\Gamma(F_2-F_1)/\sigma^2$. Equating this to the [detailed balance](markov-chain.md#detailed-balance) value proves the relation. The [functional chain rule](calculus-of-variations.md#functional-chain-rule) is understood with the same midpoint convention as the path action.

#### Gaussian Model A quench

↑ **Parent:** [Nonconserved order-parameter dynamics](#nonconserved-order-parameter-dynamics)

After a sudden change from quadratic kernel $K_I(q)$ to $K_F(q)$, each Fourier mode is an [Ornstein-Uhlenbeck process](gaussian-process.md#ornstein-uhlenbeck-process) with decay rate $r(q)=\Gamma K_F(q)$. Its equal-time covariance interpolates exponentially between $k_BT/K_I(q)$ and $k_BT/K_F(q)$.

### Conserved order-parameter dynamics

↑ **Parent:** [Order parameter](#order-parameter)

Conserved relaxational order-parameter dynamics has $\partial_t\phi=M\nabla^2(\delta F/\delta\phi)$ plus conserved thermal noise. Its relaxation rate vanishes as $q^2$ at small wavenumber.

#### Order-parameter mobility

↑ **Parent:** [Conserved order-parameter dynamics](#conserved-order-parameter-dynamics)

The positive order-parameter mobility $M$ relates the diffusive transport flux to the [chemical potential](chemical-potential.md) gradient: $\mathbf J=-M\nabla\mu$. Combining this law with local conservation gives the [Cahn--Hilliard equation](#cahn-hilliard-equation) when $\mu$ is the [functional derivative](calculus-of-variations.md#functional-derivative) of a composition [free energy](thermodynamic-potential.md#thermodynamic-free-energy).

#### Fluctuation-dissipation relation for a conserved flux

↑ **Parent:** [Conserved order-parameter dynamics](#conserved-order-parameter-dynamics)

For the flux $W_{ij}=-M\partial_i\mu_j+N_{ij}$ of a [vector order parameter](#vector-order-parameter), [microscopic reversibility](stochastic-thermodynamics.md#microscopic-reversibility) requires independent [Gaussian white noise](gaussian-process.md#gaussian-white-noise) components with covariance

$$
\langle N_{ij}(\mathbf r,t)N_{kl}(\mathbf r',t')\rangle
=2Mk_BT\,\delta_{ik}\delta_{jl}\delta(\mathbf r-\mathbf r')\delta(t-t').
$$

The current changes sign under time reversal. The resulting path-probability ratio contributes $-(k_BT)^{-1}\int W_{ij}\partial_i\mu_j$ to its logarithm; [integration by parts](calculus.md#integration-by-parts) converts this to the free-energy loss from the conserved dynamics.

#### Hydrodynamic mode

↑ **Parent:** [Conserved order-parameter dynamics](#conserved-order-parameter-dynamics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hydrodynamic_mode)

A hydrodynamic mode is a long-wavelength collective mode whose decay rate tends to zero because of a conservation law. Coupling to fast nonconserved variables renormalizes its diffusivity and eigenvector.

### Mixed conserved and nonconserved order-parameter dynamics

↑ **Parent:** [Order parameter](#order-parameter)

With constant positive [kinetic coefficient](#kinetic-coefficient) $\Gamma$ and [mobility](#order-parameter-mobility) $M$, two independent relaxation channels give

$$
\dot p_j=-\partial_iW_{ij}-\Gamma\mu_j+f_j,
\qquad W_{ij}=-M\partial_i\mu_j+N_{ij},
\qquad\mu_j=\frac{\delta F}{\delta p_j}.
$$

The deterministic mobility operator is $\Gamma-M\nabla^2$. Each channel separately satisfies [microscopic reversibility](stochastic-thermodynamics.md#microscopic-reversibility) when its noise obeys the corresponding [Model A fluctuation-dissipation relation](#model-a-fluctuation-dissipation-relation) or [fluctuation-dissipation relation for a conserved flux](#fluctuation-dissipation-relation-for-a-conserved-flux).

#### Joint path probability of an order parameter and its flux

↑ **Parent:** [Mixed conserved and nonconserved order-parameter dynamics](#mixed-conserved-and-nonconserved-order-parameter-dynamics)

Put $u_j=\dot p_j+\partial_iW_{ij}$. The additive independent noises give the forward action

$$
S_F=\int\left[\frac{|u+\Gamma\mu|^2}{2\sigma^2}
+\frac{|W+M\nabla\mu|^2}{2\sigma_N^2}\right]d\mathbf r\,dt.
$$

For a time-even [order parameter](#order-parameter) and time-odd flux, the backward action replaces $u,W$ by $-u,-W$ while keeping $\mu$ fixed on the corresponding configurations. Common normalization and [time-reversal invariance of a path Jacobian](#time-reversal-invariance-of-a-path-jacobian) then give

$$
\log\frac{P_F}{P_B}
=-\frac{2\Gamma}{\sigma^2}\int\mu_j(\dot p_j+\partial_iW_{ij})
-\frac{2M}{\sigma_N^2}\int W_{ij}\partial_i\mu_j.
$$

At the two thermal noise strengths, periodic [boundary conditions](differential-equation.md#boundary-condition) cancel the two spatial terms by [integration by parts](calculus.md#integration-by-parts), leaving $-(F_2-F_1)/(k_BT)$. Thus the joint dynamics satisfies [microscopic reversibility](stochastic-thermodynamics.md#microscopic-reversibility).

### Compositional order parameter

↑ **Parent:** [Order parameter](#order-parameter)

A compositional order parameter is a local concentration difference in a mixture. In a closed system its spatial integral is fixed, so its dynamics must take continuity-equation form.

#### Binary fluid mixture

↑ **Parent:** [Compositional order parameter](#compositional-order-parameter)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Binary_fluid_mixture)

A binary fluid mixture contains two molecular species whose local concentration difference can undergo mixing or phase separation.

##### Surfactant renormalization of the square-gradient coefficient

↑ **Parent:** [Binary fluid mixture](#binary-fluid-mixture)

If a nonconserved surfactant polarization has local energy $\nu|\mathbf p|^2/2+\lambda\mathbf p\cdot\nabla\phi$, eliminating $\mathbf p$ changes the composition-gradient coefficient from $\kappa$ to $\widetilde\kappa=\kappa-\lambda^2/\nu$. This expresses the surfactant's reduction of interfacial energy.

##### Microemulsion

↑ **Parent:** [Binary fluid mixture](#binary-fluid-mixture)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Microemulsion)

A microemulsion is a thermodynamically stable mixture of immiscible fluids and surfactant with structure on a mesoscopic length scale. In a gradient theory, a negative square-gradient coefficient stabilized by a positive fourth-gradient term favors fluctuations at nonzero wavevector.

<h5 id="cahn-hilliard-equation">Cahn--Hilliard equation</h5>

↑ **Parent:** [Binary fluid mixture](#binary-fluid-mixture)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cahn--Hilliard_equation)

The Cahn--Hilliard equation transports a conserved composition field down gradients of its chemical potential: $\partial_t\phi=\nabla\mathbin\cdot(M\nabla\mu)$ with $\mu=\delta F/\delta\phi$. Advection adds $\mathbf v\mathbin\cdot\nabla\phi$ to the left-hand side.

##### Ostwald ripening

↑ **Parent:** [Binary fluid mixture](#binary-fluid-mixture)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ostwald_ripening)

In Ostwald ripening, the higher interfacial [chemical potential](chemical-potential.md) of small droplets drives diffusion toward larger droplets, increasing the characteristic domain size. The [Gibbs--Thomson relation](surface-tension.md#gibbs-thomson-relation) supplies the curvature-dependent surface value, while [conserved order-parameter dynamics](#conserved-order-parameter-dynamics) controls transport through the surrounding phase.

###### Diffusion-controlled droplet growth

↑ **Parent:** [Ostwald ripening](#ostwald-ripening)

For a three-dimensional droplet with concentration jump $\Delta\phi$, constant [mobility](#order-parameter-mobility) $M$, and quasi-static exterior [chemical potential](chemical-potential.md),

$$
\mu(r)=\mu_\infty+(\mu_s-\mu_\infty)\frac Rr,
\qquad
\dot R=-\frac{M(\mu_s-\mu_\infty)}{\Delta\phi\,R}.
$$

The first formula solves the exterior [Laplace equation](partial-differential-equation.md#laplace-equation). The second follows from conservation: the total outward flux $4\pi MR(\mu_s-\mu_\infty)$ removes excess composition at the rate $-4\pi R^2\Delta\phi\,\dot R$. For a symmetric mixture, $\Delta\phi=2\phi_B$ and the [Gibbs--Thomson relation](surface-tension.md#gibbs-thomson-relation) gives $\mu_s=\gamma/(\phi_B R)$.

###### Constant-reservoir diffusion-controlled particle growth

↑ **Parent:** [Diffusion-controlled droplet growth](#diffusion-controlled-droplet-growth)

For an isolated growing [sphere](euclidean-geometry.md#sphere), a quasi-steady exterior [diffusion equation](diffusion-equation.md), constant surface [concentration](mathematical-physics.md#concentration) $c_s$, and a maintained far-field [concentration](mathematical-physics.md#concentration) $c_\infty$ give $c(r)=c_\infty-(c_\infty-c_s)a/r$. A sharp moving boundary with interior [concentration](mathematical-physics.md#concentration) $c_p$ then obeys $(c_p-c_s)\dot a=D(c_\infty-c_s)/a$. The displayed integrated law assumes all concentrations and the [diffusion coefficient](brownian-motion.md#diffusion-coefficient) are constant. It becomes $a\propto\sqrt t$ when the seed radius is negligible. This reservoir-fed law differs from curvature-controlled [Ostwald ripening](#ostwald-ripening) in a depleting many-particle system.

###### Surface-reaction-controlled particle growth

↑ **Parent:** [Constant-reservoir diffusion-controlled particle growth](#constant-reservoir-diffusion-controlled-particle-growth)

When attachment is much slower than exterior [diffusion](thermodynamics.md#diffusion), the surface [concentration](mathematical-physics.md#concentration) stays close to the reservoir value. An attachment coefficient $k_s$ with units of [velocity](classical-mechanics.md#velocity) gives nearly constant radial growth in the dilute-feed approximation. For a [sphere](euclidean-geometry.md#sphere) the ratio $k_sa/D$ distinguishes attachment control from transport control. A finite attachment rate leads to a [Robin boundary condition](differential-equation.md#robin-boundary-condition) rather than a fixed equilibrium surface concentration.

###### Diffusion-capacitance analogy

↑ **Parent:** [Diffusion-controlled droplet growth](#diffusion-controlled-droplet-growth)

A quasi-static [chemical potential](chemical-potential.md) outside a fixed-shape droplet solves the same [Laplace equation](partial-differential-equation.md#laplace-equation) as an [electrostatic potential](electric-field.md#electric-potential) outside an equipotential conductor. If $\mu=\mu_s$ on the droplet and zero on the surrounding reservoirs, its outward diffusive current is

$$
I=-M\int_{\partial D}\partial_n\mu\,dS
=\frac M\epsilon C\mu_s,
$$

where $C$ is the corresponding electrostatic [capacitance](electromagnetism.md#capacitance) in a medium of [permittivity](permittivity.md) $\epsilon$. The arbitrary $\epsilon$ cancels against the capacitance's proportionality to $\epsilon$. Thus electrostatic geometry directly determines evaporation rates.

###### Droplet evaporation near a planar reservoir

↑ **Parent:** [Diffusion-controlled droplet growth](#diffusion-controlled-droplet-growth)

For a spherical droplet at fixed center height $h>R$ above a flat equilibrium reservoir, the [diffusion-capacitance analogy](#diffusion-capacitance-analogy) and [sphere-plane capacitance](electromagnetism.md#sphere-plane-capacitance) give

$$
\dot R=-\frac{M\gamma}{2\phi_B^2R^2}\,c(R/h),
\qquad
\tau=\frac{2\phi_B^2}{M\gamma}\int_0^{R_0}\frac{R^2}{c(R/h)}\,dR.
$$

At large separation, $c(R/h)=1+R/(2h)+O((R/h)^2)$, so

$$
\tau=\frac{2\phi_B^2R_0^3}{3M\gamma}
\left[1-\frac{3R_0}{8h}+O((R_0/h)^2)\right].
$$

The nearby reservoir increases the total flux and shortens the lifetime. The spherical-shape assumption controls the geometry; the local current density is not uniform over the surface.

##### Model H dynamics

↑ **Parent:** [Binary fluid mixture](#binary-fluid-mixture)

Model H couples a conserved scalar composition field to an incompressible momentum density. It combines the advective [Cahn--Hilliard equation](#cahn-hilliard-equation) with the [Navier-Stokes equation](viscous-fluid-flow.md#navier-stokes-equation) and the thermodynamic force density $-\phi\nabla\mu$.

###### Energy dissipation identity for Model H

↑ **Parent:** [Model H dynamics](#model-h-dynamics)

For constant positive [order-parameter mobility](#order-parameter-mobility) $M$, [dynamic viscosity](dynamic-viscosity.md) $\eta$ and [mass density](fluid-mechanics.md#density) $\rho$, deterministic [Model H dynamics](#model-h-dynamics) dissipates the sum of composition [free energy](thermodynamic-potential.md#thermodynamic-free-energy) and kinetic energy:

$$
\frac{d}{dt}\left[F+\frac\rho2\int|\mathbf v|^2\right]=-\int[M|\nabla\mu|^2+\eta|\nabla\mathbf v|^2]\le0.
$$

Assume smooth fields and periodic or closed, no-work boundaries. Using the [chemical potential of a composition field](chemical-potential.md#chemical-potential-of-a-composition-field), [integration by parts](calculus.md#integration-by-parts) and [incompressible flow](fluid-mechanics.md#incompressible-flow) gives $\dot F=\int\phi\mathbf v\cdot\nabla\mu-M\int|\nabla\mu|^2$. Dotting the momentum equation with velocity gives $\dot E_{\rm kin}=-\int\phi\mathbf v\cdot\nabla\mu-\eta\int|\nabla\mathbf v|^2$. [Pressure](pressure.md) and convective work vanish under the boundary assumptions; the two capillary transfer terms cancel. This proves both the sign of the [Korteweg force](#korteweg-force) and its reversible exchange of energy with the composition field.

###### Korteweg force

↑ **Parent:** [Model H dynamics](#model-h-dynamics)

The Korteweg force is the capillary body-force density generated by composition gradients in a diffuse-interface fluid. Up to a pressure gradient it can be written $-\phi\nabla\mu$, where $\mu$ is the chemical potential.

###### Bicontinuous phase separation

↑ **Parent:** [Model H dynamics](#model-h-dynamics)

In bicontinuous phase separation, both fluid phases form interpenetrating connected domains. During late-stage coarsening their morphology is often statistically self-similar after lengths are divided by one characteristic domain size $L(t)$.

###### Dynamical scaling of binary-fluid coarsening

↑ **Parent:** [Bicontinuous phase separation](#bicontinuous-phase-separation)

The dynamical-scaling hypothesis replaces all macroscopic lengths by one scale $L(t)$ and the characteristic velocity by $\dot L$. Then inertial, viscous, and capillary force densities scale respectively as $\rho\ddot L+\rho\dot L^2/L$, $\eta\dot L/L^2$, and $\sigma/L^2$.

###### Drag-limited hydrodynamic coarsening

↑ **Parent:** [Dynamical scaling of binary-fluid coarsening](#dynamical-scaling-of-binary-fluid-coarsening)

Replacing domain-scale viscous stresses by a local [linear drag](fluid-mechanics.md#linear-drag) density $-\bar\eta\mathbf v$ gives the scales $L_1=(\sigma\rho/\bar\eta^2)^{1/3}$ and $t_1=\rho/\bar\eta$. The single-scale force model is

$$
\alpha g''+\beta g'^2/g=-c_dg'+c_s/g^2,\qquad L=L_1g(t/t_1),\quad c_d,c_s>0.
$$

For a regular power-law asymptotic $g\sim Cu^y$, $g'\sim Cyu^{y-1}$, $g''=Cy(y-1)u^{y-2}+o(u^{y-2})$, $y>0$, the two inertial-to-drag ratios scale as $(y-1)/u$ and $y/u$. Thus drag dominates inertia at late time, and drag-capillary balance integrates to $g^3\sim3(c_s/c_d)u$. This proves the displayed $1/3$ exponent and its independence of [mass density](fluid-mechanics.md#density). The scaling assumes a homogenized stationary network and dominant advective transport. Diffusive [Ostwald ripening](#ostwald-ripening) can have the same exponent, so its omission must be justified separately; [order-parameter mobility](#order-parameter-mobility) can otherwise enter the prefactor.

###### Hydrodynamic coarsening crossover scales

↑ **Parent:** [Dynamical scaling of binary-fluid coarsening](#dynamical-scaling-of-binary-fluid-coarsening)

Under single-length [dynamical scaling of binary-fluid coarsening](#dynamical-scaling-of-binary-fluid-coarsening), [mass density](fluid-mechanics.md#density) $\rho$, [dynamic viscosity](dynamic-viscosity.md) $\eta$ and [surface tension](surface-tension.md) $\sigma$ determine the displayed unique length and time scales by [dimensional analysis](mathematical-physics.md#dimensional-analysis). Writing $L=L_0f(t/t_0)$ reduces the force-density estimate to $\alpha f''+\beta f'^2/f=\gamma f'/f^2+\delta/f^2$. Resistive and driving terms need opposite signed geometric coefficients. [Viscous hydrodynamic coarsening](#viscous-hydrodynamic-coarsening) has $f\sim u$ and [inertial hydrodynamic coarsening](#inertial-hydrodynamic-coarsening) has $f\sim u^{2/3}$. These follow respectively from density-independent and viscosity-independent powers in $L\propto\eta^{2-3p}\rho^{p-1}\sigma^{2p-1}t^p$. They require thin interfaces, statistically self-similar bicontinuous domains, dominant advection and no additional relevant macroscopic scales. A degeneracy in the signed inertial coefficients can invalidate the pure-power force balance without invalidating the dimensional calculation.

###### Viscous hydrodynamic coarsening

↑ **Parent:** [Dynamical scaling of binary-fluid coarsening](#dynamical-scaling-of-binary-fluid-coarsening)

Balancing viscous and capillary forces gives $L(t)\sim(\sigma/\eta)t$. This regime is independent of the mass density and applies below the viscous-to-inertial crossover scale.

###### Inertial hydrodynamic coarsening

↑ **Parent:** [Dynamical scaling of binary-fluid coarsening](#dynamical-scaling-of-binary-fluid-coarsening)

Balancing inertia and capillarity gives $L(t)\sim(\sigma/\rho)^{1/3}t^{2/3}$. This regime is independent of viscosity and applies above the viscous-to-inertial crossover scale.

###### Stirring-arrested binary-fluid domain size

↑ **Parent:** [Dynamical scaling of binary-fluid coarsening](#dynamical-scaling-of-binary-fluid-coarsening)

If stirring imposes a time scale $\tau$, replacing time derivatives by $1/\tau$ predicts a steady domain size. Viscous-capillary balance gives $\Lambda\sim\sigma\tau/\eta$, while inertial-capillary balance gives $\Lambda\sim(\sigma\tau^2/\rho)^{1/3}$.

### Polar order parameter

↑ **Parent:** [Order parameter](#order-parameter)

A polar order parameter is a vector whose direction distinguishes head from tail. In an isotropic medium without an external polar field, spatial inversion makes the free energy even under $\mathbf p\mapsto-\mathbf p$.

#### Polar molecular field

↑ **Parent:** [Polar order parameter](#polar-order-parameter)

The polar molecular field is the [functional derivative](calculus-of-variations.md#functional-derivative) of the [free energy](thermodynamic-potential.md#thermodynamic-free-energy) with respect to the [polar order parameter](#polar-order-parameter). In the positive-derivative convention, dissipative dynamics is $D_t\mathbf p=-\Gamma\mathbf h$ with positive [kinetic coefficient](#kinetic-coefficient). For a quartic local term and an isotropic gradient penalty,

$$
h_i=(a+b|\mathbf p|^2)p_i-\kappa\nabla^2p_i.
$$

Some authors instead define the molecular field with a minus sign, which changes the associated stress and evolution conventions.

#### Flow alignment of a polar order parameter

↑ **Parent:** [Polar order parameter](#polar-order-parameter)

The material derivative of a polar order parameter contains rigid rotation with the local vorticity and a material-dependent alignment response to the symmetric strain-rate tensor.

##### Tumbling of a polar order parameter

↑ **Parent:** [Flow alignment of a polar order parameter](#flow-alignment-of-a-polar-order-parameter)

In [simple shear flow](viscous-fluid-flow.md#simple-shear-flow), a persistent [polar order parameter](#polar-order-parameter) with $|\xi|<1$ has no fixed angle and rotates continuously. Integrating $\dot\theta=g(\xi\cos2\theta-1)/2$ through $2\pi$ gives the displayed period. An unoriented [nematic director](#nematic-director) repeats after half that time. At $\xi=0$, the magnitude relaxes independently while the angular speed is $-g/2$.

##### Flow-alignment angle in planar shear

↑ **Parent:** [Flow alignment of a polar order parameter](#flow-alignment-of-a-polar-order-parameter)

For a uniform [polar order parameter](#polar-order-parameter) in [simple shear flow](viscous-fluid-flow.md#simple-shear-flow) $\mathbf v=(gy,0)$, the angular equation is $\dot\theta=g(\xi\cos2\theta-1)/2$. A fixed orientation for nonzero shear therefore requires $|\xi|\ge1$. For $|\xi|>1$, its angular stability condition is $g\xi\sin2\theta>0$; equality at $|\xi|=1$ requires nonlinear analysis. The ordered magnitude must separately satisfy the radial stationarity equation and be nonzero.

##### Order-parameter stress

↑ **Parent:** [Flow alignment of a polar order parameter](#flow-alignment-of-a-polar-order-parameter)

An advected order parameter contributes stress because a velocity gradient changes its free energy. For a polar vector this includes distortion, antisymmetric rotational, and symmetric flow-alignment stresses involving the molecular field.

###### Reversible stress of a polar liquid crystal

↑ **Parent:** [Order-parameter stress](#order-parameter-stress)

Using the positive [polar molecular field](#polar-molecular-field) $h_i=\delta F/\delta p_i$ and [velocity gradient](continuum-mechanics.md#velocity-gradient) $\partial_i v_j$, the reversible [order-parameter stress](#order-parameter-stress) consists of a distortion contribution and rotational and alignment contributions:

$$
\Sigma^p_{ij}=\Sigma^{(1)}_{ij}
+\frac{p_i h_j-p_jh_i}{2}
+\frac{\xi(p_i h_j+p_jh_i)}2,
\qquad \partial_i\Sigma^{(1)}_{ij}=-p_k\partial_jh_k.
$$

For a local [free-energy density](statistical-physics.md#free-energy-density), a representative is $\Sigma^{(1)}_{ij}=(f-p_kh_k)\delta_{ij}-f_{\partial_i p_k}\partial_jp_k$. The [Euler-Lagrange equation](analysis.md#euler-lagrange-equation) verifies its [divergence](multivariable-calculus.md#divergence). [Integration by parts](calculus.md#integration-by-parts) gives $\delta F=\int\Sigma^p_{ij}\partial_i u_j$ for an incompressible displacement without surface work; the corresponding mechanical power has the opposite sign. [Pressure](pressure.md) contributions may be reassigned in an [incompressible flow](fluid-mechanics.md#incompressible-flow).

## Landau theory

↑ **Parent:** [Critical phenomenon](critical-phenomenon.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Landau_theory)

Landau theory expands an effective free energy analytically in powers of an [order parameter](#order-parameter), constrained by symmetry.

### Arrott plot

↑ **Parent:** [Landau theory](#landau-theory)

An [Arrott plot](#arrott-plot) presents squared magnetisation against field divided by magnetisation. For the uniform SI Landau equation $\mu_0H=aM+bM^3$, it is a straight line

$$
M^2=\frac{\mu_0}{b}\frac HM-\frac ab.
$$

The critical mean-field isotherm has $a=0$ and passes through the origin. Horizontal intercept $a/\mu_0$ changes sign across the transition; a positive vertical intercept estimates spontaneous magnetisation squared. The original criterion concerns internal [magnetic field](magnetic-field.md) and the molecular-field regime. Demagnetizing fields and non-mean-field [critical exponents](#critical-exponent) require additional care.[1957, abstract: cubic magnetisation proportional to internal field at the Curie point](physics-bibliography.md#criterion-for-ferromagnetism-from-observations-of-magnetic-isotherms-by-anthony-arrott)

#### Extracting magnetic Landau coefficients from an Arrott plot

↑ **Parent:** [Arrott plot](#arrott-plot)

If physical ordinate is $Y=M^2$ and abscissa $X=H/M$, slope $S=dY/dX$ and horizontal intercept $X_0$ give $b=\mu_0/S$ and $a=\mu_0X_0$. Any displayed squared-magnetisation scale must be converted before using S. For example, an ordinate unit $(10^4\,\mathrm{A\,m^{-1}})^2$ equals $10^8\,\mathrm{A^2\,m^{-2}}$, not $10^4$. With a [free-energy density](statistical-physics.md#free-energy-density), the resulting units are $[a]=\mathrm{H\,m^{-1}}$ and $[b]=\mathrm{J\,m\,A^{-4}}$. [Curvature](differential-geometry.md#curvature) or differing isotherm slopes limits the accuracy of a constant-coefficient fit.

### Ginzburg-Landau theory

↑ **Parent:** [Landau theory](#landau-theory)

A long-wavelength order-parameter description extending a local [Landau free energy](#landau-free-energy) by gradient terms. For a one-component complex field, a common isotropic form is $\mathcal F=\int[\alpha|\Psi|^2+\beta|\Psi|^4/2+K|\nabla\Psi|^2]d^3r$. A charged field instead uses a covariant gradient. Static minimization determines equilibrium profiles; a dynamical law requires additional input. [Ginzburg-Landau theory of superconductivity](superconductivity.md#ginzburg-landau-theory-of-superconductivity) and the [Ginzburg-Landau functional of a dilute Bose gas](#ginzburg-landau-functional-of-a-dilute-bose-gas) realize this structure with different microscopic normalizations.

#### Ginzburg-Landau functional of a dilute Bose gas

↑ **Parent:** [Ginzburg-Landau theory](#ginzburg-landau-theory)

Take $\Psi=\langle\widehat\psi\rangle$ normalized so that $|\Psi|^2$ is condensate density. The coherent-field expectation of a dilute contact-interacting Bose Hamiltonian gives the grand-potential functional $\int[\hbar^2|\nabla\Psi|^2/(2m_B)+(V_{\rm ext}-\mu)|\Psi|^2+g_B|\Psi|^4/2]d^3r$. Its leading microscopic coefficients are therefore those displayed, with positive [s-wave scattering length](quantum-scattering.md#s-wave-scattering-length) $a_s$ for repulsion. Varying with respect to $\Psi^*$ gives the stationary [Gross–Pitaevskii equation](quantum-ideal-gas-statistics.md#gross-pitaevskii-equation). Thermal and quantum fluctuations can renormalize the coefficients; these mean-field identities are not exact universal critical coefficients.

### Quartic Landau equilibrium branches

↑ **Parent:** [Landau theory](#landau-theory)

For $f=f_0+a(T-T_c)q^2/2+bq^4/4$ with $a,b>0$, the minimum is $q=0$ above $T_c$ and $q=\pm\sqrt{a(T_c-T)/b}$ below it. The stationary solutions must be checked for stability; below $T_c$ the central solution is a maximum.

### Sign-reversal symmetry in Landau theory

↑ **Parent:** [Landau theory](#landau-theory)

A scalar [order parameter](#order-parameter) with symmetry $q\mapsto-q$ has only even powers in its zero-field [free energy](thermodynamic-potential.md#thermodynamic-free-energy). A conjugate field contributes $-hq$. Without this symmetry, odd terms can be allowed and change the transition structure.

### Analytic vector Landau expansion

↑ **Parent:** [Landau theory](#landau-theory)

For an isotropic [vector](vector-space.md#vector) [order parameter](#order-parameter), an analytic scalar [Landau free energy](#landau-free-energy) near the origin contains powers of $\mathbf m\cdot\mathbf m$. Odd powers of its magnitude are rotationally invariant but nonanalytic as functions of the Cartesian components at zero; excluding them requires analyticity, not merely writing the magnitude as a nonnegative scalar. With $d>0$, changing $b$ from positive to negative continuously creates minima at $|\mathbf m|=\sqrt{-b/(2d)}$, with an arbitrary direction.[§4.2, rotationally invariant vector expansion](physics-bibliography.md#statistical-field-theory-by-david-tong)

### Heat-capacity jump in quartic Landau theory

↑ **Parent:** [Landau theory](#landau-theory)

For zero field, $F=F_0+b(T-T_c)M^2+dM^4$ with $b,d>0$ has ordered minima $M^2=b(T_c-T)/(2d)$ below $T_c$. Minimizing gives $F_{\min}=F_0-b^2(T-T_c)^2/(4d)$. Since $C=-T\partial_T^2F_{\min}$, the ordered-phase excess [heat capacity](heat.md#heat-capacity) is $Tb^2/(2d)$ and its jump relative to the disordered side is $T_cb^2/(2d)$. The value is a total [heat capacity](heat.md#heat-capacity) or a heat-capacity density according to the normalization of $F$.

#### Curie heat-capacity density from an Arrott plot

↑ **Parent:** [Heat-capacity jump in quartic Landau theory](#heat-capacity-jump-in-quartic-landau-theory)

For [density](fluid-mechanics.md#density) $F=\alpha(T-T_c)M^2/2+bM^4/4-\mu_0HM$, the zero-field ordered minimum is $-\alpha^2(T-T_c)^2/(4b)$. Its constant-field heat-capacity [density](fluid-mechanics.md#density) jump is $\Delta c_H=T_c\alpha^2/(2b)$. In an [Arrott plot](#arrott-plot), let physical slope be $S=\mu_0/b$ and horizontal intercept be $X_0(T)=a(T)/\mu_0$. Then

$$
\Delta c_H=\frac{T_c\mu_0S}{2}\left(\frac{dX_0}{dT}\right)^2.
$$

This makes numerical sensitivity explicit: uncertainty in the intercept slope is squared. A volumetric [free energy](thermodynamic-potential.md#thermodynamic-free-energy) determines a volumetric heat-capacity jump; total or molar values need further sample information.

### Mean-field approximation

↑ **Parent:** [Landau theory](#landau-theory)

The mean-field approximation replaces interactions with a self-consistent average field, neglecting correlated fluctuations around that average.

This is a use of [mean-field theory](statistical-physics.md#mean-field-theory), whose general framework also applies beyond a Landau free-energy model.

#### Self-consistency equation

↑ **Parent:** [Mean-field approximation](#mean-field-approximation)

A self-consistency equation requires the average field assumed in a [mean-field approximation](#mean-field-approximation) to equal the expectation value calculated in that field.

### Landau free energy

↑ **Parent:** [Landau theory](#landau-theory)

A Landau free energy is a symmetry-constrained analytic expansion in an [order parameter](#order-parameter). Its minima determine the mean-field equilibrium phases.

#### Helical minimum of a complex Landau functional

↑ **Parent:** [Landau free energy](#landau-free-energy)

For $f=a|\phi|^2+|\phi|^4/2+c|\partial_x\phi|^2+|\partial_x^2\phi|^2$, a plane-wave [order parameter](#order-parameter) has quadratic coefficient $a+ck^2+k^4$. If $c<0$, this is minimized at $k^2=-c/2$, and a nonzero amplitude appears when $a<c^2/4$. If $c\ge0$, the minimizing wave number is zero and the ordered mean-field phase requires $a<0$. The arbitrary global phase is a degeneracy, not a missing minimization condition. These are functional-minimization results; finite-temperature fluctuations can invalidate long-range order in low dimensions.

#### Constrained order-parameter boundary stability

↑ **Parent:** [Landau free energy](#landau-free-energy)

A [stationary point](calculus-of-variations.md#stationary-point) on the domain $\phi\geq0$ must be tested using allowed one-sided variations. For $F=A\phi^2/2-B\phi^3+\lambda\phi^4/4$ with $B>0$, the boundary is a [local minimum](analysis.md#local-minimum) when $A>0$ and a [local maximum](analysis.md#local-maximum) when $A<0$. At $A=0$, the leading negative cubic term makes it a one-sided [local maximum](analysis.md#local-maximum) even though $F''(0)=0$; on an unrestricted real line it is instead a stationary inflection point.

#### Temperature-dependent cubic-quartic Landau free energy

↑ **Parent:** [Landau free energy](#landau-free-energy)

For $\phi\geq0$ and positive $c,B,\lambda,T_0$, define $\gamma=2B^2/(\lambda c)$. Completing the square gives

$$
F=\phi^2\left\{\frac\lambda4\left(\phi-\frac{2BT}{\lambda}\right)^2+\frac c2[(1-\gamma)T^2-T_0^2]\right\}.
$$

For $0<\gamma<1$, [phase coexistence](#phase-coexistence) occurs at $T^*=T_0/\sqrt{1-\gamma}$ with a discontinuous minimum at $\phi^*=2BT^*/\lambda$. For $\gamma\geq1$, a nonzero [global minimum](analysis.md#global-minimum) has lower [free energy](thermodynamic-potential.md#thermodynamic-free-energy) at every finite [temperature](temperature.md). Following the global equilibrium branch then does not force a restoration transition.

##### Thermal symmetry nonrestoration in a cubic-quartic model

↑ **Parent:** [Temperature-dependent cubic-quartic Landau free energy](#temperature-dependent-cubic-quartic-landau-free-energy)

When $\gamma\geq1$ in the stated model, the broken, nonzero minimum remains globally preferred at every finite [temperature](temperature.md). A metastable zero state can still exist for $T>T_0$, but its lifetime and a [nucleation](#nucleation) [temperature](temperature.md) are kinetic questions. Its disappearance at the [spinodal point](#spinodal-point) is not an equilibrium coexistence [temperature](temperature.md).

##### Latent heat of a temperature-dependent cubic-quartic Landau transition

↑ **Parent:** [Temperature-dependent cubic-quartic Landau free energy](#temperature-dependent-cubic-quartic-landau-free-energy)

At an equilibrium minimum, $dF_{\min}/dT=\partial_TF$ because $\partial_\phi F=0$. For $0<\gamma<1$, the [entropy](entropy.md) decrease at coexistence is $S_0-S_+=c(1-\gamma)T^*(\phi^*)^2$. Multiplying by $T^*$ gives the positive [latent heat](thermodynamic-potential.md#latent-heat) released on cooling. The units are total heat or heat density according to the normalization of $F$.

<h4 id="o-3-quartic-landau-minima">O(3) quartic Landau minima</h4>

↑ **Parent:** [Landau free energy](#landau-free-energy)

For $f=f_0+a(T-T_c)|\mathbf m|^2+b|\mathbf m|^4+c|\nabla\mathbf m|^2$ with positive coefficients and uniform free boundaries, the minimum is $\mathbf m=0$ at $T\ge T_c$. Below $T_c$ it is any constant vector with $|\mathbf m|^2=a(T_c-T)/(2b)$. A chosen direction leaves an $O(2)$ subgroup of $O(3)$ invariant; for proper rotations the pattern is $SO(3)\to SO(2)$. The mean-field transition is continuous, with square-root onset. Long-wavelength fluctuations can invalidate the ordered state in low dimensions.

#### Constrained order-parameter free energy

↑ **Parent:** [Landau free energy](#landau-free-energy)

Fix the spatial mean of a scalar [order parameter](#order-parameter) to $M$ and sum the [Boltzmann weights](canonical-ensemble.md#boltzmann-factor) of all configurations with that mean. The resulting constrained [partition function](canonical-ensemble.md#canonical-partition-function) $Z_M$ defines this [free-energy density](statistical-physics.md#free-energy-density), with an additive normalization fixed consistently. For an applied [conjugate field](#field-conjugate-to-an-order-parameter) $h$, $Z(h)=\int dM\,e^{-\beta_TV[F_c(M)-hM]}$, up to the chosen measure normalization. The [thermodynamic limit](statistical-physics.md#thermodynamic-limit) gives $f(h)=\inf_M[F_c(M)-hM]$. A homogeneous [Landau free energy](#landau-free-energy) is an approximation to this constrained potential; phase-separated configurations can convexify it in the full [thermodynamic limit](statistical-physics.md#thermodynamic-limit).

##### Zero-cutoff identification of constrained free energy

↑ **Parent:** [Constrained order-parameter free energy](#constrained-order-parameter-free-energy)

In a finite box, retain the constant mode $M$ while integrating all nonzero field modes using the [Wilsonian coarse-grained statistical Hamiltonian](#wilsonian-coarse-grained-statistical-hamiltonian). Below the smallest nonzero momentum, the remaining effective energy is $VU_\Lambda(M)$ and its [Boltzmann weight](canonical-ensemble.md#boltzmann-factor) is precisely the [constrained order-parameter free energy](#constrained-order-parameter-free-energy) weight. Thus the displayed equality holds with consistent field-independent normalization. It is not an identity between a bare [statistical Hamiltonian](statistical-physics.md#statistical-hamiltonian) and an unconstrained equilibrium [free energy](thermodynamic-potential.md#thermodynamic-free-energy). An analytic polynomial [Landau free energy](#landau-free-energy) further assumes a homogeneous branch and regular effective coefficients; long-distance fluctuations near and below an [upper critical dimension](#upper-critical-dimension) can invalidate that analytic approximation.

#### First-order transition in a cubic-quartic Landau potential

↑ **Parent:** [Landau free energy](#landau-free-energy)

For a real unrestricted scalar [order parameter](#order-parameter) and $A=A_2m^2/2+A_3m^3/3+A_4m^4/4$ with $A_3\ne0$ and $A_4>0$, the disordered [global minimum](analysis.md#global-minimum) is replaced discontinuously by a nonzero minimum at the displayed [phase coexistence](#phase-coexistence) condition. At coexistence $A=A_4m^2[m+2A_3/(3A_4)]^2/4$. Ordered [stationary points](calculus-of-variations.md#stationary-point) first appear at the [spinodal point](#spinodal-point) $A_2=A_3^2/(4A_4)$, while the disordered point loses local stability at $A_2=0$; neither local limit is the equilibrium transition condition.

##### Coexistence barrier of a cubic-quartic Landau transition

↑ **Parent:** [First-order transition in a cubic-quartic Landau potential](#first-order-transition-in-a-cubic-quartic-landau-potential)

At coexistence, the [landau free energy](#landau-free-energy) can factor as $F(\phi)=\lambda\phi^2(\phi-v)^2/4$. The minima at $0,v$ have equal [free energy](thermodynamic-potential.md#thermodynamic-free-energy). Differentiating shows the intermediate maximum at $v/2$, with barrier height $\lambda v^4/64$. The barrier is a local free-energy barrier; predicting spatial [nucleation](#nucleation) also requires interfacial or gradient information.

##### Bounded quartic nematic coexistence

↑ **Parent:** [First-order transition in a cubic-quartic Landau potential](#first-order-transition-in-a-cubic-quartic-landau-potential)

For $a,c>0$, $b\leq0$ and the molecular bound $Q\in[-1/2,1]$, coexistence with $Q=0$ occurs at $b_t=-\min_{0<Q\leq1}(a/Q+3cQ)$. Negative $Q$ has positive [free energy](thermodynamic-potential.md#thermodynamic-free-energy) and cannot be the stable phase in this coefficient range. Thus $a\leq3c$ gives $b_t=-\sqrt{12ac}$ and jump $0\to\sqrt{a/(3c)}$, whereas $a>3c$ gives $b_t=-(a+3c)$ and jump $0\to1$. The interior case is the usual small-order-parameter [Landau theory](#landau-theory) result. A formal unconstrained quartic minimization can violate the molecular bounds when extrapolated too far.

#### Critical endpoint of a quartic Landau free energy

↑ **Parent:** [Landau free energy](#landau-free-energy)

For the stable scalar [Landau free energy](#landau-free-energy) $f=b\lambda^4+c\lambda^3+a\lambda^2+d\lambda$, $b>0$, a stable zero-curvature equilibrium must have $f'=f''=f'''=0$. Solving these equations gives

$$
\lambda_c=-\frac c{4b},\qquad a_c=\frac{3c^2}{8b},\qquad d_c=\frac{c^3}{16b^2}.
$$

At this point $f=f(\lambda_c)+b(\lambda-\lambda_c)^4$. Varying two control parameters allows a line of [first-order phase transitions](thermodynamic-potential.md#first-order-phase-transition) to terminate here. A [spinodal point](#spinodal-point) satisfies zero curvature but need not satisfy the third-derivative condition or remain a local minimum.

#### Cubic-term removal in a conserved quartic Landau free energy

↑ **Parent:** [Landau free energy](#landau-free-energy)

For a scalar [Landau free energy](#landau-free-energy) $f=a\phi^2/2+b\phi^4/4+c\phi^3/3+d\phi$ with $b>0$, the shift $\phi=\psi-c/(3b)$ removes the cubic term. The quadratic coefficient becomes $a'=a-c^2/(3b)$ and the linear coefficient becomes $d'=d-ac/(3b)+2c^3/(27b^2)$. In a closed [binary fluid mixture](#binary-fluid-mixture), the linear term is constant at fixed total composition, leaving the symmetric quartic [phase coexistence](#phase-coexistence) construction in the shifted variable.

#### Multicritical even Landau potential

↑ **Parent:** [Landau free energy](#landau-free-energy)

For $n\geq2$ and $\lambda_n>0$, this [Landau free energy](#landau-free-energy) has [mean-field critical exponents](#mean-field-critical-exponent) $\beta=1/[2(n-1)]$ and $\alpha=(n-2)/(n-1)$ when $r$ crosses zero linearly with [temperature](temperature.md). For $n>2$, obtaining this behavior requires tuning the lower even interactions to zero.

#### Sextic even Landau potential

↑ **Parent:** [Landau free energy](#landau-free-energy)

For the [Landau free energy](#landau-free-energy) $G(\phi)=\phi^6/6+g\phi^4/4+\varepsilon\phi^2/2$, positive $g$ gives a [continuous phase transition](#continuous-phase-transition) at $\varepsilon=0$. For negative $g$, [phase coexistence](#phase-coexistence) between the disordered [global minimum](analysis.md#global-minimum) $\phi=0$ and the ordered [global minima](analysis.md#global-minimum) occurs on $\varepsilon=3g^2/16$, with $\phi^2=-3g/4$. Indeed, on that locus the [polynomial](polynomial.md) is $G(\phi)=\phi^2(\phi^2+3g/4)^2/6\geq0$, so these three zeros are [global minima](analysis.md#global-minimum). For $g<0$, the disordered and ordered [spinodal points](#spinodal-point) are respectively $\varepsilon=0$ and $\varepsilon=g^2/4$; equality of stationary [free energies](thermodynamic-potential.md#thermodynamic-free-energy) determines [phase coexistence](#phase-coexistence), while loss of a [local minimum](analysis.md#local-minimum) determines a [spinodal point](#spinodal-point).

#### Equilibrium magnetization

↑ **Parent:** [Landau free energy](#landau-free-energy)

The equilibrium magnetization is a value of the [magnetization](electromagnetism.md#magnetization) that minimizes the [Landau free energy](#landau-free-energy). A stable equilibrium has nonnegative second derivative with respect to the magnetization; degenerate nonzero minima describe symmetry-related magnetized phases.

#### Spinodal

↑ **Parent:** [Landau free energy](#landau-free-energy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spinodal)

The [spinodal](#spinodal) is the boundary where a metastable phase loses local stability. In a mean-field free-energy description the relevant curvature vanishes there, separating local minima from unstable configurations.

##### Spinodal decomposition

↑ **Parent:** [Spinodal](#spinodal)

[Spinodal decomposition](#spinodal-decomposition) is spontaneous growth of composition fluctuations in a homogeneous mixture whose local mixing [free energy](thermodynamic-potential.md#thermodynamic-free-energy) has negative composition curvature. For a mean $\phi$, equal regions at $\phi\pm\delta\phi$ change the mean free energy by $f''(\phi)(\delta\phi)^2/2+O((\delta\phi)^4)$, which is negative inside the [spinodal](#spinodal). Interfacial costs suppress sufficiently short wavelengths, while conservation of composition constrains the dynamics. Outside the spinodal but inside the [binodal](#binodal), the uniform state is instead [metastable](#metastability) and requires [nucleation](#nucleation) to begin separation.

##### Spinodal point

↑ **Parent:** [Spinodal](#spinodal)

A spinodal point is the limit of local metastability of a phase. At a mean-field spinodal, a local minimum merges with a neighboring maximum and the corresponding second derivative of the free energy vanishes.

###### Hysteresis spinodals of a scalar quartic potential

↑ **Parent:** [Spinodal point](#spinodal-point)

For the [Landau free energy](#landau-free-energy) $V(M)=rM^2/2+uM^4/4-hM$ with $r<0$ and $u>0$, stationary branches satisfy $h=rM+uM^3$. Their local stability requires $r+3uM^2>0$. At a [spinodal point](#spinodal-point), $M_{\rm sp}=\pm\sqrt{|r|/(3u)}$ and $h_{\rm sp}=(2r/3)M_{\rm sp}$, giving the displayed field magnitude. Following local minima without [nucleation](#nucleation) produces a [hysteresis](#hysteresis) loop switching at these limits. Equilibrium instead switches between the two global minima at $h=0$.

#### Metastability

↑ **Parent:** [Landau free energy](#landau-free-energy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Metastability)

A metastable phase is a local but nonglobal minimum of the thermodynamic potential. A finite nucleation barrier can delay conversion to the globally stable phase until fluctuations create a sufficiently large nucleus or the metastable minimum reaches a [spinodal point](#spinodal-point).

##### Supersaturated vapor

↑ **Parent:** [Metastability](#metastability)

A [vapor](thermodynamics.md#vapor) whose [partial pressure](ideal-gas.md#partial-pressure) exceeds its [vapor pressure](thermodynamic-potential.md#vapor-pressure) at the local [temperature](temperature.md); [nucleation](#nucleation) can permit [condensation](#condensation).

###### Atmospheric supersaturation

↑ **Parent:** [Supersaturated vapor](#supersaturated-vapor)

The fractional excess of water-vapor [pressure](pressure.md) above equilibrium saturation over a flat pure-water surface at the same [temperature](temperature.md): $s=p_v/p_{\rm sat}(T)-1$. Positive $s$ can drive droplet growth, but activation of a particular [aerosol](chemistry.md#aerosol) particle requires exceeding its [critical supersaturation](chemistry.md#critical-supersaturation). Cooling, condensation and mixing jointly determine parcel supersaturation.

##### Nucleation

↑ **Parent:** [Metastability](#metastability)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nucleation)

Nucleation forms a sufficiently large region of a new phase within an old [metastable](#metastability) phase. In [classical nucleation theory](thermodynamic-potential.md#classical-nucleation-theory), positive surface energy competes with bulk free-energy gain, producing a [critical nucleus](thermodynamic-potential.md#critical-nucleus) and a barrier to conversion. The [Arrhenius nucleation time](thermodynamic-potential.md#arrhenius-nucleation-time) depends exponentially on this barrier; boundaries and impurities can alter it. This explains how [metastability](#metastability) and [hysteresis](#hysteresis) can persist despite a different globally stable phase.

###### Burst nucleation

↑ **Parent:** [Nucleation](#nucleation)

Formation of most nuclei within an interval short compared with subsequent particle growth. A common birth period can help narrow a [particle size distribution](mixture.md#particle-size-distribution) if mixing and later growth are sufficiently uniform and secondary [nucleation](#nucleation) is suppressed.

###### La Mer diagram

↑ **Parent:** [Nucleation](#nucleation)

A schematic time history of growth-species [concentration](mathematical-physics.md#concentration) showing buildup, a short [nucleation](#nucleation) interval above an effective [nucleation](#nucleation) threshold, then growth above the equilibrium [solubility](ionic-bonding.md#solubility) but below substantial new [nucleation](#nucleation). The [concentration](mathematical-physics.md#concentration) history suggests how to separate particle birth from growth; it does not establish that every particle synthesis follows that mechanism.

###### Heterogeneous nucleation

↑ **Parent:** [Nucleation](#nucleation)

Formation of a critical nucleus at a pre-existing surface or interface. Favorable wetting can replace part of the cost of a free nucleus and lower its barrier; later deposition of a free particle on a support is a different process.

###### Deposition nucleation

↑ **Parent:** [Heterogeneous nucleation](#heterogeneous-nucleation)

Ice forms from ice-supersaturated vapour at a suitable foreign surface. The relevant temperature and surface properties differ from liquid-droplet immersion freezing.

###### Contact freezing

↑ **Parent:** [Heterogeneous nucleation](#heterogeneous-nucleation)

A suitable particle colliding with a supercooled droplet can trigger heterogeneous freezing. This is distinguished from nucleation around an inclusion already inside it.

###### Immersion freezing

↑ **Parent:** [Heterogeneous nucleation](#heterogeneous-nucleation)

Ice nucleates on an inclusion already immersed in supercooled water. The interfacial nucleation barrier, inclusion properties, droplet volume and observation time affect freezing probability.

###### Homogeneous nucleation

↑ **Parent:** [Nucleation](#nucleation)

Formation of a critical nucleus within the bulk parent phase without assistance from a pre-existing interface. Its interfacial cost competes with the bulk free-energy gain.

###### Homogeneous ice nucleation

↑ **Parent:** [Homogeneous nucleation](#homogeneous-nucleation)

Ice embryos form without a foreign nucleating surface once thermal fluctuations can overcome the free-energy barrier on the relevant timescale. An apparent freezing threshold depends on droplet volume and measurement duration.

##### Hysteresis

↑ **Parent:** [Metastability](#metastability)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hysteresis)

Dependence of a system's observed state on the path by which its control parameters were reached. In a [first-order phase transition](thermodynamic-potential.md#first-order-phase-transition), a [metastable](#metastability) local minimum may persist after another phase becomes globally stable, so increasing and decreasing the control parameter give different switching points. [Nucleation](#nucleation) and sweep rate determine actual switching; a mean-field [spinodal point](#spinodal-point) is a local-stability limit, not the equilibrium [phase coexistence](#phase-coexistence) condition.

###### Magnetic hysteresis

↑ **Parent:** [Hysteresis](#hysteresis)

[Magnetic hysteresis](#magnetic-hysteresis) means that a material's [magnetization](electromagnetism.md#magnetization) depends on its field history as well as the present applied field. A closed quasistatic magnetic cycle dissipates [energy](energy.md) per unit volume equal to its $H$–$B$ loop area. It is relevant to remanence in [permanent magnets](electromagnetism.md#permanent-magnet) and core losses in [electrical transformers](electrical-engineering.md#transformer-electrical-engineering).

###### Magnetic coercivity

↑ **Parent:** [Hysteresis](#hysteresis)

[Magnetic coercivity](#magnetic-coercivity) is the magnitude of a reverse applied [magnetic field intensity](electromagnetism.md#magnetic-field-intensity) required to bring a previously magnetized specimen's [magnetization](electromagnetism.md#magnetization) to zero on a specified [hysteresis](#hysteresis) branch. It depends on material, preparation and measurement history. It differs from [remanent magnetization](electromagnetism.md#remanent-magnetization), which is the remaining [magnetization](electromagnetism.md#magnetization) at zero applied field.

##### Superheating

↑ **Parent:** [Metastability](#metastability)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Superheating)

Superheating is the metastable persistence of a low-temperature phase above its equilibrium transition temperature.

###### Superheated liquid

↑ **Parent:** [Superheating](#superheating)

A [liquid](thermodynamics.md#liquid) maintained above its equilibrium [boiling](#boiling) [temperature](temperature.md) at the imposed [pressure](pressure.md). A barrier to [nucleation](#nucleation) can delay its conversion into [vapor](thermodynamics.md#vapor), making this a [metastable](#metastability) state.

###### Constitutional superheating

↑ **Parent:** [Superheating](#superheating)

A solid can locally exceed its [solidus](thermodynamic-potential.md#solidus) because a thin solute-diffusion layer changes composition faster than [thermal conduction](heat.md#thermal-conduction) changes [temperature](temperature.md). Near a melting [phase boundary](geophysics.md#phase-boundary), a depleted solid can join the equilibrium solidus at the interface while the adjacent, more concentrated solid remains above its own lower solidus. The assumed single sharp interface is then thermodynamically unstable to additional melting and may be replaced by a [mushy layer](geophysics.md#mushy-layer).

##### Supercooling

↑ **Parent:** [Metastability](#metastability)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Supercooling)

Supercooling is the metastable persistence of a high-temperature phase below its equilibrium transition temperature.

#### Common-tangent construction

↑ **Parent:** [Landau free energy](#landau-free-energy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Common-tangent_construction)

Two compositions coexist when one straight line is tangent to the free-energy density at both compositions. Equality of its slope gives equal chemical potentials, and equality of its intercept gives equal pressures.

##### Binodal

↑ **Parent:** [Common-tangent construction](#common-tangent-construction)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Binodal)

The binodal is the coexistence boundary: its two branches give the compositions of phases joined by the [common-tangent construction](#common-tangent-construction).

###### Saturation concentration

↑ **Parent:** [Binodal](#binodal)

For a dilute-to-dense liquid coexistence problem, the dilute-phase coexistence concentration at specified conditions. It is a branch of the coexistence boundary, not generally the concentration at the critical endpoint.

### Landau-Ginzburg theory

↑ **Parent:** [Landau theory](#landau-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Landau-Ginzburg_theory)

Landau-Ginzburg theory supplements the local Landau potential with gradient terms and treats the order parameter as a spatial field.

#### Square-gradient theory of a liquid interface

↑ **Parent:** [Landau-Ginzburg theory](#landau-ginzburg-theory)

A diffuse-interface [free energy](thermodynamic-potential.md#thermodynamic-free-energy) balances the bulk preference for coexisting compositions against a positive penalty for sharp composition gradients. For dimensionless composition $\phi$, $f_b$ is a bulk energy density and $K$ has units of energy per length. Subtract the bulk coexistence common tangent to define $\Delta\omega(\phi)$, with equal zero minima at the two compositions. A planar equilibrium profile obeys $K\phi''=\Delta\omega'(\phi)$ and $K(\phi')^2/2=\Delta\omega(\phi)$. Its [surface tension](surface-tension.md) is $\int K(\phi')^2dz$. As a [thermodynamic critical point](#thermodynamic-critical-point) is approached, the composition contrast and bulk curvature vanish, the [correlation length](#correlation-length) grows, and the intrinsic interface broadens. A [scalar quartic domain wall](#scalar-quartic-domain-wall) gives the mean-field hyperbolic-tangent profile. Thermally excited [capillary waves](surface-tension.md#capillary-wave) can broaden a measured profile further.

#### Scalar-field source Legendre transform

↑ **Parent:** [Landau-Ginzburg theory](#landau-ginzburg-theory)

For a real statistical source convention $Z[h]=\int\mathcal D\phi\,e^{-H_0[\phi]+\int h\phi}$, define $F=-\log Z$ and the displayed [Legendre transform](convex-optimization.md#convex-conjugate). On a differentiable stable branch, $\delta\Gamma/\delta m=h$. In the [Landau approximation](#landau-approximation), the branch expression is $\Gamma_{\rm L}[m]=H_0[m]$. The exact Legendre effective [free energy](thermodynamic-potential.md#thermodynamic-free-energy) is convex; a bare nonconvex [Landau free energy](#landau-free-energy) is a local approximation and requires branch or coexistence interpretation.

#### Landau approximation

↑ **Parent:** [Landau-Ginzburg theory](#landau-ginzburg-theory)

The Landau approximation evaluates a statistical field's [partition function](canonical-ensemble.md#canonical-partition-function) at a stable stationary configuration, omitting fluctuation-loop corrections to the [free energy](thermodynamic-potential.md#thermodynamic-free-energy). Functional differentiation of that stationary value still gives a connected linear response: the inverse of the saddle's quadratic fluctuation operator. Freezing fields before differentiating would lose this response. A [Gaussian field theory](#gaussian-field-theory), in contrast, permits exact integration of its quadratic fluctuations.

#### Two-component radial quartic Landau potential

↑ **Parent:** [Landau-Ginzburg theory](#landau-ginzburg-theory)

With positive $g$, the quadratic coefficients select the component with the smaller negative coefficient. Equal negative coefficients give a circle of minima in the [mean-field approximation](#mean-field-approximation); the negative diagonal is a [spin-flop transition](thermodynamic-potential.md#spin-flop-transition), ending at a [bicritical point](thermodynamic-potential.md#bicritical-point) at the origin.

#### Local derivative expansion

↑ **Parent:** [Landau-Ginzburg theory](#landau-ginzburg-theory)

A [Landau free energy](#landau-free-energy) can be expanded in local powers of the [order parameter](#order-parameter) and its spatial derivatives. Internal and spatial [symmetries](physics.md#symmetry-physics) constrain the allowed terms; truncation assumes slowly varying fields.

##### Canonical normalization of a scalar gradient term

↑ **Parent:** [Local derivative expansion](#local-derivative-expansion)

For a statistical scalar theory with gradient coefficient $K/2>0$, this rescaling gives a canonical $(\nabla\psi)^2/2$ term. A mass coefficient $r$ becomes $r/K$, a quartic coefficient $g$ becomes $g/K^2$, and a source $h$ becomes $h/\sqrt K$. Thus the simple propagator denominator $p^2+R$ and loop-coupling formulas assume these normalized coefficients. The associated measure Jacobian is field independent and belongs to the free-energy normalization.

#### Gradient energy

↑ **Parent:** [Landau-Ginzburg theory](#landau-ginzburg-theory)

A gradient energy penalizes spatial variation of an [order parameter](#order-parameter). Its leading isotropic form is usually proportional to the squared spatial gradient.

#### Gradient expansion

↑ **Parent:** [Landau-Ginzburg theory](#landau-ginzburg-theory)

A gradient expansion orders a local effective free energy by the number of spatial derivatives of slowly varying fields. Symmetry determines the allowed derivative contractions.

#### Interfacial tension

↑ **Parent:** [Landau-Ginzburg theory](#landau-ginzburg-theory)

Interfacial tension is the excess free energy per unit area of an equilibrium interface relative to its coexisting bulk phases.

#### Phi-four diffuse interface

↑ **Parent:** [Landau-Ginzburg theory](#landau-ginzburg-theory)

For $F=\int[a\phi^2/2+b\phi^4/4+\kappa|\nabla\phi|^2/2]$ with $a<0<b,\kappa$, the planar coexistence interface is

$$
\phi(x)=\phi_B\tanh\frac{x-x_0}{\xi_0},
\qquad
\phi_B=\sqrt{-a/b},
\qquad
\xi_0=\sqrt{-2\kappa/a}.
$$

##### Interfacial tension of a phi-four diffuse interface

↑ **Parent:** [Phi-four diffuse interface](#phi-four-diffuse-interface)

The excess free energy per area of the phi-four diffuse interface is

$$
\sigma=\int_{-\infty}^{\infty}\kappa(\phi')^2dx
=\sqrt{\frac{-8a^3\kappa}{9b^2}}.
$$

#### Gaussian field theory

↑ **Parent:** [Landau-Ginzburg theory](#landau-ginzburg-theory)

A Gaussian field theory has a free energy quadratic in its field modes. If $H_0=\sum_{\mathbf q}^{+}J(q)|\phi_{\mathbf q}|^2$ for a real field, then $\langle|\phi_{\mathbf q}|^2\rangle=J(q)^{-1}$ and its partition function is a product of elementary Gaussian integrals.

##### Ordered-phase obstruction in a Gaussian scalar model

↑ **Parent:** [Gaussian field theory](#gaussian-field-theory)

The uniform mode of a pure [Gaussian field theory](#gaussian-field-theory) with negative squared mass has an unbounded quadratic energy. Its [partition function](canonical-ensemble.md#canonical-partition-function) diverges even with a finite-volume ultraviolet regulator, so it supplies no stable ordered branch. At positive squared mass the zero-source average is zero. Thus the scaling dimension of the field can yield a formal [order-parameter critical exponent](#order-parameter-critical-exponent) without establishing a negative-reduced-temperature [magnetization](electromagnetism.md#magnetization) law. A stabilizing quartic interaction is relevant below four dimensions and ordinarily changes the critical theory to the [Wilson-Fisher fixed point](#wilson-fisher-fixed-point); above four its coefficient is a [dangerously irrelevant coupling](#dangerously-irrelevant-coupling) for the ordered phase.

##### Massive Gaussian field correlation tail

↑ **Parent:** [Gaussian field theory](#gaussian-field-theory)

For the positive quadratic kernel $\widetilde\Delta(p)=\kappa^{-1}p^2+m^2$, $\kappa,m>0$, the [connected correlation function](#connected-correlation-function) is its inverse. Fourier inversion gives $G(r)=\kappa(\sqrt\kappa m/r)^{D/2-1}K_{D/2-1}(\sqrt\kappa mr)/(2\pi)^{D/2}$. The [Modified Bessel function of the second kind](bessel-function.md#modified-bessel-function-of-the-second-kind) has an exponentially decaying large-argument tail, so the [correlation length](#correlation-length) is $1/(\sqrt\kappa m)$ at fixed positive [gradient](multivariable-calculus.md#gradient) coefficient. In three dimensions this becomes $\kappa e^{-\sqrt\kappa mr}/(4\pi r)$. The statement concerns the continuum long-distance theory; regulator-dependent contact terms do not define the physical [correlation length](#correlation-length).

##### Positive-wavevector sum for a real field

↑ **Parent:** [Gaussian field theory](#gaussian-field-theory)

For a real field, $\phi_{-\mathbf q}=\phi_{\mathbf q}^*$. A sum $\sum_{\mathbf q}^{+}$ takes one representative from each nonzero pair $\{\mathbf q,-\mathbf q\}$ so that every independent complex Fourier amplitude is counted once.

##### Gaussian variational approximation

↑ **Parent:** [Gaussian field theory](#gaussian-field-theory)

A Gaussian variational approximation chooses a quadratic trial kernel and minimizes a variational upper bound on the interacting free energy. The optimized kernel often equals the bare kernel plus a self-consistent, wavevector-independent mass shift.

###### Gaussian variational kernel for a gradient quartic interaction

↑ **Parent:** [Gaussian variational approximation](#gaussian-variational-approximation)

For $H=\int[a\phi^2/2+\kappa|\nabla\phi|^2/2+\gamma(\nabla^2\phi)^2/2+B\phi^2|\nabla\phi|^2]$ and an even positive trial kernel $J(q)$, define $S_0=\sum_q^+1/J(q)$ and $S_2=\sum_q^+q^2/J(q)$ using a [positive-wavevector sum for a real field](#positive-wavevector-sum-for-a-real-field). [Isserlis theorem](probability-distribution.md#isserlis-s-theorem) gives $\langle H_4\rangle_0=4BS_0S_2/V$. The [Feynman-Bogoliubov inequality](#gibbs-bogoliubov-feynman-inequality) therefore has stationary kernels

$$
J(q)=a+\kappa q^2+\gamma q^4+\frac{4B}{V}(S_2+q^2S_0).
$$

Thus both the mass and gradient coefficient shift. In the [thermodynamic limit](statistical-physics.md#thermodynamic-limit), their [self-consistency equations](#self-consistency-equation) are

$$
\bar a=a+2B\int_{|k|<\Lambda}\frac{k^2}{\bar a+\bar\kappa k^2+\gamma k^4}\frac{d^dk}{(2\pi)^d},
\quad
\bar\kappa=\kappa+2B\int_{|k|<\Lambda}\frac1{\bar a+\bar\kappa k^2+\gamma k^4}\frac{d^dk}{(2\pi)^d}.
$$

A coarse-graining [ultraviolet cutoff](quantum-field-theory.md#ultraviolet-cutoff) $\Lambda$ is necessary for the first integral in three dimensions: its large-$k$ radial integrand tends to a constant. Physical solutions require $J(q)>0$.

<h6 id="gibbs-bogoliubov-feynman-inequality">Gibbs--Bogoliubov--Feynman inequality</h6>

↑ **Parent:** [Gaussian variational approximation](#gaussian-variational-approximation)

For an exact dimensionless Hamiltonian $H$ and trial Hamiltonian $H_0$, the free energies obey

$$
F\leq F_0+\langle H-H_0\rangle_0,
$$

where $F_0=-\log Z_0$ and the expectation uses the trial Gibbs distribution $Z_0^{-1}e^{-H_0}$.

The identity $e^{-F}=e^{-F_0}\langle e^{-(H-H_0)}\rangle_0$ and the [Jensen inequality](real-analysis.md#jensen-s-inequality) for the convex [exponential function](calculus.md#exponential-function) give $\log\langle e^{-(H-H_0)}\rangle_0\geq-\langle H-H_0\rangle_0$. Taking minus the logarithm proves the bound.

#### Brazovskii model

↑ **Parent:** [Landau-Ginzburg theory](#landau-ginzburg-theory)

A Brazovskii model has a quadratic Fourier kernel minimized on a sphere of nonzero wavevector magnitude. The large phase space of soft modes can prevent the Gaussian mass from vanishing and turn a mean-field continuous transition into a fluctuation-induced first-order transition.

##### Gradient-quartic Brazovskii model

↑ **Parent:** [Brazovskii model](#brazovskii-model)

A gradient-quartic Brazovskii model stabilizes a negative quadratic gradient coefficient with $\gamma(\nabla^2\phi)^2/2$ and uses the quartic interaction $B\phi^2|\nabla\phi|^2$. For $\gamma,B>0$ and a zero-average [compositional order parameter](#compositional-order-parameter), its nonzero-wavevector instability is a candidate for [smectic phase](#smectic-phase) ordering. The [Gaussian variational kernel for a gradient quartic interaction](#gaussian-variational-kernel-for-a-gradient-quartic-interaction) shifts both the quadratic coefficients.

###### Single-mode smectic mean-field free energy

↑ **Parent:** [Gradient-quartic Brazovskii model](#gradient-quartic-brazovskii-model)

For $\phi=A\cos(q_0z)$, the [gradient-quartic Brazovskii model](#gradient-quartic-brazovskii-model) has volume-averaged [free-energy density](statistical-physics.md#free-energy-density)

$$
f(A)=\frac{a-a_c}{4}A^2+\frac{Bq_0^2}{8}A^4,
\quad q_0^2=-\frac\kappa{2\gamma},
\quad a_c=\frac{\kappa^2}{4\gamma}.
$$

The averages are $\langle\cos^2\rangle=\langle\sin^2\rangle=1/2$ and $\langle\cos^2\sin^2\rangle=1/8$. For $B>0$, the stable amplitude is zero for $a\geq a_c$ and satisfies $A^2=(a_c-a)/(Bq_0^2)$ below it. The [mean-field approximation](#mean-field-approximation) therefore predicts a [continuous phase transition](#continuous-phase-transition).

##### Nonzero-wavevector soft-mode sphere

↑ **Parent:** [Brazovskii model](#brazovskii-model)

For $G(q)=a+\kappa q^2+\gamma q^4$ with $\kappa<0<\gamma$, the minimum occurs on the sphere $q=q_0=\sqrt{-\kappa/(2\gamma)}$. The minimum value is $a-\kappa^2/(4\gamma)$.

###### Soft-mode shell integral

↑ **Parent:** [Nonzero-wavevector soft-mode sphere](#nonzero-wavevector-soft-mode-sphere)

In three dimensions, let $J(q)=r+\gamma(q^2-q_*^2)^2$, with $q_*>0$ and small $r>0$. Near the soft shell, $J(q)\simeq r+4\gamma q_*^2(q-q_*)^2$, so

$$
\int\frac{d^3q}{(2\pi)^3J(q)}
\sim\frac{q_*}{4\pi\sqrt{\gamma r}},
\qquad
\int\frac{q^2\,d^3q}{(2\pi)^3J(q)}
\sim\frac{q_*^3}{4\pi\sqrt{\gamma r}}.
$$

The radial integral uses $\int_{-\infty}^{\infty}ds/(r+As^2)=\pi/\sqrt{Ar}$. The $r^{-1/2}$ divergence obstructs the zero-mass limit of a self-consistent [Gaussian variational approximation](#gaussian-variational-approximation) at a fixed nonzero ordering wavevector. This is the mechanism behind the [Brazovskii fluctuation-induced first-order transition](#brazovskii-fluctuation-induced-first-order-transition); [Gross, Ignatiev and Chakraborty's study of fluctuation-driven ordering](https://arxiv.org/abs/cond-mat/0003026) analyzes the corresponding standard Brazovskii model.

##### Brazovskii fluctuation-induced first-order transition

↑ **Parent:** [Brazovskii model](#brazovskii-model)

In a self-consistent Gaussian treatment, fluctuations near the soft-mode sphere generate a positive mass shift that diverges as the renormalized mass approaches zero. The disordered phase therefore remains locally stable until its free energy crosses that of a finite-amplitude modulated phase, producing a first-order transition.

#### Smectic phase

↑ **Parent:** [Landau-Ginzburg theory](#landau-ginzburg-theory)

A smectic phase has one-dimensional translational order, represented at the simplest level by a periodically modulated field $\phi(\mathbf r)=A\cos(\mathbf q_0\mathbin\cdot\mathbf r)$.

##### Smectic C phase

↑ **Parent:** [Smectic phase](#smectic-phase)

A smectic C phase has layered positional order with the [nematic director](#nematic-director) tilted away from the layer normal. The tilt supplies additional orientational information beyond the density modulation of a [smectic phase](#smectic-phase).

##### Smectic A phase

↑ **Parent:** [Smectic phase](#smectic-phase)

A smectic A phase has layered positional order with the average molecular orientation along the layer normal. Molecular positions within each layer remain liquid-like. Its orientational axis is described by a [nematic director](#nematic-director).

##### Polar helical smectic

↑ **Parent:** [Smectic phase](#smectic-phase)

A polar helical smectic has a vector order parameter of constant magnitude whose direction rotates at a nonzero wavevector. For an isotropic Brazovskii free energy, all constant rotations of the helical plane are degenerate until a longitudinal-gradient term such as $|\nabla\mathbin\cdot\mathbf p|^2$ selects its orientation.

#### Ginzburg criterion

↑ **Parent:** [Landau-Ginzburg theory](#landau-ginzburg-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ginzburg_criterion)

The Ginzburg criterion requires order-parameter fluctuations inside a correlation volume to be small compared with the squared mean-field order parameter. Its failure marks the fluctuation-dominated critical region.

##### Ginzburg reduced-temperature window

↑ **Parent:** [Ginzburg criterion](#ginzburg-criterion)

For dimensionless scalar [Landau-Ginzburg theory](#landau-ginzburg-theory) with quadratic coefficient $r=a_t t$, [gradient](multivariable-calculus.md#gradient) coefficient $c>0$ and quartic term $u\phi^4/4$, the [correlation-volume derivation of the scalar Ginzburg ratio](#correlation-volume-derivation-of-the-scalar-ginzburg-ratio) gives $\mathcal G\sim u c^{-d/2}a_t^{(d-4)/2}|t|^{-(4-d)/2}$. For $d<4$, solving $\mathcal G\sim1$ gives the displayed nonuniversal window. Mean-field self-consistency requires $|t|\gg\mathrm{Gi}$ while still staying in the domain of the local expansion. In three dimensions $\mathrm{Gi}\sim u^2/(c^3a_t)$. Numerical prefactors depend on the averaging convention and microscopic normalization; no universal material value follows from dimensional power counting. At four dimensions use the [marginal Ginzburg criterion](#marginal-ginzburg-criterion) instead of this singular exponent formula.

##### Correlation-volume derivation of the scalar Ginzburg ratio

↑ **Parent:** [Ginzburg criterion](#ginzburg-criterion)

For the dimensionless scalar [Landau-Ginzburg theory](#landau-ginzburg-theory) with stiffness $c$, quadratic coefficient $r<0$ and quartic term $u\phi^4/4$, the [mean-field approximation](#mean-field-approximation) gives $\phi_0^2=|r|/u$ and [correlation length](#correlation-length) $\xi\asymp(c/|r|)^{1/2}$. Restricting the Gaussian [Fourier transform](fourier-transform.md) covariance $(cq^2+2|r|)^{-1}$ to $|q|\lesssim\xi^{-1}$ estimates the variance of the field averaged over a [correlation volume](#correlation-volume) as $c^{-d/2}|r|^{(d-2)/2}$, up to a dimension-dependent constant. Dividing by $\phi_0^2$ proves the displayed [Ginzburg criterion](#ginzburg-criterion) ratio. It diverges below four dimensions, vanishes above four and is marginal at four. Short-distance fluctuations renormalize microscopic coefficients and should not be confused with this long-distance critical test.

##### Critical region of a phase transition

↑ **Parent:** [Ginzburg criterion](#ginzburg-criterion)

The critical region is the range of control parameters near a [thermodynamic critical point](#thermodynamic-critical-point) where correlated [order parameter](#order-parameter) fluctuations invalidate a simple [mean-field approximation](#mean-field-approximation). For short-range scalar quartic theory below four dimensions, the dimensionless [Ginzburg criterion](#ginzburg-criterion) ratio grows as $g\xi^{4-D}$ in fixed microscopic units. The range where this ratio is of order one or larger is fluctuation dominated. Its width depends on nonuniversal microscopic coefficients even though the limiting [critical exponents](#critical-exponent) can be universal.

##### One-loop critical-mass subtraction

↑ **Parent:** [Ginzburg criterion](#ginzburg-criterion)

For a scalar quartic interaction $g\phi^4/4!$, the tadpole relation $R=r_\Lambda+(g/2)I_D(R)$ can be subtracted at the critical point. When $I_D(0)$ exists, $A(T-T_C)=R[1+(g/2)J_D(R)]$, with $J_D(R)=\int d^Dp\,(2\pi)^{-D}/[p^2(p^2+R)]$. This integral is finite as $R\to0$ only above four dimensions and is logarithmic at four. A self-consistent one-loop relation is not an exact interacting critical-exponent formula.

###### Infrared asymptotics of the critical-mass subtraction

↑ **Parent:** [One-loop critical-mass subtraction](#one-loop-critical-mass-subtraction)

For the scalar quartic [one-loop critical-mass subtraction](#one-loop-critical-mass-subtraction), the subtracted tadpole is $I_D(0)-I_D(R)=RJ_D(R)$. Above four dimensions $J_D(0)=K_D\Lambda^{D-4}/(D-4)$ is finite. At four dimensions $J_4=(K_4/2)\log[(\Lambda^2+R)/R]$. For $2<D<4$, $J_D\sim K_DR^{(D-4)/2}\int_0^\infty q^{D-3}(1+q^2)^{-1}dq$, which diverges as $R\to0$. Hence a smooth linear thermal mass survives this test only above the ordinary [upper critical dimension](#upper-critical-dimension) four. The massless subtraction is infrared divergent for $D\leq2$ and cannot prove absence of an interacting transition there.

###### Radial critical-mass subtraction in dimensions three to five

↑ **Parent:** [Infrared asymptotics of the critical-mass subtraction](#infrared-asymptotics-of-the-critical-mass-subtraction)

For $R>0$, a spherical [ultraviolet cutoff](quantum-field-theory.md#ultraviolet-cutoff) gives the following exact examples of the [one-loop critical-mass subtraction](#one-loop-critical-mass-subtraction) integral:

$$
J_3(R)=\frac{1}{2\pi^2\sqrt R}\arctan\frac\Lambda{\sqrt R},\qquad
J_4(R)=\frac{1}{16\pi^2}\log\frac{\Lambda^2+R}{R},\qquad
J_5(R)=\frac{1}{12\pi^3}\left(\Lambda-\sqrt R\arctan\frac\Lambda{\sqrt R}\right).
$$

The areas of the unit spheres in dimensions three, four and five are $4\pi$, $2\pi^2$ and $8\pi^2/3$. Dividing by $(2\pi)^D$ reduces the integrals to constants times $\int_0^\Lambda dp/(p^2+R)$, $\int_0^\Lambda p\,dp/(p^2+R)$ and $\int_0^\Lambda p^2dp/(p^2+R)$ respectively. Elementary integration proves the formulas. As $R\to0$, the first has a power divergence, the second a logarithmic divergence, and the third a finite limit. These examples make the ordinary [upper critical dimension](#upper-critical-dimension) four visible without treating a self-consistent one-loop equation as an exact interacting [critical exponent](#critical-exponent) prediction.

##### Marginal Ginzburg criterion

↑ **Parent:** [Ginzburg criterion](#ginzburg-criterion)

At an [upper critical dimension](#upper-critical-dimension), the leading [Ginzburg criterion](#ginzburg-criterion) ratio has zero thermal power rather than a negative one. It does not vanish asymptotically, but its magnitude can depend on the coupling. The criterion alone does not establish a power-law divergence or new critical power exponents. Running marginal interactions generally produce logarithmic corrections; the ordinary quartic and tricritical sextic scalar theories are examples.

##### Multicritical Ginzburg ratio

↑ **Parent:** [Ginzburg criterion](#ginzburg-criterion)

For a tuned [multicritical even Landau potential](#multicritical-even-landau-potential) with leading positive $M^{2n}$ term, $M^2\sim|t|^{1/(n-1)}$ and $\xi\sim|t|^{-1/2}$. Long-wavelength Gaussian fluctuations in a [correlation volume](#correlation-volume) have variance proportional to $\xi^{2-D}$. Their ratio to $M^2$ therefore scales as $|t|^{(D-2)/2-1/(n-1)}$, vanishing only for $D>2n/(n-1)$. At equality the criterion is marginal, requiring further fluctuation analysis.

#### Gaussian fluctuation correction near a critical point

↑ **Parent:** [Landau-Ginzburg theory](#landau-ginzburg-theory)

For a quadratic kernel $K(t,k)\sim t+k^2$, the singular heat-capacity correction is proportional to

$$
\int\frac{d^dk}{(t+k^2)^2}\asymp t^{d/2-2}.
$$

<h5 id="ornstein-zernike-correlation-function">Ornstein--Zernike correlation function</h5>

↑ **Parent:** [Gaussian fluctuation correction near a critical point](#gaussian-fluctuation-correction-near-a-critical-point)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ornstein--Zernike_correlation_function)

A Gaussian field with free-energy kernel $A+\kappa q^2$ has structure factor proportional to $(A+\kappa q^2)^{-1}$ and correlation length $\sqrt{\kappa/A}$.

### Mean-field critical exponent

↑ **Parent:** [Landau theory](#landau-theory)

For an ordinary quartic Landau transition, the heat-capacity and order-parameter exponents are $\alpha=0$ and $\beta=1/2$. At a tricritical sextic point they are $\alpha=1/2$ and $\beta=1/4$.

### Tricritical point

↑ **Parent:** [Landau theory](#landau-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tricritical_point)

A tricritical point is where a line of continuous transitions meets a line of first-order transitions; in a $\mathbb Z_2$ Landau expansion both quadratic and quartic coefficients vanish and a positive sextic term stabilizes the free energy.

#### Mean-field tricritical exponent calculation

↑ **Parent:** [Tricritical point](#tricritical-point)

For the sextic [Landau free energy](#landau-free-energy) $V=rM^2/2+vM^6/6-hM$, $v>0$, with $r$ linear in reduced temperature, the equation of state is $h=rM+vM^5$. Its ordered zero-field minimum satisfies $M^4=-r/v$, the inverse [magnetic susceptibility](statistical-physics.md#magnetic-susceptibility) is $4|r|$ below the transition and $r$ above, and the critical isotherm satisfies $h=vM^5$. The minimized singular [free-energy density](statistical-physics.md#free-energy-density) is $-|r|^{3/2}/(3\sqrt v)$ below and zero above. These facts give the displayed [mean-field critical exponents](#mean-field-critical-exponent), obeying both the [Rushbrooke scaling relation](#rushbrooke-scaling-relation) and [Widom scaling relation](#widom-scaling-relation). Both the quadratic and quartic coefficients must be tuned; a generic path with a positive quartic coefficient instead has ordinary critical behavior. Fluctuations change the result below the tricritical [upper critical dimension](#upper-critical-dimension) three, and marginal corrections can add logarithms at three.

##### Tricritical heat-capacity amplitude in a sextic Landau expansion

↑ **Parent:** [Mean-field tricritical exponent calculation](#mean-field-tricritical-exponent-calculation)

For $F=F_0+b(T-T_c)M^2+d'M^6$ with $b,d'>0$, the ordered minimum has $M^4=b(T_c-T)/(3d')$. Its singular [free energy](thermodynamic-potential.md#thermodynamic-free-energy) is $-2b^{3/2}(T_c-T)^{3/2}/\sqrt{27d'}$. Twice differentiating in [temperature](temperature.md) gives the displayed ordered-side [heat capacity](heat.md#heat-capacity) singularity, with mean-field [critical exponent](#critical-exponent) $\alpha=1/2$. This path keeps the quartic coefficient tuned to zero; a generic path with a positive quartic term instead crosses over to the ordinary quartic result.

#### Tricritical wing

↑ **Parent:** [Tricritical point](#tricritical-point)

For an even sextic [Landau free energy](#landau-free-energy) perturbed by a conjugate field, a tricritical wing is a [phase coexistence](#phase-coexistence) surface at nonzero field between ordered minima of different magnitudes. Two symmetry-related wings emerge from the three-phase line at zero field and terminate at ordinary critical edges. They meet the zero-field ordered coexistence sheet at the [tricritical point](#tricritical-point).

##### Tricritical three-phase line

↑ **Parent:** [Tricritical wing](#tricritical-wing)

For $V=rm^2/2+um^4/4+vm^6/6-hm$ with $v>0$, the displayed line has three [global minima](analysis.md#global-minimum), $m=0$ and $m=\pm\sqrt{-3u/(4v)}$. The factorization $V=(v/6)m^2(m^2+3u/(4v))^2$ proves their coexistence. Two nonzero-field [tricritical wings](#tricritical-wing) and the zero-field ordered coexistence sheet meet along this line. Its order-parameter discontinuity tends to zero as it terminates at the [tricritical point](#tricritical-point).

##### Tricritical wing coexistence factorization

↑ **Parent:** [Tricritical wing](#tricritical-wing)

Take two nonnegative coexisting minima $a\leq b$, put $s=a+b$ and $p=ab$, and fix $v>0$. For the sextic [Landau free energy](#landau-free-energy) with quadratic, quartic, sextic and linear terms, equal stationary minimum values occur at

$$
u=\frac{2v}{3}(-2s^2+3p),\qquad
r=\frac v3(s^4-s^2p+3p^2),\qquad h=\frac v3s^3p.
$$

At these coefficients,

$$
f(M)-f(a)=\frac v6(M-a)^2(M-b)^2[(M+s)^2+p]\geq0.
$$

Thus both are [global minima](analysis.md#global-minimum). The case $a=0$ gives the zero-field three-phase line, including the negative minimum; the limit $a=b$ gives the [tricritical wing critical edge](#tricritical-wing-critical-edge). Reflecting $M,h$ gives the negative-field wing.

##### Tricritical wing critical edge

↑ **Parent:** [Tricritical wing](#tricritical-wing)

For $f=rM^2/2+uM^4/4+vM^6/6-hM$ with $v>0$, the ordinary critical edge of a [tricritical wing](#tricritical-wing) satisfies $f^{(1)}=f^{(2)}=f^{(3)}=0$. For $u<0$, $M_c^2=-3u/(10v)$, $r_c=9u^2/(20v)$ and $h_c=6u^2M_c/(25v)$. Its fourth derivative is $-12u>0$. The two signs of $M_c$ give the two wings.

#### Tricritical crossover scaling

↑ **Parent:** [Tricritical point](#tricritical-point)

For the stable sextic [Landau free energy](#landau-free-energy) $f=rm^2/2+qm^4/4+sm^6/6-hm$, $s>0$, rescaling $m=(|r|/s)^{1/4}\psi$ gives the minimized order-parameter contribution $f_{\rm eq}=|r|^{3/2}s^{-1/2}\Phi_\sigma(X,Y)$, where $\sigma=\operatorname{sgn}r$, $X=q/(|r|s)^{1/2}$ and $Y=hs^{1/4}/|r|^{5/4}$. The two functions are $\Phi_\sigma=\min_\psi(\sigma\psi^2/2+X\psi^4/4+\psi^6/6-Y\psi)$. In particular $\Phi_-(0,0)=-1/3$, but $\Phi_+(0,0)=0$. These separate branches and removal of smooth background terms are necessary when using the homogeneous form to infer [mean-field critical exponents](#mean-field-critical-exponent).

##### Large-quartic asymptotic of tricritical scaling

↑ **Parent:** [Tricritical crossover scaling](#tricritical-crossover-scaling)

On the ordered branch of [tricritical crossover scaling](#tricritical-crossover-scaling), at zero field and $X\to+\infty$, the minimizing square is $a=\psi^2=(\sqrt{X^2+4}-X)/2\sim1/X$. Its stationarity relation $Xa+a^2=1$ gives $\Phi_-(X,0)=-a/4-a^3/12\sim-1/(4X)$. Thus the minimized [free-energy density](statistical-physics.md#free-energy-density) becomes $-r^2/(4q)$ for fixed $q>0$ as $r\uparrow0$, recovering the ordinary quartic [continuous phase transition](#continuous-phase-transition) and its [heat-capacity critical exponent](#heat-capacity-critical-exponent) $\alpha=0$. Replacing the scaling function by a nonzero constant in this limit would give an incorrect exponent.

#### Tricritical sextic beta function

↑ **Parent:** [Tricritical point](#tricritical-point)

In three dimensions, after tuning the quadratic and quartic [relevant operators](#relevant-operator), the positive sextic coupling has a [renormalization-group beta function](perturbative-quantum-field-theory.md#beta-function-physics) $d\lambda/ds=-C\lambda^2+\cdots$ with $C>0$ for increasing length scale $s$. The [Wick contractions](perturbative-quantum-field-theory.md#wick-contraction) connecting two sextic vertices with three propagators give the primitive logarithmic correction. The interaction is [marginally irrelevant](#marginally-irrelevant-operator).

## Upper critical dimension

↑ **Parent:** [Critical phenomenon](critical-phenomenon.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Upper_critical_dimension)

The upper critical dimension is the dimension above which the Gaussian or mean-field fixed point controls critical exponents. It is four for the ordinary Ising critical point and three for its tricritical point.

### Upper critical dimension of percolation

↑ **Parent:** [Upper critical dimension](#upper-critical-dimension)

Six is the predicted boundary for ordinary short-range [percolation](percolation-theory.md) to have [mean-field percolation exponents](#mean-field-percolation-exponents), with logarithmic corrections expected at the boundary. If the Fourier connectivity has leading small-momentum behavior $|k|^{-2}$, the triangle integral scales as $\int_0^\varepsilon r^{d-7}\,dr$, finite exactly for $d>6$. This is a scaling argument; rigorous nearest-neighbor results require their own dimensional hypotheses.

### Upper critical dimension of an even scalar interaction

↑ **Parent:** [Upper critical dimension](#upper-critical-dimension)

At the [Gaussian fixed point](#gaussian-fixed-point), the [engineering dimension](#engineering-dimension) of the coupling of $\phi^{2n}$ is $2n-(n-1)d$. It vanishes at the [upper critical dimension](#upper-critical-dimension) $d_c=2n/(n-1)$.

## Renormalization group

↑ **Parent:** [Critical phenomenon](critical-phenomenon.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Renormalization_group)

A [renormalization group](#renormalization-group) compares models at different observation lengths. A [Wilsonian coarse-grained statistical Hamiltonian](#wilsonian-coarse-grained-statistical-hamiltonian) sums over short-distance fluctuations; a [renormalization-group transformation](#renormalization-group-transformation) rescales coordinates and fields for comparison. [Kenneth Geddes Wilson](physicist.md#kenneth-geddes-wilson)'s 1982 lecture treats fluctuations across successive length scales to explain [critical phenomena](critical-phenomenon.md).[Section II, pp. 103–104: successive scale integration; inspected in an AGH-hosted reproduction](physics-bibliography.md#the-renormalization-group-and-critical-phenomena-by-kenneth-geddes-wilson)

The experimental motivation is [Andrews's carbon dioxide experiment](pressure.md#andrews-s-carbon-dioxide-experiment). Dried [carbon dioxide](chemical-substance.md#carbon-dioxide) occupied a [capillary tube](physics.md#capillary-tube) above [mercury](chemical-substance.md#mercury-element); a screw compressed the transmitting [water](chemical-substance.md#water). A second air-filled tube gauged [pressure](pressure.md). Flowing [water](chemical-substance.md#water) controlled [temperature](temperature.md), and a [cathetometer](physics.md#cathetometer) read column positions for [volume](thermodynamics.md#volume-thermodynamics). The [liquid meniscus](mixture.md#meniscus-liquid-surface) vanished near the [liquid-gas critical point](#liquid-gas-critical-point). Residual air and imperfect air-gauge corrections limited accuracy.[pp. 576–578: preparation, apparatus, calibration and pressure caveats; pp. 583–584: critical-temperature observations](physics-bibliography.md#the-bakerian-lecture-on-the-continuity-of-the-gaseous-and-liquid-states-of-matter-by-thomas-andrews) These observations motivate critical-point theory without determining a [correlation-length critical exponent](#correlation-length-critical-exponent). The [renormalization group](#renormalization-group) explains how critical measurements can become insensitive to many molecular details.

In 1972, [Kenneth Geddes Wilson](physicist.md#kenneth-geddes-wilson) and [Michael Ellis Fisher](physicist.md#michael-ellis-fisher) used an [epsilon expansion](#epsilon-expansion) about $d=4$ to compute nonclassical [critical exponents](#critical-exponent). Their paper distinguishes a [Gaussian fixed point](#gaussian-fixed-point) from an interacting [renormalization-group fixed point](#renormalization-group-fixed-point), tunes the thermal parameter, and extracts powers from a linearized recursion. Its Ising-like result is $\gamma=1+\epsilon/6+O(\epsilon^2)$ for $d=4-\epsilon$.[Critical Exponents in 3.99 Dimensions, Physical Review Letters 28 (1972), pp. 240–242, abstract and equations (7), (10)–(14); p. 243 discusses the more general interaction and accuracy of the approximation](physics-bibliography.md#critical-exponents-in-3-99-dimensions-by-kenneth-geddes-wilson-and-michael-ellis-fisher) The worked model below isolates this mechanism with chosen coefficients; it is not a precision calculation for the three-dimensional [Ising model](spin-model.md#ising-model).

### Block-spin coarse-graining

↑ **Parent:** [Renormalization group](#renormalization-group)

Consider [Ising spins](spin-model.md#ising-spin-variable) $s_i=\pm1$ on a square lattice of spacing $a$. Divide it into disjoint $3\times3$ blocks $B$ and retain the majority sign $S_B$. Each block contains nine spins, so a tie is impossible. For example, five positive and four negative spins produce $S_B=+1$. All $2^9$ configurations are assigned a retained sign; the individual pattern within a block is lost. A [coarse-grained variable](statistical-physics.md#coarse-grained-variable) has fewer possible values than the microscopic configuration it summarizes.

The spacing between block centres is $3a$. In coordinates $x'=x/3$ it is again $a$, so the retained pattern can be compared with the original lattice at the same numerical cutoff. This coordinate change does not physically shrink the sample. A majority picture alone does not specify the new interactions: the [blocking kernel](#blocking-kernel) and original [Boltzmann weights](canonical-ensemble.md#boltzmann-factor) determine their probabilities. The figure is a constructed configuration, not a simulated equilibrium state or a claim that majority blocking closes the nearest-neighbour [Ising model](spin-model.md#ising-model).

<a id="image-block-spin-coarse-graining-retains-a-majority-variable-then-restores-the-coordinate-convention"></a>
![](renormalization-block-spin-coarse-graining.png)

**[Figure 3](#image-block-spin-coarse-graining-retains-a-majority-variable-then-restores-the-coordinate-convention). Block-spin coarse-graining retains a majority variable, then restores the coordinate convention**. Original constructed $9\times9$ [Ising spin](spin-model.md#ising-spin-variable) pattern, its nine majority signs at spacing $3a$, and the same signs after $x'=x/3$. Red and blue mean $+1$ and $-1$. The last panel occupies one third of the original linear extent in the rescaled coordinates.

### Integrating and rescaling a statistical model

↑ **Parent:** [Renormalization group](#renormalization-group)

Use a dimensionless [statistical Hamiltonian](statistical-physics.md#statistical-hamiltonian) $\mathcal H=H/(k_BT)$, so that the [partition function](canonical-ensemble.md#canonical-partition-function) is $Z=\sum_s e^{-\mathcal H(s)}$. Choose a [normalized blocking kernel](#normalized-blocking-kernel) $B(S\mid s)$ with $\sum_S B(S\mid s)=1$. For the majority example it is one when every block has its prescribed majority, and zero otherwise. Define the coarse [statistical Hamiltonian](statistical-physics.md#statistical-hamiltonian) by the displayed sum. Then an elementary interchange of finite sums proves

$$
Z'=\sum_S e^{-\mathcal H'(S)}=\sum_s e^{-\mathcal H(s)}\sum_S B(S\mid s)=Z.
$$

The probability of a retained pattern is therefore its original marginal probability. For any observable $A(S)$ of the retained variables,

$$
\langle A\rangle'=\frac1Z\sum_s e^{-\mathcal H(s)}\sum_S B(S\mid s)A(S).
$$

This is the sense in which elimination preserves predictions for retained information. It does not reconstruct every microscopic observable from a block sign.

Next express positions in units of the enlarged spacing: $x'=x/b$, where $b>1$. In a continuum version, rescale the retained [scalar field](classical-field-theory.md#scalar-field) as well to restore a chosen [gradient energy](#gradient-energy) coefficient; any change in the integration measure contributes to the field-independent term. The result is a new set of dimensionless couplings. Repeating the procedure defines a [renormalization-group flow](#renormalization-group-flow). Additional interactions and the additive constant generally appear, even if the starting [statistical Hamiltonian](statistical-physics.md#statistical-hamiltonian) was simple. Keeping only a few terms is an approximation; the equality of [partition functions](canonical-ensemble.md#canonical-partition-function) above applies to the complete coarse weight. See also the [Wilsonian coarse-grained statistical Hamiltonian](#wilsonian-coarse-grained-statistical-hamiltonian) for integration over fast [Fourier modes](fourier-analysis.md#fourier-mode).

### A solvable infrared renormalization flow

↑ **Parent:** [Renormalization group](#renormalization-group)

Take the following bounded analytic example for a dimensionless positive coupling $g$, with fixed $\epsilon>0$ and $g(0)=g_0>0$:

$$
\frac{dg}{d\ell}=\epsilon g-g^2,\qquad
\ell=\log b=\log(L/a).
$$

Increasing $\ell$ means increasing observation length $L$, hence motion toward the [infrared fixed point](#infrared-fixed-point). This convention matters: if the inverse-length scale is $\mu=\mu_0e^{-\ell}$, the same trajectory has [renormalization-group beta function](perturbative-quantum-field-theory.md#beta-function-physics) $\beta_\mu(g)=\mu\,dg/d\mu=-\epsilon g+g^2$. The two derivatives have opposite signs.

To solve the equation, set $v=1/g$. It obeys $dv/d\ell=-\epsilon v+1$, a linear [ordinary differential equation](differential-equation.md#ordinary-differential-equation). Therefore

$$
g(\ell)=\frac{\epsilon}{1+(\epsilon/g_0-1)e^{-\epsilon\ell}}.
$$

For $\ell\geq0$ its denominator is positive, and $g$ stays between $g_0$ and $\epsilon$. Thus the trajectory is bounded on this domain. The [renormalization-group fixed points](#renormalization-group-fixed-point) are $g=0$ and $g_*=\epsilon$. The derivative of the length-flow right-hand side is $\epsilon-2g$: zero is repulsive from positive $g$, whereas $g_*$ has [eigenvalue](linear-operator-theory.md#eigenvalue) $-\epsilon$ and attracts positive trajectories. Linearization gives $g-g_*\propto e^{-\epsilon\ell}=b^{-\epsilon}$ near $g_*$. The inverse-length [beta function](complex-analysis.md#beta-function) has positive derivative at the same infrared-attractive point.

For the chosen $\epsilon=1/5$, take two starting models with $g_0=1/20$ and $g_0=3/5$. At $b=1024$, $e^{-\epsilon\ell}=1/4$, so their couplings are respectively $4/35$ and $6/25$. Both move toward $1/5$, from opposite sides. They are still visibly different: slow decay of an [irrelevant operator](#irrelevant-operator) can leave substantial corrections at accessible lengths. The case $g_0=0$ stays exactly zero and is outside this positive-coupling basin.

### Correlation-length scaling from a thermal direction

↑ **Parent:** [Renormalization group](#renormalization-group)

Add a thermal scaling coordinate $t$, with its critical value subtracted, satisfying

$$
\frac{dt}{d\ell}=y_t t,\qquad t(\ell)=b^{y_t}t_0,\qquad y_t>0.
$$

This is a [relevant direction of a fixed point](#relevant-direction-of-a-fixed-point). A thermal scaling coordinate agrees to leading order with a nonzero multiple of [reduced temperature](#reduced-temperature); in a general model it can mix several bare parameters. An ordering [conjugate field](#field-conjugate-to-an-order-parameter) is held at its critical value. The combined [stability matrix](dynamical-systems.md#stability-matrix) at $(g,t)=(\epsilon,0)$ has [eigenvalues](linear-operator-theory.md#eigenvalue) $-\epsilon$ and $y_t$. Attraction along $g$ therefore does not make the critical point attractive against thermal detuning. The [critical surface](#critical-surface) in this example is $t=0$.

Let $X=\xi/a$ denote the [correlation length](#correlation-length) in microscopic lattice units. A [renormalization-group transformation](#renormalization-group-transformation) of length factor $b$ gives

$$
X(t_0,g_0)=b\,X(b^{y_t}t_0,g(\log b)).
$$

Indeed, a tail with exponential envelope $\exp(-r/\xi)$ becomes $\exp[-r'/(\xi/b)]$ under $r'=r/b$. Choose the stopping scale $b_*=|t_0|^{-1/y_t}$ so that the transformed thermal coordinate is $+1$ or $-1$. If the stopped [correlation length](#correlation-length) tends to a finite nonzero value $C_\pm$ as the irrelevant coupling approaches $g_*$, then

$$
\frac{\xi}{a}\sim C_\pm |t_0|^{-1/y_t},\qquad \nu=\frac1{y_t}.
$$

The limit requires $|t_0|\ll1$ and enough room between $a$, $\xi$, and the sample size. Singular dependence on a [dangerously irrelevant coupling](#dangerously-irrelevant-coupling) or a [marginal operator](#marginal-operator) needs separate analysis. On an ordered branch, use the [connected correlation function](#connected-correlation-function) in a [pure thermodynamic phase](#pure-thermodynamic-phase).

For a completely specified illustrative scaling model choose $y_t=3/2$ and $X=C_+t^{-2/3}$ for $t>0$. Then $t=10^{-3}$ gives $X=100C_+$, whereas $t=10^{-6}$ gives $X=10^4C_+$. With $b=4$, $t'=8t$ and $X(t')=X(t)/4$. Models with $C_+=1$ and $C_+=2$ have different lengths but identical curves after plotting $X/C_+$ against $t$. This collapse checks the chosen scaling law; agreement of real data would test that law, rather than follow from this example. Neither $\epsilon=1/5$ nor $y_t=3/2$ is being fitted to a three-dimensional [Ising model](spin-model.md#ising-model).

<a id="image-a-chosen-renormalization-group-flow-loses-coupling-detail-while-a-correlation-length-grows"></a>
![](renormalization-flow-and-correlation-length.png)

**[Figure 4](#image-a-chosen-renormalization-group-flow-loses-coupling-detail-while-a-correlation-length-grows). A chosen renormalization-group flow loses coupling detail while a correlation length grows**. Left: exact positive trajectories of $dg/d\ell=g/5-g^2$ approach $g_*=1/5$ for increasing log length. Right: the chosen $y_t=3/2$ gives $\xi/a=C_+t^{-2/3}$; different amplitudes collapse after division by $C_+$. These are analytic model curves, not experimental data or precision three-dimensional [Ising model](spin-model.md#ising-model) predictions.

### Why microscopic differences fade near criticality

↑ **Parent:** [Renormalization group](#renormalization-group)

Near a [renormalization-group fixed point](#renormalization-group-fixed-point), expand a difference between two nearby models in [eigenvectors](linear-operator-theory.md#eigenvector) of the [stability matrix](dynamical-systems.md#stability-matrix). An [irrelevant operator](#irrelevant-operator) direction has $y_i<0$, so its dimensionless coefficient shrinks under increasing length factor $b$. A [relevant operator](#relevant-operator) direction grows and must be tuned to study the same critical behavior. This is a mechanism for losing microscopic detail, not an assertion that every parameter disappears. Critical [temperature](temperature.md), individual amplitudes and regular contributions to [free energy](thermodynamic-potential.md#thermodynamic-free-energy) can remain material dependent.

For the solvable example, write $A=\epsilon/g_0-1$. Its exact solution gives $g-\epsilon=-\epsilon A b^{-\epsilon}+O(b^{-2\epsilon})$. At the thermal stopping scale $b_*=|t_0|^{-1/y_t}$ this is of order $|t_0|^{\epsilon/y_t}$. If the stopped [correlation length](#correlation-length) is smooth in $g$, the leading correction to its power law has that order. Thus two microscopic couplings can yield the same limiting [critical exponent](#critical-exponent), yet approach it at different rates.

This mechanism makes [universality](#universality-of-critical-phenomena) useful: one tractable representative can predict [critical exponents](#critical-exponent) and normalized scaling forms for many systems in its [universality class](#universality-class). A [liquid-gas critical point](#liquid-gas-critical-point) and a scalar magnetic transition can share a long-distance description even though their microscopic constituents differ. The scope must be checked: spatial dimension, [order parameter](#order-parameter) symmetry, interaction range, and extra soft variables can change the [renormalization-group fixed point](#renormalization-group-fixed-point).

In his lecture, [Kenneth Geddes Wilson](physicist.md#kenneth-geddes-wilson) connects limiting [renormalization-group fixed points](#renormalization-group-fixed-point) with common critical behavior and states the limits of his elementary truncation.[Section II, pp. 110–112: truncation limits and common critical behavior](physics-bibliography.md#the-renormalization-group-and-critical-phenomena-by-kenneth-geddes-wilson)

### Ultraviolet fixed point

↑ **Parent:** [Renormalization group](#renormalization-group)

A zero of the [beta function](complex-analysis.md#beta-function) approached by the [running coupling](perturbative-quantum-field-theory.md#running-coupling) as the energy scale increases. A simple one-coupling fixed point with $\beta'(g_*)<0$ attracts nearby flows. Such a point can control [two-point scaling at an ultraviolet fixed point](#two-point-scaling-at-an-ultraviolet-fixed-point).

#### Two-point scaling at an ultraviolet fixed point

↑ **Parent:** [Ultraviolet fixed point](#ultraviolet-fixed-point)

If $g(t)\to g_*$, $\gamma(g(t))\to\gamma_*$ and the reference correlator has a finite nonzero fixed-point limit, the [characteristic solution of the multiplicative Callan-Symanzik equation](perturbative-quantum-field-theory.md#characteristic-solution-of-the-multiplicative-callan-symanzik-equation) gives $\log f(t)=2\gamma_*t+o(t)$. A simple attractive fixed point and smooth [anomalous dimension](#anomalous-dimension) give a finite prefactor multiplying $e^{2\gamma_*t}$. A nonsimple fixed point can retain slower corrections.

### Anisotropic renormalization group

↑ **Parent:** [Renormalization group](#renormalization-group)

A [renormalization-group transformation](#renormalization-group-transformation) can scale different coordinate directions by different factors to keep distinct gradient terms fixed. If momentum component $p_i$ scales to $b^{w_i}p_i$, its coordinate scales by $b^{-w_i}$. The momentum/volume measure has total scaling weight $\sum_iw_i$, motivating the [anisotropic effective dimension](#anisotropic-effective-dimension).

#### Anisotropic Gaussian smectic scaling

↑ **Parent:** [Anisotropic renormalization group](#anisotropic-renormalization-group)

For a Gaussian kernel $Kq_\parallel^2+Lq_\perp^4+t$, keeping both [gradient](multivariable-calculus.md#gradient) coefficients fixed gives $q'_\parallel=bq_\parallel$ and $q'_\perp=b^{1/2}q_\perp$. The volume rescales by $b^{(d+1)/2}$. Fourier-field normalization is $m'(q')=m(q)/b^{(d+5)/4}$; the real-space normalization instead divides by $b^{(3-d)/4}$. The thermal coefficient scales by $b^2$ and the uniform source by $b^{(d+5)/4}$. Thus $\xi_\parallel\sim t^{-1/2}$, $\xi_\perp\sim t^{-1/4}$ and the formal Gaussian free-energy powers are $\alpha=(7-d)/4$, $\Delta=(d+5)/8$.

#### Anisotropic effective dimension

↑ **Parent:** [Anisotropic renormalization group](#anisotropic-renormalization-group)

The effective dimension for a specified anisotropic rescaling is the total scaling weight of its coordinate measure. With $D_\perp$ directions of weight 1 and $D_\parallel$ directions of weight $\theta$, $d_{\mathrm{eff}}=D_\perp+\theta D_\parallel$. The uniaxial Gaussian [Lifshitz point](#lifshitz-point) has $\theta=1/2$, so $d_{\mathrm{eff}}=D-1/2$. This is not a topological or Hausdorff dimension.

### Renormalization-group transformation

↑ **Parent:** [Renormalization group](#renormalization-group)

A renormalization-group transformation integrates out selected short-distance degrees of freedom and restores chosen cutoff and field-normalization conventions. It defines a map $R_b$ on couplings at a length factor $b$. Its discrete [Jacobian matrix](multivariable-calculus.md#jacobian-matrix) multipliers differ from [eigenvalues](linear-operator-theory.md#eigenvalue) of the generator of a continuous [renormalization-group flow](#renormalization-group-flow); the relation for a scaling direction is $\lambda=b^y$.

#### Additive free-energy recursion under blocking

↑ **Parent:** [Renormalization-group transformation](#renormalization-group-transformation)

For dimensionless free energy per site $F(u,C)=f(u)+\beta C$, an exact [blocking kernel](#blocking-kernel) preserves the [partition function](canonical-ensemble.md#canonical-partition-function) and gives $F(u,C)=b^{-D}F(u',C')$. Thus $f(u)=b^{-D}f(u')+g(u)$, where $g(u)=\beta[b^{-D}C'-C]$ is the additive contribution from the eliminated degrees of freedom. Repeating this equality gives the displayed sum. After subtracting analytic backgrounds, the singular [free-energy density](statistical-physics.md#free-energy-density) obeys the homogeneous [scaling hypothesis for critical phenomena](#scaling-hypothesis-for-critical-phenomena), subject to marginal or dangerous-variable qualifications.

#### Blocking kernel

↑ **Parent:** [Renormalization-group transformation](#renormalization-group-transformation)

A blocking kernel assigns a conditional probability to coarse configurations given microscopic configurations. Multiplying each microscopic Boltzmann weight by the kernel and summing over microscopic configurations defines the coarse Hamiltonian. The normalization preserves the [partition function](canonical-ensemble.md#canonical-partition-function) exactly when the coarse operator space is not truncated. In $D$ dimensions a blocking factor $b$ changes the lattice spacing to $ba$ and the number of sites to $N/b^D$. Generated interactions and additive constants must be retained for the transformation to remain exact.

### Real-space renormalization group

↑ **Parent:** [Renormalization group](#renormalization-group)

A real-space [renormalization group](#renormalization-group) replaces groups of microscopic degrees of freedom by retained coarse variables, summing over the eliminated variables to define a coarse [Hamiltonian](hamiltonian-mechanics.md#hamiltonian). The effective Boltzmann weights must preserve the [partition function](canonical-ensemble.md#canonical-partition-function) up to a tracked normalization. [Spin decimation](#spin-decimation) retains selected spins rather than forming an average block variable. Coarse-graining generally generates additional interactions, so closure of a chosen finite coupling family requires justification.

#### Migdal-Kadanoff approximation

↑ **Parent:** [Real-space renormalization group](#real-space-renormalization-group)

A real-space approximation that moves or combines lattice bonds so that selected intermediate spins can be summed through a chain recursion. On a one-dimensional nearest-neighbour [Ising model](spin-model.md#ising-model), no transverse [bond moving](#bond-moving) is needed and [exact zero-field Ising-chain decimation](#exact-zero-field-ising-chain-decimation) closes exactly. In higher dimensions, neglected geometric [correlations](variance.md#pearson-correlation-coefficient) generally make the transformed model approximate on the original lattice. The order of [bond moving](#bond-moving) and decimation must be stated; the two operations need not commute. The bond-moving-first convention is described in [Position Space Renormalization Group by Mehran Kardar](physics-bibliography.md#position-space-renormalization-group-by-mehran-kardar) lecture 14, section V.D.

##### Bond moving

↑ **Parent:** [Migdal-Kadanoff approximation](#migdal-kadanoff-approximation)

In the bond-moving-first hypercubic construction with blocking [length](physics.md#length) $b$, combine $b^{d-1}$ transverse-equivalent bonds into each link of a surviving $b$-link chain. Summing that chain gives the displayed [Migdal-Kadanoff approximation](#migdal-kadanoff-approximation). For $b=2$, it becomes $K'=\tfrac12\log\cosh(2^dK)$. The $d=1$ specialization is exact; the higher-dimensional formula is a convention-dependent approximation, not an exact closure of the original hypercubic model.

#### Normalized blocking kernel

↑ **Parent:** [Real-space renormalization group](#real-space-renormalization-group)

A [normalized blocking kernel](#normalized-blocking-kernel) assigns probabilities or delta constraints for [coarse-grained variables](statistical-physics.md#coarse-grained-variable) given a microscopic configuration. Multiplying the microscopic Boltzmann weight by this kernel and summing over eliminated variables defines the blocked [statistical Hamiltonian](statistical-physics.md#statistical-hamiltonian). Normalization preserves the [partition function](canonical-ensemble.md#canonical-partition-function) exactly when all generated operators and the field-independent constant are retained. A finite-coupling truncation may lose that exactness.

##### Identity-operator contribution to renormalization-group free energy

↑ **Parent:** [Normalized blocking kernel](#normalized-blocking-kernel)

If an energy per site $C$ multiplies the identity operator, blocking sends $C$ to $b^DC+c(u)$. For [free energy](thermodynamic-potential.md#thermodynamic-free-energy) per site $F=C+f(u)$, exact [partition function](canonical-ensemble.md#canonical-partition-function) invariance gives the displayed inhomogeneous equation with $g=b^{-D}c$. It records eliminated-mode [entropy](entropy.md), vacuum contributions and measure normalization. Removing a suitable regular background leaves homogeneous singular scaling; additive logarithmic resonances can obstruct a strictly analytic subtraction.

###### Analytic subtraction of an inhomogeneous renormalization recursion

↑ **Parent:** [Identity-operator contribution to renormalization-group free energy](#identity-operator-contribution-to-renormalization-group-free-energy)

For the [renormalization-group transformation](#renormalization-group-transformation) $f(u)=b^{-D}f(R_bu)+g(u)$, a background solving $a(u)=b^{-D}a(R_bu)+g(u)$ leaves a homogeneous remainder. In linear scaling coordinates $t'=b^{\lambda_t}t$ and $h'=b^{\lambda_h}h$, an analytic source term $g_{mn}t^mh^n$ is removed by $a_{mn}=g_{mn}/[1-b^{m\lambda_t+n\lambda_h-D}]$ unless the denominator vanishes. Such a resonance may produce a logarithm and invalidate a pure homogeneous power law. The [scaling hypothesis for critical phenomena](#scaling-hypothesis-for-critical-phenomena) concerns the singular remainder. A regular field-dependent background cannot generally be represented by a function of temperature alone; an arbitrary analytic identity term proportional to $h^2$ makes this explicit.

###### Renormalization-group free-energy resonance

↑ **Parent:** [Analytic subtraction of an inhomogeneous renormalization recursion](#analytic-subtraction-of-an-inhomogeneous-renormalization-recursion)

An analytic source monomial $g_{mn}t^mh^n$ in an additive [renormalization-group transformation](#renormalization-group-transformation) of [free-energy density](statistical-physics.md#free-energy-density) is resonant when its scaling degree equals the spatial dimension. The analytic background coefficient would require division by $1-b^{m\lambda_t+n\lambda_h-D}=0$. On a branch with $t\ne0$ and $\lambda_t>0$, a particular nonanalytic background is $-g_{mn}t^mh^n\log|t|/(\lambda_t\log b)$: substituting $t'=b^{\lambda_t}t$, $h'=b^{\lambda_h}h$ verifies the additive recursion exactly. Thus logarithms can be required even when the eliminated-mode source is analytic. This is distinct from marginal interaction running, which can create additional logarithmic corrections.

#### Reciprocal coordinate at infinite coupling

↑ **Parent:** [Real-space renormalization group](#real-space-renormalization-group)

An infinite positive coupling coordinate $v$ can be studied through $w=1/v$, with $v=\infty$ represented by $w=0$. For example, $v'=v^4/A(u)$ with $A(u)>0$ becomes $w'=A(u)w^4$, a smooth map at zero. This gives a well-defined boundary [renormalization-group fixed point](#renormalization-group-fixed-point) whose derivative in the reciprocal direction is zero. One should use this chart rather than substituting infinity into an ordinary finite-coordinate Jacobian.

#### Spin decimation

↑ **Parent:** [Real-space renormalization group](#real-space-renormalization-group)

[Spin decimation](#spin-decimation) sums over spins at selected lattice sites while retaining the others. For alternate-site elimination in a nearest-neighbour periodic chain of even length, the coarse [spin-chain transfer matrix](spin-model.md#transfer-matrix-for-a-classical-spin-chain) is $W^2$, because its $(s,t)$ entry sums $W_{sa}W_{at}$ over the eliminated middle spin. Exact preservation $\operatorname{tr}(W^2)^{N/2}=\operatorname{tr}W^N$ requires keeping the scalar normalization as well as the entry ratios.

##### Exact zero-field Ising-chain decimation

↑ **Parent:** [Spin decimation](#spin-decimation)

Keep every $b$th spin in a ferromagnetic nearest-neighbour [Ising model](spin-model.md#ising-model) at zero field, with coupling $K=J/(k_BT)$. Multiplying its two-state [transfer matrix](combinatorics.md#transfer-matrix) $b$ times yields the displayed recursion. For $b=2$, direct summation of one intermediate spin gives $2\cosh[K(s+s')]=A e^{K'ss'}$, with $K'=\tfrac12\log\cosh2K$. The new spacing is $ba$ before coordinate rescaling. All finite positive couplings flow toward the disordered fixed point $K=0$; the ordered zero-temperature endpoint is unstable to a nonzero domain-wall number per bond.

###### Finite-field Ising-chain decimation

↑ **Parent:** [Exact zero-field Ising-chain decimation](#exact-zero-field-ising-chain-decimation)

Use the symmetric [transfer matrix](combinatorics.md#transfer-matrix) $T_{ss'}=\exp[Kss'+h(s+s')/2]$ with dimensionless field $h$. For blocking [length](physics.md#length) two set $W=T^2$, then write $W_{ss'}=A\exp[K'ss'+h'(s+s')/2]$. Matching its three independent entries proves the title relations and gives $A=(W_{++}W_{--}W_{+-}^2)^{1/4}$. Explicitly $W_{\pm\pm}=e^{2K\pm2h}+e^{-2K}$ and $W_{+-}=2\cosh h$. At zero field the exact chain recursion is recovered; at $K=0$ the independent-spin field stays unchanged. Splitting the field equally between neighboring bonds is essential for this normalization.

###### Domain-wall scaling coordinate of an Ising chain

↑ **Parent:** [Exact zero-field Ising-chain decimation](#exact-zero-field-ising-chain-decimation)

A reversed bond costs $2J$, so its [Boltzmann factor](canonical-ensemble.md#boltzmann-factor) $w=e^{-2J/(k_BT)}$ is a natural thermal coordinate near the zero-temperature chain fixed point. Exact length-two decimation gives $w'\simeq2w$, and the [One-dimensional Ising correlation function](spin-model.md#one-dimensional-ising-correlation-function) gives $\xi/a=-1/\log\tanh K\sim1/(2w)$. This is a [length](physics.md#length) exponent one with respect to $w$. The [correlation length](#correlation-length) instead diverges exponentially in inverse physical [temperature](temperature.md); claiming a conventional finite power $T^{-1}$ would confuse scaling coordinates. Choosing $e^{-K}$ gives multiplier $\sqrt2$ and power two in that alternative coordinate, the same physical [length](physics.md#length).

###### Ising-chain decimation constant

↑ **Parent:** [Exact zero-field Ising-chain decimation](#exact-zero-field-ising-chain-decimation)

For a periodic even chain, eliminating alternate spins gives $Z_N(K)=A^{N/2}Z_{N/2}(K')$. Thus dimensionless [free energy](thermodynamic-potential.md#thermodynamic-free-energy) per original spin obeys $f(K)=-\tfrac12\log A+\tfrac12 f(K')$. The exact solution $f(K)=-\log(2\cosh K)$ satisfies this relation. The multiplicative constant cancels from normalized retained-spin [probabilities](probability-theory.md#probability) but records eliminated-spin [entropy](entropy.md); discarding it loses thermodynamics even if the interaction recursion is correct.

##### Checkerboard decimation of the square-lattice Ising model

↑ **Parent:** [Spin decimation](#spin-decimation)

Checkerboard [spin decimation](#spin-decimation) retains one parity sublattice of a square-lattice [Ising model](spin-model.md#ising-model) and sums over the other. The retained primitive vectors are $a(1,1)$ and $a(1,-1)$, so the coarse lattice is again square with spacing $\sqrt2a$. A rotation and length rescaling restore the original geometry. Every original nearest-neighbour bond joins the two parity classes, whereas a diagonal next-nearest-neighbour bond stays within one class.

###### Leading checkerboard Ising decimation recursion

↑ **Parent:** [Checkerboard decimation of the square-lattice Ising model](#checkerboard-decimation-of-the-square-lattice-ising-model)

For dimensionless nearest-neighbour coupling $K$ and diagonal coupling $L$, the second cumulant in [checkerboard decimation of the square-lattice Ising model](#checkerboard-decimation-of-the-square-lattice-ising-model) generates $K^2$ for each pair of retained neighbours of an eliminated centre. A retained diagonal pair shares two centres, and an axial pair at distance $2a$ shares one. The displayed two-coupling recursion neglects $K^4$, $K^2L$, and $L^2$, treating $L$ as order $K^2$. Its finite nontrivial [renormalization-group fixed point](#renormalization-group-fixed-point) is $(K,L)=(1/3,1/9)$. Higher orders generate additional operators, so the closure is a property of the truncation.

##### Spin-1 chain decimation recursion

↑ **Parent:** [Spin decimation](#spin-decimation)

For the [spin inversion symmetry](spin-model.md#spin-inversion-symmetry) parameterization $W=c\begin{pmatrix}1&x&y\\x&z&x\\y&x&1\end{pmatrix}$ with positive entries, [spin decimation](#spin-decimation) gives the same form with $x'=x(1+y+z)/(1+x^2+y^2)$, $y'=(x^2+2y)/(1+x^2+y^2)$ and $z'=(z^2+2x^2)/(1+x^2+y^2)$. Multiply $W$ by itself and divide by its $(+,+)$ entry to prove these ratios. The leftover scalar is an additive free-energy coupling; dropping it leaves normalized expectations unchanged but loses the full [free energy](thermodynamic-potential.md#thermodynamic-free-energy).

### Momentum-shell renormalization group

↑ **Parent:** [Renormalization group](#renormalization-group)

The momentum-shell renormalization group splits a field into slow modes below $\Lambda/\zeta$ and fast modes in $\Lambda/\zeta<|k|<\Lambda$, integrates out the fast modes, then rescales momenta and fields to restore the cutoff and kinetic normalization.

#### Wilsonian coarse-grained statistical Hamiltonian

↑ **Parent:** [Momentum-shell renormalization group](#momentum-shell-renormalization-group)

Integrate field modes with momenta between a fixed microscopic [ultraviolet cutoff](quantum-field-theory.md#ultraviolet-cutoff) $\Lambda_0$ and a lower cutoff $\Lambda$, retaining the modes below $\Lambda$ as backgrounds. The exact [statistical Hamiltonian](statistical-physics.md#statistical-hamiltonian) includes all generated interactions and field-independent constants. Integrating its retained modes reproduces the original [partition function](canonical-ensemble.md#canonical-partition-function), so long-distance observables do not depend on the arbitrary intermediate cutoff. With sources retained, the corresponding coarse observables reproduce long-distance response and [connected correlation functions](#connected-correlation-function). A local [gradient expansion](#gradient-expansion) or a finite-coupling truncation is an additional approximation, rather than a consequence of cutoff independence. The momentum-shell construction is also explained in [the Cambridge statistical field theory lecture notes](https://www.damtp.cam.ac.uk/user/tong/sft/sfthtml/S3.html).

#### One-loop shell quartic renormalization

↑ **Parent:** [Momentum-shell renormalization group](#momentum-shell-renormalization-group)

For centered fast [Fourier modes](fourier-analysis.md#fourier-mode) and $V=u\int\phi^4/4!$, the two-fast-field vertex is $(u/4)\int\varphi^2\eta^2$. Its connected second [cumulant](probability-distribution.md#cumulant) uses $\langle\eta^2(x)\eta^2(y)\rangle_c=2G_>(x-y)^2$, producing $-u^2\int\varphi^2(x)\varphi^2(y)G_>(x-y)^2/16$. Extracting the local zero-external-momentum quartic coefficient gives $u'=b^{4-D}(u-3u^2I_2/2)+\cdots$, where $I_2=\int_{\rm shell}d^Dp\,(2\pi)^{-D}K(p)^{-2}>0$. At $D=4$ its sign makes weak positive quartic coupling [marginally irrelevant](#marginally-irrelevant-operator) for increasing length scale, after tuning the critical mass. This local truncation omits generated derivative and higher-order operators; it is not the exact complete finite-shell effective action.

#### One-loop shell mass renormalization in scalar quartic theory

↑ **Parent:** [Momentum-shell renormalization group](#momentum-shell-renormalization-group)

For interaction $V=u\int\phi^4/4!$, split $\phi=\varphi+\eta$ into slow and fast [Fourier modes](fourier-analysis.md#fourier-mode), with a centered fast [Gaussian measure](gaussian-process.md#gaussian-measure). The first [cumulant expansion](probability-distribution.md#cumulant-expansion) term is $\langle V\rangle=(u/24)\int[\varphi^4+6G_>(0)\varphi^2+3G_>(0)^2]$ by [Wick theorem](perturbative-quantum-field-theory.md#wick-s-theorem). The constant shifts the [free energy](thermodynamic-potential.md#thermodynamic-free-energy), the quadratic term gives $\delta r=uG_>(0)/2$, and there is no [gradient](multivariable-calculus.md#gradient) correction at this order. Rescaling gives $r'=b^2[r+uG_>(0)/2]+O(u^2)$ and $u'=b^{4-D}u+O(u^2)$. The mass shift mixes thermal and quartic perturbations; the interacting critical tuning need not have zero bare mass.

#### Gaussian shell covariance

↑ **Parent:** [Momentum-shell renormalization group](#momentum-shell-renormalization-group)

For a centered shell [Gaussian measure](gaussian-process.md#gaussian-measure) of a real [scalar field](classical-field-theory.md#scalar-field) with positive shell kernel $K(p)=\kappa p^2+r$, its [Gaussian functional integral](quantum-field-theory.md#gaussian-functional-integral) gives $\langle\widetilde\phi(p)\widetilde\phi(q)\rangle=(2\pi)^D\delta^{(D)}(p+q)/K(p)$ on the shell. Inverse [Fourier transforms](fourier-transform.md) therefore yield $G_>(x-y)=\int_{\Lambda/b<|p|\leq\Lambda}d^Dp\,(2\pi)^{-D}e^{ip\cdot(x-y)}/K(p)$. The kernel must be positive throughout the shell. [Translation invariance](physics.md#translation-invariance) makes the separation essential; a numerator involving $x$ alone is valid only with $y=0$ or if $x$ is redefined as the separation.

#### Quartic interaction generated by a sextic interaction

↑ **Parent:** [Momentum-shell renormalization group](#momentum-shell-renormalization-group)

Splitting a [scalar field](classical-field-theory.md#scalar-field) into slow and fast components $\phi=\varphi+\eta$, the [Wick contractions](perturbative-quantum-field-theory.md#wick-contraction) in $\lambda\langle(\varphi+\eta)^6\rangle$ generate $15\lambda\langle\eta^2\rangle\varphi^4$. A vanishing bare quartic coupling is therefore not generally preserved by [renormalization-group flow](#renormalization-group-flow).

#### Cumulant expansion of a coarse-grained free energy

↑ **Parent:** [Momentum-shell renormalization group](#momentum-shell-renormalization-group)

Writing the interaction as $V$ and averaging over the fast modes, which have a [Gaussian distribution](probability-distribution.md#normal-distribution), gives the [cumulant expansion](probability-distribution.md#cumulant-expansion) $F_{\mathrm{eff}}=F_0+\langle V\rangle-\tfrac12(\langle V^2\rangle-\langle V\rangle^2)+\cdots$. The second cumulant selects [connected Feynman diagrams](perturbative-quantum-field-theory.md#connected-feynman-diagram).

### Engineering dimension

↑ **Parent:** [Renormalization group](#renormalization-group)

The engineering dimension of a field, parameter or operator is its dimension under the rescaling that leaves the quadratic theory invariant. Interactions can change it into a full [scaling dimension](string-theory.md#scaling-dimension).

#### Anomalous dimension

↑ **Parent:** [Engineering dimension](#engineering-dimension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Anomalous_dimension)

An anomalous dimension is the interaction-generated difference between a full [scaling dimension](string-theory.md#scaling-dimension) and its [engineering dimension](#engineering-dimension). For a scalar field, momentum-dependent self-energy corrections require [wave-function renormalization](perturbative-quantum-field-theory.md#wave-function-renormalization) and produce $\Delta_\phi=(d-2+\eta)/2$.

##### Field-renormalization anomalous dimension

↑ **Parent:** [Anomalous dimension](#anomalous-dimension)

If $\phi_B=Z_\phi^{1/2}\phi_R$, differentiating a renormalized $n$-point function at fixed bare parameters gives $(\mu\partial_\mu+\beta\partial_g+n\gamma_\phi)G_{n,R}=0$. With this convention the field [scaling dimension](string-theory.md#scaling-dimension) at a fixed point is its [engineering dimension](#engineering-dimension) plus $\gamma_\phi$. The critical exponent $\eta$ for scalar two-point decay is $2\gamma_\phi$.

##### Field scaling and anomalous dimension

↑ **Parent:** [Anomalous dimension](#anomalous-dimension)

Under a length blocking factor $b$, a scalar scaling field transforms as $\phi'(x')=b^{x_\phi}\phi_<(bx')$. Its critical [connected correlation function](#connected-correlation-function) consequently decays as $r^{-2x_\phi}$. Comparing with $r^{-(D-2+\eta)}$ identifies the anomalous part of the field dimension. The uniform [conjugate field](#field-conjugate-to-an-order-parameter) has scaling exponent $y_h=D-x_\phi$. Wave-function factors must be defined explicitly before assigning a sign to their logarithmic derivatives.

### Renormalization-group flow

↑ **Parent:** [Renormalization group](#renormalization-group)

A renormalization-group flow is the trajectory of effective couplings as the observation scale changes.

#### Repulsive renormalization-group trajectory

↑ **Parent:** [Renormalization-group flow](#renormalization-group-flow)

A repulsive renormalization-group trajectory leaves a [renormalization-group fixed point](#renormalization-group-fixed-point) along its unstable manifold as the coarse-graining length increases. Its tangent directions are [relevant operators](#relevant-operator). The [critical surface](#critical-surface) is instead the stable manifold, whose irrelevant coordinates approach the critical fixed point after relevant fields are tuned. For a discrete step, relevance is determined by multipliers larger than one in magnitude, not merely by their being positive.

#### Renormalization-group fixed point

↑ **Parent:** [Renormalization-group flow](#renormalization-group-flow)

A renormalization-group fixed point is a set of couplings left unchanged by coarse-graining. It describes a scale-invariant theory.

##### Infrared fixed point

↑ **Parent:** [Renormalization-group fixed point](#renormalization-group-fixed-point)

An infrared fixed point attracts renormalization-group flows toward low energies or long distances. If it is interacting, it defines a nontrivial scale-invariant quantum or statistical field theory.

##### Stability matrix of a renormalization-group fixed point

↑ **Parent:** [Renormalization-group fixed point](#renormalization-group-fixed-point)

The stability matrix is the Jacobian of the beta functions at a [renormalization-group fixed point](#renormalization-group-fixed-point). Its eigenvalues classify perturbations as relevant, irrelevant, or marginal.

##### Critical surface

↑ **Parent:** [Renormalization-group fixed point](#renormalization-group-fixed-point)

The critical surface is the stable manifold of a critical [renormalization-group fixed point](#renormalization-group-fixed-point). Tuning every relevant direction places a theory on this surface.

### Gaussian fixed point

↑ **Parent:** [Renormalization group](#renormalization-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaussian_fixed_point)

At the Gaussian fixed point all interaction couplings vanish and scaling dimensions follow from the quadratic theory.

#### Gaussian critical exponent

↑ **Parent:** [Gaussian fixed point](#gaussian-fixed-point)

For quadratic dispersion $p^2+t$ with no interacting anomalous dimension, the thermal and uniform-source scaling eigenvalues are $y_t=2$ and $y_h=(d+2)/2$. The generic homogeneous singular [free-energy density](statistical-physics.md#free-energy-density) has $2-\alpha=d/2$ and gap exponent $\Delta=(d+2)/4$. These Gaussian-model values below the upper critical dimension are not the exponents of an interacting scalar critical point.

##### Gaussian free-energy logarithms at integer singular powers

↑ **Parent:** [Gaussian critical exponent](#gaussian-critical-exponent)

A Gaussian [determinant](multilinear-algebra.md#determinant) with effective dimension $D$ has a singular free-energy contribution proportional to $t^{D/2}$ after subtraction of cutoff-dependent analytic terms. When $D/2$ is a positive integer, a logarithm replaces the pure power. Differentiating the [determinant](multilinear-algebra.md#determinant) sufficiently often gives a marginal momentum integral proportional to $\log t$. For the anisotropic kernel $q_\parallel^2+q_\perp^4+t$, $D=(d+1)/2$, so logarithms occur at $d=3,7,11,\ldots$. These qualify simple homogeneous-power formulas rather than changing the nominal scaling dimensions.

##### Gaussian order-parameter scaling index

↑ **Parent:** [Gaussian critical exponent](#gaussian-critical-exponent)

The [Gaussian momentum-shell scaling](#gaussian-momentum-shell-scaling) has thermal eigenvalue $2$ and source eigenvalue $(D+2)/2$. The formal homogeneous magnetization index is therefore $[D-(D+2)/2]/2=(D-2)/4$. A free quadratic Hamiltonian alone does not possess a stable negative-mass ordered phase, so this index is not a claim of spontaneous magnetization in an unstabilized Gaussian integral. In $2<D<4$, a quartic interaction is relevant at the [Gaussian fixed point](#gaussian-fixed-point) and changes the generic scalar critical behavior.

##### Gaussian specific-heat infrared threshold

↑ **Parent:** [Gaussian critical exponent](#gaussian-critical-exponent)

Two thermal derivatives of a regulated Gaussian [determinant](multilinear-algebra.md#determinant) produce this integral. For $0<D<4$, rescaling $p=\sqrt t\,q$ yields a divergent power $t^{D/2-2}$ and [heat-capacity critical exponent](#heat-capacity-critical-exponent) $\alpha=(4-D)/2$. At four dimensions the singularity is logarithmic, with power exponent zero. Above four the leading [heat capacity](heat.md#heat-capacity) is a finite cutoff-dependent background; its leading bounded-power convention has exponent zero, although the background-subtracted singular Gaussian contribution retains the negative index $2-D/2$. In a stable quartic theory the mean-field ordered [free energy](thermodynamic-potential.md#thermodynamic-free-energy) proportional to $-t^2/u$ instead produces a heat-capacity jump. This is why a [dangerously irrelevant coupling](#dangerously-irrelevant-coupling) qualifies naive [hyperscaling relation](#hyperscaling-relation).

#### Gaussian momentum-shell scaling

↑ **Parent:** [Gaussian fixed point](#gaussian-fixed-point)

After integrating a free-field momentum shell, restore the cutoff with $x'=x/b$ and $\phi'(x')=b^{(D-2)/2}\phi_<(bx')$. The [gradient](multivariable-calculus.md#gradient) coefficient is invariant, the mass changes as $r'=b^2r$, and a uniform conjugate field changes as $h'=b^{(D+2)/2}h$. This follows by counting measure, derivative and field factors in the quadratic [Hamiltonian](hamiltonian-mechanics.md#hamiltonian). A nonuniform source instead obeys $h'(x')=b^{(D+2)/2}h(bx')$, with the source on the right projected onto the retained [Fourier modes](fourier-analysis.md#fourier-mode). The field has [engineering dimension](#engineering-dimension) $(D-2)/2$ and zero [anomalous dimension](#anomalous-dimension).

##### Gaussian free-energy scaling relation

↑ **Parent:** [Gaussian momentum-shell scaling](#gaussian-momentum-shell-scaling)

For a stable massive [Gaussian field theory](#gaussian-field-theory), a finite blocking step yields $F(t,h)=F_{\mathrm{shell}}(t)+b^{-d}F(b^2t,b^{(d+2)/2}h)$ for [free-energy density](statistical-physics.md#free-energy-density). The finite-step shell and measure terms are analytic backgrounds. Generic-dimension singular scaling is homogeneous after subtracting those backgrounds; resonances such as [Gaussian free-energy logarithm at effective dimension two](#gaussian-free-energy-logarithm-at-effective-dimension-two) need additive logarithmic terms.

###### Gaussian free-energy logarithm at effective dimension two

↑ **Parent:** [Gaussian free-energy scaling relation](#gaussian-free-energy-scaling-relation)

For a quadratic determinant in two effective momentum dimensions, differentiating the [free-energy density](statistical-physics.md#free-energy-density) with respect to the squared mass $R$ gives a term proportional to $\log(\Lambda^2/R)$. Integration gives $F_S\propto R\log R$ after subtracting analytic terms. Its thermal power index is still 1, but a strictly homogeneous pure-power expression misses this logarithm. It is a Gaussian determinant resonance, distinct from interaction-generated logarithms at an upper critical dimension.

### Wilson-Fisher fixed point

↑ **Parent:** [Renormalization group](#renormalization-group)

Below four dimensions, the scalar quartic theory has an interacting Wilson-Fisher fixed point that controls the Ising universality class.

This is a particular [fixed point](function.md#fixed-point) of the [renormalization group](#renormalization-group), governing the long-distance behavior of a [critical phenomenon](critical-phenomenon.md).

#### Thermal relevant direction at the Wilson-Fisher fixed point

↑ **Parent:** [Wilson-Fisher fixed point](#wilson-fisher-fixed-point)

The scalar [Wilson-Fisher fixed point](#wilson-fisher-fixed-point) is attractive within its [critical surface](#critical-surface), but has a relevant thermal direction. With $r=m^2\Lambda^{-2}$, $\lambda=g\Lambda^{-\epsilon}$, and $K_D=\Omega_D/(2\pi)^D$, its one-loop equations are $\dot r=2r+K_D\lambda/[2(1+r)]$ and $\dot\lambda=\epsilon\lambda-3K_D\lambda^2/[2(1+r)^2]$. Their [stability matrix](dynamical-systems.md#stability-matrix) at $r_*=-\epsilon/6+O(\epsilon^2)$ and $\lambda_*=16\pi^2\epsilon/3+O(\epsilon^2)$ has the displayed [eigenvalues](linear-operator-theory.md#eigenvalue). Thus an unrestricted claim of infrared attraction is false: the bare mass must be tuned to the critical surface.

<h4 id="o-n-model">O(N) model</h4>

↑ **Parent:** [Wilson-Fisher fixed point](#wilson-fisher-fixed-point)

The $O(N)$ model has an $N$-component real field and an [orthogonal group](linear-algebra.md#orthogonal-group) symmetry. Its standard Landau-Ginzburg interaction is $g(\boldsymbol\phi\cdot\boldsymbol\phi)^2$; below the upper critical dimension its continuous transition is governed by an $O(N)$ [Wilson-Fisher fixed point](#wilson-fisher-fixed-point).

#### Epsilon expansion

↑ **Parent:** [Wilson-Fisher fixed point](#wilson-fisher-fixed-point)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Epsilon_expansion)

The epsilon expansion computes critical quantities perturbatively in $\epsilon=d_c-d$ below an [upper critical dimension](#upper-critical-dimension) $d_c$. For scalar quartic theory, $d_c=4$ and the [Wilson-Fisher fixed point](#wilson-fisher-fixed-point) coupling is of order $\epsilon$.

##### Coupled Ising fixed points near four dimensions

↑ **Parent:** [Epsilon expansion](#epsilon-expansion)

The quartic interaction $g_1\phi_1^4+g_2\phi_2^4+\lambda\phi_1^2\phi_2^2$ includes the [Gaussian fixed point](#gaussian-fixed-point), single and double [Ising model](spin-model.md#ising-model) [Wilson-Fisher fixed points](#wilson-fisher-fixed-point), and an [O(N) model](#o-n-model) fixed point with $N=2$. A rotation of two decoupled identical [Ising models](spin-model.md#ising-model) produces a second coordinate representation of their [renormalization-group fixed point](#renormalization-group-fixed-point).

###### Field-rotation equivalence of decoupled Ising theories

↑ **Parent:** [Coupled Ising fixed points near four dimensions](#coupled-ising-fixed-points-near-four-dimensions)

The [orthogonal transformation](linear-algebra.md#orthogonal-transformation) $\psi_\pm=(\phi_1\pm\phi_2)/\sqrt2$ takes $g(\phi_1^4+\phi_2^4+6\phi_1^2\phi_2^2)$ to $2g(\psi_+^4+\psi_-^4)$. These are the same two decoupled [Ising models](spin-model.md#ising-model) expressed in rotated fields.

### Renormalization-group relevance

↑ **Parent:** [Renormalization group](#renormalization-group)

The relevance of a perturbation is determined by the eigenvalue of its dimensionless coupling under linearized [renormalization-group flow](#renormalization-group-flow). Positive, negative and zero eigenvalues define relevant, irrelevant and marginal perturbations, respectively.

#### Relevant operator

↑ **Parent:** [Renormalization-group relevance](#renormalization-group-relevance)

An operator is relevant at a fixed point when its coupling has positive renormalization-group eigenvalue. Its dimensionless coupling grows under coarse-graining and drives the theory away from the fixed point unless tuned.

##### Relevant direction of a fixed point

↑ **Parent:** [Relevant operator](#relevant-operator)

A perturbation of a [renormalization-group fixed point](#renormalization-group-fixed-point) is relevant if it grows as the coarse-graining length increases. For a continuous flow $d\delta g/d\ell=M\delta g$, an [eigenvector](linear-operator-theory.md#eigenvector) of the linearized [matrix](vector-space.md#matrix) with [eigenvalue](linear-operator-theory.md#eigenvalue) $\sigma$ grows as $e^{\sigma\ell}$; a positive real part is relevant, a negative real part is irrelevant and a zero real part requires nonlinear analysis. For a discrete transformation with length factor $b>1$, its [Jacobian matrix](multivariable-calculus.md#jacobian-matrix) multiplier $\lambda$ instead gives $\delta g_n=\lambda^n\delta g_0$: $|\lambda|>1$ is relevant, $|\lambda|<1$ is irrelevant and $|\lambda|=1$ requires nonlinear analysis. For a positive multiplier the scaling exponent is $y=\log\lambda/\log b$. Thus a positive discrete [eigenvalue](linear-operator-theory.md#eigenvalue) smaller than one is an [irrelevant operator](#irrelevant-operator) direction, while the sign criterion belongs to the continuous generator.

###### Thermal exponent from a discrete renormalization map

↑ **Parent:** [Relevant direction of a fixed point](#relevant-direction-of-a-fixed-point)

A discrete [renormalization group](#renormalization-group) with length factor $b>1$ and positive relevant thermal multiplier $\lambda_t>1$ sends $t$ to $\lambda_t t$ and the [correlation length](#correlation-length) to $\xi/b$. Combining this with $\xi\sim|t|^{-\nu}$ gives the displayed [correlation-length critical exponent](#correlation-length-critical-exponent). The corresponding [scaling dimension](string-theory.md#scaling-dimension) is $y_t=\log\lambda_t/\log b=1/\nu$. Relevance of discrete multipliers is determined by magnitude relative to one, unlike the sign criterion for continuous-flow [eigenvalues](linear-operator-theory.md#eigenvalue).

#### Irrelevant operator

↑ **Parent:** [Renormalization-group relevance](#renormalization-group-relevance)

An operator is irrelevant at a fixed point when its coupling has negative renormalization-group eigenvalue. Its dimensionless coupling decreases under coarse-graining.

#### Marginal operator

↑ **Parent:** [Renormalization-group relevance](#renormalization-group-relevance)

An operator is marginal at linear order when its coupling has zero renormalization-group eigenvalue. Nonlinear terms in its [renormalization-group beta function](perturbative-quantum-field-theory.md#beta-function-physics) determine whether it is marginally relevant, marginally irrelevant, or exactly marginal.

##### Marginally irrelevant operator

↑ **Parent:** [Marginal operator](#marginal-operator)

### Universality class

↑ **Parent:** [Renormalization group](#renormalization-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Universality_class)

Systems belong to one universality class when their long-distance renormalization-group flows approach the same fixed point.

#### Universal singular free-energy amplitude ratio

↑ **Parent:** [Universality class](#universality-class)

Under the [scaling hypothesis for critical phenomena](#scaling-hypothesis-for-critical-phenomena), $F_s=A_f|a_tt|^{D/y_t}\Phi_\pm(0)$ at zero field. The common free-energy and thermal metric factors cancel from $A_+/A_-$, leaving a property of the [universality class](#universality-class). This concerns the singular part at equal $|t|$, not the ratio of full [free energies](thermodynamic-potential.md#thermodynamic-free-energy) including arbitrary analytic identity terms. Matching constants in $\Phi_\pm$ belong to the same scaling solution and cannot be assigned independently.

#### Universal specific-heat amplitude ratio

↑ **Parent:** [Universality class](#universality-class)

When the singular [free-energy density](statistical-physics.md#free-energy-density) has $F_s=A_f|a_tt|^{2-\alpha}\Phi_\pm(0)$, the same thermal and free-energy metric factors multiply the singular [heat capacity](heat.md#heat-capacity) above and below the critical point. Their ratio cancels these factors and depends only on the normalized scaling functions of the [universality class](#universality-class). This statement concerns singular amplitudes, not regular heat-capacity backgrounds, and needs separate treatment at logarithmic resonances or zero amplitudes. Branch matching constants belong to the fixed-point scaling functions and cannot be chosen as independent nonuniversal parameters.

#### Percolation universality hypothesis

↑ **Parent:** [Universality class](#universality-class)

Ordinary short-range independent [bond percolation](bond-percolation.md) and [site percolation](site-percolation.md) on regular lattices of the same spatial dimension are expected to share their [percolation critical exponents](#percolation-critical-exponents) and large-scale limiting behavior. Their [percolation critical probabilities](percolation-theory.md#percolation-critical-probability) can differ. Long-range or correlated models can lie in a different [universality class](#universality-class). A theorem for one lattice alone does not establish this transfer.

### Dangerously irrelevant coupling

↑ **Parent:** [Renormalization group](#renormalization-group)

An irrelevant coupling is dangerously irrelevant when setting it to zero makes a scaling function singular or removes the term needed to stabilize the ordered phase.

## Scaling relation for critical exponents

↑ **Parent:** [Critical phenomenon](critical-phenomenon.md)

Homogeneity at a fixed point relates thermodynamic critical exponents to the correlation-length exponent $\nu$ and anomalous dimension $\eta$.

### Exponent inference from a magnetic data collapse

↑ **Parent:** [Scaling relation for critical exponents](#scaling-relation-for-critical-exponents)

If magnetic data collapse with independently specified [critical exponents](#critical-exponent) $\beta,\gamma$, the ordinary scaling identities infer $\Delta=\beta+\gamma$, $\delta=1+\gamma/\beta$, and the displayed exponents. The [Fisher scaling relation](#fisher-scaling-relation) then gives $\eta=2-\gamma/\nu$. These are conditional inferences, not five additional independent measurements. [Hyperscaling](#hyperscaling-relation) is needed for the spatial exponents, and subtraction can make small inferred $\alpha$ or $\eta$ unusually sensitive to uncertainty. A slope on linear axes is not a fitted logarithmic exponent.

### Fisher scaling relation

↑ **Parent:** [Scaling relation for critical exponents](#scaling-relation-for-critical-exponents)

The [correlation-function susceptibility sum rule](#correlation-function-susceptibility-sum-rule) and $G(r)=r^{-(D-2+\eta)}f_G(r/\xi)$ give $\chi_s\propto\xi^{2-\eta}$ when $f_G(0)$ is finite, its large-distance tail is integrable and $\eta<2$. With [correlation-length critical exponent](#correlation-length-critical-exponent) $\nu$, this gives the displayed relation for the [magnetic-susceptibility critical exponent](#magnetic-susceptibility-critical-exponent). Microscopic distances contribute a regular background rather than the divergent critical power.

#### Matching the amplitude of a massive critical correlation tail

↑ **Parent:** [Fisher scaling relation](#fisher-scaling-relation)

A [connected correlation function](#connected-correlation-function) with critical [anomalous dimension](#anomalous-dimension) $\eta$ scales as $G(r)=\xi^{-(D-2+\eta)}\mathcal G(r/\xi)$. If its large-distance shape is $s^{-(D-1)/2}e^{-s}$, substitution of $s=r/\xi$ produces the displayed amplitude. The extra $\xi^{-\eta}$ relative to the [massive Gaussian field correlation tail](#massive-gaussian-field-correlation-tail) is necessary for matching at $r$ of order $\xi$. Integrating over space gives [magnetic susceptibility](statistical-physics.md#magnetic-susceptibility) proportional to $\xi^{2-\eta}$; omitting that factor would instead make the long-distance contribution scale as $\xi^2$.

### Scaling hypothesis for critical phenomena

↑ **Parent:** [Scaling relation for critical exponents](#scaling-relation-for-critical-exponents)

The scaling hypothesis treats the singular equilibrium [free-energy density](statistical-physics.md#free-energy-density) as a generalized homogeneous function of thermal and field-like scaling variables. Choosing the blocking factor to make the thermal variable order one gives $F_s=|t|^{D/y_t}f_\pm(h/|t|^{y_h/y_t})$. It concerns the singular contribution after subtracting analytic backgrounds. [Dangerously irrelevant couplings](#dangerously-irrelevant-coupling) or marginal logarithms can qualify this simple two-variable form. Differentiation yields [scaling relations for critical exponents](#scaling-relation-for-critical-exponents).

#### Magnetization scaling-function matching

↑ **Parent:** [Scaling hypothesis for critical phenomena](#scaling-hypothesis-for-critical-phenomena)

Differentiate $f_s=|t|^{2-\alpha}g_{f,\pm}(h/|t|^\Delta)$ with respect to its [conjugate field](#field-conjugate-to-an-order-parameter). A finite nonzero one-sided ordered-branch [amplitude](wave.md#wave-amplitude) gives $\beta=2-\alpha-\Delta$. To approach a finite critical isotherm as $t\to0$ at fixed small $h$, the large-argument function must behave as $g_m(x)\sim C\operatorname{sgn}(x)|x|^{1/\delta}$. Cancelling the remaining thermal power yields $\beta=\Delta/\delta$. An analytic background, branch selection and [thermodynamic limit](statistical-physics.md#thermodynamic-limit) must be distinguished from the singular [free energy](thermodynamic-potential.md#thermodynamic-free-energy) being differentiated.

#### Mean-field scalar free-energy scaling

↑ **Parent:** [Scaling hypothesis for critical phenomena](#scaling-hypothesis-for-critical-phenomena)

For a scalar quartic [Landau free energy](#landau-free-energy) $r_tt m^2/2+um^4/4-hm$ with $r_t,u>0$, rescaling $m=(r_t/u)^{1/2}|t|^{1/2}\psi$ gives this minimized scaling form, with $a=r_t^2/u$ and $b=\sqrt u/r_t^{3/2}$. The two functions minimize $\pm\psi^2/2+\psi^4/4-H\psi$. In particular $f_+(0)=0$ and $f_-(0)=-1/4$. Below the transition the equilibrium field dependence has a cusp at zero; pure-phase derivatives are one-sided. The form gives [order-parameter critical exponent](#order-parameter-critical-exponent) $\beta=1/2$ and [magnetic-susceptibility critical exponent](#magnetic-susceptibility-critical-exponent) $\gamma=1$.

### Widom scaling relation

↑ **Parent:** [Scaling relation for critical exponents](#scaling-relation-for-critical-exponents)

The Widom scaling relation is

$$
\gamma=\beta(\delta-1).
$$

It follows by differentiating the homogeneous critical equation of state with respect to the external field.

### Rushbrooke scaling relation

↑ **Parent:** [Scaling relation for critical exponents](#scaling-relation-for-critical-exponents)

The Rushbrooke scaling relation is

$$
\alpha+2\beta+\gamma=2.
$$

It follows from the homogeneous scaling form of the singular free energy.

### Hyperscaling relation

↑ **Parent:** [Scaling relation for critical exponents](#scaling-relation-for-critical-exponents)

When the singular free energy in one correlation volume is of order one, $\alpha=2-d\nu$. Hyperscaling can fail above the upper critical dimension because of a dangerously irrelevant coupling.

## Goldstone boson

↑ **Parent:** [Critical phenomenon](critical-phenomenon.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Goldstone_boson)

Each broken continuous internal-symmetry generator normally produces a massless Goldstone mode; for a symmetry breaking pattern $G\to H$, their number is $\dim G-\dim H$ in the standard relativistic setting.

### Type-B Goldstone boson

↑ **Parent:** [Goldstone boson](#goldstone-boson)

A gapless mode associated with a canonically paired pair of broken symmetry generators. In an isotropic ferromagnet, the nonzero expectation of $[S^x,S^y]=iS^z$ makes two transverse coordinates one dynamical pair, giving one quadratic magnon branch. Broken-generator counting without this pairing would incorrectly predict two independent modes. This contrasts with the linear phase mode of a [superfluid](statistical-physics.md#superfluid).

### Goldstone-mode effective free energy

↑ **Parent:** [Goldstone boson](#goldstone-boson)

For a broken $O(2)$ symmetry with order-parameter magnitude $v$, the long-wavelength phase field has free energy

$$
F_\theta=\frac{\rho_s}{2}\int d^dx\,(\nabla\theta)^2,
$$

where $\rho_s$ is the stiffness, equal to $\gamma v^2$ in the simplest Landau-Ginzburg model.

#### Phase stiffness

↑ **Parent:** [Goldstone-mode effective free energy](#goldstone-mode-effective-free-energy)

The phase stiffness is the coefficient of $\tfrac12\int d^dx\,(\nabla\theta)^2$ in the long-distance [free energy](thermodynamic-potential.md#thermodynamic-free-energy). Its renormalized value determines the [thermal phase fluctuations](statistical-physics.md#thermal-phase-fluctuation) and algebraic [correlation function](#correlation-function) of a two-dimensional [O(N) model](#o-n-model) with $N=2$.

Operationally impose a small phase difference $\phi$ between opposite sides of a square sample of side $L$. The smooth minimum has $\theta=\phi x/L$, so the two-dimensional excess [free energy](thermodynamic-potential.md#thermodynamic-free-energy) is

$$
F(\phi)-F(0)=\tfrac12\rho_s\phi^2+o(\phi^2),
\qquad \rho_s=\left.\frac{\partial^2F}{\partial\phi^2}\right|_{\phi=0}.
$$

The derivative concerns a prescribed twist at the stated observation scale; in $d$ dimensions its conventional size factor is $L^{d-2}$. This response definition includes thermal fluctuations and [vortices](#phase-vortex) after equilibration, whereas a microscopic gradient coefficient need not. A finite [phase stiffness](#phase-stiffness) requires no nonzero spatially uniform [order parameter](#order-parameter); the [Berezinskii–Kosterlitz–Thouless transition](#berezinskii-kosterlitz-thouless-transition) is the instructive example.

#### Phase-difference variance

↑ **Parent:** [Goldstone-mode effective free energy](#goldstone-mode-effective-free-energy)

For a Gaussian phase field of stiffness $\rho_s$,

$$
\langle[\theta(x)-\theta(0)]^2\rangle
=\frac2{\rho_s}\int\frac{d^dk}{(2\pi)^d}\frac{1-\cos(k\cdot x)}{k^2}.
$$

Its infrared divergence rules out conventional long-range order in dimensions at or below two.

##### Infrared-regulated phase covariance

↑ **Parent:** [Phase-difference variance](#phase-difference-variance)

Fix the uniform [order-parameter phase](#order-parameter-phase) and retain finite system size $L$ before evaluating a massless [Gaussian functional integral](quantum-field-theory.md#gaussian-functional-integral). In $d\le2$, its coincident and separated [order-parameter phase](#order-parameter-phase) [covariances](variance.md#covariance) each acquire a divergent additive constant as $L\to\infty$. Their difference $2[G_L(0)-G_L(r)]$ instead has a finite fixed-separation limit for $d>0$. This is why physical [XY model](statistical-physics.md#xy-model) [correlations](variance.md#pearson-correlation-coefficient) are obtained from [Gaussian phase averaging](partial-differential-equation.md#gaussian-phase-averaging) of angle differences. An [ultraviolet cutoff](quantum-field-theory.md#ultraviolet-cutoff) also remains necessary for coincident-point quantities; infrared cancellation does not remove it. The logarithmic two-dimensional [Green function](green-s-function.md) follows from the $d\to2$ power-law expression only after subtracting its constant pole.

##### Infrared spin-wave correlations of the XY model

↑ **Parent:** [Phase-difference variance](#phase-difference-variance)

For the [Gaussian functional integral](quantum-field-theory.md#gaussian-functional-integral) with dimensionless [phase stiffness](#phase-stiffness) $K$ and a microscopic cutoff $a$, the [Gaussian phase averaging](partial-differential-equation.md#gaussian-phase-averaging) identity gives the displayed [correlation function](#correlation-function). In two dimensions the [phase-difference variance](#phase-difference-variance) is $(\pi K)^{-1}\log(r/a)+O(1)$, so the [XY model](statistical-physics.md#xy-model) has algebraic [spin wave](#spin-wave) correlations with exponent $1/(2\pi K)$. In one dimension the variance is $r/K$, giving exponential decay. Above two dimensions the variance has a finite large-distance limit within the low-temperature [spin wave](#spin-wave) approximation. The [Laplacian](multivariable-calculus.md#laplacian) Green function solves $-K\nabla^2G=\delta$; integration over a sphere fixes $G(r)=r^{2-d}/[(d-2)S_dK]+C$ for $d\ne2$ and $G(r)=-(2\pi K)^{-1}\log(r/a)+C$ for $d=2$. A fixed uniform phase and ultraviolet regularization are required to define $G$ itself; phase differences eliminate the constant.

#### Spin wave

↑ **Parent:** [Goldstone-mode effective free energy](#goldstone-mode-effective-free-energy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spin_wave)

A spin wave is a smooth long-wavelength fluctuation of the orientation of an ordered continuous-symmetry field. In an $O(2)$ phase it is a fluctuation of the angle $\theta$ governed at leading order by the Gaussian gradient energy.

##### Magnon

↑ **Parent:** [Spin wave](#spin-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Magnon)

A [magnon](#magnon) is a quantum of a [spin wave](#spin-wave).

###### Triplon

↑ **Parent:** [Magnon](#magnon)

A mobile spin-triplet excitation above a singlet background in a quantum magnet. At low [density](fluid-mechanics.md#density), an appropriate triplet branch can be described as bosonic quasiparticles with an [effective mass](bloch-s-theorem.md#band-effective-mass) and repulsive interaction. Applied [magnetic field](magnetic-field.md) can lower one branch toward condensation. The term does not imply that the total excitation number is conserved on thermodynamic timescales.

##### Linear spin-wave approximation

↑ **Parent:** [Spin wave](#spin-wave)

The [linear spin-wave approximation](#linear-spin-wave-approximation) expands a [Holstein–Primakoff transformation](angular-momentum-operator.md#holstein-primakoff-transformation) about a classical ordered state and retains the quadratic oscillator [Hamiltonian](hamiltonian-mechanics.md#hamiltonian). It gives the leading order-$S$ excitation energies above the order-$S^2$ classical energy. In a [Heisenberg antiferromagnet](angular-momentum-operator.md#heisenberg-antiferromagnet), first make a [bipartite spin rotation](angular-momentum-operator.md#bipartite-spin-rotation). The approximation also predicts a zero-point reduction of the order parameter; infrared-divergent [quantum depletion of Néel order](statistical-physics.md#quantum-depletion-of-neel-order) signals that the assumed ordered state is not a valid thermodynamic starting point.

###### Isotropic spin-wave vacuum energy comparison

↑ **Parent:** [Linear spin-wave approximation](#linear-spin-wave-approximation)

The polarized [ground state](quantum-mechanics.md#ground-state) of an isotropic [Heisenberg model](angular-momentum-operator.md#heisenberg-model) with ferromagnetic exchange is an exact state. Its normal-ordered harmonic [Hamiltonian](hamiltonian-mechanics.md#hamiltonian) has no pair-creation terms, no vacuum magnon occupation and no additional zero-point shift. An antiferromagnetic [Néel state](statistical-physics.md#neel-state) instead generates anomalous terms, a squeezed [Bogoliubov transformation](quantum-field-theory.md#bogoliubov-transformation) vacuum, a negative energy correction and reduced staggered magnetization. Neither statement licenses omitting normal-ordering constants from an arbitrary spin-wave model with anisotropy or a different reference state.

###### Full-zone antiferromagnetic Nambu counting

↑ **Parent:** [Linear spin-wave approximation](#linear-spin-wave-approximation)

For a rotated nearest-neighbour chain, a full-zone sum of $JS(a_k^\dagger,a_{-k})M_k(a_k,a_{-k}^\dagger)^T$ contains a normal-ordering constant $JSN$. Rewriting the classical constant as $-JNS(S+1)$ compensates it. One must not additionally halve the sum without changing mode counting.

###### Heisenberg-chain spin-wave comparison

↑ **Parent:** [Linear spin-wave approximation](#linear-spin-wave-approximation)

With unit lattice spacing and $\hbar=1$, a nearest-neighbour [Heisenberg model](angular-momentum-operator.md#heisenberg-model) has quadratic low-momentum [ferromagnetic magnons](statistical-physics.md#ferromagnetic-magnon) and linear antiferromagnetic modes in the [linear spin-wave approximation](#linear-spin-wave-approximation). The ferromagnetic polarized vacuum is an exact [ground state](quantum-mechanics.md#ground-state), whereas the assumed antiferromagnetic ordered vacuum has [quantum depletion of Néel order](statistical-physics.md#quantum-depletion-of-neel-order). In one dimension its logarithmic [infrared divergence](quantum-field-theory.md#infrared-divergence) invalidates finite ordered [magnetization](electromagnetism.md#magnetization) and prevents the linear approximation from deciding the exact gap.

###### Easy-plane XXZ antiferromagnetic spin-wave spectrum

↑ **Parent:** [Linear spin-wave approximation](#linear-spin-wave-approximation)

For $0<\Delta<1$, choose a planar Néel reference and rotate local axes to align its longitudinal [spins](angular-momentum-operator.md#spin). One phase convention gives the displayed full-zone spectrum, linear near $k=0$ with slope $JS\sqrt{2(1+\Delta)}$, and gapped at $k=\pi$ by $2JS\sqrt{2(1-\Delta)}$. Shifting a sublattice phase can interchange the [momentum](momentum.md) locations. Folding the magnetic zone separates the gapless in-plane mode from the gapped out-of-plane polarization. An easy-axis reference in this regime is unstable and does not supply this physical expansion.

###### Easy-axis XXZ antiferromagnetic spin-wave spectrum

↑ **Parent:** [Linear spin-wave approximation](#linear-spin-wave-approximation)

After a [bipartite spin rotation](angular-momentum-operator.md#bipartite-spin-rotation), a leading [Holstein–Primakoff transformation](angular-momentum-operator.md#holstein-primakoff-transformation) expansion gives $H_2=-J\Delta NS^2+JS\sum_k[2\Delta n_k+\cos k(a_ka_{-k}+a_k^\dagger a_{-k}^\dagger)]$. The [bosonic Bogoliubov diagonalization](quantum-field-theory.md#bosonic-bogoliubov-diagonalization) gives the displayed spectrum and [vacuum energy](perturbative-quantum-field-theory.md#vacuum-energy) $-J\Delta NS^2+JS\sum_k[\sqrt{\Delta^2-\cos^2k}-\Delta]$. The anisotropy gap is $2JS\sqrt{\Delta^2-1}$. At $\Delta=1$ the finite-angle transformation is singular at its [zero modes](linear-operator-theory.md#zero-mode), and [quantum depletion of Néel order](statistical-physics.md#quantum-depletion-of-neel-order) is infrared divergent in one dimension.

### Mermin-Wagner theorem

↑ **Parent:** [Goldstone boson](#goldstone-boson)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mermin–Wagner_theorem)

The Mermin-Wagner theorem forbids spontaneous breaking of a continuous internal symmetry at positive temperature in one- and two-dimensional systems with sufficiently short-range interactions.

## ↑ Ancestors (4)

1. [Statistical physics](statistical-physics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (5)

- [Nobel Prize in Physics in 1982](nobel-prize-in-physics.md#nobel-prize-in-physics-in-1982)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2022.md#section-b/4/f/solution)
- [Renormalization group](#renormalization-group)
- [Surface correction to thermodynamic free energy](statistical-physics.md#surface-correction-to-thermodynamic-free-energy)
- [Wilson-Fisher fixed point](#wilson-fisher-fixed-point)
