# Mathematical biology

↑ **Parent:** [Branches of physics](physics.md#branches-of-physics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mathematical_biology)

**Table of contents**

- [FitzHugh-Nagumo model](#fitzhugh-nagumo-model)
- [Epidemic](#epidemic)
- [Metapopulation](#metapopulation)
  - [Globally coupled underdominant metapopulation](#globally-coupled-underdominant-metapopulation)
    - [Symmetric underdominant two-cluster equilibrium](#symmetric-underdominant-two-cluster-equilibrium)
    - [Invariant-rectangle criterion for underdominant coexistence](#invariant-rectangle-criterion-for-underdominant-coexistence)
  - [Levins metapopulation model](#levins-metapopulation-model)
    - [Colonization-competition tradeoff invasion fitness](#colonization-competition-tradeoff-invasion-fitness)
- [Allee effect](#allee-effect)
- [Food web](#food-web)
  - [Competitive exclusion principle](#competitive-exclusion-principle)
  - [Food chain](#food-chain)
    - [Lotka-Volterra food-chain parity](#lotka-volterra-food-chain-parity)
- [Gene regulatory network](#gene-regulatory-network)
  - [Mutual repression](#mutual-repression)
    - [Common-strength Hill repression criterion](#common-strength-hill-repression-criterion)
    - [Equal-strength power-law mutual repression](#equal-strength-power-law-mutual-repression)
    - [Mutual repression stability criterion](#mutual-repression-stability-criterion)
- [Monod equation](#monod-equation)
- [Chemostat](#chemostat)
  - [Monod chemostat equilibrium and relaxation](#monod-chemostat-equilibrium-and-relaxation)
  - [Dilution rate](#dilution-rate)
- [Two-season seed-bank recurrence](#two-season-seed-bank-recurrence)
- [Population dynamics](#population-dynamics)
  - [Carrying capacity](#carrying-capacity)
  - [Nicholson-Bailey model](#nicholson-bailey-model)
    - [Instability of the Nicholson-Bailey equilibrium](#instability-of-the-nicholson-bailey-equilibrium)
  - [Symmetric competition model](#symmetric-competition-model)
  - [Logistic growth equation](#logistic-growth-equation)
    - [Constant-quota harvested logistic growth](#constant-quota-harvested-logistic-growth)
- [Ricker population map](#ricker-population-map)
- [Squared-denominator population map](#squared-denominator-population-map)
  - [Post-initial invariant interval for a squared-denominator population map](#post-initial-invariant-interval-for-a-squared-denominator-population-map)
- [Distinction between linear resonance and nonlinear periodic bifurcation](#distinction-between-linear-resonance-and-nonlinear-periodic-bifurcation)
- [Age-structured population equation](#age-structured-population-equation)
  - [Net reproduction rate](#net-reproduction-rate)
- [Moran process](#moran-process)
- [Demographic stochasticity](#demographic-stochasticity)
- [Mathematical epidemiology](#mathematical-epidemiology)
  - [Contact reciprocity in a two-group epidemic](#contact-reciprocity-in-a-two-group-epidemic)
  - [Macroparasite burden model](#macroparasite-burden-model)
    - [Mating-limited macroparasite transmission](#mating-limited-macroparasite-transmission)
    - [Aggregation of macroparasite burdens](#aggregation-of-macroparasite-burdens)
    - [Immigration-death worm-burden model](#immigration-death-worm-burden-model)
  - [Stochastic epidemic model](#stochastic-epidemic-model)
  - [Recovery rate](#recovery-rate)
  - [Quarantine](#quarantine)
  - [Incubation period](#incubation-period)
  - [Back-calculation of infection incidence](#back-calculation-of-infection-incidence)
    - [Discrete back-calculation with endpoint cohorts](#discrete-back-calculation-with-endpoint-cohorts)
  - [Calendar time](#calendar-time)
  - [Incidence (epidemiology)](#incidence-epidemiology)
  - [Infection age](#infection-age)
  - [Imported infection](#imported-infection)
  - [Infectivity profile](#infectivity-profile)
    - [Generation interval](#generation-interval)
      - [Generation-interval distribution](#generation-interval-distribution)
        - [Infectious disease renewal equation](#infectious-disease-renewal-equation)
          - [Total infectiousness](#total-infectiousness)
          - [Time-varying reproduction number](#time-varying-reproduction-number)
            - [Instantaneous reproduction number](#instantaneous-reproduction-number)
            - [Case reproduction number](#case-reproduction-number)
- [Per capita](#per-capita)
- [Lotka-Volterra predator-prey model](#lotka-volterra-predator-prey-model)
  - [Annual pulse-breeding predator-prey model](#annual-pulse-breeding-predator-prey-model)
    - [Area-preserving seasonal predator-prey map](#area-preserving-seasonal-predator-prey-map)
  - [Fixed-quota harvesting of Lotka-Volterra populations](#fixed-quota-harvesting-of-lotka-volterra-populations)
    - [Event-triggered harvesting by conserved energy](#event-triggered-harvesting-by-conserved-energy)
  - [Logistic predator-prey model](#logistic-predator-prey-model)
    - [Quadratic discrete predator-prey map](#quadratic-discrete-predator-prey-map)
- [Age-structured population model](#age-structured-population-model)
  - [Von Foerster equation](#von-foerster-equation)
  - [Seed-bank population recurrence](#seed-bank-population-recurrence)
  - [Euler-Lotka equation](#euler-lotka-equation)
    - [Discrete Euler-Lotka equation](#discrete-euler-lotka-equation)
- [Law of mass action](#law-of-mass-action)
- [Chemical reaction network](#chemical-reaction-network)
  - [Mean-field joint removal of two chemical species](#mean-field-joint-removal-of-two-chemical-species)
    - [Exclusive joint removal has a diffusing difference mode](#exclusive-joint-removal-has-a-diffusing-difference-mode)
    - [Linear noise of two species with joint removal](#linear-noise-of-two-species-with-joint-removal)
  - [Chemical species](#chemical-species)
    - [Mole fraction](#mole-fraction)
    - [Volume mixing ratio](#volume-mixing-ratio)
  - [Stoichiometric vector](#stoichiometric-vector)
  - [Rate equation](#rate-equation)
    - [Reaction-rate elasticity](#reaction-rate-elasticity)
  - [Stochastic chemical kinetics](#stochastic-chemical-kinetics)
    - [Molecular-flux-weighted reaction event size](#molecular-flux-weighted-reaction-event-size)
    - [Mean molecular lifetime](#mean-molecular-lifetime)
    - [Compartment-based stochastic diffusion](#compartment-based-stochastic-diffusion)
      - [Asymmetric simple exclusion process](#asymmetric-simple-exclusion-process)
    - [Immigration--death process](#immigration-death-process)
      - [Pair immigration with linear deaths](#pair-immigration-with-linear-deaths)
    - [Stochastic quasi-steady-state approximation](#stochastic-quasi-steady-state-approximation)
      - [Slow-scale stochastic simulation algorithm](#slow-scale-stochastic-simulation-algorithm)
    - [Molecular copy number](#molecular-copy-number)
    - [Reaction propensity function](#reaction-propensity-function)
      - [Power-law reaction propensity](#power-law-reaction-propensity)
    - [Chemical master equation](#chemical-master-equation)
    - [Gillespie algorithm](#gillespie-algorithm)
    - [Moment hierarchy](#moment-hierarchy)
      - [Moment equation](#moment-equation)
      - [Moment closure](#moment-closure)
        - [Central-moment closure](#central-moment-closure)
- [Enzyme kinetics](#enzyme-kinetics)
  - [Sequential two-site enzyme reaction network](#sequential-two-site-enzyme-reaction-network)
  - [Michaelis-Menten kinetics](#michaelis-menten-kinetics)
    - [Michaelis-Menten equation](#michaelis-menten-equation)
  - [Quasi-steady-state approximation](#quasi-steady-state-approximation)
    - [Quasi-steady rate law for a two-substrate allosteric enzyme](#quasi-steady-rate-law-for-a-two-substrate-allosteric-enzyme)
- [Autocatalysis](#autocatalysis)
  - [Autocatalytic biochemical switch](#autocatalytic-biochemical-switch)
    - [Saturating autocatalytic switch](#saturating-autocatalytic-switch)
      - [Strong-autocatalysis switching threshold](#strong-autocatalysis-switching-threshold)
- [Cubic saturation population model](#cubic-saturation-population-model)
- [Exponential density-dependent birth model](#exponential-density-dependent-birth-model)
- [Survival-augmented Ricker map](#survival-augmented-ricker-map)
  - [Nonlinear stability at the Ricker flip threshold](#nonlinear-stability-at-the-ricker-flip-threshold)
  - [Stability interval of the survival-augmented Ricker equilibrium](#stability-interval-of-the-survival-augmented-ricker-equilibrium)
- [Malthusian delay differential equation](#malthusian-delay-differential-equation)
  - [Method of steps for a delay differential equation](#method-of-steps-for-a-delay-differential-equation)
  - [Characteristic equation of a delay differential equation](#characteristic-equation-of-a-delay-differential-equation)
    - [Periodic solution of a scalar delay equation](#periodic-solution-of-a-scalar-delay-equation)
    - [Stability threshold for delayed quadratic crowding](#stability-threshold-for-delayed-quadratic-crowding)
    - [Delay-independent stability from an undelayed linearization](#delay-independent-stability-from-an-undelayed-linearization)
- [Epidemic threshold](#epidemic-threshold)
  - [Vertical transmission](#vertical-transmission)
  - [Horizontal transmission](#horizontal-transmission)
- [Kramers-Moyal expansion](#kramers-moyal-expansion)
  - [Constant-birth pair-annihilation process](#constant-birth-pair-annihilation-process)
  - [Kramers-Moyal master equation](#kramers-moyal-master-equation)
- [Compartmental models (epidemiology)](#compartmental-models-epidemiology)
  - [SIS model](#sis-model)
    - [Assortatively mixed two-risk-group SIS model](#assortatively-mixed-two-risk-group-sis-model)
      - [Small-core SIS endemic expansion](#small-core-sis-endemic-expansion)
    - [Homogeneous SIS susceptible fraction](#homogeneous-sis-susceptible-fraction)
    - [Cooperative SIS coinfection threshold](#cooperative-sis-coinfection-threshold)
  - [Conservation of population](#conservation-of-population)
  - [Prevalence](#prevalence)
  - [SI model](#si-model)
    - [Uniform almost-sure fluid limit of the SI model](#uniform-almost-sure-fluid-limit-of-the-si-model)
    - [Logistic solution of the SI model](#logistic-solution-of-the-si-model)
    - [Plant SI model with logistic total population](#plant-si-model-with-logistic-total-population)
      - [Uniform per-capita culling in the plant SI model](#uniform-per-capita-culling-in-the-plant-si-model)
  - [SEIR model](#seir-model)
    - [Force of infection](#force-of-infection)
    - [Final size relation for an epidemic](#final-size-relation-for-an-epidemic)
  - [SIR model](#sir-model)
    - [Farm-size stratified SIR model](#farm-size-stratified-sir-model)
    - [Discrete SIR epidemic on a graph](#discrete-sir-epidemic-on-a-graph)
      - [Adjacency-matrix bound for a discrete SIR epidemic](#adjacency-matrix-bound-for-a-discrete-sir-epidemic)
        - [Resolvent bound for a discrete SIR epidemic](#resolvent-bound-for-a-discrete-sir-epidemic)
          - [Spectral condition for a small discrete SIR outbreak](#spectral-condition-for-a-small-discrete-sir-outbreak)
    - [Epidemic threshold for the closed SIR model](#epidemic-threshold-for-the-closed-sir-model)
    - [SIR susceptible-recovered identity](#sir-susceptible-recovered-identity)
    - [Stochastic SIR model](#stochastic-sir-model)
      - [Two-event probability in a stochastic SIR model](#two-event-probability-in-a-stochastic-sir-model)
      - [Chain-binomial epidemic model](#chain-binomial-epidemic-model)
  - [Mass-action interaction](#mass-action-interaction)
  - [Spatial SIR model](#spatial-sir-model)
    - [Mass-action infection](#mass-action-infection)
    - [Diffusion of infectives](#diffusion-of-infectives)
  - [Disease-free equilibrium](#disease-free-equilibrium)
  - [Endemic equilibrium](#endemic-equilibrium)
  - [Susceptible-infective model with exponential density-dependent birth](#susceptible-infective-model-with-exponential-density-dependent-birth)
    - [Disease-free equilibrium of the susceptible-infective model with exponential birth](#disease-free-equilibrium-of-the-susceptible-infective-model-with-exponential-birth)
    - [Endemic equilibrium of the susceptible-infective model with exponential birth](#endemic-equilibrium-of-the-susceptible-infective-model-with-exponential-birth)
  - [Basic reproduction number](#basic-reproduction-number)
    - [Next-generation matrix](#next-generation-matrix)
      - [Susceptible-weighted next-generation matrix](#susceptible-weighted-next-generation-matrix)
    - [Epidemic invasion threshold](#epidemic-invasion-threshold)
  - [SIR model with demography and permanent immunity](#sir-model-with-demography-and-permanent-immunity)
    - [Endemic equilibrium of the SIR model with demography](#endemic-equilibrium-of-the-sir-model-with-demography)
  - [SIR model with waning immunity](#sir-model-with-waning-immunity)
    - [SIRS Markov chain](#sirs-markov-chain)
      - [Fluid limit of the SIRS Markov chain](#fluid-limit-of-the-sirs-markov-chain)
    - [Endemic equilibrium of the SIR model with waning immunity](#endemic-equilibrium-of-the-sir-model-with-waning-immunity)
- [Dispersal with mortality and immobile deposition](#dispersal-with-mortality-and-immobile-deposition)
  - [Remnant density from diffusion with mortality and deposition](#remnant-density-from-diffusion-with-mortality-and-deposition)
  - [Diffusion length](#diffusion-length)
- [Biological fluid dynamics](#biological-fluid-dynamics)
  - [Phototaxis](#phototaxis)
    - [Phototactic concentration in a vertical channel](#phototactic-concentration-in-a-vertical-channel)
      - [Zero-flux pressure gradient in a cell-driven channel](#zero-flux-pressure-gradient-in-a-cell-driven-channel)
    - [Phototactic orientation Fokker-Planck equation](#phototactic-orientation-fokker-planck-equation)
      - [Small-vorticity phototactic orientation response](#small-vorticity-phototactic-orientation-response)
  - [Bioconvection](#bioconvection)
    - [Long-wave bioconvection threshold in weak stratification](#long-wave-bioconvection-threshold-in-weak-stratification)
      - [Clamped-quartic solvability in shallow bioconvection](#clamped-quartic-solvability-in-shallow-bioconvection)
  - [Cell conservation in a swimming suspension](#cell-conservation-in-a-swimming-suspension)
    - [Closed-channel cell-flux constraint](#closed-channel-cell-flux-constraint)
  - [Gyrotaxis](#gyrotaxis)
    - [Gyrotactic focusing in a downward pipe flow](#gyrotactic-focusing-in-a-downward-pipe-flow)
      - [Stresslet correction to gyrotactic pipe flow](#stresslet-correction-to-gyrotactic-pipe-flow)
    - [Gyrotactic circular paths in a rotating cylinder](#gyrotactic-circular-paths-in-a-rotating-cylinder)
    - [Gyrotactic orientation Fokker-Planck equation](#gyrotactic-orientation-fokker-planck-equation)
      - [Zero-flow steady gyrotactic orientation distribution](#zero-flow-steady-gyrotactic-orientation-distribution)
      - [Rapid-rotation mean gyrotactic orientation](#rapid-rotation-mean-gyrotactic-orientation)
        - [Gyrotactic concentration layer at a rotating-cylinder wall](#gyrotactic-concentration-layer-at-a-rotating-cylinder-wall)
    - [Bottom-heavy spherical-cell orientation dynamics](#bottom-heavy-spherical-cell-orientation-dynamics)
      - [Quasistatic gyrotactic balance with half-rate reorientation](#quasistatic-gyrotactic-balance-with-half-rate-reorientation)
      - [Deterministic alignment of an initially isotropic orientation distribution](#deterministic-alignment-of-an-initially-isotropic-orientation-distribution)
      - [Gyrotactic reorientation time](#gyrotactic-reorientation-time)
        - [Weak-noise relaxation of gyrotactic alignment](#weak-noise-relaxation-of-gyrotactic-alignment)
  - [Lighthill elongated-body theory](#lighthill-elongated-body-theory)
    - [Active bending beam for a swimming fish](#active-bending-beam-for-a-swimming-fish)
    - [Recoil correction in elongated-body theory](#recoil-correction-in-elongated-body-theory)
      - [Quadratic-bend turning with finite body mass](#quadratic-bend-turning-with-finite-body-mass)
      - [Endpoint momentum flux in elongated-body recoil](#endpoint-momentum-flux-in-elongated-body-recoil)
      - [Free-end compatibility for a swimming beam](#free-end-compatibility-for-a-swimming-beam)
  - [Volvox](#volvox)
    - [Hydrodynamic attraction of hovering Volvox colonies](#hydrodynamic-attraction-of-hovering-volvox-colonies)
  - [Microcirculation](#microcirculation)
    - [Murray's law](#murray-s-law)
    - [Fahraeus--Lindqvist effect](#fahraeus-lindqvist-effect)
      - [Cell-free layer](#cell-free-layer)
    - [Zweifach--Fung effect](#zweifach-fung-effect)
  - [Cytoplasmic streaming](#cytoplasmic-streaming)
  - [Resistive-force theory](#resistive-force-theory)
    - [Shear-dependent settling of a sphere-and-tail body](#shear-dependent-settling-of-a-sphere-and-tail-body)
    - [Linear resistive-force propulsion of a travelling filament](#linear-resistive-force-propulsion-of-a-travelling-filament)
      - [Fixed-speed energy optimum for a planar flagellum](#fixed-speed-energy-optimum-for-a-planar-flagellum)
    - [Nonlinear resistive-force balance for a travelling filament](#nonlinear-resistive-force-balance-for-a-travelling-filament)
    - [Basal bending moment of a planar flagellum](#basal-bending-moment-of-a-planar-flagellum)
    - [Head-drag correction to planar flagellar propulsion](#head-drag-correction-to-planar-flagellar-propulsion)
    - [Finite-amplitude propulsion of an inextensible periodic filament](#finite-amplitude-propulsion-of-an-inextensible-periodic-filament)
      - [Cross-resistance of an asymmetric planar waveform](#cross-resistance-of-an-asymmetric-planar-waveform)
    - [Oscillating rigid rod in resistive-force theory](#oscillating-rigid-rod-in-resistive-force-theory)
      - [Power of a rocking rod](#power-of-a-rocking-rod)
      - [Mean transverse force from a rocking rod](#mean-transverse-force-from-a-rocking-rod)
    - [Power of a periodic planar filament](#power-of-a-periodic-planar-filament)
    - [Propulsive force of a periodic planar filament](#propulsive-force-of-a-periodic-planar-filament)
      - [Travelling-wave stationarity of planar filament propulsion](#travelling-wave-stationarity-of-planar-filament-propulsion)
        - [Bandwidth limitation in fixed-power filament optimization](#bandwidth-limitation-in-fixed-power-filament-optimization)
    - [First-order free swimming of a planar filament](#first-order-free-swimming-of-a-planar-filament)
      - [First-order periodic transverse swimming velocity](#first-order-periodic-transverse-swimming-velocity)
      - [Least-squares projection of filament deformation velocity](#least-squares-projection-of-filament-deformation-velocity)
    - [Rigid-body velocity in a deforming swimmer frame](#rigid-body-velocity-in-a-deforming-swimmer-frame)
    - [Parallel and perpendicular drag coefficients of a slender filament](#parallel-and-perpendicular-drag-coefficients-of-a-slender-filament)
      - [Anisotropic slender-filament drag from Stokeslet integration](#anisotropic-slender-filament-drag-from-stokeslet-integration)
    - [Sperm number](#sperm-number)
      - [Elastohydrodynamic penetration length](#elastohydrodynamic-penetration-length)
      - [Elastohydrodynamic boundary layer of a filament](#elastohydrodynamic-boundary-layer-of-a-filament)
- [Chemotaxis](#chemotaxis)
  - [Chemotactic instability with a wavenumber cutoff](#chemotactic-instability-with-a-wavenumber-cutoff)
  - [Keller--Segel model](#keller-segel-model)
    - [Keller--Segel aggregation threshold](#keller-segel-aggregation-threshold)
      - [Fastest-growing Keller--Segel mode](#fastest-growing-keller-segel-mode)
    - [Logarithmic chemotactic sensitivity](#logarithmic-chemotactic-sensitivity)
      - [Nutrient-consuming chemotactic travelling band](#nutrient-consuming-chemotactic-travelling-band)
        - [Speed of a nutrient-consuming chemotactic band](#speed-of-a-nutrient-consuming-chemotactic-band)
  - [Chemotactic pattern-forming instability](#chemotactic-pattern-forming-instability)
  - [Chemotactic telegraph equation](#chemotactic-telegraph-equation)
- [Biopolymer mechanics](#biopolymer-mechanics)
  - [Hydrodynamic drag models for a polymer](#hydrodynamic-drag-models-for-a-polymer)
  - [Polymerization Brownian ratchet](#polymerization-brownian-ratchet)
    - [Reaction-limited polymerization Brownian ratchet](#reaction-limited-polymerization-brownian-ratchet)
    - [Diffusion-limited Brownian ratchet with constant load](#diffusion-limited-brownian-ratchet-with-constant-load)
  - [Bending and torsion of filament bundles](#bending-and-torsion-of-filament-bundles)
  - [Adhesive-cell rolling threshold](#adhesive-cell-rolling-threshold)
  - [de Gennes confinement scaling](#de-gennes-confinement-scaling)
    - [Polymer coil in slit confinement](#polymer-coil-in-slit-confinement)
  - [Gaussian chain](#gaussian-chain)
    - [Debye scattering function for a Gaussian chain](#debye-scattering-function-for-a-gaussian-chain)
  - [Ideal chain](#ideal-chain)
    - [Three-dimensional entropic chain stiffness](#three-dimensional-entropic-chain-stiffness)
    - [Gaussian limit of the end-to-end distribution of a freely jointed chain](#gaussian-limit-of-the-end-to-end-distribution-of-a-freely-jointed-chain)
    - [Planar freely jointed chain](#planar-freely-jointed-chain)
    - [Force-extension of a three-dimensional freely jointed chain](#force-extension-of-a-three-dimensional-freely-jointed-chain)
    - [Langevin function](#langevin-function)
  - [Inextensible filament](#inextensible-filament)
    - [Axial and arclength travelling-wave speeds](#axial-and-arclength-travelling-wave-speeds)
    - [Quadratic longitudinal displacement of an inextensible planar filament](#quadratic-longitudinal-displacement-of-an-inextensible-planar-filament)
    - [Filament bending modulus](#filament-bending-modulus)
    - [Filament tension](#filament-tension)
  - [Monge representation](#monge-representation)
  - [Stokesian dynamics of an elastic filament](#stokesian-dynamics-of-an-elastic-filament)
    - [Overdamped relaxation of a free filament](#overdamped-relaxation-of-a-free-filament)
    - [Small-slope elastohydrodynamic filament equation](#small-slope-elastohydrodynamic-filament-equation)
      - [Uniform-load bending of a clamped filament](#uniform-load-bending-of-a-clamped-filament)
        - [Tip stiffness of a uniformly loaded cantilever](#tip-stiffness-of-a-uniformly-loaded-cantilever)
      - [Boundary expression for transverse filament thrust](#boundary-expression-for-transverse-filament-thrust)
      - [Oscillatory bending of a moment-free semi-infinite filament](#oscillatory-bending-of-a-moment-free-semi-infinite-filament)
  - [Microtubule](#microtubule)
  - [Thermal bending fluctuations of a clamped filament](#thermal-bending-fluctuations-of-a-clamped-filament)
    - [Clamped--free bending mode](#clamped-free-bending-mode)
      - [Fourth inverse-power sum of the cantilever spectrum](#fourth-inverse-power-sum-of-the-cantilever-spectrum)
      - [Constrained variational characterization of bending modes](#constrained-variational-characterization-of-bending-modes)
      - [Overdamped relaxation of a clamped--free filament](#overdamped-relaxation-of-a-clamped-free-filament)
    - [Free--free biharmonic eigenvalue equation](#free-free-biharmonic-eigenvalue-equation)
  - [Follower force on a filament](#follower-force-on-a-filament)
    - [Two-link follower-force filament model](#two-link-follower-force-filament-model)
      - [Dimensionless follower load](#dimensionless-follower-load)
  - [Worm-like chain](#worm-like-chain)
    - [Kuhn length](#kuhn-length)
    - [High-force worm-like chain elasticity](#high-force-worm-like-chain-elasticity)
      - [Transverse tangent correlation of a stretched worm-like chain](#transverse-tangent-correlation-of-a-stretched-worm-like-chain)
        - [Periodic finite-length tangent correlation of a stretched worm-like chain](#periodic-finite-length-tangent-correlation-of-a-stretched-worm-like-chain)
    - [Persistence length](#persistence-length)
  - [Euler buckling of an elastic filament](#euler-buckling-of-an-elastic-filament)
    - [Polymerization-driven cantilever postbuckling](#polymerization-driven-cantilever-postbuckling)
    - [Thermal rounding of a buckling transition](#thermal-rounding-of-a-buckling-transition)
    - [Self-buckling of a vertical rod](#self-buckling-of-a-vertical-rod)
      - [Bessel threshold for self-buckling of a vertical rod](#bessel-threshold-for-self-buckling-of-a-vertical-rod)
- [Lipid bilayer](#lipid-bilayer)
  - [Line tension](#line-tension)
    - [Fixed-area capillary spectrum of a circular boundary](#fixed-area-capillary-spectrum-of-a-circular-boundary)
      - [Translation mode of a circular boundary](#translation-mode-of-a-circular-boundary)
  - [Lipid vesicle](#lipid-vesicle)
    - [Fixed-volume capillary spectrum of a cylindrical membrane](#fixed-volume-capillary-spectrum-of-a-cylindrical-membrane)
    - [Axisymmetric membrane deformation](#axisymmetric-membrane-deformation)
  - [Interaction between lipid bilayers](#interaction-between-lipid-bilayers)
    - [Hamaker constant](#hamaker-constant)
    - [Debye–Hückel screening length](#debye-huckel-screening-length)
    - [Helfrich repulsion](#helfrich-repulsion)
    - [Membrane unbinding transition](#membrane-unbinding-transition)
  - [Helfrich energy](#helfrich-energy)
    - [Thermal membrane undulation](#thermal-membrane-undulation)
    - [Membrane bending modulus](#membrane-bending-modulus)
    - [Membrane tension](#membrane-tension)
    - [Membrane elastic length](#membrane-elastic-length)
    - [Small-slope elastic membrane energy](#small-slope-elastic-membrane-energy)
      - [Capillary height-difference correlation](#capillary-height-difference-correlation)
        - [Pinned capillary-wave correlation](#pinned-capillary-wave-correlation)
      - [Dimensionless adhesion strength](#dimensionless-adhesion-strength)
      - [Membrane-mediated interaction potential](#membrane-mediated-interaction-potential)
    - [Cylindrical membrane equilibrium radius](#cylindrical-membrane-equilibrium-radius)
      - [Entropic membrane-tether force--extension relation](#entropic-membrane-tether-force-extension-relation)
    - [Fluctuation-supported membrane--particle gap](#fluctuation-supported-membrane-particle-gap)
      - [Confined-sphere drag coefficient](#confined-sphere-drag-coefficient)

## FitzHugh-Nagumo model

↑ **Parent:** [Mathematical biology](mathematical-biology.md)

The [FitzHugh-Nagumo model](#fitzhugh-nagumo-model) represents an excitable cell by a fast activation variable and a slower recovery variable. A common nondimensional form is $\dot V=V-V^3/3-W+I$, $\dot W=\varepsilon(V+a-bW)$. Its cubic activation response and recovery feedback can produce an excitable resting state or sustained oscillations through [bifurcations](dynamical-systems.md#bifurcation). Particular reductions and travelling-wave equations can have additional state variables; their signs and parameter conventions must be stated separately.

## Epidemic

↑ **Parent:** [Mathematical biology](mathematical-biology.md)

An [epidemic](#epidemic) is a period of growing infection incidence in a population. [Compartmental models](#compartmental-models-epidemiology) describe transmission, recovery and depletion or renewal of susceptible hosts. An [epidemic invasion threshold](#epidemic-invasion-threshold) concerns growth after a small introduction; a [final size relation for an epidemic](#final-size-relation-for-an-epidemic) concerns the total susceptible depletion of a closed outbreak. These are distinct from an endemic [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system) with continuing transmission.

## Metapopulation

↑ **Parent:** [Mathematical biology](mathematical-biology.md)

A [metapopulation](#metapopulation) describes occupied habitat patches with local colonization and extinction. The patch occupancy variable differs from population abundance within a patch.

### Globally coupled underdominant metapopulation

↑ **Parent:** [Metapopulation](#metapopulation)

This model couples deterministic [underdominant allele-frequency dynamics](biology.md#underdominant-allele-frequency-dynamics) in equal-sized habitats by global migration. Starting with $m$ pure habitats of one [allele](biology.md#allele) and $N-m$ of the other preserves two within-class frequencies $x,y$, reducing the system to $\dot x=f(x)-\sigma(1-q)(x-y)$, $\dot y=f(y)+\sigma q(x-y)$ with $q=m/N$. Migration is conservative in the [mean](probability-theory.md#expected-value), but selection need not conserve global [allele frequency](biology.md#allele-frequency).

#### Symmetric underdominant two-cluster equilibrium

↑ **Parent:** [Globally coupled underdominant metapopulation](#globally-coupled-underdominant-metapopulation)

With equally many initially pure habitats of each [allele](biology.md#allele), symmetry preserves $y=1-x$. The heterogeneous [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system) exists for $\sigma<s/2$. Its full-system [eigenvalues](linear-operator-theory.md#eigenvalue) are $-s+3\sigma$ in the mean-frequency direction and $-s+2\sigma$ in the antisymmetric direction, so it attracts general nearby perturbations only for $\sigma<s/3$. Exact symmetry can preserve both [alleles](biology.md#allele) beyond this robust range; at stronger migration it approaches the unstable uniform midpoint.

#### Invariant-rectangle criterion for underdominant coexistence

↑ **Parent:** [Globally coupled underdominant metapopulation](#globally-coupled-underdominant-metapopulation)

In the two-class [globally coupled underdominant metapopulation](#globally-coupled-underdominant-metapopulation), the rectangle $3/4\le x\le1$, $0\le y\le1/4$ is forward invariant under the displayed bound. On its inner edges, selection points inward with magnitude $3s/32$ while outward migration is at most $(3/4)\sigma(1-q)$ or $(3/4)\sigma q$; the outer edges also point inward. Thus prescribed initial state $(1,0)$ cannot approach global [allele fixation](biology.md#allele-fixation) when $0<q<1$. Maximizing $f(u)/u=s(1-u)(2u-1)$ gives $s/8$ at $u=3/4$, making the bound optimal within this particular symmetric worst-case rectangle argument, not a universal sharp migration threshold.

### Levins metapopulation model

↑ **Parent:** [Metapopulation](#metapopulation)

Colonization of empty habitat at rate $c$ and extinction of occupied habitat at rate $m$ give the displayed patch-occupancy equation. The positive [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system) is $1-m/c$ when $c>m$. Competition can be incorporated through replacement fluxes between patches occupied by different species.

#### Colonization-competition tradeoff invasion fitness

↑ **Parent:** [Levins metapopulation model](#levins-metapopulation-model)

A resident trait $x$ occupies fraction $1-m/c(x)$ when its colonization rate exceeds fire extinction. With net competitive replacement given by ability difference $B(y)-B(x)$, a rare mutant has the displayed per-capita growth. The [selection gradient](game-theory.md#selection-gradient) is $g(x)=mc'(x)/c(x)+[1-m/c(x)]B'(x)$. A singular trait with negative mutant-fitness curvature is a strict local [evolutionarily stable strategy](game-theory.md#evolutionarily-stable-strategy). Global strict uninvadability requires that $mc(y)+[c(x)-m]B(y)$ be smaller than its resident value for every other trait. Monotonicity alone does not specify the shape or existence of an optimum.

## Allee effect

↑ **Parent:** [Mathematical biology](mathematical-biology.md)

An [Allee effect](#allee-effect) makes per-capita growth less favorable at low abundance. A strong effect permits a stable zero state and a stable positive state separated by a finite threshold. Cooperative infections can exhibit the same positive-feedback structure: neither disease invades alone, but sufficiently many joint infections sustain both.

## Food web

↑ **Parent:** [Mathematical biology](mathematical-biology.md)

A [food web](#food-web) records resource-consumer interactions among species. A linear [food chain](#food-chain) is a special case. Positive interaction coefficients alone do not imply persistence: the per-capita growth balances must admit feasible positive long-term [mean](probability-theory.md#expected-value) abundances.

### Competitive exclusion principle

↑ **Parent:** [Food web](#food-web)

Two consumers with different break-even requirements cannot both have bounded persistent abundance on a single well-mixed limiting resource when their per-capita growth is linear in that resource. For $\dot Y/Y=cX-d$ and $\dot Z/Z=eX-f$, differentiation of $\log Y/c-\log Z/e$ gives the nonzero constant $-d/c+f/e$ when their break-even levels differ. This excludes simultaneous bounded persistence without assuming convergence to an [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system). Additional resources, environmental variation or different interactions can invalidate the simple one-resource argument.

### Food chain

↑ **Parent:** [Food web](#food-web)

A [food chain](#food-chain) orders species so that each consumer feeds on the level below and may be eaten by the level above. Basal resource growth, consumer mortality, conversion efficiency and density regulation determine whether all levels can persist.

#### Lotka-Volterra food-chain parity

↑ **Parent:** [Food chain](#food-chain)

For an unregulated exponential basal resource and nearest-neighbor [Lotka-Volterra equations](dynamical-systems.md#lotka-volterra-equations), the weighted interaction matrix is [skew-symmetric matrix](linear-algebra.md#skew-symmetric-matrix). An even chain has an invertible tridiagonal interaction matrix; its positive [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system), when feasible, fixes all long-term [means](probability-theory.md#expected-value). An odd chain has a null direction and requires a special balance between resource growth and mortality to permit bounded full coexistence. For a three-level chain, $X_1^{b_2}X_3^{a_1}=C\exp[(b_2r-a_1d_3)t]$. A positive even-chain [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system) gives a conserved coercive relative-entropy-type function, proving every species remains bounded above and away from zero.

## Gene regulatory network

↑ **Parent:** [Mathematical biology](mathematical-biology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gene_regulatory_network)

A network describing how gene products affect the production of other gene products. Positive and negative regulatory interactions can generate [multistability](dynamical-systems.md#multistability), oscillations, and noise-sensitive transitions.

// Target: mathematical-biology.bigb

### Mutual repression

↑ **Parent:** [Gene regulatory network](#gene-regulatory-network)

Two components mutually repress when each inhibits the other's production. With decreasing $f,g$, the two negative interactions create a positive feedback loop. Sufficiently strong repression can produce two stable states: high $x$, low $y$, and the reverse.

// Target: mathematical-biology.bigb

#### Common-strength Hill repression criterion

↑ **Parent:** [Mutual repression](#mutual-repression)

For $\dot x=\lambda/(1+y^m)-x$, $\dot y=\lambda/(1+x^n)-y$, the equilibrium slope product is $K=mn x^ny^m/[(1+x^n)(1+y^m)]$. A value $K>1$ gives a saddle separating attracting alternatives. Both exponents greater than one allow this at sufficiently large common $\lambda$. If both are at most one it is impossible. If $0<m\le1<n$, define $Y(x)$ as the unique positive solution of $Y^{-1}+Y^{m-1}=x^{-1}+x^{n-1}$ and set $K_{m,n}(x)=mn x^nY(x)^m/[(1+x^n)(1+Y(x)^m)]$. All equilibria are parameterized by $\lambda=x(1+Y^m)$, whose [derivative](calculus.md#derivative) is $(1+Y^m)(1-K)/(1-mY^m/(1+Y^m))$. Thus multistability for some common strength occurs exactly when $\max_{x>0}K_{m,n}(x)>1$. For $m=1$ the maximum is $(n-1)^2[(n+1)/(n-1)]^{(n+1)/n}/(4n)$. Consequently $mn>1$ alone is not sufficient when the two synthesis strengths are required to coincide.

#### Equal-strength power-law mutual repression

↑ **Parent:** [Mutual repression](#mutual-repression)

For positive $m,n$, this [mutual repression](#mutual-repression) system can display [bistability](dynamical-systems.md#bistability) for some $\lambda$ exactly when both $m>1$ and $n>1$. If either exponent is at most one, it has a unique stable equilibrium for every $\lambda$. To prove the less obvious case $m\le1<n$, put $a=x/(1+x)$ and $b=y/(1+y)$ at equilibrium. Equality of the two expressions for $\lambda$ gives $a\le b(1-b)^{n-1}$. The loop gain is then bounded by $mn b^2(1-b)^{n-1}$, whose maximum is $4mn(n-1)^{n-1}/(n+1)^{n+1}<1$. Swap the two components for the other case. If both exponents exceed one, sufficiently large $\lambda$ yields two stable equilibria with $(x,y)\sim(\lambda,\lambda^{1-m})$ and $(x,y)\sim(\lambda^{1-n},\lambda)$. The weaker condition $mn\le1$ is sufficient to exclude multistability, but does not exhaust all exclusions when the same production prefactor is imposed.

// Target: mathematical-biology.bigb

#### Mutual repression stability criterion

↑ **Parent:** [Mutual repression](#mutual-repression)

At an equilibrium $x_*=f(y_*)$, $y_*=g(x_*)$, the [Jacobian matrix](calculus.md#jacobian-matrix) has eigenvalues $-1\pm\sqrt{f'(y_*)g'(x_*)}$. Its product of repression gains is also $(\partial\log f/\partial\log y)(\partial\log g/\partial\log x)$. Product below one gives a stable node, above one a saddle, and equality the threshold for a zero eigenvalue. Robust multiple stable equilibria require an intervening unstable equilibrium; a gain exceeding one alone is not a sufficient global criterion for a particular pair of repression functions.

// Target: mathematical-biology.bigb

## Monod equation

↑ **Parent:** [Mathematical biology](mathematical-biology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Monod_equation)

## Chemostat

↑ **Parent:** [Mathematical biology](mathematical-biology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chemostat)

A chemostat maintains a well-mixed culture at constant volume by feeding fresh nutrient solution and removing the same volume of culture. Its [dilution rate](#dilution-rate) is the volumetric flow divided by the culture volume.

### Monod chemostat equilibrium and relaxation

↑ **Parent:** [Chemostat](#chemostat)

For a dimensionless [chemostat](#chemostat) with [Monod equation](#monod-equation) kinetics,

$$
n'=\alpha\frac{cn}{1+c}-n,\qquad c'=\beta-c-\frac{cn}{1+c},
$$

the total nutrient equivalent $z=c+n/\alpha$ satisfies $z'=\beta-z$. The positive [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system) is $c_*=1/(\alpha-1)$, $n_*=\alpha(\beta-c_*)$, provided $\alpha>1$ and $\beta>c_*$. The [Jacobian matrix](calculus.md#jacobian-matrix) has [eigenvalues](linear-operator-theory.md#eigenvalue) $-1$ and $-n_* /(1+c_*)^2$, so the positive [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system) is [locally asymptotically stable](dynamical-systems.md#asymptotic-stability).

### Dilution rate

↑ **Parent:** [Chemostat](#chemostat)

## Two-season seed-bank recurrence

↑ **Parent:** [Mathematical biology](mathematical-biology.md)

A seed-producing population with first-season and second-season recruitment leads to nonnegative recurrence coefficients $a,b$. Its characteristic roots are $(a\pm\sqrt{a^2+4b})/2$. The nonnegative dominant root is below one precisely when $a+b<1$, giving deterministic decay of every finite initial population. This is a mean-population model; literal integer extinction requires a stochastic interpretation or a separate integer-population argument.

## Population dynamics

↑ **Parent:** [Mathematical biology](mathematical-biology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Population_dynamics)

### Carrying capacity

↑ **Parent:** [Population dynamics](#population-dynamics)

A [carrying capacity](#carrying-capacity) is an abundance scale at which a specified environment's net population growth vanishes. In the [logistic growth equation](#logistic-growth-equation), positive unharvested populations approach $K$. It depends on the species, resources and environment rather than being an immutable universal population [limit](calculus.md#limit-of-a-function).

### Nicholson-Bailey model

↑ **Parent:** [Population dynamics](#population-dynamics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nicholson–Bailey_model)

The [Nicholson-Bailey model](#nicholson-bailey-model) describes seasonal host-parasitoid interaction. [Hosts](biology.md#host-biology) surviving random attacks reproduce, while [parasitoid](biology.md#parasitoid) offspring are proportional to attacked [hosts](biology.md#host-biology). For $r>1$, its positive [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system) is $Y_*=(\log r)/a$, $X_*=rY_*/[c(r-1)]$. Counting attacked rather than surviving [hosts](biology.md#host-biology) makes its [predator](biology.md#predator) reproduction law different from the [annual pulse-breeding predator-prey model](#annual-pulse-breeding-predator-prey-model).

#### Instability of the Nicholson-Bailey equilibrium

↑ **Parent:** [Nicholson-Bailey model](#nicholson-bailey-model)

At the positive [Nicholson-Bailey model](#nicholson-bailey-model) [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system), $\operatorname{tr}J_*=1+\log r/(r-1)$ lies between one and two, and the displayed [determinant](linear-algebra.md#determinant) exceeds one. These follow from $(r-1)/r<\log r<r-1$ for $r>1$. The [discriminant](polynomial.md#discriminant) is therefore negative, and the conjugate [eigenvalues](linear-operator-theory.md#eigenvalue) have [moduli](complex-analysis.md#modulus) greater than one. Nearby annual samples spiral outward rather than approach coexistence.

### Symmetric competition model

↑ **Parent:** [Population dynamics](#population-dynamics)

Two populations grow at the same per-capita rate and each loses members at a rate proportional to their product. On the invariant diagonal $x=y=z$, the [logistic differential equation](differential-equation.md#logistic-differential-equation) gives $z(t)=\lambda/[\mu+(\lambda-\mu)e^{-\lambda t}]$ for $z(0)=1$ and positive rates. The positive symmetric equilibrium $(\lambda/\mu,\lambda/\mu)$ is stable along that diagonal but unstable transversely: $(x-y)'=\lambda(x-y)$, while the [Jacobian matrix](calculus.md#jacobian-matrix) has eigenvalues $-\lambda,+\lambda$. Thus an exactly symmetric deterministic solution can relax toward coexistence while a small imbalance grows. A corresponding [density-dependent Markov jump process](markov-process.md#density-dependent-markov-jump-process) has a controlled [fluid limit](queueing-theory.md#fluid-limit) on each fixed finite interval, rather than uniform control for all time.

### Logistic growth equation

↑ **Parent:** [Population dynamics](#population-dynamics)

For positive growth rate $r$ and carrying capacity $K$, the logistic growth equation has solutions $N(t)=K/[1+be^{-rt}]$ for an initial value between zero and $K$. Its per-capita growth falls linearly with population size; the curve's inflection point occurs at $N=K/2$. A translated and scaled [logistic function](statistical-learning.md#logistic-function) has the same form. In [nonlinear regression](statistical-modelling.md#nonlinear-regression) for biological size, an analogous saturation curve need not imply that circumference itself obeys a mechanistic population law.

#### Constant-quota harvested logistic growth

↑ **Parent:** [Logistic growth equation](#logistic-growth-equation)

For a fixed catch rate $h$, natural logistic growth can replace the catch at two abundances if $0<h<rK/4$. The upper [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system) $N_+=K[1+\sqrt{1-4h/(rK)}]/2$ attracts, and the lower $N_-$ is an unstable survival threshold. They meet in a [saddle-node bifurcation](dynamical-systems.md#saddle-node-bifurcation) at $h=rK/4$, $N=K/2$. Above this catch every positive population declines to zero. Below it a population initially under $N_-$ also becomes extinct. A constant catch is stopped at extinction to avoid negative abundances; it is distinct from per-capita harvesting proportional to $N$.

## Ricker population map

↑ **Parent:** [Mathematical biology](mathematical-biology.md)

The Ricker population map models density-dependent reproduction with a declining per-capita growth factor. Its nonzero equilibrium is $K$, with multiplier $1-r$. It loses stability through a [period-doubling bifurcation](dynamical-systems.md#period-doubling-bifurcation) at $r=2$. Every population after the first update is bounded by $K e^{r-1}/r$, the maximum of the update function on nonnegative populations.

## Squared-denominator population map

↑ **Parent:** [Mathematical biology](mathematical-biology.md)

Here $r>0$ is the low-density per-generation multiplication factor and $b>0$ sets the inverse crowding scale. The positive [fixed point](function.md#fixed-point) is $(\sqrt r-1)/b$ when $r>1$; its derivative $2/\sqrt r-1$ lies strictly between minus one and one, so it is locally asymptotically stable. The map reaches its maximum $r/(4b)$ at $N=1/b$ and decreases thereafter. Stability follows from the derivative, not from assuming that every overcompensating population map undergoes period doubling.

### Post-initial invariant interval for a squared-denominator population map

↑ **Parent:** [Squared-denominator population map](#squared-denominator-population-map)

Starting at $N_1=1/b$ with $r>4$, the next two iterates are the maximum $M=r/(4b)$ and its image $L=4r^2/[b(r+4)^2]$. Since $1/b<L\leq M$ and the [squared-denominator population map](#squared-denominator-population-map) decreases on $[L,M]$, its image there lies in $[L,M]$. Thus the displayed interval is invariant after the initial step, and both bounds are attained. The initial value itself is below $L$, so it must not be included in the lower-bound assertion.

## Distinction between linear resonance and nonlinear periodic bifurcation

↑ **Parent:** [Mathematical biology](mathematical-biology.md)

Roots of unity among the linearization multipliers give periodic linearized perturbations but do not by themselves prove a branch of nonlinear periodic solutions. For the normalized delayed recurrence $F_r(x,y)=(y,r(1+y)/(1+(r-1)(1+x)^2)-1)$, the multipliers at $r=2$ are $e^{\pm i\pi/3}$. Nevertheless, with $Q=x^2-xy+y^2$, its sixth iterate has leading displacement $(r-2)Bv+QDv$, where $B=\left(\begin{smallmatrix}1&1\\-1&2\end{smallmatrix}\right)$ and $D=\left(\begin{smallmatrix}-1/2&-1\\1&-3/2\end{smallmatrix}\right)$. The identity $\det(Bv,QDv)=Q^2/2$ obstructs cancellation for small nonzero $v$. Indeed any putative local six-cycle requires $r-2=O(|v|^2)$ by the norm equation, and then its determinant equation would read $0=Q^2/2+O(|v|^5)$, impossible. This is a concrete caution against promoting a linear resonance to a nonlinear bifurcation assertion.

## Age-structured population equation

↑ **Parent:** [Mathematical biology](mathematical-biology.md)

The density of individuals at age $a$ evolves by transport with unit ageing speed and loss rate $\mu(a)$. New individuals enter at age zero through the integral birth boundary. Exponential separated profiles lead to the [Euler-Lotka equation](#euler-lotka-equation).

### Net reproduction rate

↑ **Parent:** [Age-structured population equation](#age-structured-population-equation)

The mean lifetime number of offspring is the birth rate integrated against the probability of surviving to each age. For a continuous age model it is $\int_0^\infty b(a)\exp[-\int_0^a\mu(s)ds]da$. The [Euler-Lotka equation](#euler-lotka-equation) compares this with one to locate positive population growth.

## Moran process

↑ **Parent:** [Mathematical biology](mathematical-biology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Moran_process)

A fixed-size neutral population evolves by reproduction events in which one individual replaces another. Types are copied along directed reproduction arrows. Backward ancestral lineages merge when one such arrow joins them; the coalescence rate depends on the chosen time normalization.

## Demographic stochasticity

↑ **Parent:** [Mathematical biology](mathematical-biology.md)

Randomness in individual births, deaths and maturation makes a finite population fluctuate even in a fixed environment. Near a deterministic extinction threshold it can drive the population into an absorbing extinct state.

## Mathematical epidemiology

↑ **Parent:** [Mathematical biology](mathematical-biology.md)

Mathematical epidemiology uses [mathematical models](mathematics.md#mathematical-model) and [statistical inference](statistical-inference.md) to study the occurrence, transmission, and control of disease in populations.

### Contact reciprocity in a two-group epidemic

↑ **Parent:** [Mathematical epidemiology](#mathematical-epidemiology)

Each undirected cross-group partnership is counted once from each group's contact total. Thus group size times per-person contact rate times cross-group fraction must agree. If one group occupies fraction $p$ while its cross-group per-person rate stays fixed, aggregate cross-group contact is order $p$ and the other group's cross-contact fraction is order $p$. Assigning both per-person rates independently generally breaks this balance.

### Macroparasite burden model

↑ **Parent:** [Mathematical epidemiology](#mathematical-epidemiology)

A [macroparasite burden model](#macroparasite-burden-model) tracks the distribution of [within-host parasite burdens](biology.md#within-host-parasite-burden) and couples it to transmission or environmental infectious stages. [Mean](probability-theory.md#expected-value) burden alone is insufficient when worm mating, nonlinear fecundity, [immunity](biology.md#immunity-medical) or [host](biology.md#host-biology) mortality depend on that distribution.

#### Mating-limited macroparasite transmission

↑ **Parent:** [Macroparasite burden model](#macroparasite-burden-model)

For sexually reproducing worms, an infected [host](biology.md#host-biology) need not contain both sexes. Independent random sexes split a Poisson total burden of [mean](probability-theory.md#expected-value) $m$ into independent male and female [Poisson distributions](discrete-probability-distribution.md#poisson-distribution) of [mean](probability-theory.md#expected-value) $m/2$, giving the displayed [probability](probability-theory.md#probability) of a fertile mixed-sex burden. For an arbitrary burden [probability generating function](probability-theory.md#probability-generating-function) $G$, this [probability](probability-theory.md#probability) is $1-2G(1/2)+G(0)$. Its low-burden behaviour can introduce an [Allee effect](#allee-effect) in transmission, so an asexual mean-burden invasion calculation is not automatically valid.

#### Aggregation of macroparasite burdens

↑ **Parent:** [Macroparasite burden model](#macroparasite-burden-model)

If host-specific [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system) [mean](probability-theory.md#expected-value) burden has a [gamma distribution](continuous-probability-distribution.md#gamma-distribution), conditional [Poisson distributions](discrete-probability-distribution.md#poisson-distribution) produce a [Poisson-gamma mixture](discrete-probability-distribution.md#poisson-gamma-mixture), hence a [negative binomial distribution](discrete-probability-distribution.md#negative-binomial-distribution). With [mean](probability-theory.md#expected-value) $m$ and shape $k$, its zero-burden [probability](probability-theory.md#probability) is $(1+m/k)^{-k}$. Decreasing $k$ increases aggregation: a smaller infected-host [prevalence](#prevalence) can accompany the same [mean](probability-theory.md#expected-value) burden and more heavily infected individuals.

#### Immigration-death worm-burden model

↑ **Parent:** [Macroparasite burden model](#macroparasite-burden-model)

[Independent](random-variable.md#independent-random-variables) worm acquisition at rate $\lambda$ and loss at rate $\mu j$ produce a [birth-death process](markov-process.md#birth-death-process) for [within-host parasite burden](biology.md#within-host-parasite-burden). Summing its forward equations against $j$ gives $d\mathbb E[j]/dt=\lambda-\mu\mathbb E[j]$. At constant exposure, detailed balance $\lambda p_j=\mu(j+1)p_{j+1}$ yields a [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) with [mean](probability-theory.md#expected-value) $\lambda/\mu$. Heterogeneous acquisition rates change the pooled burden distribution even when each individual [host](biology.md#host-biology) follows this model.

### Stochastic epidemic model

↑ **Parent:** [Mathematical epidemiology](#mathematical-epidemiology)

A [stochastic epidemic model](#stochastic-epidemic-model) represents infection and recovery as random events. A [continuous-time Markov chain](markov-process.md#continuous-time-markov-chain) can track integer counts, while a [stochastic SIR model](#stochastic-sir-model) illustrates random fade-out and finite-population outbreak variability that a deterministic [limit](calculus.md#limit-of-a-function) does not show.

### Recovery rate

↑ **Parent:** [Mathematical epidemiology](#mathematical-epidemiology)

In a continuous-time epidemic model, a constant [recovery rate](#recovery-rate) $\gamma$ gives an [exponential distribution](continuous-probability-distribution.md#exponential-distribution) of infectious duration with [mean](probability-theory.md#expected-value) $1/\gamma$. Other duration distributions require additional stages or infection-age structure.

### Quarantine

↑ **Parent:** [Mathematical epidemiology](#mathematical-epidemiology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quarantine)

[Quarantine](#quarantine) restricts contacts of exposed individuals whose infection status is uncertain, with monitoring to detect illness. It differs from [isolation](biology.md#isolation-health-care) of recognized infected or ill individuals. An [incubation period](#incubation-period) [quantile](probability-theory.md#quantile-function) can enter a duration calculation, but assumptions about exposure time, symptom detection and infectiousness are needed before the calculation describes transmission risk.

### Incubation period

↑ **Parent:** [Mathematical epidemiology](#mathematical-epidemiology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Incubation_period)

The [incubation period](#incubation-period) is the interval from infection to symptom onset in a person who develops symptoms. Its [probability distribution](probability-theory.md#probability-distribution) describes onset times, not the full timing of infectiousness. Exposure may only be known to fall in an interval, requiring a corresponding observation model when estimating this distribution.

### Back-calculation of infection incidence

↑ **Parent:** [Mathematical epidemiology](#mathematical-epidemiology)

Observed symptom-onset intensity is the [convolution](fourier-analysis.md#convolution) of past infection intensity with the incubation delay density: $\mu(t)=\int_0^\infty h(t-s)f(s)ds$. Back-calculation infers the infection history from that relation. Include pre-observation infections unless their absence is known.

#### Discrete back-calculation with endpoint cohorts

↑ **Parent:** [Back-calculation of infection incidence](#back-calculation-of-infection-incidence)

For equal-width time bins and infections assigned to bin-end time $t_i$, let $q_\ell=\Pr((\ell-1)\Delta\leq T<\ell\Delta)$. The next onset-bin mean is $\mu_k=\sum_{i<k}h_iq_{k-i}$. Assigning infections instead to bin starts shifts the index by one. Bin probabilities integrate a delay density; they are not the density itself.

### Calendar time

↑ **Parent:** [Mathematical epidemiology](#mathematical-epidemiology)

Calendar time locates an event on a shared external timeline, in contrast with an individual's age or the time elapsed since an individual event.

### Incidence (epidemiology)

↑ **Parent:** [Mathematical epidemiology](#mathematical-epidemiology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Incidence_(epidemiology))

Incidence measures the occurrence of new cases in a population during a specified period.

### Infection age

↑ **Parent:** [Mathematical epidemiology](#mathematical-epidemiology)

The infection age of an infected individual is the time elapsed since that individual's infection.

### Imported infection

↑ **Parent:** [Mathematical epidemiology](#mathematical-epidemiology)

An imported infection is acquired outside the population or observation system being modelled and enters it as an external source of incidence.

### Infectivity profile

↑ **Parent:** [Mathematical epidemiology](#mathematical-epidemiology)

An infectivity profile describes how an infected individual's transmission rate varies with [infection age](#infection-age).

#### Generation interval

↑ **Parent:** [Infectivity profile](#infectivity-profile)

The generation interval is the time between infection of a source individual and infection of a secondary case caused by that source.

##### Generation-interval distribution

↑ **Parent:** [Generation interval](#generation-interval)

The generation-interval distribution gives the probability law of the [generation interval](#generation-interval). In discrete time, its probabilities $g_\tau$ form a nonnegative sequence summing to one.

###### Infectious disease renewal equation

↑ **Parent:** [Generation-interval distribution](#generation-interval-distribution)

The infectious disease renewal equation expresses current [incidence](#incidence-epidemiology) as a [convolution](fourier-analysis.md#convolution) of past incidence with an [infectivity profile](#infectivity-profile), multiplied by a time-varying transmission level.

###### Total infectiousness

↑ **Parent:** [Infectious disease renewal equation](#infectious-disease-renewal-equation)

For incidence $I_t$ and discrete generation-interval probabilities $g_\tau$, the total infectiousness at time $t$ is $\Lambda_t=\sum_{\tau\geq1}g_\tau I_{t-\tau}$.

###### Time-varying reproduction number

↑ **Parent:** [Infectious disease renewal equation](#infectious-disease-renewal-equation)

A time-varying reproduction number describes transmission at a specified calendar time while allowing transmission conditions to change during an epidemic.

###### Instantaneous reproduction number

↑ **Parent:** [Time-varying reproduction number](#time-varying-reproduction-number)

The instantaneous reproduction number freezes the transmission conditions at calendar time $t$ and counts the expected secondary infections produced over a complete infectious lifetime under those conditions.

###### Case reproduction number

↑ **Parent:** [Time-varying reproduction number](#time-varying-reproduction-number)

The case reproduction number is the expected number of secondary infections actually generated by a person infected at time $t$, allowing transmission conditions to change during that person's infectious lifetime.

## Per capita

↑ **Parent:** [Mathematical biology](mathematical-biology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Per_capita)

A per-capita quantity is a total quantity divided by the number of individuals in the population.

## Lotka-Volterra predator-prey model

↑ **Parent:** [Mathematical biology](mathematical-biology.md)

The Lotka-Volterra predator-prey model couples exponential prey growth and predator mortality through a bilinear encounter term. Its positive coexistence equilibrium is surrounded by closed conserved-energy curves, so the populations oscillate periodically in the idealized model.

### Annual pulse-breeding predator-prey model

↑ **Parent:** [Lotka-Volterra predator-prey model](#lotka-volterra-predator-prey-model)

An [annual pulse-breeding predator-prey model](#annual-pulse-breeding-predator-prey-model) combines continuous [predation](biology.md#predation) and mortality between short reproduction episodes with an annual [difference equation](real-analysis.md#difference-equation). If surviving [predators](biology.md#predator) produce offspring in proportion to [prey](biology.md#prey) surviving the year, retained adults give the displayed map. Here $r$ combines [prey](biology.md#prey) reproduction and natural survival, $s$ is [predator](biology.md#predator) survival, and $\kappa$ integrates [predation](biology.md#predation) over declining [predator](biology.md#predator) abundance. The positive annual [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system) is $X_*=(1-s)/(sb)$, $Y_*=\log r/\kappa$ for $r>1$ and $0<s<1$.

#### Area-preserving seasonal predator-prey map

↑ **Parent:** [Annual pulse-breeding predator-prey model](#annual-pulse-breeding-predator-prey-model)

The [annual pulse-breeding predator-prey model](#annual-pulse-breeding-predator-prey-model) is an [area-preserving map](dynamical-systems.md#area-preserving-map) in logarithmic population coordinates: $u'=u+\log r-\kappa e^v$, then $v'=v+\log s+\log(1+be^{u'})$. Each step is a shear of [determinant](linear-algebra.md#determinant) one. At a positive [fixed point](function.md#fixed-point), the ordinary-population [Jacobian matrix](calculus.md#jacobian-matrix) has [determinant](linear-algebra.md#determinant) one and [trace](linear-algebra.md#matrix-trace) $2-(1-s)\log r$. [Eigenvalues](linear-operator-theory.md#eigenvalue) lie on the [unit circle](complex-analysis.md#complex-unit-circle) for $0<(1-s)\log r<4$, but this linear neutrality does not prove nonlinear stability at every resonance. Area preservation excludes an isolated attracting positive periodic cycle.

### Fixed-quota harvesting of Lotka-Volterra populations

↑ **Parent:** [Lotka-Volterra predator-prey model](#lotka-volterra-predator-prey-model)

In logarithmic prey/predator coordinates, the [Lotka-Volterra predator-prey model](#lotka-volterra-predator-prey-model) has divergence zero. Removing a fixed prey quota $h$ changes $\log X$ to $\log(X-h)$ and expands logarithmic area by $X/(X-h)$. Thus a periodic annually harvested orbit has an expanding [return map](dynamical-systems.md#poincare-map) [determinant](linear-algebra.md#determinant) and cannot be asymptotically stable. A continuous-quota approximation gives a coexistence [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system) with positive [Jacobian matrix](calculus.md#jacobian-matrix) [trace](linear-algebra.md#matrix-trace) $h/X_*$, unlike proportional harvesting, which only changes the prey growth parameter in this idealized model.

#### Event-triggered harvesting by conserved energy

↑ **Parent:** [Fixed-quota harvesting of Lotka-Volterra populations](#fixed-quota-harvesting-of-lotka-volterra-populations)

The predator-prey [first integral](differential-equation.md#first-integral) $H=cX-d\log X+bY-a\log Y$ changes by the displayed amount when $h$ prey are removed. At a fixed prey threshold this increment is constant; sufficiently high thresholds reduce oscillation energy until the threshold is no longer crossed. At a fixed predator threshold, the increment depends on the prey abundance and on the crossing direction. A rising-predator balanced-quota cycle has negative return multiplier of magnitude greater than one; its leading small-oscillation approximation is marginal rather than a robust attractor.

### Logistic predator-prey model

↑ **Parent:** [Lotka-Volterra predator-prey model](#lotka-volterra-predator-prey-model)

This [Lotka-Volterra predator-prey model](#lotka-volterra-predator-prey-model) includes self-limitation of the prey through the term $-bx^2$, with positive constants $a,b,c,d,e$. A positive coexistence [equilibrium point](dynamical-systems.md#equilibrium-point-of-a-dynamical-system) exists when $a>be/d$, at $x_*=e/d$, $y_*=(a-bx_*)/c$. The [Lyapunov function](dynamical-systems.md#lyapunov-function)

$$
V=d[x-x_*-x_*\log(x/x_*)]
+c[y-y_*-y_*\log(y/y_*)]
$$

satisfies $\dot V=-bd(x-x_*)^2$: its predator-prey cross terms cancel. Its sublevel sets are compact in the positive quadrant. The only invariant subset of $\{\dot V=0\}$ is the coexistence [equilibrium point](dynamical-systems.md#equilibrium-point-of-a-dynamical-system), because staying on $x=x_*$ requires $y=y_*$. The [LaSalle invariance principle](dynamical-systems.md#lasalle-s-invariance-principle) therefore proves convergence to coexistence for every positive initial state.

#### Quadratic discrete predator-prey map

↑ **Parent:** [Logistic predator-prey model](#logistic-predator-prey-model)

This map equals an explicit unit-step update of a logistic predator-prey differential equation. Its coexistence [fixed point](function.md#fixed-point) is $(b,(1-a-b)/a)$, requiring $a+b<1$. Its [trace](linear-algebra.md#matrix-trace) and [determinant](linear-algebra.md#determinant) are $T=2-b/a$ and $D=(1-2b)/a$. The [Schur stability criterion](numerical-analysis.md#schur-stability-criterion) gives stability precisely when $b>(1-a)/2$ and $b<a+1/3$. The coexistence flip at $b=a+1/3$ is subcritical on $1/9<a<1/3$, with effective cubic coefficient $-9/[(3a+1)^2(9a-1)]$ when the $-1$ eigenvector has first component one. The unit-circle crossing $a+2b=1$ is a supercritical [Neimark–Sacker bifurcation](dynamical-systems.md#neimark-sacker-bifurcation) away from the [strong resonances of a planar map](dynamical-systems.md#strong-resonance-of-a-planar-map) $a=1/7,1/5$; in the eigenvector normalization $q_1=1$ its cubic radial coefficient is $-1/[a^2(1-a)]$. The whole nonnegative quadrant is not forward invariant, because $x'$ can become negative. Local fixed-point stability is therefore not a global population-dynamics classification.

// Destination: dynamical-systems.bigb

## Age-structured population model

↑ **Parent:** [Mathematical biology](mathematical-biology.md)

An age-structured population model tracks a density $n(a,t)$ transported toward greater age, reduced by age-dependent mortality, and replenished at age zero by births.

The continuous-age transport version is the [Von Foerster equation](#von-foerster-equation). Discrete age-class models are other members of this broader modeling class.

### Von Foerster equation

↑ **Parent:** [Age-structured population model](#age-structured-population-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Von_Foerster_equation)

The [Von Foerster equation](#von-foerster-equation) transports a population density through age while mortality removes individuals. A birth boundary condition at age zero closes the model; for a prescribed fertility rate it has the form $n(0,t)=\int b(a,t)n(a,t)\,da$.

### Seed-bank population recurrence

↑ **Parent:** [Age-structured population model](#age-structured-population-model)

A [seed-bank population recurrence](#seed-bank-population-recurrence) includes delayed recruitment from seeds that survive more than one season. For $a,b\ge0$, recruitment function $N$ with $N(0)=0$ and $N'(0)=1$ gives extinction multipliers solving $\lambda^2-a\lambda-b=0$. If $N$ is strictly concave, bounded and increasing, a positive fixed point exists uniquely exactly when $a+b>1$; it solves $M=N((a+b)M)$. The dominant extinction multiplier then exceeds one.

### Euler-Lotka equation

↑ **Parent:** [Age-structured population model](#age-structured-population-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euler-Lotka_equation)

For birth rate $b(a)$, death rate $d(a)$ and exponential population growth rate $r$, the Euler-Lotka equation is

$$
1=\int_0^\infty b(a)\exp\left(-ra-\int_0^ad(s)ds\right)da.
$$

#### Discrete Euler-Lotka equation

↑ **Parent:** [Euler-Lotka equation](#euler-lotka-equation)

For annual survival probabilities $1-\mu_i$, age-specific offspring numbers $b_a$, and a population multiplier $\gamma$, the discrete Euler-Lotka equation is

$$
1=\sum_{a=1}^{\infty}
\left[\prod_{i=0}^{a-1}(1-\mu_i)\right]\gamma^{-a}b_a.
$$

Its value at $\gamma=1$ is the expected lifetime offspring count of a newborn under the fixed vital rates. A value above one implies a growing mode $\gamma>1$, while a value below one implies decline.

## Law of mass action

↑ **Parent:** [Mathematical biology](mathematical-biology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Law_of_mass_action)

The law of mass action assigns an elementary reaction a rate constant times the product of its reactant concentrations, with each concentration raised to its stoichiometric multiplicity.

## Chemical reaction network

↑ **Parent:** [Mathematical biology](mathematical-biology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chemical_reaction_network)

A chemical reaction network specifies [chemical species](#chemical-species), reactions between them, and their [stoichiometric vectors](#stoichiometric-vector). It can be modelled deterministically by [reaction-rate equations](#rate-equation) or stochastically by molecule-copy-number jumps.

### Mean-field joint removal of two chemical species

↑ **Parent:** [Chemical reaction network](#chemical-reaction-network)

Equal constant production, individual linear removal, and joint bimolecular removal give $d(\mu_1-\mu_2)/dt=-\beta(\mu_1-\mu_2)$. For $\beta>0$ the unique stable equilibrium is symmetric and solves $\lambda=\beta\mu+C\mu^2$. For $\beta=0<C$, every point on $\mu_1\mu_2=\lambda/C$ is an equilibrium: the difference is conserved and trajectories approach the equilibrium on their own constant-difference line.

// Target: mathematical-biology.bigb

#### Exclusive joint removal has a diffusing difference mode

↑ **Parent:** [Mean-field joint removal of two chemical species](#mean-field-joint-removal-of-two-chemical-species)

If individual removal is absent, simultaneous removal of one molecule from each species leaves $X_1-X_2$ unchanged. Independent constant-rate births change it by plus or minus one, each at rate $\lambda$. The difference is therefore a symmetric [continuous-time random walk](markov-process.md#continuous-time-random-walk) on the integers with variance growing as displayed. It has no normalizable stationary law. This explains why a deterministic attracting line of equilibria does not provide a stationary stochastic distribution.

// Target: probability-and-statistics.bigb

#### Linear noise of two species with joint removal

↑ **Parent:** [Mean-field joint removal of two chemical species](#mean-field-joint-removal-of-two-chemical-species)

For $E=C\mu/(\beta+C\mu)<1$ and mean lifetime $\tau=(\beta+C\mu)^{-1}$, the normalized restoring matrix is $M=\tau^{-1}\begin{pmatrix}1&E\\E&1\end{pmatrix}$ and the diffusion matrix is $D=(\tau\mu)^{-1}\begin{pmatrix}2&E\\E&2\end{pmatrix}$. Solving the [normalized stationary fluctuation-dissipation relation for a reaction network](markov-process.md#normalized-stationary-fluctuation-dissipation-relation-for-a-reaction-network) gives the displayed covariance. The sum mode remains damped, but the difference mode's restoring rate is $\beta=(1-E)/\tau$. Its noise grows without bound relative to that restoring rate as $E\to1$, giving strong negative correlations and invalidating small-fluctuation closure near exclusive joint removal.

// Target: mathematical-biology.bigb

### Chemical species

↑ **Parent:** [Chemical reaction network](#chemical-reaction-network)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chemical_species)

A chemical species is a class of chemically identical entities treated as one component of a reaction system.

#### Mole fraction

↑ **Parent:** [Chemical species](#chemical-species)

The mole fraction of species $i$ is $x_i=N_i/\sum_jN_j$, where $N_i$ is its amount in moles. It is dimensionless and equals the [volume mixing ratio](#volume-mixing-ratio) for an [ideal gas](thermodynamics.md#ideal-gas) mixture.

#### Volume mixing ratio

↑ **Parent:** [Chemical species](#chemical-species)

For an [ideal gas](thermodynamics.md#ideal-gas) mixture, the volume mixing ratio $x_i$ equals the [mole fraction](#mole-fraction), number fraction, and ratio of partial to total [pressure](thermodynamics.md#pressure): $x_i=N_i/N=n_i/n=P_i/P$, with $\sum_i x_i=1$. This equivalence fails for general nonideal mixtures.

### Stoichiometric vector

↑ **Parent:** [Chemical reaction network](#chemical-reaction-network)

The stoichiometric vector of reaction $r$ records its net change in each [chemical species](#chemical-species). If the copy-number state is $x$, firing the reaction changes it to $x+\nu_r$.

### Rate equation

↑ **Parent:** [Chemical reaction network](#chemical-reaction-network)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rate_equation)

A reaction-rate equation is an [ordinary differential equation](differential-equation.md#ordinary-differential-equation) for continuously varying species concentrations. Under the [law of mass action](#law-of-mass-action), its reaction rates are monomials in those concentrations.

#### Reaction-rate elasticity

↑ **Parent:** [Rate equation](#rate-equation)

The displayed logarithmic derivative compares the loss and production flux sensitivities of species $i$ to the mean amount $\mu_j$. At a steady state $v_i^+=v_i^-=v_i$, it converts the normalized negative drift Jacobian into $M_{ij}=H_{ij}/\tau_i$, where $\tau_i=\mu_i/v_i$ is the [mean molecular lifetime](#mean-molecular-lifetime). For constant production and loss proportional to $\mu^\alpha$, the scalar elasticity is $H=\alpha$.

// Target: mathematical-biology.bigb

### Stochastic chemical kinetics

↑ **Parent:** [Chemical reaction network](#chemical-reaction-network)

Stochastic chemical kinetics models molecular copy numbers as a [continuous-time Markov chain](markov-process.md#continuous-time-markov-chain). Each reaction has a state-dependent [reaction propensity function](#reaction-propensity-function) and changes the state by its [stoichiometric vector](#stoichiometric-vector) when it fires.

#### Molecular-flux-weighted reaction event size

↑ **Parent:** [Stochastic chemical kinetics](#stochastic-chemical-kinetics)

This noise-relevant event size weights absolute stoichiometric jump sizes by their molecular turnover flux. At stationarity the denominator is twice the balanced production or removal flux $v_i$, so the normalized diffusion diagonal is $D_{ii}=2\langle s_i\rangle/(\tau_i\mu_i)$. Fixed birth bursts of size $b$ and unit deaths give $\langle s\rangle=(b+1)/2$. This quantity is not the event-count-weighted average absolute jump size.

// Target: mathematical-biology.bigb

#### Mean molecular lifetime

↑ **Parent:** [Stochastic chemical kinetics](#stochastic-chemical-kinetics)

At stationarity, the mean number $\mu_i$ divided by the molecular removal flux $v_i$ is the mean time a molecule remains in the system. Birth or death event rates must be multiplied by the numbers of molecules changed in each event before computing this lifetime.

// Target: mathematical-biology.bigb

#### Compartment-based stochastic diffusion

↑ **Parent:** [Stochastic chemical kinetics](#stochastic-chemical-kinetics)

Compartment-based stochastic diffusion represents molecular motion by nearest-neighbour jumps on a spatial lattice. Jump rates of order $D/h^2\pm v/(2h)$ converge to an advection--diffusion equation as compartment width $h$ tends to zero.

##### Asymmetric simple exclusion process

↑ **Parent:** [Compartment-based stochastic diffusion](#compartment-based-stochastic-diffusion)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Asymmetric_simple_exclusion_process)

The asymmetric simple exclusion process permits at most one particle per lattice site and biases jumps in one direction. A mean-field hydrodynamic limit has advective flux proportional to $c(1-c)$ because both an occupied departure site and vacant arrival site are required.

<h4 id="immigration-death-process">Immigration--death process</h4>

↑ **Parent:** [Stochastic chemical kinetics](#stochastic-chemical-kinetics)

An immigration--death process has constant birth rate $b$ and linear death rate $dy$ in state $y$. Its stationary distribution is Poisson with mean $b/d$.

##### Pair immigration with linear deaths

↑ **Parent:** [Immigration--death process](#immigration-death-process)

A population jumps from $n$ to $n+2$ at a constant immigration rate $\lambda$ and from $n$ to $n-1$ at rate $\beta n$. Applying its [Markov jump-process generator](markov-process.md#markov-jump-process-generator) to $n$ and $n^2$ gives the displayed mean and variance equations. For $\beta>0$ and finite initial second moment, the stationary mean and variance are $2\lambda/\beta$ and $3\lambda/\beta$. Interpreting the pair-arrival rate as proportional to population instead would produce a different branching process.

#### Stochastic quasi-steady-state approximation

↑ **Parent:** [Stochastic chemical kinetics](#stochastic-chemical-kinetics)

A stochastic quasi-steady-state approximation replaces fast species by their stationary conditional distribution given the slow species. Averaging slow propensities over that distribution yields a reduced Markov jump process.

##### Slow-scale stochastic simulation algorithm

↑ **Parent:** [Stochastic quasi-steady-state approximation](#stochastic-quasi-steady-state-approximation)

A slow-scale stochastic simulation algorithm applies the Gillespie algorithm to propensities averaged over fast conditional equilibrium, avoiding explicit simulation of every fast reaction.

#### Molecular copy number

↑ **Parent:** [Stochastic chemical kinetics](#stochastic-chemical-kinetics)

The molecular copy number of a [chemical species](#chemical-species) is the [nonnegative integer](arithmetic.md#natural-number) number of its molecules in a specified reactor or compartment.

#### Reaction propensity function

↑ **Parent:** [Stochastic chemical kinetics](#stochastic-chemical-kinetics)

The reaction propensity $a_r(x)$ is the instantaneous rate at which reaction $r$ fires when the copy-number state is $x$. Conditional on the present state, its reaction clock has an [exponential distribution](continuous-probability-distribution.md#exponential-distribution) of rate $a_r(x)$.

##### Power-law reaction propensity

↑ **Parent:** [Reaction propensity function](#reaction-propensity-function)

A power-law propensity uses the same reactant monomial as a deterministic [law of mass action](#law-of-mass-action), scaled by reactor volume. For example, a bimolecular channel may be assigned $a(x)=\alpha x^2/V$. This convention differs at small copy number from the combinatorial propensity $\alpha x(x-1)/V$ and must therefore be stated explicitly.

#### Chemical master equation

↑ **Parent:** [Stochastic chemical kinetics](#stochastic-chemical-kinetics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chemical_master_equation)

For reactions with [stoichiometric vectors](#stoichiometric-vector) $\nu_r$ and [reaction propensity functions](#reaction-propensity-function) $a_r$, the probability mass function $p(x,t)$ obeys

$$
\partial_t p(x,t)=\sum_r\left[a_r(x-\nu_r)p(x-\nu_r,t)-a_r(x)p(x,t)\right].
$$

It is the [forward operator of a Markov jump process](markov-process.md#forward-operator-of-a-markov-jump-process) equation for the copy-number [continuous-time Markov chain](markov-process.md#continuous-time-markov-chain).

#### Gillespie algorithm

↑ **Parent:** [Stochastic chemical kinetics](#stochastic-chemical-kinetics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gillespie_algorithm)

The Gillespie algorithm samples an exact path of a well-mixed stochastic reaction network. At state $x$, let $a_0(x)=\sum_ra_r(x)$; draw a waiting time with [exponential distribution](continuous-probability-distribution.md#exponential-distribution) of rate $a_0$, choose reaction $r$ with probability $a_r/a_0$, and update $x\leftarrow x+\nu_r$.

#### Moment hierarchy

↑ **Parent:** [Stochastic chemical kinetics](#stochastic-chemical-kinetics)

A moment hierarchy is the coupled family of equations obtained by applying a [Markov jump-process generator](markov-process.md#markov-jump-process-generator) to powers of the state. Nonlinear [reaction propensity functions](#reaction-propensity-function) make a moment of one order depend on higher-order moments, so the hierarchy generally does not close after finitely many equations.

##### Moment equation

↑ **Parent:** [Moment hierarchy](#moment-hierarchy)

For a [Markov jump-process generator](markov-process.md#markov-jump-process-generator) $L$, differentiating an integrable observable gives $d\mathbb E[f(X_t)]/dt=\mathbb E[Lf(X_t)]$, when the generator identity and interchange are justified. Choosing powers gives equations for [moments](probability-theory.md#moment). These need not form a closed finite system.

##### Moment closure

↑ **Parent:** [Moment hierarchy](#moment-hierarchy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Moment_closure)

A moment closure replaces higher moments in a [moment hierarchy](#moment-hierarchy) by functions of retained lower moments. It converts an infinite hierarchy into a finite approximate system.

###### Central-moment closure

↑ **Parent:** [Moment closure](#moment-closure)

A central-moment closure sets selected high-order [central moments](probability-theory.md#central-moment) to zero. For example, setting the third central moment of $X$ to zero gives

$$
\mathbb E[X^3]=3\mathbb E[X]\mathbb E[X^2]-2(\mathbb E[X])^3.
$$

## Enzyme kinetics

↑ **Parent:** [Mathematical biology](mathematical-biology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Enzyme_kinetics)

Enzyme kinetics models how free enzyme, substrate, enzyme-substrate complexes, and product concentrations evolve through a reaction mechanism.

### Sequential two-site enzyme reaction network

↑ **Parent:** [Enzyme kinetics](#enzyme-kinetics)

An [enzyme](biology.md#enzyme) may bind one molecule of a [substrate](biology.md#substrate-biochemistry) to form $C_1$, then a second to form $C_2$, with product-release reactions $C_1\to E+P$ and $C_2\to C_1+P$. The [law of mass action](#law-of-mass-action) gives conservation laws $e+c_1+c_2=e_0$ and $s+c_1+2c_2+p=s_0$. Scaling substrate by $s_0$, complexes by $e_0$ and time by $(k_1e_0)^{-1}$ exposes the small ratio $\epsilon=e_0/s_0$: the substrate evolves on the slow scale while the complex equations have the form $\epsilon v_i'=g_i$. This is a starting point for [quasi-steady-state approximation](#quasi-steady-state-approximation) when $\epsilon\ll1$.

### Michaelis-Menten kinetics

↑ **Parent:** [Enzyme kinetics](#enzyme-kinetics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Michaelis–Menten_kinetics)

[Michaelis-Menten kinetics](#michaelis-menten-kinetics) models substrate binding to an enzyme, complex dissociation and product formation. Under the relevant quasi-steady-state regime, its initial-rate law is the saturating relation given by the following equation.

#### Michaelis-Menten equation

↑ **Parent:** [Michaelis-Menten kinetics](#michaelis-menten-kinetics)

The Michaelis-Menten rate law is

$$
v=\frac{V_{\max}s}{K_M+s}.
$$

It is linear at low substrate concentration and saturates at $V_{\max}$ at high concentration.

### Quasi-steady-state approximation

↑ **Parent:** [Enzyme kinetics](#enzyme-kinetics)

When enzyme complexes relax much faster than substrate concentrations, the quasi-steady-state approximation sets the time derivatives of the fast complexes to zero and solves their algebraic balance equations.

It approximates the fast intermediate by a [steady state](chemistry.md#steady-state-chemistry) balance without requiring the entire chemical system to be at equilibrium.

#### Quasi-steady rate law for a two-substrate allosteric enzyme

↑ **Parent:** [Quasi-steady-state approximation](#quasi-steady-state-approximation)

For sequential binding with dimensionless parameters $\alpha,\beta,\gamma$, the reduced product rate has the form

$$
\frac{dp}{dt}
=A\frac{u^2}{\alpha+u+(\beta/\gamma)u^2}.
$$

It is quadratic at low substrate concentration and saturates at high concentration.

## Autocatalysis

↑ **Parent:** [Mathematical biology](mathematical-biology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Autocatalysis)

Autocatalysis is a reaction mechanism in which a product promotes its own production.

### Autocatalytic biochemical switch

↑ **Parent:** [Autocatalysis](#autocatalysis)

An autocatalytic biochemical switch uses bistability and a transient input to move a system from one stable concentration to another. A [saddle-node bifurcation](dynamical-systems.md#saddle-node-bifurcation) supplies a threshold above which the low-concentration equilibrium disappears.

#### Saturating autocatalytic switch

↑ **Parent:** [Autocatalytic biochemical switch](#autocatalytic-biochemical-switch)

For

$$
\dot g=s+k\frac{g^2}{1+g^2}-g,
\qquad k>2,
$$

the zero-input stable states are $0$ and $(k+\sqrt{k^2-4})/2$. The switching threshold is the [saddle-node bifurcation](dynamical-systems.md#saddle-node-bifurcation) determined by $f(g_c,s_c)=\partial_gf(g_c,s_c)=0$ on the low-concentration branch.

##### Strong-autocatalysis switching threshold

↑ **Parent:** [Saturating autocatalytic switch](#saturating-autocatalytic-switch)

For $k\gg1$, the low-concentration saddle node of the [saturating autocatalytic switch](#saturating-autocatalytic-switch) has

$$
g_c\sim\frac1{2k},
\qquad
s_c\sim\frac1{4k}.
$$

## Cubic saturation population model

↑ **Parent:** [Mathematical biology](mathematical-biology.md)

The equation

$$
\dot n=\alpha n-\beta n^3
=\alpha n\left(1-\frac{n^2}{K^2}\right),
\qquad K=\sqrt{\alpha/\beta},
$$

has an unstable zero equilibrium and a stable positive equilibrium $K$. Its per-capita density correction is quadratic rather than the logistic model's linear correction.

## Exponential density-dependent birth model

↑ **Parent:** [Mathematical biology](mathematical-biology.md)

If a population $N$ has per-capita birth rate $be^{-aN}$ and per-capita death rate $d$, then

$$
\dot N=N\left(be^{-aN}-d\right).
$$

When $b>d$, its positive [equilibrium](dynamical-systems.md#equilibrium-of-an-autonomous-differential-equation) is

$$
N^*=\frac1a\log\frac bd,
$$

and the derivative of the scalar vector field there is $-adN^*<0$, so the equilibrium is locally [asymptotically stable](dynamical-systems.md#asymptotic-stability).

## Survival-augmented Ricker map

↑ **Parent:** [Mathematical biology](mathematical-biology.md)

The population iteration

$$
x_{n+1}=x_n\bigl(r+ke^{-\lambda x_n}\bigr),
\qquad 0\leq r<1,
$$

combines annual survival with density-dependent recruitment. Its positive equilibrium is

$$
x_*=\frac1\lambda\log\frac{k}{1-r},
$$

which exists when $k>1-r$.

### Nonlinear stability at the Ricker flip threshold

↑ **Parent:** [Survival-augmented Ricker map](#survival-augmented-ricker-map)

At the upper multiplier-$-1$ threshold of $x\mapsto sx+kxe^{-\gamma x}$, set $u=\gamma(x-x_*)$. The second iterate is $u-2(s^2-s/2+1/6)u^3+O(u^4)$. Since its cubic damping coefficient is positive for $0\leq s<1$, this endpoint is locally [asymptotically stable](dynamical-systems.md#asymptotic-stability) despite the inconclusive linear multiplier.

### Stability interval of the survival-augmented Ricker equilibrium

↑ **Parent:** [Survival-augmented Ricker map](#survival-augmented-ricker-map)

At the positive equilibrium,

$$
g'(x_*)=1-(1-r)\log\frac{k}{1-r}.
$$

The fixed point is strictly [linearly stable](dynamical-systems.md#linear-stability) when

$$
1-r<k<(1-r)e^{2/(1-r)}.
$$

The upper endpoint is also locally [asymptotically stable](dynamical-systems.md#asymptotic-stability), as the [nonlinear stability at the Ricker flip threshold](#nonlinear-stability-at-the-ricker-flip-threshold) shows; hence the full local asymptotic-stability interval includes that endpoint. The lower endpoint has no positive equilibrium.

## Malthusian delay differential equation

↑ **Parent:** [Mathematical biology](mathematical-biology.md)

The scalar equation $n'(t)=rn(t-\tau)$ makes the present growth rate depend on the population one delay time earlier. A history function on $[-\tau,0]$ is required in place of a single initial value.

This is one linear [delay differential equation](differential-equation.md#delay-differential-equation), rather than the entire delayed-evolution class.

### Method of steps for a delay differential equation

↑ **Parent:** [Malthusian delay differential equation](#malthusian-delay-differential-equation)

Given the solution on one interval of length $\tau$, the delayed term is known on the next interval, where the delay equation becomes an ordinary differential equation. Repeating this process constructs the solution interval by interval.

### Characteristic equation of a delay differential equation

↑ **Parent:** [Malthusian delay differential equation](#malthusian-delay-differential-equation)

Substitution of $n(t)=e^{\lambda t}$ into $n'(t)=rn(t-\tau)$ gives the transcendental characteristic equation

$$
\lambda=re^{-\lambda\tau}.
$$

#### Periodic solution of a scalar delay equation

↑ **Parent:** [Characteristic equation of a delay differential equation](#characteristic-equation-of-a-delay-differential-equation)

Purely imaginary characteristic roots produce oscillatory solutions. In particular, $r\tau=-\pi/2$ gives $\lambda=\mathord\pm i\pi/(2\tau)$ and the real solution $\cos(\pi t/(2\tau))$.

#### Stability threshold for delayed quadratic crowding

↑ **Parent:** [Characteristic equation of a delay differential equation](#characteristic-equation-of-a-delay-differential-equation)

For

$$
x'(t)=\alpha\left[x(t)-x(t-T)^2\right],
$$

linearization about $x=1$ gives $u'=\alpha[u(t)-2u(t-T)]$. The equilibrium is stable for

$$
0\leq T<\frac{\pi}{3\sqrt3\alpha}
$$

and loses stability through imaginary roots $\lambda=\mathord\pm i\sqrt3\alpha$ at equality.

#### Delay-independent stability from an undelayed linearization

↑ **Parent:** [Characteristic equation of a delay differential equation](#characteristic-equation-of-a-delay-differential-equation)

For $x'(t)=\alpha x(t-T)[1-x(t)]$, linearization about $x=1$ is $u'=-\alpha u$ because the delayed perturbation appears only in a quadratic term. The equilibrium is therefore locally asymptotically stable for every delay $T\geq0$.

## Epidemic threshold

↑ **Parent:** [Mathematical biology](mathematical-biology.md)

A cross-infection model's disease-free equilibrium becomes a saddle when the product of infection gains exceeds the product of recovery rates.

### Vertical transmission

↑ **Parent:** [Epidemic threshold](#epidemic-threshold)

Infection passed from a parent to its offspring. In a population model, the corresponding infected births remain in the infected compartment rather than entering the susceptible compartment.

### Horizontal transmission

↑ **Parent:** [Epidemic threshold](#epidemic-threshold)

Infection transferred between individuals in the same generation, often modeled by a [law of mass action](#law-of-mass-action) term proportional to susceptible and infected populations. This contrasts with [vertical transmission](#vertical-transmission) from parent to offspring.

## Kramers-Moyal expansion

↑ **Parent:** [Mathematical biology](mathematical-biology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kramers–Moyal_expansion)

The Kramers-Moyal expansion Taylor-expands the gain terms of a jump-process master equation in the jump size. Keeping its first two terms yields a [Fokker-Planck equation](probability-theory.md#fokker-planck-equation) whose drift and diffusion coefficients are the first two infinitesimal jump moments.

### Constant-birth pair-annihilation process

↑ **Parent:** [Kramers-Moyal expansion](#kramers-moyal-expansion)

For jumps $n\to n+1$ at rate $\lambda$ and $n\to n-2$ at rate $\beta n^2$, the diffusion approximation has

$$
A(n)=\lambda-2\beta n^2,
\qquad
B(n)=\lambda+4\beta n^2.
$$

The stable deterministic population is $n_*=\sqrt{\lambda/(2\beta)}$. Its linear-noise stationary approximation is normal with mean $n_*$ and variance $3n_*/4$.

### Kramers-Moyal master equation

↑ **Parent:** [Kramers-Moyal expansion](#kramers-moyal-expansion)

For a jump process with rate $W(n,r)$ from state $n$ to $n+r$, probability balance gives

$$
\partial_tP(n,t)=\sum_r
\big[P(n-r,t)W(n-r,r)-P(n,t)W(n,r)\big].
$$

The first term is inflow from $n-r$ and the second is outflow from $n$.

## Compartmental models (epidemiology)

↑ **Parent:** [Mathematical biology](mathematical-biology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Compartmental_models_(epidemiology))

A compartmental model divides a conserved population into states and uses differential equations for transition rates.

### SIS model

↑ **Parent:** [Compartmental models (epidemiology)](#compartmental-models-epidemiology)

An [SIS model](#sis-model) returns recovered hosts directly to susceptibility, so immunity does not accumulate. For homogeneous frequency-dependent transmission, a positive endemic state exists at $I_*=1-1/\mathcal R_0$ when $\mathcal R_0=\beta/\gamma>1$. This epidemiological model is distinct from the galaxy-dynamics abbreviation SIS for a singular isothermal sphere.

#### Assortatively mixed two-risk-group SIS model

↑ **Parent:** [SIS model](#sis-model)

For high-risk group fraction $p$, fixed total contact rates and reciprocal cross-group contacts, let $C=Bp/(1-p)$. The displayed [SIS model](#sis-model) describes within-group infectious fractions. In fractions the transmission [matrix](vector-space.md#matrix) is $M=\begin{pmatrix}A&B\\C&D-C\end{pmatrix}$; in infected-person counts it is $\operatorname{diag}(p,1-p)M\operatorname{diag}(p,1-p)^{-1}$. A common [recovery rate](#recovery-rate) gives [basic reproduction number](#basic-reproduction-number) $\rho(M)/\gamma$. The [mean](probability-theory.md#expected-value) population susceptible fraction does not generally equal its reciprocal.

##### Small-core SIS endemic expansion

↑ **Parent:** [Assortatively mixed two-risk-group SIS model](#assortatively-mixed-two-risk-group-sis-model)

For fixed $A>\gamma>D$, let $x_0=1-\gamma/A$. The rare high-risk group's [SIS model](#sis-model) has $x=x_0+pB^2\gamma/[A^2(\gamma-D)]+O(p^2)$, whereas low-risk infection is $y=pBx_0/(\gamma-D)+O(p^2)$. Substitution into both [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system) equations proves these coefficients. The leading [basic reproduction number](#basic-reproduction-number) is $A/\gamma$ with correction $pB^2/[\gamma(A-D)]$, while global susceptibility tends to one. These expressions explain why an endemic core can coexist with a large susceptible majority; they are nonuniform when a group is near its own threshold.

#### Homogeneous SIS susceptible fraction

↑ **Parent:** [SIS model](#sis-model)

For $\dot i=\beta i(1-i)-\gamma i$, a positive [endemic equilibrium](#endemic-equilibrium) requires $R_0=\beta/\gamma>1$ and gives susceptible fraction $s_*=\gamma/\beta$. Below threshold the disease-free susceptible fraction is one. The reciprocal relation is a property of this homogeneous scalar [SIS model](#sis-model), not a universal identity for heterogeneous populations.

#### Cooperative SIS coinfection threshold

↑ **Parent:** [SIS model](#sis-model)

For two otherwise symmetric [SIS models](#sis-model) with recovery rate $\gamma$, primary transmission $\beta$ and secondary susceptibility multiplier $q$, split hosts into uninfected, singly infected and doubly infected classes. The displayed conditions give stable disease-free and joint endemic states, with an intermediate saddle: a strong [Allee effect](#allee-effect). The endemic susceptible fraction solves $(q-1)S^2-qS+\mathcal R_0^{-2}=0$. The smaller root is the stable high-prevalence state. Coinfected hosts recover each infection independently, so recovery from coinfection leads to a single-infection class rather than directly to complete susceptibility.

### Conservation of population

↑ **Parent:** [Compartmental models (epidemiology)](#compartmental-models-epidemiology)

If every transition transfers individuals between compartments without births, deaths, immigration, or emigration, the sum of all compartment sizes is constant.

### Prevalence

↑ **Parent:** [Compartmental models (epidemiology)](#compartmental-models-epidemiology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prevalence)

Disease prevalence is the proportion of a population that is infected at a specified time. In a susceptible-infective model with total population $N=S+I$, it is $\theta=I/N$.

### SI model

↑ **Parent:** [Compartmental models (epidemiology)](#compartmental-models-epidemiology)

The SI model divides a closed population into susceptible and permanently infectious compartments. Under frequency-dependent homogeneous mixing,

$$
\dot S=-\beta SI/N,
\qquad
\dot I=\beta SI/N,
$$

and [conservation of population](#conservation-of-population) gives $S+I=N$.

#### Uniform almost-sure fluid limit of the SI model

↑ **Parent:** [SI model](#si-model)

The stochastic [SI model](#si-model) with susceptible fraction $X_n$, initial limit $a$, and total infection rate $n\lambda X_n(1-X_n)$ has deterministic limit

$$
x(t)=\frac{ae^{-\lambda t}}{1-a+ae^{-\lambda t}}.
$$

The [Poisson time-change representation of a Markov chain](markov-process.md#poisson-time-change-representation-of-a-markov-chain) writes $X_n$ as its integrated drift minus a centered Poisson error. On $[0,T]$ its clock is at most $n\lambda T/4$. The [Poisson maximal concentration bound](probability-theory.md#poisson-maximal-concentration-bound) makes every fixed error tolerance have summable probabilities in $n$, so the [Borel-Cantelli lemma](probability-theory.md#borel-cantelli-lemmas) gives uniform error decay [almost surely](convergence-of-random-variables.md#almost-sure-convergence). The [Gronwall inequality](probability-and-statistics.md#gronwall-inequality) transfers that decay to $X_n-x$, because the drift is [Lipschitz continuous](real-analysis.md#lipschitz-continuity). The assertion is for fixed finite intervals and does not claim approximation over times growing with $n$.

#### Logistic solution of the SI model

↑ **Parent:** [SI model](#si-model)

If $S(0)=N\theta/(1+\theta)$ and $I(0)=N/(1+\theta)$, then

$$
I(t)=\frac{N}{1+\theta e^{-\beta t}},
\qquad
\dot I(t)=\frac{N\beta\theta e^{-\beta t}}{(1+\theta e^{-\beta t})^2}.
$$

After centering time at the incidence peak $t_*=\beta^{-1}\log\theta$, the incidence curve is $N\beta/[4\cosh^2\{\beta(t-t_*)/2\}]$.

#### Plant SI model with logistic total population

↑ **Parent:** [SI model](#si-model)

The plant-disease model

$$
\dot S=(S+I)(1-S)-\beta IS,
\qquad
\dot I=-(S+I)I+\beta IS
$$

has total population $N=S+I$ and [disease prevalence](#prevalence) $\theta=I/N$ satisfying

$$
\dot N=N(1-N),
\qquad
\dot\theta=\theta\{\beta N(1-\theta)-1\}.
$$

Thus infection does not alter total-population growth. The invasion threshold at the carrying capacity $N=1$ is $\beta=1$.

##### Uniform per-capita culling in the plant SI model

↑ **Parent:** [Plant SI model with logistic total population](#plant-si-model-with-logistic-total-population)

Removing susceptible and infected plants at the same per-capita rate $k$ changes the reduced equations to

$$
\dot N=N(1-k-N),
\qquad
\dot\theta=\theta\{\beta N(1-\theta)-1\}.
$$

For $0\leq k<1$, the surviving population has carrying capacity $1-k$, and infection invades precisely when $\beta(1-k)>1$.

### SEIR model

↑ **Parent:** [Compartmental models (epidemiology)](#compartmental-models-epidemiology)

The SEIR model divides a population into susceptible, exposed, infectious, and recovered compartments.

#### Force of infection

↑ **Parent:** [SEIR model](#seir-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Force_of_infection)

The force of infection is the instantaneous infection hazard experienced by a susceptible individual. Under homogeneous frequency-dependent mixing it is $\beta I(t)/N$.

#### Final size relation for an epidemic

↑ **Parent:** [SEIR model](#seir-model)

For a closed homogeneous epidemic, integrating $dS/dR$ relates the ultimately susceptible population to cumulative infections through an exponential equation.

The relation constrains the final outcome of [compartmental models](#compartmental-models-epidemiology) rather than describing their whole time-dependent solution.

### SIR model

↑ **Parent:** [Compartmental models (epidemiology)](#compartmental-models-epidemiology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/SIR_model)

The SIR model divides a closed population into susceptible, infectious, and recovered compartments. Infection transfers people from $S$ to $I$, and recovery transfers them from $I$ to $R$.

#### Farm-size stratified SIR model

↑ **Parent:** [SIR model](#sir-model)

Here $s(n)$ and $i(n)$ weight susceptibility and infectiousness of a farm with $n$ animals, with size distribution $P_n$ and recovery rate $\gamma$. The rank-one next-generation matrix has reproduction number $\mathcal R_0=(\beta/\gamma)\sum_n s(n)i(n)P_n$. Susceptibility proportional to size preferentially depletes large susceptible farms. Infectivity heterogeneity alone leaves an exactly homogeneous aggregate SIR trajectory for representative initial infections. When both weights equal size, the second rather than first size moment governs invasion.

#### Discrete SIR epidemic on a graph

↑ **Parent:** [SIR model](#sir-model)

In this discrete-time [SIR model](#sir-model), each infected [vertex](graph.md#vertex-graph-theory) is infectious for one step, can infect each susceptible [neighbour](graph-theory.md#neighbour-of-a-vertex) with probability $\beta$, and is then permanently removed. The [adjacency matrix of a graph](graph-theory.md#adjacency-matrix) describes the possible transmissions. If the initial removed set is empty, eventual removal and ever becoming infected are the same event.

##### Adjacency-matrix bound for a discrete SIR epidemic

↑ **Parent:** [Discrete SIR epidemic on a graph](#discrete-sir-epidemic-on-a-graph)

The conditional [union bound](probability-inequality.md#boole-s-inequality) gives $\mathbb EX_i(k+1)\leq\beta\sum_jA_{ij}\mathbb EX_j(k)$ in a [discrete SIR epidemic on a graph](#discrete-sir-epidemic-on-a-graph). Iteration bounds the infection vector at step $k$ by $(\beta A)^kX(0)$. Each [vertex](graph.md#vertex-graph-theory) is infected at most once, so summing the probabilities in time gives the displayed bound. Powers of the [adjacency matrix of a graph](graph-theory.md#adjacency-matrix) count [walks](graph-theory.md#walk-in-a-graph), which can overcount impossible reinfections without invalidating the upper bound. Initially removed individuals must be counted separately when bounding all eventual removals.

###### Resolvent bound for a discrete SIR epidemic

↑ **Parent:** [Adjacency-matrix bound for a discrete SIR epidemic](#adjacency-matrix-bound-for-a-discrete-sir-epidemic)

When $\beta\rho(A)<1$, summing the [adjacency-matrix bound for a discrete SIR epidemic](#adjacency-matrix-bound-for-a-discrete-sir-epidemic) gives the displayed [Neumann series](banach-algebra.md#neumann-series) bound on the expected total infected count $Z$. For an undirected [graph](graph.md), the [adjacency matrix of a graph](graph-theory.md#adjacency-matrix) is a [symmetric matrix](linear-algebra.md#symmetric-matrix), so its Euclidean [operator norm](continuous-dual-space.md#operator-norm) equals its [spectral radius](analysis.md#spectral-radius). The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) then yields $\mathbb EZ\leq\sqrt{nm}/(1-\beta\rho)$ for $m$ initially infected [vertices](graph.md#vertex-graph-theory).

###### Spectral condition for a small discrete SIR outbreak

↑ **Parent:** [Resolvent bound for a discrete SIR epidemic](#resolvent-bound-for-a-discrete-sir-epidemic)

The displayed condition and the [resolvent bound for a discrete SIR epidemic](#resolvent-bound-for-a-discrete-sir-epidemic) imply $\mathbb EZ=o(n)$. The [Markov inequality](probability-inequality.md#markov-inequality) then makes $Z/n\to0$ in probability. A sufficient special case is a sublinear initial infected count $m=o(n)$ with a fixed positive gap $1-\beta\rho\geq\eta>0$. The inequality $\beta\rho<1$ at each finite population size alone does not control a shrinking gap or an initially macroscopic outbreak.

#### Epidemic threshold for the closed SIR model

↑ **Parent:** [SIR model](#sir-model)

The deterministic [SIR model](#sir-model) with initial susceptible count $S_0$ grows initially exactly when $\beta S_0>\gamma$. Its [basic reproduction number](#basic-reproduction-number) is $\beta S_0/\gamma$ under unnormalized [mass-action infection](#mass-action-infection). If that ratio is at most one, decreasing $S$ prevents later infectious growth.

#### SIR susceptible-recovered identity

↑ **Parent:** [SIR model](#sir-model)

For the closed deterministic [SIR model](#sir-model) with $S(0)=S_0$, $R(0)=0$, infection rate $\beta SI$ and recovery rate $\gamma I$, division of the two flow equations gives $S(t)=S_0e^{-\beta R(t)/\gamma}$. Population conservation then expresses $I$ in terms of $R$.

#### Stochastic SIR model

↑ **Parent:** [SIR model](#sir-model)

The [stochastic SIR model](#stochastic-sir-model) is a [continuous-time Markov chain](markov-process.md#continuous-time-markov-chain) with infection jump $(-1,1,0)$ at rate $\beta SI$ and recovery jump $(0,-1,1)$ at rate $\gamma I$. The state space consists of nonnegative integer compartment counts with conserved total population.

##### Two-event probability in a stochastic SIR model

↑ **Parent:** [Stochastic SIR model](#stochastic-sir-model)

With one initial infectious individual, two events require an infection as the first event. If it occurs at time $s$, its density is $\beta N e^{-(\beta N+\gamma)s}$ and the next total event rate is $2\beta(N-1)+2\gamma$. Integrating this density times the chance of another event before a fixed horizon gives the two-event probability.

##### Chain-binomial epidemic model

↑ **Parent:** [Stochastic SIR model](#stochastic-sir-model)

A [chain-binomial epidemic model](#chain-binomial-epidemic-model) uses discrete time, with conditionally independent [binomial distributions](discrete-probability-distribution.md#binomial-distribution) for infection and recovery counts given the current compartments. It requires valid probability parameters; replacing $1-e^{-\beta I\delta t}$ by $\beta I\delta t$ is a small-step approximation.

### Mass-action interaction

↑ **Parent:** [Compartmental models (epidemiology)](#compartmental-models-epidemiology)

Under mass action, random pairwise encounters between populations of sizes $X$ and $Y$ occur at a rate proportional to $XY$.

### Spatial SIR model

↑ **Parent:** [Compartmental models (epidemiology)](#compartmental-models-epidemiology)

A spatial SIR-type model combines compartment transitions with diffusion in the compartments whose members move appreciably.

#### Mass-action infection

↑ **Parent:** [Spatial SIR model](#spatial-sir-model)

Mass-action transmission at unit nondimensional rate transfers population from susceptible to infected compartments at rate $SI$.

#### Diffusion of infectives

↑ **Parent:** [Spatial SIR model](#spatial-sir-model)

A Laplacian term in the infected-population equation models unbiased random migration of infective individuals.

### Disease-free equilibrium

↑ **Parent:** [Compartmental models (epidemiology)](#compartmental-models-epidemiology)

A disease-free equilibrium is an [equilibrium](dynamical-systems.md#equilibrium-of-an-autonomous-differential-equation) of an epidemic model at which every infected compartment is zero.

### Endemic equilibrium

↑ **Parent:** [Compartmental models (epidemiology)](#compartmental-models-epidemiology)

An endemic equilibrium is an [equilibrium](dynamical-systems.md#equilibrium-of-an-autonomous-differential-equation) at which infection persists, so at least one infected compartment is positive.

### Susceptible-infective model with exponential density-dependent birth

↑ **Parent:** [Compartmental models (epidemiology)](#compartmental-models-epidemiology)

The equations

$$
\dot S=S\left(be^{-aS}-\beta I-d\right),
\qquad
\dot I=I\left(\beta S-d-\delta\right)
$$

combine [mass-action infection](#mass-action-infection) with an [exponential density-dependent birth model](#exponential-density-dependent-birth-model). Susceptibles reproduce at per-capita rate $be^{-aS}$, while infectives have no reproductive term and die at total per-capita rate $d+\delta$.

#### Disease-free equilibrium of the susceptible-infective model with exponential birth

↑ **Parent:** [Susceptible-infective model with exponential density-dependent birth](#susceptible-infective-model-with-exponential-density-dependent-birth)

For $b>d$, the disease-free equilibrium is

$$
(S,I)=\left(\frac1a\log\frac bd,0\right).
$$

It is linearly unstable precisely when

$$
\frac1a\log\frac bd>\frac{d+\delta}{\beta}.
$$

#### Endemic equilibrium of the susceptible-infective model with exponential birth

↑ **Parent:** [Susceptible-infective model with exponential density-dependent birth](#susceptible-infective-model-with-exponential-density-dependent-birth)

When the disease-free equilibrium is unstable, the positive equilibrium satisfies

$$
S^*=\frac{d+\delta}{\beta},
\qquad
\beta I^*+d=be^{-aS^*}.
$$

Its Jacobian has negative trace and positive determinant, so the equilibrium is locally asymptotically stable.

### Basic reproduction number

↑ **Parent:** [Compartmental models (epidemiology)](#compartmental-models-epidemiology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Basic_reproduction_number)

The basic reproduction number $\mathcal R_0$ is the expected number of secondary infections caused by one infective in an otherwise susceptible population.

#### Next-generation matrix

↑ **Parent:** [Basic reproduction number](#basic-reproduction-number)

The entry $K_{ij}$ is the expected number of newly infected type-$i$ individuals produced by a newly infected type-$j$ individual while the population is disease-free. In a compartmental [linearization](algebra.md#linearization), $F$ describes new-infection production and $V$ transitions and removal. Provided the infection-lifetime subsystem is transient, its integrated occupation [matrix](vector-space.md#matrix) is $V^{-1}$, yielding $K=FV^{-1}$. The [basic reproduction number](#basic-reproduction-number) is its [spectral radius](analysis.md#spectral-radius). This construction is described in [the original next-generation-matrix derivation](https://pubmed.ncbi.nlm.nih.gov/19892718/).

##### Susceptible-weighted next-generation matrix

↑ **Parent:** [Next-generation matrix](#next-generation-matrix)

For a heterogeneous [SIS model](#sis-model) with common [recovery rate](#recovery-rate) and a positive [endemic equilibrium](#endemic-equilibrium) $I_*$, force balance gives $\operatorname{diag}(s_*)KI_*=I_*$. When the transmission [matrix](vector-space.md#matrix) is irreducible and nonnegative, the positive [equilibrium](dynamical-systems.md#equilibrium-point-of-a-dynamical-system) vector and the [Perron–Frobenius theorem](vector-space.md#perron-frobenius-theorem) imply the displayed [spectral radius](analysis.md#spectral-radius) identity. It replaces the homogeneous scalar relation $s_*=1/R_0$: different recipient types generally have different susceptible fractions.

#### Epidemic invasion threshold

↑ **Parent:** [Basic reproduction number](#basic-reproduction-number)

A rare infection grows initially when $\mathcal R_0>1$ and decays when $\mathcal R_0<1$.

### SIR model with demography and permanent immunity

↑ **Parent:** [Compartmental models (epidemiology)](#compartmental-models-epidemiology)

With susceptible, infective, and immune populations $X,Y,Z$, equal per-capita birth and death rate $\mu$, mass-action transmission coefficient $\beta$, and recovery rate $\nu$, the equations are

$$
X'=\mu N-\beta XY-\mu X,
\qquad Y'=\beta XY-(\mu+\nu)Y,
\qquad Z'=\nu Y-\mu Z.
$$

The conserved population is $N=X+Y+Z$, and the threshold population is $N_c=(\mu+\nu)/\beta$.

#### Endemic equilibrium of the SIR model with demography

↑ **Parent:** [SIR model with demography and permanent immunity](#sir-model-with-demography-and-permanent-immunity)

When $N>N_c=(\mu+\nu)/\beta$, the positive equilibrium is

$$
X^*=N_c,
\qquad
Y^*=\frac{\mu}{\mu+\nu}(N-N_c),
\qquad
Z^*=\frac{\nu}{\mu+\nu}(N-N_c).
$$

On the invariant plane $X+Y+Z=N$, the $(X,Y)$ Jacobian at this equilibrium has negative trace $-(\mu+\beta Y^*)$ and positive determinant $\beta Y^*(\mu+\nu)$, so both eigenvalues have negative real part and the equilibrium is locally asymptotically stable.

### SIR model with waning immunity

↑ **Parent:** [Compartmental models (epidemiology)](#compartmental-models-epidemiology)

For susceptible, infective, and recovered populations $S,I,R$, mass-action infection coefficient $\beta$, recovery rate $\nu$, and immunity-loss rate $f$, the SIRS equations are

$$
S'=fR-\beta IS,
\qquad I'=\beta IS-\nu I,
\qquad R'=\nu I-fR.
$$

They conserve $S+I+R=N$ and have basic reproduction number $\mathcal R_0=\beta N/\nu$.

#### SIRS Markov chain

↑ **Parent:** [SIR model with waning immunity](#sir-model-with-waning-immunity)

In a closed population of size $n$, a frequency-dependent SIRS epidemic has the displayed transitions at rates $\lambda SI/n$, $\gamma I$, and $\nu R$. The [exponential distribution](continuous-probability-distribution.md#exponential-distribution) of infectious lifetimes and the constant immunity-loss hazard make the compartment counts a [continuous-time Markov chain](markov-process.md#continuous-time-markov-chain). Each jump preserves $S+I+R=n$.

##### Fluid limit of the SIRS Markov chain

↑ **Parent:** [SIRS Markov chain](#sirs-markov-chain)

For convergent initial proportions, the scaled [SIRS Markov chain](#sirs-markov-chain) converges uniformly in probability on each fixed finite interval to the solution of these equations. The [Poisson time-change representation of a Markov chain](markov-process.md#poisson-time-change-representation-of-a-markov-chain) writes it as its integrated drift plus centered Poisson errors. Bounded rates, Poisson concentration and the [Gronwall inequality](probability-and-statistics.md#gronwall-inequality) control the error. This finite-time limit does not by itself justify an approximation over time intervals growing with the population size.

#### Endemic equilibrium of the SIR model with waning immunity

↑ **Parent:** [SIR model with waning immunity](#sir-model-with-waning-immunity)

When $\beta N>\nu$ and $f>0$, the positive equilibrium is

$$
S^*=\frac\nu\beta,
\qquad
I^*=\frac{f(\beta N-\nu)}{\beta(f+\nu)},
\qquad
R^*=\frac{\nu(\beta N-\nu)}{\beta(f+\nu)}.
$$

Writing $a=\beta I^*>0$, the reduced $(S,I)$ Jacobian has characteristic polynomial

$$
\lambda^2+(f+a)\lambda+a(f+\nu).
$$

Both roots have negative real part. Its discriminant is negative for sufficiently small $f$ and positive for sufficiently large $f$, giving respectively a stable focus and a stable node.

## Dispersal with mortality and immobile deposition

↑ **Parent:** [Mathematical biology](mathematical-biology.md)

For diffusing organisms of density $n$ that die at rate $\mu$ and deposit an immobile material of density $e$ at rate $\lambda$,

$$
n_t=Dn_{xx}-\mu n,
\qquad
e_t=\lambda n.
$$

An initial point population $N\delta(x)$ leaves the [remnant density from diffusion with mortality and deposition](#remnant-density-from-diffusion-with-mortality-and-deposition)

$$
e(x,\infty)=\frac{N\lambda}{2\sqrt{D\mu}}e^{-|x|\sqrt{\mu/D}}.
$$

### Remnant density from diffusion with mortality and deposition

↑ **Parent:** [Dispersal with mortality and immobile deposition](#dispersal-with-mortality-and-immobile-deposition)

The remnant profile is the time integral of a decaying [heat kernel](diffusion-equation.md#heat-kernel). Its length scale is $\sqrt{D/\mu}$ and its total mass is $N\lambda/\mu$, the initial population times the mean deposition over an exponential lifetime.

### Diffusion length

↑ **Parent:** [Dispersal with mortality and immobile deposition](#dispersal-with-mortality-and-immobile-deposition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Diffusion_length)

For diffusivity $D$ and removal rate $\mu$, the diffusion length $\sqrt{D/\mu}$ is the characteristic distance travelled before removal.

## Biological fluid dynamics

↑ **Parent:** [Mathematical biology](mathematical-biology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Biological_fluid_dynamics)

Biological fluid dynamics studies flows generated by and acting on organisms, cells, tissues, and biological transport networks.

### Phototaxis

↑ **Parent:** [Biological fluid dynamics](#biological-fluid-dynamics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Phototaxis)

Phototaxis is directed organism motion in response to light. An ideal spherical swimmer subject to light [torque](classical-mechanics.md#torque) $\mathbf p\times\mathbf L$ and rotational resistance $\alpha$ aligns towards the light while ambient [vorticity](fluid-mechanics.md#vorticity) rotates it. Its deterministic orientation satisfies $\dot{\mathbf p}=\boldsymbol\omega\times\mathbf p/2+[\mathbf L-(\mathbf p\cdot\mathbf L)\mathbf p]/\alpha$. The right-hand side is perpendicular to $\mathbf p$ and preserves its unit length.

#### Phototactic concentration in a vertical channel

↑ **Parent:** [Phototaxis](#phototaxis)

In a long channel $-a<x<a$, uniform horizontal mean swimming $V_sK_0\mathbf e_x$ and isotropic translational [diffusion coefficient](brownian-motion.md#diffusion-coefficient) $D$ give zero transverse cell flux when $n'=\beta n$, $\beta=V_sK_0/D$. Normalizing the transverse mean concentration to $n_0$ gives the displayed exponential. For $\beta a\gg1$, cells form a layer of thickness $\beta^{-1}$ at the illuminated wall. This is a bulk approximation; exact closed-end [cell conservation equation](#cell-conservation-in-a-swimming-suspension) also requires the integrated axial cell flux to vanish.

##### Zero-flux pressure gradient in a cell-driven channel

↑ **Parent:** [Phototactic concentration in a vertical channel](#phototactic-concentration-in-a-vertical-channel)

In the [Boussinesq approximation](geophysical-fluid-dynamics.md#boussinesq-approximation), downward excess cell weight gives $\mu w''=G+g'n(x)$. The [no-slip boundary condition](viscous-fluid-flow.md#no-slip-boundary-condition) at both walls and zero total fluid flux determine the excess axial pressure gradient $G$, with $b=a\beta$. In particular, $w=C[e^{\beta x}-\cosh b-(x/a)\sinh b]+G(x^2-a^2)/(2\mu)$, $C=g'n_0a\beta/(\mu\beta^2\sinh b)$. For large $b$, writing $\xi=x/a$ and $W=g'n_0a^2/(\mu b)$ gives the outer profile $w/W=(1+\xi)(1-3\xi)/2$. A thin layer restores no slip at the illuminated wall. Cells descend there and fluid returns upward on the other side. At $b=0$ the limiting solution is $G=-g'n_0$, $w=0$.

#### Phototactic orientation Fokker-Planck equation

↑ **Parent:** [Phototaxis](#phototaxis)

For isotropic [rotational diffusion](thermodynamics.md#rotational-diffusion), orientation drift and [probability density](quantum-mechanics.md#probability-density) obey the displayed [Fokker-Planck equation](probability-theory.md#fokker-planck-equation), normalized with respect to solid angle. Without flow, constant light $L\mathbf e_x$ gives the zero-current density $f_0=\lambda e^{\lambda p_x}/(4\pi\sinh\lambda)$, $\lambda=L/(\alpha D_r)$. Integration over the sphere gives unit mass; its mean projection is the [Langevin function](#langevin-function). The zero-light limit is the uniform density $1/(4\pi)$.

##### Small-vorticity phototactic orientation response

↑ **Parent:** [Phototactic orientation Fokker-Planck equation](#phototactic-orientation-fokker-planck-equation)

For light along $\mathbf e_x$, [vorticity](fluid-mechanics.md#vorticity) along $\mathbf e_y$ and $\varepsilon=\omega/(2D_r)$, spherical coordinates $\mathbf p=(\cos\theta,\sin\theta\cos\phi,\sin\theta\sin\phi)$ give a first orientation-density correction proportional to $\sin\phi\,g(\theta)$. The linearized alignment-diffusion operator preserves azimuthal harmonics and the rotation of the axisymmetric equilibrium forces only this sine harmonic. Angular integration makes the first correction to the mean purely vertical. Uniqueness follows from the weighted identity $\mathcal A(f_0h)=\nabla_p\cdot(f_0\nabla_ph)$: [integration by parts](calculus.md#integration-by-parts) shows the only homogeneous smooth solution is a multiple of $f_0$, removed by normalization.

### Bioconvection

↑ **Parent:** [Biological fluid dynamics](#biological-fluid-dynamics)

Bioconvection is buoyancy-driven fluid motion generated by a nonuniform concentration of swimming microorganisms. Upward swimming can create a dense upper layer, while a disturbance redistributes the cells and drives overturning. A [cell conservation equation](#cell-conservation-in-a-swimming-suspension) coupled to incompressible [Newtonian fluid](viscous-fluid-flow.md#newtonian-fluid) dynamics describes its linear stability under an appropriate dilute-suspension approximation.

#### Long-wave bioconvection threshold in weak stratification

↑ **Parent:** [Bioconvection](#bioconvection)

For upward swimming with $h=V_sH/D\to0$, no-slip impermeable plates, and stationary long-wave modes with horizontal [wavenumber](wave-equation.md#wavenumber) $\kappa=h\kappa'\ne0$, the leading concentration mode is constant and the vertical [velocity](classical-mechanics.md#velocity) mode is $W_0=-\kappa'^2R_0z^2(z+1)^2/24$. The next concentration solvability condition is $\kappa'^2+\int_{-1}^0W_0dz=0$. Since $\int z^2(z+1)^2dz=1/30$, this gives $R_0=720$, independently of the leading gyrotactic parameter. The exactly uniform horizontal mode $\kappa'=0$ instead changes conserved total cell number and does not select the instability threshold.

##### Clamped-quartic solvability in shallow bioconvection

↑ **Parent:** [Long-wave bioconvection threshold in weak stratification](#long-wave-bioconvection-threshold-in-weak-stratification)

For the constant leading cell-concentration mode normalized to one, the leading vertical [velocity](classical-mechanics.md#velocity) mode in shallow long-wave [bioconvection](#bioconvection) solves $W_1^{(4)}=-R_0\alpha^2$ and $W_1=W_1'=0$ at both $z=0,1$. The displayed quartic satisfies all four conditions and is unique because a homogeneous cubic with those conditions is zero. Its integral is $-R_0\alpha^2/720$. The next cell-conservation solvability condition is $\alpha^2+\sigma_2=-\int W_1dz$, hence $\sigma_2=\alpha^2(R_0/720-1)$. The leading threshold is independent of the distinguished leading gyrotactic coefficient; a horizontally uniform conservation mode does not select it.

### Cell conservation in a swimming suspension

↑ **Parent:** [Biological fluid dynamics](#biological-fluid-dynamics)

If $C$ is the cell number density, $\mathbf u$ the fluid [velocity](classical-mechanics.md#velocity), $V_s\langle\mathbf p\rangle$ the mean swimming [velocity](classical-mechanics.md#velocity), and $D$ an isotropic translational [diffusion](thermodynamics.md#diffusion) coefficient, conservation is $\partial_tC+\nabla\cdot[C(\mathbf u+V_s\langle\mathbf p\rangle)-D\nabla C]=0$. Impermeable boundaries have zero normal total cell flux. For constant cell volume $v$, the volume fraction is $vC$ and obeys the same equation, but its buoyancy coefficient has no additional factor $v$.

#### Closed-channel cell-flux constraint

↑ **Parent:** [Cell conservation in a swimming suspension](#cell-conservation-in-a-swimming-suspension)

A genuinely closed steady channel with impermeable sidewalls and ends must have zero integrated axial cell flux through every section, not only zero fluid flux. In the bulk phototactic ansatz $n'=\beta n$, $\omega_y=-w'$, and $\langle p_z\rangle=-K_1w'/(2D_r)$, the axial flux is $[1+V_s\beta K_1/(2D_r)]\int nw\,dx$. Meanwhile the momentum equation, zero fluid flux and [integration by parts](calculus.md#integration-by-parts) give $g'\int nw\,dx=-\mu\int(w')^2dx$. Thus a nontrivial bulk profile is generally incompatible with exact closed-end cell conservation unless the prefactor vanishes. Additional axial concentration variation is needed; neglecting end regions does not itself remove this global constraint.

### Gyrotaxis

↑ **Parent:** [Biological fluid dynamics](#biological-fluid-dynamics)

Gyrotaxis is the orientation response of swimming cells to the competition between gravity-induced [torque](classical-mechanics.md#torque) and fluid rotation. A bottom-heavy spherical cell tends to point upward in still fluid, while ambient [vorticity](fluid-mechanics.md#vorticity) rotates it. The response changes the mean swimming direction and can focus cells or contribute to [bioconvection](#bioconvection).

#### Gyrotactic focusing in a downward pipe flow

↑ **Parent:** [Gyrotaxis](#gyrotaxis)

For a bottom-heavy spherical swimmer in axial flow $u_z=W_0(-1+r^2+w)$, the [bottom-heavy spherical-cell orientation dynamics](#bottom-heavy-spherical-cell-orientation-dynamics) with aligning rate $1/B$ gives $\sin\theta=-\lambda(2r+w')$, $\lambda=BW_0/(2R)$. On the upward-stable branch $\cos\theta>0$, the cells tilt inward in a downward [Poiseuille flow](viscous-fluid-flow.md#hagen-poiseuille-equation). Zero radial cell flux with scalar [diffusivity](brownian-motion.md#diffusion-coefficient) gives $n'=\chi n\sin\theta$, $\chi=V_cR/D$. For $w=0$, integration and the average normalization $2\int_0^1nr\,dr=1$ give the displayed concentration. A steady deterministic orientation requires $|\lambda(2r+w')|<1$; beyond this shear threshold the stationary orientation closure fails.

##### Stresslet correction to gyrotactic pipe flow

↑ **Parent:** [Gyrotactic focusing in a downward pipe flow](#gyrotactic-focusing-in-a-downward-pipe-flow)

Let weak excess-cell buoyancy be $\gamma\ll1$ and the swimming [stresslet](stokes-flow.md#force-dipole-flow) coefficient be $\sigma=\gamma\sigma_1$. Set $w=\gamma w_1$ and use the leading [gyrotactic focusing in a downward pipe flow](#gyrotactic-focusing-in-a-downward-pipe-flow) density $n_0=Ae^{-ar^2}$. With active stress entering as $+Sn\mathbf p\mathbf p$, the axial momentum equation integrates from the regular axis to the displayed derivative. The wall condition gives $w_1(r)=-\int_r^1w_1'(s)ds$. Both terms of the integrand are positive for $\sigma_1\geq0$, so the correction increases downward flow. A negative stresslet strength can oppose this effect; reversal at a given radius requires $\sigma_1$ smaller than minus the ratio of the integrated buoyancy and stresslet coefficients. This convention must be specified before attaching extensile or contractile sign labels.

#### Gyrotactic circular paths in a rotating cylinder

↑ **Parent:** [Gyrotaxis](#gyrotaxis)

For fluid [velocity](classical-mechanics.md#velocity) $\Omega(-x_3,0,x_1)$ and $B\Omega<1$, the stable deterministic orientation is $\mathbf p=(-B\Omega,0,\sqrt{1-B^2\Omega^2})$. Once this orientation has relaxed, swimming at speed $V_s$ shifts the centre of the circular material trajectories to $(-V_s\sqrt{1-B^2\Omega^2}/\Omega,-V_sB)$ in the $(x_1,x_3)$ plane. Its distance from the cylinder axis is $V_s/\Omega$. General initial orientations produce an orientation transient before these circular paths.

#### Gyrotactic orientation Fokker-Planck equation

↑ **Parent:** [Gyrotaxis](#gyrotaxis)

For orientation [probability density](quantum-mechanics.md#probability-density) $f$ on the unit sphere, deterministic drift $\dot{\mathbf p}$ and isotropic rotational [diffusion](thermodynamics.md#diffusion) coefficient $D_R$ give $\partial_tf+\nabla_p\cdot(f\dot{\mathbf p}-D_R\nabla_pf)=0$. The derivatives are tangential to the sphere, and normalization is $\int f\,d\Omega=1$. The spherical divergence of $\mathbf k-p_3\mathbf p$ is $-2p_3$.

##### Zero-flow steady gyrotactic orientation distribution

↑ **Parent:** [Gyrotactic orientation Fokker-Planck equation](#gyrotactic-orientation-fokker-planck-equation)

For aligning rate $1/B$, positive rotational [diffusivity](brownian-motion.md#diffusion-coefficient) $D_r$ and $\Lambda=(BD_r)^{-1}$, the zero-current steady [Fokker-Planck equation](probability-theory.md#fokker-planck-equation) gives $f_{0,\theta}=-\Lambda\sin\theta f_0$. Normalization over the unit sphere gives the displayed density per unit solid angle. Its mean direction is $\langle\mathbf p\rangle=(\coth\Lambda-1/\Lambda)\mathbf k$, the [Langevin function](#langevin-function). As $BD_r\to0$, it concentrates weakly into a point mass at the upward pole; the limit is not an ordinary bounded probability density.

##### Rapid-rotation mean gyrotactic orientation

↑ **Parent:** [Gyrotactic orientation Fokker-Planck equation](#gyrotactic-orientation-fokker-planck-equation)

For rigid fluid rotation with [vorticity](fluid-mechanics.md#vorticity) $-2\Omega\mathbf e_2$, $B\Omega\gg1$, and $BD_R$ of order one, the normalized steady density is $f=(4\pi)^{-1}[1-2p_1/(B\Omega)]+O((B\Omega)^{-2})$. The result follows by acting with the rotation generator on $p_1$ and using $\int p_i p_jd\Omega=4\pi\delta_{ij}/3$. Reversing the imposed rotation reverses the mean horizontal swimming direction.

###### Gyrotactic concentration layer at a rotating-cylinder wall

↑ **Parent:** [Rapid-rotation mean gyrotactic orientation](#rapid-rotation-mean-gyrotactic-orientation)

With $\beta^2=\Omega R^2/D$ and $\varepsilon=2V_sR/(3B\Omega D)$, the first angular harmonic of the steady [cell conservation equation](#cell-conservation-in-a-swimming-suspension) satisfies $a''+a'/r-a/r^2-i\beta^2a=0$ and $a'(1)=-1$. The regular solution is $a=-I_1(qr)/[qI_1'(q)]$, $q=e^{i\pi/4}\beta$. At large $\beta$ it gives the displayed layer with width $1/\beta$. The exact [Modified Bessel function of the first kind](analysis.md#modified-bessel-function-of-the-first-kind) expression remains regular at the axis, unlike extrapolation of the boundary-layer formula there.

#### Bottom-heavy spherical-cell orientation dynamics

↑ **Parent:** [Gyrotaxis](#gyrotaxis)

For a spherical cell with its [centre of mass](classical-mechanics.md#center-of-mass) displaced by $-\ell_g\mathbf p$ from its geometric centre, gravity produces [torque](classical-mechanics.md#torque) $mg\ell_g\mathbf p\times\mathbf k$. Rotational resistance $\zeta_r$ gives angular [velocity](classical-mechanics.md#velocity) $\boldsymbol\omega/2+(mg\ell_g/\zeta_r)\mathbf p\times\mathbf k$. Taking its cross product with $\mathbf p$ gives the displayed orientation equation with $B=\zeta_r/(mg\ell_g)$. Steady orientation therefore requires the two terms on the right to sum to zero; placing the [vorticity](fluid-mechanics.md#vorticity) term alone on the other side changes its sign.

##### Quasistatic gyrotactic balance with half-rate reorientation

↑ **Parent:** [Bottom-heavy spherical-cell orientation dynamics](#bottom-heavy-spherical-cell-orientation-dynamics)

This convention defines the [gyrotactic reorientation time](#gyrotactic-reorientation-time) by an aligning rate $1/(2B)$. Multiplying the [torque](classical-mechanics.md#torque) balance by $2B$ and perturbing about the upward direction gives $\mathbf p_\perp=B\boldsymbol\omega\times\mathbf e_z$. For an [incompressible flow](fluid-mechanics.md#incompressible-flow), its horizontal [divergence](calculus.md#divergence) is $-B\nabla^2w$, because $\nabla\times\boldsymbol\omega=-\nabla^2\mathbf u$. The parameter $B$ is half the reorientation parameter used in the convention with aligning rate $1/B$; writing the governing equation prevents a factor-of-two ambiguity.

##### Deterministic alignment of an initially isotropic orientation distribution

↑ **Parent:** [Bottom-heavy spherical-cell orientation dynamics](#bottom-heavy-spherical-cell-orientation-dynamics)

Without rotational [diffusion](thermodynamics.md#diffusion), $x=p_z$ follows $\dot x=(1-x^2)/B$, hence $x=(x_0+\tanh(t/B))/(1+x_0\tanh(t/B))$. Pushing forward the initial uniform orientation distribution gives $f=\alpha/[\pi(1+\alpha-(1-\alpha)x)^2]$, $\alpha=e^{-2t/B}$, per unit solid angle. Integrating $2\pi xf$ yields the displayed mean, interpreted continuously as zero at $t=0$. Its late deficit is $(4t/B-2)e^{-2t/B}+O((t/B)e^{-4t/B})$. At each finite time the density is smooth and normalized; the infinitely late distribution is a point mass at the upward pole.

##### Gyrotactic reorientation time

↑ **Parent:** [Bottom-heavy spherical-cell orientation dynamics](#bottom-heavy-spherical-cell-orientation-dynamics)

In the convention with aligning rate $1/B$, the tilt angle in still fluid obeys $\dot\theta=-\sin\theta/B$, so $\tan(\theta/2)$ decays as $e^{-t/B}$. Some conventions instead put $1/(2B)$ in the orientation equation; their parameter has a different factor of two. Specify the dynamical equation when comparing reorientation times.

###### Weak-noise relaxation of gyrotactic alignment

↑ **Parent:** [Gyrotactic reorientation time](#gyrotactic-reorientation-time)

Close to the upward pole, the two Cartesian tilt components of [bottom-heavy spherical-cell orientation dynamics](#bottom-heavy-spherical-cell-orientation-dynamics) obey the displayed [Ornstein-Uhlenbeck process](stochastic-process.md#ornstein-uhlenbeck-process). Thus $d\langle|\mathbf q|^2\rangle/dt=-2\langle|\mathbf q|^2\rangle/B+4D_r$. The stationary spread is $2BD_r$, and late axisymmetric variance perturbations relax on $B/2$ in this weak-noise approximation. The zero-noise mean from [deterministic alignment of an initially isotropic orientation distribution](#deterministic-alignment-of-an-initially-isotropic-orientation-distribution) has the same exponential scale but a different transient prefactor. Reaching a tiny diffusion-supported mean-deficit floor $BD_r$ from an initially isotropic population takes order $B\log[(BD_r)^{-1}]$, with logarithmic corrections. Equality of limiting mean directions does not make the full transients identical, and the alignment time is not automatically the pure rotational-diffusion time $D_r^{-1}$.

### Lighthill elongated-body theory

↑ **Parent:** [Biological fluid dynamics](#biological-fluid-dynamics)

In the small-amplitude [slender-body theory](stokes-flow.md#slender-body-theory) approximation, an undulating swimmer accelerates an [added mass](physics.md#added-mass) of fluid per unit length $m(x)$. With $\mathcal D=\partial_t+U\partial_x$ and transverse displacement $h$, the lateral [force](classical-mechanics.md#force) on the body is $-\mathcal D(m\mathcal Dh)$. Its reaction on the fluid has the opposite sign. For a periodic stroke and the usual negligible leading-edge added-mass contribution, the mean trailing-edge thrust is $m\langle h_t^2-U^2h_x^2\rangle/2$. This is a reactive inertial model, distinct from viscous [resistive-force theory](#resistive-force-theory).

#### Active bending beam for a swimming fish

↑ **Parent:** [Lighthill elongated-body theory](#lighthill-elongated-body-theory)

An active swimming beam has a total internal [bending moment](continuum-mechanics.md#bending-moment) $G$ containing passive elasticity and muscular actuation. Neglecting cross-sectional rotary inertia, slice [angular momentum](classical-mechanics.md#angular-momentum) balance identifies the internal transverse force with $G_x$. Slice [linear momentum](classical-mechanics.md#momentum) balance then gives $G_{xx}=m_bh_{tt}-F_{\rm body}$. In [Lighthill elongated-body theory](#lighthill-elongated-body-theory), $F_{\rm body}=-\mathcal D(m\mathcal Dh)$, where $\mathcal D=\partial_t+U\partial_x$. The body and its hydrodynamic [added mass](physics.md#added-mass) therefore contribute with the same sign to the acceleration coefficient. The positive quantity $\mathcal D(m\mathcal Dh)$ is the reaction on the fluid.

#### Recoil correction in elongated-body theory

↑ **Parent:** [Lighthill elongated-body theory](#lighthill-elongated-body-theory)

A deforming free swimmer must satisfy total linear and angular [momentum](classical-mechanics.md#momentum) balances. The unknown lateral translation and yaw are its recoil correction. If the reference translation is the true [centre of mass](classical-mechanics.md#center-of-mass), the prescribed deformation must first have its mass-weighted mean removed. Otherwise the reference translation differs from actual [centre of mass](classical-mechanics.md#center-of-mass) displacement. The body [mass](classical-mechanics.md#mass) and its hydrodynamic [added mass](physics.md#added-mass) contribute with the same sign to its effective inertial coefficient.

##### Quadratic-bend turning with finite body mass

↑ **Parent:** [Recoil correction in elongated-body theory](#recoil-correction-in-elongated-body-theory)

Put $B_j=[m(x)(x-\bar x)^j]_0^L$, $M_j=\int m(x)(x-\bar x)^jdx$, $A=\int\alpha(t)dt$, and $C=B_0(B_2-M_1)-B_1(B_1-M_0)$. For quadratic bending $h_0=-\alpha(t)(x-\bar x)^2$, the linear [recoil correction in elongated-body theory](#recoil-correction-in-elongated-body-theory) with a stable post-stroke relaxation gives the displayed angle. It follows by setting time [derivatives](calculus.md#derivative) to zero in the integrated lateral and [angular momentum](classical-mechanics.md#angular-momentum) equations. The simpler $2UA$ is exact in the zero-body-mass limit, or when $B_1=M_0$, but is not a generic finite-body-mass identity. For $L=1$, $\bar x=1/2$, and $m(x)=m_*x^2$, it becomes $2UA/(1+2M_b/m_*)$. Body deformation inertia affects [derivative](calculus.md#derivative) forcing during the stroke, not this final integral relation when the deformation and its time [derivative](calculus.md#derivative) return to zero.

##### Endpoint momentum flux in elongated-body recoil

↑ **Parent:** [Recoil correction in elongated-body theory](#recoil-correction-in-elongated-body-theory)

With $r=x-\bar x$, lateral relative [velocity](classical-mechanics.md#velocity) $w=(\partial_t+U\partial_x)h$, $Q=\int mw\,dx$ and $P=\int rmw\,dx$, the [Lighthill elongated-body theory](#lighthill-elongated-body-theory) [force](classical-mechanics.md#force) on the fluid is $F_z=(\partial_t+U\partial_x)(mw)$. [Integration by parts](calculus.md#integration-by-parts) gives $\int F_zdx=\dot Q+U[mw]_0^L$ and $\int rF_zdx=\dot P+U[rmw]_0^L-UQ$. The endpoint terms are [momentum](classical-mechanics.md#momentum) fluxes and must not be discarded when a tail has nonzero [added mass](physics.md#added-mass). If both endpoint added masses vanish, total lateral body-plus-fluid [momentum](classical-mechanics.md#momentum) is conserved; a finite-mass body cannot then finish with zero relative crossflow and a new nonzero transverse [velocity](classical-mechanics.md#velocity).

##### Free-end compatibility for a swimming beam

↑ **Parent:** [Recoil correction in elongated-body theory](#recoil-correction-in-elongated-body-theory)

For $G_{xx}=R$, zero [bending moment](continuum-mechanics.md#bending-moment) and transverse force at the leading end give $G(x)=\int_0^x(x-s)R(s)\,ds$. The two trailing-end [free-end bending boundary conditions](continuum-mechanics.md#free-end-bending-boundary-conditions) hold exactly when the displayed two integrals vanish. They express total transverse force and [torque](classical-mechanics.md#torque) balance. Adding unknown rigid translation and yaw to a prescribed deformation supplies the two degrees of freedom of the [swimming recoil correction](#recoil-correction-in-elongated-body-theory). Its principal inertial matrix is the weighted moment matrix of $1$ and $x-x_c$ with weight $m_b+m$, hence is positive definite for a nondegenerate positive mass distribution.

### Volvox

↑ **Parent:** [Biological fluid dynamics](#biological-fluid-dynamics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Volvox)

Volvox is a genus of spherical colonial green algae whose flagella propel the colony through water. A colony hovering below a free surface exerts a net gravitational point force on the surrounding fluid.

#### Hydrodynamic attraction of hovering Volvox colonies

↑ **Parent:** [Volvox](#volvox)

Two bottom-heavy Volvox colonies hovering at equal depth below a stress-free surface are drawn together by the image flow of their downward Stokeslets. At large separation $x$, their relative speed scales as $-x^{-2}$ and their collision time scales as $x_0^3$.

### Microcirculation

↑ **Parent:** [Biological fluid dynamics](#biological-fluid-dynamics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Microcirculation)

Microcirculation is blood flow through arterioles, capillaries, and venules, where vessel dimensions are comparable with cellular length scales.

<h4 id="murray-s-law">Murray's law</h4>

↑ **Parent:** [Microcirculation](#microcirculation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Murray's_law)

Murray's law balances viscous pumping power against the metabolic cost of maintaining blood volume. For cylindrical vessels it gives $Q\propto R^3$ and hence $R_0^3=R_1^3+R_2^3$ at an ideal bifurcation.

<h4 id="fahraeus-lindqvist-effect">Fahraeus--Lindqvist effect</h4>

↑ **Parent:** [Microcirculation](#microcirculation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fahraeus--Lindqvist_effect)

The Fahraeus--Lindqvist effect is the reduction of blood's apparent viscosity as a small vessel narrows over much of the microvascular range. Red blood cells migrate toward the centre and leave a relatively low-viscosity cell-free plasma layer near the wall.

##### Cell-free layer

↑ **Parent:** [Fahraeus--Lindqvist effect](#fahraeus-lindqvist-effect)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cell-free_layer)

A cell-free layer is a near-wall region of plasma depleted of suspended blood cells. Because plasma is less viscous than the cell-rich core, the layer can substantially reduce hydraulic resistance.

<h4 id="zweifach-fung-effect">Zweifach--Fung effect</h4>

↑ **Parent:** [Microcirculation](#microcirculation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Zweifach--Fung_effect)

The Zweifach--Fung effect, or plasma skimming, is the disproportionate entry of red blood cells into the higher-flow daughter at an asymmetric microvascular bifurcation.

### Cytoplasmic streaming

↑ **Parent:** [Biological fluid dynamics](#biological-fluid-dynamics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cytoplasmic_streaming)

Cytoplasmic streaming is directed cytoplasmic flow within a cell, often driven by molecular motors acting along the boundary and used to enhance intracellular transport.

### Resistive-force theory

↑ **Parent:** [Biological fluid dynamics](#biological-fluid-dynamics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Resistive-force_theory)

Resistive-force theory approximates the local viscous force on a slender filament by separate drag coefficients multiplying its velocity components parallel and perpendicular to the tangent.

#### Shear-dependent settling of a sphere-and-tail body

↑ **Parent:** [Resistive-force theory](#resistive-force-theory)

For a heavy spherical head with a much thinner long rigid tail, let $P$ be its excess weight, $H=6\pi\mu a$ the head translation resistance, and $K=K_NL$ the tail normal translation resistance. Neglect tail [mass](classical-mechanics.md#mass) relative to head [mass](classical-mechanics.md#mass), sphere rotation resistance relative to tail rotation resistance, and $a/L$ in tail lever arms. In shear $\alpha z\mathbf e_1$, the stable orientation satisfies $\sin\theta=\alpha/(\beta+\sqrt{\beta^2+\alpha^2})$, $\cos\theta>0$, with $\beta=3P/[L(K+4H)]$. Resolving [resistive-force theory](#resistive-force-theory) [force](classical-mechanics.md#force) and [torque](classical-mechanics.md#torque) balance gives the displayed signed vertical [velocity](classical-mechanics.md#velocity). Since $0<\gamma<1$, stronger shear increases $U_z$ towards zero and reduces the downward settling speed. The stable head is below the far tail end. Very large shear can make the neglected sphere-rotation contribution significant.

#### Linear resistive-force propulsion of a travelling filament

↑ **Parent:** [Resistive-force theory](#resistive-force-theory)

For a periodic [inextensible filament](#inextensible-filament), let $q=\mathbf t\cdot\mathbf i$, $\alpha=\langle q\rangle=V/c$, $\beta=\langle q^2\rangle$ and $\gamma=\kappa_T/\kappa_N$. The material velocity is $(V-U)\mathbf i-c\mathbf t$. Applying the linear local drag tensor $\kappa_T\mathbf t\mathbf t+\kappa_N(I-\mathbf t\mathbf t)$ gives thrust $T=\kappa_NL\{V(1-\gamma)(1-\beta)-U[1-(1-\gamma)\beta]\}$. Equating this to head drag $\delta\kappa_NLU$ gives the displayed speed ratio. Whole spatial periods, or period averages, are needed for $c\int q\,ds=VL$. [Cauchy-Schwarz](probability-and-statistics.md#cauchy-schwarz-inequality) gives $\alpha^2\leq\beta$, with equality only for constant axial tangent projection almost everywhere.

##### Fixed-speed energy optimum for a planar flagellum

↑ **Parent:** [Linear resistive-force propulsion of a travelling filament](#linear-resistive-force-propulsion-of-a-travelling-filament)

In [resistive-force theory](#resistive-force-theory) with $0<\gamma<1$, head drag $\delta\geq0$ and the ideal constant-inclination condition $\alpha^2=\beta$, put $r=1-\gamma$, $d=1+\delta$, $A=r(\delta^2-\gamma)$ and $B=\gamma d^2$. At prescribed swimming speed $U$, eliminating wave speed using [linear resistive-force propulsion of a travelling filament](#linear-resistive-force-propulsion-of-a-travelling-filament) gives

$$
\frac{E}{\kappa_NLU^2}=\frac{(d-r\beta)(\gamma d+\delta r\beta)}{r^2\beta(1-\beta)}.
$$

Its derivative has numerator $A\beta^2+2B\beta-B$. This numerator is strictly increasing on $(0,1)$, is negative at zero, and equals $(\delta+\gamma)^2$ at one. Thus its unique zero is the displayed global minimum. When $A=0$ the formula gives $\beta_*=1/2$; when $\delta=0$ it gives $1/(1+\sqrt\gamma)$. A planar sawtooth realizes constant inclination in the ideal model; smooth rounding and elastic costs change that idealization.

#### Nonlinear resistive-force balance for a travelling filament

↑ **Parent:** [Resistive-force theory](#resistive-force-theory)

For an inextensible planar filament with tailward tangent $\mathbf t=(X_s,Y_s)$, a travelling shape has material velocity $(V-U)\mathbf i-c\mathbf t$ in stationary fluid. Thus the relative fluid velocity is the displayed vector. With $\mathbf n=(-Y_s,X_s)$ and $q=V-U>0$, a local inertial normal [drag](fluid-mechanics.md#drag-physics) $K_N|w_n|w_n\mathbf n$ has axial component $-K_Nq^2|Y_s|^3$. A positive tangential slip $w_t=c-qX_s$ gives the opposite axial force. A prescribed tangential law $K_Tw_t^{3/2}h(s)\mathbf t$ therefore gives the [force-free](stokes-flow.md#force-free) balance $K_Nq^2\int|Y_s|^3ds=K_T\int(c-qX_s)^{3/2}X_sh(s)ds$. The weight $h(s)$ is part of the constitutive approximation and must be justified separately from its speed exponent.

#### Basal bending moment of a planar flagellum

↑ **Parent:** [Resistive-force theory](#resistive-force-theory)

At leading order in slope, the [hydrodynamic torque](continuum-mechanics.md#hydrodynamic-torque) on the distal filament is $-\mu K_N\int_0^L s(Y_t-V)ds$. The displayed opposite [torque](classical-mechanics.md#torque) is required at its base. It is the total internal [bending moment](continuum-mechanics.md#bending-moment); identifying it with the active moment assumes no separate passive elastic moment. If a passive moment is specified, subtract that contribution to determine the required active moment.

#### Head-drag correction to planar flagellar propulsion

↑ **Parent:** [Resistive-force theory](#resistive-force-theory)

For a small-slope inextensible filament with prescribed transverse coordinate $Y(s,t)$, tangential-to-normal resistance ratio $\gamma$, and head drag parameter $\delta$, transverse [force balance](classical-mechanics.md#force-balance) gives $V=\int_0^L Y_tds/[L(1+\delta)]$. The mean axial swimming speed is $-(1-\gamma)\langle\int_0^L Y_s(Y_t-V)ds\rangle/[L(\delta+\gamma)]$. The mean material longitudinal deformation velocity vanishes for a periodic inextensible stroke anchored longitudinally at its base. A moving base offset must be distinguished from a coordinate measured relative to the actual attachment point.

#### Finite-amplitude propulsion of an inextensible periodic filament

↑ **Parent:** [Resistive-force theory](#resistive-force-theory)

With drag ratio $\rho=c_\parallel/c_\perp$, squared-tangent average $\beta=\Lambda^{-1}\int x_s^2ds$, and axial wave speed $V$, [resistive-force theory](#resistive-force-theory) gives the displayed axial swimming ratio. Pure axial free swimming additionally requires vanishing cross-tangent average, as in reflection-symmetric waveforms; otherwise a transverse [force](classical-mechanics.md#force) or translation is present.

##### Cross-resistance of an asymmetric planar waveform

↑ **Parent:** [Finite-amplitude propulsion of an inextensible periodic filament](#finite-amplitude-propulsion-of-an-inextensible-periodic-filament)

An asymmetric periodic planar filament can have nonzero cross-tangent average $\delta$ despite periodic vertical position. Its translational resistance per arclength period is $c_\perp\Lambda[I+(\rho-1)M]$, with $M_{xx}=\beta$, $M_{xy}=\delta$ and $M_{yy}=1-\beta$. Full [force](classical-mechanics.md#force) balance can therefore yield transverse translation, so an axial-only propulsion formula needs a symmetry or constraint assumption.

#### Oscillating rigid rod in resistive-force theory

↑ **Parent:** [Resistive-force theory](#resistive-force-theory)

A rigid rod with moving centre and changing orientation has material [velocity](classical-mechanics.md#velocity) $\dot{\mathbf X}+s\dot\theta\mathbf n$. Its centred rotational [velocity](classical-mechanics.md#velocity) is odd in arclength and has no resultant [force](classical-mechanics.md#force), while its orientation-dependent resistance tensor couples translation to transverse [force](classical-mechanics.md#force). [Resistive-force theory](#resistive-force-theory) uses per-length coefficients $c_\parallel,c_\perp$.

##### Power of a rocking rod

↑ **Parent:** [Oscillating rigid rod in resistive-force theory](#oscillating-rigid-rod-in-resistive-force-theory)

The leading mean [viscous dissipation](stokes-flow.md#viscous-dissipation) of a translating and rotating rigid rod is $c_\perp\epsilon^2\omega^2(La^2+L^3/12)/2$ for equal dimensionless translation and angle amplitudes. Both terms are quadratic in amplitude; rotational material [velocity](classical-mechanics.md#velocity) cannot be omitted simply because the angle is small.

##### Mean transverse force from a rocking rod

↑ **Parent:** [Oscillating rigid rod in resistive-force theory](#oscillating-rigid-rod-in-resistive-force-theory)

For $x=\epsilon a\cos\omega t$ and a tangent $(\sin\theta,\cos\theta)$ with $\theta=\epsilon\cos(\omega t+\phi)$, the leading [force](classical-mechanics.md#force) on the fluid is $\langle F_y\rangle=-(c_\perp-c_\parallel)L\epsilon^2a\omega\sin\phi/2$. The sign changes under reversal of the tilt convention. Quadrature strokes maximize its magnitude; reciprocal strokes give zero, consistent with [kinematic reversibility of Stokes flow](stokes-flow.md#kinematic-reversibility-of-stokes-flow).

#### Power of a periodic planar filament

↑ **Parent:** [Resistive-force theory](#resistive-force-theory)

The leading [viscous dissipation](stokes-flow.md#viscous-dissipation) due to a small planar filament stroke is $\dot W=\xi_\perp T^{-1}\int_0^T\int_0^\lambda y_t^2\,dx\,dt$. It follows from the work against the local [resistive-force theory](#resistive-force-theory) force. The transverse velocity controls the leading power; the quadratic longitudinal velocity contributes only at higher order.

#### Propulsive force of a periodic planar filament

↑ **Parent:** [Resistive-force theory](#resistive-force-theory)

For a small-amplitude planar filament without mean axial drift, [resistive-force theory](#resistive-force-theory) gives the leading time-averaged force on the filament as $F_x=(\xi_\perp-\xi_\parallel)T^{-1}\int_0^T\int_0^\lambda y_x y_t\,dx\,dt$. The [parallel and perpendicular drag coefficients of a slender filament](#parallel-and-perpendicular-drag-coefficients-of-a-slender-filament) must differ to obtain propulsion at this order. A right-going wave gives negative axial force; a left-going wave gives positive axial force.

##### Travelling-wave stationarity of planar filament propulsion

↑ **Parent:** [Propulsive force of a periodic planar filament](#propulsive-force-of-a-periodic-planar-filament)

For the leading periodic [propulsive force of a periodic planar filament](#propulsive-force-of-a-periodic-planar-filament) and [power of a periodic planar filament](#power-of-a-periodic-planar-filament) functionals, the [Euler-Lagrange equation](analysis.md#euler-lagrange-equation) for $F_x+\Gamma(\dot W-\dot W_0)$ gives $(\xi_\perp-\xi_\parallel)y_{xt}+\Gamma\xi_\perp y_{tt}=0$. For nonzero thrust, $y_t$ obeys an advection equation and the active [travelling wave](analysis.md#travelling-wave) is $f(x-ct)$, with $c=(\xi_\perp-\xi_\parallel)/(\Gamma\xi_\perp)$. A static periodic shape may be added without changing leading force or power. Stationarity is a necessary extremum condition, not by itself an existence theorem for a global maximum.

###### Bandwidth limitation in fixed-power filament optimization

↑ **Parent:** [Travelling-wave stationarity of planar filament propulsion](#travelling-wave-stationarity-of-planar-filament-propulsion)

At fixed leading [power of a periodic planar filament](#power-of-a-periodic-planar-filament), the family $a\sin(mkx+\Omega t)$ has [propulsive force of a periodic planar filament](#propulsive-force-of-a-periodic-planar-filament) increasing with spatial harmonic $m$. The formal quadratic objective is unbounded without a spatial cutoff; large harmonics eventually invalidate the small-slope model. With a finite admissible [Fourier series](fourier-series.md) band, force divided by power is a weighted average of the signed ratios $-(\xi_\perp-\xi_\parallel)k_j/(\xi_\perp\Omega_j)$. An allowed extremal ratio is attained by a [travelling wave](analysis.md#travelling-wave) mode, or by a superposition with one common phase speed.

#### First-order free swimming of a planar filament

↑ **Parent:** [Resistive-force theory](#resistive-force-theory)

For $y=\epsilon g(x,t)$ on $0\leq x\leq L$, uniform local drag and force/torque balance give $U_1=0$, $V_1=-4\langle g_t\rangle_x+6\langle xg_t\rangle_x/L$, and $\Omega_1=6\langle g_t\rangle_x/L-12\langle xg_t\rangle_x/L^2$. The tangent can be replaced by the undeformed direction at this order because the velocity is already first order.

##### First-order periodic transverse swimming velocity

↑ **Parent:** [First-order free swimming of a planar filament](#first-order-free-swimming-of-a-planar-filament)

The first-order lateral translation and rotation of a prescribed planar filament are time derivatives of fixed linear spatial averages of its shape. A periodic shape therefore gives zero temporal mean of both quantities. Net laboratory displacement can still arise at second order.

##### Least-squares projection of filament deformation velocity

↑ **Parent:** [First-order free swimming of a planar filament](#first-order-free-swimming-of-a-planar-filament)

At first order, the transverse drag depends on $g_t+V_1+\Omega_1x$. Its zero force and torque conditions make this residual orthogonal to $1$ and $x$. Thus $-V_1-\Omega_1x$ is the [linear least-squares projection](probability-and-statistics.md#linear-least-squares-projection) of the prescribed transverse deformation velocity onto the span of $1$ and $x$. This recasts a force-balance calculation as a projection.

#### Rigid-body velocity in a deforming swimmer frame

↑ **Parent:** [Resistive-force theory](#resistive-force-theory)

A material point at body-frame position $\mathbf r$ has velocity relative to stationary ambient fluid $\mathbf U+\boldsymbol\Omega\times\mathbf r+(\partial_t\mathbf r)_{\rm body}$. The translational, rotational and deformation terms must all be retained before assigning perturbation orders.

#### Parallel and perpendicular drag coefficients of a slender filament

↑ **Parent:** [Resistive-force theory](#resistive-force-theory)

The local [resistive-force theory](#resistive-force-theory) coefficients $\xi_\parallel$ and $\xi_\perp$ describe drag along and across a filament tangent. For very slender bodies their leading logarithmic values have ratio $\xi_\perp/\xi_\parallel\simeq2$. Geometry, ends and nonlocal fluid interactions affect the corrections. Anisotropy enables propulsion by rotating [helices](topology.md#helix).

##### Anisotropic slender-filament drag from Stokeslet integration

↑ **Parent:** [Parallel and perpendicular drag coefficients of a slender filament](#parallel-and-perpendicular-drag-coefficients-of-a-slender-filament)

Integrating a [Stokeslet](stokes-flow.md#stokeslet) distribution along a straight slender filament explains the leading drag anisotropy. Axial motion samples the tensor component $2/(8\pi\mu|z|)$, while transverse motion samples $1/(8\pi\mu|z|)$. Integrating on both sides from radius $a$ to cutoff $\ell$ gives $\xi_\parallel\sim2\pi\mu/\ln(\ell/a)$ and $\xi_\perp\sim4\pi\mu/\ln(\ell/a)$. End effects and nonlocal hydrodynamic interactions supply the corrections retained by [slender-body theory](stokes-flow.md#slender-body-theory).

#### Sperm number

↑ **Parent:** [Resistive-force theory](#resistive-force-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sperm_number)

The sperm number compares filament length with an [elastohydrodynamic penetration length](#elastohydrodynamic-penetration-length). For periodic forcing at angular frequency $\omega$, the usual convention is

$$
\operatorname{Sp}=L\left(\frac{c_\perp\omega}{B}\right)^{1/4}.
$$

Its fourth power is a viscous-to-bending ratio on the full filament length. In steady cross-flow problems a different convention also occurs: $\operatorname{Sp}=\zeta_\perp L^3U/A$, where $U$ is flow speed and $A$ the [filament bending modulus](#filament-bending-modulus). The defining formula distinguishes these conventions.

##### Elastohydrodynamic penetration length

↑ **Parent:** [Sperm number](#sperm-number)

The elastohydrodynamic penetration length balances the transverse viscous force $c_\perp\omega y$ against the bending force $By/\ell_\omega^4$ in a periodically driven filament. The [sperm number](#sperm-number) $L/\ell_\omega$ distinguishes nearly rigid, weakly deformed filaments from long filaments whose response is localized near the actuator.

##### Elastohydrodynamic boundary layer of a filament

↑ **Parent:** [Sperm number](#sperm-number)

When viscous drag creates a large axial tension $T$, a clamped filament turns toward its outer direction in a boundary layer of length $\sqrt{A/T}$.

## Chemotaxis

↑ **Parent:** [Mathematical biology](mathematical-biology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chemotaxis)

Chemotaxis is directed cell motion up or down a chemical concentration gradient.

### Chemotactic instability with a wavenumber cutoff

↑ **Parent:** [Chemotaxis](#chemotaxis)

For a homogeneous state with linear decay rate $A>0$, chemical decay $\gamma>0$, chemical diffusivity $D>0$ and chemotactic coupling $\beta\chi_0n_0$, a spatial mode $q=k^2$ has determinant $Q(q)=Dq^2-Bq+A\gamma$, where $B=\beta\chi_0n_0-AD-\gamma$. The trace is negative, so an instability requires $Q(q)<0$. Without a cutoff, the sharp continuous-wavenumber threshold is $B>2\sqrt{DA\gamma}$. With $q>q_0$, minimize $Dq+A\gamma/q$ over that range; its unconstrained minimizer is $\sqrt{A\gamma/D}$. Discrete geometries additionally require an actual allowed Laplacian eigenvalue in the open unstable band.

<h3 id="keller-segel-model">Keller--Segel model</h3>

↑ **Parent:** [Chemotaxis](#chemotaxis)

A Keller--Segel model couples the density of moving cells to a chemical field that biases their motion. A common cell conservation law is $b_t=Db_{xx}-\partial_x(\chi(c)b c_x)$. Chemical dynamics depend on the application: the attractant may be produced by cells, or a nutrient may instead be consumed. The nutrient-consumption model $c_t=-kb$ with no nutrient diffusion gives travelling bacterial bands rather than prescribing the chemical externally.

<h4 id="keller-segel-aggregation-threshold">Keller--Segel aggregation threshold</h4>

↑ **Parent:** [Keller--Segel model](#keller-segel-model)

For a homogeneous [Keller--Segel model](#keller-segel-model) with nonnegative chemical production, linearized cell diffusion $D_2>0$, attraction coefficient $D_1>0$, and chemical diffusion $D_\rho>0$, put $c=\kappa-a_0f'_0$ and $\kappa=(\rho k(\rho))'|_{\rho_0}$. A [Fourier mode](fourier-analysis.md#fourier-mode) with squared [wavenumber](wave-equation.md#wavenumber) $z$ has [determinant](linear-algebra.md#determinant) $z[D_2(c+D_\rho z)-D_1f_0]$. If $c\geq0$, a growing mode on the infinite plane exists exactly when $D_1f_0>D_2c$, and $0<z<(D_1f_0-D_2c)/(D_2D_\rho)$ is the unstable band. If $c<0$, the homogeneous chemical mode is already unstable. Dividing the threshold by $D_2\kappa$ to obtain a sum of two ratios is valid only when $\kappa>0$. Positivity of $k$ does not guarantee positivity of $(\rho k)'$.

<h5 id="fastest-growing-keller-segel-mode">Fastest-growing Keller--Segel mode</h5>

↑ **Parent:** [Keller--Segel aggregation threshold](#keller-segel-aggregation-threshold)

For the two-field [Keller--Segel model](#keller-segel-model), put $a=D_2$, $b=D_\rho$, $C=D_1f_0\geq0$, $c=\kappa-a_0f'_0$. The upper growth rate is $s_+(z)=-[c+(a+b)z]/2+\sqrt{[c+(b-a)z]^2+4Cz}/2$. When $C>\max(ac,-bc)$ its unique maximum occurs at positive $z_*$ satisfying $s_+'(z_*)=0$. For equal diffusion coefficients $a=b$, this gives $z_*=(C^2/a^2-c^2)/(4C)$. For $c<0$ and $C\leq-bc$, the fastest growth is homogeneous, with infinite [wavelength](wave-equation.md#wavelength). The finite-domain answer must maximize the growth rate over the permitted [Fourier modes](fourier-analysis.md#fourier-mode). Eliminating chemical dynamics instantaneously generally changes this selected scale.

#### Logarithmic chemotactic sensitivity

↑ **Parent:** [Keller--Segel model](#keller-segel-model)

For positive chemical concentration $c$, taking $\chi(c)=\alpha/c$ makes the [chemotaxis](#chemotaxis) drift velocity $\chi(c)c_x=\alpha\partial_x\log c$. Cells then respond to a relative chemical gradient. This singular response can remain finite where the concentration tends to zero if its logarithmic derivative has a finite limit.

##### Nutrient-consuming chemotactic travelling band

↑ **Parent:** [Logarithmic chemotactic sensitivity](#logarithmic-chemotactic-sensitivity)

For a [Keller--Segel model](#keller-segel-model) with $c_t=-kb$, a positive-speed [travelling wave](analysis.md#travelling-wave) $B(z),C(z)$, $z=x-vt$, satisfies $vC'=kB$ and $DB'+vB-\alpha BC'/C=0$ when the integrated bacterial flux constant is zero. Writing $\mu=\alpha/D>1$ and $\xi=v(z-z_0)/D$, its positive band solution is

$$
C=C_\infty(1+e^{-\xi})^{-1/(\mu-1)},\qquad
B=\frac{v^2C_\infty}{kD(\mu-1)}e^{-\xi}(1+e^{-\xi})^{-\mu/(\mu-1)}.
$$

To derive it, integrate $B'/B=\mu C'/C-v/D$ to obtain $B=KC^\mu e^{-vz/D}$, then separate $vC'=kB$. The positive integration constant is a translation of the wave. Concentration rises monotonically from zero behind to $C_\infty$ ahead; $B$ vanishes at both ends and has a unique maximum at $\xi=-\log(\mu-1)$. The condition $\mu>1$ describes this exponential-tail branch; it is not asserted to exclude every limiting or weak travelling wave at other parameter values.

###### Speed of a nutrient-consuming chemotactic band

↑ **Parent:** [Nutrient-consuming chemotactic travelling band](#nutrient-consuming-chemotactic-travelling-band)

For a [nutrient-consuming chemotactic travelling band](#nutrient-consuming-chemotactic-travelling-band) in a tube of cross-sectional area $a$, let $N=a\int_{\mathbb R}B(z)dz$. Integrating $vC'=kB$ between depleted nutrient behind and $C_\infty$ ahead gives $vC_\infty=kN/a$, hence $v=Nk/(aC_\infty)$. This is a nutrient budget: advancing by a unit length supplies $aC_\infty$ nutrient, while the bacteria consume at total rate $kN$. Diffusion and chemotactic sensitivity affect the band shape and admissibility, but not this speed at fixed $N,k,a,C_\infty$.

### Chemotactic pattern-forming instability

↑ **Parent:** [Chemotaxis](#chemotaxis)

A chemotactic pattern-forming instability occurs when cells produce an attractant and drift up its gradient strongly enough that positive aggregation feedback overcomes diffusion and turnover at a finite wavelength.

### Chemotactic telegraph equation

↑ **Parent:** [Chemotaxis](#chemotaxis)

A chemotactic telegraph equation describes persistent motion with finite turning rate and a turning bias set by a chemical gradient. Its large-turning-rate limit is a drift--diffusion equation with chemotactic drift.

## Biopolymer mechanics

↑ **Parent:** [Mathematical biology](mathematical-biology.md)

Biopolymer mechanics studies bending, stretching, thermal fluctuations, and force-induced deformation of filamentous biological macromolecules.

### Hydrodynamic drag models for a polymer

↑ **Parent:** [Biopolymer mechanics](#biopolymer-mechanics)

The drag of a translating [polymer](chemistry.md#polymer) depends on conformation and hydrodynamic interactions. A nondraining coil has $\zeta\sim6\pi\eta R_h$; a long aligned rod has $\zeta_\parallel\sim2\pi\eta L/\log(L/a)$ and roughly twice that transverse drag; a freely draining model sums the monomer drag coefficients. Mechanical power is $\zeta U^2$. These models cannot be interchanged without changing the assumed conformation and solvent-mediated coupling.

### Polymerization Brownian ratchet

↑ **Parent:** [Biopolymer mechanics](#biopolymer-mechanics)

A [polymerization Brownian ratchet](#polymerization-brownian-ratchet) advances a filament by incorporating a monomer when thermal motion opens enough space between its tip and a resisting load. The irreversible chemical step rectifies the load's fluctuations. The elementary load advance $a$ depends on tip geometry; two staggered strands can give $a=\delta/2$, whereas two aligned strands do not automatically give this step. An effective addition rate must refer to the same elementary advance.

#### Reaction-limited polymerization Brownian ratchet

↑ **Parent:** [Polymerization Brownian ratchet](#polymerization-brownian-ratchet)

When load-gap equilibration is fast compared with chemical events, an opposing force gives an exponential gap distribution. The probability of room for an addition is $e^{-Fa/(k_BT)}$. With unloaded addition rate $u$ and removal rate $w$, assumed force-independent except for this steric gating, the velocity is the displayed expression. For $u>w$, stall occurs at $F_s=(k_BT/a)\log(u/w)$. Concentration is included in $u=k_{\rm on}c$ if the on-rate constant is bimolecular.

#### Diffusion-limited Brownian ratchet with constant load

↑ **Parent:** [Polymerization Brownian ratchet](#polymerization-brownian-ratchet)

In the instantaneous-addition, negligible-removal ratchet, the gap reflects at zero and a first passage to $a$ triggers addition and resets the gap to zero. With load diffusion coefficient $D$ and opposing drift $DF/(k_BT)$, the mean passage time solves $DT''-DFT'/(k_BT)=-1$, $T'(0)=0$, $T(a)=0$. It is $T(0)=a^2(e^z-1-z)/(Dz^2)$, giving the displayed speed and zero-load limit $2D/a$. The finite-load slowdown is not simply $e^{-z}$ in this diffusion-limited regime.

### Bending and torsion of filament bundles

↑ **Parent:** [Biopolymer mechanics](#biopolymer-mechanics)

For independent sliding filaments in a filled bundle, bending energies add and $B\sim NEr^4\sim Er^2R^2$. A coherently bonded one-filament-thick tube has $B\sim ErR^3$, while a bonded filled rod has $B\sim ER^4$. The same torsional scalings apply with the [shear modulus](continuum-mechanics.md#shear-modulus) instead of [Young's modulus](continuum-mechanics.md#young-s-modulus) if individual sliding filaments are forced to undergo a common material twist. Completely free filament spin/slip does not define that torsional response: collective helical bending alone begins at fourth order in the twist rate.

### Adhesive-cell rolling threshold

↑ **Parent:** [Biopolymer mechanics](#biopolymer-mechanics)

For a weakly adhering elastic sphere, balancing elastic contact energy $Ga^5/R^2$ against adhesion $Ja^2$ gives contact radius $a\sim(JR^2/G)^{1/3}$. If peeling the rear contact dissipates work of order $J$ per unit area, its rolling moment is $M_r\sim JaR$. Balancing this with a fluid shear moment $\eta\dot\gamma R^3$ gives the displayed estimate. A perfectly reversible elastic contact has no such net rolling-energy barrier; adhesive hysteresis or bond kinetics must justify a finite threshold, and the corresponding dissipative adhesion energy replaces $J$.

### de Gennes confinement scaling

↑ **Parent:** [Biopolymer mechanics](#biopolymer-mechanics)

For a long self-avoiding [polymer](chemistry.md#polymer) in a tube of diameter $D$, represent each confinement blob by $g$ statistical segments of length $b$, with $D\sim bg^{3/5}$. Excluded-volume repulsion orders the blobs along the tube, giving $X\sim(N/g)D=L(b/D)^{2/3}$. More generally, a segment excluded-volume parameter $v$ gives $X\sim L[v/(bD^2)]^{1/3}$. This requires many blobs and $D$ smaller than the free coil size; $b\ll D\ll L$ alone does not ensure that. An ideal chain without intersegment repulsion is not a one-dimensional string of nonoverlapping blobs.

#### Polymer coil in slit confinement

↑ **Parent:** [de Gennes confinement scaling](#de-gennes-confinement-scaling)

In a slit, a confinement blob is three-dimensional but the chain of blobs forms a two-dimensional [self-avoiding walk](combinatorics.md#self-avoiding-walk). With $g\sim(D/b)^{5/3}$ and in-plane exponent $3/4$, $R_\parallel\sim D(N/g)^{3/4}$. There is no single preferred axial extension as in a tube. A strictly planar chain confined further to a narrow strip is a different geometry and gives $X\sim L(b/D)^{1/3}$ under the two-dimensional blob estimate.

### Gaussian chain

↑ **Parent:** [Biopolymer mechanics](#biopolymer-mechanics)

An ideal [Gaussian chain](#gaussian-chain) is a [polymer](chemistry.md#polymer) model whose independent segment vectors have zero mean and isotropic [Gaussian distribution](probability-theory.md#normal-distribution). If $\langle|\mathbf r|^2\rangle=b^2$, each Cartesian [variance](variance.md) is $b^2/3$, so a displacement across $\ell$ links has density $(3/(2\pi\ell b^2))^{3/2}\exp[-3R^2/(2\ell b^2)]$ and [characteristic function](probability-theory.md#characteristic-function) $\exp[-k^2b^2\ell/6]$. The continuous-contour version uses the same [characteristic function](probability-theory.md#characteristic-function) for any contour separation. It is the large-scale limit of a [freely jointed chain](#ideal-chain), while allowing unbounded Gaussian segment lengths and omitting interactions between distant parts of the chain.

#### Debye scattering function for a Gaussian chain

↑ **Parent:** [Gaussian chain](#gaussian-chain)

A continuum [Gaussian chain](#gaussian-chain) has separation [characteristic function](probability-theory.md#characteristic-function) $e^{-a|s-t|}$, $a=k^2b^2/6$. Integrating over a contour of length $N$ gives the [polymer scattering function](critical-phenomenon.md#polymer-scattering-function)

$$
g(k)=\frac2N\int_0^N(N-s)e^{-as}\,ds=N\mathcal D(x),\qquad x=aN=k^2R_g^2,
$$

where $R_g^2=Nb^2/6$ in this continuum convention and $\mathcal D(x)=2(e^{-x}-1+x)/x^2$, with continuous value $\mathcal D(0)=1$. Its limits are $\mathcal D(x)=1-x/3+x^2/12+\cdots$ and $\mathcal D(x)\sim2/x$ for large $x$.

For a discrete chain with $N$ sites, retain the self terms and let $z=e^{-k^2b^2/6}$. The exact finite expression is $g_N=1+(2/N)\sum_{\ell=1}^{N-1}(N-\ell)z^\ell=(1+z)/(1-z)-2z(1-z^N)/[N(1-z)^2]$, with $g_N(0)=N$. Taking $N\to\infty$ while $x=Nk^2b^2/6$ stays fixed gives $g_N/N\to\mathcal D(x)$. The continuum expression describes the coil scaling range, whereas the discrete expression tends to one as $kb\to\infty$.

### Ideal chain

↑ **Parent:** [Biopolymer mechanics](#biopolymer-mechanics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ideal_chain)

An [ideal chain](#ideal-chain), also called a [freely jointed chain](#ideal-chain), consists of fixed-length links with independent orientations and no bending energy between successive links. It neglects segment interactions and excluded volume. A [one-dimensional freely jointed chain](statistical-physics.md#one-dimensional-freely-jointed-chain) restricts each link to two orientations. At fixed force its [canonical partition function](statistical-physics.md#canonical-partition-function) factors into one-link angular integrals. The resulting extension is entropic and depends on [temperature](thermodynamics.md#temperature) and on whether the orientations are allowed in one, two, or three dimensions.

#### Three-dimensional entropic chain stiffness

↑ **Parent:** [Ideal chain](#ideal-chain)

A three-dimensional [ideal chain](#ideal-chain) of $N$ independent segments of length $b$ has $\langle R^2\rangle=Nb^2=Lb$. The isotropic small-force susceptibility gives $\langle z\rangle=F\langle R^2\rangle/(3k_BT)$, so $k_s=3k_BT/(Lb)$. For a long [worm-like chain](#worm-like-chain), the statistical segment is $b=2l_p$. This stiffness describes entropic end-to-end extension, not axial stretching of the material backbone, whose spring constant is $EA/L$.

#### Gaussian limit of the end-to-end distribution of a freely jointed chain

↑ **Parent:** [Ideal chain](#ideal-chain)

For an isotropic fixed-length step $b$, angular integration gives the [characteristic function](probability-theory.md#characteristic-function) $\widehat\psi(\mathbf k)=\sin(kb)/(kb)$. Independence makes the [characteristic function](probability-theory.md#characteristic-function) of the sum of $N$ steps its $N$th power. Since $\ln[\sin(kb)/(kb)]=-k^2b^2/6+O(k^4b^4)$, the central scaling $k=O((b\sqrt N)^{-1})$ gives $\widehat\Phi\to\exp[-Nb^2k^2/6]$. The inverse [Fourier transform](analysis.md#fourier-transform) is

$$
\Phi(\mathbf R,N)\sim\left(\frac3{2\pi Nb^2}\right)^{3/2}\exp\left[-\frac{3R^2}{2Nb^2}\right].
$$

This is a density with respect to three-dimensional vector volume, not a radial density; the radial density is $4\pi R^2\Phi$. It has $\langle R^2\rangle=Nb^2$. The approximation holds on the central coil scale $R=O(b\sqrt N)$, not near the fully stretched finite-length boundary $R=Nb$.

#### Planar freely jointed chain

↑ **Parent:** [Ideal chain](#ideal-chain)

If each link is restricted to a plane, $Z_1=\int_0^{2\pi}e^{\xi\cos\theta}d\theta=2\pi I_0(\xi)$, with $\xi=Fb/(k_BT)$. Differentiating gives $L/(Nb)=I_1(\xi)/I_0(\xi)$, where $I_n$ are [Modified Bessel functions of the first kind](analysis.md#modified-bessel-function-of-the-first-kind). The high-force angular Gaussian has $\langle\theta^2\rangle\sim1/\xi$, so $Nb-L\sim Nk_BT/(2F)$, half the three-dimensional coefficient.

#### Force-extension of a three-dimensional freely jointed chain

↑ **Parent:** [Ideal chain](#ideal-chain)

Independent link orientations make the [canonical partition function](statistical-physics.md#canonical-partition-function) $Z_1^N$, with the one-link integral defining the [Langevin function](#langevin-function). Differentiating its logarithm with respect to force gives $L=Nb\mathscr L(Fb/(k_BT))$. At high extension, $Nb-L\sim Nk_BT/F$, so the force diverges inversely with remaining length deficit. This requires rigid links and excludes axial bond stretching.

#### Langevin function

↑ **Parent:** [Ideal chain](#ideal-chain)

The [Langevin function](#langevin-function) is the mean projection of a freely orientable three-dimensional unit vector weighted by $e^{\xi\cos\theta}$. Integrating over solid angle gives $Z_1=4\pi\sinh\xi/\xi$, and differentiation gives $\langle\cos\theta\rangle=\partial_\xi\log Z_1=\coth\xi-1/\xi$. It behaves as $\xi/3$ at small argument and $1-1/\xi$ at large positive argument.

### Inextensible filament

↑ **Parent:** [Biopolymer mechanics](#biopolymer-mechanics)

An inextensible filament keeps the length of every material segment fixed. With material [arc length](riemannian-geometry.md#arc-length) $s$, its centerline obeys $|\mathbf r_s|=1$ and has [unit tangent vector](differential-geometry.md#unit-tangent-vector) $\mathbf t=\mathbf r_s$. A [filament tension](#filament-tension) acts as a [Lagrange multiplier](mathematical-optimization.md#lagrange-multiplier) for this constraint.

#### Axial and arclength travelling-wave speeds

↑ **Parent:** [Inextensible filament](#inextensible-filament)

For a periodic [inextensible filament](#inextensible-filament) with arclength period $\Lambda$ and projected axial period $\lambda$, material points slide tangentially through the wave frame at speed $Q$. An axial pattern speed $V$ relative to mean filament motion gives $Q\lambda/\Lambda=V$. Confusing the two speeds changes the swimming-to-wave-speed ratio by $\lambda/\Lambda$.

#### Quadratic longitudinal displacement of an inextensible planar filament

↑ **Parent:** [Inextensible filament](#inextensible-filament)

Write a small planar displacement in arclength coordinates as $X=s+X_2$ and $Y=y$. The [inextensibility](#inextensible-filament) relation $X_s^2+Y_s^2=1$ gives $X_{2,s}=-y_s^2/2$ to quadratic order. Thus longitudinal material velocity enters one order later than the transverse velocity. For a periodic material stroke with no mean axial drift, its mean velocity vanishes, although its instantaneous contribution is needed for exact local force balance.

#### Filament bending modulus

↑ **Parent:** [Inextensible filament](#inextensible-filament)

The filament bending modulus multiplies squared [curvature of a space curve](differential-geometry.md#curvature-of-a-space-curve) in the bending energy, $E_b=(B/2)\int\kappa^2\,ds$. It has dimensions force times length squared. In the small-slope [Monge representation](#monge-representation), the leading elastic force per unit length is $-By_{xxxx}$.

#### Filament tension

↑ **Parent:** [Inextensible filament](#inextensible-filament)

Filament tension is the axial force enforcing local [inextensibility](#inextensible-filament). Its force density is $\partial_s(T\mathbf r_s)$. A pre-existing constant tension contributes $Ty_{xx}$ to small-slope transverse dynamics; in an unloaded, initially straight filament, tension induced by transverse motion begins at second order in amplitude.

### Monge representation

↑ **Parent:** [Biopolymer mechanics](#biopolymer-mechanics)

The Monge representation describes a nearly flat curve or surface as a single-valued height over a reference line or plane. For a planar curve $(x,h(x))$ with small slope, arclength is $ds=dx+O(h_x^2)$ and signed curvature is $\kappa=h_{xx}+O(h_x^2h_{xx})$.

### Stokesian dynamics of an elastic filament

↑ **Parent:** [Biopolymer mechanics](#biopolymer-mechanics)

In local Stokesian filament dynamics, viscous drag balances the variational elastic force without inertia. A small-slope filament of bending modulus $A$ and transverse drag $\zeta$ obeys $\zeta h_t=-Ah_{xxxx}$.

#### Overdamped relaxation of a free filament

↑ **Parent:** [Stokesian dynamics of an elastic filament](#stokesian-dynamics-of-an-elastic-filament)

The [overdamped filament bending equation](#small-slope-elastohydrodynamic-filament-equation) diagonalizes in the complete [free-free bending spectrum](continuum-mechanics.md#free-free-bending-spectrum). Positive modes decay at rates $Ak_n^4/\zeta$, while translation and tilt remain fixed. The long-time shape is the affine least-squares projection of the initial height. Free-end boundary values conserve the total height integral and its first spatial moment. For square-integrable initial data the expansion gives the smoothing semigroup solution.

#### Small-slope elastohydrodynamic filament equation

↑ **Parent:** [Stokesian dynamics of an elastic filament](#stokesian-dynamics-of-an-elastic-filament)

For a straight, unloaded [inextensible filament](#inextensible-filament) with small transverse displacement, [resistive-force theory](#resistive-force-theory) gives viscous force density $-c_\perp y_t$. Variation of the bending energy gives $-By_{xxxx}$, while the induced [filament tension](#filament-tension) is higher order. Their instantaneous balance yields $c_\perp y_t=-By_{xxxx}$. It is an overdamped fourth-order diffusion equation: short-wavelength bends relax much faster than long ones. [Wiggins and Goldstein's flexive-propulsion paper](https://arxiv.org/abs/cond-mat/9707346) develops the elastic-wave mechanism for low-Reynolds-number propulsion.

##### Uniform-load bending of a clamped filament

↑ **Parent:** [Small-slope elastohydrodynamic filament equation](#small-slope-elastohydrodynamic-filament-equation)

Let positive transverse displacement point along a uniform load per unit length $w$. The [filament bending modulus](#filament-bending-modulus) $B$ gives energy $\int_0^L[B(h_{xx})^2/2-wh]dx$. The [variational derivative](classical-mechanics.md#variational-derivative) is $Bh_{xxxx}-w$, so [resistive-force theory](#resistive-force-theory) gives $\zeta_\perp h_t=-Bh_{xxxx}+w$. Clamping imposes $h(0)=h_x(0)=0$, while a free tip imposes $h_{xx}(L)=h_{xxx}(L)=0$. The steady solution is

$$
h_s(x)=\frac{w}{24B}x^2(x^2-4Lx+6L^2).
$$

Its tip displacement is $wL^4/(8B)$. For a submerged cylindrical filament under [Newtonian gravity](classical-mechanics.md#gravitational-acceleration), [buoyancy](fluid-mechanics.md#buoyancy) gives $w=(\rho_f-\rho)\pi a^2g$. This linear approximation requires small slope and negligible inertia.

###### Tip stiffness of a uniformly loaded cantilever

↑ **Parent:** [Uniform-load bending of a clamped filament](#uniform-load-bending-of-a-clamped-filament)

For a [uniform-load bending of a clamped filament](#uniform-load-bending-of-a-clamped-filament), total load $F=wL$ and tip displacement $\delta=wL^4/(8B)$ obey [Hooke's law](continuum-mechanics.md#hooke-s-law) in the form $F=k_{\rm eff}\delta$, with $k_{\rm eff}=8B/L^3$. This stiffness depends on the specified distributed loading. A concentrated tip force instead gives $3B/L^3$, so equal total forces with different distributions are not interchangeable.

##### Boundary expression for transverse filament thrust

↑ **Parent:** [Small-slope elastohydrodynamic filament equation](#small-slope-elastohydrodynamic-filament-equation)

The anisotropic-drag contribution to axial force from a small-slope transverse motion is $F=(c_\perp-c_\parallel)\int y_xy_t\,dx$. Using the [small-slope elastohydrodynamic filament equation](#small-slope-elastohydrodynamic-filament-equation) and [integration by parts](calculus.md#integration-by-parts) gives

$$
F=B\left(1-\frac{c_\parallel}{c_\perp}\right)\left[\frac12y_{xx}^2-y_xy_{xxx}\right]_0^L.
$$

Thus this propulsive contribution is determined by endpoint slope, bending moment, and shear. A separately imposed axial translation adds ordinary longitudinal drag. Exact second-order longitudinal motion required by [inextensibility](#inextensible-filament) also contributes to instantaneous total drag, but its time-derivative contribution averages to zero over a deformation cycle.

##### Oscillatory bending of a moment-free semi-infinite filament

↑ **Parent:** [Small-slope elastohydrodynamic filament equation](#small-slope-elastohydrodynamic-filament-equation)

In units of [elastohydrodynamic penetration length](#elastohydrodynamic-penetration-length) and inverse forcing frequency, $y_t=-y_{xxxx}$. Prescribing $y(0,t)=y_0\cos t$, zero bending moment $y_{xx}(0,t)=0$, and decay at infinity gives

$$
y(x,t)=\frac{y_0}{2}\left[e^{-Cx}\cos(t+Sx)+e^{-Sx}\cos(t-Cx)\right],\qquad C=\cos(\pi/8),\quad S=\sin(\pi/8).
$$

The two components have [phase velocities](wave-equation.md#phase-velocity) $-1/S$ and $1/C$. Their unequal spatial attenuation produces a nonreciprocal shape cycle even though the endpoint actuation is reciprocal.

### Microtubule

↑ **Parent:** [Biopolymer mechanics](#biopolymer-mechanics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Microtubule)

A microtubule is a stiff hollow cytoskeletal filament assembled from tubulin. Its millimetre-scale persistence length makes bending fluctuations measurable over micrometre lengths.

### Thermal bending fluctuations of a clamped filament

↑ **Parent:** [Biopolymer mechanics](#biopolymer-mechanics)

A clamped filament of length $L$ and bending modulus $A$ has equilibrium tip variance $k_BT L^3/(3A)$. Under local transverse viscous drag, each bending mode relaxes exponentially at a rate proportional to its fourth power of wavenumber.

<h4 id="clamped-free-bending-mode">Clamped--free bending mode</h4>

↑ **Parent:** [Thermal bending fluctuations of a clamped filament](#thermal-bending-fluctuations-of-a-clamped-filament)

The bending modes of a filament clamped at one end and force-free and torque-free at the other obey $\cos\alpha_n\cosh\alpha_n=-1$. The slowest mode has $\alpha_1\simeq1.875$.

##### Fourth inverse-power sum of the cantilever spectrum

↑ **Parent:** [Clamped--free bending mode](#clamped-free-bending-mode)

For the positive roots $q_n$ of $\cos q\cosh q=-1$, $\sum_nq_n^{-4}=1/12$. The [tip-force compliance of a cantilever](continuum-mechanics.md#tip-force-compliance-of-a-cantilever) is $L^3/(3A)$ directly, whereas expansion in normalized [clamped--free bending modes](#clamped-free-bending-mode) and $W_n(L)^2=4L^{-1}\int W_n^2dx$ gives $4L^3\sum_nq_n^{-4}/A$. Equating the two responses proves the sum and evaluates the full thermal endpoint [variance](variance.md).

##### Constrained variational characterization of bending modes

↑ **Parent:** [Clamped--free bending mode](#clamped-free-bending-mode)

The [elastic energy](continuum-mechanics.md#elastic-energy) $U=A\int(W'')^2dx/2$ minimized without forcing gives $W''''=0$. With fixed $\int W^2dx$, stationarity of $U-Ak^4\int W^2dx/2$ gives $W''''=k^4W$: a bending eigenmode. A general admissible shape expands in these [normal modes](wave-equation.md#normal-mode). The [natural boundary conditions for a free endpoint](analysis.md#natural-boundary-conditions-for-a-free-endpoint) are $W''(L)=W'''(L)=0$, while the clamp imposes $W(0)=W'(0)=0$.

<h5 id="overdamped-relaxation-of-a-clamped-free-filament">Overdamped relaxation of a clamped--free filament</h5>

↑ **Parent:** [Clamped--free bending mode](#clamped-free-bending-mode)

For $\zeta_\perp h_t=-Bh_{xxxx}$, separated [normal modes](wave-equation.md#normal-mode) decay at rates $B\alpha_n^4/(\zeta_\perp L^4)$. Clamping at zero and vanishing moment and shear at $L$ give $\cos\alpha_n\cosh\alpha_n=-1$. A mode is

$$
\phi_n(s)=\cosh(\alpha_ns)-\cos(\alpha_ns)-\eta_n[\sinh(\alpha_ns)-\sin(\alpha_ns)],\qquad
\eta_n=\frac{\cosh\alpha_n+\cos\alpha_n}{\sinh\alpha_n+\sin\alpha_n},\quad s=x/L.
$$

The fourth-order operator is [self-adjoint](linear-operator-theory.md#self-adjoint-operator): two [integration by parts](calculus.md#integration-by-parts) operations give $\int f g''''=\int f''g''$ under these boundary conditions. Its zero eigenspace is trivial and its [eigenfunctions](linear-operator-theory.md#eigenfunction) form an orthogonal complete basis. Thus a nonzero projection on the first mode gives long-time decay proportional to $\phi_1(x/L)\exp[-B\alpha_1^4t/(\zeta_\perp L^4)]$, where $\alpha_1=1.8751040687\ldots$. If this projection vanishes, the lowest excited mode replaces it.

<h4 id="free-free-biharmonic-eigenvalue-equation">Free--free biharmonic eigenvalue equation</h4>

↑ **Parent:** [Thermal bending fluctuations of a clamped filament](#thermal-bending-fluctuations-of-a-clamped-filament)

A filament free of moment and shear at both ends has $h_{xx}=h_{xxx}=0$. Its positive biharmonic eigenvalues $q_n^4$ obey $\cos(q_nL)\cosh(q_nL)=1$, in addition to the two rigid zero modes representing translation and rotation.

### Follower force on a filament

↑ **Parent:** [Biopolymer mechanics](#biopolymer-mechanics)

A follower force acts along the instantaneous tangent at its point of application. Its direction changes with the filament, making its generalized force nonconservative and allowing oscillatory instabilities in overdamped dynamics.

#### Two-link follower-force filament model

↑ **Parent:** [Follower force on a filament](#follower-force-on-a-filament)

A two-link follower-force model replaces a filament by two rigid links with torsional springs and point drags. The nonsymmetric linearized stiffness can produce a Hopf bifurcation even without inertia.

##### Dimensionless follower load

↑ **Parent:** [Two-link follower-force filament model](#two-link-follower-force-filament-model)

The dimensionless follower load compares the moment scale $\Gamma\ell$ of a tangential tip force with a torsional spring constant $k$. In the equal-link two-degree-of-freedom model, straight motion loses stability through a Hopf bifurcation at $\Sigma=3$.

### Worm-like chain

↑ **Parent:** [Biopolymer mechanics](#biopolymer-mechanics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Worm-like_chain)

The worm-like chain models an inextensible filament with bending energy $A\int\kappa^2ds/2$ and thermal tangent fluctuations.

#### Kuhn length

↑ **Parent:** [Worm-like chain](#worm-like-chain)

The [Kuhn length](#kuhn-length) is the link length of an equivalent long [ideal chain](#ideal-chain) with the same contour length and mean squared end-to-end distance. A three-dimensional [worm-like chain](#worm-like-chain) satisfies $\langle R^2\rangle\sim2l_pL$ for $L\gg l_p$, hence $b_K=2l_p$.

#### High-force worm-like chain elasticity

↑ **Parent:** [Worm-like chain](#worm-like-chain)

A strongly stretched inextensible [worm-like chain](#worm-like-chain) has two small transverse tangent components. Its quadratic energy is $\frac12\int[A|\partial_s\mathbf t_\perp|^2+f|\mathbf t_\perp|^2]ds-fL$. For a long bulk chain, the [equipartition theorem](statistical-physics.md#equipartition-theorem) assigns each Fourier mode covariance $k_BT/(Aq^2+f)$. Integrating over $q$ and summing both components gives $\langle|\mathbf t_\perp|^2\rangle=k_BT/\sqrt{Af}$, hence the extension deficit is half that value. With [persistence length](#persistence-length) $L_p=A/(k_BT)$, the deficit is $\sqrt{k_BT/(4L_pf)}$. It requires small slopes and negligible stretching of the backbone.

##### Transverse tangent correlation of a stretched worm-like chain

↑ **Parent:** [High-force worm-like chain elasticity](#high-force-worm-like-chain-elasticity)

The bulk tangent [covariance](variance.md#covariance) is twice the inverse [Fourier transform](analysis.md#fourier-transform) of $k_BT/(Aq^2+f)$, one term for each transverse direction. Equivalently the inverse of $-A\partial_r^2+f$ is $e^{-|r|/\xi}/(2\sqrt{Af})$. This gives the displayed correlation and identifies a force-dependent [correlation length](critical-phenomenon.md#correlation-length), different from the zero-force [persistence length](#persistence-length). Finite chains require endpoint conditions or a periodic convention.

###### Periodic finite-length tangent correlation of a stretched worm-like chain

↑ **Parent:** [Transverse tangent correlation of a stretched worm-like chain](#transverse-tangent-correlation-of-a-stretched-worm-like-chain)

Periodizing the bulk [transverse tangent correlation of a stretched worm-like chain](#transverse-tangent-correlation-of-a-stretched-worm-like-chain) gives $C_L(r)=\sum_{j\in\mathbb Z}C(r+jL)$, where $d_L(r)$ is the distance to zero on the periodic interval. Summing the geometric series yields the displayed result. At zero separation its finite-length factor is $\coth(L/(2\xi))$; for $L\gg\xi$ the bulk result is recovered. Periodic tangent fluctuations are a mathematical boundary convention, not a claim that a pulled physical chain forms a closed loop.

#### Persistence length

↑ **Parent:** [Worm-like chain](#worm-like-chain)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Persistence_length)

The persistence length is the decay length of tangent correlations. A common three-dimensional convention is $L_p=A/(k_BT)$; a strictly planar chain has tangent-correlation length $2A/(k_BT)$.

### Euler buckling of an elastic filament

↑ **Parent:** [Biopolymer mechanics](#biopolymer-mechanics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euler_buckling_of_an_elastic_filament)

A pinned filament of length $L$ and bending modulus $A$ first buckles under compressive force $F_c=\pi^2A/L^2$.

#### Polymerization-driven cantilever postbuckling

↑ **Parent:** [Euler buckling of an elastic filament](#euler-buckling-of-an-elastic-filament)

A clamped filament touching a laterally sliding, moment-free wall has fixed projected gap $d$. For an inextensible small-amplitude elastica, parameterize its tip angle by $k=\sin(\theta_{\rm tip}/2)$. Then $\ell=\sqrt{B/F}K(k)$ and $d=\sqrt{B/F}[2E(k)-K(k)]$, where $K,E$ are complete elliptic integrals. Their small-$k$ expansions give the displayed decrease of wall force with excess contour length. It concerns the weakly buckled branch, before overhang or additional wall contact changes the boundary conditions.

#### Thermal rounding of a buckling transition

↑ **Parent:** [Euler buckling of an elastic filament](#euler-buckling-of-an-elastic-filament)

Thermal fluctuations smooth the zero-temperature pitchfork in filament buckling: the mean compression remains analytic and nonzero below the mechanical threshold, with rounding controlled by $L/L_p$.

#### Self-buckling of a vertical rod

↑ **Parent:** [Euler buckling of an elastic filament](#euler-buckling-of-an-elastic-filament)

A vertical rod can buckle under its own distributed weight. For a rod clamped below and free above, the threshold is set by a Bessel-function eigenvalue rather than the sinusoidal mode of a rod under constant end load.

##### Bessel threshold for self-buckling of a vertical rod

↑ **Parent:** [Self-buckling of a vertical rod](#self-buckling-of-a-vertical-rod)

For a uniform [elastic filament](continuum-mechanics.md#elastic-filament) clamped below and free above, its own weight gives [filament tension](#filament-tension) $T(z)=-\lambda g(L-z)$. With [filament bending modulus](#filament-bending-modulus) $B=EI$, the static slope $u$ satisfies $Bu''+\lambda g(L-z)u=0$, $u(0)=0$, and $u'(L)=0$. Setting $\eta=(2/3)\sqrt{\lambda g/B}(L-z)^{3/2}$ gives $u=\eta^{1/3}J_{-1/3}(\eta)$ up to amplitude; the $J_{1/3}$ branch violates the zero-moment condition. The first positive zero $j_{-1/3,1}$ therefore yields $\lambda gL_c^3/B\simeq7.83735$. This is a [self-buckling of a vertical rod](#self-buckling-of-a-vertical-rod) threshold, not a constant-end-load Euler threshold.

## Lipid bilayer

↑ **Parent:** [Mathematical biology](mathematical-biology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lipid_bilayer)

A lipid bilayer is a self-assembled double layer of amphiphilic molecules. Its bending modulus controls thermal undulations and the resulting interaction between nearby membranes.

### Line tension

↑ **Parent:** [Lipid bilayer](#lipid-bilayer)

[Line tension](#line-tension) is energy per unit length of a boundary, such as the edge between two phases of a [lipid bilayer](#lipid-bilayer). Positive [line tension](#line-tension) tends to minimize the perimeter at fixed domain area. Its dimensions and geometry differ from [surface tension](fluid-mechanics.md#surface-tension), which is energy per unit area.

#### Fixed-area capillary spectrum of a circular boundary

↑ **Parent:** [Line tension](#line-tension)

For a circular domain of radius $R_0$ with [line tension](#line-tension) $\gamma$, the stiffness of a real polar sine or cosine amplitude with integer angular harmonic $m$ is $K_m=\pi\gamma(m^2-1)/R_0$, when the enclosed area is fixed. The [equipartition theorem](statistical-physics.md#equipartition-theorem) gives $\langle u_m^2\rangle=k_BT R_0/[\pi\gamma(m^2-1)]$ for $m\ge2$. A positive-[frequency](physics.md#frequency) complex [Fourier mode](fourier-analysis.md#fourier-mode) coefficient has half this variance. The uniform mode is forbidden and $m=1$ is translation.

##### Translation mode of a circular boundary

↑ **Parent:** [Fixed-area capillary spectrum of a circular boundary](#fixed-area-capillary-spectrum-of-a-circular-boundary)

The first polar sine and cosine harmonics of a circular boundary represent displacements of its centre. A complete translation leaves perimeter and area unchanged, so [line tension](#line-tension) supplies zero stiffness to these modes. The centre of an unconfined domain has no normalizable positional [thermal equilibrium](thermodynamics.md#thermal-equilibrium) in an infinite plane; recentering the boundary removes this freedom from a shape spectrum.

### Lipid vesicle

↑ **Parent:** [Lipid bilayer](#lipid-bilayer)

A lipid vesicle is a closed [lipid bilayer](#lipid-bilayer) enclosing fluid. Its shape and [thermal membrane undulations](#thermal-membrane-undulation) depend on [membrane tension](#membrane-tension), [membrane bending modulus](#membrane-bending-modulus), and constraints such as fixed enclosed volume.

#### Fixed-volume capillary spectrum of a cylindrical membrane

↑ **Parent:** [Lipid vesicle](#lipid-vesicle)

For a tension-dominated cylindrical [lipid vesicle](#lipid-vesicle) of fixed length $L$ and volume, a real axisymmetric sine amplitude $u_q$ has stiffness $K_q=\pi\sigma L[(qR_0)^2-1]/R_0$. Fixed volume requires a mean-radius shift $-u_q^2/(4R_0)$. Stable modes have $\langle u_q^2\rangle=k_BT/K_q$ by the [equipartition theorem](statistical-physics.md#equipartition-theorem). Modes with $qR_0<1$ have the [Rayleigh–Plateau instability](fluid-mechanics.md#rayleigh-plateau-instability), rather than a negative equilibrium variance. Bending modifies very short wavelengths and near-marginal modes.

#### Axisymmetric membrane deformation

↑ **Parent:** [Lipid vesicle](#lipid-vesicle)

An axisymmetric cylindrical membrane deformation is invariant under rotations about the cylinder axis, so its radius depends only on the axial coordinate. Its [surface area](differential-geometry.md#surface-area) is $2\pi\int R\sqrt{1+R_z^2}\,dz$, and its enclosed volume is $\pi\int R^2\,dz$. These scalar shape constraints are the basis of the [fixed-volume capillary spectrum of a cylindrical membrane](#fixed-volume-capillary-spectrum-of-a-cylindrical-membrane).

### Interaction between lipid bilayers

↑ **Parent:** [Lipid bilayer](#lipid-bilayer)

Nearby lipid bilayers experience attractive van der Waals forces, screened electrostatic repulsion, and fluctuation-induced steric repulsion.

#### Hamaker constant

↑ **Parent:** [Interaction between lipid bilayers](#interaction-between-lipid-bilayers)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hamaker_constant)

The Hamaker constant sets the strength of pairwise-summed van der Waals attraction between macroscopic bodies across a medium.

<h4 id="debye-huckel-screening-length">Debye–Hückel screening length</h4>

↑ **Parent:** [Interaction between lipid bilayers](#interaction-between-lipid-bilayers)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Debye–Hückel_screening_length)

The Debye–Hückel screening length is the distance over which mobile ions suppress an electrostatic potential in the linearized electrolyte theory.

#### Helfrich repulsion

↑ **Parent:** [Interaction between lipid bilayers](#interaction-between-lipid-bilayers)

Helfrich repulsion is the entropic interaction produced when neighboring membranes suppress each other's thermal undulations. Its free energy per area scales as $(k_BT)^2/(k_cd^2)$.

#### Membrane unbinding transition

↑ **Parent:** [Interaction between lipid bilayers](#interaction-between-lipid-bilayers)

A membrane unbinding transition sends the equilibrium layer spacing to infinity. In a dilute lamellar stack, competition between a quadratic virial attraction and cubic Helfrich repulsion gives a continuous transition with spacing exponent one.

### Helfrich energy

↑ **Parent:** [Lipid bilayer](#lipid-bilayer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Helfrich_energy)

The Helfrich energy of a fluid membrane combines surface tension with curvature elasticity. Without spontaneous curvature or a topological term,

$$
E=\int dS\left[\sigma+\frac{k_c}{2}(2H)^2\right].
$$

#### Thermal membrane undulation

↑ **Parent:** [Helfrich energy](#helfrich-energy)

A thermal membrane undulation is a shape fluctuation excited by thermal energy. In a planar membrane, a Fourier mode has stiffness $k_cq^4+\sigma q^2$, so tension suppresses long-wavelength excess area while bending suppresses short wavelengths.

#### Membrane bending modulus

↑ **Parent:** [Helfrich energy](#helfrich-energy)

The membrane bending modulus sets the energy cost of curvature. A larger $k_c$ suppresses thermal undulations and resists wrapping around small objects.

#### Membrane tension

↑ **Parent:** [Helfrich energy](#helfrich-energy)

Membrane tension is the free-energy cost per added projected area. Together with bending elasticity it selects a length scale and controls the radius of a pulled membrane tube.

#### Membrane elastic length

↑ **Parent:** [Helfrich energy](#helfrich-energy)

The membrane elastic length is the distance over which bending-dominated deformation relaxes under tension. In a small-slope one-dimensional membrane it is $\xi=\sqrt{k_c/\sigma}$.

#### Small-slope elastic membrane energy

↑ **Parent:** [Helfrich energy](#helfrich-energy)

For a nearly flat membrane represented by height $h(x)$, the quadratic bending-and-tension energy per invariant transverse length is

$$
E=\frac12\int\left(k_ch_{xx}^2+\sigma h_x^2\right)dx.
$$

Its free equilibrium equation is $k_ch_{xxxx}-\sigma h_{xx}=0$.

##### Capillary height-difference correlation

↑ **Parent:** [Small-slope elastic membrane energy](#small-slope-elastic-membrane-energy)

For a tension-dominated membrane with internal dimension $D$, the massless Gaussian height [covariance](variance.md#covariance) has spectrum $k_BT/(\sigma q^2)$. Removing the uniform translation mode leaves the height difference well-defined. Its [variance](variance.md) grows linearly with distance for $D=1$, logarithmically for $D=2$, and approaches a cutoff-dependent constant for $D>2$. A microscopic cutoff is necessary when the short-distance integral diverges. This distinguishes rough positional order from a failure of the local small-slope approximation.

###### Pinned capillary-wave correlation

↑ **Parent:** [Capillary height-difference correlation](#capillary-height-difference-correlation)

Adding positive quadratic confinement $t\int h^2/2$ to the membrane energy changes its height spectrum to $k_BT/(\sigma q^2+t)$. The continuous height-shift [symmetry](physics.md#symmetry-physics) is explicitly broken. [Connected correlation function](critical-phenomenon.md#connected-correlation-function) decay on the finite length $\xi$ and the height-difference [variance](variance.md) saturates for every internal dimension, although its saturation value can depend on a microscopic cutoff. A negative confinement coefficient gives an unstable quadratic model rather than pinning.

##### Dimensionless adhesion strength

↑ **Parent:** [Small-slope elastic membrane energy](#small-slope-elastic-membrane-energy)

For a membrane of bending modulus $k_c$ adhering with energy per area $\mathcal U$ to a cylinder of radius $R$, $U=R^2\mathcal U/k_c$ compares adhesion with bending cost.

##### Membrane-mediated interaction potential

↑ **Parent:** [Small-slope elastic membrane energy](#small-slope-elastic-membrane-energy)

A membrane-mediated interaction potential is the separation-dependent energy produced when deformation fields around two membrane-bound objects overlap. Its sign and range depend on membrane tension, bending stiffness, inclusion geometry, and which side of the membrane each object occupies.

#### Cylindrical membrane equilibrium radius

↑ **Parent:** [Helfrich energy](#helfrich-energy)

Minimizing the [Helfrich energy](#helfrich-energy) per length of an unconstrained cylindrical membrane gives $r_0=\sqrt{k_c/(2\sigma)}$, balancing the area cost against bending curvature.

<h5 id="entropic-membrane-tether-force-extension-relation">Entropic membrane-tether force--extension relation</h5>

↑ **Parent:** [Cylindrical membrane equilibrium radius](#cylindrical-membrane-equilibrium-radius)

When a tether draws area from the thermal undulations of a finite vesicle, extension raises membrane tension rather than drawing area from a fixed-tension reservoir. The tether therefore narrows and its required pulling force increases with length.

<h4 id="fluctuation-supported-membrane-particle-gap">Fluctuation-supported membrane--particle gap</h4>

↑ **Parent:** [Helfrich energy](#helfrich-energy)

Thermal membrane undulations generate [Helfrich repulsion](#helfrich-repulsion) from a nearby particle. For a sphere of radius $R$ tightly enclosed by a high-tension membrane,

$$
\delta\simeq\left(\frac{(k_BT)^2R}{64k_c\sigma}\right)^{1/3}.
$$

##### Confined-sphere drag coefficient

↑ **Parent:** [Fluctuation-supported membrane--particle gap](#fluctuation-supported-membrane-particle-gap)

For a sphere of radius $R$ moving through a membrane tube with a uniform narrow gap $\delta\ll R$, [lubrication theory](viscous-fluid-flow.md#lubrication-theory) gives

$$
\zeta_{\rm tube}\simeq\frac{12\pi\mu R^3}{\delta^2}.
$$

It exceeds the unbounded-fluid [Stokes drag law](stokes-flow.md#stokes-s-law) coefficient by $2R^2/\delta^2$.

## ↑ Ancestors (3)

1. [Branches of physics](physics.md#branches-of-physics)
2. [Physics](physics.md)
3. [Codex Wiki](README.md)
