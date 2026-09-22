# Partial differential equation

↑ **Parent:** [Analysis](analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Partial_differential_equation)

A partial differential equation relates a multivariable function to its partial derivatives.

**Table of contents**

- [Kuramoto-Sivashinsky equation](#kuramoto-sivashinsky-equation)
  - [Primary periodic bifurcation of the Kuramoto-Sivashinsky equation](#primary-periodic-bifurcation-of-the-kuramoto-sivashinsky-equation)
- [Green's identities](#green-s-identities)
  - [Green's third identity](#green-s-third-identity)
  - [Green's first identity](#green-s-first-identity)
    - [Gradient pairing with a boundary-constant function and a harmonic function](#gradient-pairing-with-a-boundary-constant-function-and-a-harmonic-function)
      - [Boundary flux from a singular harmonic potential](#boundary-flux-from-a-singular-harmonic-potential)
- [Maximum principle](#maximum-principle)
  - [Strong maximum principle for harmonic functions](#strong-maximum-principle-for-harmonic-functions)
  - [Maximum principle for harmonic functions](#maximum-principle-for-harmonic-functions)
- [Burgers' equation](#burgers-equation)
  - [Viscous Burgers equation](#viscous-burgers-equation)
    - [Modified Burgers equation with cubic flux](#modified-burgers-equation-with-cubic-flux)
      - [Traveling front of the cubic-flux Burgers equation](#traveling-front-of-the-cubic-flux-burgers-equation)
    - [Fay solution](#fay-solution)
      - [Fay shock-layer asymptotics](#fay-shock-layer-asymptotics)
    - [Burgers N-wave](#burgers-n-wave)
      - [Cole-Hopf solution for a Burgers N-wave](#cole-hopf-solution-for-a-burgers-n-wave)
    - [Viscous Burgers step solution with negative flux](#viscous-burgers-step-solution-with-negative-flux)
      - [Midpoint symmetry of a viscous Burgers step](#midpoint-symmetry-of-a-viscous-burgers-step)
    - [Cole-Hopf transformation](#cole-hopf-transformation)
      - [Sinusoidal Cole-Hopf solution for negative-flux Burgers flow](#sinusoidal-cole-hopf-solution-for-negative-flux-burgers-flow)
      - [Finite-exponential Cole-Hopf solution](#finite-exponential-cole-hopf-solution)
        - [Extremal-state asymptotics of exponential Burgers solutions](#extremal-state-asymptotics-of-exponential-burgers-solutions)
- [Semilinear partial differential equation](#semilinear-partial-differential-equation)
  - [Semilinear heat equation](#semilinear-heat-equation)
- [Obstacle problem](#obstacle-problem)
- [Parabolic comparison principle](#parabolic-comparison-principle)
  - [Invariant interval for a cubic reaction-diffusion equation](#invariant-interval-for-a-cubic-reaction-diffusion-equation)
- [Domain of dependence](#domain-of-dependence)
- [Linear partial differential equation](#linear-partial-differential-equation)
- [Ill-posed problem](#ill-posed-problem)
- [Linear partial differential operator](#linear-partial-differential-operator)
- [Liouville equation](#liouville-equation)
- [Radial function](#radial-function)
- [Periodic domain](#periodic-domain)
- [Energy estimate](#energy-estimate)
  - [Bootstrap argument](#bootstrap-argument)
  - [Wave energy estimate](#wave-energy-estimate)
    - [Local wave energy estimate](#local-wave-energy-estimate)
  - [Hole-filling argument](#hole-filling-argument)
    - [Dyadic energy decay](#dyadic-energy-decay)
  - [Signed power test for a Laplacian eigenfunction](#signed-power-test-for-a-laplacian-eigenfunction)
  - [Caccioppoli inequality](#caccioppoli-inequality)
    - [Caccioppoli inequality with bounded lower-order terms](#caccioppoli-inequality-with-bounded-lower-order-terms)
      - [Strong local Sobolev compactness for a fixed elliptic equation](#strong-local-sobolev-compactness-for-a-fixed-elliptic-equation)
    - [Annular Caccioppoli inequality](#annular-caccioppoli-inequality)
    - [Power Caccioppoli inequality](#power-caccioppoli-inequality)
      - [Uniform power gain for elliptic solutions](#uniform-power-gain-for-elliptic-solutions)
    - [Logarithmic Caccioppoli inequality](#logarithmic-caccioppoli-inequality)
- [Second-order partial differential equation](#second-order-partial-differential-equation)
- [Quasilinear partial differential equation](#quasilinear-partial-differential-equation)
  - [Averaged linearization of a nonlinear divergence-form equation](#averaged-linearization-of-a-nonlinear-divergence-form-equation)
  - [p-Laplacian](#p-laplacian)
  - [Principal symbol of a partial differential equation](#principal-symbol-of-a-partial-differential-equation)
    - [Characteristic hypersurface](#characteristic-hypersurface)
      - [Characteristic plane](#characteristic-plane)
      - [Non-characteristic hypersurface](#non-characteristic-hypersurface)
      - [Characteristic coordinate](#characteristic-coordinate)
        - [Expanding-flow transformation of a wave equation](#expanding-flow-transformation-of-a-wave-equation)
    - [Hyperbolic partial differential equation](#hyperbolic-partial-differential-equation)
      - [Hyperbolicity](#hyperbolicity)
      - [Travel-time coordinate for a one-dimensional variable-speed wave equation](#travel-time-coordinate-for-a-one-dimensional-variable-speed-wave-equation)
        - [Characteristic curves for speed one minus y squared](#characteristic-curves-for-speed-one-minus-y-squared)
- [Cauchy problem](#cauchy-problem)
  - [Noncharacteristic Cauchy data](#noncharacteristic-cauchy-data)
  - [Continuous dependence on initial data](#continuous-dependence-on-initial-data)
  - [Cauchy data](#cauchy-data)
    - [Boundary jet](#boundary-jet)
  - [Cauchy-Kovalevskaya theorem](#cauchy-kovalevskaya-theorem)
    - [Holmgren uniqueness theorem](#holmgren-uniqueness-theorem)
      - [Parabolic-cap proof of Holmgren uniqueness](#parabolic-cap-proof-of-holmgren-uniqueness)
    - [Uniform Cauchy radius for polynomial forcing](#uniform-cauchy-radius-for-polynomial-forcing)
    - [General-order Cauchy-Kovalevskaya theorem](#general-order-cauchy-kovalevskaya-theorem)
    - [Analytic Goursat problem for a Klein--Gordon equation](#analytic-goursat-problem-for-a-klein-gordon-equation)
      - [Global continuation for the analytic Goursat problem](#global-continuation-for-the-analytic-goursat-problem)
- [Solution of a partial differential equation](#solution-of-a-partial-differential-equation)
  - [Classical solution](#classical-solution)
    - [Positive-time smoothing for a semilinear heat equation](#positive-time-smoothing-for-a-semilinear-heat-equation)
    - [Bounded parabolic differentiability class](#bounded-parabolic-differentiability-class)
  - [Weak solution](#weak-solution)
    - [Viscosity solution](#viscosity-solution)
      - [Continuous viscosity harmonic functions are classical](#continuous-viscosity-harmonic-functions-are-classical)
    - [Weak-strong uniqueness principle](#weak-strong-uniqueness-principle)
    - [Weak energy solution of a variable-coefficient wave equation](#weak-energy-solution-of-a-variable-coefficient-wave-equation)
    - [Weak formulation](#weak-formulation)
    - [Galerkin method](#galerkin-method)
      - [Fourier truncation](#fourier-truncation)
      - [Aubin-Lions lemma](#aubin-lions-lemma)
        - [Weak continuity from evolution-space bounds](#weak-continuity-from-evolution-space-bounds)
          - [Strong continuity from weak continuity and an energy equality](#strong-continuity-from-weak-continuity-and-an-energy-equality)
- [Transport equation](#transport-equation)
  - [Compact third-order advection stencil](#compact-third-order-advection-stencil)
  - [Hamiltonian transport equation](#hamiltonian-transport-equation)
    - [Casimir invariant of a transport equation](#casimir-invariant-of-a-transport-equation)
  - [Commuting velocity derivative for kinetic transport](#commuting-velocity-derivative-for-kinetic-transport)
  - [Dispersion with a nonlinear velocity map](#dispersion-with-a-nonlinear-velocity-map)
  - [Free transport equation](#free-transport-equation)
    - [Free transport dispersion](#free-transport-dispersion)
    - [Absolutely continuous representative along free characteristics](#absolutely-continuous-representative-along-free-characteristics)
    - [Free-transport semigroup](#free-transport-semigroup)
  - [Characteristic curve](#characteristic-curve)
    - [Characteristic flow map](#characteristic-flow-map)
      - [Phase-space flow Jacobian](#phase-space-flow-jacobian)
      - [Global characteristic flow under linear growth](#global-characteristic-flow-under-linear-growth)
    - [Method of characteristics](#method-of-characteristics)
      - [Weighted Euler first-order equation](#weighted-euler-first-order-equation)
      - [Fold tangency obstruction for characteristic data](#fold-tangency-obstruction-for-characteristic-data)
      - [Characteristic equations for a transport equation](#characteristic-equations-for-a-transport-equation)
  - [Linear transport equation](#linear-transport-equation)
    - [Transport of a Dirac point mass](#transport-of-a-dirac-point-mass)
    - [Coercive energy estimate for kinetic transport](#coercive-energy-estimate-for-kinetic-transport)
    - [Lp conservation for incompressible transport](#lp-conservation-for-incompressible-transport)
    - [Inflow transport boundary condition](#inflow-transport-boundary-condition)
      - [Corner compatibility for constant-speed transport](#corner-compatibility-for-constant-speed-transport)
    - [Weak transport solution under characteristic coordinates](#weak-transport-solution-under-characteristic-coordinates)
    - [Adjoint transport equation](#adjoint-transport-equation)
  - [System of conservation laws](#system-of-conservation-laws)
    - [Riemann problem](#riemann-problem)
      - [Single-rarefaction matching conditions for an ideal-gas Riemann problem](#single-rarefaction-matching-conditions-for-an-ideal-gas-riemann-problem)
      - [Contact discontinuity](#contact-discontinuity)
    - [Conservation law flux](#conservation-law-flux)
    - [Quasilinear system](#quasilinear-system)
      - [Hyperbolic system](#hyperbolic-system)
    - [Flux Jacobian](#flux-jacobian)
      - [Characteristic speed](#characteristic-speed)
        - [Kinematic wave](#kinematic-wave)
  - [Scalar conservation law](#scalar-conservation-law)
    - [Sonic point of a scalar flux](#sonic-point-of-a-scalar-flux)
    - [Uniformly convex scalar flux](#uniformly-convex-scalar-flux)
    - [Viscous scalar conservation law](#viscous-scalar-conservation-law)
      - [Vanishing viscosity approximation](#vanishing-viscosity-approximation)
    - [Maximum representation for a concave conservation law](#maximum-representation-for-a-concave-conservation-law)
      - [Square-root decay before characteristic crossing](#square-root-decay-before-characteristic-crossing)
    - [Characteristic solution of a scalar conservation law](#characteristic-solution-of-a-scalar-conservation-law)
    - [Concave-flux characteristic lifespan](#concave-flux-characteristic-lifespan)
    - [Bounded-derivative Burgers flux](#bounded-derivative-burgers-flux)
    - [Shock wave](#shock-wave)
      - [Rankine-Hugoniot conditions](#rankine-hugoniot-conditions)
      - [Entropy shock](#entropy-shock)
    - [Rarefaction wave](#rarefaction-wave)
      - [Self-similar ideal-gas rarefaction](#self-similar-ideal-gas-rarefaction)
    - [Inviscid Burgers equation](#inviscid-burgers-equation)
      - [Periodic backward-sawtooth Burgers solution](#periodic-backward-sawtooth-burgers-solution)
      - [Burgers Riemann problem with negative flux](#burgers-riemann-problem-with-negative-flux)
      - [Entropy solution](#entropy-solution)
        - [Kruzhkov entropy inequality](#kruzhkov-entropy-inequality)
        - [Discrete entropy inequality](#discrete-entropy-inequality)
        - [Averaged initial trace of an entropy solution](#averaged-initial-trace-of-an-entropy-solution)
        - [Entropy flux for a scalar conservation law](#entropy-flux-for-a-scalar-conservation-law)
          - [Kruzhkov entropy flux](#kruzhkov-entropy-flux)
            - [Doubling of variables for scalar conservation laws](#doubling-of-variables-for-scalar-conservation-laws)
              - [Kato inequality for scalar conservation laws](#kato-inequality-for-scalar-conservation-laws)
                - [Local L1 contraction for scalar conservation laws](#local-l1-contraction-for-scalar-conservation-laws)
                  - [Order preservation for scalar entropy solutions](#order-preservation-for-scalar-entropy-solutions)
    - [Characteristic crossing](#characteristic-crossing)
      - [Gradient blow-up](#gradient-blow-up)
- [Elliptic boundary value problem](elliptic-boundary-value-problem.md)
  - [Direct spherical-shell H2 estimate](elliptic-boundary-value-problem.md#direct-spherical-shell-h2-estimate)
  - [Dirichlet realization of an elliptic operator](elliptic-boundary-value-problem.md#dirichlet-realization-of-an-elliptic-operator)
  - [Nonlinear elliptic boundary value problem](elliptic-boundary-value-problem.md#nonlinear-elliptic-boundary-value-problem)
    - [Ordered subsolution and supersolution](elliptic-boundary-value-problem.md#ordered-subsolution-and-supersolution)
      - [Monotone iteration for a semilinear elliptic equation](elliptic-boundary-value-problem.md#monotone-iteration-for-a-semilinear-elliptic-equation)
    - [Small-data existence for a nonlinear elliptic Dirichlet problem](elliptic-boundary-value-problem.md#small-data-existence-for-a-nonlinear-elliptic-dirichlet-problem)
    - [Cubic gradient nonlinearity](elliptic-boundary-value-problem.md#cubic-gradient-nonlinearity)
  - [Fredholm alternative for an elliptic Dirichlet problem](elliptic-boundary-value-problem.md#fredholm-alternative-for-an-elliptic-dirichlet-problem)
    - [Small positive zeroth-order perturbation of a Dirichlet problem](elliptic-boundary-value-problem.md#small-positive-zeroth-order-perturbation-of-a-dirichlet-problem)
    - [Boundary compatibility in the self-adjoint Fredholm alternative](elliptic-boundary-value-problem.md#boundary-compatibility-in-the-self-adjoint-fredholm-alternative)
  - [Uniformly elliptic operator](elliptic-boundary-value-problem.md#uniformly-elliptic-operator)
    - [Quadratic ellipticity does not bound a nonsymmetric coefficient matrix](elliptic-boundary-value-problem.md#quadratic-ellipticity-does-not-bound-a-nonsymmetric-coefficient-matrix)
    - [Nondivergence-form elliptic operator](elliptic-boundary-value-problem.md#nondivergence-form-elliptic-operator)
    - [Divergence-form elliptic operator](elliptic-boundary-value-problem.md#divergence-form-elliptic-operator)
      - [Constant flux for a one-dimensional divergence-form equation](elliptic-boundary-value-problem.md#constant-flux-for-a-one-dimensional-divergence-form-equation)
      - [Constant shifts of a divergence-form equation](elliptic-boundary-value-problem.md#constant-shifts-of-a-divergence-form-equation)
      - [Homogeneous divergence-form elliptic equation](elliptic-boundary-value-problem.md#homogeneous-divergence-form-elliptic-equation)
      - [Weak supersolution of a divergence-form elliptic equation](elliptic-boundary-value-problem.md#weak-supersolution-of-a-divergence-form-elliptic-equation)
      - [Weak subsolution of a divergence-form elliptic equation](elliptic-boundary-value-problem.md#weak-subsolution-of-a-divergence-form-elliptic-equation)
        - [Local boundedness of weak elliptic subsolutions](elliptic-boundary-value-problem.md#local-boundedness-of-weak-elliptic-subsolutions)
    - [Strict positivity implies coercivity for an elliptic Dirichlet form](elliptic-boundary-value-problem.md#strict-positivity-implies-coercivity-for-an-elliptic-dirichlet-form)
    - [Constant-coefficient elliptic second-derivative estimate](elliptic-boundary-value-problem.md#constant-coefficient-elliptic-second-derivative-estimate)
      - [Perturbation of a constant-coefficient elliptic second-derivative estimate](elliptic-boundary-value-problem.md#perturbation-of-a-constant-coefficient-elliptic-second-derivative-estimate)
        - [Coefficient-freezing interior second-derivative estimate](elliptic-boundary-value-problem.md#coefficient-freezing-interior-second-derivative-estimate)
          - [Interior H2 regularity for continuous nondivergence coefficients](elliptic-boundary-value-problem.md#interior-h2-regularity-for-continuous-nondivergence-coefficients)
    - [Strictly elliptic operator](elliptic-boundary-value-problem.md#strictly-elliptic-operator)
    - [Weak maximum principle for elliptic operators](elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators)
      - [Maximum bound for a monotone reaction term](elliptic-boundary-value-problem.md#maximum-bound-for-a-monotone-reaction-term)
      - [Supremum norm barrier for an elliptic Dirichlet problem](elliptic-boundary-value-problem.md#supremum-norm-barrier-for-an-elliptic-dirichlet-problem)
      - [Strong maximum principle for elliptic operators](elliptic-boundary-value-problem.md#strong-maximum-principle-for-elliptic-operators)
      - [Exponential perturbation proof of the weak maximum principle with drift](elliptic-boundary-value-problem.md#exponential-perturbation-proof-of-the-weak-maximum-principle-with-drift)
      - [Failure of the weak maximum principle with a positive zeroth-order coefficient](elliptic-boundary-value-problem.md#failure-of-the-weak-maximum-principle-with-a-positive-zeroth-order-coefficient)
      - [Alexandrov–Bakelman–Pucci estimate](elliptic-boundary-value-problem.md#alexandrov-bakelman-pucci-estimate)
      - [Strong minimum principle for elliptic operators](elliptic-boundary-value-problem.md#strong-minimum-principle-for-elliptic-operators)
    - [Schauder estimates](elliptic-boundary-value-problem.md#schauder-estimates)
      - [Interpolation inequality in Holder spaces](elliptic-boundary-value-problem.md#interpolation-inequality-in-holder-spaces)
      - [Interior Schauder estimate](elliptic-boundary-value-problem.md#interior-schauder-estimate)
        - [Necessity of Hölder forcing for Schauder estimates](elliptic-boundary-value-problem.md#necessity-of-holder-forcing-for-schauder-estimates)
        - [Blow-up compactness proof of an interior Schauder estimate](elliptic-boundary-value-problem.md#blow-up-compactness-proof-of-an-interior-schauder-estimate)
          - [Taylor normalization in elliptic blow-up arguments](elliptic-boundary-value-problem.md#taylor-normalization-in-elliptic-blow-up-arguments)
      - [Boundary Schauder estimate](elliptic-boundary-value-problem.md#boundary-schauder-estimate)
        - [Global Schauder estimate](elliptic-boundary-value-problem.md#global-schauder-estimate)
          - [Compactness of zero-boundary Poisson solutions](elliptic-boundary-value-problem.md#compactness-of-zero-boundary-poisson-solutions)
          - [Compactness proof of a nonnegative elliptic solution estimate](elliptic-boundary-value-problem.md#compactness-proof-of-a-nonnegative-elliptic-solution-estimate)
      - [Simon absorption lemma](elliptic-boundary-value-problem.md#simon-absorption-lemma)
    - [De Giorgi-Nash-Moser theorem](elliptic-boundary-value-problem.md#de-giorgi-nash-moser-theorem)
      - [Compactness of normalized weak elliptic solutions](elliptic-boundary-value-problem.md#compactness-of-normalized-weak-elliptic-solutions)
      - [Moser iteration](elliptic-boundary-value-problem.md#moser-iteration)
        - [Moser product on geometric radii](elliptic-boundary-value-problem.md#moser-product-on-geometric-radii)
        - [Liouville theorem for integrable nonnegative elliptic subsolutions](elliptic-boundary-value-problem.md#liouville-theorem-for-integrable-nonnegative-elliptic-subsolutions)
        - [Weak Harnack inequality](elliptic-boundary-value-problem.md#weak-harnack-inequality)
          - [Propagation of zeros by the weak Harnack inequality](elliptic-boundary-value-problem.md#propagation-of-zeros-by-the-weak-harnack-inequality)
          - [Oscillation decay estimate](elliptic-boundary-value-problem.md#oscillation-decay-estimate)
            - [Inhomogeneous oscillation decay implies Hölder continuity](elliptic-boundary-value-problem.md#inhomogeneous-oscillation-decay-implies-holder-continuity)
          - [Harnack inequality for uniformly elliptic divergence-form equations](elliptic-boundary-value-problem.md#harnack-inequality-for-uniformly-elliptic-divergence-form-equations)
  - [Degenerate elliptic operator](elliptic-boundary-value-problem.md#degenerate-elliptic-operator)
    - [Sine-mode expansion for a quadratically degenerate elliptic equation](elliptic-boundary-value-problem.md#sine-mode-expansion-for-a-quadratically-degenerate-elliptic-equation)
      - [Forced zero trace at a quadratically degenerate boundary](elliptic-boundary-value-problem.md#forced-zero-trace-at-a-quadratically-degenerate-boundary)
    - [Failure of a coercive Dirichlet estimate under degeneracy](elliptic-boundary-value-problem.md#failure-of-a-coercive-dirichlet-estimate-under-degeneracy)
  - [Method of continuity](elliptic-boundary-value-problem.md#method-of-continuity)
  - [Hopf lemma](elliptic-boundary-value-problem.md#hopf-lemma)
    - [Hopf dichotomy with classical regularity away from the zero set](elliptic-boundary-value-problem.md#hopf-dichotomy-with-classical-regularity-away-from-the-zero-set)
    - [Interior sphere condition](elliptic-boundary-value-problem.md#interior-sphere-condition)
- [Helmholtz equation](#helmholtz-equation)
  - [Helmholtz Green-function reciprocity](#helmholtz-green-function-reciprocity)
  - [Discrete Helmholtz resonance](#discrete-helmholtz-resonance)
  - [Dirichlet-to-Neumann map for a Helmholtz half-space](#dirichlet-to-neumann-map-for-a-helmholtz-half-space)
  - [Outgoing Green function for the three-dimensional Helmholtz equation](#outgoing-green-function-for-the-three-dimensional-helmholtz-equation)
    - [Weyl plane-wave representation](#weyl-plane-wave-representation)
  - [Wave scattering at a planar interface](#wave-scattering-at-a-planar-interface)
    - [Vertical wavenumber](#vertical-wavenumber)
    - [Snell's law](#snell-s-law)
    - [Scalar-wave interface condition](#scalar-wave-interface-condition)
    - [Reflection and transmission coefficients at a scalar-wave interface](#reflection-and-transmission-coefficients-at-a-scalar-wave-interface)
      - [Reflection coefficient](#reflection-coefficient)
      - [Transmission coefficient](#transmission-coefficient)
  - [Phase screen](#phase-screen)
    - [Phase-to-intensity conversion near a deterministic phase screen](#phase-to-intensity-conversion-near-a-deterministic-phase-screen)
    - [Random phase screen](#random-phase-screen)
      - [Stationary phase-screen power spectrum](#stationary-phase-screen-power-spectrum)
      - [Gaussian phase-screen correlation](#gaussian-phase-screen-correlation)
      - [Gaussian phase averaging](#gaussian-phase-averaging)
    - [Parabolic wave equation](#parabolic-wave-equation)
      - [Stationary intensity under free paraxial propagation](#stationary-intensity-under-free-paraxial-propagation)
      - [Mutual coherence in a white-noise parabolic medium](#mutual-coherence-in-a-white-noise-parabolic-medium)
      - [Norm conservation for the scalar parabolic wave equation](#norm-conservation-for-the-scalar-parabolic-wave-equation)
      - [Colored Gaussian paraxial mean propagator](#colored-gaussian-paraxial-mean-propagator)
      - [Paraxial approximation](#paraxial-approximation)
      - [Split-step Fourier method](#split-step-fourier-method)
      - [Free-space diffraction](#free-space-diffraction)
        - [Sommerfeld half-plane diffraction](#sommerfeld-half-plane-diffraction)
          - [Wiener-Hopf solution of rigid half-plane diffraction](#wiener-hopf-solution-of-rigid-half-plane-diffraction)
        - [Fresnel propagator](#fresnel-propagator)
          - [One-dimensional transverse Fresnel propagation](#one-dimensional-transverse-fresnel-propagation)
        - [Free-space fourth-moment propagator](#free-space-fourth-moment-propagator)
    - [Coherent and diffuse wave fields](#coherent-and-diffuse-wave-fields)
      - [Coherent attenuation by a Gaussian phase screen](#coherent-attenuation-by-a-gaussian-phase-screen)
      - [Coherent attenuation in a white-noise random medium](#coherent-attenuation-in-a-white-noise-random-medium)
    - [Phase curvature](#phase-curvature)
- [Modified Helmholtz equation](#modified-helmholtz-equation)
  - [Quadrant modified Helmholtz Dirichlet Poisson formula](#quadrant-modified-helmholtz-dirichlet-poisson-formula)
  - [Modified Helmholtz closed spectral one-form](#modified-helmholtz-closed-spectral-one-form)
  - [Two-dimensional modified Helmholtz fundamental solution](#two-dimensional-modified-helmholtz-fundamental-solution)
  - [Modified Helmholtz adjoint plane wave](#modified-helmholtz-adjoint-plane-wave)
    - [Side localization of modified Helmholtz plane waves](#side-localization-of-modified-helmholtz-plane-waves)
  - [Radial modified Helmholtz equation](#radial-modified-helmholtz-equation)
- [Poisson equation](#poisson-equation)
  - [Poisson equation on a disk with angular forcing](#poisson-equation-on-a-disk-with-angular-forcing)
  - [Neumann Poisson problem](#neumann-poisson-problem)
  - [Radial Poisson gradient estimate](#radial-poisson-gradient-estimate)
    - [Failure of L2-to-Linfinity Poisson gradient bounds in three dimensions](#failure-of-l2-to-linfinity-poisson-gradient-bounds-in-three-dimensions)
  - [Poisson kernel for the upper half-space](#poisson-kernel-for-the-upper-half-space)
    - [Poisson kernel for the upper half-plane](#poisson-kernel-for-the-upper-half-plane)
    - [Poisson integral](#poisson-integral)
      - [Dirichlet Poisson integral in a quadrant](#dirichlet-poisson-integral-in-a-quadrant)
        - [Bounded Dirichlet uniqueness in a quadrant](#bounded-dirichlet-uniqueness-in-a-quadrant)
        - [Zero-boundary harmonic growth in a quadrant](#zero-boundary-harmonic-growth-in-a-quadrant)
        - [Holomorphic derivative of a quadrant Dirichlet solution](#holomorphic-derivative-of-a-quadrant-dirichlet-solution)
      - [Schwarz integral formula](#schwarz-integral-formula)
        - [Schwarz integral on the unit disk](#schwarz-integral-on-the-unit-disk)
        - [Harmonic quadrant solution from tangential boundary derivatives](#harmonic-quadrant-solution-from-tangential-boundary-derivatives)
- [Nonlinear partial differential equation](#nonlinear-partial-differential-equation)
  - [Nonlinear Schrödinger equation](#nonlinear-schrodinger-equation)
  - [Complex Ginzburg–Landau equation](#complex-ginzburg-landau-equation)
    - [Benjamin-Feir stability condition](#benjamin-feir-stability-condition)
      - [Long-wave phase reduction of the complex Ginzburg-Landau equation](#long-wave-phase-reduction-of-the-complex-ginzburg-landau-equation)
    - [Real-coefficient cubic-quintic amplitude equation](#real-coefficient-cubic-quintic-amplitude-equation)
      - [Stationary front of a cubic-quintic amplitude equation](#stationary-front-of-a-cubic-quintic-amplitude-equation)
    - [Nonlinear Ginzburg-Landau equation](#nonlinear-ginzburg-landau-equation)
      - [Ginzburg-Landau plane wave](#ginzburg-landau-plane-wave)
        - [Cubic amplitude saturation](#cubic-amplitude-saturation)
    - [Linear complex Ginzburg-Landau equation](#linear-complex-ginzburg-landau-equation)
      - [Airy global modes of a linearly confined Ginzburg-Landau equation](#airy-global-modes-of-a-linearly-confined-ginzburg-landau-equation)
      - [Green function of the linear complex Ginzburg-Landau equation](#green-function-of-the-linear-complex-ginzburg-landau-equation)
    - [Radial flow near a driven vortex core](#radial-flow-near-a-driven-vortex-core)
- [Moving-boundary problem](#moving-boundary-problem)
- [Diffusion equation](diffusion-equation.md)
  - [Diffusive time scale](diffusion-equation.md#diffusive-time-scale)
  - [Variable-coefficient conservative diffusion equation](diffusion-equation.md#variable-coefficient-conservative-diffusion-equation)
  - [Infinite propagation speed](diffusion-equation.md#infinite-propagation-speed)
  - [Periodic homogenization of a diffusion equation](diffusion-equation.md#periodic-homogenization-of-a-diffusion-equation)
  - [Porous medium equation](diffusion-equation.md#porous-medium-equation)
    - [Spherical nonlinear-diffusion source profile](diffusion-equation.md#spherical-nonlinear-diffusion-source-profile)
    - [Compact radial cubic-diffusion profile](diffusion-equation.md#compact-radial-cubic-diffusion-profile)
    - [Finite propagation in porous-medium diffusion](diffusion-equation.md#finite-propagation-in-porous-medium-diffusion)
    - [Forced filling similarity for power-law diffusion](diffusion-equation.md#forced-filling-similarity-for-power-law-diffusion)
    - [Separable draining profile for power-law diffusion](diffusion-equation.md#separable-draining-profile-for-power-law-diffusion)
    - [Barenblatt solution](diffusion-equation.md#barenblatt-solution)
      - [Radial cubic-diffusion source profile](diffusion-equation.md#radial-cubic-diffusion-source-profile)
      - [Planar volume-conserving nonlinear-diffusion similarity](diffusion-equation.md#planar-volume-conserving-nonlinear-diffusion-similarity)
        - [Semicircular pulse under cubic diffusion](diffusion-equation.md#semicircular-pulse-under-cubic-diffusion)
      - [Two-dimensional Barenblatt profile for quadratic porous-medium diffusion](diffusion-equation.md#two-dimensional-barenblatt-profile-for-quadratic-porous-medium-diffusion)
  - [Fick's first law](diffusion-equation.md#fick-s-first-law)
  - [Heat equation](diffusion-equation.md#heat-equation)
    - [Reaction-diffusion spectral decay threshold](diffusion-equation.md#reaction-diffusion-spectral-decay-threshold)
    - [Heat evolution of bounded data need not converge at large times](diffusion-equation.md#heat-evolution-of-bounded-data-need-not-converge-at-large-times)
    - [Dirichlet heat-reaction threshold on the unit square](diffusion-equation.md#dirichlet-heat-reaction-threshold-on-the-unit-square)
    - [Heat operator](diffusion-equation.md#heat-operator)
    - [Heat-equation uniqueness under Gaussian growth](diffusion-equation.md#heat-equation-uniqueness-under-gaussian-growth)
    - [Backward heat equation](diffusion-equation.md#backward-heat-equation)
      - [Space-time harmonic functions along Brownian motion](diffusion-equation.md#space-time-harmonic-functions-along-brownian-motion)
    - [Heat equation maximum principle](diffusion-equation.md#heat-equation-maximum-principle)
    - [Heat equation energy identity](diffusion-equation.md#heat-equation-energy-identity)
    - [Dirichlet boundary-forcing heat-kernel formula](diffusion-equation.md#dirichlet-boundary-forcing-heat-kernel-formula)
      - [Half-line drift boundary kernel](diffusion-equation.md#half-line-drift-boundary-kernel)
    - [Dirichlet energy dissipation for the heat equation](diffusion-equation.md#dirichlet-energy-dissipation-for-the-heat-equation)
    - [Radial heat equation in three dimensions](diffusion-equation.md#radial-heat-equation-in-three-dimensions)
    - [Sinusoidally forced heat equation on a half-line](diffusion-equation.md#sinusoidally-forced-heat-equation-on-a-half-line)
    - [Potential Burgers equation](diffusion-equation.md#potential-burgers-equation)
    - [Heat kernel](diffusion-equation.md#heat-kernel)
      - [Heat kernel trace formula](diffusion-equation.md#heat-kernel-trace-formula)
      - [Positive diffusivity requirement for the forward heat kernel](diffusion-equation.md#positive-diffusivity-requirement-for-the-forward-heat-kernel)
      - [Heat-kernel convolution](diffusion-equation.md#heat-kernel-convolution)
      - [Riemannian heat kernel](diffusion-equation.md#riemannian-heat-kernel)
        - [Heat kernel on a finite isometric quotient](diffusion-equation.md#heat-kernel-on-a-finite-isometric-quotient)
          - [Heat semigroup descent through a finite normal covering](diffusion-equation.md#heat-semigroup-descent-through-a-finite-normal-covering)
        - [Spectral expansion of the Riemannian heat kernel](diffusion-equation.md#spectral-expansion-of-the-riemannian-heat-kernel)
        - [Heat parametrix](diffusion-equation.md#heat-parametrix)
          - [Heat-kernel transport equations](diffusion-equation.md#heat-kernel-transport-equations)
          - [Volterra parametrix correction](diffusion-equation.md#volterra-parametrix-correction)
      - [Gaussian interval mass](diffusion-equation.md#gaussian-interval-mass)
      - [Heat Poisson kernel](diffusion-equation.md#heat-poisson-kernel)
      - [Dirichlet heat kernel on an interval](diffusion-equation.md#dirichlet-heat-kernel-on-an-interval)
        - [Thermal trace of an interval image kernel](diffusion-equation.md#thermal-trace-of-an-interval-image-kernel)
      - [Gaussian heat kernel](diffusion-equation.md#gaussian-heat-kernel)
        - [Newtonian potential of the Brownian heat kernel](diffusion-equation.md#newtonian-potential-of-the-brownian-heat-kernel)
      - [Neumann heat kernel on an interval](diffusion-equation.md#neumann-heat-kernel-on-an-interval)
      - [Heat semigroup](diffusion-equation.md#heat-semigroup)
        - [Spectral construction of a parabolic solution](diffusion-equation.md#spectral-construction-of-a-parabolic-solution)
      - [Heat kernel expansion](diffusion-equation.md#heat-kernel-expansion)
        - [Heat invariants](diffusion-equation.md#heat-invariants)
          - [Integrated second scalar heat coefficient](diffusion-equation.md#integrated-second-scalar-heat-coefficient)
          - [Spectral determination of hyperbolic curvature on a surface](diffusion-equation.md#spectral-determination-of-hyperbolic-curvature-on-a-surface)
        - [Curvature coefficient of the scalar heat kernel](diffusion-equation.md#curvature-coefficient-of-the-scalar-heat-kernel)
        - [Normal-coordinate divergence-form heat parametrix](diffusion-equation.md#normal-coordinate-divergence-form-heat-parametrix)
      - [Gaussian approximate identity](diffusion-equation.md#gaussian-approximate-identity)
      - [Heat-kernel solution](diffusion-equation.md#heat-kernel-solution)
        - [Heat equation with interval-indicator initial data](diffusion-equation.md#heat-equation-with-interval-indicator-initial-data)
      - [Neumann heat kernel on a half-line](diffusion-equation.md#neumann-heat-kernel-on-a-half-line)
    - [Probabilistic representation of the heat equation with time-dependent Dirichlet data](diffusion-equation.md#probabilistic-representation-of-the-heat-equation-with-time-dependent-dirichlet-data)
    - [Duhamel's principle](diffusion-equation.md#duhamel-s-principle)
      - [Causal diffusion from a finite-duration planar point source](diffusion-equation.md#causal-diffusion-from-a-finite-duration-planar-point-source)
      - [Cancellation of two heat-kernel impulses](diffusion-equation.md#cancellation-of-two-heat-kernel-impulses)
  - [Advection-diffusion equation](diffusion-equation.md#advection-diffusion-equation)
    - [Homogenization of a periodic advection-diffusion equation](diffusion-equation.md#homogenization-of-a-periodic-advection-diffusion-equation)
    - [Transported step forcing in an advection-diffusion equation](diffusion-equation.md#transported-step-forcing-in-an-advection-diffusion-equation)
    - [Half-line advection-diffusion global relation](diffusion-equation.md#half-line-advection-diffusion-global-relation)
    - [Constant-flux tracer inlet solution](diffusion-equation.md#constant-flux-tracer-inlet-solution)
    - [Constant-concentration inlet solution](diffusion-equation.md#constant-concentration-inlet-solution)
    - [Dirichlet gauge transform for constant drift](diffusion-equation.md#dirichlet-gauge-transform-for-constant-drift)
      - [Weighted sine transform for half-line drift diffusion](diffusion-equation.md#weighted-sine-transform-for-half-line-drift-diffusion)
      - [Resolvent kernel for Dirichlet advection-diffusion on an interval](diffusion-equation.md#resolvent-kernel-for-dirichlet-advection-diffusion-on-an-interval)
    - [Gamma impulse solution for linearly increasing diffusivity](diffusion-equation.md#gamma-impulse-solution-for-linearly-increasing-diffusivity)
    - [Robin gauge transform for constant drift](diffusion-equation.md#robin-gauge-transform-for-constant-drift)
    - [Weighted Neumann heat kernel with constant drift](diffusion-equation.md#weighted-neumann-heat-kernel-with-constant-drift)
      - [Resolvent kernel for Neumann advection-diffusion on an interval](diffusion-equation.md#resolvent-kernel-for-neumann-advection-diffusion-on-an-interval)
      - [Neumann boundary-forcing formula](diffusion-equation.md#neumann-boundary-forcing-formula)
    - [Advection-diffusion heat-kernel solution](diffusion-equation.md#advection-diffusion-heat-kernel-solution)
      - [Half-line drift reflection kernel](diffusion-equation.md#half-line-drift-reflection-kernel)
  - [Nonlinear diffusion equation](diffusion-equation.md#nonlinear-diffusion-equation)
    - [Logarithmic diffusion](diffusion-equation.md#logarithmic-diffusion)
    - [Principal diffusion coefficients](diffusion-equation.md#principal-diffusion-coefficients)
    - [Perona-Malik equation](diffusion-equation.md#perona-malik-equation)
      - [Forward-backward threshold for gradient-weighted exponential diffusion](diffusion-equation.md#forward-backward-threshold-for-gradient-weighted-exponential-diffusion)
      - [Regularized Perona-Malik diffusion](diffusion-equation.md#regularized-perona-malik-diffusion)
    - [Two-dimensional Barenblatt solution with diffusivity proportional to concentration](diffusion-equation.md#two-dimensional-barenblatt-solution-with-diffusivity-proportional-to-concentration)
      - [Linear-reaction time change for quadratic nonlinear diffusion](diffusion-equation.md#linear-reaction-time-change-for-quadratic-nonlinear-diffusion)
  - [Reaction–diffusion system](diffusion-equation.md#reaction-diffusion-system)
    - [Bistable cubic reaction-diffusion equation](diffusion-equation.md#bistable-cubic-reaction-diffusion-equation)
      - [Logistic front of a bistable cubic equation](diffusion-equation.md#logistic-front-of-a-bistable-cubic-equation)
    - [Basally forced quadratic activator-inhibitor model](diffusion-equation.md#basally-forced-quadratic-activator-inhibitor-model)
      - [Weak focus at the Hopf threshold of a basal activator-inhibitor model](diffusion-equation.md#weak-focus-at-the-hopf-threshold-of-a-basal-activator-inhibitor-model)
      - [Turing threshold of a basally forced quadratic activator-inhibitor model](diffusion-equation.md#turing-threshold-of-a-basally-forced-quadratic-activator-inhibitor-model)
    - [Inhibitor in a reaction-diffusion system](diffusion-equation.md#inhibitor-in-a-reaction-diffusion-system)
    - [Activator in a reaction-diffusion system](diffusion-equation.md#activator-in-a-reaction-diffusion-system)
    - [Quadratic activator-inhibitor model](diffusion-equation.md#quadratic-activator-inhibitor-model)
      - [Turing threshold of the quadratic activator-inhibitor model](diffusion-equation.md#turing-threshold-of-the-quadratic-activator-inhibitor-model)
      - [Positive-quadrant Dulac multiplier for quadratic activation](diffusion-equation.md#positive-quadrant-dulac-multiplier-for-quadratic-activation)
    - [Spatially homogeneous equilibrium](diffusion-equation.md#spatially-homogeneous-equilibrium)
    - [Morphogen reaction-diffusion equation](diffusion-equation.md#morphogen-reaction-diffusion-equation)
      - [Mixed Dirichlet-Neumann modes on an interval](diffusion-equation.md#mixed-dirichlet-neumann-modes-on-an-interval)
        - [Critical length for a linearly growing morphogen](diffusion-equation.md#critical-length-for-a-linearly-growing-morphogen)
    - [Fast-inhibitor elimination in a reaction-diffusion system](diffusion-equation.md#fast-inhibitor-elimination-in-a-reaction-diffusion-system)
      - [Dispersion relation after fast-inhibitor elimination](diffusion-equation.md#dispersion-relation-after-fast-inhibitor-elimination)
    - [Turing pattern](diffusion-equation.md#turing-pattern)
      - [Turing instability](diffusion-equation.md#turing-instability)
        - [Fast-inhibitor cubic activator growth rate](diffusion-equation.md#fast-inhibitor-cubic-activator-growth-rate)
        - [Two-species diffusion-driven instability criterion](diffusion-equation.md#two-species-diffusion-driven-instability-criterion)
          - [Impossibility of a two-species Turing instability at equal diffusivities](diffusion-equation.md#impossibility-of-a-two-species-turing-instability-at-equal-diffusivities)
          - [Near-unity diffusivity ratio for a Turing instability](diffusion-equation.md#near-unity-diffusivity-ratio-for-a-turing-instability)
    - [Brusselator](diffusion-equation.md#brusselator)
      - [Hopf coefficient of the Brusselator](diffusion-equation.md#hopf-coefficient-of-the-brusselator)
      - [Brusselator trapping region](diffusion-equation.md#brusselator-trapping-region)
      - [Brusselator periodic-orbit criterion](diffusion-equation.md#brusselator-periodic-orbit-criterion)
      - [Turing threshold of the Brusselator](diffusion-equation.md#turing-threshold-of-the-brusselator)
        - [Discrete-mode Turing threshold for the Brusselator](diffusion-equation.md#discrete-mode-turing-threshold-for-the-brusselator)
        - [Brusselator Turing-before-Hopf diffusivity condition](diffusion-equation.md#brusselator-turing-before-hopf-diffusivity-condition)
- [Similarity solution](#similarity-solution)
  - [Similarity reduction](#similarity-reduction)
  - [Similarity ansatz](#similarity-ansatz)
  - [Similarity profile](#similarity-profile)
- [Separation of variables](#separation-of-variables)
  - [Separation constant](#separation-constant)
  - [Dirichlet problem on an annulus for one Fourier mode](#dirichlet-problem-on-an-annulus-for-one-fourier-mode)
- [Polynomial ansatz](#polynomial-ansatz)
- [Harmonic function](#harmonic-function)
  - [Componentwise harmonic vector field](#componentwise-harmonic-vector-field)
  - [Harmonic odd reflection across a hyperplane](#harmonic-odd-reflection-across-a-hyperplane)
  - [Harmonic Hardy space of the upper half-space](#harmonic-hardy-space-of-the-upper-half-space)
    - [Poisson representation of harmonic h1 by finite measures](#poisson-representation-of-harmonic-h1-by-finite-measures)
  - [Gradient of a dipole potential](#gradient-of-a-dipole-potential)
  - [Kelvin transform](#kelvin-transform)
    - [Spherical inversion preserves angular derivatives](#spherical-inversion-preserves-angular-derivatives)
  - [Harmonic functions of Brownian motion](#harmonic-functions-of-brownian-motion)
  - [Pluriharmonic function](#pluriharmonic-function)
  - [Compact convergence of locally bounded harmonic functions](#compact-convergence-of-locally-bounded-harmonic-functions)
  - [Poisson integral on the unit disk](#poisson-integral-on-the-unit-disk)
    - [Poisson integral converges nontangentially at Lebesgue points](#poisson-integral-converges-nontangentially-at-lebesgue-points)
    - [Poisson kernel on the circle](#poisson-kernel-on-the-circle)
      - [Uniform Poisson summability of continuous circle functions](#uniform-poisson-summability-of-continuous-circle-functions)
      - [Conjugate Poisson kernel on the circle](#conjugate-poisson-kernel-on-the-circle)
        - [One-sided Fourier spectrum excludes jumps](#one-sided-fourier-spectrum-excludes-jumps)
  - [Angular average of a logarithmic potential](#angular-average-of-a-logarithmic-potential)
  - [Vanishing harmonic function by level-set integration](#vanishing-harmonic-function-by-level-set-integration)
  - [Weakly harmonic Sobolev function](#weakly-harmonic-sobolev-function)
  - [Discrete harmonic function](#discrete-harmonic-function)
    - [Bounded harmonic function theorem on a recurrent graph](#bounded-harmonic-function-theorem-on-a-recurrent-graph)
    - [Harmonic maximum principle on a finite graph](#harmonic-maximum-principle-on-a-finite-graph)
    - [Bounded harmonic function theorem on the integer lattice](#bounded-harmonic-function-theorem-on-the-integer-lattice)
  - [Removable singularity for a bounded harmonic function](#removable-singularity-for-a-bounded-harmonic-function)
  - [Harmonic replacement](#harmonic-replacement)
  - [Mean value property for harmonic functions](#mean-value-property-for-harmonic-functions)
    - [Harnack inequality for harmonic functions](#harnack-inequality-for-harmonic-functions)
      - [Harnack inequality on the unit disk](#harnack-inequality-on-the-unit-disk)
        - [Sharp gradient bound for positive harmonic functions](#sharp-gradient-bound-for-positive-harmonic-functions)
    - [Local converse to the mean value property](#local-converse-to-the-mean-value-property)
  - [Weyl lemma](#weyl-lemma)
  - [Interior derivative estimate for a harmonic function](#interior-derivative-estimate-for-a-harmonic-function)
  - [Polynomial-growth Liouville theorem for harmonic functions](#polynomial-growth-liouville-theorem-for-harmonic-functions)
    - [Liouville lemma for globally Hölder harmonic functions](#liouville-lemma-for-globally-holder-harmonic-functions)
  - [Harmonic function as the real part of a holomorphic function](#harmonic-function-as-the-real-part-of-a-holomorphic-function)
  - [Subharmonic function](#subharmonic-function)
    - [Modulus powers of holomorphic functions are subharmonic](#modulus-powers-of-holomorphic-functions-are-subharmonic)
    - [Laplacian identity for the squared modulus of a holomorphic function](#laplacian-identity-for-the-squared-modulus-of-a-holomorphic-function)
    - [Harmonic majorant](#harmonic-majorant)
      - [Least harmonic majorant by expanding disk lifts](#least-harmonic-majorant-by-expanding-disk-lifts)
    - [Harmonic lifting of a continuous subharmonic function](#harmonic-lifting-of-a-continuous-subharmonic-function)
    - [Locally integrable supremum theorem for subharmonic functions](#locally-integrable-supremum-theorem-for-subharmonic-functions)
    - [Superharmonic function](#superharmonic-function)
    - [Canonical representative of a subharmonic distribution](#canonical-representative-of-a-subharmonic-distribution)
    - [Maximum principle for subharmonic functions](#maximum-principle-for-subharmonic-functions)
      - [Strong maximum principle for subharmonic functions](#strong-maximum-principle-for-subharmonic-functions)
      - [Gradient maximum principle for harmonic functions](#gradient-maximum-principle-for-harmonic-functions)
  - [Harmonic Liouville theorem](#harmonic-liouville-theorem)
    - [Gaussian heat-kernel proof of the harmonic Liouville theorem](#gaussian-heat-kernel-proof-of-the-harmonic-liouville-theorem)
    - [One-sided bounded harmonic functions on the punctured plane are constant](#one-sided-bounded-harmonic-functions-on-the-punctured-plane-are-constant)
    - [Brownian coupling proof of the harmonic Liouville theorem](#brownian-coupling-proof-of-the-harmonic-liouville-theorem)
    - [Surjectivity of a nonconstant entire harmonic function](#surjectivity-of-a-nonconstant-entire-harmonic-function)
  - [Scale-periodic harmonic function from an elliptic function](#scale-periodic-harmonic-function-from-an-elliptic-function)
  - [Harmonic polynomial](#harmonic-polynomial)
    - [Harmonic decomposition of homogeneous polynomials](#harmonic-decomposition-of-homogeneous-polynomials)
  - [Harmonic conjugate](#harmonic-conjugate)
    - [Global harmonic conjugate criterion by vanishing periods](#global-harmonic-conjugate-criterion-by-vanishing-periods)
      - [Logarithmic cancellation on an exterior annulus](#logarithmic-cancellation-on-an-exterior-annulus)
    - [Composition of harmonic conjugate pairs](#composition-of-harmonic-conjugate-pairs)
    - [Harmonic angle and logarithmic radius](#harmonic-angle-and-logarithmic-radius)
    - [Local harmonic conjugate](#local-harmonic-conjugate)
    - [Log modulus has no global harmonic conjugate on the punctured plane](#log-modulus-has-no-global-harmonic-conjugate-on-the-punctured-plane)
  - [Harmonic functions are smooth](#harmonic-functions-are-smooth)
  - [Harmonic functions are real analytic](#harmonic-functions-are-real-analytic)
    - [Unique continuation for harmonic functions](#unique-continuation-for-harmonic-functions)
- [Smooth bump function](#smooth-bump-function)
  - [Disjoint-support zero-product construction](#disjoint-support-zero-product-construction)
- [Laplace operator](#laplace-operator)
  - [Neumann Laplacian](#neumann-laplacian)
  - [Dirichlet Laplacian](#dirichlet-laplacian)
    - [Dirichlet resonance in an equilateral triangle](#dirichlet-resonance-in-an-equilateral-triangle)
    - [Fractional Dirichlet domain scale](#fractional-dirichlet-domain-scale)
  - [Polar-coordinate Laplacian identity](#polar-coordinate-laplacian-identity)
  - [Rotational commutator for the Laplacian](#rotational-commutator-for-the-laplacian)
  - [Laplace equation](#laplace-equation)
    - [Harmonic Fourier expansions in planar concentric domains](#harmonic-fourier-expansions-in-planar-concentric-domains)
    - [Separated Laplace mode with a Robin edge](#separated-laplace-mode-with-a-robin-edge)
    - [Spherical harmonic matching with a derivative jump](#spherical-harmonic-matching-with-a-derivative-jump)
    - [Fourier solution of the strip Dirichlet problem](#fourier-solution-of-the-strip-dirichlet-problem)
    - [Harmonic matching across a circle with a derivative jump](#harmonic-matching-across-a-circle-with-a-derivative-jump)
    - [Zero-boundary harmonic function with pointwise vertical decay](#zero-boundary-harmonic-function-with-pointwise-vertical-decay)
    - [Exterior harmonic potential with no flux through a sphere](#exterior-harmonic-potential-with-no-flux-through-a-sphere)
    - [Green function of the Laplacian](#green-function-of-the-laplacian)
      - [Point-source potential with one compact spatial dimension](#point-source-potential-with-one-compact-spatial-dimension)
      - [Fundamental solution of the Laplace equation](#fundamental-solution-of-the-laplace-equation)
    - [Laplace equation in polar coordinates](#laplace-equation-in-polar-coordinates)
    - [Laplace equation in cylindrical coordinates](#laplace-equation-in-cylindrical-coordinates)
      - [Side boundary data do not determine a bounded harmonic function in a half-cylinder](#side-boundary-data-do-not-determine-a-bounded-harmonic-function-in-a-half-cylinder)
  - [Radial Laplacian](#radial-laplacian)
  - [Laplacian in spherical coordinates](#laplacian-in-spherical-coordinates)
    - [Axisymmetric harmonic function](#axisymmetric-harmonic-function)
  - [Laplacian eigenfunction](#laplacian-eigenfunction)
    - [Laplacian eigenvalue](#laplacian-eigenvalue)
    - [Dirichlet Laplacian eigenfunction](#dirichlet-laplacian-eigenfunction)
      - [Dirichlet eigenfunction supremum estimate](#dirichlet-eigenfunction-supremum-estimate)
      - [Dirichlet Laplacian eigenvalue](#dirichlet-laplacian-eigenvalue)
- [Wave equation](wave-equation.md)
  - [Regular time-harmonic spherical wave](wave-equation.md#regular-time-harmonic-spherical-wave)
  - [Retarded acoustic Green function](wave-equation.md#retarded-acoustic-green-function)
  - [All-time boundedness of a wave equation with a reaction term](wave-equation.md#all-time-boundedness-of-a-wave-equation-with-a-reaction-term)
  - [Vector field method for wave equations](wave-equation.md#vector-field-method-for-wave-equations)
    - [Commuted wave energy](wave-equation.md#commuted-wave-energy)
    - [Klainerman-Sobolev inequality](wave-equation.md#klainerman-sobolev-inequality)
    - [Commutation vector field for the wave equation](wave-equation.md#commutation-vector-field-for-the-wave-equation)
      - [Scaling vector field](wave-equation.md#scaling-vector-field)
      - [Lorentz boost vector field](wave-equation.md#lorentz-boost-vector-field)
      - [Spatial rotation vector field](wave-equation.md#spatial-rotation-vector-field)
      - [Spacetime translation vector field](wave-equation.md#spacetime-translation-vector-field)
  - [Wave energy](wave-equation.md#wave-energy)
  - [Reflected-step solution of the wave equation](wave-equation.md#reflected-step-solution-of-the-wave-equation)
  - [Wave speed](wave-equation.md#wave-speed)
    - [Slowness](wave-equation.md#slowness)
  - [Kirchhoff formula](wave-equation.md#kirchhoff-formula)
    - [Method of descent for the wave equation](wave-equation.md#method-of-descent-for-the-wave-equation)
    - [Strong Huygens principle](wave-equation.md#strong-huygens-principle)
  - [Finite propagation speed](wave-equation.md#finite-propagation-speed)
    - [Weak Huygens principle](wave-equation.md#weak-huygens-principle)
    - [Shrinking cone energy argument](wave-equation.md#shrinking-cone-energy-argument)
    - [Characteristic diamond for speed one minus y squared](wave-equation.md#characteristic-diamond-for-speed-one-minus-y-squared)
  - [Radiation field](wave-equation.md#radiation-field)
    - [Scattering map](wave-equation.md#scattering-map)
  - [One-dimensional wave equation](wave-equation.md#one-dimensional-wave-equation)
  - [d'Alembert operator](wave-equation.md#d-alembert-operator)
  - [Semilinear wave equation](wave-equation.md#semilinear-wave-equation)
    - [Wave map](wave-equation.md#wave-map)
      - [Small data global regularity for wave maps](wave-equation.md#small-data-global-regularity-for-wave-maps)
      - [Global regularity for one-dimensional wave maps](wave-equation.md#global-regularity-for-one-dimensional-wave-maps)
      - [Stationary wave map](wave-equation.md#stationary-wave-map)
      - [Wave map energy](wave-equation.md#wave-map-energy)
        - [Wave map energy and criticality](wave-equation.md#wave-map-energy-and-criticality)
      - [Wave map Cauchy data](wave-equation.md#wave-map-cauchy-data)
    - [Null form for wave equations](wave-equation.md#null-form-for-wave-equations)
      - [Classical null condition for wave equations](wave-equation.md#classical-null-condition-for-wave-equations)
    - [Focusing semilinear wave equation](wave-equation.md#focusing-semilinear-wave-equation)
      - [Localized ordinary differential equation blowup for a wave equation](wave-equation.md#localized-ordinary-differential-equation-blowup-for-a-wave-equation)
    - [Smooth continuation criterion for semilinear wave equations](wave-equation.md#smooth-continuation-criterion-for-semilinear-wave-equations)
    - [Almost global existence for wave equations](wave-equation.md#almost-global-existence-for-wave-equations)
    - [Defocusing semilinear wave equation](wave-equation.md#defocusing-semilinear-wave-equation)
      - [H2 bound for the defocusing cubic wave equation](wave-equation.md#h2-bound-for-the-defocusing-cubic-wave-equation)
      - [Morawetz identity for the defocusing wave equation](wave-equation.md#morawetz-identity-for-the-defocusing-wave-equation)
        - [Distributional bilaplacian of the radial coordinate in three dimensions](wave-equation.md#distributional-bilaplacian-of-the-radial-coordinate-in-three-dimensions)
        - [Morawetz estimate for the defocusing wave equation](wave-equation.md#morawetz-estimate-for-the-defocusing-wave-equation)
      - [Radial reduction of the three-dimensional wave equation](wave-equation.md#radial-reduction-of-the-three-dimensional-wave-equation)
        - [Outgoing shell source estimate for a radial wave](wave-equation.md#outgoing-shell-source-estimate-for-a-radial-wave)
        - [Outgoing-energy identity for a radial defocusing wave](wave-equation.md#outgoing-energy-identity-for-a-radial-defocusing-wave)
    - [Local weak solution by contraction for a semilinear wave equation](wave-equation.md#local-weak-solution-by-contraction-for-a-semilinear-wave-equation)
  - [Elastic wave](wave-equation.md#elastic-wave)
    - [Characteristic crossing in a boundary-generated elastic simple wave](wave-equation.md#characteristic-crossing-in-a-boundary-generated-elastic-simple-wave)
    - [Elastic slowness surface](wave-equation.md#elastic-slowness-surface)
      - [Vertical slowness sextic of an anisotropic solid](wave-equation.md#vertical-slowness-sextic-of-an-anisotropic-solid)
      - [Elastic wave surface](wave-equation.md#elastic-wave-surface)
        - [Slowness curvature and wave-surface cusps](wave-equation.md#slowness-curvature-and-wave-surface-cusps)
      - [Elastic energy velocity](wave-equation.md#elastic-energy-velocity)
        - [Elastic mode classification by vertical energy flux](wave-equation.md#elastic-mode-classification-by-vertical-energy-flux)
          - [Free-surface anisotropic reflection amplitudes](wave-equation.md#free-surface-anisotropic-reflection-amplitudes)
    - [Elastodynamic Green tensor](wave-equation.md#elastodynamic-green-tensor)
      - [Far-field P and S radiation from a point force](wave-equation.md#far-field-p-and-s-radiation-from-a-point-force)
      - [Elastodynamic surface-jump representation](wave-equation.md#elastodynamic-surface-jump-representation)
      - [Point-moment elastodynamic displacement](wave-equation.md#point-moment-elastodynamic-displacement)
    - [Seismic moment tensor](wave-equation.md#seismic-moment-tensor)
      - [Explosion radiation in an isotropic elastic solid](wave-equation.md#explosion-radiation-in-an-isotropic-elastic-solid)
      - [Double-couple fault source](wave-equation.md#double-couple-fault-source)
        - [Double-couple radiation pattern](wave-equation.md#double-couple-radiation-pattern)
      - [Tensile-crack seismic source](wave-equation.md#tensile-crack-seismic-source)
        - [Tensile-crack radiation pattern](wave-equation.md#tensile-crack-radiation-pattern)
    - [Energy uniqueness for traction-driven elasticity](wave-equation.md#energy-uniqueness-for-traction-driven-elasticity)
      - [Elastic energy uniqueness with restoring boundary springs](wave-equation.md#elastic-energy-uniqueness-with-restoring-boundary-springs)
    - [Seismic impedance](wave-equation.md#seismic-impedance)
      - [Seismic layer transfer matrix](wave-equation.md#seismic-layer-transfer-matrix)
        - [Periodic seismic multilayer stop band](wave-equation.md#periodic-seismic-multilayer-stop-band)
      - [Flux-normalized elastic characteristic amplitudes](wave-equation.md#flux-normalized-elastic-characteristic-amplitudes)
        - [Zero-frequency scattering through an elastic layer](wave-equation.md#zero-frequency-scattering-through-an-elastic-layer)
    - [Love wave](wave-equation.md#love-wave)
      - [Anisotropic Love-wave dispersion](wave-equation.md#anisotropic-love-wave-dispersion)
      - [Rigid-base approximation to Love waves](wave-equation.md#rigid-base-approximation-to-love-waves)
        - [Group-velocity minimum of a high-contrast Love wave](wave-equation.md#group-velocity-minimum-of-a-high-contrast-love-wave)
      - [Love-wave cutoff frequencies](wave-equation.md#love-wave-cutoff-frequencies)
      - [Love-wave interface reflection phase](wave-equation.md#love-wave-interface-reflection-phase)
      - [Strict cutoff of the second Love-wave mode](wave-equation.md#strict-cutoff-of-the-second-love-wave-mode)
    - [Rayleigh wave](wave-equation.md#rayleigh-wave)
    - [Rigid elastic waveguide mode](wave-equation.md#rigid-elastic-waveguide-mode)
      - [Ray asymptotics of a clamped elastic waveguide mode](wave-equation.md#ray-asymptotics-of-a-clamped-elastic-waveguide-mode)
    - [Helmholtz separation of elastic waves](wave-equation.md#helmholtz-separation-of-elastic-waves)
      - [P-SV displacement potentials](wave-equation.md#p-sv-displacement-potentials)
    - [P wave](wave-equation.md#p-wave)
      - [P-wavefront discontinuity transport](wave-equation.md#p-wavefront-discontinuity-transport)
        - [Transmitted jump at a collimating solid-fluid interface](wave-equation.md#transmitted-jump-at-a-collimating-solid-fluid-interface)
        - [Ray-tube conservation for a P-wave jump](wave-equation.md#ray-tube-conservation-for-a-p-wave-jump)
      - [Reflection of a P-wave from a rigid plane](wave-equation.md#reflection-of-a-p-wave-from-a-rigid-plane)
      - [Longitudinal polarization](wave-equation.md#longitudinal-polarization)
    - [S wave](wave-equation.md#s-wave)
      - [Transverse polarization](wave-equation.md#transverse-polarization)
      - [SV-wave](wave-equation.md#sv-wave)
      - [SH-wave](wave-equation.md#sh-wave)
        - [SH ray-tube amplitude transport](wave-equation.md#sh-ray-tube-amplitude-transport)
          - [Refraction of a cylindrical SH wavefront](wave-equation.md#refraction-of-a-cylindrical-sh-wavefront)
        - [SH line-source near-field singularity](wave-equation.md#sh-line-source-near-field-singularity)
        - [Guided SH modes between rigid and free planes](wave-equation.md#guided-sh-modes-between-rigid-and-free-planes)
    - [Elastic-interface boundary conditions](wave-equation.md#elastic-interface-boundary-conditions)
      - [P-SV mode conversion at a solid interface](wave-equation.md#p-sv-mode-conversion-at-a-solid-interface)
      - [Snell law for elastic waves](wave-equation.md#snell-law-for-elastic-waves)
    - [Acoustic reflection and transmission at an interface](wave-equation.md#acoustic-reflection-and-transmission-at-an-interface)
      - [Lossless acoustic membrane scattering](wave-equation.md#lossless-acoustic-membrane-scattering)
      - [Equal displacement-amplitude condition at an acoustic interface](wave-equation.md#equal-displacement-amplitude-condition-at-an-acoustic-interface)
  - [Damping](wave-equation.md#damping)
    - [Critical damping](wave-equation.md#critical-damping)
  - [Wave equation on a string](wave-equation.md#wave-equation-on-a-string)
    - [Impulsively struck fixed-end string](wave-equation.md#impulsively-struck-fixed-end-string)
    - [Modal energy of a localized velocity impulse on a string](wave-equation.md#modal-energy-of-a-localized-velocity-impulse-on-a-string)
    - [Periodic reflection for a fixed-end string](wave-equation.md#periodic-reflection-for-a-fixed-end-string)
    - [Linearly damped string](wave-equation.md#linearly-damped-string)
      - [Velocity-impulse Green function for a damped string](wave-equation.md#velocity-impulse-green-function-for-a-damped-string)
      - [Separated solution of the damped string equation](wave-equation.md#separated-solution-of-the-damped-string-equation)
      - [Energy dissipation identity for a linearly damped string](wave-equation.md#energy-dissipation-identity-for-a-linearly-damped-string)
  - [Normal mode](wave-equation.md#normal-mode)
    - [Mode shape](wave-equation.md#mode-shape)
    - [Countability of elastic eigenfrequencies](wave-equation.md#countability-of-elastic-eigenfrequencies)
    - [Eigenfrequency](wave-equation.md#eigenfrequency)
    - [Modal energy distribution](wave-equation.md#modal-energy-distribution)
    - [Node (physics)](wave-equation.md#node-physics)
  - [Fourier transform method for the wave equation](wave-equation.md#fourier-transform-method-for-the-wave-equation)
    - [Low-frequency decomposition of the wave propagator](wave-equation.md#low-frequency-decomposition-of-the-wave-propagator)
    - [Entire wave cosine multiplier](wave-equation.md#entire-wave-cosine-multiplier)
  - [D'Alembert's formula](wave-equation.md#d-alembert-s-formula)
    - [Rectangular pulse splitting under the wave equation](wave-equation.md#rectangular-pulse-splitting-under-the-wave-equation)
    - [D'Alembert formula with initial velocity](wave-equation.md#d-alembert-formula-with-initial-velocity)
      - [Central zero region for odd compactly supported initial velocity](wave-equation.md#central-zero-region-for-odd-compactly-supported-initial-velocity)
  - [Wavenumber](wave-equation.md#wavenumber)
    - [Wavelength](wave-equation.md#wavelength)
  - [Dispersion relation](wave-equation.md#dispersion-relation)
    - [Spatial root of a dispersion relation](wave-equation.md#spatial-root-of-a-dispersion-relation)
    - [Spatiotemporal wave-packet stability](wave-equation.md#spatiotemporal-wave-packet-stability)
      - [Modulational instability](wave-equation.md#modulational-instability)
        - [Benjamin-Feir instability](wave-equation.md#benjamin-feir-instability)
        - [Focusing nonlinear Schrodinger modulation dispersion](wave-equation.md#focusing-nonlinear-schrodinger-modulation-dispersion)
      - [Briggs-Bers criterion](wave-equation.md#briggs-bers-criterion)
        - [Bounded temporal growth condition for cubic dispersion](wave-equation.md#bounded-temporal-growth-condition-for-cubic-dispersion)
        - [Quartic impulse-response Laplace resolvent](wave-equation.md#quartic-impulse-response-laplace-resolvent)
          - [Physical-sheet growth rate of a quartic impulse response](wave-equation.md#physical-sheet-growth-rate-of-a-quartic-impulse-response)
        - [Spatial pinch point](wave-equation.md#spatial-pinch-point)
          - [False complex saddle in dissipative cubic dispersion](wave-equation.md#false-complex-saddle-in-dissipative-cubic-dispersion)
          - [False spatial saddle in quartic dispersion](wave-equation.md#false-spatial-saddle-in-quartic-dispersion)
      - [Convective wave-packet instability](wave-equation.md#convective-wave-packet-instability)
      - [Absolute wave-packet instability](wave-equation.md#absolute-wave-packet-instability)
      - [Finite maximum temporal growth rate](wave-equation.md#finite-maximum-temporal-growth-rate)
    - [Wave dispersion](wave-equation.md#wave-dispersion)
      - [Nondispersive wave](wave-equation.md#nondispersive-wave)
    - [Dispersion diagram](wave-equation.md#dispersion-diagram)
    - [Ray tracing](wave-equation.md#ray-tracing)
      - [Travel time](wave-equation.md#travel-time)
      - [Elastic ray](wave-equation.md#elastic-ray)
        - [Spherical elastic ray invariant](wave-equation.md#spherical-elastic-ray-invariant)
          - [Herglotz–Wiechert inversion](wave-equation.md#herglotz-wiechert-inversion)
            - [Hidden turning-ray zone from nonmonotone spherical slowness](wave-equation.md#hidden-turning-ray-zone-from-nonmonotone-spherical-slowness)
          - [Core-reflected travel time](wave-equation.md#core-reflected-travel-time)
        - [Hyperbolic interface collimation of P-waves](wave-equation.md#hyperbolic-interface-collimation-of-p-waves)
      - [Hamiltonian ray equations for a local dispersion relation](wave-equation.md#hamiltonian-ray-equations-for-a-local-dispersion-relation)
        - [Simple turning point of a variable-speed wave](wave-equation.md#simple-turning-point-of-a-variable-speed-wave)
          - [Airy scaling at a variable-speed wave turning point](wave-equation.md#airy-scaling-at-a-variable-speed-wave-turning-point)
            - [Decaying Airy continuation and ray reflection](wave-equation.md#decaying-airy-continuation-and-ray-reflection)
            - [Turning-point enhancement of wave amplitude](wave-equation.md#turning-point-enhancement-of-wave-amplitude)
      - [Stationary square-root-dispersion wake](wave-equation.md#stationary-square-root-dispersion-wake)
    - [Growth rate](wave-equation.md#growth-rate)
    - [Phase velocity and group velocity](wave-equation.md#phase-velocity-and-group-velocity)
      - [Phase-group orthogonality for degree-zero dispersion](wave-equation.md#phase-group-orthogonality-for-degree-zero-dispersion)
      - [Phase velocity](wave-equation.md#phase-velocity)
        - [Horizontal phase velocity](wave-equation.md#horizontal-phase-velocity)
        - [Phase speed](wave-equation.md#phase-speed)
      - [Group velocity](wave-equation.md#group-velocity)
      - [Crest and trough](wave-equation.md#crest-and-trough)
        - [Wave crest](wave-equation.md#wave-crest)
        - [Wave trough](wave-equation.md#wave-trough)
      - [Wave packet](wave-equation.md#wave-packet)
        - [Envelope (waves)](wave-equation.md#envelope-waves)
      - [Ninth-order dispersive advection equation](wave-equation.md#ninth-order-dispersive-advection-equation)
  - [Klein-Gordon equation](wave-equation.md#klein-gordon-equation)
    - [Exponential initial-velocity tail for the Klein-Gordon equation](wave-equation.md#exponential-initial-velocity-tail-for-the-klein-gordon-equation)
    - [Stationary-phase asymptotic of a Klein-Gordon wave along a subluminal ray](wave-equation.md#stationary-phase-asymptotic-of-a-klein-gordon-wave-along-a-subluminal-ray)
      - [Upward zero crossings of an oscillatory stationary-phase tail](wave-equation.md#upward-zero-crossings-of-an-oscillatory-stationary-phase-tail)
- [Green second identity](#green-second-identity)
- [Lie point symmetry](#lie-point-symmetry)
  - [Infinitesimal generator of a Lie point symmetry](#infinitesimal-generator-of-a-lie-point-symmetry)
  - [Prolongation of a Lie point symmetry](#prolongation-of-a-lie-point-symmetry)
    - [Second prolongation of a Lie point symmetry](#second-prolongation-of-a-lie-point-symmetry)
  - [Scaling symmetry](#scaling-symmetry)
    - [Scaling symmetry of a partial differential equation](#scaling-symmetry-of-a-partial-differential-equation)
      - [Simultaneous spacetime scaling symmetry of the wave equation](#simultaneous-spacetime-scaling-symmetry-of-the-wave-equation)
  - [Symmetry reduction of a partial differential equation](#symmetry-reduction-of-a-partial-differential-equation)
    - [Group-invariant solution](#group-invariant-solution)
    - [Projective Lie symmetry of the potential Burgers equation](#projective-lie-symmetry-of-the-potential-burgers-equation)
    - [Similarity variable](#similarity-variable)

## Kuramoto-Sivashinsky equation

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)

The Kuramoto-Sivashinsky equation $u_t+uu_x+u_{xx}+u_{xxxx}=0$ combines destabilizing long-wave growth, stabilizing fourth-order [diffusion](thermodynamics.md#diffusion), and nonlinear transport. Its potential form is $\Phi_t=-\Phi_{xx}-\Phi_{xxxx}+(\Phi_x)^2$, with $u=-2\Phi_x$. It arises as a long-wave phase [amplitude equation](dynamical-systems.md#amplitude-equation) near loss of the [Benjamin-Feir stability condition](#benjamin-feir-stability-condition). On a domain of period $P$, the zero solution's [Fourier modes](fourier-analysis.md#fourier-mode) grow at rate $k^2-k^4$, $k=2\pi n/P$.

### Primary periodic bifurcation of the Kuramoto-Sivashinsky equation

↑ **Parent:** [Kuramoto-Sivashinsky equation](#kuramoto-sivashinsky-equation)

Fix zero mean and period $P$ in the [Kuramoto-Sivashinsky equation](#kuramoto-sivashinsky-equation). At $P=2\pi$ the first [Fourier mode](fourier-analysis.md#fourier-mode) becomes neutral and all higher modes are damped. For $k=2\pi/P$, expand $u=a\sin(kx)+b\sin(2kx)+\cdots$. The first equations are $\dot a=\lambda_1a+kab/2+\cdots$, $\dot b=\lambda_2b-ka^2/2+\cdots$, with $\lambda_j=(jk)^2-(jk)^4$. Slaving the second harmonic gives $\dot a=\lambda_1a+k^2a^3/(4\lambda_2)+\cdots$. Since $\lambda_2=-12$ at onset, this is a [supercritical bifurcation](dynamical-systems.md#supercritical-bifurcation). The small nonzero branch is stable in the sense of [orbital stability](dynamical-systems.md#orbital-stability) against disturbances of the same fixed period, modulo [translation](geometry-and-topology.md#translation-geometry); stability against disturbances of larger period does not follow from this local argument.

<h2 id="green-s-identities">Green's identities</h2>

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Green's_identities)

Green's identities relate volume integrals involving gradients and Laplacians to boundary values and normal derivatives. They follow from the divergence theorem and include [Green's first identity](#green-s-first-identity), [Green second identity](#green-second-identity) and [Green's third identity](#green-s-third-identity).

<h3 id="green-s-third-identity">Green's third identity</h3>

↑ **Parent:** [Green's identities](#green-s-identities)

Green's third identity represents a function inside a domain through its boundary values, normal derivatives, and a volume term involving its Laplacian.

<h3 id="green-s-first-identity">Green's first identity</h3>

↑ **Parent:** [Green's identities](#green-s-identities)

For smooth functions $u,v$ on a region $V$,

$$
\int_V\left(u\Delta v+\nabla u\cdot\nabla v\right)dV
=\int_{\partial V}u\frac{\partial v}{\partial n}\,dS.
$$

#### Gradient pairing with a boundary-constant function and a harmonic function

↑ **Parent:** [Green's first identity](#green-s-first-identity)

If $f$ is constant on the boundary and $g$ is a regular [harmonic function](#harmonic-function) throughout a volume, the [divergence theorem](calculus.md#divergence-theorem) applied to $f\nabla g$ gives $\int_V\nabla f\cdot\nabla g=\int_{\partial V}f\partial_ng$. The constant boundary value factors out; a second application of the divergence theorem makes the remaining flux $\int_V\Delta g=0$. This requires enough regularity to use [Green's first identity](#green-s-first-identity) over the entire volume.

##### Boundary flux from a singular harmonic potential

↑ **Parent:** [Gradient pairing with a boundary-constant function and a harmonic function](#gradient-pairing-with-a-boundary-constant-function-and-a-harmonic-function)

Although $1/r$ is harmonic away from the origin in three dimensions, it is not a regular [harmonic function](#harmonic-function) on a ball containing the origin. Its [gradient](calculus.md#gradient) is $-\widehat r/r^2$, so the displayed improper volume integral follows by canceling the $r^2$ in the spherical volume element. On the annulus $\varepsilon<r<a$, [Green's first identity](#green-s-first-identity) gives outer boundary contribution $-4\pi$ and inner contribution $4\pi\varepsilon/a$, recovering the same limit. Its global [Laplacian](calculus.md#laplacian) contains a [Dirac delta distribution](distribution-theory.md#dirac-delta-function), so the regular-harmonic gradient-pairing theorem is inapplicable.

## Maximum principle

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Maximum_principle)

A maximum principle bounds a solution through its boundary or initial data, often forbidding nonconstant solutions from attaining an interior extremum. Weak and strong versions depend on the differential operator and hypotheses. The [maximum principle for harmonic functions](#maximum-principle-for-harmonic-functions) and its strong counterpart are examples.

### Strong maximum principle for harmonic functions

↑ **Parent:** [Maximum principle](#maximum-principle)

If a harmonic function on a connected domain attains an interior maximum or minimum, it is constant. The mean value property forces equality throughout every sufficiently small ball around an interior extremum, and connectedness propagates the equality.

This is the strong harmonic instance of the [maximum principle](#maximum-principle).

### Maximum principle for harmonic functions

↑ **Parent:** [Maximum principle](#maximum-principle)

A continuous function harmonic on a bounded domain attains its maximum and minimum on the boundary. Apply the strictly subharmonic result to $u+\epsilon|x|^2$ and let $\epsilon\downarrow0$, then apply the same argument to $-u$.

## Burgers' equation

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Burgers'_equation)

The one-dimensional equation $u_t+uu_x=\nu u_{xx}$ combines nonlinear transport with diffusion. Positive $\nu$ gives the [viscous Burgers equation](#viscous-burgers-equation); setting $\nu=0$ gives the [Inviscid Burgers equation](#inviscid-burgers-equation).

### Viscous Burgers equation

↑ **Parent:** [Burgers' equation](#burgers-equation)

The viscous Burgers equation adds diffusion with viscosity $\nu>0$ to nonlinear transport. Smooth initial data remain smooth, and the diffusion regularizes the shocks of the [Inviscid Burgers equation](#inviscid-burgers-equation).

#### Modified Burgers equation with cubic flux

↑ **Parent:** [Viscous Burgers equation](#viscous-burgers-equation)

The cubic-flux variant replaces the quadratic conservative flux of [Burgers' equation](#burgers-equation) by $-q^3/3$. Its inviscid [characteristic speed](#characteristic-speed) is $-q^2$, while positive diffusivity regularizes [shock waves](#shock-wave). It is not linearized by the usual [Cole-Hopf transformation](#cole-hopf-transformation).

##### Traveling front of the cubic-flux Burgers equation

↑ **Parent:** [Modified Burgers equation with cubic flux](#modified-burgers-equation-with-cubic-flux)

For a front written in $s=Z+c\theta$ connecting $0$ at $s=-\infty$ to nonzero $\beta$ at $s=+\infty$, one integration gives $\epsilon c^2q'=q-cq^3/3$. The endpoint condition fixes $c=3/\beta^2$. Setting $w=q^2$ gives a logistic equation and the displayed profile, with the sign of $q$ selected by $\beta$. The propagation speed in the $\theta$ coordinate is $-\beta^2/3$, agreeing with the [Rankine-Hugoniot condition](#rankine-hugoniot-conditions) for flux $-q^3/3$.

#### Fay solution

↑ **Parent:** [Viscous Burgers equation](#viscous-burgers-equation)

The Fay solution is a periodic solution of the negative-flux [viscous Burgers equation](#viscous-burgers-equation) for $Z>0$. Its [Fourier series](fourier-series.md) has exponentially decreasing coefficients at each positive $\delta Z$. Expanding $1/\sinh(ns)=2\sum_{j\ge0}e^{-(2j+1)ns}$ and summing the sine series gives

$$
q=2\delta\sin\theta\sum_{j\ge0}\frac1{\cosh((2j+1)s)-\cos\theta},\qquad s=\delta Z.
$$

For $s\gg1$, the first harmonic gives $q\sim4\delta e^{-s}\sin\theta$. The [Fay shock-layer asymptotics](#fay-shock-layer-asymptotics) describe its opposite, small-$s$ regime.

##### Fay shock-layer asymptotics

↑ **Parent:** [Fay solution](#fay-solution)

For $|\theta|\ll1$ and $s=\delta Z\ll1$, the [Fay solution](#fay-solution) becomes $q\sim4\delta\theta\sum_{j\ge0}[((2j+1)s)^2+\theta^2]^{-1}$. The partial-fraction identity for the [hyperbolic tangent](calculus.md#hyperbolic-tangent) sums this to the displayed smooth shock layer. It resolves the odd transition from $-\pi/Z$ to $+\pi/Z$ on angular thickness $O(\delta Z)$; at $\theta=0$ both sides vanish and the comparison is read through their derivatives.

#### Burgers N-wave

↑ **Parent:** [Viscous Burgers equation](#viscous-burgers-equation)

A localized negative-flux Burgers N-wave has initial profile $-U\theta$ on $|\theta|<L$ and zero outside, for $U,L>0$. The [Cole-Hopf solution for a Burgers N-wave](#cole-hopf-solution-for-a-burgers-n-wave) expresses its viscous evolution in Gaussian interval masses. In the [vanishing-viscosity limit](viscous-fluid-flow.md#vanishing-viscosity-limit), the interior slope becomes $-U/(1+UZ)$ and its entropy-shock fronts move to $\pm L\sqrt{1+UZ}$.

##### Cole-Hopf solution for a Burgers N-wave

↑ **Parent:** [Burgers N-wave](#burgers-n-wave)

For the negative-flux [viscous Burgers equation](#viscous-burgers-equation), the [Cole-Hopf transformation](#cole-hopf-transformation) uses $f=2\alpha\partial_\theta\log\psi$. Initial N-wave data give $\psi_0=\exp[U(L^2-\theta^2)/(4\alpha)]$ inside $[-L,L]$ and one outside. Completing the square in the [heat kernel](diffusion-equation.md#heat-kernel) convolution gives, with $a=1+UZ$,

$$
\psi=1-I_\alpha(\theta,L,Z)+I_\alpha(\theta,La,Za)a^{-1/2}e^{U(L^2-\theta^2/a)/(4\alpha)}.
$$

The [Gaussian interval masses](diffusion-equation.md#gaussian-interval-mass) and their exponentially weighted tails must be treated together when taking the small-diffusion limit.

#### Viscous Burgers step solution with negative flux

↑ **Parent:** [Viscous Burgers equation](#viscous-burgers-equation)

For positive diffusivity, the [Cole-Hopf transformation](#cole-hopf-transformation) with $f=2\alpha\partial_\theta\log\psi$ converts the negative-flux equation into the [heat equation](diffusion-equation.md#heat-equation). Step data give a ratio of two Gaussian-tail integrals $J$. At $\theta=-UZ/2$, $J=1$ and $f=U/2$. Its [vanishing-viscosity limit](viscous-fluid-flow.md#vanishing-viscosity-limit) selects the shock or [rarefaction wave](#rarefaction-wave) in the [Burgers Riemann problem with negative flux](#burgers-riemann-problem-with-negative-flux), depending on the sign of $U$.

##### Midpoint symmetry of a viscous Burgers step

↑ **Parent:** [Viscous Burgers step solution with negative flux](#viscous-burgers-step-solution-with-negative-flux)

The [viscous Burgers step solution with negative flux](#viscous-burgers-step-solution-with-negative-flux) is symmetric around $\theta=-Uz/2$ after subtracting $U/2$. Its Gaussian-tail ratio equals one precisely at this midpoint, giving $f=U/2$ for either sign of $U$. For $U>0$ this point becomes the entropy-shock center in the [vanishing viscosity approximation](#vanishing-viscosity-approximation); for $U<0$ it is the center of a [rarefaction wave](#rarefaction-wave). The same trajectory therefore does not by itself identify a [shock](#shock-wave).

#### Cole-Hopf transformation

↑ **Parent:** [Viscous Burgers equation](#viscous-burgers-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cole-Hopf_transformation)

The Cole-Hopf transformation $u=-2\nu\phi_x/\phi$ converts the [viscous Burgers equation](#viscous-burgers-equation) into the [heat equation](diffusion-equation.md#heat-equation) $\phi_t=\nu\phi_{xx}$. Initial data $u(x,0)=g(x)$ correspond to $\phi(x,0)=C\exp[-(2\nu)^{-1}\int^xg(s)\,ds]$.

##### Sinusoidal Cole-Hopf solution for negative-flux Burgers flow

↑ **Parent:** [Cole-Hopf transformation](#cole-hopf-transformation)

For $q_Z-qq_\theta=\delta q_{\theta\theta}$ and initial data $q=\sin\theta$, the [Cole-Hopf transformation](#cole-hopf-transformation) $q=2\delta\psi_\theta/\psi$ gives $\psi(\theta,0)=\exp[-\cos\theta/(2\delta)]$. The [Fourier series](fourier-series.md) of this exponential and the [heat equation](diffusion-equation.md#heat-equation) give the displayed exact positive diffusion solution. Its first harmonic gives $q\sim4\delta[I_1(a)/I_0(a)]e^{-\delta Z}\sin\theta$. The [large-argument asymptotic expansion of a modified Bessel function](analysis.md#large-argument-asymptotic-expansion-of-a-modified-bessel-function) makes the ratio tend to one as $\delta\to0$.

##### Finite-exponential Cole-Hopf solution

↑ **Parent:** [Cole-Hopf transformation](#cole-hopf-transformation)

For the negative-flux [viscous Burgers equation](#viscous-burgers-equation) $q_Z-qq_\theta=\epsilon q_{\theta\theta}$, set $q=2\epsilon\partial_\theta\log\psi$. A sum of exponentials in the initial heat data evolves into $\psi=\sum_je^{A_j}$, giving the displayed [softmax function](statistical-learning.md#softmax-function) average. Two terms produce a traveling tanh shock from the lower to the higher state, with speed minus their mean.

###### Extremal-state asymptotics of exponential Burgers solutions

↑ **Parent:** [Finite-exponential Cole-Hopf solution](#finite-exponential-cole-hopf-solution)

For ordered states $q_1<\cdots<q_N$, in the moving frame $\theta=sZ+\xi$ the first and last exponents in the [finite-exponential Cole-Hopf solution](#finite-exponential-cole-hopf-solution) have the same leading coefficient. Each interior state's coefficient is smaller by $(q_j-q_1)(q_N-q_j)/(4\epsilon)>0$. Thus the large-$Z$ moving-frame profile is the two-state shock between the extremes. At fixed $\theta$, the endpoint of largest absolute value dominates; equal opposite extremes leave a stationary shock.

## Semilinear partial differential equation

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)

A semilinear partial differential equation is linear in its highest-order derivatives, with their coefficients depending only on the independent variables; lower-order terms may depend nonlinearly on the solution and its lower derivatives. A [semilinear heat equation](#semilinear-heat-equation) such as $u_t=\Delta u+f(u)$ is an example. This differs from a quasilinear equation, whose highest-order derivative coefficients can depend on the solution or its lower derivatives.

### Semilinear heat equation

↑ **Parent:** [Semilinear partial differential equation](#semilinear-partial-differential-equation)

A [heat equation](diffusion-equation.md#heat-equation) with a nonlinear reaction term depending on the value of its solution.

## Obstacle problem

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Obstacle_problem)

An obstacle constraint requires a solution to lie above a given function. In an [optimal stopping](martingale.md#optimal-stopping) problem, the value dominates the payoff, satisfies a generator equation where continuation is optimal, and a generator inequality where stopping is optimal. The complementary conditions can be expressed as a maximum equal to zero.

## Parabolic comparison principle

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)

A first-contact argument compares a smooth solution with a subsolution or supersolution. At a first spatial minimum of their difference, the Hessian is nonnegative; a strictly favorable time derivative then contradicts contact. For $u_t=u^2u_{xx}+u^3$, a positive decreasing constant-in-space barrier proves that positive periodic initial data stay positive for the lifetime of the smooth solution.

### Invariant interval for a cubic reaction-diffusion equation

↑ **Parent:** [Parabolic comparison principle](#parabolic-comparison-principle)

For $u_t=\Delta u+\lambda u-u^3$ with zero [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition), choose $K\geq\max(\|u_0\|_\infty,\sqrt{\max(\lambda,0)})$. The constants $K$ and $-K$ are a supersolution and a subsolution. More explicitly, testing with $(u-K)_+$ gives $\frac12\frac d{dt}\|(u-K)_+\|_2^2\leq\lambda\|(u-K)_+\|_2^2$, since the reaction derivative is at most $\lambda$ and the reaction at $K$ is nonpositive. The [Gronwall inequality](probability-and-statistics.md#gronwall-inequality) and the corresponding argument for $-u$ prove that $[-K,K]$ is invariant. A local [variation-of-constants formula](functional-analysis.md#variation-of-constants-formula) in the supremum norm then has a lifespan depending only on $K$, which prevents finite-time loss of the [classical solution](#classical-solution).

## Domain of dependence

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)

The domain of dependence of a solution value consists of the initial and boundary locations whose data can influence it. For $u_t+a u_x=0$ on the whole line, $u(x,t)=u(x-at,0)$, so its initial-data domain of dependence is the foot of the characteristic. For a finite-difference scheme, repeated stencil dependencies determine a numerical domain of dependence. The [Courant–Friedrichs–Lewy condition](finite-difference.md#courant-friedrichs-lewy-condition) requires the numerical domain to cover the physical one for convergence; it is necessary under its usual hyperbolic hypotheses, but not in general sufficient for [stability](numerical-analysis.md#stability-of-a-numerical-method).

## Linear partial differential equation

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)

A linear partial differential equation is a [partial differential equation](partial-differential-equation.md) in which the unknown function and its [partial derivatives](calculus.md#partial-derivative) occur linearly, with coefficients independent of the unknown. Its homogeneous solutions obey the [superposition principle](vector-space.md#superposition-principle).

## Ill-posed problem

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)

An ill-posed problem fails existence, uniqueness or continuous dependence in the specified function spaces. Backward [heat equation](diffusion-equation.md#heat-equation) evolution is unstable because its [Fourier modes](fourier-analysis.md#fourier-mode) grow like $e^{t|\xi|^2}$, making arbitrarily small high-frequency errors grow without a uniform bound.

## Linear partial differential operator

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)

A linear partial differential operator sends a function to a linear combination of its partial derivatives. If its coefficients are constant, the [Fourier transform of a derivative](fourier-analysis.md#fourier-transform-of-a-derivative) turns it into multiplication by its polynomial symbol $P(\xi)$.

## Liouville equation

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)

The elliptic Liouville equation $\Delta u=e^{2u}$ describes conformal metrics of constant negative Gaussian curvature under a common sign convention.

## Radial function

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radial_function)

A radial function depends only on the distance from the origin: $f(x)=g(|x|)$. Differential operators then reduce to radial formulas such as $\Delta f=g''+(n-1)g'/r$.

## Periodic domain

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)

A periodic domain identifies opposite faces of a fundamental cell, producing a flat torus. Periodic integration by parts has no boundary term, and zero-mean functions have no zero Fourier mode.

## Energy estimate

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Energy_estimate)

An energy estimate tests a differential equation against the solution or one of its derivatives to control a norm by initial data and forcing. Coercive terms represent dissipation, while [Young inequality](nonlinear-analysis.md#young-s-inequality-for-products) and the [Gronwall inequality](probability-and-statistics.md#gronwall-inequality) control lower-order terms.

### Bootstrap argument

↑ **Parent:** [Energy estimate](#energy-estimate)

A bootstrap argument assumes an a priori bound on an initial time interval and derives a strict improvement using an [energy estimate](#energy-estimate) or another inequality. [Continuity](calculus.md#continuous-function) extends the improved bound to the entire interval under consideration. For example $A(t)\leq C\varepsilon+C\int_0^t(1+s)^{-1}A(s)^2\,ds$ closes $A\leq2C\varepsilon$ when $\varepsilon\log(1+t)$ is sufficiently small. The strict improvement is what prevents a first failure time.

### Wave energy estimate

↑ **Parent:** [Energy estimate](#energy-estimate)

If $\Box u=F$ with [d'Alembert operator](wave-equation.md#d-alembert-operator) $\Box=-\partial_t^2+\Delta$, then $\|\partial u(t)\|_2\leq\|\partial u(0)\|_2+\int_0^t\|F(s)\|_2\,ds$, where $\partial u=(u_t,\nabla u)$. Test the [wave equation](wave-equation.md) against $u_t$, use [integration by parts](calculus.md#integration-by-parts), and apply the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality). The same [energy estimate](#energy-estimate) applies to a finite system of [wave equations](wave-equation.md).

#### Local wave energy estimate

↑ **Parent:** [Wave energy estimate](#wave-energy-estimate)

For the unit-speed [wave equation](wave-equation.md), the integral of $(u_t^2+|\nabla u|^2)/2$ over $B_r(x_0)$ at time $T\geq0$ is at most its initial integral over $B_{r+T}(x_0)$. On a shrinking ball the outward energy flux minus the loss from its moving boundary is $-((u_t-\partial_nu)^2+|\nabla_{\mathrm{tan}}u|^2)/2$, hence nonpositive. This estimate establishes the [domain of dependence](#domain-of-dependence) and [finite propagation speed](wave-equation.md#finite-propagation-speed) without any assumptions at spatial infinity.

### Hole-filling argument

↑ **Parent:** [Energy estimate](#energy-estimate)

An estimate $E(R)\leq C(E(2R)-E(R))$ bounds the energy in a ball by the energy in the surrounding [annulus](topology.md#annulus-mathematics). Moving the smaller-ball energy to the left gives the strict contraction $E(R)\leq\theta E(2R)$ with $\theta=C/(1+C)<1$. Iteration turns this contraction into decay at small scales.

#### Dyadic energy decay

↑ **Parent:** [Hole-filling argument](#hole-filling-argument)

If $E(R/2)\leq\theta E(R)$ and $E$ is nondecreasing, then $E(2^{-k}R)\leq\theta^kE(R)$. Between dyadic radii, monotonicity gives $E(r)\leq2^\mu(r/R)^\mu E(R)$ for any $0<\mu\leq-\log_2\theta$. This transfers a discrete contraction into a uniform power bound.

### Signed power test for a Laplacian eigenfunction

↑ **Parent:** [Energy estimate](#energy-estimate)

For a smooth [Dirichlet Laplacian eigenfunction](#dirichlet-laplacian-eigenfunction), testing $-\Delta u=\lambda u$ with $|u|^{\gamma-2}u$ for $\gamma\geq2$ gives the displayed [energy estimate](#energy-estimate). The [Sobolev chain rule](distribution-theory.md#sobolev-chain-rule) for $v=|u|^{\gamma/2}$ then yields $\int|Dv|^2=\lambda\gamma^2/[4(\gamma-1)]\int|u|^\gamma$. The absolute value and the sign in the test function permit nodal changes. At $\gamma=2$, use the Lipschitz absolute-value chain rule and the fact that a [gradient of a Sobolev function vanishes on a level set](distribution-theory.md#gradient-of-a-sobolev-function-vanishes-on-a-level-set).

### Caccioppoli inequality

↑ **Parent:** [Energy estimate](#energy-estimate)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Caccioppoli_inequality)

A Caccioppoli inequality is a local energy estimate obtained by testing an elliptic equation with a cutoff times the solution. It controls the gradient on a smaller ball by the function and forcing on a larger ball.

#### Caccioppoli inequality with bounded lower-order terms

↑ **Parent:** [Caccioppoli inequality](#caccioppoli-inequality)

For $\operatorname{div}(A Du)+b\cdot Du+cu=f$ with bounded measurable coefficients and uniformly elliptic $A$, testing with $\eta^2u$ and using [Young inequality](nonlinear-analysis.md#young-s-inequality-for-products) gives $\int\eta^2|Du|^2\leq C\int(1+|D\eta|^2)u^2+C\int\eta^2f^2$. No sign condition on $c$ is needed for this interior estimate. A cutoff equal to one on $U$ and supported in $V$ yields the displayed bound; the constant depends only on dimension, ellipticity, coefficient bounds and the separation of $U$ from the boundary of $V$.

##### Strong local Sobolev compactness for a fixed elliptic equation

↑ **Parent:** [Caccioppoli inequality with bounded lower-order terms](#caccioppoli-inequality-with-bounded-lower-order-terms)

Solutions of one fixed bounded-coefficient uniformly elliptic equation $Lu=f$ that are bounded in global $L^2$ have a subsequence converging strongly in $H^1$ on every relatively compact subdomain. Local energy bounds and the [Rellich-Kondrachov compactness theorem](sobolev-space.md#rellich-kondrachov-theorem) first give local strong $L^2$ and weak $H^1$ convergence on a smooth exhaustion. Pass to the weak equation to identify the limit. Differences solve $L(u_k-u)=0$, so the interior [Caccioppoli inequality](#caccioppoli-inequality) upgrades the local strong $L^2$ convergence to strong gradient convergence. Global weak $L^2$ convergence preserves the original global bound.

#### Annular Caccioppoli inequality

↑ **Parent:** [Caccioppoli inequality](#caccioppoli-inequality)

For a [weak solution](#weak-solution) of a [uniformly elliptic](elliptic-boundary-value-problem.md#uniformly-elliptic-operator) homogeneous [divergence-form elliptic operator](elliptic-boundary-value-problem.md#divergence-form-elliptic-operator), testing with $\eta^2(u-c)$ and choosing the [gradient](calculus.md#gradient) of the [cutoff function](distribution-theory.md#cutoff-function) in $B_{2R}\setminus B_R$ gives $\int_{B_R}|\nabla u|^2\leq CR^{-2}\int_{B_{2R}\setminus B_R}|u-c|^2$. The arbitrary constant $c$ can be chosen as an annular average, which makes the estimate suitable for a [hole-filling argument](#hole-filling-argument).

#### Power Caccioppoli inequality

↑ **Parent:** [Caccioppoli inequality](#caccioppoli-inequality)

For a nonnegative bounded [weak subsolution](elliptic-boundary-value-problem.md#weak-subsolution-of-a-divergence-form-elliptic-equation) and $\beta>1$, test with $\eta^2(u+\varepsilon)^{\beta-1}$. Uniform ellipticity and [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) give $\int |Du|^2u^{\beta-2}\eta^2\leq4\Lambda_*^2/[\lambda^2(\beta-1)^2]\int u^\beta|D\eta|^2$, with $\Lambda_*$ an [operator norm](continuous-dual-space.md#operator-norm) bound for the coefficient [matrix](vector-space.md#matrix). The [Sobolev chain rule](distribution-theory.md#sobolev-chain-rule) and $\varepsilon\downarrow0$ justify fractional powers and zero values. An entrywise bound $\Lambda$ yields $\Lambda_*\leq n\Lambda$.

##### Uniform power gain for elliptic solutions

↑ **Parent:** [Power Caccioppoli inequality](#power-caccioppoli-inequality)

For a nonnegative $H^1$ [weak solution](#weak-solution) of a [homogeneous divergence-form elliptic equation](elliptic-boundary-value-problem.md#homogeneous-divergence-form-elliptic-equation) on $B_1\subset\mathbb R^\ell$, $\ell\ge2$, with symmetric measurable $\lambda I\le A\le\Lambda I$, set $R=\Lambda/\lambda$ and $\alpha=1+1/\ell$. There is $D_\ell\ge1$ independent of $q\ge2$ such that

$$
\|u\|_{L^{q\alpha}(B_{r_1})}\le\left(\frac{D_\ell R}{r_2-r_1}\right)^{2/q}\|u\|_{L^q(B_{r_2})},\qquad0<r_1<r_2\le1.
$$

Test the equation with a cutoff times $u^{q-1}$, first regularized or truncated, to get $\int\zeta^2|\nabla u^{q/2}|^2\le[q/(q-1)]^2R^2\int u^q|\nabla\zeta|^2$. Apply a fixed-domain [Sobolev embedding theorem](sobolev-space.md#sobolev-embedding-theorem) to $\zeta u^{q/2}$ and take the $2/q$ power. Keeping the constant inside that power is crucial for [Moser iteration](elliptic-boundary-value-problem.md#moser-iteration).

#### Logarithmic Caccioppoli inequality

↑ **Parent:** [Caccioppoli inequality](#caccioppoli-inequality)

For a positive weak supersolution $u$ of a uniformly elliptic divergence-form equation, testing with $\eta^2/u$ gives

$$
\int\eta^2|D\log u|^2\leq C\int|D\eta|^2.
$$

The constant depends only on the ellipticity bounds.

## Second-order partial differential equation

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)

A second-order partial differential equation contains derivatives of the unknown function of order at most two and at least one second derivative. Its [principal symbol](#principal-symbol-of-a-partial-differential-equation) determines its characteristic directions and elliptic, parabolic or hyperbolic type.

## Quasilinear partial differential equation

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quasilinear_partial_differential_equation)

A quasilinear partial differential equation is linear in its highest-order derivatives, while its coefficients may depend on the independent variables, the unknown function, and lower-order derivatives.

### Averaged linearization of a nonlinear divergence-form equation

↑ **Parent:** [Quasilinear partial differential equation](#quasilinear-partial-differential-equation)

For a $C^1$ flux $F$ and a [weak solution](#weak-solution) of $\operatorname{div}F(Du)=0$, [discrete integration by parts](calculus.md#discrete-integration-by-parts) and the [fundamental theorem of calculus along a line segment](calculus.md#fundamental-theorem-of-calculus-along-a-line-segment) show that $w_h=\delta_{\ell,-h}u$ solves $\operatorname{div}(A_hDw_h)=0$, with $p_-=Du(x-he_\ell)$ and $p_+=Du(x)$. Coercive quadratic-form bounds and [operator norm](continuous-dual-space.md#operator-norm) bounds for $DF$ on all segments between these [gradients](calculus.md#gradient) pass to $A_h$. This produces a [divergence-form elliptic operator](elliptic-boundary-value-problem.md#divergence-form-elliptic-operator) without initially assuming second [partial derivatives](calculus.md#partial-derivative) of $u$.

### p-Laplacian

↑ **Parent:** [Quasilinear partial differential equation](#quasilinear-partial-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/p-Laplacian)

The p-Laplacian is the nonlinear divergence-form operator

$$
\Delta_pu=\operatorname{div}(|Du|^{p-2}Du).
$$

It is the [Euler-Lagrange operator](analysis.md#euler-lagrange-equation) of the [p-energy](calculus-of-variations.md#p-energy). For $p>2$ it is [degenerately elliptic](elliptic-boundary-value-problem.md#degenerate-elliptic-operator) where $Du=0$.

### Principal symbol of a partial differential equation

↑ **Parent:** [Quasilinear partial differential equation](#quasilinear-partial-differential-equation)

For a scalar differential operator of order $k$, the principal symbol replaces each order-$k$ derivative $\partial^\alpha$ by $\xi^\alpha$ and discards lower-order terms. For a [quasilinear partial differential equation](#quasilinear-partial-differential-equation), the coefficients are evaluated at the prescribed lower-order data.

#### Characteristic hypersurface

↑ **Parent:** [Principal symbol of a partial differential equation](#principal-symbol-of-a-partial-differential-equation)

A [hypersurface](differential-geometry.md#hypersurface) $\Sigma=\{\phi=0\}$ is characteristic for a differential equation at $x\in\Sigma$ when its [principal symbol](#principal-symbol-of-a-partial-differential-equation) vanishes on the conormal $d\phi(x)$:

$$
p(x,d\phi(x))=0.
$$

It is non-characteristic where this quantity is nonzero.

##### Characteristic plane

↑ **Parent:** [Characteristic hypersurface](#characteristic-hypersurface)

A characteristic plane is a planar [characteristic hypersurface](#characteristic-hypersurface). For $u_{zz}-m^2u_{xx}=0$, the planes $x\pm mz=\text{constant}$ carry the two travelling-wave families.

##### Non-characteristic hypersurface

↑ **Parent:** [Characteristic hypersurface](#characteristic-hypersurface)

A non-characteristic hypersurface satisfies $p(x,d\phi(x))\ne0$. This lets the equation solve for the highest derivative normal to the hypersurface.

##### Characteristic coordinate

↑ **Parent:** [Characteristic hypersurface](#characteristic-hypersurface)

A characteristic coordinate is a function constant along one family of [characteristics](#characteristic-hypersurface). For a second-order equation in two variables, two independent characteristic coordinates reduce the principal part to a mixed derivative.

###### Expanding-flow transformation of a wave equation

↑ **Parent:** [Characteristic coordinate](#characteristic-coordinate)

The change of variables $X=\rho e^{-t}$, $S=e^{-t}>0$ turns

$$
u_{tt}-\partial_\rho((1-\rho^2)u_\rho)+\partial_\rho(\rho u_t)+\rho u_{\rho t}=0
$$

into $w_{SS}-w_{XX}=0$. Indeed, with $D=\partial_t+\rho\partial_\rho$, the original operator is $D^2+D-\partial_\rho^2$, while $D=-S\partial_S$ and $\partial_\rho=S\partial_X$. Its [characteristic curves](#characteristic-curve) are $\rho=-1+Ce^t$ and $\rho=1+Ce^t$, including the characteristic lines $\rho=\pm1$. General smooth solutions have the form $F(e^{-t}(\rho+1))+G(e^{-t}(\rho-1))$. Zero [Cauchy data](#cauchy-data) on $-1<\rho<1$ at $t=0$ force vanishing throughout that strip for $t\geq0$, but not for all negative time: $u=(e^{-t}(\rho+1)-2)_+^3$ is a global $C^2$ counterexample. Thus the characteristic barriers describe a forward domain of dependence, not a barrier in both time directions.

#### Hyperbolic partial differential equation

↑ **Parent:** [Principal symbol of a partial differential equation](#principal-symbol-of-a-partial-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hyperbolic_partial_differential_equation)

A scalar second-order equation

$$
Au_{tt}+2Bu_{tx}+Cu_{xx}+\text{lower-order terms}=0
$$

is hyperbolic where $B^2-AC>0$. Equivalently, its [principal symbol](#principal-symbol-of-a-partial-differential-equation) has two distinct real characteristic directions.

##### Hyperbolicity

↑ **Parent:** [Hyperbolic partial differential equation](#hyperbolic-partial-differential-equation)

For a one-dimensional first-order system $v_t+A(v,x,t)v_x=s$, hyperbolicity means that the coefficient [matrix](vector-space.md#matrix) has real [eigenvalues](linear-operator-theory.md#eigenvalue) and a complete set of [eigenvectors](linear-operator-theory.md#eigenvector). Distinct real eigenvalues give strict hyperbolicity and separate [characteristic curves](#characteristic-curve). Along a curve of speed $\lambda$, a left [eigenvector](linear-operator-theory.md#eigenvector) $\ell A=\lambda\ell$ gives the compatibility equation $\ell\,dv/dt=\ell s$.

##### Travel-time coordinate for a one-dimensional variable-speed wave equation

↑ **Parent:** [Hyperbolic partial differential equation](#hyperbolic-partial-differential-equation)

For a one-dimensional [wave equation](wave-equation.md) whose [principal symbol](#principal-symbol-of-a-partial-differential-equation) is $\xi_t^2-c(y)^2\xi_y^2$, a travel-time coordinate is

$$
s(y)=\int^y\frac{dr}{c(r)}.
$$

Its two families of [characteristic curves](#characteristic-curve) are $s(y)-t=\text{constant}$ and $s(y)+t=\text{constant}$ wherever the [wave speed](wave-equation.md#wave-speed) $c$ is positive.

###### Characteristic curves for speed one minus y squared

↑ **Parent:** [Travel-time coordinate for a one-dimensional variable-speed wave equation](#travel-time-coordinate-for-a-one-dimensional-variable-speed-wave-equation)

For $c(y)=1-y^2$ in the strip $|y|<1$, the travel-time coordinate is $s(y)=\operatorname{artanh}y$. The [characteristic curves](#characteristic-curve) are

$$
\operatorname{artanh}y\pm x=\text{constant},
$$

equivalently $y=\tanh(C\mp x)$. Outside the strip the same separated [ordinary differential equation](differential-equation.md#ordinary-differential-equation) gives [hyperbolic cotangent](calculus.md#hyperbolic-cotangent) branches, and the equilibrium curves $y=\pm1$ are also characteristic.

## Cauchy problem

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cauchy_problem)

A Cauchy problem prescribes a solution and enough of its derivatives on a hypersurface to determine local evolution away from that hypersurface.

### Noncharacteristic Cauchy data

↑ **Parent:** [Cauchy problem](#cauchy-problem)

For $au_{x_1}+bu_{x_2}=c$ with data along $(\xi(s),\eta(s))$, the initial curve is noncharacteristic when its tangent is linearly independent of the projected characteristic vector $(a,b)$ evaluated at the initial value of $u$. The determinant is $a\eta'-b\xi'$, up to sign. For $C^1$ coefficients and data this permits the [inverse function theorem](calculus.md#inverse-function-theorem) to invert the local characteristic parametrization and gives a unique local [classical solution](#classical-solution).

### Continuous dependence on initial data

↑ **Parent:** [Cauchy problem](#cauchy-problem)

Continuous dependence means that convergence of the initial data in a specified topology implies convergence of the corresponding solutions in the specified solution topology. It is a stability requirement, not merely existence or uniqueness. [Smooth-data instability of the Cauchy-Riemann Cauchy problem](analysis.md#smooth-data-instability-of-the-cauchy-riemann-cauchy-problem) gives a counterexample even when the initial data converge uniformly with every fixed number of derivatives.

### Cauchy data

↑ **Parent:** [Cauchy problem](#cauchy-problem)

For a scalar equation of order $k$, Cauchy data consist of the first $k$ normal jets $u,\partial_Nu,\ldots,\partial_N^{k-1}u$ on the initial hypersurface.

These prescribed values define the initial conditions of a [Cauchy problem](#cauchy-problem).

#### Boundary jet

↑ **Parent:** [Cauchy data](#cauchy-data)

The boundary jet through order $m-1$ is the collection of traces $\partial^\alpha u|_{\partial\Omega}$ with $|\alpha|\le m-1$. Vanishing of the whole jet is stronger than vanishing of one [derivative](calculus.md#derivative). On a smooth [hypersurface](differential-geometry.md#hypersurface), zero normal Cauchy [derivatives](calculus.md#derivative) through order $m-1$, together with their tangential [derivatives](calculus.md#derivative), give a zero full boundary jet.

### Cauchy-Kovalevskaya theorem

↑ **Parent:** [Cauchy problem](#cauchy-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cauchy–Kovalevskaya_theorem)

For an order-$k$ scalar [quasilinear partial differential equation](#quasilinear-partial-differential-equation) with real-analytic coefficients, real-analytic [Cauchy data](#cauchy-data) on a real-analytic [non-characteristic hypersurface](#non-characteristic-hypersurface) determine a unique real-analytic solution in a neighbourhood of each point of that hypersurface.

#### Holmgren uniqueness theorem

↑ **Parent:** [Cauchy-Kovalevskaya theorem](#cauchy-kovalevskaya-theorem)

For a linear differential operator with [real analytic](analysis.md#real-analytic-function) coefficients, a classical solution with zero [Cauchy data](#cauchy-data) on a [real analytic](analysis.md#real-analytic-function) [non-characteristic hypersurface](#non-characteristic-hypersurface) vanishes locally near that [hypersurface](differential-geometry.md#hypersurface). The solution itself need not be [real analytic](analysis.md#real-analytic-function). A proof solves the [real analytic](analysis.md#real-analytic-function) inhomogeneous [formal adjoint](hilbert-space.md#formal-adjoint) problem against [polynomial](polynomial.md) sources, annihilates all [polynomial](polynomial.md) moments using boundary jets, and uses [polynomial](polynomial.md) density to force the solution to vanish.

##### Parabolic-cap proof of Holmgren uniqueness

↑ **Parent:** [Holmgren uniqueness theorem](#holmgren-uniqueness-theorem)

Near a non-characteristic plane $x=0$, use the small cap $\omega_\varepsilon=\{x>0,\ x+y^2<\varepsilon\}$. Its curved face is non-characteristic by continuity of the [principal symbol](#principal-symbol-of-a-partial-differential-equation). A [polynomial](polynomial.md) coordinate change flattens that face. Uniform [real analytic](analysis.md#real-analytic-function) coefficient bounds and the [uniform Cauchy radius for polynomial forcing](#uniform-cauchy-radius-for-polynomial-forcing) solve $P^*v=g$ throughout a common cap, with zero [boundary jet](#boundary-jet) on the curved face. The [complete boundary-jet condition for formal adjoints](hilbert-space.md#complete-boundary-jet-condition-for-formal-adjoints) then gives $\int_{\omega_\varepsilon}ug=0$ for every [polynomial](polynomial.md) $g$. Uniform approximation of $\bar u$ gives $\int|u|^2=0$. Repeating on the other side of the plane proves two-sided local uniqueness.

#### Uniform Cauchy radius for polynomial forcing

↑ **Parent:** [Cauchy-Kovalevskaya theorem](#cauchy-kovalevskaya-theorem)

For a linear [real analytic](analysis.md#real-analytic-function) non-characteristic [Cauchy problem for a partial differential equation](#cauchy-problem) with zero data, the local [real analytic](analysis.md#real-analytic-function) radius may be chosen uniformly over [polynomial](polynomial.md) forcing terms. Fix an analyticity exponent $R^{-1}$. Each [polynomial](polynomial.md), including a [polynomial](polynomial.md) obtained by a [polynomial](polynomial.md) coordinate change, satisfies the corresponding factorial [derivative](calculus.md#derivative) bound with some finite prefactor, uniformly over a compact parameter range. Divide the forcing by that prefactor to put all such data in one fixed majorant class. The [Cauchy-Kovalevskaya theorem](#cauchy-kovalevskaya-theorem) supplies a common radius, and linearity rescales the solution back without shrinking it. This argument does not bound the amplitudes of the resulting solutions uniformly.

#### General-order Cauchy-Kovalevskaya theorem

↑ **Parent:** [Cauchy-Kovalevskaya theorem](#cauchy-kovalevskaya-theorem)

A [real analytic](analysis.md#real-analytic-function) system solved for the highest [normal derivatives](differential-geometry.md#normal-derivative), with [real analytic](analysis.md#real-analytic-function) [Cauchy data](#cauchy-data), has a unique local [real analytic](analysis.md#real-analytic-function) solution. For common order $m$, its normal form is $\partial_t^mU=F(t,x,\{\partial_t^j\partial_x^\alpha U:j<m,\ j+|\alpha|\le m\})$. An invertible coefficient/Jacobian matrix for the highest [normal derivatives](differential-geometry.md#normal-derivative) is the system's [non-characteristic hypersurface](#non-characteristic-hypersurface) condition. A [real analytic](analysis.md#real-analytic-function) coordinate change flattens the initial [hypersurface](differential-geometry.md#hypersurface), and adjoining [derivatives](calculus.md#derivative) through order $m-1$ reduces the problem to a first-order [real analytic](analysis.md#real-analytic-function) system. Uniqueness here is in the [real analytic](analysis.md#real-analytic-function) class; it does not assert [Hadamard well-posedness](inverse-problem.md#well-posed-problem) in smooth or Sobolev [norms](functional-analysis.md#norm).

<h4 id="analytic-goursat-problem-for-a-klein-gordon-equation">Analytic Goursat problem for a Klein--Gordon equation</h4>

↑ **Parent:** [Cauchy-Kovalevskaya theorem](#cauchy-kovalevskaya-theorem)

In null coordinates, the characteristic boundary problem

$$
u_{\xi\eta}=-\frac14u,\qquad
u(\xi,0)=a(\xi),\qquad
u(0,\eta)=b(\eta)
$$

is a Volterra integral equation. Compatible analytic boundary data determine a unique analytic solution.

##### Global continuation for the analytic Goursat problem

↑ **Parent:** [Analytic Goursat problem for a Klein--Gordon equation](#analytic-goursat-problem-for-a-klein-gordon-equation)

On a compact characteristic rectangle, the Volterra iterates for the analytic Goursat problem are bounded by $C^m/(m!)^2$. Their series and differentiated series converge throughout the rectangle, extending the local analytic solution globally across it.

## Solution of a partial differential equation

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)

A solution of a partial differential equation is a function satisfying the equation in a specified sense and obeying its initial or boundary data.

### Classical solution

↑ **Parent:** [Solution of a partial differential equation](#solution-of-a-partial-differential-equation)

A classical solution has enough ordinary derivatives for the differential equation and its data to hold pointwise.

#### Positive-time smoothing for a semilinear heat equation

↑ **Parent:** [Classical solution](#classical-solution)

For a [semilinear partial differential equation](#semilinear-partial-differential-equation) $u_t=\Delta u+F(u)$ with smooth $F$ and smooth fixed boundary data, local boundedness permits positive-time [elliptic regularity](distribution-theory.md#elliptic-regularity) and parabolic smoothing. If $u_t$ is continuous with values in a [Hölder space](sobolev-space.md#holder-space), elliptic estimates first give continuous $C^{2,\beta}$ spatial regularity for $u$. Time difference quotients then solve a linear parabolic equation with coefficient converging to $F'(u)$; smoothing away from the initial time gives $u_t\in C(C^2)$, hence $u\in C^1(C^2)$. It is essential to gain spatial regularity for the time derivative too; $u\in C(C^2)\cap C^1(C^0)$ alone does not imply $C^1(C^2)$.

#### Bounded parabolic differentiability class

↑ **Parent:** [Classical solution](#classical-solution)

The notation $C_b^{1,2}([0,\infty)\times\mathbb R)$ ordinarily denotes functions with continuous time derivative and two continuous space derivatives, with the function and indicated derivatives bounded globally. A different condition, often intended in finite-horizon [partial differential equations](partial-differential-equation.md), is membership in $C_b^{1,2}([0,T]\times\mathbb R)$ for each finite $T$, allowing bounds to grow with $T$. These conventions must be distinguished in a long-time growth problem: the second permits divergence with time; the first does not. There is no universal notation for the finite-horizon condition, so it should be stated explicitly.

### Weak solution

↑ **Parent:** [Solution of a partial differential equation](#solution-of-a-partial-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weak_solution)

A weak solution satisfies an integrated identity in which derivatives are transferred to test functions. It can therefore exist with fewer classical derivatives.

#### Viscosity solution

↑ **Parent:** [Weak solution](#weak-solution)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Viscosity_solution)

For a [partial differential equation](partial-differential-equation.md) $F(x,u,Du,D^2u)=0$ whose operator is nonincreasing in the Hessian variable, a continuous viscosity subsolution satisfies $F(x_0,u(x_0),D\phi(x_0),D^2\phi(x_0))\leq0$ whenever a smooth [test function](distribution-theory.md#test-function) $\phi$ touches it from above. A viscosity supersolution satisfies the reverse inequality for tests touching from below. A viscosity solution satisfies both conditions. For $F=-\operatorname{tr}D^2u$, these conditions are respectively $\Delta\phi\geq0$ and $\Delta\phi\leq0$. They make sense even when $u$ has no classical second derivatives.

##### Continuous viscosity harmonic functions are classical

↑ **Parent:** [Viscosity solution](#viscosity-solution)

Let a continuous function satisfy both viscosity inequalities for the [Laplace operator](#laplace-operator). On any relatively compact ball, take its [harmonic replacement](#harmonic-replacement) $h$ with matching boundary values. If $u-h$ has a positive maximum, the function $h+\varepsilon(R^2-|x-a|^2)$ still lies below $u$ somewhere for sufficiently small positive $\varepsilon$, while matching it on the boundary. At an interior maximum of their difference it is a valid upper test, but its Laplacian is $-2n\varepsilon<0$, a contradiction. The opposite perturbation excludes a negative minimum. Thus $u=h$ throughout the ball and is a smooth [harmonic function](#harmonic-function). A locally defined test is extended near its touching point using a smooth [cutoff function](distribution-theory.md#cutoff-function) when global tests are required.

#### Weak-strong uniqueness principle

↑ **Parent:** [Weak solution](#weak-solution)

A weak-strong uniqueness principle says that a [weak solution](#weak-solution) with the same data as a sufficiently regular [classical solution](#classical-solution) agrees with that solution throughout its interval of regular existence, within the specified weak class. The conclusion is class-dependent: all bounded weak solutions of a prescribed $C^1$ linear transport field satisfy it, while nonlinear conservation laws require an admissibility condition such as an [entropy solution](#entropy-solution) condition.

#### Weak energy solution of a variable-coefficient wave equation

↑ **Parent:** [Weak solution](#weak-solution)

For $u_{tt}+L(t)u=f$ with homogeneous [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition), smooth uniformly elliptic principal coefficients, and initial data $(\psi_0,\psi_1)\in H_0^1(U)\times L^2(U)$, a space-time $H^1$ [weak solution](#weak-solution) has zero lateral trace, trace $u(0)=\psi_0$, and satisfies

$$
\int_0^T\bigl[-(u_t,v_t)_{L^2}+B_t[u,v]\bigr]dt
=\int_0^T(f,v)_{L^2}dt+(\psi_1,v(0))_{L^2}
$$

for every space-time $H^1$ test function with zero lateral trace and $v(T)=0$. The velocity initial condition is encoded by the last term; an arbitrary space-time $H^1$ function need not have an $L^2$ trace of its time derivative. The equation itself gives $u_{tt}\in L^2(0,T;H^{-1}(U))$, so $u_t$ has a continuous $H^{-1}$ representative.

#### Weak formulation

↑ **Parent:** [Weak solution](#weak-solution)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weak_formulation)

A weak formulation multiplies a differential equation by a [test function](distribution-theory.md#test-function), integrates, and uses [integration by parts](calculus.md#integration-by-parts) to move derivatives away from the unknown function. Natural boundary conditions appear in the resulting boundary terms.

#### Galerkin method

↑ **Parent:** [Weak solution](#weak-solution)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Galerkin_method)

The Galerkin method seeks an approximate solution in a finite-dimensional subspace and requires the equation's residual to be orthogonal to that subspace. Uniform energy estimates and compactness can then produce a [weak solution](#weak-solution) as the subspaces become dense.

##### Fourier truncation

↑ **Parent:** [Galerkin method](#galerkin-method)

A [Fourier truncation](#fourier-truncation) retains a finite set of boundary-compatible [Fourier modes](fourier-analysis.md#fourier-mode) and projects the PDE onto their span by the Galerkin method. Nonlinear products can generate unretained harmonics, so their coefficients are discarded by projection rather than declared zero pointwise. Agreement with a perturbation expansion through cubic order requires retention of every quadratically forced mode that feeds back on the critical mode at cubic order.

// Destination: dynamical-systems.bigb

##### Aubin-Lions lemma

↑ **Parent:** [Galerkin method](#galerkin-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Aubin-Lions_lemma)

If $X_0$ embeds compactly into $X$ and $X$ embeds continuously into $X_1$, then boundedness in $L^p(0,T;X_0)$ together with a suitable time-derivative bound in $L^q(0,T;X_1)$ makes a family relatively compact in $L^p(0,T;X)$. A standard case is

$$
L^2(0,T;H^1)\cap H^1(0,T;H^{-1})Subset L^2(0,T;L^2).
$$

###### Weak continuity from evolution-space bounds

↑ **Parent:** [Aubin-Lions lemma](#aubin-lions-lemma)

If $u\in L^\infty(0,T;H)$ and $u_t\in L^q(0,T;V')$ for a dense continuous embedding $V\hookrightarrow H$ and some $q>1$, then $u$ has a representative in $C([0,T];H_{\rm weak})$. Indeed, its pairing with each element of a dense subset of $V$ is absolutely continuous, and the uniform $H$ bound extends continuity to every element of $H$.

###### Strong continuity from weak continuity and an energy equality

↑ **Parent:** [Weak continuity from evolution-space bounds](#weak-continuity-from-evolution-space-bounds)

If $u:[0,T]\to H$ is weakly continuous and an energy equality makes $t\mapsto\|u(t)\|_H$ continuous, then $u$ is strongly continuous. This follows from the [Radon-Riesz theorem](hilbert-space.md#radon-riesz-theorem) applied whenever $t_n\to t$.

## Transport equation

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transport_equation)

A transport equation carries a quantity along the flow of a velocity field $b$. For a smooth solution of $u_t+b\mathbin\cdot\nabla u=0$, the value of $u$ is constant along each characteristic curve.

### Compact third-order advection stencil

↑ **Parent:** [Transport equation](#transport-equation)

Let $a=\mu(1+\mu)/2$, $b=(1+\mu)(2-\mu)$, $c=(1-\mu)(2-\mu)/2$, $d=2-\mu$, and $e=1+\mu$. The implicit stencil $aU_{j-1}^{n+1}+bU_j^{n+1}+cU_{j+1}^{n+1}=dU_j^n+eU_{j+1}^n$ for $u_t=u_x$ has centered characteristic moments zero through degree three and fourth moment $K(\mu)$. Its Fourier numerator and denominator satisfy $|L(\theta)|^2-|N(\theta)|^2=K(\mu)(1-\cos\theta)^2$. The marching operator is a contraction exactly for nonnegative [Courant numbers](finite-difference.md#courant-number) in $[0,1]\cup[2,\infty)$; with signed Courant numbers, also include $(-\infty,-1]$. At the four roots of $K$ the method becomes an exact integer grid translation rather than merely third order.

### Hamiltonian transport equation

↑ **Parent:** [Transport equation](#transport-equation)

Transport along a [Hamiltonian flow](classical-mechanics.md#hamiltonian-flow). The solution is $f(\cdot,t)=f_I\circ\Phi_{-t}$ wherever the inverse characteristic exists. Equality of mixed derivatives makes the transport vector field divergence-free, so its flow preserves phase-space volume. Smoothness of the Hamiltonian alone gives local characteristics, not a complete flow on all of phase space.

#### Casimir invariant of a transport equation

↑ **Parent:** [Hamiltonian transport equation](#hamiltonian-transport-equation)

For an incompressible transport flow, every integrable function of the transported scalar has constant integral: the scalar is unchanged along characteristics and the flow's Jacobian determinant equals one. For a finite integral on infinite phase space, require integrability; $F(0)=0$ and compactly supported data are one common choice. For a whole-space conservation statement also require no escape or boundary flux at infinity.

### Commuting velocity derivative for kinetic transport

↑ **Parent:** [Transport equation](#transport-equation)

The differential operators $Z_j$ commute with $D=\partial_t+a(v)\cdot\nabla_x$. Indeed $[D,\partial_{v_j}]=-\sum_i(\partial_{v_j}a_i)\partial_{x_i}$, canceled by differentiating the explicit time factor in $Z_j$. Hence $Z_jf$ satisfies the same [transport equation](#transport-equation) as $f$, and obeys the same [L2 norm](real-analysis.md#l2-norm) conservation when boundary fluxes vanish. For the standard [Jacobian matrix](calculus.md#jacobian-matrix) $(Da)_{ij}=\partial_{v_j}a_i$, the vector of these derivatives is $\nabla_vf+t(Da)^T\nabla_xf$.

### Dispersion with a nonlinear velocity map

↑ **Parent:** [Transport equation](#transport-equation)

For $f(t,x,v)=f_0(x-ta(v),v)$, apply the [area formula](calculus.md#area-formula-geometric-measure-theory) to the velocity map and bound the initial data by their velocity [essential supremum](measure-theory.md#essential-supremum). This gives the displayed [mixed Lebesgue norm](measure-theory.md#mixed-lebesgue-norm) estimate whenever the [weighted inverse multiplicity](calculus.md#weighted-inverse-multiplicity) is essentially bounded. If $a$ is injective and $|\det Da|\geq\alpha>0$, the constant is at most $1/\alpha$. In dimension one a derivative bounded away from zero gives a global [diffeomorphism](geometry-and-topology.md#diffeomorphism); in higher dimensions determinant bounds alone do not.

### Free transport equation

↑ **Parent:** [Transport equation](#transport-equation)

Particles keep their velocity and move along straight trajectories. The [method of characteristics](#method-of-characteristics) gives $f(t,x,v)=f_0(x-tv,v)$. The shear preserves [Lebesgue measure](measure-theory.md#lebesgue-measure) and every [Lp norm](real-analysis.md#lp-norm). Compact initial [support](function.md#support) remains compact at each finite time, but need not remain in one compact set for all times.

#### Free transport dispersion

↑ **Parent:** [Free transport equation](#free-transport-equation)

For the [free transport equation](#free-transport-equation), substitute $y=x-tv$ into $\int|f_0(x-tv,v)|\,dv$. The resulting factor $|t|^{-d}$ and the bound by $\sup_v|f_0(y,v)|$ prove this [mixed Lebesgue norm](measure-theory.md#mixed-lebesgue-norm) estimate. The right side contains initial data. The same-time mixed norm is not a conserved replacement: prescribing a product $\psi(x)\chi(v)$ at a later time and dilating $\chi$ disproves such a claim.

#### Absolutely continuous representative along free characteristics

↑ **Parent:** [Free transport equation](#free-transport-equation)

A [distributional weak solution](#weak-solution) of $\partial_tf+v\cdot\nabla_xf=g$, with locally integrable $f,g$, becomes $\partial_tF=G$ after the shear $F(t,x,v)=f(t,x+tv,v)$. For almost every characteristic label, there is an [absolutely continuous function](sobolev-space.md#absolutely-continuous-function) representing $F$, and its increments are the [integrals](calculus.md#integral) of $G$ for every pair of times. Arbitrary modifications on time slices can destroy this every-time identity without changing the distributional solution.

#### Free-transport semigroup

↑ **Parent:** [Free transport equation](#free-transport-equation)

For $1\leq p<\infty$, these operators are isometries on the phase-space [Lp space](measure-theory.md#lp-space), with $U_tU_s=U_{t+s}$. They form a [strongly continuous semigroup](functional-analysis.md#c0-semigroup) for $t\geq0$ and extend to a group for all real times. Strong continuity follows by smooth compactly supported approximation and measure preservation. They preserve the [essential supremum](measure-theory.md#essential-supremum) as well, but strong continuity is not claimed on the whole $L^\infty$ space.

### Characteristic curve

↑ **Parent:** [Transport equation](#transport-equation)

For the transport field $b(t,x)$, a characteristic curve solves

$$
\dot X(t)=b(t,X(t)).
$$

The chain rule converts differentiation of $u(t,X(t))$ into the transport operator applied to $u$.

#### Characteristic flow map

↑ **Parent:** [Characteristic curve](#characteristic-curve)

The characteristic flow map $Z_{s,t}(x)$ is the point reached at time $t$ by the [characteristic curve](#characteristic-curve) that passes through $x$ at time $s$. Whenever the flow is invertible, transport solutions pull their initial data back by $Z_{0,t}^{-1}$.

##### Phase-space flow Jacobian

↑ **Parent:** [Characteristic flow map](#characteristic-flow-map)

The [Jacobian determinant](calculus.md#jacobian-determinant) of a differentiable [characteristic flow map](#characteristic-flow-map) measures its change of volume. The variational equation and the [Liouville formula for a fundamental matrix](differential-equation.md#liouville-formula-for-a-fundamental-matrix) give the displayed formula for a complete smooth field $b$. For kinetic advection with $b=(v,F)$, its [divergence](calculus.md#divergence) is $\nabla_v\cdot F$. A zero [divergence](calculus.md#divergence) preserves phase-space [Lebesgue measure](measure-theory.md#lebesgue-measure).

##### Global characteristic flow under linear growth

↑ **Parent:** [Characteristic flow map](#characteristic-flow-map)

If $F\in C^1(\mathbb R\times\mathbb R^d)$ and $|F(t,x)|\le K(1+|x|)$, every [characteristic curve](#characteristic-curve) is defined for all real time. The [Gronwall inequality](probability-and-statistics.md#gronwall-inequality) bounds $1+|X(t)|$ on each bounded time interval, so local [ordinary differential equation](differential-equation.md#ordinary-differential-equation) existence cannot terminate through escape to infinity. Uniqueness and the variational equation give a global $C^1$ spatial flow diffeomorphism, with Jacobian $J>0$ satisfying $J_t=(\operatorname{div}F)(t,X)J$.

#### Method of characteristics

↑ **Parent:** [Characteristic curve](#characteristic-curve)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Method_of_characteristics)

The method of characteristics solves a first-order partial differential equation by reducing it to ordinary differential equations along [characteristic curves](#characteristic-curve).

##### Weighted Euler first-order equation

↑ **Parent:** [Method of characteristics](#method-of-characteristics)

For $x f_x+\beta y f_y=\gamma f$, the curves in the [method of characteristics](#method-of-characteristics) are $x=x_0e^s$, $y=y_0e^{\beta s}$ and $f=f_0e^{\gamma s}$. On either component $x\ne0$, the invariant is $y|x|^{-\beta}$, giving $f=|x|^\gamma F(y|x|^{-\beta})$. A coordinate change that includes $y/x$ may be singular on an axis, so smooth continuation there must be checked against the original [partial differential equation](partial-differential-equation.md).

##### Fold tangency obstruction for characteristic data

↑ **Parent:** [Method of characteristics](#method-of-characteristics)

If initial data are parameterized by $s$ and their characteristic invariant is $D(s)$, a solution constant on [characteristics](algebra.md#characteristic-of-a-field) requires $f(s)=F(D(s))$. At a fold $D'(s_0)=0$, equal invariant values must have equal data, and $f'(s)/D'(s)$ must extend continuously if $F$ is [continuously differentiable](calculus.md#continuously-differentiable-function). The condition $f'(s_0)=0$ alone is insufficient: for $D(s)=1/4-(s-1/2)^2$, the data $|s-1/2|^{3/2}$ would require a derivative of $F$ blowing up at $1/4$.

##### Characteristic equations for a transport equation

↑ **Parent:** [Method of characteristics](#method-of-characteristics)

For a [transport equation](#transport-equation) $\partial_tf+b(t,z)\cdot\nabla_zf=h$, solve $\dot z=b(t,z)$. The [chain rule](calculus.md#chain-rule) then gives $d[f(t,z(t))]/dt=h(t,z(t))$. Initial data and the time [integral](calculus.md#integral) of this source determine the solution along each [characteristic curve](#characteristic-curve).

### Linear transport equation

↑ **Parent:** [Transport equation](#transport-equation)

A linear transport equation has a prescribed velocity field and is linear in the transported unknown.

#### Transport of a Dirac point mass

↑ **Parent:** [Linear transport equation](#linear-transport-equation)

For the constant-velocity [linear transport equation](#linear-transport-equation) $u_t+c\cdot\nabla_xu=0$, a [Dirac delta distribution](distribution-theory.md#dirac-delta-function) initially at zero moves along $x=ct$. Its spacetime [distribution](distribution-theory.md#distribution-mathematical-analysis) pairs by $\langle u,\varphi\rangle=\int\varphi(ct,t)\,dt$, and its initial trace is obtained by [weak convergence of distributions](distribution-theory.md#weak-convergence-of-distributions). The [Fourier representation of the Dirac delta function](distribution-theory.md#fourier-representation-of-the-dirac-delta-function) writes it as an [oscillatory integral](distribution-theory.md#oscillatory-integral) with [phase function](distribution-theory.md#phase-function) $(x-ct)\cdot\theta$. Its [singular support](distribution-theory.md#singular-support) is precisely the trajectory; it has [order-zero distribution](distribution-theory.md#order-zero-distribution) regularity as a measure, without becoming a [smooth function](analysis.md#smooth-function).

#### Coercive energy estimate for kinetic transport

↑ **Parent:** [Linear transport equation](#linear-transport-equation)

If a velocity operator satisfies $\operatorname{Re}\langle Lh,h\rangle\geq\delta\|h\|_2^2$, then sufficiently regular solutions of $\partial_tf+v\cdot\nabla_xf+Lf=0$ obey the displayed estimate when spatial boundary fluxes vanish. The free-transport part contributes zero to the energy [derivative](calculus.md#derivative). Integrating the resulting differential inequality avoids dividing by a possibly zero [norm](functional-analysis.md#norm).

#### Lp conservation for incompressible transport

↑ **Parent:** [Linear transport equation](#linear-transport-equation)

Scalar advection preserves every finite [Lp norm](real-analysis.md#lp-norm) if its complete differentiable characteristic flow preserves volume and the initial datum belongs to the corresponding [Lp space](measure-theory.md#lp-space). In general the $p$th power of the [norm](functional-analysis.md#norm) is the initial $|f_0|^p$ weighted by the [phase-space flow Jacobian](#phase-space-flow-jacobian). Completeness alone preserves the [essential supremum](measure-theory.md#essential-supremum), but does not preserve finite-$p$ [norms](functional-analysis.md#norm) for compressible transport.

#### Inflow transport boundary condition

↑ **Parent:** [Linear transport equation](#linear-transport-equation)

For a [transport equation](#transport-equation) on a domain, prescribe boundary data only where the velocity points into the domain. On $x>0$ with speed $a>0$, a bounded [weak solution](#weak-solution) with initial data $u_0$ and inflow data $f$ satisfies

$$
\int u(\varphi_t+a\varphi_x)+\int u_0\varphi(0,x)+a\int f(t)\varphi(t,0)=0.
$$

The integrals are over the quadrant and its two boundary rays. Backtracking [characteristic curves](#characteristic-curve) gives $u_0(x-at)$ when $x\ge at$ and $f(t-x/a)$ otherwise. Corner values need not match for a bounded [weak solution](#weak-solution).

##### Corner compatibility for constant-speed transport

↑ **Parent:** [Inflow transport boundary condition](#inflow-transport-boundary-condition)

For the [transport equation](#transport-equation) $u_t+a u_x=0$ on the quadrant with $a>0$, smooth initial and inflow data glue across $x=at$ to order $m$ precisely when $f^{(j)}(0)=(-a)^j u_0^{(j)}(0)$ for $0\le j\le m$. Matching all orders yields a smooth solution; matching orders zero and one yields a [classical solution](#classical-solution) up to the two boundaries.

#### Weak transport solution under characteristic coordinates

↑ **Parent:** [Linear transport equation](#linear-transport-equation)

For a complete $C^1$ velocity flow, the bounded [weak solution](#weak-solution) of $u_t+F\cdot\nabla u=0$ is its initial value pulled back by the inverse flow. Its weak identity is $\int u(\varphi_t+\operatorname{div}(F\varphi))+\int u_0\varphi(0)=0$; the divergence term is essential. Changing to flow coordinates gives $\int w\partial_t(J\zeta)+\int u_0\zeta(0)=0$. Approximation in the spatial parameter permits $\zeta=\eta/J$, since $J$ and $J_t$ are continuous and $J>0$ on compact sets. Hence $\partial_tw=0$ distributionally, proving uniqueness without requiring second [derivatives](calculus.md#derivative) of $F$.

#### Adjoint transport equation

↑ **Parent:** [Linear transport equation](#linear-transport-equation)

An adjoint transport equation transfers the transport operator from a weak solution to a test function. Solving the terminal-value adjoint equation allows arbitrary compactly supported source terms to be used in uniqueness proofs.

### System of conservation laws

↑ **Parent:** [Transport equation](#transport-equation)

A system of conservation laws evolves a vector of conserved variables $U$ through a flux vector $F(U)$. For a smooth solution it has quasilinear form $U_t+A(U)U_x=0$, where $A(U)=DF(U)$ is the [flux Jacobian](#flux-jacobian).

#### Riemann problem

↑ **Parent:** [System of conservation laws](#system-of-conservation-laws)

A Riemann problem for a one-dimensional [system of conservation laws](#system-of-conservation-laws) $\partial_tU+\partial_xf(U)=0$ has two constant initial states, $U_L$ for $x<0$ and $U_R$ for $x>0$. The data and equation are invariant under $(x,t)\mapsto(\lambda x,\lambda t)$. When the physically admissible [entropy solution](#entropy-solution) is unique, this invariance makes it a [self-similar solution](#similarity-solution) depending on $x/t$. For ideal-gas [compressible flow](compressible-flow.md), the characteristic speeds are $u-c,u,u+c$. The two acoustic families carry [shock waves](#shock-wave) or [rarefaction waves](#rarefaction-wave), while the middle family carries a [contact discontinuity](#contact-discontinuity). Sufficiently strong separating velocities can instead create a vacuum region.

##### Single-rarefaction matching conditions for an ideal-gas Riemann problem

↑ **Parent:** [Riemann problem](#riemann-problem)

Two positive uniform ideal-gas states can be joined by one nontrivial [rarefaction wave](#rarefaction-wave) precisely when their [specific entropy](thermodynamics.md#specific-entropy) agrees, $p_L/\rho_L^\gamma=p_R/\rho_R^\gamma$, and for one $\sigma\in\{\pm1\}$ they satisfy $u_R-u_L=2\sigma(c_R-c_L)/(\gamma-1)$ with $\sigma(c_R-c_L)>0$. These equations are the constant-entropy and [Riemann invariant](compressible-flow.md#riemann-invariant) conditions of the [self-similar ideal-gas rarefaction](#self-similar-ideal-gas-rarefaction). They are sufficient because its affine $u,c$ profiles match the two states at $\xi_L=u_L+\sigma c_L$ and $\xi_R=u_R+\sigma c_R$, and $\xi_R>\xi_L$. The left family has $c_R<c_L$, while the right family has $c_R>c_L$. The inequality $u_R>u_L$ alone does not impose the two matching equalities.

##### Contact discontinuity

↑ **Parent:** [Riemann problem](#riemann-problem)

A contact discontinuity in one-dimensional gas dynamics moves with the common fluid [velocity](classical-mechanics.md#velocity) $s=u_L=u_R$ and has continuous [pressure](thermodynamics.md#pressure), while [mass density](fluid-mechanics.md#density) and [specific entropy](thermodynamics.md#specific-entropy) can jump. The mass jump condition $s[\rho]=[\rho u]$ is automatic with common $u=s$; momentum conservation $s[\rho u]=[\rho u^2+p]$ then requires $[p]=0$. The energy jump condition is also satisfied. Thus a contact is a material interface, not a compression shock. A smooth self-similar positive-density flow cannot spread this zero-speed-relative-to-the-fluid family into a fan: $u=x/t$ on an interval would require both $du/d(x/t)=1$ and, from continuity, $du/d(x/t)=0$.

#### Conservation law flux

↑ **Parent:** [System of conservation laws](#system-of-conservation-laws)

A [conservation law flux](#conservation-law-flux) $F(U)$ transports the conserved density $U$ across a surface. In one dimension $U_t+\partial_xF(U)=0$; a moving discontinuity satisfies $s[U]=[F]$. For a stationary [shock wave](#shock-wave), each conserved flux has the same value on both sides.

#### Quasilinear system

↑ **Parent:** [System of conservation laws](#system-of-conservation-laws)

A first-order quasilinear system has the form $U_t+A(U,x,t)U_x=S(U,x,t)$: derivatives of the unknown enter linearly, while their coefficient matrix may depend on the unknown itself.

##### Hyperbolic system

↑ **Parent:** [Quasilinear system](#quasilinear-system)

A quasilinear system is hyperbolic where its principal coefficient matrix has real eigenvalues and enough independent eigenvectors. The eigenvalues are its [characteristic speeds](#characteristic-speed).

#### Flux Jacobian

↑ **Parent:** [System of conservation laws](#system-of-conservation-laws)

The flux Jacobian is the [Jacobian matrix](calculus.md#jacobian-matrix) of the flux in a [system of conservation laws](#system-of-conservation-laws). Its [eigenvalues](linear-operator-theory.md#eigenvalue) are the local [characteristic speeds](#characteristic-speed), and its left and right [eigenvectors](linear-operator-theory.md#eigenvector) select the corresponding wave variables and directions in state space.

##### Characteristic speed

↑ **Parent:** [Flux Jacobian](#flux-jacobian)

A characteristic speed is an [eigenvalue](linear-operator-theory.md#eigenvalue) of the [flux Jacobian](#flux-jacobian). Along a corresponding [characteristic curve](#characteristic-curve), an associated wave variable obeys an [ordinary differential equation](differential-equation.md#ordinary-differential-equation) obtained by projecting the governing system onto the matching left [eigenvector](linear-operator-theory.md#eigenvector).

###### Kinematic wave

↑ **Parent:** [Characteristic speed](#characteristic-speed)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kinematic_wave)

A kinematic wave is a disturbance whose propagation speed is determined by the local relation between a conserved density and its flux. In a [scalar conservation law](#scalar-conservation-law) $u_t+f(u)_x=0$, smooth values travel at speed $f'(u)$.

### Scalar conservation law

↑ **Parent:** [Transport equation](#transport-equation)

A scalar conservation law in one space dimension has the form $u_t+\partial_xf(u)=0$. While a classical solution exists, it obeys the quasilinear transport equation $u_t+f'(u)u_x=0$.

#### Sonic point of a scalar flux

↑ **Parent:** [Scalar conservation law](#scalar-conservation-law)

For a differentiable [scalar conservation law](#scalar-conservation-law) $u_t+f(u)_x=0$, a [sonic point of a scalar flux](#sonic-point-of-a-scalar-flux) is a state $s$ where its [characteristic speed](#characteristic-speed) $f'(s)$ vanishes. If $f$ is convex and this zero is unique, $f'<0$ on the left and $f'>0$ on the right, so $s$ is the unique minimum of the flux. The definition refers to a vanishing transport speed in a [scalar conservation law](#scalar-conservation-law). In compressible [fluid mechanics](fluid-mechanics.md), a [sonic point](compressible-flow.md#sonic-point) instead refers to flow at the local sound speed.

#### Uniformly convex scalar flux

↑ **Parent:** [Scalar conservation law](#scalar-conservation-law)

In the common PDE convention, a uniformly convex scalar flux is a $C^2$ flux satisfying $F''(z)\geq\kappa>0$ throughout the specified state interval, with one constant $\kappa$. Equivalently, $F(z)-\kappa z^2/2$ is a [convex function](real-analysis.md#convex-function). This guarantees strict inequality below nontrivial chords and strict ordering of the two endpoint [derivatives](calculus.md#derivative) around the chord slope. On the whole real line it is incompatible with a globally bounded first [derivative](calculus.md#derivative).

#### Viscous scalar conservation law

↑ **Parent:** [Scalar conservation law](#scalar-conservation-law)

Positive $\varepsilon$ adds diffusion to a one-dimensional [scalar conservation law](#scalar-conservation-law). For a sufficiently decaying smooth solution, the divergence structure gives $\frac12\frac d{dt}\|u\|_2^2+\varepsilon\|u_x\|_2^2=0$, so the $L^2$ [energy estimate](#energy-estimate) is uniform in $\varepsilon$. If $|F'|\leq M$, testing against $-u_{xx}$ also yields $\|u_x(t)\|_2^2\leq e^{M^2t/\varepsilon}\|u_x(0)\|_2^2$. Thin [travelling waves](analysis.md#travelling-wave) explain why a uniform [gradient](calculus.md#gradient) bound generally fails.

##### Vanishing viscosity approximation

↑ **Parent:** [Viscous scalar conservation law](#viscous-scalar-conservation-law)

This approximation studies the limit of a [viscous scalar conservation law](#viscous-scalar-conservation-law) as its positive diffusion coefficient tends to zero. Under hypotheses giving compactness and appropriate convergence, the viscous entropy dissipation selects an [entropy solution](#entropy-solution) of the inviscid [scalar conservation law](#scalar-conservation-law). Fixed-phase decreasing [travelling waves](analysis.md#travelling-wave) for a strictly convex flux converge to an [entropy shock](#entropy-shock). Translating each profile differently can change or destroy the limit, so phase or initial data must specify the family.

#### Maximum representation for a concave conservation law

↑ **Parent:** [Scalar conservation law](#scalar-conservation-law)

Let $f$ be smooth and strictly concave, with $f(0)=0$ and $f'$ bijective, and let $u_0$ be smooth with compact support. For $0<t<t_*$ in the smooth [concave-flux characteristic lifespan](#concave-flux-characteristic-lifespan), the primitive $U_x=u$ solves the [Hamilton-Jacobi equation](classical-mechanics.md#hamilton-jacobi-equation) $U_t+f(U_x)=0$ and obeys

$$
U(t,x)=\max_y\left\{U(0,y)+t g\left(\frac{x-y}{t}\right)\right\},
$$

where $g$ is the [concave Legendre dual](convex-optimization.md#concave-legendre-dual). The tangent inequality for a [concave function](real-analysis.md#concave-function) bounds every candidate by $U(t,x)$, and the backward [characteristic curve](#characteristic-curve) attains equality. Its foot $x_0$ is the unique maximizer, and $u(t,x)=h((x-x_0)/t)$ for $h=(f')^{-1}$. This statement concerns the smooth solution, without asserting a post-crossing continuation.

##### Square-root decay before characteristic crossing

↑ **Parent:** [Maximum representation for a concave conservation law](#maximum-representation-for-a-concave-conservation-law)

Under the [inverse-flux quadratic bounds](convex-optimization.md#inverse-flux-quadratic-bounds), smooth compactly supported data in a [scalar conservation law](#scalar-conservation-law) satisfy

$$
\|u(t,\cdot)\|_\infty\le-2k_-\sqrt{\frac{2\|u_0\|_1}{-k_+}}\,t^{-1/2}\qquad(0<t<t_*).
$$

At the maximizing foot $x_0$, the [maximum representation for a concave conservation law](#maximum-representation-for-a-concave-conservation-law) bounds $U$ below by $-\|u_0\|_1$ and above by $\|u_0\|_1+k_+(x-x_0-ct)^2/t$. This bounds the deviation of the [characteristic speed](#characteristic-speed) from $c$; the linear inverse-flux bound then controls $u$. The time interval ends at the first [characteristic crossing](#characteristic-crossing).

#### Characteristic solution of a scalar conservation law

↑ **Parent:** [Scalar conservation law](#scalar-conservation-law)

Before [characteristic crossing](#characteristic-crossing), the [scalar conservation law](#scalar-conservation-law) $u_t+f(u)_x=0$ has solution $u(t,X_t(\xi))=u_0(\xi)$ with $X_t(\xi)=\xi+t f'(u_0(\xi))$. When this map is a [diffeomorphism](geometry-and-topology.md#diffeomorphism), the solution is $u_0\circ X_t^{-1}$. Its spatial derivative is $u_0'(\xi)/(1+t f''(u_0(\xi))u_0'(\xi))$.

#### Concave-flux characteristic lifespan

↑ **Parent:** [Scalar conservation law](#scalar-conservation-law)

For smooth compactly supported data in the [scalar conservation law](#scalar-conservation-law) $u_t+f(u)_x=0$, put $m=\min_\xi f''(u_0(\xi))u_0'(\xi)$. Its smooth [characteristic solution of a scalar conservation law](#characteristic-solution-of-a-scalar-conservation-law) exists until $t_*=-1/m$ if $m<0$, and for all times if $m\ge0$. The [characteristic flow map](#characteristic-flow-map) $X_t(\xi)=\xi+t f'(u_0(\xi))$ has derivative $1+t f''(u_0)u_0'$; its first zero produces gradient blowup. The formula applies to smooth fluxes of either concavity, although it is particularly useful for a [concave function](real-analysis.md#concave-function) flux.

#### Bounded-derivative Burgers flux

↑ **Parent:** [Scalar conservation law](#scalar-conservation-law)

This $C^1$ flux has $|f'|\le1$ globally and agrees with the [Inviscid Burgers equation](#inviscid-burgers-equation) flux on $[-1,1]$. It allows Burgers examples to satisfy a global bounded-speed hypothesis. For Riemann data $-1$ to the left and $1$ to the right, both the stationary expansion discontinuity and the fan $u=x/t$ on $|x|<t$, with exterior values $\pm1$, are bounded weak solutions. Only the fan is an [entropy solution](#entropy-solution).

#### Shock wave

↑ **Parent:** [Scalar conservation law](#scalar-conservation-law)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Shock_wave)

A shock wave is a moving discontinuity of a [weak solution](#weak-solution) to a conservation law. Its speed is fixed by the [Rankine-Hugoniot condition](#rankine-hugoniot-conditions), while an entropy condition selects the physically admissible direction of compression.

##### Rankine-Hugoniot conditions

↑ **Parent:** [Shock wave](#shock-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rankine–Hugoniot_conditions)

The [Rankine-Hugoniot condition](#rankine-hugoniot-conditions) expresses [conservation laws](physics.md#conservation-law) across a moving discontinuity of a [weak solution](#weak-solution). Across a discontinuity $x=\sigma t$ in $u_t+f(u)_x=0$, with left and right states $u_-$ and $u_+$, conservation requires

$$
\sigma(u_+-u_-)=f(u_+)-f(u_-).
$$

Writing $[u]=u_+-u_-$ and $[f(u)]=f(u_+)-f(u_-)$ gives $\sigma[u]=[f(u)]$. The same relation holds componentwise for a [system of conservation laws](#system-of-conservation-laws); in [compressible flow](compressible-flow.md), conservation of [mass](classical-mechanics.md#mass), [momentum](classical-mechanics.md#momentum) and [energy](classical-mechanics.md#energy) supplies the jump conditions for a [shock wave](#shock-wave). Integrating the [weak solution](#weak-solution) identity over a thin space-time region crossing the discontinuity yields this balance between the swept-up conserved quantity and the difference of fluxes.

##### Entropy shock

↑ **Parent:** [Shock wave](#shock-wave)

For a scalar equation with strictly convex flux and states $u_l>u_r$, the [Rankine-Hugoniot condition](#rankine-hugoniot-conditions) determines a discontinuity speed strictly between the right and left [characteristic speeds](#characteristic-speed). [Characteristic curves](#characteristic-curve) enter this compressive discontinuity from both sides. Its [entropy flux for a scalar conservation law](#entropy-flux-for-a-scalar-conservation-law) inequalities make it an [entropy solution](#entropy-solution). It is the limit of a phase-normalized decreasing [travelling wave](analysis.md#travelling-wave) in the [vanishing viscosity approximation](#vanishing-viscosity-approximation).

#### Rarefaction wave

↑ **Parent:** [Scalar conservation law](#scalar-conservation-law)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rarefaction_wave)

A rarefaction wave is a continuous expanding fan of characteristics that connects two constant states of a hyperbolic conservation law.

##### Self-similar ideal-gas rarefaction

↑ **Parent:** [Rarefaction wave](#rarefaction-wave)

For $\gamma>1$ and positive [mass density](fluid-mechanics.md#density) and [pressure](thermodynamics.md#pressure), let $\xi=x/t$ in one-dimensional adiabatic [compressible flow](compressible-flow.md). The smooth equations are $(u-\xi)\rho'+\rho u'=0$, $(u-\xi)u'+p'/\rho=0$ and $(u-\xi)p'+\gamma p u'=0$. Away from a constant branch, their coefficient determinant forces $\xi=u+\sigma c$ with $\sigma=\pm1$ and [adiabatic sound speed](compressible-flow.md#adiabatic-sound-speed) $c=\sqrt{\gamma p/\rho}$. The entropy equation gives $p=K\rho^\gamma$, and combining continuity with $c'/c=(\gamma-1)\rho'/(2\rho)$ gives

$$
u'=\frac2{\gamma+1},\qquad c'=\sigma\frac{\gamma-1}{\gamma+1},\qquad u-\frac{2\sigma c}{\gamma-1}=J.
$$

Thus $u=[2\xi+(\gamma-1)J]/(\gamma+1)$, $c=\sigma(\gamma-1)(\xi-J)/(\gamma+1)$, $\rho=(c^2/(\gamma K))^{1/(\gamma-1)}$ and $p=K\rho^\gamma$, on intervals where $c>0$. The [specific entropy](thermodynamics.md#specific-entropy) is constant. Together with uniform branches, these exhaust smooth positive-gas self-similar solutions; a [contact discontinuity](#contact-discontinuity) is not a smooth fan.

#### Inviscid Burgers equation

↑ **Parent:** [Scalar conservation law](#scalar-conservation-law)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inviscid_Burgers_equation)

The inviscid Burgers equation is the [scalar conservation law](#scalar-conservation-law)

$$
u_t+\left(\frac{u^2}{2}\right)_x=0.
$$

Its discontinuities obey the [Rankine-Hugoniot condition](#rankine-hugoniot-conditions) $\sigma=(u_-+u_+)/2$. Restricting to [entropy solutions](#entropy-solution) restores uniqueness for bounded initial data.

##### Periodic backward-sawtooth Burgers solution

↑ **Parent:** [Inviscid Burgers equation](#inviscid-burgers-equation)

For the negative-flux equation $f_Z-ff_\theta=0$, a period-two increasing initial ramp develops rarefaction fans at odd points and steepens at even points. Before $Z=1$, its central ramp is $f=(\theta-2m)/(1-Z)$ on $|\theta-2m|<1-Z$, and its odd-point fans are $f=-(\theta-(2m+1))/Z$. After $Z=1$, stationary compressive shocks occupy the even points and $f=(2m+1-\theta)/Z$ between consecutive shocks. The amplitude decays as $1/Z$. The [Rankine-Hugoniot condition](#rankine-hugoniot-conditions) and incoming [characteristic speeds](#characteristic-speed) certify the post-breaking [entropy solution](#entropy-solution).

##### Burgers Riemann problem with negative flux

↑ **Parent:** [Inviscid Burgers equation](#inviscid-burgers-equation)

For left state zero and right state $U$, negative-flux [Inviscid Burgers equation](#inviscid-burgers-equation) gives a shock at $\theta=-UZ/2$ when $U>0$, and a [rarefaction wave](#rarefaction-wave) $f=-\theta/Z$ on $0<\theta<-UZ$ when $U<0$. This is the standard positive-flux equation after setting $u=-f$; [entropy solution](#entropy-solution) selection reverses which step direction is compressive.

##### Entropy solution

↑ **Parent:** [Inviscid Burgers equation](#inviscid-burgers-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Entropy_solution)

An entropy solution is a [weak solution](#weak-solution) of a nonlinear [scalar conservation law](#scalar-conservation-law) that also satisfies entropy inequalities selecting physically admissible shocks. For convex fluxes, this excludes expansion shocks and restores uniqueness for bounded initial data.

###### Kruzhkov entropy inequality

↑ **Parent:** [Entropy solution](#entropy-solution)

For a scalar [conservation law](physics.md#conservation-law) law $u_t+f(u)_x=0$, the Kruzhkov entropy inequalities require

$$
\partial_t|u-c|+\partial_x\bigl(\operatorname{sgn}(u-c)[f(u)-f(c)]\bigr)\le0
$$

in distributions for every real constant $c$, together with the initial trace. This means the integral against every nonnegative compactly supported test function is nonpositive after applying the distributional derivatives. For a smooth solution the entropy balance is an equality away from $u=c$. For a viscous approximation $u_t+f(u)_x=\varepsilon u_{xx}$, smooth convex approximations $\eta$ of $|u-c|$ give $\partial_t\eta(u)+\partial_xq(u)=\varepsilon\partial_{xx}\eta(u)-\varepsilon\eta''(u)u_x^2\le\varepsilon\partial_{xx}\eta(u)$, with $q'=\eta'f'$. Letting the entropy smoothing vanish and then taking a bounded, strongly locally convergent zero-viscosity limit proves the inequality. The discrete entropy inequality of a monotone conservative scheme is its numerical analogue.

###### Discrete entropy inequality

↑ **Parent:** [Entropy solution](#entropy-solution)

For a scalar conservative monotone update with flux $F$, define $Q(a,b;c)=F(a\vee c,b\vee c)-F(a\wedge c,b\wedge c)$. Monotonicity and preservation of constant states give $|U_j^{n+1}-c|\leq|U_j^n-c|-(k/d)(Q_{j+1/2}-Q_{j-1/2})$. At equal states $Q(u,u;c)=\operatorname{sgn}(u-c)(f(u)-f(c))$, the [Kruzhkov entropy flux](#kruzhkov-entropy-flux). Such discrete inequalities connect stability of a [monotone conservative scheme](numerical-analysis.md#monotone-conservative-scheme) with the admissibility of its limiting [entropy solution](#entropy-solution).

###### Averaged initial trace of an entropy solution

↑ **Parent:** [Entropy solution](#entropy-solution)

For a bounded [entropy solution](#entropy-solution) with its initial entropy inequalities, the displayed limit holds on every compact spatial set. Test a constant-level entropy with $(1-t/\delta)_+\rho(x)$. The flux remainder is $O(\delta)$, giving a bound by $\int\rho|u_0-k|$. A finite smooth partition and constant levels approximate the initial function in local $L^1$; the triangle inequality makes the limsup arbitrarily small. This averaged trace suffices for one-sided time mollifiers supported in $[\delta,2\delta]$.

###### Entropy flux for a scalar conservation law

↑ **Parent:** [Entropy solution](#entropy-solution)

A convex entropy $\eta$ is paired with any flux antiderivative satisfying $q'(z)=\eta'(z)f'(z)$ almost everywhere. Its admissibility inequality is $\partial_t\eta(u)+\partial_xq(u)\le0$ distributionally, with the matching initial entropy trace. Affine entropies $\eta(z)=\pm z$ recover the [weak formulation](#weak-formulation), while bounded classical solutions satisfy equality for smooth entropies and then by approximation for piecewise smooth convex entropies.

###### Kruzhkov entropy flux

↑ **Parent:** [Entropy flux for a scalar conservation law](#entropy-flux-for-a-scalar-conservation-law)

For $\eta_k(z)=|z-k|$, the displayed flux is continuous at $z=k$ and has [derivative](calculus.md#derivative) $\operatorname{sgn}(z-k)f'(z)$ almost everywhere. On a bounded state range with $|f'|\le M$, its symmetric two-state version $Q(a,b)$ obeys $|Q(a,b)|\le M|a-b|$ and is Lipschitz in both arguments. The vanishing factor at $a=b$ removes any sign-function jump contribution.

###### Doubling of variables for scalar conservation laws

↑ **Parent:** [Kruzhkov entropy flux](#kruzhkov-entropy-flux)

Apply the [entropy solution](#entropy-solution) inequality for $u(t,x)$ with level $v(s,y)$ and for $v(s,y)$ with level $u(t,x)$, integrate both in the other pair of variables, and add them. Symmetry of the [Kruzhkov entropy flux](#kruzhkov-entropy-flux) produces [derivatives](calculus.md#derivative) $\partial_t+\partial_s$ and $\partial_x+\partial_y$. A nonnegative mollifier concentrated near the diagonal then yields the [Kato inequality for scalar conservation laws](#kato-inequality-for-scalar-conservation-laws). Boundary-time terms require an initial trace argument, not merely interior translation continuity.

###### Kato inequality for scalar conservation laws

↑ **Parent:** [Doubling of variables for scalar conservation laws](#doubling-of-variables-for-scalar-conservation-laws)

For bounded [entropy solutions](#entropy-solution) of the same scalar law, $Q(u,v)=\operatorname{sgn}(u-v)(f(u)-f(v))$ satisfies the displayed distributional inequality, with initial value $|u_0-v_0|$ in its test-function form. The [doubling of variables for scalar conservation laws](#doubling-of-variables-for-scalar-conservation-laws), local translation continuity and the [averaged initial trace of an entropy solution](#averaged-initial-trace-of-an-entropy-solution) prove it. Its significance is comparison between two solutions rather than an inequality against a constant state.

###### Local L1 contraction for scalar conservation laws

↑ **Parent:** [Kato inequality for scalar conservation laws](#kato-inequality-for-scalar-conservation-laws)

If $|f'|\le M$ on the solutions' state range, the [Kato inequality for scalar conservation laws](#kato-inequality-for-scalar-conservation-laws) implies the displayed estimate for almost every $s\in[0,t]$. Approximate the shrinking interval by smooth cutoffs $W$ satisfying $W_s+M|W_x|\le0$ and multiply by a temporal cutoff ending at $s$. Since $|Q|\le M|u-v|$, the lateral flux cannot increase the integral. The estimate gives uniqueness and a [finite propagation speed](wave-equation.md#finite-propagation-speed) without global $L^1$ assumptions on the data.

###### Order preservation for scalar entropy solutions

↑ **Parent:** [Local L1 contraction for scalar conservation laws](#local-l1-contraction-for-scalar-conservation-laws)

Subtract the weak equation for $u-v$ from its [Kato inequality for scalar conservation laws](#kato-inequality-for-scalar-conservation-laws) and divide by two. The result is an inequality for $(v-u)_+$ with a flux bounded in magnitude by $M(v-u)_+$. The same shrinking-interval argument proves $u_0\ge v_0\Rightarrow u\ge v$ almost everywhere. Choosing the constant solution $v=0$ proves preservation of nonnegativity even when $f(0)\ne0$. Two-sided absolute-value contraction alone should not be mistaken for this one-sided comparison proof.

#### Characteristic crossing

↑ **Parent:** [Scalar conservation law](#scalar-conservation-law)

Characteristic crossing occurs when the map from an initial point to its position at time $t$ loses injectivity. For $u_t+f(u)_x=0$, its Jacobian is $1+t f''(u_0)u_0'$ in the autonomous case, so a negative value of $f''(u_0)u_0'$ causes finite-time crossing.

##### Gradient blow-up

↑ **Parent:** [Characteristic crossing](#characteristic-crossing)

Gradient blow-up means that a solution stays bounded while the norm of a spatial derivative tends to infinity. In a scalar conservation law this happens as characteristics meet, because the derivative contains the reciprocal of the characteristic-map Jacobian.

## Elliptic boundary value problem

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)

[This section is present in another page, follow this link to view it.](elliptic-boundary-value-problem.md)

## Helmholtz equation

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Helmholtz_equation)

The Helmholtz equation is the constant-coefficient elliptic equation

$$
\Delta u+k^2u=0.
$$

On a bounded domain, nonzero Dirichlet solutions occur when $k^2$ is an eigenvalue of the negative Laplacian.

### Helmholtz Green-function reciprocity

↑ **Parent:** [Helmholtz equation](#helmholtz-equation)

Two [Green functions](analysis.md#green-s-function) of the same [Helmholtz equation](#helmholtz-equation) with the same homogeneous [Robin boundary condition](differential-equation.md#robin-boundary-condition) satisfy the displayed reciprocity by [Green's second identity](#green-second-identity). It is a bilinear identity without complex conjugation, so it concerns the transpose rather than the Hermitian adjoint. In an exterior problem both kernels use the same radiation convention.

### Discrete Helmholtz resonance

↑ **Parent:** [Helmholtz equation](#helmholtz-equation)

On a square Dirichlet grid with spacing $h=1/J$ and interior indices $1,\ldots,J-1$, the [five-point Laplacian](finite-difference.md#five-point-laplacian) is diagonalized by products of the sine modes used in the [discrete sine transform](numerical-analysis.md#discrete-sine-transform). The discrete equation $(\Delta_h+\lambda I)U=F$ is nonsingular exactly when $\lambda$ is not one of the displayed positive [eigenvalues](linear-operator-theory.md#eigenvalue) of $-\Delta_h$, with $1\leq p,q\leq J-1$. Values below the first resonance are sufficient but not necessary for invertibility.

### Dirichlet-to-Neumann map for a Helmholtz half-space

↑ **Parent:** [Helmholtz equation](#helmholtz-equation)

For the upward derivative at a flat boundary, the [Dirichlet-to-Neumann map for a Helmholtz half-space](#dirichlet-to-neumann-map-for-a-helmholtz-half-space) is the [Fourier multiplier](analysis.md#fourier-multiplier) $i\beta(q)$. The outward normal of the upper half-space points downward and has the opposite sign. Its evanescent multiplier grows like $|q|$, explaining why fine roughness matters even when the height is small.

### Outgoing Green function for the three-dimensional Helmholtz equation

↑ **Parent:** [Helmholtz equation](#helmholtz-equation)

The outgoing [Green function](analysis.md#green-s-function) satisfies $(\Delta+k^2)G_k=-\delta_{\mathbf r'}$ and the [Sommerfeld radiation condition](inverse-problem.md#sommerfeld-radiation-condition). For time dependence $e^{-i\omega t}$, its radial phase travels outward. Away from its source it solves the homogeneous [Helmholtz equation](#helmholtz-equation). At large $r$, $G_k=e^{ikr}e^{-ik\widehat{\mathbf r}\cdot\mathbf r'}/(4\pi r)+O(r^{-2})$.

#### Weyl plane-wave representation

↑ **Parent:** [Outgoing Green function for the three-dimensional Helmholtz equation](#outgoing-green-function-for-the-three-dimensional-helmholtz-equation)

Here $m=\sqrt{1-p^2-q^2}$ has nonnegative imaginary part. This representation of the outgoing [Helmholtz equation](#helmholtz-equation) kernel separates propagating [plane waves](quantum-mechanics.md#plane-wave) from [evanescent waves](continuum-mechanics.md#evanescent-wave). The absolute vertical separation is required for fields on either side of a source; choosing its sign fixes the upward or downward angular spectrum.

### Wave scattering at a planar interface

↑ **Parent:** [Helmholtz equation](#helmholtz-equation)

Wave scattering at a planar interface separates an incident [plane wave](quantum-mechanics.md#plane-wave) into reflected and transmitted plane waves. Translation invariance parallel to the interface conserves the tangential component of the wavevector.

#### Vertical wavenumber

↑ **Parent:** [Wave scattering at a planar interface](#wave-scattering-at-a-planar-interface)

Relative to a distinguished propagation coordinate $z$, the vertical wavenumber is the corresponding wavevector component $q$. For a plane wave of wavenumber $k$ making angle $\theta$ with the vertical, $q=k\cos\theta$.

<h4 id="snell-s-law">Snell's law</h4>

↑ **Parent:** [Wave scattering at a planar interface](#wave-scattering-at-a-planar-interface)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Snell's_law)

Snell's law follows from conservation of tangential wavenumber across a planar interface. If angles are measured from the interface normal, it reads $n_1\sin\theta_1=n_2\sin\theta_2$.

#### Scalar-wave interface condition

↑ **Parent:** [Wave scattering at a planar interface](#wave-scattering-at-a-planar-interface)

For a scalar field satisfying second-order wave equations with the same leading coefficient on either side of an interface, continuity of the field and its normal derivative supplies two interface conditions. Different constitutive laws can instead impose weighted normal-derivative continuity.

#### Reflection and transmission coefficients at a scalar-wave interface

↑ **Parent:** [Wave scattering at a planar interface](#wave-scattering-at-a-planar-interface)

For incident and transmitted normal wavenumbers $q_0$ and $q_1$, continuity of a scalar field and its normal derivative gives

$$
R=\frac{q_0-q_1}{q_0+q_1},
\qquad
T=\frac{2q_0}{q_0+q_1}.
$$

##### Reflection coefficient

↑ **Parent:** [Reflection and transmission coefficients at a scalar-wave interface](#reflection-and-transmission-coefficients-at-a-scalar-wave-interface)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reflection_coefficient)

The reflection coefficient is the complex ratio between reflected and incident wave amplitudes. Its modulus determines amplitude attenuation and its argument determines the phase shift on reflection.

##### Transmission coefficient

↑ **Parent:** [Reflection and transmission coefficients at a scalar-wave interface](#reflection-and-transmission-coefficients-at-a-scalar-wave-interface)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transmission_coefficient)

The transmission coefficient is the complex ratio between transmitted and incident wave amplitudes. Flux transmission may also contain an impedance or normal-wavenumber factor and therefore need not equal $|T|^2$.

### Phase screen

↑ **Parent:** [Helmholtz equation](#helmholtz-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Phase_screen)

A phase screen is a thin inhomogeneous layer idealized as changing only a wave's phase. A random phase screen converts a coherent incident wave into coherent and diffuse components whose moments are determined by the phase covariance.

#### Phase-to-intensity conversion near a deterministic phase screen

↑ **Parent:** [Phase screen](#phase-screen)

For $E(0,z)=e^{i\phi(z)}$ and sufficiently smooth real phase, expand free [paraxial propagation](#paraxial-approximation) as $E=E_0+ixE_0''/(2k)-x^2E_0''''/(8k^2)+O(x^3)$. Taking the squared modulus gives the displayed intensity. Negative phase curvature initially focuses the field. With $\phi=\cos z$, $I=1+(x/k)\cos z+(x/k)^2\cos2z+O(x^3)$, with transverse length scaled so the modulation wavenumber is one. Period-averaged intensity stays one.

#### Random phase screen

↑ **Parent:** [Phase screen](#phase-screen)

##### Stationary phase-screen power spectrum

↑ **Parent:** [Random phase screen](#random-phase-screen)

For the [random phase screen](#random-phase-screen) $E(z)=e^{i\beta W(z)}$, the [Gaussian phase-screen correlation](#gaussian-phase-screen-correlation) and [spectral measure of a stationary random field](time-series.md#spectral-measure-of-a-stationary-random-field) give

$$
S_E(\nu)=\frac1{2\pi}\int_{\mathbb R}e^{-\beta^2(1-\rho(\zeta))}e^{-i\nu\zeta}\,d\zeta.
$$

If $\rho(\zeta)\to0$ and $e^{\beta^2\rho}-1$ is integrable, this is $e^{-\beta^2}\delta(\nu)$ plus the continuous density $(2\pi)^{-1}e^{-\beta^2}\int(e^{\beta^2\rho(\zeta)}-1)e^{-i\nu\zeta}d\zeta$. The total mass is one, split into coherent mass $e^{-\beta^2}$ and diffuse mass $1-e^{-\beta^2}$. Without the decay and integrability assumptions there may be additional spectral atoms or singular components.

##### Gaussian phase-screen correlation

↑ **Parent:** [Random phase screen](#random-phase-screen)

Let $W(z)$ be a stationary real [Gaussian process](stochastic-process.md#gaussian-process) of mean zero and [variance](variance.md) one, with [autocorrelation](time-series.md#autocorrelation) $\rho(\zeta)$. The [random phase screen](#random-phase-screen) $E(z)=e^{i\beta W(z)}$ has uncentered correlation $C_E(\zeta)=\mathbb E[E(z+\zeta)\overline{E(z)}]=e^{-\beta^2(1-\rho(\zeta))}$. This follows from the [characteristic function](probability-theory.md#characteristic-function) of the Gaussian difference, whose [variance](variance.md) is $2(1-\rho(\zeta))$. Joint Gaussianity is essential; normal one-point [marginal distributions](probability-theory.md#marginal-distribution) alone are insufficient.

##### Gaussian phase averaging

↑ **Parent:** [Random phase screen](#random-phase-screen)

For a centered real [Gaussian random variable](probability-theory.md#gaussian-random-variable) $\phi$, its [characteristic function](probability-theory.md#characteristic-function) gives $\mathbb E e^{i\phi}=\exp[-\operatorname{Var}(\phi)/2]$. Applied to a [random phase screen](#random-phase-screen), this controls the [coherent and diffuse wave fields](#coherent-and-diffuse-wave-fields).

#### Parabolic wave equation

↑ **Parent:** [Phase screen](#phase-screen)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Parabolic_wave_equation)

The parabolic wave equation is a one-way, slowly varying envelope approximation to the [Helmholtz equation](#helmholtz-equation). For carrier wavenumber $k$ and transverse coordinate $z$, a common form is $2ikE_x+E_{zz}=0$.

##### Stationary intensity under free paraxial propagation

↑ **Parent:** [Parabolic wave equation](#parabolic-wave-equation)

The free [parabolic wave equation](#parabolic-wave-equation) multiplies each transverse [Fourier mode](fourier-analysis.md#fourier-mode) by $e^{-i\nu^2x/(2k)}$, of unit modulus. A statistically stationary input therefore keeps its uncentered spectral measure and mean intensity. A pure phase screen of unit incident amplitude has total mean intensity one even when its coherent intensity is smaller. This statement does not require a Gaussian joint phase distribution; second-order stationarity and free paraxial propagation suffice.

##### Mutual coherence in a white-noise parabolic medium

↑ **Parent:** [Parabolic wave equation](#parabolic-wave-equation)

A [parabolic wave equation](#parabolic-wave-equation) driven by longitudinal [Gaussian white noise](stochastic-process.md#gaussian-white-noise) with transverse [covariance kernel](random-variable.md#covariance-kernel) $C$ has the displayed closed [mutual coherence](numerical-analysis.md#coherence-of-a-normalized-matrix) equation. The noise is the derivative of a [longitudinal Brownian field with transverse covariance](brownian-motion.md#longitudinal-brownian-field-with-transverse-covariance); the physical smooth-noise limit uses the [Stratonovich integral](stochastic-calculus.md#stratonovich-integral). Conversion to the [Itô integral](stochastic-calculus.md#ito-integral) supplies the attenuation drift and the cross variation supplies the $C(\mathbf s_1-\mathbf s_2)$ term. For unit plane-wave incidence and transverse [statistical homogeneity](probability-and-statistics.md#statistical-homogeneity), $\Gamma=\exp[-k^2\mu^2x(C(0)-C(\mathbf s_1-\mathbf s_2))]$. General Gaussian colored media do not have this local closure.

##### Norm conservation for the scalar parabolic wave equation

↑ **Parent:** [Parabolic wave equation](#parabolic-wave-equation)

For $U_x=iL(x)U$ with a self-adjoint transverse [differential operator](analysis.md#differential-operator) $L(x)$, differentiating the squared [L2 norm](real-analysis.md#l2-norm) gives $i\langle U,LU\rangle-i\langle LU,U\rangle=0$. Reality of the refractive coefficient and vanishing transverse boundary flux are required. This is exact for the scalar envelope model. Its physical interpretation as leading paraxial power uses a fixed reference impedance; a varying local impedance or a longitudinal electromagnetic polarization requires a consistent Maxwell calculation and cannot be inferred from this invariant alone.

##### Colored Gaussian paraxial mean propagator

↑ **Parent:** [Parabolic wave equation](#parabolic-wave-equation)

For $E_x=i\Delta_\perp E/(2k)+ik\mu WE$, a jointly Gaussian colored medium has covariance $C(s,\mathbf r)$. Averaging the equation gives a term $\langle WE\rangle$; the [Furutsu–Novikov formula](stochastic-process.md#novikov-s-theorem) expresses it through the random propagator and the functional derivative of $E$. It does not generally close in the mean field alone. A phase-screen product followed by Gaussian averaging gives a formal exact mean propagator, with factor $\exp[-k^2\mu^2\Delta x^2\sum_{j,l}C(x_j-x_l,\mathbf r_j-\mathbf r_l)/2]$ for each transverse path. In the longitudinal white-noise limit the covariance collapses to equal slices, and the mean closes as $m_x=i\Delta_\perp m/(2k)-k^2\mu^2A(0)m/2$.

##### Paraxial approximation

↑ **Parent:** [Parabolic wave equation](#parabolic-wave-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Paraxial_approximation)

The paraxial approximation describes waves whose propagation directions make small angles with a preferred axis. Factoring out a carrier $e^{ikx}$ and neglecting the envelope's second longitudinal derivative turns the [Helmholtz equation](#helmholtz-equation) into a [parabolic wave equation](#parabolic-wave-equation) and suppresses backward propagation.

##### Split-step Fourier method

↑ **Parent:** [Parabolic wave equation](#parabolic-wave-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Split-step_Fourier_method)

The split-step Fourier method alternates local phase accumulation with free diffraction. For $E_x=(D+S)E$ over a step $\Delta x$, [Lie-Trotter splitting](numerical-analysis.md#lie-product-formula) gives

$$
E(x+\Delta x)\simeq e^{\Delta xD}e^{\Delta xS}E(x),
$$

and a transverse [Fourier transform](analysis.md#fourier-transform) applies the constant-coefficient diffraction exponential efficiently.

##### Free-space diffraction

↑ **Parent:** [Parabolic wave equation](#parabolic-wave-equation)

In a homogeneous medium, a paraxial envelope satisfies $E_x=i\Delta_\perp E/(2k)$. This free-space diffraction spreads transverse Fourier modes by the phase factor $\exp(-ix|\mathbf p|^2/(2k))$.

###### Sommerfeld half-plane diffraction

↑ **Parent:** [Free-space diffraction](#free-space-diffraction)

For a Neumann screen on the negative horizontal axis, the [Helmholtz equation](#helmholtz-equation) has an exact solution in [Fresnel integrals](analysis.md#fresnel-integral). With time dependence $e^{i\omega t}$, a wave incident from angle $0<\theta_0<\pi$ has total field $e^{ikr\cos(\theta-\theta_0)}\mathcal F(s_-)+e^{ikr\cos(\theta+\theta_0)}\mathcal F(-s_+)$, where $s_\pm=\sqrt{2kr}\cos[(\theta\pm\theta_0)/2]$ and $\mathcal F(s)=\tfrac12\operatorname{erfc}(-e^{i\pi/4}s)$. The angular derivatives cancel on both faces of the screen. Away from the two shadow boundaries, the [Fresnel tail expansion](analysis.md#fresnel-tail-expansion) splits this into incident/reflected [geometrical optics](optics.md#geometrical-optics) fields and an outgoing edge wave proportional to $r^{-1/2}e^{-ikr}$.

###### Wiener-Hopf solution of rigid half-plane diffraction

↑ **Parent:** [Sommerfeld half-plane diffraction](#sommerfeld-half-plane-diffraction)

For a rigid screen $x<0$, use time dependence $e^{i\omega t}$ and inverse [Fourier transform](analysis.md#fourier-transform) $e^{-i\kappa x}$. The scattered field is odd in $y$. Its upper-face trace is supported on $x<0$, while its normal derivative on $x>0$ is unknown. With the outgoing factor $\gamma=\sqrt{\kappa^2-k_0^2}$, these traces satisfy $\gamma\widehat\phi^-+G^+=b/(\kappa+a)$, where $a=k_0\cos\theta_0$ and $b=k_0\sin\theta_0$. Factor $\gamma=\sqrt{\kappa-k_0}\sqrt{\kappa+k_0}$ into upper/lower analytic factors. [Pole subtraction in a Wiener-Hopf equation](differential-equation.md#pole-subtraction-in-a-wiener-hopf-equation) and the finite-energy edge condition give the displayed trace. The forcing-pole [residue](analysis.md#residue) yields [geometrical optics](optics.md#geometrical-optics), while [stationary phase](analysis.md#stationary-phase-method) yields the outgoing edge wave

$$
\phi_d\sim\sqrt{\frac{2}{\pi k_0r}}\frac{\sin(\theta_0/2)\sin(\theta/2)}{\cos\theta+\cos\theta_0}e^{-ik_0r-i\pi/4}.
$$

The angular formula excludes the shadow-boundary transition regions; the exact integral supplies their uniform continuation.

###### Fresnel propagator

↑ **Parent:** [Free-space diffraction](#free-space-diffraction)

In two transverse dimensions, the [Fresnel propagator](#fresnel-propagator) has kernel $k_0(2\pi i x)^{-1}\exp(ik_0|\mathbf z-\mathbf z'|^2/(2x))$ for $x>0$. It evolves the homogeneous [parabolic wave equation](#parabolic-wave-equation).

###### One-dimensional transverse Fresnel propagation

↑ **Parent:** [Fresnel propagator](#fresnel-propagator)

For one transverse coordinate, the [parabolic wave equation](#parabolic-wave-equation) $2ikE_x+E_{zz}=0$ has the [Fresnel propagator](#fresnel-propagator) kernel

$$
(U_x f)(z)=\sqrt{\frac{k}{2\pi ix}}\int_{\mathbb R}
e^{ik(z-z')^2/(2x)}f(z')\,dz',\qquad x>0.
$$

The square root uses $\sqrt{1/i}=e^{-i\pi/4}$. With $\widehat f(\nu)=(2\pi)^{-1}\int f(z)e^{-i\nu z}dz$, its [Fourier transform](analysis.md#fourier-transform) multiplier is $e^{-i\nu^2x/(2k)}$. This distinguishes the one-transverse-coordinate prefactor from the two-coordinate kernel. The operator is unitary on $L^2(\mathbb R)$, although its spatial integral is interpreted as an oscillatory integral.

###### Free-space fourth-moment propagator

↑ **Parent:** [Free-space diffraction](#free-space-diffraction)

For $m_x=(i/k)m_{r_1r_2}$, the free-space fourth-moment propagator multiplies the two-dimensional Fourier transform by $e^{-ixp_1p_2/k}$. In physical coordinates its oscillatory kernel is

$$
K_x(r_1,r_2)=\frac{k}{2\pi x}e^{ikr_1r_2/x}.
$$

#### Coherent and diffuse wave fields

↑ **Parent:** [Phase screen](#phase-screen)

The coherent field is the ensemble mean $\langle E\rangle$ of a randomly scattered wave. The zero-mean remainder $E-\langle E\rangle$ is the diffuse or incoherent field.

##### Coherent attenuation by a Gaussian phase screen

↑ **Parent:** [Coherent and diffuse wave fields](#coherent-and-diffuse-wave-fields)

For a unit-amplitude [random phase screen](#random-phase-screen) $e^{i\beta W}$ with standard normal [marginal distribution](probability-theory.md#marginal-distribution), the [characteristic function](probability-theory.md#characteristic-function) gives coherent amplitude $m=\mathbb E[e^{i\beta W}]=e^{-\beta^2/2}$. The coherent power is $|m|^2=e^{-\beta^2}$, although the total power remains one. In homogeneous paraxial space the mean constant transverse field propagates without additional attenuation. Under decorrelation at large separation, the remaining power $1-e^{-\beta^2}$ is diffuse.

##### Coherent attenuation in a white-noise random medium

↑ **Parent:** [Coherent and diffuse wave fields](#coherent-and-diffuse-wave-fields)

For a [parabolic wave equation](#parabolic-wave-equation) driven by longitudinal [Gaussian white noise](stochastic-process.md#gaussian-white-noise) with transverse [covariance kernel](random-variable.md#covariance-kernel) $B$, the mean envelope obeys $\partial_x m=i\Delta_\perp m/(2k_0)-\gamma m$. This closure requires [independent increments](stochastic-process.md#independent-increments) in the longitudinal direction; [statistical homogeneity](probability-and-statistics.md#statistical-homogeneity) and one-point [Gaussian distributions](probability-theory.md#normal-distribution) alone are insufficient.

#### Phase curvature

↑ **Parent:** [Phase screen](#phase-screen)

Phase curvature is a transverse second derivative of wave phase. Under subsequent free-space propagation, positive and negative curvature cause local defocusing and focusing and thereby convert phase modulation into amplitude modulation.

## Modified Helmholtz equation

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)

The modified Helmholtz equation is

$$
\Delta u-m^2u=0.
$$

It reduces to the [Laplace equation](#laplace-equation) when $m=0$.

### Quadrant modified Helmholtz Dirichlet Poisson formula

↑ **Parent:** [Modified Helmholtz equation](#modified-helmholtz-equation)

Here $B(p)=\sqrt{p^2+4\lambda}$ and $S_j$ are the [Fourier sine transforms](analysis.md#fourier-sine-transform) of the boundary values. The [modified Helmholtz closed spectral one-form](#modified-helmholtz-closed-spectral-one-form) and its reflected [global relations](differential-equation.md#global-relation-for-a-linear-boundary-value-problem) remove the unknown normal traces. Equivalently, four reflected [fundamental solutions](distribution-theory.md#fundamental-solution-of-a-linear-differential-operator) give a zero-boundary [Green function](analysis.md#green-s-function) in the quadrant. Its inward derivatives give the displayed formula. The two terms recover the bottom and left traces respectively; matching corner values ensure continuity at the corner.

### Modified Helmholtz closed spectral one-form

↑ **Parent:** [Modified Helmholtz equation](#modified-helmholtz-equation)

For $k\ne0$, differentiation gives $dW=-2e^{-ikz-\lambda\bar z/(ik)}(q_{z\bar z}-\lambda q)dz\wedge d\bar z$. Thus the [differential form](differential-form.md) is closed precisely for the [modified Helmholtz equation](#modified-helmholtz-equation) $\Delta q-4\lambda q=0$. Integrating around an oriented domain gives a [global relation](differential-equation.md#global-relation-for-a-linear-boundary-value-problem). The primitive $\mu e^{-ikz-\lambda\bar z/(ik)}$ also produces compatible first-order equations whose spectral jumps reconstruct $q$.

### Two-dimensional modified Helmholtz fundamental solution

↑ **Parent:** [Modified Helmholtz equation](#modified-helmholtz-equation)

For $m>0$, the decaying fundamental solution of $-\Delta+m^2$ in two dimensions is $K_0(mr)/(2\pi)$, with $K_0$ the [Modified Bessel function of the second kind](analysis.md#modified-bessel-function-of-the-second-kind). [Green second identity](#green-second-identity) reconstructs an interior solution from its [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition) $f$ and outward [normal derivative](differential-geometry.md#normal-derivative) $h$ as $q(r)=\int_{\partial\Omega}(\Gamma_m h-f\partial_n\Gamma_m)ds$.

### Modified Helmholtz adjoint plane wave

↑ **Parent:** [Modified Helmholtz equation](#modified-helmholtz-equation)

For $k>0$, a nonzero [spectral parameter for a linear boundary value problem](differential-equation.md#spectral-parameter-for-a-linear-boundary-value-problem) gives

$$
v_\lambda=\exp[ik(\lambda z-\overline z/\lambda)/2]=e^{Ax+By},\quad A=ik(\lambda-\lambda^{-1})/2,\quad B=-k(\lambda+\lambda^{-1})/2.
$$

The identity $A^2+B^2=k^2$ proves that this solves the [modified Helmholtz equation](#modified-helmholtz-equation). The reciprocal companion is $v_{1/\lambda}=\overline{v_{\overline\lambda}}$.

#### Side localization of modified Helmholtz plane waves

↑ **Parent:** [Modified Helmholtz adjoint plane wave](#modified-helmholtz-adjoint-plane-wave)

On a square, a normalized [modified Helmholtz adjoint plane wave](#modified-helmholtz-adjoint-plane-wave) with positive normal growth toward one side has magnitude one there, magnitude $e^{-2\eta}$ on the opposite side, and an adjacent-side magnitude integral bounded by $1/\eta$. Thus large tangential spectral frequencies suppress remote-side normal-trace coefficients. Paired [sine collocation of square modified Helmholtz global relations](differential-equation.md#sine-collocation-of-square-modified-helmholtz-global-relations) further cancels adjacent-side unknown traces exactly.

### Radial modified Helmholtz equation

↑ **Parent:** [Modified Helmholtz equation](#modified-helmholtz-equation)

For a [radial function](#radial-function) in three dimensions, $(\Delta-1)y=g(x)$ becomes $y''+2y'/x-y=g(x)$. Setting $u=xy$ gives $u''-u=xg(x)$, reducing it to a constant-coefficient [linear ordinary differential equation](differential-equation.md#linear-ordinary-differential-equation). If $g=e^{-3x}/x^2$, a decaying particular solution obtained by [variation of parameters](differential-equation.md#variation-of-parameters) is

$$
y(x)=\alpha\frac{e^{-x}}x+\frac{e^{-x}E_1(2x)-e^xE_1(4x)}{2x}.
$$

The [small-argument expansion of the exponential integral](complex-analysis.md#small-argument-expansion-of-the-exponential-integral) gives

$$
y(x)=\frac{\alpha+\tfrac12\log2}{x}+\log x-\alpha+\tfrac32\log2+\gamma-1+O(x\log x).
$$

The undetermined decaying homogeneous coefficient $\alpha$ is fixed by a boundary condition or by a [matched asymptotic expansion](differential-equation.md#matched-asymptotic-expansion).

## Poisson equation

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poisson_equation)

### Poisson equation on a disk with angular forcing

↑ **Parent:** [Poisson equation](#poisson-equation)

For the [Poisson equation](#poisson-equation) $\Delta u=\sum_{n\geq1}b_n\sin(n\theta)$ on the unit disk with zero [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition), [separation of variables](#separation-of-variables) in [polar coordinates](calculus.md#polar-coordinates) gives $r^2R_n''+rR_n'-n^2R_n=r^2$. For $n\ne2$, boundedness at $r=0$ and $R_n(1)=0$ select $R_n=(r^n-r^2)/(n^2-4)$. The resonant mode is $R_2=r^2\log r/4$. For discontinuous angular data, the [Poisson equation](#poisson-equation) is interpreted in its [weak formulation](#weak-formulation); its [Dirichlet energy](differential-geometry.md#dirichlet-energy) gives uniqueness. [Orthogonality](linear-algebra.md#orthogonal-vectors) of the angular [Fourier modes](fourier-analysis.md#fourier-mode) gives $\int u f\,dA=-\sum_n\pi b_n^2/[4(n+2)^2]$, with the resonant case obtained directly or by the limit $n\to2$.

### Neumann Poisson problem

↑ **Parent:** [Poisson equation](#poisson-equation)

On a smooth bounded connected domain, the homogeneous Neumann problem seeks $u\in H^1(U)$ such that $\int\nabla u\cdot\nabla v=\int fv$ for every $v\in H^1(U)$. For $f\in L^2(U)$ it is solvable exactly when $\int f=0$, and the [weak solution](#weak-solution) is unique up to constants. The [Poincare-Wirtinger inequality](sobolev-space.md#poincare-wirtinger-inequality) and the [Riesz representation theorem](hilbert-space.md#riesz-representation-theorem) give existence on the [mean-zero Sobolev space](sobolev-space.md#mean-zero-sobolev-space). The test function one gives necessity of the compatibility condition.

### Radial Poisson gradient estimate

↑ **Parent:** [Poisson equation](#poisson-equation)

For a radial Dirichlet solution on a fixed three-dimensional shell $a<r<b$, $(r^2U')'=r^2F$. Thus $r^2U'=C_0+\int_a^rs^2F(s)\,ds$, and $U(a)=U(b)=0$ bounds $|C_0|$ by the supremum of that integral. [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) in the radial volume measure bounds the integral by $C\|f\|_2$. Since $r\ge a>0$, the displayed [gradient](calculus.md#gradient) bound follows. The estimate exploits radiality and does not extend to arbitrary forcing in three dimensions.

#### Failure of L2-to-Linfinity Poisson gradient bounds in three dimensions

↑ **Parent:** [Radial Poisson gradient estimate](#radial-poisson-gradient-estimate)

Inside any three-dimensional domain containing a ball, let $u_\varepsilon(x)=\varepsilon^{1/2}\phi((x-x_0)/\varepsilon)$ for a fixed smooth compactly supported nonconstant function. The right-hand side $f_\varepsilon=\Delta u_\varepsilon$ has constant $L^2$ [norm](functional-analysis.md#norm), whereas $\|\nabla u_\varepsilon\|_\infty=\varepsilon^{-1/2}\|\nabla\phi\|_\infty$ diverges. The functions have zero boundary trace, giving a scaling counterexample to a uniform $L^2$-forcing [gradient](calculus.md#gradient) estimate.

### Poisson kernel for the upper half-space

↑ **Parent:** [Poisson equation](#poisson-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poisson_kernel_for_the_upper_half-space)

The upper-half-space Poisson kernel gives the harmonic extension of boundary data.

#### Poisson kernel for the upper half-plane

↑ **Parent:** [Poisson kernel for the upper half-space](#poisson-kernel-for-the-upper-half-space)

For the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis), the Poisson kernel is

$$
P_y(x-v)=\frac1\pi\frac{y}{(x-v)^2+y^2}.
$$

It is the density of [harmonic measure](brownian-motion.md#harmonic-measure) on the real boundary as viewed from $x+iy$.

#### Poisson integral

↑ **Parent:** [Poisson kernel for the upper half-space](#poisson-kernel-for-the-upper-half-space)

The Poisson integral convolves boundary data with the [Poisson kernel](#poisson-kernel-for-the-upper-half-plane) to produce a [harmonic function](#harmonic-function) in a half-space. In the upper half-plane,

$$
u(x,y)=\frac1\pi\int_{\mathbb R}\frac{y f(v)}{(x-v)^2+y^2}\,dv.
$$

##### Dirichlet Poisson integral in a quadrant

↑ **Parent:** [Poisson integral](#poisson-integral)

The [conformal map](geometry-and-topology.md#conformal-map) $w=z^2$ sends $x,y>0$ to the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis). For bounded continuous boundary values $g_2$ on the horizontal axis and $g_1$ on the vertical axis with equal corner values, set $f(s)=g_2(\sqrt s)$ for $s>0$ and $f(s)=g_1(\sqrt{-s})$ for $s<0$. The bounded [harmonic function](#harmonic-function) with those [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition) is

$$
u(z)=\frac1\pi\int_{\mathbb R}\frac{\operatorname{Im}(z^2)f(s)}{|s-z^2|^2}\,ds.
$$

Equivalently, if $z^2=a+ic$ with $c>0$, this is $\frac{2c}{\pi}\int_0^\infty r\left[g_2(r)/((r^2-a)^2+c^2)+g_1(r)/((r^2+a)^2+c^2)\right]dr$. The [Poisson kernel](#poisson-kernel-for-the-upper-half-plane) is a positive [approximate identity](fourier-analysis.md#approximate-identity), so the prescribed edge values are attained. Boundedness is essential for uniqueness on this unbounded domain.

###### Bounded Dirichlet uniqueness in a quadrant

↑ **Parent:** [Dirichlet Poisson integral in a quadrant](#dirichlet-poisson-integral-in-a-quadrant)

Two bounded [harmonic functions](#harmonic-function) continuous to the quadrant edges with the same [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition) are equal. Their difference is bounded and zero on both axes. [Odd reflection](sobolev-space.md#odd-reflection) across each axis gives a bounded harmonic extension away from the corner; the [removable singularity for a bounded harmonic function](#removable-singularity-for-a-bounded-harmonic-function) fills in that corner. The [harmonic Liouville theorem](#harmonic-liouville-theorem) makes that extension constant, and oddness makes the constant zero. This does not exclude unbounded examples such as the [zero-boundary harmonic growth in a quadrant](#zero-boundary-harmonic-growth-in-a-quadrant).

###### Zero-boundary harmonic growth in a quadrant

↑ **Parent:** [Dirichlet Poisson integral in a quadrant](#dirichlet-poisson-integral-in-a-quadrant)

The [harmonic function](#harmonic-function) $v(x,y)=xy$ vanishes on both axes but is nonzero in the quadrant, and $v_z=-iz/2$. More generally $\operatorname{Im}z^{2m}$, for a positive integer $m$, vanishes on both axes and is harmonic. Adding these unbounded functions leaves all edge [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition) unchanged. Thus decay of the boundary data does not imply decay of every solution, and an edge-data-only formula cannot determine an arbitrary solution's [Wirtinger derivative](analysis.md#wirtinger-derivatives). A boundedness or suitable growth condition must select the solution.

###### Holomorphic derivative of a quadrant Dirichlet solution

↑ **Parent:** [Dirichlet Poisson integral in a quadrant](#dirichlet-poisson-integral-in-a-quadrant)

For the bounded [Dirichlet Poisson integral in a quadrant](#dirichlet-poisson-integral-in-a-quadrant), the [Wirtinger derivative](analysis.md#wirtinger-derivatives) is

$$
u_z(z)=\frac{2z}{\pi i}\int_0^\infty r\left[\frac{g_2(r)}{(r^2-z^2)^2}+\frac{g_1(r)}{(r^2+z^2)^2}\right]dr.
$$

This follows by differentiating the [Schwarz integral formula](#schwarz-integral-formula) composed with $z^2$, remembering that for real boundary data $u_z$ is half the derivative of a [holomorphic function](complex-analysis.md#holomorphic-function) whose [real part](complex-analysis.md#real-part) is $u$. For complex boundary data, apply the construction to the real and imaginary parts separately and use linearity. If the data and their [derivatives](calculus.md#derivative) decay sufficiently, [integration by parts](calculus.md#integration-by-parts) gives

$$
u_z(z)=\frac z{\pi i}\left[\int_0^\infty\frac{g_2'(r)}{r^2-z^2}\,dr+\int_0^\infty\frac{g_1'(r)}{r^2+z^2}\,dr\right].
$$

The endpoint terms cancel exactly when $g_1(0)=g_2(0)$. Interior denominators do not vanish because $\operatorname{Im}z^2>0$.

##### Schwarz integral formula

↑ **Parent:** [Poisson integral](#poisson-integral)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schwarz_integral_formula)

The Schwarz integral formula reconstructs a [holomorphic function](complex-analysis.md#holomorphic-function) from boundary values of its [real part](complex-analysis.md#real-part). For a real boundary function $f$ on the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) satisfying $\int_{\mathbb R}|f(s)|/(1+s^2)\,ds<\infty$, the regularized form is

$$
W(w)=\frac1{\pi i}\int_{\mathbb R}f(s)\left[\frac1{s-w}-\frac{s}{1+s^2}\right]ds.
$$

Its [real part](complex-analysis.md#real-part) is the [Poisson integral](#poisson-integral) of $f$. The subtraction makes the integral converge and changes only the imaginary normalization. [Integration by parts](calculus.md#integration-by-parts), when the boundary terms vanish, gives $W'(w)=(\pi i)^{-1}\int f'(s)/(s-w)\,ds$; jumps of $f$ are included as [Dirac delta function](distribution-theory.md#dirac-delta-function) terms in its [distributional derivative](distribution-theory.md#distributional-derivative).

###### Schwarz integral on the unit disk

↑ **Parent:** [Schwarz integral formula](#schwarz-integral-formula)

For real boundary data $u$, the displayed holomorphic integral has real part equal to the disk [Poisson integral](#poisson-integral) of $u$ and imaginary part its normalized [harmonic conjugate](#harmonic-conjugate). If $u\geq0$ is not identically zero, the real part is strictly positive inside the disk. A [holomorphic logarithm](complex-analysis.md#holomorphic-logarithm) then has imaginary part between $-\pi/2$ and $\pi/2$, while its real part records the logarithm of the magnitude. This separates uniform imaginary-part control from large real parts on small boundary sets.

###### Harmonic quadrant solution from tangential boundary derivatives

↑ **Parent:** [Schwarz integral formula](#schwarz-integral-formula)

For a [harmonic function](#harmonic-function) in the quadrant with boundary derivatives $u_y(0,y)=g_1(y)$ and $u_x(x,0)=g_2(x)$, integrating the data to equal corner values and applying the [Schwarz integral formula](#schwarz-integral-formula) after the [conformal map](geometry-and-topology.md#conformal-map) $w=z^2$ gives

$$
u_z(z)=\frac z{\pi i}\left[\int_0^\infty\frac{g_2(r)}{r^2-z^2}\,dr+\int_0^\infty\frac{g_1(r)}{r^2+z^2}\,dr\right].
$$

These are [tangential boundary derivatives](differential-equation.md#tangential-boundary-derivative), so uniqueness requires an additional normalization or growth restriction. A homogeneous contribution has the form $ih(z^2)/z$ with $h$ [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) in the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) and real on its boundary away from zero. For example, $u=xy$ has zero prescribed derivatives on both edges.

## Nonlinear partial differential equation

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nonlinear_partial_differential_equation)

A nonlinear partial differential equation depends nonlinearly on the unknown function or one of its derivatives.

<h3 id="nonlinear-schrodinger-equation">Nonlinear Schrödinger equation</h3>

↑ **Parent:** [Nonlinear partial differential equation](#nonlinear-partial-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nonlinear_Schrödinger_equation)

The nonlinear Schrödinger equation adds an amplitude-dependent interaction to Schrödinger-type wave evolution. Its [Laplacian](calculus.md#laplacian) term disperses the complex wave amplitude, while the sign and form of the nonlinear term determine focusing or defocusing behavior. A one-dimensional cubic specialization is the [focusing nonlinear Schrodinger equation](integrable-systems.md#focusing-nonlinear-schrodinger-equation); members of this broader family need not be [integrable systems](integrable-systems.md).

<h3 id="complex-ginzburg-landau-equation">Complex Ginzburg–Landau equation</h3>

↑ **Parent:** [Nonlinear partial differential equation](#nonlinear-partial-differential-equation)

The [complex Ginzburg–Landau equation](#complex-ginzburg-landau-equation) is a nonlinear complex-amplitude evolution equation with linear and cubic terms and generally complex coefficients. The driven-condensate form $\Psi_t=(\alpha-\beta|\Psi|^2)\Psi+i(\nabla^2-g|\Psi|^2+s)\Psi$ has gain/loss coefficients $\alpha,\beta$ and conservative interaction/frequency coefficients $g,s$. A uniform nonzero state has [number density](statistical-physics.md#number-density) $\alpha/\beta$ when $\alpha,\beta>0$.

A [complex Ginzburg–Landau equation](#complex-ginzburg-landau-equation) describes a [complex number](complex-analysis.md#complex-number) disturbance amplitude through linear amplification, [advection](fluid-mechanics.md#advection), complex [diffusion equation](diffusion-equation.md) terms, and often [cubic amplitude saturation](#cubic-amplitude-saturation). A constant-coefficient example is $\psi_t+U\psi_x=\mu\psi+(1+ic_d)\psi_{xx}-|\psi|^2\psi$. Here real $U,\mu,c_d$ describe transport, linear [growth rate](wave-equation.md#growth-rate) and dispersive [diffusion equation](diffusion-equation.md) terms. Omitting the cubic term gives the [linear complex Ginzburg-Landau equation](#linear-complex-ginzburg-landau-equation).

#### Benjamin-Feir stability condition

↑ **Parent:** [Complex Ginzburg–Landau equation](#complex-ginzburg-landau-equation)

For $A_t=A+(1+ib)A_{xx}-(1+ic)|A|^2A$, the uniform oscillation $A=e^{-ict}$ has phase [diffusion](thermodynamics.md#diffusion) coefficient $D=1+bc$. Its amplitude-phase [dispersion relation](wave-equation.md#dispersion-relation) is $\lambda^2+(2+2k^2)\lambda+2Dk^2+(1+b^2)k^4=0$. Thus $D<0$ gives a long-wavelength [modulational instability](wave-equation.md#modulational-instability), whereas $D>0$ gives [linear stability](dynamical-systems.md#linear-stability) of all nonzero [Fourier modes](fourier-analysis.md#fourier-mode). On a fixed periodic domain, instability requires an allowed wavenumber with $k^2<-2D/(1+b^2)$.

##### Long-wave phase reduction of the complex Ginzburg-Landau equation

↑ **Parent:** [Benjamin-Feir stability condition](#benjamin-feir-stability-condition)

Write $A=e^{-ict}(1+r)e^{i\phi}$. The amplitude relaxes at rate two, while the phase is neutral under constant shifts. Eliminating the damped amplitude on long scales gives $\phi_t=(1+bc)\phi_{xx}+(c-b)(\phi_x)^2-E\phi_{xxxx}+\cdots$, where the linear phase branch has $E=b^2(1+c^2)/2$. Near $1+bc=0$, $E=(1+b^2)/2$ at leading order. Constant phase [symmetry](physics.md#symmetry-physics) forbids undifferentiated phase terms; spatial parity of the leading amplitude equation forbids odd linear derivatives. Balancing negative phase diffusion against the fourth derivative produces the [Kuramoto-Sivashinsky equation](#kuramoto-sivashinsky-equation).

#### Real-coefficient cubic-quintic amplitude equation

↑ **Parent:** [Complex Ginzburg–Landau equation](#complex-ginzburg-landau-equation)

For real $\mu$ and $\alpha>0$, this complex [amplitude equation](dynamical-systems.md#amplitude-equation) has a destabilizing cubic term and a saturating quintic term. Nonzero uniform intensities solve $\mu+\alpha q-q^2=0$. The upper branch is radially stable and the lower branch radially unstable; constant phase is neutral because multiplication by $e^{i\phi_0}$ preserves the equation. Stable conduction and the stable upper pattern coexist for $-\alpha^2/4<\mu<0$. At the fold, a zero radial eigenvalue conceals one-sided nonlinear instability, so strict stability cannot be inferred from eigenvalues alone.

##### Stationary front of a cubic-quintic amplitude equation

↑ **Parent:** [Real-coefficient cubic-quintic amplitude equation](#real-coefficient-cubic-quintic-amplitude-equation)

A nontrivial stationary front of the [real-coefficient cubic-quintic amplitude equation](#real-coefficient-cubic-quintic-amplitude-equation) joining a nonzero pattern to zero must have constant phase. Writing $A=Re^{i\phi}$ gives $R^2\phi'=J$; the finite first integral contains $J^2/(2R^2)$, so approaching zero forces $J=0$. Equal endpoint potentials then give $R_-^2=3\alpha/4$ and the unique parameter $\mu_M=-3\alpha^2/16$. The explicit profile is $A=e^{i\phi_0}\sqrt{(3\alpha/4)/(1+e^{\sqrt3\alpha(x-x_0)/2})}$. This proves existence as well as the necessary equal-potential condition. The zero solution is excluded from the term front.

#### Nonlinear Ginzburg-Landau equation

↑ **Parent:** [Complex Ginzburg–Landau equation](#complex-ginzburg-landau-equation)

This nondispersive cubic [complex Ginzburg–Landau equation](#complex-ginzburg-landau-equation) balances linear growth against nonlinear damping. Its real-wavenumber [Ginzburg-Landau plane wave](#ginzburg-landau-plane-wave) has amplitude $\sqrt{\mu-k^2}$ when $\mu>k^2$. Relaxation within that single-mode amplitude family does not by itself establish stability against general perturbations.

##### Ginzburg-Landau plane wave

↑ **Parent:** [Nonlinear Ginzburg-Landau equation](#nonlinear-ginzburg-landau-equation)

With real $k,U$ and $\mu>k^2$, substitution into the [nonlinear Ginzburg-Landau equation](#nonlinear-ginzburg-landau-equation) cancels the [material derivative](continuum-mechanics.md#material-derivative) and gives $Q^2=\mu-k^2$. A complex $k$ makes the modulus spatially varying, so it generally does not admit this constant-amplitude [nonlinear Ginzburg-Landau equation](#nonlinear-ginzburg-landau-equation) ansatz.

###### Cubic amplitude saturation

↑ **Parent:** [Ginzburg-Landau plane wave](#ginzburg-landau-plane-wave)

For $a>0$, the positive amplitude [ordinary differential equation](differential-equation.md#ordinary-differential-equation) $R'=aR-R^3$ has solution $R(t)=\sqrt a[1+(a/R_0^2-1)e^{-2at}]^{-1/2}$. This follows from the [logistic differential equation](differential-equation.md#logistic-differential-equation) for $R^2$. Every $R_0>0$ approaches $\sqrt a$ as a [monotone function](calculus.md#monotonic-function), and the positive distance to this limit decreases; an oscillating complex wave carrying this amplitude has no ordinary monotone ordering.

#### Linear complex Ginzburg-Landau equation

↑ **Parent:** [Complex Ginzburg–Landau equation](#complex-ginzburg-landau-equation)

A [normal mode](wave-equation.md#normal-mode) $e^{i(kx-\omega t)}$ has [dispersion relation](wave-equation.md#dispersion-relation) $\omega=Uk+(c_d-i)k^2+i\mu$. The [absolute wavenumber](hydrodynamic-stability.md#absolute-wavenumber) is the saddle where $d\omega/dk=0$. The [Green function of the linear complex Ginzburg-Landau equation](#green-function-of-the-linear-complex-ginzburg-landau-equation) distinguishes [convective hydrodynamic instability](hydrodynamic-stability.md#convective-hydrodynamic-instability) from [absolute hydrodynamic instability](hydrodynamic-stability.md#absolute-hydrodynamic-instability).

##### Airy global modes of a linearly confined Ginzburg-Landau equation

↑ **Parent:** [Linear complex Ginzburg-Landau equation](#linear-complex-ginzburg-landau-equation)

On $x>0$ with a homogeneous wall condition, positive [diffusion](thermodynamics.md#diffusion) $\gamma$ and growth $\mu(x)=\mu_0-\epsilon\lambda x$, remove constant drift by $A=e^{Ux/(2\gamma)-i\omega t}f$. The scale $\xi=(\epsilon\lambda/\gamma)^{1/3}x$ reduces the [eigenvalue problem](linear-operator-theory.md#eigenvalue-problem) to the [Airy ordinary differential equation](differential-equation.md#airy-ordinary-differential-equation). Decay selects $f=\operatorname{Ai}(\xi+z_n)$, where $\operatorname{Ai}(z_n)=0$ enforces the wall. The least negative zero $z_1$ sets the [global instability](hydrodynamic-stability.md#global-hydrodynamic-instability) threshold $\mu_0>U^2/(4\gamma)+|z_1|(\epsilon^2\gamma\lambda^2)^{1/3}$. A locally absolutely unstable pocket can therefore exist without an unstable [global mode](hydrodynamic-stability.md#global-hydrodynamic-mode).

##### Green function of the linear complex Ginzburg-Landau equation

↑ **Parent:** [Linear complex Ginzburg-Landau equation](#linear-complex-ginzburg-landau-equation)

For $t>0$ this [Green function](analysis.md#green-s-function) is the response to a point impulse on the infinite line, using the continuous [square root](algebra.md#square-root) of $1+ic_d$. The [Fourier transform](analysis.md#fourier-transform) multiplies the initial transform by $e^{\mu t-ikUt-(1+ic_d)k^2t}$; its Gaussian inverse gives the displayed expression. At fixed $x$, its exponential rate is $\mu-U^2/[4(1+c_d^2)]$, whereas along $x=Ut$ it is $\mu$. Thus a temporally growing flow with $0<\mu<U^2/[4(1+c_d^2)]$ is convectively rather than absolutely unstable.

#### Radial flow near a driven vortex core

↑ **Parent:** [Complex Ginzburg–Landau equation](#complex-ginzburg-landau-equation)

For $[\nabla^2+\xi(1-|\psi|^2)]\psi=0$ and a regular unit-charge core $\psi=f(r)e^{i[\theta+\chi(r)]}$, write current [velocity](classical-mechanics.md#velocity) $u_r=2\chi'$ when the time-dependent kinetic operator is $-\nabla^2$. Separating the imaginary part gives

$$
(rf^2u_r)'=-2\operatorname{Im}\xi\;rf^2(1-f^2).
$$

With $f=ar+O(r^3)$ and no singular core flux, integration gives $u_r=-\operatorname{Im}\xi\,r/2+O(r^3)$. If $\xi=gn_\infty-i\alpha$, the slope is $\alpha/2$. The phase-gradient convention $k=\chi'$ has half this slope, $\alpha/4$. These are local regularity results, not a global vortex-existence assertion.

## Moving-boundary problem

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Moving-boundary_problem)

A moving-boundary problem determines both a field and part of the domain boundary on which that field is posed. An additional kinematic or conservation law determines the boundary motion.

## Diffusion equation

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)

[This section is present in another page, follow this link to view it.](diffusion-equation.md)

## Similarity solution

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)

A similarity solution combines independent variables into scale-invariant coordinates and reduces a PDE to an ODE.

### Similarity reduction

↑ **Parent:** [Similarity solution](#similarity-solution)

A reduction obtained by substituting a scale-invariant ansatz into a differential equation.

### Similarity ansatz

↑ **Parent:** [Similarity solution](#similarity-solution)

A similarity ansatz assumes a profile invariant under a prescribed rescaling, commonly in the displayed power-law form. Substitution into a [partial differential equation](partial-differential-equation.md) fixes compatible exponents and can reduce it to an [ordinary differential equation](differential-equation.md#ordinary-differential-equation) for $F$. Boundary conditions and conserved quantities must also be compatible with the scaling; the ansatz alone does not establish existence of a solution.

### Similarity profile

↑ **Parent:** [Similarity solution](#similarity-solution)

A [similarity profile](#similarity-profile) is the time-independent function left after expressing a evolving field in its scaled coordinate, for example $\rho(z,t)=\rho_0f(z/Z(t))$. Integrating such profiles converts a global [conservation law](physics.md#conservation-law) into an algebraic relation among the time-dependent scales.

## Separation of variables

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Separation_of_variables)

Separation of variables seeks a product of one-variable factors, reducing a PDE to ordinary differential equations.

### Separation constant

↑ **Parent:** [Separation of variables](#separation-of-variables)

A [separation constant](#separation-constant) arises when an equation is a sum of functions of independent variables. If $F(r)+G(\theta)=0$ on a product region, each function is constant, with opposite signs. Boundary or regularity conditions can then select discrete values, as for [scalar spheroidal harmonics](general-relativity.md#scalar-spheroidal-harmonic).

### Dirichlet problem on an annulus for one Fourier mode

↑ **Parent:** [Separation of variables](#separation-of-variables)

The harmonic function on $a<r<b$ with boundary values $u(a,\theta)=0$ and $u(b,\theta)=\cos(n\theta)$ is

$$
u(r,\theta)=
\frac{b^n(r^{2n}-a^{2n})}{r^n(b^{2n}-a^{2n})}
\cos(n\theta).
$$

## Polynomial ansatz

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polynomial_ansatz)

A polynomial ansatz determines an unknown polynomial solution by matching coefficients after applying the differential operator.

## Harmonic function

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Harmonic_function)

A harmonic function satisfies Laplace's equation $\Delta u=0$.

### Componentwise harmonic vector field

↑ **Parent:** [Harmonic function](#harmonic-function)

A vector field in Euclidean space is componentwise harmonic when each Cartesian component is a [harmonic function](#harmonic-function), equivalently its componentwise [Laplacian](calculus.md#laplacian) vanishes. Constant and linear vector fields are examples, as are constant linear combinations of derivatives of $1/r$ away from the origin in three dimensions. Such fields supply the vector potentials in the [Papkovich–Neuber representation](stokes-flow.md#papkovich-neuber-representation). Componentwise harmonicity does not by itself require zero divergence or zero curl.

### Harmonic odd reflection across a hyperplane

↑ **Parent:** [Harmonic function](#harmonic-function)

A [harmonic function](#harmonic-function) on one side of a hyperplane that is continuous up to an open portion of the hyperplane and zero there extends harmonically by odd reflection. One local proof takes a ball centered on the boundary and assigns odd continuous boundary data on its sphere. The [Poisson integral](#poisson-integral) on the ball is odd, so it vanishes on the equatorial disk. Uniqueness by the [maximum principle for harmonic functions](#maximum-principle-for-harmonic-functions) identifies it with the original function on the half-ball. Thus the odd extension is harmonic near each boundary point. A globally bounded zero-boundary harmonic function on a half-space is consequently zero by the [Liouville theorem for harmonic functions](#harmonic-liouville-theorem).

### Harmonic Hardy space of the upper half-space

↑ **Parent:** [Harmonic function](#harmonic-function)

For the upper half-space $H^{d+1}=\mathbb R^d\times(0,\infty)$, this is the space of [harmonic functions](#harmonic-function) with finite [norm](functional-analysis.md#norm) $\|u\|_{h^1}=\sup_{t>0}\int_{\mathbb R^d}|u(x,t)|\,dx$. It differs from an analytic [Hardy space](analysis.md#hardy-space): no [holomorphic function](complex-analysis.md#holomorphic-function) condition is imposed, and its boundary object can be a singular finite [Borel measure](measure-theory.md#borel-measure).

#### Poisson representation of harmonic h1 by finite measures

↑ **Parent:** [Harmonic Hardy space of the upper half-space](#harmonic-hardy-space-of-the-upper-half-space)

The [Poisson kernel for the upper half-space](#poisson-kernel-for-the-upper-half-space) gives an isometric bijection from finite real or complex [Borel measures](measure-theory.md#borel-measure), with their [total variation norm of a measure](measure-theory.md#total-variation-norm-of-a-measure), onto the [harmonic Hardy space of the upper half-space](#harmonic-hardy-space-of-the-upper-half-space). The kernel has unit mass, so [Tonelli theorem](measure-theory.md#tonelli-theorem) gives the upper norm bound. Its [approximate identity](fourier-analysis.md#approximate-identity) property gives weak-star convergence to the original measure and hence the reverse norm bound. For surjectivity, the [mean value property for harmonic functions](#mean-value-property-for-harmonic-functions) bounds each shifted harmonic function; bounded harmonic uniqueness gives $u(\cdot,s+t)=P_t*u(\cdot,s)$. A weak-star limit of the uniformly bounded measures $u(\cdot,s)\,dx$ then gives the required boundary measure. In particular $|u(x,t)|\leq c_dt^{-d}\|u\|_{h^1}$, where $c_d=\Gamma((d+1)/2)/\pi^{(d+1)/2}$.

### Gradient of a dipole potential

↑ **Parent:** [Harmonic function](#harmonic-function)

Away from the origin, a dipole potential $(d\cdot x)/|x|^3$ is [harmonic](#harmonic-function). Its [gradient](calculus.md#gradient) is angularly nonuniform, decays as $r^{-3}$, and has zero spherical mean because $\langle n\otimes n\rangle=I/3$. That cancellation distinguishes a self-dipole field from the regular incident field that excites a small inclusion.

### Kelvin transform

↑ **Parent:** [Harmonic function](#harmonic-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kelvin_transform)

In three-dimensional [Euclidean space](functional-analysis.md#euclidean-norm), spherical inversion together with the displayed weight maps [harmonic functions](#harmonic-function) to [harmonic functions](#harmonic-function) on the inverted domain. The [Laplacian](calculus.md#laplacian) satisfies $\Delta K_a u(\mathbf x)=(a/r)^5(\Delta u)(a^2\mathbf x/r^2)$. The formula is for $r>0$; a new singularity may occur at the origin.

#### Spherical inversion preserves angular derivatives

↑ **Parent:** [Kelvin transform](#kelvin-transform)

For $\overline{\mathbf r}=a^2\mathbf r/r^2$, the [chain rule](calculus.md#chain-rule) gives $\nabla_{\mathbf r}=(a^2/r^2)(I-2\widehat{\mathbf r}\widehat{\mathbf r}^{\,T})\nabla_{\overline{\mathbf r}}$. The radial term is killed by crossing with $\mathbf r$, giving the identity. Purely angular [vector spherical harmonics](analysis.md#vector-spherical-harmonic) are therefore unchanged as angular basis functions. This is distinct from pushing forward a physical vector field by the inversion Jacobian.

### Harmonic functions of Brownian motion

↑ **Parent:** [Harmonic function](#harmonic-function)

For a $C^2$ [harmonic function](#harmonic-function) $u$ and [Brownian motion](brownian-motion.md) stopped before leaving its domain, [Itô formula](stochastic-calculus.md#ito-s-lemma) gives $du(B_t)=\nabla u(B_t)\cdot dB_t+\frac12\Delta u(B_t)dt$. The drift vanishes. On a compact subdomain, the stopped process is a bounded [martingale](martingale.md). [Optional stopping theorem](martingale.md#optional-sampling-theorem-for-a-supermartingale) at an almost-surely finite exit time therefore gives the boundary mean formula. At the centre of a disk, [rotational invariance of planar Brownian motion](brownian-motion.md#rotational-invariance-of-planar-brownian-motion) makes the exit law uniform on the boundary circle. This proves the [mean value property for harmonic functions](#mean-value-property-for-harmonic-functions) probabilistically.

### Pluriharmonic function

↑ **Parent:** [Harmonic function](#harmonic-function)

A smooth real function on a [complex manifold](complex-geometry.md#complex-manifold) is pluriharmonic if $\partial\bar\partial f=0$. A complex-valued function satisfies the same equation exactly when both real and imaginary parts are pluriharmonic. Restrictions to complex coordinate lines are [harmonic functions](#harmonic-function). On a compact connected [complex manifold](complex-geometry.md#complex-manifold), choose a maximum of $|f|$ and apply the harmonic maximum principle successively along coordinate lines; the function is constant on a polydisc, then on the manifold by open-and-closed propagation. Without connectedness, constancy is componentwise.

### Compact convergence of locally bounded harmonic functions

↑ **Parent:** [Harmonic function](#harmonic-function)

A locally uniformly bounded sequence of [harmonic functions](#harmonic-function) with a pointwise limit converges uniformly on compact subsets, and its limit is harmonic. A radial [mollifier](distribution-theory.md#mollifier) of fixed local radius reproduces each harmonic function by the [mean value property for harmonic functions](#mean-value-property-for-harmonic-functions). Differentiating that convolution gives uniform interior gradient bounds, hence equicontinuity. A finite covering of a compact set converts pointwise convergence to uniform convergence. Passing to the limit in the radial convolution identity proves smoothness; passing to the limit against the Laplacian of each [test function](distribution-theory.md#test-function) proves harmonicity.

### Poisson integral on the unit disk

↑ **Parent:** [Harmonic function](#harmonic-function)

The disk [Poisson integral](#poisson-integral) is the [harmonic function](#harmonic-function) with boundary data $u$, given by

$$
P_r[u](t)=\int_{\mathbb T}\frac{1-r^2}{|e^{2\pi is}-re^{2\pi it}|^2}u(s)\,ds.
$$

It is the real part of the [Schwarz integral on the unit disk](#schwarz-integral-on-the-unit-disk) for real data. The nonnegative kernel has integral one; smooth boundary data extend smoothly to the circle. This disk formula should be distinguished from the half-plane formula.

#### Poisson integral converges nontangentially at Lebesgue points

↑ **Parent:** [Poisson integral on the unit disk](#poisson-integral-on-the-unit-disk)

For $F\in L^1(\partial\mathbb D)$ and a [Lebesgue point](measure-theory.md#lebesgue-point) $\xi_0$, its [Poisson integral](#poisson-integral) tends to $F(\xi_0)$ through every fixed [Stolz region](complex-analysis.md#stolz-region). If $\delta=1-|z|$, the [Poisson kernel](#poisson-kernel-for-the-upper-half-plane) there is at most $C_A\delta/(\delta^2+d(\xi,\xi_0)^2)$, where $d$ is shorter angular distance. Dyadic annuli about $\xi_0$ bound the near contribution by small local averages of $|F-F(\xi_0)|$ times a summable sequence $C_A2^{-k}$. The contribution outside a fixed small arc is $O(\delta)\|F-F(\xi_0)\|_1$ and vanishes. This is the local kernel argument underlying the [Fatou theorem for bounded holomorphic functions](analysis.md#fatou-theorem-for-bounded-holomorphic-functions).

#### Poisson kernel on the circle

↑ **Parent:** [Poisson integral on the unit disk](#poisson-integral-on-the-unit-disk)

For $0<r<1$, the [geometric series](real-analysis.md#geometric-series) gives $P_r(t)=1+2\sum_{n\ge1}r^n\cos nt$. Hence this positive even kernel has normalized integral one, and normalized [convolution](fourier-analysis.md#convolution) with it multiplies the $n$th [Fourier coefficient](fourier-series.md#fourier-coefficient) by $r^{|n|}$. Its mass outside any fixed neighbourhood of zero tends to zero as $r\uparrow1$. If an integrable function has finite one-sided limits $A,B$ at zero, evenness gives half the mass to each side and the convolution tends to $(A+B)/2$.

##### Uniform Poisson summability of continuous circle functions

↑ **Parent:** [Poisson kernel on the circle](#poisson-kernel-on-the-circle)

The [Poisson kernel on the circle](#poisson-kernel-on-the-circle) is nonnegative, has normalized integral one, and its mass outside any fixed arc about zero tends to zero as $r\uparrow1$. Split the convolution error into a short arc, controlled by the [modulus of continuity](topological-analysis.md#modulus-of-continuity), and its complement, controlled by the vanishing kernel mass. This proves [uniform convergence](real-analysis.md#uniform-convergence) for every continuous periodic function. Its Fourier multiplier is $r^{|n|}$, so the convolution is the Abel sum of the [Fourier series](fourier-series.md).

##### Conjugate Poisson kernel on the circle

↑ **Parent:** [Poisson kernel on the circle](#poisson-kernel-on-the-circle)

The [geometric series](real-analysis.md#geometric-series) gives $Q_r(t)=2\sum_{n\ge1}r^n\sin nt$. Its [convolution](fourier-analysis.md#convolution) multiplier is $-i\operatorname{sgn}(n)r^{|n|}$ for nonzero frequencies and zero at frequency zero. Since the series is uniformly absolutely convergent for $r<1$, these identities hold for every [Lebesgue integrable function](measure-theory.md#lebesgue-integrable-function) by termwise integration. If all negative [Fourier coefficients](fourier-series.md#fourier-coefficient) vanish, $Q_r*f=-i(P_r*f-\widehat f(0))$.

###### One-sided Fourier spectrum excludes jumps

↑ **Parent:** [Conjugate Poisson kernel on the circle](#conjugate-poisson-kernel-on-the-circle)

Let an integrable function have finite one-sided limits $A,B$ at zero. Oddness gives $(Q_r*f)(0)=(2\pi)^{-1}\int_0^\pi Q_r(t)[f(-t)-f(t)]\,dt$. Also $\int_0^\delta Q_r(t)\,dt=\log[(1-2r\cos\delta+r^2)/(1-r)^2]=2\log(1/(1-r))+O_\delta(1)$. Thus $(Q_r*f)(0)/\log(1/(1-r))\to(A-B)/\pi$: make the near-zero error in $f(-t)-f(t)$ arbitrarily small and bound the remaining integral uniformly. When negative [Fourier coefficients](fourier-series.md#fourier-coefficient) vanish, the conjugate-kernel identity makes this convolution bounded because $P_r*f$ tends to $(A+B)/2$. Therefore $A=B$. A [removable discontinuity](calculus.md#removable-discontinuity) caused solely by altering a point value is not excluded.

### Angular average of a logarithmic potential

↑ **Parent:** [Harmonic function](#harmonic-function)

For $r<1$, average the real part of the convergent power series for $\log(1+re^{i\theta})$: every nonconstant Fourier mode vanishes. For $r>1$, factor out $r$ and apply the same argument to $r^{-1}$. The boundary singularity at $r=1$ is logarithmically integrable. This identity computes the expected logarithmic distance after an isotropic Gaussian displacement.

### Vanishing harmonic function by level-set integration

↑ **Parent:** [Harmonic function](#harmonic-function)

For a smooth [harmonic function](#harmonic-function) on a manifold without boundary, assume its nonzero superlevel sets are compact. On a regular positive superlevel set $\{U>\varepsilon\}$, [integration by parts](calculus.md#integration-by-parts) gives $\int|\nabla U|^2=-\varepsilon\int_{\partial\{U>\varepsilon\}}|\nabla U|\leq0$. Applying the same argument to $-U$ proves $U=0$. This avoids assuming an unstated decay rate for the boundary flux at infinity.

### Weakly harmonic Sobolev function

↑ **Parent:** [Harmonic function](#harmonic-function)

An element $h\in H^1_{\mathrm{loc}}(U)$ is weakly harmonic on an [open set](topology.md#open-set) $U$ when $\int_U\nabla h\cdot\nabla\phi=0$ for every [test function](distribution-theory.md#test-function) $\phi\in C_c^\infty(U)$. This is the statement $\Delta h=0$ in [distributions](distribution-theory.md#distribution-mathematical-analysis). It requires no regularity of the [domain boundary](topology.md#boundary-of-a-domain). The [Weyl lemma](#weyl-lemma), a form of [elliptic regularity](distribution-theory.md#elliptic-regularity), identifies such an element with a [smooth](analysis.md#smooth-function) [harmonic function](#harmonic-function).

### Discrete harmonic function

↑ **Parent:** [Harmonic function](#harmonic-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Discrete_harmonic_function)

A real function $h$ on the [vertices of a graph](graph.md#vertex-graph-theory) of an unweighted [locally finite graph](graph-theory.md#locally-finite-graph) is a [discrete harmonic function](#discrete-harmonic-function) at $u$ when $\deg(u)h(u)=\sum_{v\sim u}h(v)$, equivalently $Lh(u)=0$ for the [Graph Laplacian](graph-theory.md#laplacian-matrix). For positive degree this says its value is the average over its [graph neighbours](graph-theory.md#neighbour-of-a-vertex); at an isolated [vertex of a graph](graph.md#vertex-graph-theory) the Laplacian condition is vacuous. On an [electrical network](markov-process.md#electrical-network) the corresponding equation uses conductance weights and the [Weighted graph Laplacian](graph-theory.md#weighted-graph-laplacian). [Voltages](markov-process.md#voltage) away from sources and sinks, and hitting [probabilities](probability-theory.md#probability) away from their prescribed boundaries, are [discrete harmonic functions](#discrete-harmonic-function).

#### Bounded harmonic function theorem on a recurrent graph

↑ **Parent:** [Discrete harmonic function](#discrete-harmonic-function)

Every bounded [harmonic function on a graph](#discrete-harmonic-function) is constant if the connected [locally finite graph](graph-theory.md#locally-finite-graph) is recurrent. Along its [random walk on a graph](markov-process.md#random-walk-on-a-graph), the harmonic values form a bounded [martingale](martingale.md) and converge almost surely. Recurrence visits each vertex infinitely often, making every vertex value a subsequential limit of the same convergent sequence. Thus every value agrees.

#### Harmonic maximum principle on a finite graph

↑ **Parent:** [Discrete harmonic function](#discrete-harmonic-function)

A real function $h$ on a finite [connected graph](graph.md#connected-graph) satisfying $Lh=0$ everywhere is constant. At a maximum [graph vertex](graph.md#vertex-graph-theory), the identity $\deg(u)h(u)=\sum_{v\sim u}h(v)$ forces every [graph neighbour](graph-theory.md#neighbour-of-a-vertex) to have the same maximum. Connectedness propagates it to every [graph vertex](graph.md#vertex-graph-theory). This proves uniqueness of [voltage](markov-process.md#voltage) up to an additive constant, and identifies sums of oppositely directed occupation [voltages](markov-process.md#voltage).

#### Bounded harmonic function theorem on the integer lattice

↑ **Parent:** [Discrete harmonic function](#discrete-harmonic-function)

Every bounded [discrete harmonic function](#discrete-harmonic-function) on $\mathbb Z^d$ is constant. After rescaling its range to $[0,1]$, place it in the compact convex set of all such functions; translation invariance and the mean-value identity force every extreme point to be constant, and the [Krein-Milman theorem](functional-analysis.md#krein-milman-theorem) finishes the proof.

### Removable singularity for a bounded harmonic function

↑ **Parent:** [Harmonic function](#harmonic-function)

A [harmonic function](#harmonic-function) on a punctured ball that is bounded near the missing point extends uniquely to a harmonic function on the whole ball. The extension can be defined by the [mean value property for harmonic functions](#mean-value-property-for-harmonic-functions); interior estimates then give smoothness across the point.

### Harmonic replacement

↑ **Parent:** [Harmonic function](#harmonic-function)

The harmonic replacement of $u$ in a domain $D$ is the [harmonic function](#harmonic-function) $w$ having the same boundary trace as $u$. Thus $u-w\in H_0^1(D)$, and subtracting the weak equations permits local energy estimates for the error $u-w$.

### Mean value property for harmonic functions

↑ **Parent:** [Harmonic function](#harmonic-function)

For every closed ball contained in the domain of a harmonic function, the value at its centre equals both its average over the ball and its average over the boundary sphere.

#### Harnack inequality for harmonic functions

↑ **Parent:** [Mean value property for harmonic functions](#mean-value-property-for-harmonic-functions)

If $u\geq0$ is a [harmonic function](#harmonic-function) on a neighbourhood of $\overline{B_{4r}(y)}$, then

$$
\sup_{B_r(y)}u\leq3^n\inf_{B_r(y)}u.
$$

For $x,z\in B_r(y)$, use $B_r(x)\subset B_{3r}(z)\subset B_{4r}(y)$ and the [mean value property for harmonic functions](#mean-value-property-for-harmonic-functions). Nonnegativity lets us enlarge the integral, and the ratio of volumes is $3^n$. This compares values without requiring derivative bounds.

##### Harnack inequality on the unit disk

↑ **Parent:** [Harnack inequality for harmonic functions](#harnack-inequality-for-harmonic-functions)

For a nonnegative [harmonic function](#harmonic-function) on the [unit disc](topology.md#unit-disc), the displayed inequalities are sharp. Apply the [Poisson integral on the unit disk](#poisson-integral-on-the-unit-disk) on radius $R>|z|$, bound its positive kernel between $(R-|z|)/(R+|z|)$ and its reciprocal, and use the [mean value property for harmonic functions](#mean-value-property-for-harmonic-functions). Letting $R\uparrow1$ proves the assertion. Positive [Poisson kernels](#poisson-kernel-for-the-upper-half-plane) with one boundary pole give equality in the appropriate radial directions.

###### Sharp gradient bound for positive harmonic functions

↑ **Parent:** [Harnack inequality on the unit disk](#harnack-inequality-on-the-unit-disk)

For a positive [harmonic function](#harmonic-function) on the [unit disc](topology.md#unit-disc), choose a global [harmonic conjugate](#harmonic-conjugate) and apply the [Carathéodory derivative bound for the right half-plane](analysis.md#caratheodory-derivative-bound-for-the-right-half-plane) to $u+iv$. This gives $|\nabla u(0)|\le2u(0)$ by the [Cauchy-Riemann equations](analysis.md#cauchy-riemann-equations). A [disk automorphism](topology.md#automorphism-of-the-unit-disk) sending zero to $z$ has derivative modulus $1-|z|^2$, so the [chain rule](calculus.md#chain-rule) gives the displayed bound. Composing a boundary-pole [Poisson kernel](#poisson-kernel-for-the-upper-half-plane) with a [disk automorphism](topology.md#automorphism-of-the-unit-disk) attains equality, proving the coefficient is optimal at every point.

#### Local converse to the mean value property

↑ **Parent:** [Mean value property for harmonic functions](#mean-value-property-for-harmonic-functions)

If a continuous function has the spherical mean value property at every point for some sequence of radii decreasing to zero, then it is harmonic. Comparison on each relatively compact ball with the harmonic function having the same boundary data proves the result by propagating any hypothetical interior extremum along one of the admissible spheres.

### Weyl lemma

↑ **Parent:** [Harmonic function](#harmonic-function)

The Weyl lemma says that every locally integrable distributional solution of $\Delta u=0$ agrees almost everywhere with a smooth harmonic function. Convolution with a [mollifier](distribution-theory.md#mollifier) and the harmonic mean value property provide a standard proof.

### Interior derivative estimate for a harmonic function

↑ **Parent:** [Harmonic function](#harmonic-function)

If $u$ is harmonic on $B_r(x_0)$, then for every integer $m\geq1$,

$$
|D^mu(x_0)|\leq C(n,m)r^{-m}\sup_{B_r(x_0)}|u|.
$$

The first-order estimate follows by differentiating the ball mean-value formula and applying the divergence theorem; iteration gives higher orders.

### Polynomial-growth Liouville theorem for harmonic functions

↑ **Parent:** [Harmonic function](#harmonic-function)

If an entire harmonic function on $\mathbb R^n$ grows like $O(1+|x|^{k+\alpha})$ with $k\in\mathbb N$ and $0<\alpha<1$, then it is a harmonic polynomial of degree at most $k$. Apply the interior derivative estimate of order $k+1$ on expanding balls.

<h4 id="liouville-lemma-for-globally-holder-harmonic-functions">Liouville lemma for globally Hölder harmonic functions</h4>

↑ **Parent:** [Polynomial-growth Liouville theorem for harmonic functions](#polynomial-growth-liouville-theorem-for-harmonic-functions)

A [harmonic function](#harmonic-function) on all of $\mathbb R^n$ with a finite global [Hölder seminorm](sobolev-space.md#holder-seminorm) of exponent $0<\mu<1$ is constant. Indeed $|w(x)-w(0)|\leq C|x|^\mu$, and the [interior derivative estimate for a harmonic function](#interior-derivative-estimate-for-a-harmonic-function) on balls of radius $R$ bounds $|\nabla w(0)|$ by $CR^{\mu-1}$. Letting $R\to\infty$ makes this [gradient](calculus.md#gradient) zero, and translating the centre proves the assertion everywhere.

### Harmonic function as the real part of a holomorphic function

↑ **Parent:** [Harmonic function](#harmonic-function)

A real-valued function $u$ on a [simply connected domain](complex-analysis.md#simply-connected-domain) is [harmonic](#harmonic-function) exactly when

$$
u=\operatorname{Re}f
$$

for some [holomorphic function](complex-analysis.md#holomorphic-function) $f$. One construction observes that $u_x-iu_y$ is holomorphic and takes its [holomorphic primitive](complex-analysis.md#primitive-of-a-holomorphic-function-on-a-simply-connected-domain).

### Subharmonic function

↑ **Parent:** [Harmonic function](#harmonic-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Subharmonic_function)

A twice differentiable function is strictly subharmonic where $\Delta u>0$. It cannot have an interior local maximum because the Hessian at such a maximum is negative semidefinite.

#### Modulus powers of holomorphic functions are subharmonic

↑ **Parent:** [Subharmonic function](#subharmonic-function)

For every [holomorphic function](complex-analysis.md#holomorphic-function) and $p>0$, $|f|^p$ is [subharmonic](#subharmonic-function). Away from its zeros the displayed [Laplacian](calculus.md#laplacian) calculation proves this. At the zeros, use the smooth approximations $(|f|^2+\varepsilon)^{p/2}$, whose [Laplacians](calculus.md#laplacian) are nonnegative, and let $\varepsilon\downarrow0$ in their mean inequalities. This permits [Poisson integral](#poisson-integral) comparison for fractional modulus powers even when a global analytic fractional power does not exist.

#### Laplacian identity for the squared modulus of a holomorphic function

↑ **Parent:** [Subharmonic function](#subharmonic-function)

Write a [holomorphic function](complex-analysis.md#holomorphic-function) as $f=u+iv$. The [Cauchy-Riemann equations](analysis.md#cauchy-riemann-equations) make $u,v$ [harmonic functions](#harmonic-function) and give $u_x=v_y$, $u_y=-v_x$. The [product rule](calculus.md#product-rule) therefore gives $\Delta(u^2+v^2)=2(|\nabla u|^2+|\nabla v|^2)=4|f'|^2$. Thus its squared [modulus](complex-analysis.md#modulus) is [subharmonic](#subharmonic-function) and is harmonic only where $f'$ vanishes.

#### Harmonic majorant

↑ **Parent:** [Subharmonic function](#subharmonic-function)

A harmonic majorant of a real function $u$ is a real [harmonic function](#harmonic-function) $h$ with $h\geq u$ pointwise. A least harmonic majorant lies below every other harmonic majorant. A continuous [subharmonic function](#subharmonic-function) need not have one: $u(z)=(1-|z|^2)^{-1}$ on the [unit disk](geometry-and-topology.md#unit-disk) has increasing circular means diverging to infinity, whereas any harmonic majorant would have the same finite mean on every centered circle.

##### Least harmonic majorant by expanding disk lifts

↑ **Parent:** [Harmonic majorant](#harmonic-majorant)

For continuous [subharmonic function](#subharmonic-function) $u$ on the [unit disk](geometry-and-topology.md#unit-disk), let $H_r$ be the [Poisson integral](#poisson-integral) of its values on $|z|=r$, evaluated inside that disk. Harmonic comparison gives $H_s\geq H_r\geq u$ for $|z|<r<s<1$. The [Harnack inequality for harmonic functions](#harnack-inequality-for-harmonic-functions) makes their limit either finite and harmonic everywhere or everywhere infinite. In the finite case every [harmonic majorant](#harmonic-majorant) dominates every $H_r$, so their limit is the least harmonic majorant. The supremum must restrict $r>|z|$; the Poisson expression evaluated outside its circle does not have this interpretation.

#### Harmonic lifting of a continuous subharmonic function

↑ **Parent:** [Subharmonic function](#subharmonic-function)

On a relatively compact coordinate disk $V$ in a [Riemann surface](complex-analysis.md#riemann-surfaces), replace a continuous [subharmonic function](#subharmonic-function) $u$ inside $V$ by the [Poisson integral](#poisson-integral) of its boundary values, leaving it unchanged outside. The resulting function $L_Vu$ is continuous and subharmonic, equals $u$ off $V$, is harmonic on $V$, and satisfies $L_Vu\geq u$. The [maximum principle for subharmonic functions](#maximum-principle-for-subharmonic-functions) proves the inequality. The pasting assertion follows from harmonic comparison: a harmonic comparison function dominating the pasted function on the boundary of a test domain first dominates $u$, then dominates the disk lift on its part inside $V$.

#### Locally integrable supremum theorem for subharmonic functions

↑ **Parent:** [Subharmonic function](#subharmonic-function)

For a countable family of [subharmonic functions](#subharmonic-function), a [locally integrable](distribution-theory.md#locally-integrable-function) pointwise supremum is subharmonic in the [distributional derivative](distribution-theory.md#distributional-derivative) sense. Finite maxima preserve subharmonicity: approximate the maximum by the smooth convex coordinatewise increasing function $(s+t+\sqrt{(s-t)^2+\delta^2})/2$, apply the [chain rule](calculus.md#chain-rule) after mollification, then pass to a local [L1 norm](functional-analysis.md#l1-norm) convergence limit. The maxima $g_N=\max(f_1,\ldots,f_N)$ increase to $g$ and are bounded in absolute value by $|f_1|+|g|$ on compact sets, so the [dominated convergence theorem](measure-theory.md#dominated-convergence-theorem) completes the proof. The hypothesis cannot be omitted: $f_j=j$ has infinite supremum. To obtain a pointwise [subharmonic function](#subharmonic-function), take the [canonical representative of a subharmonic distribution](#canonical-representative-of-a-subharmonic-distribution).

#### Superharmonic function

↑ **Parent:** [Subharmonic function](#subharmonic-function)

A locally integrable real function is superharmonic in the distributional sense if its [Laplacian](calculus.md#laplacian) is nonpositive on every nonnegative [test function](distribution-theory.md#test-function). Equivalently its negative is a [subharmonic function](#subharmonic-function). The canonical lower semicontinuous representative satisfies the reverse ball mean inequality. A function both subharmonic and superharmonic has zero distributional Laplacian and a smooth [harmonic function](#harmonic-function) representative by the [Weyl lemma](#weyl-lemma).

#### Canonical representative of a subharmonic distribution

↑ **Parent:** [Subharmonic function](#subharmonic-function)

For locally integrable real $u$ with nonnegative [distributional derivative](distribution-theory.md#distributional-derivative) $\Delta u$, its ball means increase with radius. To see this, mollify: for a smooth subharmonic function the derivative of its spherical mean is the integral of $\Delta u$ over the ball divided by the sphere area. The ball means inherit monotonicity; local $L^1$ convergence passes this to $u$. Their decreasing-radius limit exists, may be minus infinity at exceptional points, and equals $u$ almost everywhere by the [Lebesgue differentiation theorem](measure-theory.md#lebesgue-differentiation-theorem). It is upper semicontinuous as an infimum of continuous ball means and satisfies the mean-value inequality. Arbitrary changes of a representative on a null set can destroy its pointwise maximum principle.

#### Maximum principle for subharmonic functions

↑ **Parent:** [Subharmonic function](#subharmonic-function)

A continuous [subharmonic function](#subharmonic-function) on the closure of a bounded domain attains its maximum on the boundary. If it is twice differentiable, the strict condition $\Delta u>0$ rules out an interior maximum immediately because the [Hessian matrix](calculus.md#hessian-matrix) there would be negative semidefinite.

##### Strong maximum principle for subharmonic functions

↑ **Parent:** [Maximum principle for subharmonic functions](#maximum-principle-for-subharmonic-functions)

If the [canonical representative of a subharmonic distribution](#canonical-representative-of-a-subharmonic-distribution) on a connected domain attains a finite global maximum at an interior point, it is constant. The ball mean inequality forces equality almost everywhere on a small ball around the maximum. The canonical representative then equals the maximum everywhere on that ball. The maximum set is open by this argument and closed by upper semicontinuity; [connectedness](geometry-and-topology.md#connected-space) makes it the whole domain.

##### Gradient maximum principle for harmonic functions

↑ **Parent:** [Maximum principle for subharmonic functions](#maximum-principle-for-subharmonic-functions)

For a [harmonic function](#harmonic-function) $w$ smooth inside a bounded domain and $C^1$ on its closure, $\Delta|Dw|^2=2|D^2w|^2\geq0$. The [weak maximum principle for elliptic operators](elliptic-boundary-value-problem.md#weak-maximum-principle-for-elliptic-operators) and continuity of the [gradient](calculus.md#gradient) imply $\sup_\Omega|Dw|=\sup_{\partial\Omega}|Dw|$.

### Harmonic Liouville theorem

↑ **Parent:** [Harmonic function](#harmonic-function)

A bounded [harmonic function](#harmonic-function) on the [complex plane](complex-analysis.md#complex-plane) is constant. More generally, an entire harmonic function bounded on either side is constant: write it as $\operatorname{Re}f$ by [harmonic function as the real part of a holomorphic function](#harmonic-function-as-the-real-part-of-a-holomorphic-function), then apply the [Liouville theorem](complex-analysis.md#liouville-theorem) to $e^f$ or $e^{-f}$.

#### Gaussian heat-kernel proof of the harmonic Liouville theorem

↑ **Parent:** [Harmonic Liouville theorem](#harmonic-liouville-theorem)

A bounded entire [harmonic function](#harmonic-function) satisfies $u(x)=\mathbb E_xu(B_t)$ because $u(B)$ is a bounded [local martingale](martingale.md#local-martingale). The [Gaussian heat kernel](diffusion-equation.md#gaussian-heat-kernel) has a directional derivative with $L^1$ norm $\sqrt{2/\pi}/\sqrt t$. Consequently $|u(x)-u(y)|\leq\|u\|_\infty\sqrt{2/\pi}|x-y|/\sqrt t$; letting $t\to\infty$ proves the [harmonic Liouville theorem](#harmonic-liouville-theorem) in every dimension.

#### One-sided bounded harmonic functions on the punctured plane are constant

↑ **Parent:** [Harmonic Liouville theorem](#harmonic-liouville-theorem)

A [harmonic function](#harmonic-function) on $\mathbb R^2\setminus\{0\}$ bounded on one side is constant. Shift and change sign to make it nonnegative. Its circular mean has the form $a\log r+b$; positivity for every $r>0$ forces $a=0$. For $|x|=r$, the [mean value property for harmonic functions](#mean-value-property-for-harmonic-functions) bounds its value by the mean integral over $r/2<|z|<3r/2$, giving at most $8b$. A [removable singularity for a bounded harmonic function](#removable-singularity-for-a-bounded-harmonic-function) fills the origin, and the [harmonic Liouville theorem](#harmonic-liouville-theorem) finishes the proof. The dimensional distinction matters: $|x|^{2-n}$ is a positive nonconstant [harmonic function](#harmonic-function) on punctured $\mathbb R^n$ for $n\geq3$.

#### Brownian coupling proof of the harmonic Liouville theorem

↑ **Parent:** [Harmonic Liouville theorem](#harmonic-liouville-theorem)

For a bounded harmonic function $f$ on $\mathbb R^d$, the processes $f(B_t^x)$ and $f(B_t^y)$ are bounded martingales. Couple the Brownian motions from $x$ and $y$ so that they coalesce in finite time almost surely. Then

$$
|f(x)-f(y)|
\leq2\lVert f\rVert_\infty\mathbb P(T>t)
\longrightarrow0,
$$

which proves that $f$ is constant in every dimension.

#### Surjectivity of a nonconstant entire harmonic function

↑ **Parent:** [Harmonic Liouville theorem](#harmonic-liouville-theorem)

Every nonconstant harmonic function $u:\mathbb C\to\mathbb R$ is unbounded above and below by the [harmonic Liouville theorem](#harmonic-liouville-theorem). The [intermediate value theorem](calculus.md#intermediate-value-theorem) then gives $u(\mathbb C)=\mathbb R$.

### Scale-periodic harmonic function from an elliptic function

↑ **Parent:** [Harmonic function](#harmonic-function)

Let $\wp_\Lambda$ be the [Weierstrass elliptic function](complex-analysis.md#weierstrass-elliptic-function) for

$$
\Lambda=(\log q)\mathbb Z+2\pi i\mathbb Z,
\qquad q>1.
$$

Because $2\pi i$ is a [period](complex-analysis.md#period-lattice), the formula

$$
u(z)=\operatorname{Re}\wp_\Lambda(\log z)
$$

is independent of the branch of the [complex logarithm](analysis.md#complex-logarithm). It is a nonconstant harmonic function on

$$
\mathbb C^*\setminus\{q^m:m\in\mathbb Z\}
$$

and its other period gives $u(qz)=u(z)$.

### Harmonic polynomial

↑ **Parent:** [Harmonic function](#harmonic-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Harmonic_polynomial)

A harmonic polynomial is a polynomial annihilated by the Laplacian.

#### Harmonic decomposition of homogeneous polynomials

↑ **Parent:** [Harmonic polynomial](#harmonic-polynomial)

If $\mathcal P_\ell$ is the space of degree-$\ell$ [homogeneous polynomials](algebra.md#homogeneous-polynomial) and $\mathcal H_\ell$ its [harmonic polynomials](#harmonic-polynomial), then $\mathcal P_\ell=\mathcal H_\ell\oplus|x|^2\mathcal P_{\ell-2}$. Under the [Fischer inner product](linear-algebra.md#fischer-inner-product), the second summand is orthogonal to the kernel of the [Laplacian](calculus.md#laplacian). Iteration expresses every polynomial restricted to the unit [sphere](geometry-and-topology.md#sphere) as a sum of [spherical harmonics](analysis.md#spherical-harmonic).

### Harmonic conjugate

↑ **Parent:** [Harmonic function](#harmonic-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Harmonic_conjugate)

A harmonic conjugate v makes u+iv holomorphic; it exists globally on simply connected domains.

#### Global harmonic conjugate criterion by vanishing periods

↑ **Parent:** [Harmonic conjugate](#harmonic-conjugate)

For a [harmonic function](#harmonic-function) $u$, the function $g=u_x-iu_y$ is holomorphic. It is the [derivative](calculus.md#derivative) of a single-valued [holomorphic function](complex-analysis.md#holomorphic-function) exactly when its integrals around all closed curves vanish. A primitive then has [real part](complex-analysis.md#real-part) $u$ after adjusting a real constant. [Simply connected](algebraic-topology.md#simply-connected-space) domains satisfy this condition; on an [annulus](topology.md#annulus-mathematics) $u=\log|z|$ fails because the [derivative](calculus.md#derivative) has period $2\pi i$.

##### Logarithmic cancellation on an exterior annulus

↑ **Parent:** [Global harmonic conjugate criterion by vanishing periods](#global-harmonic-conjugate-criterion-by-vanishing-periods)

For $|z|>1$, both logarithms in the display can use their [principal logarithms](analysis.md#principal-complex-logarithm). The [real part](complex-analysis.md#real-part) is $\log(|z+1|^2/|z-1|^2)$ and the [derivative](calculus.md#derivative) is $2/(z+1)-2/(z-1)$. The two [residues](analysis.md#residue) cancel on a loop surrounding both points. Equivalently $f=4\sum_{m\ge0}z^{-(2m+1)}/(2m+1)$ is globally single-valued outside the unit [circle](topology.md#circle), although individual logarithms of $z+1$ and $z-1$ are not.

// Destination: complex-dynamics.bigb

#### Composition of harmonic conjugate pairs

↑ **Parent:** [Harmonic conjugate](#harmonic-conjugate)

If $u+iv$ and $p+iq$ are [holomorphic functions](complex-analysis.md#holomorphic-function), with the image of the first inside the domain of the second, then $p(u,v)+iq(u,v)$ is holomorphic by the [chain rule](calculus.md#chain-rule). Directly, their [Cauchy-Riemann equations](analysis.md#cauchy-riemann-equations) imply $[p(u,v)]_x=[q(u,v)]_y$ and $[p(u,v)]_y=-[q(u,v)]_x$. Differentiating these relations proves harmonicity of both parts. No nonvanishing derivative hypothesis is required.

#### Harmonic angle and logarithmic radius

↑ **Parent:** [Harmonic conjugate](#harmonic-conjugate)

On a domain carrying a [branch of the complex logarithm](analysis.md#branch-of-the-complex-logarithm), the [holomorphic function](complex-analysis.md#holomorphic-function) $-i\operatorname{Log}z$ has real part equal to the chosen angle and imaginary part $-\log|z|$. These are [harmonic conjugates](#harmonic-conjugate); their [level sets](topology.md#level-set) are rays and circles, meeting orthogonally. For the principal real arctangent $\phi=\arctan(y/x)$, its domain has the two components $x>0$ and $x<0$. The corresponding [holomorphic functions](complex-analysis.md#holomorphic-function) are $-i\operatorname{Log}z$ and $-i\operatorname{Log}(-z)$, using the [complex logarithm](analysis.md#complex-logarithm) on the right half-plane. This formulation does not assert a globally single-valued angle on the punctured plane.

#### Local harmonic conjugate

↑ **Parent:** [Harmonic conjugate](#harmonic-conjugate)

On a disc, the closed one-form $-u_y\,dx+u_x\,dy$ has a potential $v$ when $\Delta u=0$. The Cauchy--Riemann equations then make $u+iv$ holomorphic.

#### Log modulus has no global harmonic conjugate on the punctured plane

↑ **Parent:** [Harmonic conjugate](#harmonic-conjugate)

The function $\log|z|$ is [harmonic](#harmonic-function) on the [punctured complex plane](complex-analysis.md#punctured-complex-plane), but it is not globally the real part of a [holomorphic function](complex-analysis.md#holomorphic-function) there. Such a function would have derivative $1/z$, whose integral around the unit circle is $2\pi i$, whereas the integral of a derivative around a closed curve is zero.

### Harmonic functions are smooth

↑ **Parent:** [Harmonic function](#harmonic-function)

Every $C^2$ harmonic function is locally the real part of a holomorphic function and is therefore infinitely differentiable.

### Harmonic functions are real analytic

↑ **Parent:** [Harmonic function](#harmonic-function)

Harmonic functions admit locally convergent power-series expansions.

#### Unique continuation for harmonic functions

↑ **Parent:** [Harmonic functions are real analytic](#harmonic-functions-are-real-analytic)

A harmonic function on a connected domain that vanishes on a nonempty open subset vanishes everywhere.

## Smooth bump function

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)

A smooth bump function is a smooth function with compact support. The flat exponential construction gives bumps supported in prescribed balls.

### Disjoint-support zero-product construction

↑ **Parent:** [Smooth bump function](#smooth-bump-function)

Two nonzero functions with disjoint supports have identically zero pointwise product. Separated continuous tent functions or smooth bumps provide examples.

## Laplace operator

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Laplace_operator)

The Laplace operator is the divergence of the gradient, $\Delta=\nabla\cdot\nabla$.

### Neumann Laplacian

↑ **Parent:** [Laplace operator](#laplace-operator)

The nonnegative Neumann Laplacian is the [self-adjoint](linear-operator-theory.md#self-adjoint-operator) realization of $-\operatorname{div}\operatorname{grad}$ with vanishing outward [normal derivative](differential-geometry.md#normal-derivative). Its weak quadratic form is the [Dirichlet energy](differential-geometry.md#dirichlet-energy) on $H^1$. On a connected compact domain the constants give a one-dimensional zero [eigenvalue](linear-operator-theory.md#eigenvalue) space.

### Dirichlet Laplacian

↑ **Parent:** [Laplace operator](#laplace-operator)

The nonnegative Dirichlet Laplacian is the [self-adjoint](linear-operator-theory.md#self-adjoint-operator) realization of $-\operatorname{div}\operatorname{grad}$ with zero boundary values. On a bounded domain, its weak form is the [Dirichlet energy](differential-geometry.md#dirichlet-energy) on $H_0^1$. For polygonal domains the weak operator domain is preferable to a requirement of smoothness at corners.

#### Dirichlet resonance in an equilateral triangle

↑ **Parent:** [Dirichlet Laplacian](#dirichlet-laplacian)

If $\beta_1,\beta_2,\beta_3$ are the affine barycentric coordinates of an [equilateral triangle](geometry-and-topology.md#equilateral-triangle) of side $\ell$, then $h=\prod_j\sin(\pi\beta_j)=\frac14\sum_j\sin(2\pi\beta_j)$ vanishes on the boundary and satisfies $\Delta h=-16\pi^2h/(3\ell^2)$. Thus the problem $\Delta q-4\lambda q=0$ with zero [Dirichlet boundary data](differential-equation.md#dirichlet-boundary-data) has distinct solutions zero and $h$ at the displayed negative parameter. Their normal traces differ, demonstrating failure of a uniquely determined [Dirichlet-to-Neumann map](differential-equation.md#dirichlet-to-neumann-map) at resonance.

#### Fractional Dirichlet domain scale

↑ **Parent:** [Dirichlet Laplacian](#dirichlet-laplacian)

For the positive [Dirichlet Laplacian](#dirichlet-laplacian) $A$ on a bounded smooth domain, with normalized [eigenfunctions](linear-operator-theory.md#eigenfunction) $e_j$ and positive [eigenvalues](linear-operator-theory.md#eigenvalue) $\mu_j$, define $A^\alpha u=\sum_j\mu_j^\alpha(u,e_j)e_j$ on the vectors for which $\sum_j\mu_j^{2\alpha}|(u,e_j)|^2<\infty$. The resulting [Hilbert space](hilbert-space.md) embeds in the [Sobolev space](sobolev-space.md) $H^{2\alpha}$, with the boundary conditions appropriate to the exponent. In particular $H_\alpha$ embeds in $C^{0,\beta}$ whenever $0<\beta<\min(1,2\alpha-n/2)$. High powers impose further boundary compatibility; ordinary smoothness alone does not imply membership in every fractional domain.

### Polar-coordinate Laplacian identity

↑ **Parent:** [Laplace operator](#laplace-operator)

In $\mathbb R^{d+1}$, $g=dr^2+r^2g_{S^d}$ and the volume density is $r^d$. With the nonnegative [Laplacian](calculus.md#laplacian) convention, $\widetilde\Delta=-\partial_r^2-(d/r)\partial_r+r^{-2}\Delta_{S^d}$. The identity separates radial homogeneity from the angular [Laplace-Beltrami operator](differential-geometry.md#laplace-beltrami-operator) and derives the [spectrum of the Laplacian on a sphere](riemannian-geometry.md#spectrum-of-the-laplacian-on-a-sphere).

### Rotational commutator for the Laplacian

↑ **Parent:** [Laplace operator](#laplace-operator)

The infinitesimal rotation $R_{ij}=x_i\partial_j-x_j\partial_i$ commutes with the [Laplacian](calculus.md#laplacian): the extra terms $2\partial_i\partial_j$ cancel. It is tangent to every sphere, so it preserves zero Dirichlet traces on spherical shells. If $\Delta u=f$ and $f$ is radial, uniqueness applied to $R_{ij}u$ forces all these rotation [derivatives](calculus.md#derivative) to vanish, hence $u$ is radial.

### Laplace equation

↑ **Parent:** [Laplace operator](#laplace-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Laplace_equation)

Laplace's equation is

$$
\Delta u=0.
$$

Its solutions are [harmonic functions](#harmonic-function).

#### Harmonic Fourier expansions in planar concentric domains

↑ **Parent:** [Laplace equation](#laplace-equation)

A single-valued [harmonic function](#harmonic-function) in a planar [annulus](topology.md#annulus-mathematics) has radial [Fourier modes](fourier-analysis.md#fourier-mode) $1,\log r$ and $r^n,r^{-n}$ multiplying $\cos(n\theta),\sin(n\theta)$ for integers $n\ge1$. Substitute $R(r)\Theta(\theta)$ in [Laplace's equation](#laplace-equation): periodicity gives $\Theta''+n^2\Theta=0$, while $r^2R''+rR'-n^2R=0$. Regularity at the origin excludes $\log r,r^{-n}$; boundedness at infinity excludes $\log r,r^n$. Coefficients must give locally convergent [series](real-analysis.md#series-mathematics), with the boundary regularity required by the particular [Dirichlet problem](analysis.md#dirichlet-problem). Mere finiteness at each finite exterior point does not imply boundedness at infinity.

#### Separated Laplace mode with a Robin edge

↑ **Parent:** [Laplace equation](#laplace-equation)

For $0<x<L$, $0<y<H$, choose $k=m\pi/H>0$ and seek a [harmonic function](#harmonic-function) with zero values on the horizontal edges, boundary value $\sin(ky)$ at $x=L$, and $\phi+\alpha\partial_n\phi=0$ at $x=0$, with constant $\alpha\ge0$. [Separation of variables](#separation-of-variables) gives $\phi=[\alpha k\cosh(kx)+\sinh(kx)]\sin(ky)/[\alpha k\cosh(kL)+\sinh(kL)]$. The outward derivative at the left edge is $-\partial_x$, giving $F(0)-\alpha F'(0)=0$. The denominator is positive and [Poisson uniqueness with a nonnegative Robin normal coefficient](differential-equation.md#poisson-uniqueness-with-a-nonnegative-robin-normal-coefficient) proves uniqueness in the regular solution class.

#### Spherical harmonic matching with a derivative jump

↑ **Parent:** [Laplace equation](#laplace-equation)

For a regular interior and a decaying exterior harmonic potential with continuous values on the unit sphere, the same coefficient multiplies the two radial branches of each [Legendre polynomial](differential-equation.md#legendre-polynomial) mode. Its exterior-minus-interior radial derivative is $-(2n+1)a_nP_n$. Thus an axisymmetric prescribed jump $j_nP_n(\cos\theta)$ produces coefficient $a_n=-j_n/(2n+1)$. This diagonal matching rule reduces a spherical interface problem to its angular-mode coefficients.

#### Fourier solution of the strip Dirichlet problem

↑ **Parent:** [Laplace equation](#laplace-equation)

For the [Laplace equation](#laplace-equation) on $0<y<1$, prescribe bottom data $g$ and zero top data. A horizontal [Fourier transform](analysis.md#fourier-transform) reduces the equation to $\widehat u_{yy}-s^2\widehat u=0$, giving the displayed multiplier and its limit $1-y$ at $s=0$. Integrable transformed data give a bounded inverse-transform solution. The bounded solution is unique by the [maximum principle for harmonic functions](#maximum-principle-for-harmonic-functions), using barriers $\varepsilon\cosh(\delta x)\cos(\delta(y-1/2))$ for $0<\delta<\pi$ on expanding rectangles. Without a growth condition, one can add $e^{\pi x}\sin(\pi y)$, so the two boundary traces alone do not determine an arbitrary harmonic function on an infinite strip.

#### Harmonic matching across a circle with a derivative jump

↑ **Parent:** [Laplace equation](#laplace-equation)

For a single-valued [harmonic function](#harmonic-function) tending to zero both at the origin and at infinity, match an angular [Fourier series](fourier-series.md) across the unit circle. A nonzero mode with continuous interface value $K_n\cos(n\theta)$ has interior field $K_nr^n\cos(n\theta)$ and exterior field $K_nr^{-n}\cos(n\theta)$. Its exterior-minus-interior radial [derivative](calculus.md#derivative) is $-2nK_n\cos(n\theta)$. Thus a prescribed jump coefficient $j_n$ determines $K_n=-j_n/(2n)$. Sine modes obey the same relation. The constant mode must have zero jump under these decay conditions.

#### Zero-boundary harmonic function with pointwise vertical decay

↑ **Parent:** [Laplace equation](#laplace-equation)

The imaginary part of the entire function $e^{z^2}$ is a [harmonic function](#harmonic-function). On the upper half-plane it vanishes at $y=0$ and tends to zero as $y\to\infty$ for every fixed $x$, but is nonzero and grows rapidly in the horizontal direction. Adding it to a [Poisson integral](#poisson-integral) preserves those boundary and vertical-decay conditions. A boundedness or suitable transform-growth condition is therefore needed to make the half-plane [Dirichlet problem](analysis.md#dirichlet-problem) unique.

#### Exterior harmonic potential with no flux through a sphere

↑ **Parent:** [Laplace equation](#laplace-equation)

An axisymmetric harmonic potential outside a sphere of radius $r_0$, with far field $v_0r\cos\theta$ and zero radial derivative on the sphere, is

$$
U=v_0(r+r_0^3/(2r^2))\cos\theta.
$$

The regular spherical expansion in [Legendre polynomials](differential-equation.md#legendre-polynomial) fixes all coefficients. A spatial constant remains arbitrary if only the far-field gradient is specified, and is fixed by prescribing the potential difference at infinity.

#### Green function of the Laplacian

↑ **Parent:** [Laplace equation](#laplace-equation)

In three dimensions,

$$
-\nabla^2\frac1{4\pi|x-x'|}=\delta^{(3)}(x-x').
$$

Consequently the decaying solution of $-\nabla^2u=f$ in free space is

$$
u(x)=\frac1{4\pi}\int_{\mathbb R^3}\frac{f(x')}{|x-x'|}\,d^3x'.
$$

This is the free-space [Green function](analysis.md#green-s-function) for the negative [Laplace operator](#laplace-operator).

##### Point-source potential with one compact spatial dimension

↑ **Parent:** [Green function of the Laplacian](#green-function-of-the-laplacian)

For three noncompact spatial coordinates of radius $r$ and a circle of circumference $L$, the positive Laplace Green function on the source slice is $G(r,0)=\sum_{n\in\mathbb Z}[4\pi^2(r^2+n^2L^2)]^{-1}=(4\pi Lr)^{-1}\coth(\pi r/L)$. At $r\ll L$ this is $1/(4\pi^2r^2)$; at $r\gg L$ it is $1/(4\pi Lr)$ with exponentially small corrections. The long-distance coefficient also follows by replacing the dense image sum with $L^{-1}\int_{-\infty}^{\infty}dy/(r^2+y^2)=\pi/(Lr)$. Electric and gravitational potentials inherit this crossover after multiplying by their signed source couplings.

##### Fundamental solution of the Laplace equation

↑ **Parent:** [Green function of the Laplacian](#green-function-of-the-laplacian)

Up to normalization and sign convention, a fundamental solution of the Laplace equation is $\Phi(x)=|x|^{2-n}$ for $n\geq3$ and $\Phi(x)=\log|x|$ for $n=2$. It is harmonic away from the origin and satisfies $\Delta\Phi=c_n\delta_0$ distributionally.

#### Laplace equation in polar coordinates

↑ **Parent:** [Laplace equation](#laplace-equation)

In plane [polar coordinates](calculus.md#polar-coordinates), [Laplace's equation](#laplace-equation) is

$$
\frac1r\frac{\partial}{\partial r}
\left(r\frac{\partial\phi}{\partial r}\right)
+\frac1{r^2}\frac{\partial^2\phi}{\partial\theta^2}=0.
$$

[Separation of variables](#separation-of-variables) gives radial powers $r^n,r^{-n}$ for positive angular modes and $1,\log r$ for the zero mode.

#### Laplace equation in cylindrical coordinates

↑ **Parent:** [Laplace equation](#laplace-equation)

In cylindrical coordinates $(r,\theta,z)$, [Laplace's equation](#laplace-equation) is

$$
\frac1r\frac{\partial}{\partial r}
\left(r\frac{\partial\phi}{\partial r}\right)
+\frac1{r^2}\frac{\partial^2\phi}{\partial\theta^2}
+\frac{\partial^2\phi}{\partial z^2}=0.
$$

##### Side boundary data do not determine a bounded harmonic function in a half-cylinder

↑ **Parent:** [Laplace equation in cylindrical coordinates](#laplace-equation-in-cylindrical-coordinates)

In the unit half-cylinder $z\ge0$, specifying only the curved-side boundary values does not determine a bounded [harmonic function](#harmonic-function). The displayed nonzero function, where $j_{0,1}$ is a positive zero of the [Bessel function of the first kind](analysis.md#bessel-function-of-the-first-kind) $J_0$, is regular at the axis, bounded, harmonic, and zero on $r=1$. It may be added to any particular solution without changing the side data, and even decays at infinity. Boundary information at the base $z=0$ is still required for uniqueness.

### Radial Laplacian

↑ **Parent:** [Laplace operator](#laplace-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radial_Laplacian)

For radial $u(r)$ in $n$ dimensions, $\Delta u=u\prime\prime+(n-1)u\prime/r$.

### Laplacian in spherical coordinates

↑ **Parent:** [Laplace operator](#laplace-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Laplacian_in_spherical_coordinates)

The spherical-coordinate Laplacian splits into a radial operator and the sphere’s angular Laplacian divided by $r^2$.

#### Axisymmetric harmonic function

↑ **Parent:** [Laplacian in spherical coordinates](#laplacian-in-spherical-coordinates)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Axisymmetric_harmonic_function)

Axisymmetric harmonic functions separate into radial powers times Legendre polynomials.

### Laplacian eigenfunction

↑ **Parent:** [Laplace operator](#laplace-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Laplacian_eigenfunction)

A Laplacian eigenfunction satisfies $-\Delta u=\lambda u$ together with specified boundary conditions.

#### Laplacian eigenvalue

↑ **Parent:** [Laplacian eigenfunction](#laplacian-eigenfunction)

A scalar $\lambda$ for which a nonzero [Laplacian eigenfunction](#laplacian-eigenfunction) satisfies this equation, with specified boundary conditions or on a closed [manifold](topology.md#topological-manifold), is an eigenvalue of the positive [Laplacian](calculus.md#laplacian). A [Dirichlet Laplacian eigenvalue](#dirichlet-laplacian-eigenvalue) imposes zero boundary values; other boundary conditions generally change the [spectrum](linear-operator-theory.md#spectrum-functional-analysis).

#### Dirichlet Laplacian eigenfunction

↑ **Parent:** [Laplacian eigenfunction](#laplacian-eigenfunction)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dirichlet_Laplacian_eigenfunction)

A Dirichlet Laplacian eigenfunction vanishes on the boundary and satisfies $-\Delta u=\lambda u$.

##### Dirichlet eigenfunction supremum estimate

↑ **Parent:** [Dirichlet Laplacian eigenfunction](#dirichlet-laplacian-eigenfunction)

For $n\geq3$ and a bounded smooth domain, a [Dirichlet Laplacian eigenfunction](#dirichlet-laplacian-eigenfunction) with [eigenvalue](linear-operator-theory.md#eigenvalue) $\lambda$ satisfies the displayed estimate. A [signed power test for a Laplacian eigenfunction](#signed-power-test-for-a-laplacian-eigenfunction) and the zero-boundary [Sobolev inequality](sobolev-space.md#sobolev-inequality) give a [Moser iteration](elliptic-boundary-value-problem.md#moser-iteration) with exponents $p_j=2[n/(n-2)]^j$. The [geometric series](real-analysis.md#geometric-series) $\sum_j1/p_j=n/4$ gives the exact power of $\lambda$, while $\sum_j(\log p_j)/p_j<\infty$ controls the remaining constant. The constant depends only on dimension, because the zero-boundary [Sobolev inequality](sobolev-space.md#sobolev-inequality) follows by extension by zero to the whole space.

##### Dirichlet Laplacian eigenvalue

↑ **Parent:** [Dirichlet Laplacian eigenfunction](#dirichlet-laplacian-eigenfunction)

A Dirichlet Laplacian eigenvalue is a number $\lambda$ for which $-\Delta u=\lambda u$ has a nonzero solution with zero boundary trace. At such a value, the shifted operator $\Delta+\lambda$ is not invertible.

## Wave equation

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)

[This section is present in another page, follow this link to view it.](wave-equation.md)

## Green second identity

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Green_second_identity)

Green’s second identity is the divergence theorem applied to phi grad psi minus psi grad phi.

## Lie point symmetry

↑ **Parent:** [Partial differential equation](partial-differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lie_point_symmetry)

A Lie point symmetry is a continuous transformation of independent and dependent variables that maps solutions of a differential equation to solutions.

### Infinitesimal generator of a Lie point symmetry

↑ **Parent:** [Lie point symmetry](#lie-point-symmetry)

A one-parameter point transformation has infinitesimal generator

$$
V=\sum_i\xi^i(x,u)\partial_{x_i}+\eta(x,u)\partial_u.
$$

Its flow recovers the finite transformations.

### Prolongation of a Lie point symmetry

↑ **Parent:** [Lie point symmetry](#lie-point-symmetry)

The prolongation of a point-symmetry generator is its induced vector field on derivatives of the dependent variable. A generator is a symmetry of a differential equation $F=0$ when its required prolongation sends $F$ to zero on the solution manifold.

#### Second prolongation of a Lie point symmetry

↑ **Parent:** [Prolongation of a Lie point symmetry](#prolongation-of-a-lie-point-symmetry)

For $V=\xi^i\partial_{x_i}+\eta\partial_u$, the second prolongation adds coefficients for $u_i$ and $u_{ij}$ obtained by total differentiation:

$$
\eta_i=D_i\eta-u_jD_i\xi^j,
\qquad
\eta_{ij}=D_j\eta_i-u_{ik}D_j\xi^k.
$$

### Scaling symmetry

↑ **Parent:** [Lie point symmetry](#lie-point-symmetry)

A scaling symmetry acts by weighted dilations of the independent and dependent variables. Its infinitesimal generator is a weighted sum of Euler vector fields such as $x\partial_x+pu\partial_u$.

#### Scaling symmetry of a partial differential equation

↑ **Parent:** [Scaling symmetry](#scaling-symmetry)

A scaling is a symmetry when every term of the equation transforms with the same weight.

##### Simultaneous spacetime scaling symmetry of the wave equation

↑ **Parent:** [Scaling symmetry of a partial differential equation](#scaling-symmetry-of-a-partial-differential-equation)

The flow of $V=t\partial_t+x\partial_x$ is $(t,x,u)\mapsto(e^\epsilon t,e^\epsilon x,u)$. Its second prolongation scales both $u_{tt}$ and $u_{xx}$ with weight minus two, so it preserves $u_{tt}-u_{xx}=0$.

### Symmetry reduction of a partial differential equation

↑ **Parent:** [Lie point symmetry](#lie-point-symmetry)

An invariant of a one-parameter symmetry group becomes a similarity variable that reduces a PDE to an ODE.

#### Group-invariant solution

↑ **Parent:** [Symmetry reduction of a partial differential equation](#symmetry-reduction-of-a-partial-differential-equation)

A group-invariant solution is constant along the prolonged symmetry orbits. For a scaling of two independent variables with fixed dependent variable, it depends only on a ratio such as $x/t$.

#### Projective Lie symmetry of the potential Burgers equation

↑ **Parent:** [Symmetry reduction of a partial differential equation](#symmetry-reduction-of-a-partial-differential-equation)

The vector field

$$
V=4t^2\partial_t+4tx\partial_x-(x^2+2t)\partial_u
$$

generates the local transformations

$$
T=\frac{t}{1-4\epsilon t},
\quad
X=\frac{x}{1-4\epsilon t},
\quad
U=u-\frac{\epsilon x^2}{1-4\epsilon t}
+\frac12\log(1-4\epsilon t).
$$

Its second prolongation sends $u_t-u_{xx}-u_x^2$ to $-8t$ times that expression, so it is a [Lie point symmetry](#lie-point-symmetry) of the [potential Burgers equation](diffusion-equation.md#potential-burgers-equation).

#### Similarity variable

↑ **Parent:** [Symmetry reduction of a partial differential equation](#symmetry-reduction-of-a-partial-differential-equation)

A similarity variable is constant along symmetry-group orbits and parametrizes group-invariant solutions.

## ↑ Ancestors (4)

1. [Analysis](analysis.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (48)

- [Boundary trace of a function](differential-equation.md#boundary-trace-of-a-function)
- [Bounded parabolic differentiability class](#bounded-parabolic-differentiability-class)
- [Conserved-mean convection amplitude equations](dynamical-systems.md#conserved-mean-convection-amplitude-equations)
- [Exponential payoff transform PDE](mathematical-finance.md#exponential-payoff-transform-pde)
- [Feynman-Kac formula](stochastic-calculus.md#feynman-kac-formula)
- [Finite-horizon extension of a boundary transform](differential-equation.md#finite-horizon-extension-of-a-boundary-transform)
- [Finite-time spectral boundary transform](differential-equation.md#finite-time-spectral-boundary-transform)
- [Finite-time stability versus power boundedness](finite-difference.md#finite-time-stability-versus-power-boundedness)
- [Hirota's bilinear method](integrable-systems.md#hirota-s-bilinear-method)
- [Infinite-dimensional Hamiltonian integrability](integrable-systems.md#infinite-dimensional-hamiltonian-integrability)
- [Linear partial differential equation](#linear-partial-differential-equation)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-22.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-54.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-54.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-56.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-59.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-61.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-3.md#29c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-67.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-35.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-2.md#6b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-1.md#29a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-83.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-71.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-2.md#2a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2.md#13a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-39.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-39.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-39.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-69.md#1/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-10.md#3/3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-3.md#3c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-328.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-3.md#7a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-202.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-202.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-211.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-328.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-332.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-332.md#1/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-105.md#1/a/solution)
- [Similarity ansatz](#similarity-ansatz)
- [Viscosity solution](#viscosity-solution)
- [Weighted Euler first-order equation](#weighted-euler-first-order-equation)
