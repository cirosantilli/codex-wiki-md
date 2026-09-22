# Differential equation

↑ **Parent:** [Analysis](analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Differential_equation)

**Table of contents**

- [Direction field](#direction-field)
- [Isocline](#isocline)
- [Jump condition](#jump-condition)
- [Delay differential equation](#delay-differential-equation)
- [Solution of a differential equation](#solution-of-a-differential-equation)
- [Ordinary differential equation](#ordinary-differential-equation)
  - [First integral of an ordinary differential equation](#first-integral-of-an-ordinary-differential-equation)
  - [Second-order differential equation](#second-order-differential-equation)
  - [Painlevé equation](#painleve-equation)
    - [Painlevé II equation](#painleve-ii-equation)
    - [Painlevé transcendent](#painleve-transcendent)
  - [Complex ordinary differential equation](#complex-ordinary-differential-equation)
    - [Painlevé property](#painleve-property)
    - [Painlevé determinateness theorem](#painleve-determinateness-theorem)
    - [Movable singularity of a complex differential equation](#movable-singularity-of-a-complex-differential-equation)
    - [Fixed singularity of a complex differential equation](#fixed-singularity-of-a-complex-differential-equation)
    - [Holomorphic dependence of ordinary differential equations on parameters](#holomorphic-dependence-of-ordinary-differential-equations-on-parameters)
  - [Periodic solution](#periodic-solution)
  - [Variational equation](#variational-equation)
  - [Osgood uniqueness criterion](#osgood-uniqueness-criterion)
  - [Distributional regularity of a constant-coefficient ordinary differential equation](#distributional-regularity-of-a-constant-coefficient-ordinary-differential-equation)
    - [Coordinate-degenerate constant-coefficient differential equation](#coordinate-degenerate-constant-coefficient-differential-equation)
    - [Exponential polynomial solution of a constant-coefficient differential equation](#exponential-polynomial-solution-of-a-constant-coefficient-differential-equation)
  - [Implicit solution](#implicit-solution)
  - [Exact first-order ordinary differential equation](#exact-first-order-ordinary-differential-equation)
  - [Continuous dependence of an ODE solution on parameters](#continuous-dependence-of-an-ode-solution-on-parameters)
  - [Exponential relaxation time](#exponential-relaxation-time)
  - [Initial value problem](#initial-value-problem)
    - [L2 initial condition](#l2-initial-condition)
  - [Degenerate ordinary differential equation](#degenerate-ordinary-differential-equation)
    - [Continuation through a zero of the leading ODE coefficient](#continuation-through-a-zero-of-the-leading-ode-coefficient)
  - [Compact support solvability for a constant-coefficient ordinary differential equation](#compact-support-solvability-for-a-constant-coefficient-ordinary-differential-equation)
  - [Singular point of a differential equation](#singular-point-of-a-differential-equation)
  - [Dissipative vector field](#dissipative-vector-field)
  - [Peano existence theorem](#peano-existence-theorem)
  - [Separable differential equation](#separable-differential-equation)
    - [Cubic logistic differential equation](#cubic-logistic-differential-equation)
  - [Nonlinear ordinary differential equation](#nonlinear-ordinary-differential-equation)
    - [Ermakov-Pinney equation](#ermakov-pinney-equation)
      - [Exact amplitude-phase equation](#exact-amplitude-phase-equation)
    - [Position-dependent damping](#position-dependent-damping)
    - [Logistic differential equation](#logistic-differential-equation)
      - [Euler discretization of logistic growth](#euler-discretization-of-logistic-growth)
  - [Picard-Lindelöf theorem](#picard-lindelof-theorem)
    - [Finite-dimensional continuation criterion](#finite-dimensional-continuation-criterion)
    - [Bielecki norm method](#bielecki-norm-method)
  - [Finite-time blowup](#finite-time-blowup)
  - [Linear differential equation](#linear-differential-equation)
    - [Fuchsian linear differential system](#fuchsian-linear-differential-system)
      - [Analytic solution at a maximal integer Fuchsian exponent](#analytic-solution-at-a-maximal-integer-fuchsian-exponent)
      - [Residue and monodromy of a constant Fuchsian system](#residue-and-monodromy-of-a-constant-fuchsian-system)
    - [Fundamental matrix of a linear differential equation](#fundamental-matrix-of-a-linear-differential-equation)
      - [Gauge transformation of a linear differential system](#gauge-transformation-of-a-linear-differential-system)
        - [Formal cubic-exponential two-by-two system](#formal-cubic-exponential-two-by-two-system)
      - [Liouville formula for a fundamental matrix](#liouville-formula-for-a-fundamental-matrix)
    - [Floquet theory](#floquet-theory)
      - [Floquet exponent](#floquet-exponent)
      - [Floquet growth rate](#floquet-growth-rate)
      - [Monodromy matrix of a periodic linear system](#monodromy-matrix-of-a-periodic-linear-system)
    - [Characteristic root of a constant-coefficient differential equation](#characteristic-root-of-a-constant-coefficient-differential-equation)
    - [Laplace contour-integral method for a linear differential equation](#laplace-contour-integral-method-for-a-linear-differential-equation)
    - [Homogeneous linear differential equation](#homogeneous-linear-differential-equation)
      - [Solution space of a homogeneous linear differential equation](#solution-space-of-a-homogeneous-linear-differential-equation)
    - [Linearized equation](#linearized-equation)
    - [Inhomogeneous linear differential equation](#inhomogeneous-linear-differential-equation)
  - [Local existence for a scalar autonomous ordinary differential equation with continuous vector field](#local-existence-for-a-scalar-autonomous-ordinary-differential-equation-with-continuous-vector-field)
  - [Singular perturbation](#singular-perturbation)
    - [Beyond-all-orders boundary-value sensitivity](#beyond-all-orders-boundary-value-sensitivity)
    - [Adiabatic elimination](#adiabatic-elimination)
    - [Matched asymptotic expansion](#matched-asymptotic-expansion)
      - [Endpoint derivative in a negative-drift boundary layer](#endpoint-derivative-in-a-negative-drift-boundary-layer)
      - [Logistic crossover in a weakly nonlinear Euler equation](#logistic-crossover-in-a-weakly-nonlinear-euler-equation)
        - [Nonlinear crossover delayed by a small unstable-mode coefficient](#nonlinear-crossover-delayed-by-a-small-unstable-mode-coefficient)
      - [Nonlinear endpoint layer with a quadratic reaction](#nonlinear-endpoint-layer-with-a-quadratic-reaction)
        - [One-third-power scaling at a nonlinear turning endpoint](#one-third-power-scaling-at-a-nonlinear-turning-endpoint)
      - [Asymptotic matching condition](#asymptotic-matching-condition)
      - [Square-root reaction problem with nested boundary layers](#square-root-reaction-problem-with-nested-boundary-layers)
        - [First integral of a square-root reaction layer](#first-integral-of-a-square-root-reaction-layer)
      - [Nested layers at an essential singular endpoint](#nested-layers-at-an-essential-singular-endpoint)
      - [Matched expansion with square-root and logarithmic corrections](#matched-expansion-with-square-root-and-logarithmic-corrections)
      - [Logarithmic matching in a small-exponent boundary layer](#logarithmic-matching-in-a-small-exponent-boundary-layer)
      - [Gaussian interior layer of a conservative drift equation](#gaussian-interior-layer-of-a-conservative-drift-equation)
      - [Oscillatory endpoint with a quadratically vanishing drift](#oscillatory-endpoint-with-a-quadratically-vanishing-drift)
      - [First-order composite expansion for a positive drift](#first-order-composite-expansion-for-a-positive-drift)
      - [Logarithmically enhanced nonlinear boundary layer](#logarithmically-enhanced-nonlinear-boundary-layer)
      - [Boundary layer around a moving endpoint](#boundary-layer-around-a-moving-endpoint)
      - [Square-root boundary layer at a vanishing drift](#square-root-boundary-layer-at-a-vanishing-drift)
        - [Error-function logarithmic switchback](#error-function-logarithmic-switchback)
      - [Overlap region](#overlap-region)
      - [Intermediate asymptotic region](#intermediate-asymptotic-region)
      - [Interior layer at a simple zero of advection](#interior-layer-at-a-simple-zero-of-advection)
        - [Endpoint layers for reversed diffusion](#endpoint-layers-for-reversed-diffusion)
      - [Distinguished limit](#distinguished-limit)
      - [Inner expansion](#inner-expansion)
        - [Square-root-degenerate endpoint layer](#square-root-degenerate-endpoint-layer)
        - [Inner variable](#inner-variable)
      - [Outer expansion](#outer-expansion)
      - [Additive composite expansion](#additive-composite-expansion)
      - [Multiplicative composite expansion](#multiplicative-composite-expansion)
      - [Outflow boundary layer](#outflow-boundary-layer)
      - [Switchback term](#switchback-term)
        - [Logarithmic overlap creates a switchback term](#logarithmic-overlap-creates-a-switchback-term)
    - [Method of multiple scales](#method-of-multiple-scales)
      - [Slow oscillator damping by a relaxing auxiliary variable](#slow-oscillator-damping-by-a-relaxing-auxiliary-variable)
      - [Averaged oscillator damping by a power of velocity](#averaged-oscillator-damping-by-a-power-of-velocity)
      - [Second-order resonance from quadratic oscillator coupling](#second-order-resonance-from-quadratic-oscillator-coupling)
      - [Averaged amplitude for position-dependent damping](#averaged-amplitude-for-position-dependent-damping)
        - [Absolute-value damping amplitude law](#absolute-value-damping-amplitude-law)
        - [Van der Pol amplitude evolution](#van-der-pol-amplitude-evolution)
          - [Shifted Van der Pol amplitude evolution](#shifted-van-der-pol-amplitude-evolution)
        - [Odd position-dependent damping has zero first-order amplitude drift](#odd-position-dependent-damping-has-zero-first-order-amplitude-drift)
      - [Secular term](#secular-term)
      - [Whitham modulation theory](#whitham-modulation-theory)
        - [Averaged Lagrangian](#averaged-lagrangian)
          - [Modulated-wave first integral](#modulated-wave-first-integral)
          - [Whitham modulation equation](#whitham-modulation-equation)
            - [Wave-action density](#wave-action-density)
              - [Wave-action conservation law](#wave-action-conservation-law)
      - [Amplitude-phase equations for a weakly perturbed oscillator](#amplitude-phase-equations-for-a-weakly-perturbed-oscillator)
        - [Oscillator coupled to slow damping feedback](#oscillator-coupled-to-slow-damping-feedback)
        - [Velocity-only forcing in averaged oscillator equations](#velocity-only-forcing-in-averaged-oscillator-equations)
          - [Quadratically damped oscillator](#quadratically-damped-oscillator)
          - [Cubic velocity anti-damping](#cubic-velocity-anti-damping)
        - [Conservative forcing in averaged oscillator equations](#conservative-forcing-in-averaged-oscillator-equations)
      - [Slow time](#slow-time)
      - [Weakly nonlinear expansion](#weakly-nonlinear-expansion)
        - [Quadratic wave interaction](#quadratic-wave-interaction)
          - [Resonant three-wave triad](#resonant-three-wave-triad)
          - [Detuning of a wave resonance](#detuning-of-a-wave-resonance)
          - [Phase matching for a quadratic wave interaction](#phase-matching-for-a-quadratic-wave-interaction)
            - [Two-to-one resonance of dispersive waves](#two-to-one-resonance-of-dispersive-waves)
              - [Explosive two-to-one amplitude system](#explosive-two-to-one-amplitude-system)
      - [Harmonic balance](#harmonic-balance)
      - [Solvability condition in the method of multiple scales](#solvability-condition-in-the-method-of-multiple-scales)
      - [Parametric resonance](#parametric-resonance)
        - [Primary instability tongue of a weak Mathieu oscillator](#primary-instability-tongue-of-a-weak-mathieu-oscillator)
        - [Primary parametric resonance of a two-to-one oscillator pair](#primary-parametric-resonance-of-a-two-to-one-oscillator-pair)
        - [Second instability tongue of a weak Mathieu oscillator](#second-instability-tongue-of-a-weak-mathieu-oscillator)
          - [Slow amplitudes for the second Mathieu instability tongue](#slow-amplitudes-for-the-second-mathieu-instability-tongue)
          - [Fourth-order edges of the second Mathieu instability tongue](#fourth-order-edges-of-the-second-mathieu-instability-tongue)
  - [Lie point symmetry of an ordinary differential equation](#lie-point-symmetry-of-an-ordinary-differential-equation)
    - [Prolongation of a vector field](#prolongation-of-a-vector-field)
      - [First prolongation](#first-prolongation)
      - [Jet space of a scalar ordinary differential equation](#jet-space-of-a-scalar-ordinary-differential-equation)
        - [Solution manifold](#solution-manifold)
      - [Lie-symmetry determining equation for a first-order ordinary differential equation](#lie-symmetry-determining-equation-for-a-first-order-ordinary-differential-equation)
      - [Second prolongation of the rotation generator for plane graphs](#second-prolongation-of-the-rotation-generator-for-plane-graphs)
      - [Total derivative operator](#total-derivative-operator)
      - [Schwarzian derivative](#schwarzian-derivative)
        - [Prolongations of the projective vector fields on the line](#prolongations-of-the-projective-vector-fields-on-the-line)
        - [Projective transformation weights of the Schwarzian derivative](#projective-transformation-weights-of-the-schwarzian-derivative)
      - [Affine-scaling symmetry of u double prime equals u prime squared over u minus u squared](#affine-scaling-symmetry-of-u-double-prime-equals-u-prime-squared-over-u-minus-u-squared)
  - [Boundary value problem](#boundary-value-problem)
    - [Neumann boundary-value problem](#neumann-boundary-value-problem)
    - [Boundary trace of a function](#boundary-trace-of-a-function)
    - [Oblique derivative boundary condition](#oblique-derivative-boundary-condition)
      - [Corner compatibility for collinear oblique derivative data](#corner-compatibility-for-collinear-oblique-derivative-data)
      - [Rational-angle oblique derivative problem on a quadrant](#rational-angle-oblique-derivative-problem-on-a-quadrant)
        - [Quarter-plane oblique boundary spectral functions](#quarter-plane-oblique-boundary-spectral-functions)
          - [Single-function spectral elimination for a rational-angle quadrant](#single-function-spectral-elimination-for-a-rational-angle-quadrant)
        - [Homogeneous corner ambiguity in a quadrant Laplace problem](#homogeneous-corner-ambiguity-in-a-quadrant-laplace-problem)
    - [Dirichlet-to-Neumann map](#dirichlet-to-neumann-map)
      - [Semistrip Dirichlet-to-Neumann sine transforms](#semistrip-dirichlet-to-neumann-sine-transforms)
    - [Riemann-Hilbert problem](#riemann-hilbert-problem)
      - [Sectorial half-line mKdV Riemann-Hilbert reconstruction](#sectorial-half-line-mkdv-riemann-hilbert-reconstruction)
      - [Half-line NLS Riemann-Hilbert reconstruction](#half-line-nls-riemann-hilbert-reconstruction)
      - [Negative-index scalar Riemann-Hilbert moment conditions](#negative-index-scalar-riemann-hilbert-moment-conditions)
      - [Matrix NLS reconstruction from a normalized Riemann-Hilbert problem](#matrix-nls-reconstruction-from-a-normalized-riemann-hilbert-problem)
      - [Canonical factorization of a rational scalar Riemann-Hilbert jump](#canonical-factorization-of-a-rational-scalar-riemann-hilbert-jump)
    - [Wiener-Hopf method](#wiener-hopf-method)
      - [Mixed Dirichlet-Neumann half-plane diffraction](#mixed-dirichlet-neumann-half-plane-diffraction)
      - [Wiener-Hopf factorization](#wiener-hopf-factorization)
      - [Wiener-Hopf equation](#wiener-hopf-equation)
        - [Wiener-Hopf kernel](#wiener-hopf-kernel)
        - [Pole subtraction in a Wiener-Hopf equation](#pole-subtraction-in-a-wiener-hopf-equation)
    - [Fokas method](#fokas-method)
      - [Two-trace half-line cubic dispersion representation](#two-trace-half-line-cubic-dispersion-representation)
      - [Boundary spectral representation of a holomorphic function on a semistrip](#boundary-spectral-representation-of-a-holomorphic-function-on-a-semistrip)
      - [Quadrant modified Helmholtz spectral reconstruction](#quadrant-modified-helmholtz-spectral-reconstruction)
      - [Neumann spectral formula for half-line constant drift](#neumann-spectral-formula-for-half-line-constant-drift)
      - [Dirichlet spectral formula for half-line constant drift](#dirichlet-spectral-formula-for-half-line-constant-drift)
      - [Local relation](#local-relation)
      - [Dispersion symmetry elimination of a boundary trace](#dispersion-symmetry-elimination-of-a-boundary-trace)
        - [Cubic-dispersion elimination of one missing boundary trace](#cubic-dispersion-elimination-of-one-missing-boundary-trace)
        - [Cubic Stokes dispersion symmetry](#cubic-stokes-dispersion-symmetry)
      - [Upper-quadrant cancellation of reflected boundary transforms](#upper-quadrant-cancellation-of-reflected-boundary-transforms)
    - [Global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem)
      - [Dirichlet spectral formula for Airy flow with negative transport](#dirichlet-spectral-formula-for-airy-flow-with-negative-transport)
      - [Finite-interval Airy global relation](#finite-interval-airy-global-relation)
        - [Finite-interval Airy spectral determinant](#finite-interval-airy-spectral-determinant)
      - [Semistrip Laplace spectral global relation](#semistrip-laplace-spectral-global-relation)
      - [Drift-diffusion half-line global relation](#drift-diffusion-half-line-global-relation)
      - [Half-line linear dispersive Stokes global relation](#half-line-linear-dispersive-stokes-global-relation)
        - [Dirichlet spectral representation for the linear dispersive Stokes equation](#dirichlet-spectral-representation-for-the-linear-dispersive-stokes-equation)
      - [Half-line Schrodinger boundary-trace elimination](#half-line-schrodinger-boundary-trace-elimination)
      - [Finite-time spectral boundary transform](#finite-time-spectral-boundary-transform)
        - [Finite-horizon extension of a boundary transform](#finite-horizon-extension-of-a-boundary-transform)
      - [Polygonal modified Helmholtz global relation](#polygonal-modified-helmholtz-global-relation)
        - [Dirichlet reconstruction in an equilateral triangle](#dirichlet-reconstruction-in-an-equilateral-triangle)
      - [Half-line drift global relation](#half-line-drift-global-relation)
        - [Exponential-decay contour for half-line drift diffusion](#exponential-decay-contour-for-half-line-drift-diffusion)
      - [Collocation points for a global relation](#collocation-points-for-a-global-relation)
      - [Conjugate global relations for the modified Helmholtz equation](#conjugate-global-relations-for-the-modified-helmholtz-equation)
        - [Rotationally invariant Neumann reconstruction in an equilateral triangle](#rotationally-invariant-neumann-reconstruction-in-an-equilateral-triangle)
        - [Sine collocation of square modified Helmholtz global relations](#sine-collocation-of-square-modified-helmholtz-global-relations)
          - [Square modified Helmholtz Dirichlet-to-Neumann coefficients](#square-modified-helmholtz-dirichlet-to-neumann-coefficients)
          - [Diagonal dominance of paired square global-relation collocation](#diagonal-dominance-of-paired-square-global-relation-collocation)
    - [Spectral parameter for a linear boundary value problem](#spectral-parameter-for-a-linear-boundary-value-problem)
    - [Boundary lifting](#boundary-lifting)
      - [Uniform half-line Schrodinger representation by boundary lifting](#uniform-half-line-schrodinger-representation-by-boundary-lifting)
  - [Boundary condition](#boundary-condition)
    - [Dynamic boundary condition for the heat equation](#dynamic-boundary-condition-for-the-heat-equation)
      - [Dirichlet energy dissipation with a dynamic heat boundary condition](#dirichlet-energy-dissipation-with-a-dynamic-heat-boundary-condition)
      - [Repeated-root dynamic-boundary heat kernel](#repeated-root-dynamic-boundary-heat-kernel)
        - [Repeated-root unstable heat boundary mode](#repeated-root-unstable-heat-boundary-mode)
    - [Clamped boundary condition](#clamped-boundary-condition)
    - [Periodic boundary conditions](#periodic-boundary-conditions)
    - [Vanishing boundary condition](#vanishing-boundary-condition)
    - [Initial condition](#initial-condition)
      - [Initial velocity](#initial-velocity)
      - [Initial displacement](#initial-displacement)
    - [Dirichlet boundary condition](#dirichlet-boundary-condition)
      - [Dirichlet boundary data](#dirichlet-boundary-data)
      - [Perfectly conducting thermal boundary condition](#perfectly-conducting-thermal-boundary-condition)
    - [Neumann boundary condition](#neumann-boundary-condition)
      - [Neumann boundary data](#neumann-boundary-data)
      - [Initial incompatibility with a Neumann boundary condition](#initial-incompatibility-with-a-neumann-boundary-condition)
      - [Neumann eigenfunction](#neumann-eigenfunction)
    - [Tangential boundary derivative](#tangential-boundary-derivative)
    - [Robin boundary condition](#robin-boundary-condition)
      - [Poisson uniqueness with a nonnegative Robin normal coefficient](#poisson-uniqueness-with-a-nonnegative-robin-normal-coefficient)
      - [Symmetric Robin strip transform](#symmetric-robin-strip-transform)
        - [Solvability of a decaying Robin strip](#solvability-of-a-decaying-robin-strip)
      - [Weak Robin problem for a uniformly elliptic operator](#weak-robin-problem-for-a-uniformly-elliptic-operator)
    - [Mixed boundary condition](#mixed-boundary-condition)
    - [Far-field boundary condition](#far-field-boundary-condition)
  - [Sign-decay differential equation](#sign-decay-differential-equation)
    - [Explicit Euler method for the sign-decay equation](#explicit-euler-method-for-the-sign-decay-equation)
  - [Parameter sensitivity equation](#parameter-sensitivity-equation)
  - [Differential inequality](#differential-inequality)
  - [Bernoulli differential equation](#bernoulli-differential-equation)
    - [Finite-time extinction in a sublinear Bernoulli equation](#finite-time-extinction-in-a-sublinear-bernoulli-equation)
  - [Tangent addition functional equation](#tangent-addition-functional-equation)
  - [Linear ordinary differential equation](#linear-ordinary-differential-equation)
    - [Characteristic equation of a constant-coefficient differential equation](#characteristic-equation-of-a-constant-coefficient-differential-equation)
    - [Method of undetermined coefficients](#method-of-undetermined-coefficients)
      - [Resonant exponential particular solution](#resonant-exponential-particular-solution)
    - [Weighted energy estimate for two coupled modes](#weighted-energy-estimate-for-two-coupled-modes)
    - [Newton's law of cooling](#newton-s-law-of-cooling)
      - [Impulse versus finite-duration cooling](#impulse-versus-finite-duration-cooling)
      - [Cumulative thermal destruction under exponential warming and cooling](#cumulative-thermal-destruction-under-exponential-warming-and-cooling)
      - [Newton cooling with an instantaneous temperature jump](#newton-cooling-with-an-instantaneous-temperature-jump)
      - [Heat transfer coefficient](#heat-transfer-coefficient)
    - [Homogeneous solution](#homogeneous-solution)
    - [Particular solution](#particular-solution)
    - [General solution](#general-solution)
    - [Dominant eigenmode in a forced linear system](#dominant-eigenmode-in-a-forced-linear-system)
    - [Second-order linear differential equation](#second-order-linear-differential-equation)
      - [Quadratic-variable reduction of a singular oscillator](#quadratic-variable-reduction-of-a-singular-oscillator)
      - [Repeated-root constant-coefficient differential equation](#repeated-root-constant-coefficient-differential-equation)
      - [Singular point of a second-order linear ODE](#singular-point-of-a-second-order-linear-ode)
      - [Reciprocal-coordinate reduction of a beam-type equation](#reciprocal-coordinate-reduction-of-a-beam-type-equation)
      - [Liouville transformation of a second-order equation](#liouville-transformation-of-a-second-order-equation)
      - [Power substitution for an oscillatory second-order equation](#power-substitution-for-an-oscillatory-second-order-equation)
      - [Mathieu equation](#mathieu-equation)
        - [Mathieu characteristic value](#mathieu-characteristic-value)
      - [Airy ordinary differential equation](#airy-ordinary-differential-equation)
        - [Forced Airy boundary-value problem](#forced-airy-boundary-value-problem)
        - [Airy power-series fundamental pair](#airy-power-series-fundamental-pair)
        - [Airy function](#airy-function)
          - [Airy displacement integral](#airy-displacement-integral)
      - [Elimination of the first derivative](#elimination-of-the-first-derivative)
      - [Sturm-Picone comparison theorem](#sturm-picone-comparison-theorem)
        - [Sturm comparison theorem](#sturm-comparison-theorem)
          - [Wronskian proof of Sturm comparison](#wronskian-proof-of-sturm-comparison)
      - [Power-series solution of a differential equation](#power-series-solution-of-a-differential-equation)
      - [Kummer differential equation](#kummer-differential-equation)
        - [Confluent hypergeometric function](#confluent-hypergeometric-function)
          - [Confluent hypergeometric function of the first kind](#confluent-hypergeometric-function-of-the-first-kind)
      - [Wronskian](#wronskian)
        - [Abel's identity](#abel-s-identity)
      - [Variation of parameters](#variation-of-parameters)
      - [Reduction of order](#reduction-of-order)
        - [First correction to a regular singular solution by reduction of order](#first-correction-to-a-regular-singular-solution-by-reduction-of-order)
        - [Reduction of order across a zero of the known solution](#reduction-of-order-across-a-zero-of-the-known-solution)
      - [Cauchy-Euler equation](#cauchy-euler-equation)
        - [Euler-Cauchy classification from two regular singular points](#euler-cauchy-classification-from-two-regular-singular-points)
        - [Euler-Cauchy equation](#euler-cauchy-equation)
        - [General solution of an Euler-Cauchy equation](#general-solution-of-an-euler-cauchy-equation)
          - [Power-law ansatz](#power-law-ansatz)
            - [Indicial equation](#indicial-equation)
              - [Indicial root](#indicial-root)
              - [Indicial exponent](#indicial-exponent)
            - [Log-periodic oscillation](#log-periodic-oscillation)
      - [Legendre differential equation](#legendre-differential-equation)
        - [Associated Legendre differential equation](#associated-legendre-differential-equation)
        - [Associated Legendre function](#associated-legendre-function)
        - [Legendre polynomial](#legendre-polynomial)
          - [Weighted orthogonality of Legendre polynomial derivatives](#weighted-orthogonality-of-legendre-polynomial-derivatives)
          - [Generating function and norm of Legendre polynomials](#generating-function-and-norm-of-legendre-polynomials)
          - [Orthogonality of Legendre polynomials](#orthogonality-of-legendre-polynomials)
          - [Legendre polynomial recurrence relation](#legendre-polynomial-recurrence-relation)
          - [Schläfli contour integral for Legendre polynomials](#schlafli-contour-integral-for-legendre-polynomials)
          - [Debye asymptotic for Legendre polynomials](#debye-asymptotic-for-legendre-polynomials)
            - [Hyperbolic Debye asymptotic for Legendre polynomials](#hyperbolic-debye-asymptotic-for-legendre-polynomials)
              - [Legendre boundary layer at x equals one](#legendre-boundary-layer-at-x-equals-one)
      - [Change of independent variable in a second-order ODE](#change-of-independent-variable-in-a-second-order-ode)
    - [First-order linear differential equation](#first-order-linear-differential-equation)
      - [Causal response of a first-order relaxation equation](#causal-response-of-a-first-order-relaxation-equation)
      - [Resonant exponential forcing in a first-order equation](#resonant-exponential-forcing-in-a-first-order-equation)
    - [Integrating factor](#integrating-factor)
      - [Heaviside forcing in a first-order integrating-factor equation](#heaviside-forcing-in-a-first-order-integrating-factor-equation)
      - [Integrating factor for a differential one-form](#integrating-factor-for-a-differential-one-form)
      - [Bounded solution selected by a terminal condition](#bounded-solution-selected-by-a-terminal-condition)
    - [Resonance in a differential equation](#resonance-in-a-differential-equation)
      - [Resonance condition](#resonance-condition)
      - [Resonant forcing](#resonant-forcing)
    - [Linear system of differential equations](#linear-system-of-differential-equations)
      - [Exponential forcing of a constant-coefficient differential system](#exponential-forcing-of-a-constant-coefficient-differential-system)
      - [Cauchy-Euler differential system](#cauchy-euler-differential-system)
      - [Eigenvector method for a differential equation](#eigenvector-method-for-a-differential-equation)
      - [State transition matrix](#state-transition-matrix)
      - [Complex form of a planar linear system](#complex-form-of-a-planar-linear-system)
    - [Jump condition for an impulse](#jump-condition-for-an-impulse)
      - [Impulse cancellation of a harmonic oscillator](#impulse-cancellation-of-a-harmonic-oscillator)
  - [First integral](#first-integral)

## Direction field

↑ **Parent:** [Differential equation](differential-equation.md)

A direction field for $y'=f(x,y)$ assigns to each point in the domain the tangent direction $(1,f(x,y))$. Solution graphs are curves tangent to these directions. Normalizing the vectors makes a useful sketch; orienting them with positive first component records increasing independent variable. An [isocline](#isocline) collects points with one common slope.

## Isocline

↑ **Parent:** [Differential equation](differential-equation.md)

For a first-order [differential equation](differential-equation.md) $y'=f(x,y)$, an isocline is a [level set](topology.md#level-set) on which the slope of each solution is the same constant $k$. These curves organize a [direction field](#direction-field): draw tangent vectors proportional to $(1,k)$ along each isocline. Points where the right-hand side is undefined must be excluded.

## Jump condition

↑ **Parent:** [Differential equation](differential-equation.md)

A jump condition relates the one-sided limits of a solution or its derivatives across a discontinuity or singular forcing. Integrating a [differential equation](differential-equation.md) across a shrinking interval containing a [Dirac delta](distribution-theory.md#dirac-delta-function) source determines the permitted jump. A [jump condition for an impulse](#jump-condition-for-an-impulse) and [Rankine-Hugoniot condition](partial-differential-equation.md#rankine-hugoniot-conditions) are specific instances with different governing equations.

## Delay differential equation

↑ **Parent:** [Differential equation](differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Delay_differential_equation)

A [delay differential equation](#delay-differential-equation) relates a derivative at the current argument to values at earlier arguments. For example, the [Buchstab function](analytic-number-theory.md#buchstab-function) obeys $\frac{d}{du}(u w(u))=w(u-1)$ for $u>2$.

## Solution of a differential equation

↑ **Parent:** [Differential equation](differential-equation.md)

A classical solution is a sufficiently differentiable [function](function.md) that satisfies a [differential equation](differential-equation.md) and any prescribed initial or boundary conditions. A [weak solution](partial-differential-equation.md#weak-solution) instead satisfies an appropriate integral or distributional identity in a specified [function space](functional-analysis.md#function-space). For a smooth locally [Lipschitz continuous](real-analysis.md#lipschitz-continuity) vector field, an [ordinary differential equation](#ordinary-differential-equation) has a unique local solution for each initial state; this does not by itself ensure global existence or boundedness.

## Ordinary differential equation

↑ **Parent:** [Differential equation](differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ordinary_differential_equation)

### First integral of an ordinary differential equation

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)

A first integral of $y'=f(t,y)$ is a differentiable function $I(t,y)$ whose value is constant along solutions through every time and state in its domain. The [chain rule](calculus.md#chain-rule) makes this equivalent to the displayed pointwise identity. For $I(y)=y^TSy$ with symmetric $S$, it becomes $y^TSf(t,y)=0$. This identity at the implicit stage is what proves exact [Runge-Kutta conservation of quadratic invariants](numerical-analysis.md#runge-kutta-conservation-of-quadratic-invariants) for the [implicit midpoint rule](numerical-analysis.md#implicit-midpoint-rule). Invariance asserted only on the image of one initial-time flow needs that image to contain the stage under consideration.

### Second-order differential equation

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)

A second-order [ordinary differential equation](#ordinary-differential-equation) involves a second [derivative](calculus.md#derivative) as its highest derivative. In explicit form $y''=f(x,y,y')$, introducing $v=y'$ converts it into the first-order system $y'=v$, $v'=f(x,y,v)$. Under local regularity and [Lipschitz continuity](real-analysis.md#lipschitz-continuity) in the dependent variables, an [initial value problem](#initial-value-problem) is specified by both $y(x_0)$ and $y'(x_0)$. The linear case is a [second-order linear differential equation](#second-order-linear-differential-equation).

<h3 id="painleve-equation">Painlevé equation</h3>

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)

<h4 id="painleve-ii-equation">Painlevé II equation</h4>

↑ **Parent:** [Painlevé equation](#painleve-equation)

The second [Painlevé equation](#painleve-equation), in its standard normalization. [Similarity reductions](partial-differential-equation.md#similarity-reduction) of some [integrable systems](integrable-systems.md) give equations of this form, after rescaling variables.

<h4 id="painleve-transcendent">Painlevé transcendent</h4>

↑ **Parent:** [Painlevé equation](#painleve-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Painlevé_transcendent)

A special-function solution of one of the six [Painlevé equations](#painleve-equation).

### Complex ordinary differential equation

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)

A first-order [ordinary differential equation](#ordinary-differential-equation) with complex independent and dependent variables is solved by a [holomorphic function](complex-analysis.md#holomorphic-function) on an ordinary domain, and its [analytic continuation](complex-analysis.md#analytic-continuation) can have [branch points](complex-analysis.md#branch-point). A [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) right-hand side gives local existence and uniqueness by the integral [contraction mapping](analysis.md#contraction-mapping) used in the [Picard-Lindelöf theorem](#picard-lindelof-theorem).

<h4 id="painleve-property">Painlevé property</h4>

↑ **Parent:** [Complex ordinary differential equation](#complex-ordinary-differential-equation)

The [Painlevé property](#painleve-property) excludes movable critical singularities, such as [branch points](complex-analysis.md#branch-point), of the analytically continued general solution of a complex [differential equation](differential-equation.md). A common stronger formulation requires every movable singularity to be a [pole](isolated-singularity.md#pole), so local solutions are meromorphic there. Fixed singularities determined by the coefficients are distinguished from movable ones whose locations depend on initial data. [Riccati equations](analysis.md#riccati-equation) with meromorphic coefficients have only movable [poles](isolated-singularity.md#pole) at [ordinary points](complex-analysis.md#ordinary-point-criterion-for-a-second-order-equation): linearization expresses their solutions as [logarithmic derivatives](analytic-number-theory.md#logarithmic-derivative) of linear-system solutions. More generally, set $w=f/g$ and solve the holomorphic linear system $f'=bf+cg$, $g'=-af$. Its quotient satisfies $w'=aw^2+bw+c$ directly. Initial data $g(z_0)=1$, $f(z_0)=w(z_0)$ recover every local solution, and holomorphic $f,g$ make the quotient a [meromorphic function](isolated-singularity.md#meromorphic-function), even at zeros of $a$. At a zero of $g$ with $a\ne0$, uniqueness prevents $f=0$ there, so $g'=-af\ne0$ and the [pole](isolated-singularity.md#pole) is simple. This proves the absence of movable branching without assuming that the quadratic coefficient never vanishes.

<h4 id="painleve-determinateness-theorem">Painlevé determinateness theorem</h4>

↑ **Parent:** [Complex ordinary differential equation](#complex-ordinary-differential-equation)

For a first-order [ordinary differential equation](#ordinary-differential-equation) rational in the dependent variable, with coefficients [meromorphic](isolated-singularity.md#meromorphic-function) on the chosen independent-variable surface, [analytic continuation](complex-analysis.md#analytic-continuation) along an arc ending outside the fixed exceptional set has a definite limit in the [Riemann sphere](complex-analysis.md#riemann-sphere). Its movable singularities are [poles](isolated-singularity.md#pole) or [algebraic branch points](complex-analysis.md#algebraic-branch-point). To see the limiting assertion, the cluster set of a continuous lifted arc is connected and compact. Any cluster value where the vector field is [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) permits uniform local continuation by the [Picard-Lindelöf theorem](#picard-lindelof-theorem). Otherwise the cluster set lies in finitely many coefficient poles, so it is a singleton. At a pole of the vector field, the inverse equation is [holomorphic](complex-analysis.md#complex-differentiability-at-a-point); its solution has a finite-order critical point, giving a convergent root expansion. The reciprocal dependent variable handles infinity. Points where both reduced numerator and denominator vanish belong to the fixed exceptional set and are excluded from this argument.

#### Movable singularity of a complex differential equation

↑ **Parent:** [Complex ordinary differential equation](#complex-ordinary-differential-equation)

A solution has a movable singularity if its location varies with the initial data. For example $w'=w^2$ has solutions $w=-1/(z-c)$, whose [pole](isolated-singularity.md#pole) moves with $c$. The [Painlevé determinateness theorem](#painleve-determinateness-theorem) restricts movable singularities of first-order equations rational in the dependent variable to [poles](isolated-singularity.md#pole) and [algebraic branch points](complex-analysis.md#algebraic-branch-point).

#### Fixed singularity of a complex differential equation

↑ **Parent:** [Complex ordinary differential equation](#complex-ordinary-differential-equation)

A singular location is fixed if its position is determined by the coefficients, independently of the initial data. Not every solution must actually be singular there. For a rational first-order equation, coefficient poles and exceptional fibres where the reduced numerator and denominator have common zeros are included among the possible fixed locations.

#### Holomorphic dependence of ordinary differential equations on parameters

↑ **Parent:** [Complex ordinary differential equation](#complex-ordinary-differential-equation)

If the right-hand side and initial data are jointly [holomorphic](complex-analysis.md#complex-differentiability-at-a-point), the local solution is jointly [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) in its independent variable and parameters. On a smaller closed [polydisc](complex-geometry.md#polydisc), bound $|A|$ by $M$ and $|\partial_w A|$ by $L$. Choose $r$ so that $rM$ stays inside the dependent-variable disc and $rL<1$. The integral [contraction mapping](analysis.md#contraction-mapping) has jointly [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) iterates converging uniformly, so [locally uniform convergence of holomorphic functions](complex-analysis.md#locally-uniform-convergence-of-holomorphic-functions) proves the assertion. Shifting the dependent variable turns initial values into parameters.

### Periodic solution

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)

A solution with a period $T>0$. A nonconstant periodic solution of an autonomous system traces a [periodic orbit](dynamical-systems.md#periodic-orbit); constant equilibria are also periodic functions, so they must be excluded when asserting absence of periodic orbits.

### Variational equation

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)

Differentiating a smooth [characteristic flow map](partial-differential-equation.md#characteristic-flow-map) in its initial point gives this linear equation, with $Y(s)=I$. The [Liouville formula for a fundamental matrix](#liouville-formula-for-a-fundamental-matrix) then gives $\det Y(t)=\exp(\int_s^t\operatorname{div}b(r,X(r))\,dr)$. Incompressible [Hamiltonian flows](classical-mechanics.md#hamiltonian-flow) preserve [Lebesgue measure](measure-theory.md#lebesgue-measure) because this [divergence](calculus.md#divergence) vanishes.

### Osgood uniqueness criterion

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)

If a continuous nondecreasing modulus $\mu$ satisfies this divergence condition, an estimate $|b(t,x)-b(t,y)|\leq A(t)\mu(|x-y|)$ with locally integrable $A$ gives uniqueness of [characteristic curves](partial-differential-equation.md#characteristic-curve). Apply a regularized integral comparison to their separation. For the [log-Lipschitz modulus](topological-analysis.md#log-lipschitz-modulus), $\delta'(t)\leq A(t)\delta(1-\log\delta)$ gives $\delta(t)\leq\exp(1-(1-\log\delta(0))\exp(-\int_0^tA))$ while $\delta\leq1$. Zero initial separation stays zero. Unlike the usual linear [Gronwall inequality](probability-and-statistics.md#gronwall-inequality), this criterion allows non-Lipschitz vector fields.

### Distributional regularity of a constant-coefficient ordinary differential equation

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)

For a nonzero constant-coefficient polynomial differential operator in one variable, every homogeneous [distribution](distribution-theory.md#distribution-mathematical-analysis) solution is a [classical solution](partial-differential-equation.md#classical-solution), indeed analytic. Factor the [polynomial](polynomial.md) into powers of distinct [characteristic roots of a constant-coefficient differential equation](#characteristic-root-of-a-constant-coefficient-differential-equation). The [kernel decomposition for coprime polynomials](linear-operator-theory.md#kernel-decomposition-for-coprime-polynomials) reduces the equation to $(D-\lambda)^m v=0$, and [multiplication of a distribution by a smooth function](distribution-theory.md#multiplication-of-a-distribution-by-a-smooth-function) reduces this to $D^m(e^{-\lambda x}v)=0$. The fact that [a distribution with zero derivative is constant](distribution-theory.md#a-distribution-with-zero-derivative-is-constant), iterated, makes the latter distribution a [polynomial](polynomial.md) of degree less than $m$.

#### Coordinate-degenerate constant-coefficient differential equation

↑ **Parent:** [Distributional regularity of a constant-coefficient ordinary differential equation](#distributional-regularity-of-a-constant-coefficient-ordinary-differential-equation)

For a positive-order constant-coefficient [ordinary differential equation](#ordinary-differential-equation), the [kernel of multiplication by a coordinate](distribution-theory.md#kernel-of-multiplication-by-a-coordinate) gives $xP(D)u=0$ exactly when $P(D)u=C\delta_0$. Hence every solution is $u=v+CE$, where $P(D)v=0$ and $E$ is any [fundamental solution of a linear differential operator](distribution-theory.md#fundamental-solution-of-a-linear-differential-operator). Taking a [retarded fundamental solution of a constant-coefficient ordinary differential operator](distribution-theory.md#retarded-fundamental-solution-of-a-constant-coefficient-ordinary-differential-operator) shows that the extra freedom is a single jump in the derivative of order one below the operator order. The coordinate multiplies the already differentiated distribution: this is a different operator from $P(D)(xu)$.

#### Exponential polynomial solution of a constant-coefficient differential equation

↑ **Parent:** [Distributional regularity of a constant-coefficient ordinary differential equation](#distributional-regularity-of-a-constant-coefficient-ordinary-differential-equation)

If a degree-$n$ characteristic [polynomial](polynomial.md) has distinct [roots of a polynomial](polynomial.md#root-of-a-polynomial) $\lambda_j$ of multiplicities $m_j$, all homogeneous [distribution](distribution-theory.md#distribution-mathematical-analysis) solutions are the displayed combinations. There are $\sum_jm_j=n$ independent coefficients. Repeated [characteristic roots of a constant-coefficient differential equation](#characteristic-root-of-a-constant-coefficient-differential-equation) account for the polynomial factors multiplying exponentials; conjugate pairs give real sine and cosine combinations when real solutions are desired.

### Implicit solution

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)

A solution specified by a relation $F(x,y)=C$, instead of by an explicit graph $y=f(x)$. Differentiating the relation verifies its [ordinary differential equation](#ordinary-differential-equation). Where $F_y\ne0$, the [implicit function theorem](calculus.md#implicit-function-theorem) supplies a local graph; other points may require a different parameterization.

### Exact first-order ordinary differential equation

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)

An equation $P(x,y)+Q(x,y)y'=0$ is exact if $P\,dx+Q\,dy$ is an [exact differential form](differential-form.md#exact-differential-form): there is a potential $F$ with $F_x=P$ and $F_y=Q$. Its solution curves are levels $F=C$. For continuously differentiable coefficients, $P_y=Q_x$ suffices locally and globally on a [simply connected](algebraic-topology.md#simply-connected-space) domain. Global topology matters; a closed form on a punctured domain need not be exact.

### Continuous dependence of an ODE solution on parameters

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)

On a common compact solution domain, a right-hand side continuous in parameters and uniformly Lipschitz in the state yields continuous dependence of the solution on those parameters. The [Gronwall inequality](probability-and-statistics.md#gronwall-inequality) controls the difference of two solutions. A transverse zero of an event function persists under a small parameter change, which allows a simple stellar surface in the [Newtonian limit](general-relativity.md#newtonian-limit) to persist in relativistic models.

### Exponential relaxation time

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)

For a stable first-order linear equation $u'=-(u-u_\infty)/\tau$, the time $\tau>0$ is the interval over which a deviation from equilibrium decays by the factor $e^{-1}$. This is the dynamical exponential-decay sense, distinct from a Markov chain's spectral relaxation time.

### Initial value problem

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Initial_value_problem)

An initial value problem specifies an [ordinary differential equation](#ordinary-differential-equation) together with the state at a starting time. For a continuous [linear differential equation](#linear-differential-equation) $u'=A(t)u$, every prescribed finite vector $u_0$ at $t_0$ determines a unique solution on the coefficient interval. This is different from a [boundary value problem](#boundary-value-problem), which can prescribe values at distinct endpoints.

#### L2 initial condition

↑ **Parent:** [Initial value problem](#initial-value-problem)

An L2 initial condition specifies a square-integrable initial function up to equality almost everywhere. It need not have pointwise nodal values or classical derivatives. [L2-compatible initialization of grid data](finite-difference.md#l2-compatible-initialization-of-grid-data) uses bounded averaging or projection, and evolution estimates use the relevant [L2 norm](real-analysis.md#l2-norm).

### Degenerate ordinary differential equation

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)

A degenerate ordinary differential equation has a highest-derivative coefficient that vanishes somewhere in its domain. Its solutions can have lower regularity at that point than in the interior. A [boundary value problem](#boundary-value-problem) normally imposes endpoint values by continuous extension while requiring the differential equation in the interior. Requiring it pointwise at a degenerate endpoint with all derivatives finite can impose an extra condition and destroy existence. In a [square-root-degenerate endpoint layer](#square-root-degenerate-endpoint-layer), the product of a vanishing square-root coefficient with a diverging second derivative has a finite nonzero interior limit.

#### Continuation through a zero of the leading ODE coefficient

↑ **Parent:** [Degenerate ordinary differential equation](#degenerate-ordinary-differential-equation)

An equation $a(x)y''+b(x)y'+c(x)y=0$ can remain meaningful at a zero of $a$ even though its normalized [second-order linear differential equation](#second-order-linear-differential-equation) has singular coefficients. A global continuation problem must specify its solution regularity. Across a point where a homogeneous solution vanishes to second order, its coefficient may change in a piecewise $C^1$ continuation; requiring continuity of the second derivative can eliminate that freedom. The usual continuous-coefficient [uniqueness theorem for ordinary differential equations](analysis.md#uniqueness-theorem-for-ordinary-differential-equations) cannot simply be applied across such a point.

### Compact support solvability for a constant-coefficient ordinary differential equation

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)

Use $D=-i\partial_x$. For a nonzero one-variable [polynomial](polynomial.md) $P$ and $v\in\mathcal E'(\mathbb R)$, a compactly supported solution to $P(D)u=v$ exists exactly when $v$ annihilates every smooth solution of the transposed equation $P(-D)\varphi=0$. For simple roots $\alpha_j$, these test solutions span the exponentials $e^{-i\alpha_jx}$, so the condition is $\widehat v(\alpha_j)=0$. Dividing the entire transform by $P$ and applying [polynomial division preservation of exponential type](distribution-theory.md#polynomial-division-preservation-of-exponential-type) and the [Paley–Wiener–Schwartz theorem](distribution-theory.md#paley-wiener-schwartz-theorem) constructs the compactly supported solution. It is unique because an entire function killed by a nonzero polynomial must vanish identically. For a root of multiplicity $r$, the conditions become $\widehat v^{(k)}(\alpha)=0$ for $0\leq k<r$, corresponding to $x^ke^{-i\alpha x}$.

### Singular point of a differential equation

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)

### Dissipative vector field

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)

A real [vector field](calculus.md#vector-field) $f$ is dissipative in an [inner product](linear-algebra.md#inner-product) if

$$
\langle f(x)-f(y),x-y\rangle\leq0
$$

for all $x,y$. Two solutions of the [ordinary differential equation](#ordinary-differential-equation) $y'=f(y)$ satisfy

$$
\frac{d}{dt}\|x(t)-y(t)\|^2
=2\langle f(x(t))-f(y(t)),x(t)-y(t)\rangle\leq0.
$$

Thus their distance never increases. The linear case $f(y)=Ay$ recovers the [dissipative operator](functional-analysis.md#dissipative-operator) condition. [B-stability](numerical-analysis.md#b-stability) asks whether a [Runge-Kutta method](numerical-analysis.md#runge-kutta-method) preserves this contraction for every positive [step size](convex-optimization.md#step-size).

### Peano existence theorem

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Peano_existence_theorem)

A continuous finite-dimensional [vector field](calculus.md#vector-field) has a local solution through every initial point. The theorem asserts existence without uniqueness; local [Lipschitz continuity](real-analysis.md#lipschitz-continuity) supplies uniqueness through the [Picard-Lindelöf theorem](#picard-lindelof-theorem).

### Separable differential equation

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Separable_differential_equation)

A first-order ordinary differential equation is separable when it can be written as $g(y)\,dy=f(x)\,dx$. Integrating each side then gives an implicit solution, subject to any exceptional solutions lost during division.

#### Cubic logistic differential equation

↑ **Parent:** [Separable differential equation](#separable-differential-equation)

The substitution $z=y^{-2}$ turns the nonzero solutions into $\dot z=1-z$. Thus $y=\pm(1+Ke^{-t})^{-1/2}$ where the denominator is positive, together with $y=0$. The nonzero [equilibrium points](dynamical-systems.md#equilibrium-point-of-a-dynamical-system) $\pm1$ are attracting and $0$ is unstable. The sign of nonzero initial data is preserved.

### Nonlinear ordinary differential equation

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)

#### Ermakov-Pinney equation

↑ **Parent:** [Nonlinear ordinary differential equation](#nonlinear-ordinary-differential-equation)

This nonlinear [ordinary differential equation](#ordinary-differential-equation) governs the amplitude of a complex oscillator solution. Independent real solutions of $y''+p(x)y=0$ can be combined into a nonvanishing complex solution; its modulus satisfies the equation with $c$ equal to the squared [Wronskian](#wronskian). A real positive amplitude and a conserved phase flux give an exact representation, not merely a [WKB approximation](analysis.md#wkb-approximation).

##### Exact amplitude-phase equation

↑ **Parent:** [Ermakov-Pinney equation](#ermakov-pinney-equation)

Substitution of $y=Ae^{i\epsilon^{-1}\int\sigma dX}$ into $\epsilon^2y''+k^2y=0$ gives the displayed real amplitude equation and conserved imaginary-part flux. Conversely these equations produce an exact complex solution wherever $A\ne0$. The [WKB approximation](analysis.md#wkb-approximation) is obtained by expanding this exact system where $|k|$ stays positive.

#### Position-dependent damping

↑ **Parent:** [Nonlinear ordinary differential equation](#nonlinear-ordinary-differential-equation)

In $x\prime\prime+\epsilon f(x)x\prime+x=0$, the damping coefficient depends on the displacement. The oscillator energy $E=(x\prime^2+x^2)/2$ satisfies $E\prime=-\epsilon f(x)x\prime^2$. Positive $f$ dissipates energy and negative $f$ supplies it; a changing sign can select a stable amplitude. The [averaged amplitude for position-dependent damping](#averaged-amplitude-for-position-dependent-damping) measures the net effect over an oscillation.

#### Logistic differential equation

↑ **Parent:** [Nonlinear ordinary differential equation](#nonlinear-ordinary-differential-equation)

The logistic differential equation $y'=ry(1-y/K)$ has equilibria $0$ and $K$ and the nonconstant solutions

$$
y(x)=\frac{K}{1+Ce^{-rx}}.
$$

A nonlinear ordinary differential equation depends nonlinearly on the unknown function or its derivatives.

Its nonconstant solutions are [logistic functions](statistical-learning.md#logistic-function); the equation determines that family together with its equilibrium solutions.

##### Euler discretization of logistic growth

↑ **Parent:** [Logistic differential equation](#logistic-differential-equation)

The [Forward Euler method](numerical-analysis.md#euler-method) applied to the [logistic differential equation](#logistic-differential-equation) $y'=ry(1-ay)$ becomes the [logistic map](dynamical-systems.md#logistic-map) after $u=a(\lambda-1)y/\lambda$, $\lambda=1+r\Delta t$. The positive [equilibrium point](dynamical-systems.md#equilibrium-point-of-a-dynamical-system) of the [differential equation](differential-equation.md) has perturbations decaying as $e^{-rt}$. Its discrete [fixed-point multiplier](dynamical-systems.md#multiplier-of-a-periodic-orbit-of-an-iteration) is $1-r\Delta t=2-\lambda$: for $r\Delta t>2$, the discretization has an artificial oscillatory [instability](dynamical-systems.md#instability), leading initially to alternation on successive steps. This contrasts with the positive perturbation multiplier $e^{-r\Delta t}$ of the exact time-step map.

<h3 id="picard-lindelof-theorem">Picard-Lindelöf theorem</h3>

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Picard–Lindelöf_theorem)

A vector field that is continuous in time and locally [Lipschitz continuous](real-analysis.md#lipschitz-continuity) in the state variable gives a unique local solution to its initial-value problem. A solution extends while it remains in a compact subset of the vector field's domain.

#### Finite-dimensional continuation criterion

↑ **Parent:** [Picard-Lindelöf theorem](#picard-lindelof-theorem)

A maximal solution of a locally Lipschitz ordinary differential equation on a finite-dimensional space can end at a finite time only by leaving every compact subset of the vector field's domain. In particular, a bounded solution for an everywhere-defined vector field extends globally.

#### Bielecki norm method

↑ **Parent:** [Picard-Lindelöf theorem](#picard-lindelof-theorem)

On $C([a,b],X)$, an exponentially or polynomially weighted sup norm can make a Volterra integral operator contractive even when the ordinary sup norm does not. For integration from $1$ to $t$, the weight $t^{-c}$ gives contraction factor at most $Mb/(c+1)$ for an $M$-Lipschitz vector field.

### Finite-time blowup

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)

A solution has finite-time blowup when it becomes unbounded, or leaves every compact subset of its state space, as time approaches a finite endpoint of its maximal interval of existence.

### Linear differential equation

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_differential_equation)

A linear differential equation is linear in the unknown function and its derivatives.

#### Fuchsian linear differential system

↑ **Parent:** [Linear differential equation](#linear-differential-equation)

In a fixed frame, a first-order [linear differential equation](#linear-differential-equation) is Fuchsian at a finite point when its coefficient matrix has at most a [simple pole](isolated-singularity.md#simple-pole) there. Its residue is $R$. The global object is the matrix-valued one-form $A(z)\,dz$: in the coordinate $t=1/z$ its coefficient is $-t^{-2}A(1/t)$. A Fuchsian system has intrinsic [regular singular points](complex-analysis.md#regular-singular-point), but an intrinsically regular singular system may have higher-order coefficient poles in a different meromorphic frame.

##### Analytic solution at a maximal integer Fuchsian exponent

↑ **Parent:** [Fuchsian linear differential system](#fuchsian-linear-differential-system)

Suppose the [matrix](vector-space.md#matrix) $B$ is [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) at zero and $0$ is an [eigenvalue](linear-operator-theory.md#eigenvalue) of $R$. Let $m$ be the largest nonnegative integer for which $-m$ is an [eigenvalue](linear-operator-theory.md#eigenvalue) of $R$. Seek $F=z^m\sum_{n\geq0}h_nz^n$, with $h_0\in\ker(mI+R)$ nonzero. The [Frobenius method](complex-analysis.md#frobenius-method) gives $((m+n)I+R)h_n=-\sum_{j=0}^{n-1}B_jh_{n-1-j}$ for $n\geq1$, where scalar terms multiply the identity. Every left-hand [matrix](vector-space.md#matrix) is invertible by the choice of $m$. Its inverse is $O(1/n)$, so a scalar convergent majorant proves convergence of the series. This yields a nonzero analytic solution; it is necessarily nonconstant when $m>0$, but can be constant when $m=0$. For the displayed sign convention, indicial exponents are eigenvalues of $-R$.

##### Residue and monodromy of a constant Fuchsian system

↑ **Parent:** [Fuchsian linear differential system](#fuchsian-linear-differential-system)

A [fundamental matrix](#fundamental-matrix-of-a-linear-differential-equation) for $F'=RF/z$ on a chosen logarithm branch is $\exp(R\log z)$. A counterclockwise circuit changes the logarithm by $2\pi i$, giving the displayed [monodromy](complex-analysis.md#monodromy) matrix and the cyclic group it generates. Changing the solution basis conjugates the matrix. The residue eigenvalues exponentiate to the monodromy eigenvalues; the latter do not determine the former uniquely.

#### Fundamental matrix of a linear differential equation

↑ **Parent:** [Linear differential equation](#linear-differential-equation)

For a system of [linear differential equations](#linear-differential-equation) $u'=A(t)u$, a fundamental matrix has columns forming a [basis](vector-space.md#basis) of its solution space. It solves $X'=A(t)X$ and is invertible at every time in its interval. Every solution is $u(t)=X(t)c$ for a constant vector $c$: differentiating $X^{-1}u$ gives zero. Invertibility at one time implies invertibility throughout the interval by uniqueness of the [initial value problem](#initial-value-problem). This notion is distinct from a Markov-chain fundamental matrix or the projective-geometric matrix used in stereo vision.

##### Gauge transformation of a linear differential system

↑ **Parent:** [Fundamental matrix of a linear differential equation](#fundamental-matrix-of-a-linear-differential-equation)

Writing $Y=GZ$ with an invertible [matrix](vector-space.md#matrix)-valued function gives $Z'=\Lambda Z$ exactly when $\Lambda=G^{-1}AG-G^{-1}G'$. For a [formal power series](commutative-algebra.md#formal-power-series) transformation at an [irregular singular point](complex-analysis.md#irregular-singular-point), coefficient comparison recursively removes off-diagonal terms when leading diagonal [eigenvalues](linear-operator-theory.md#eigenvalue) are distinct. This is a differential-system change of frame, not specifically an electromagnetic gauge transformation.

###### Formal cubic-exponential two-by-two system

↑ **Parent:** [Gauge transformation of a linear differential system](#gauge-transformation-of-a-linear-differential-system)

For $D=\operatorname{diag}(1,-1)$, $A=D\lambda^2+\left(\begin{smallmatrix}0&U\\V&0\end{smallmatrix}\right)\lambda+\left(\begin{smallmatrix}d&P\\R&-d\end{smallmatrix}\right)$, the formal diagonal exponent has $h=d+UV/2$ and $\theta=(UR+VP)/2$. Matching the gauge equation gives the off-diagonal first coefficient $(-U/2,V/2)$ and the diagonal one $\rho D$, where $\rho=UV(d+h)/4-PR/2$. The second coefficient has diagonal entries $\rho^2/2-UV/8\pm h\theta/2$ and off-diagonal entries $(U\rho-P)/2,(V\rho+R)/2$. With $G_0=I$ and negative-index coefficients zero, the coefficient comparison is

$$
[D,G_m]=-A_1G_{m-1}-A_2G_{m-2}+G_{m-2}hD+G_{m-3}[\theta D-(m-3)I].
$$

Its diagonal equations at $m=2,3,4,5$ give $h,\theta,\rho$ and the second diagonal coefficient respectively. Its off-diagonal equations determine the next coefficients because the [commutator](lie-algebra.md#commutator) with $D$ multiplies the upper and lower entries by $2$ and $-2$. This proves the expansion and supplies the recursion for all higher orders. The generally nonzero $\theta$ supplies [formal monodromy](complex-analysis.md#formal-monodromy).

##### Liouville formula for a fundamental matrix

↑ **Parent:** [Fundamental matrix of a linear differential equation](#fundamental-matrix-of-a-linear-differential-equation)

If $\dot\Phi=A(t)\Phi$ and $\Phi(0)=I$, differentiation of the [determinant](linear-algebra.md#determinant) gives $\det\Phi(t)=\exp(\int_0^t\operatorname{tr}A(s)\,ds)$. For a planar [periodic orbit](dynamical-systems.md#periodic-orbit) this gives the nontrivial [Floquet multiplier](dynamical-systems.md#floquet-multiplier), since the tangent multiplier is one.

#### Floquet theory

↑ **Parent:** [Linear differential equation](#linear-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Floquet_theory)

For a continuous periodic coefficient matrix $A(t+L)=A(t)$, a [fundamental matrix](#fundamental-matrix-of-a-linear-differential-equation) $X$ for $X'=A(t)X$, normalized by $X(0)=I$, obeys $X(t+L)=X(t)X(L)$. The invertible matrix $X(L)$ has a complex [matrix logarithm](vector-space.md#matrix-logarithm); set $B=L^{-1}\log X(L)$ and $P(t)=X(t)e^{-tB}$. Since $X(L)=e^{LB}$ commutes with $B$, direct substitution gives $P(t+L)=P(t)$ and proves the factorization. A real logarithm is not required for this complex representation.

The [eigenvalues](linear-operator-theory.md#eigenvalue) of $X(L)$ are [Floquet multipliers](dynamical-systems.md#floquet-multiplier). All solutions are bounded for forward time when every multiplier has modulus at most one and those on the unit circle have no nontrivial [Jordan blocks](linear-operator-theory.md#jordan-block). In a real undamped second-order scalar equation with no first-derivative term, the monodromy determinant is one. Distinct conjugate unit-modulus multipliers give bounded solutions; a nontrivial Jordan block at multiplier $1$ or $-1$ gives an unbounded second solution even when one periodic or antiperiodic solution exists.

##### Floquet exponent

↑ **Parent:** [Floquet theory](#floquet-theory)

For a [Floquet multiplier](dynamical-systems.md#floquet-multiplier) $m\ne0$ of a period-$T$ linear variational equation, a Floquet exponent is any logarithmic rate $\rho$ satisfying the displayed relation. Its real part is uniquely $T^{-1}\log|m|$, while its imaginary part is defined modulo $2\pi/T$. Negative transverse real parts give local attraction to a [periodic orbit](dynamical-systems.md#periodic-orbit); the autonomous phase direction has multiplier one and exponent zero. Constant-coefficient amplitude equations supply exponents directly as the [eigenvalues](linear-operator-theory.md#eigenvalue) of their [Jacobian matrix](calculus.md#jacobian-matrix).

##### Floquet growth rate

↑ **Parent:** [Floquet theory](#floquet-theory)

The maximal asymptotic growth rate of a finite-dimensional periodic [linear differential equation](#linear-differential-equation) is $P^{-1}\log\rho(N)$, where $P$ is the coefficient period and $N$ the [monodromy matrix of a periodic linear system](#monodromy-matrix-of-a-periodic-linear-system). The [spectral radius](analysis.md#spectral-radius) selects the dominant [Floquet multiplier](dynamical-systems.md#floquet-multiplier). Generic initial data attain this rate; data lying entirely in other invariant subspaces can grow or decay at different rates.

##### Monodromy matrix of a periodic linear system

↑ **Parent:** [Floquet theory](#floquet-theory)

For $\dot Y=K(t)Y$ with coefficient period $P$, the monodromy matrix maps $Y(0)$ to $Y(P)$. Its [eigenvalues](linear-operator-theory.md#eigenvalue) are the [Floquet multipliers](dynamical-systems.md#floquet-multiplier). For piecewise constant coefficients it is the time-ordered product of the segment [matrix exponentials](linear-operator-theory.md#matrix-exponential), with the earliest segment on the right. Its determinant is $\exp(\int_0^P\operatorname{tr}K(t)\,dt)$.

#### Characteristic root of a constant-coefficient differential equation

↑ **Parent:** [Linear differential equation](#linear-differential-equation)

For the homogeneous [linear differential equation](#linear-differential-equation) $P(\partial_x)u=0$, a characteristic root is a [root of a polynomial](polynomial.md#root-of-a-polynomial) $P(r)=0$. A simple root supplies an exponential solution $e^{rx}$; a root of multiplicity $m$ supplies $x^je^{rx}$ for $0\leq j<m$. The sign of the [real part](complex-analysis.md#real-part) of $r$ determines spatial growth or decay.

#### Laplace contour-integral method for a linear differential equation

↑ **Parent:** [Linear differential equation](#linear-differential-equation)

The Laplace contour-integral method seeks a solution in the form

$$
w(z)=\int_\gamma e^{zt}f(t)\,dt.
$$

Replacing multiplication by $z$ with differentiation of $e^{zt}$ in $t$ and integrating by parts turns the differential equation for $w$ into a first-order equation for $f$. The contour $\gamma$ must make the resulting endpoint term vanish; finite endpoints are often branch points of $f$, while infinite ends must enter sectors where the exponential decays.

#### Homogeneous linear differential equation

↑ **Parent:** [Linear differential equation](#linear-differential-equation)

A homogeneous linear differential equation has zero forcing term. Its solutions are closed under addition and scalar multiplication.

##### Solution space of a homogeneous linear differential equation

↑ **Parent:** [Homogeneous linear differential equation](#homogeneous-linear-differential-equation)

The solutions of a homogeneous linear differential equation on a common domain form a [vector space](vector-space.md). For a regular scalar equation of order $n$, prescribing the first $n$ initial data at an ordinary point gives an isomorphism of this solution space with the scalar field to the power $n$.

#### Linearized equation

↑ **Parent:** [Linear differential equation](#linear-differential-equation)

A linearized equation retains terms first order in a perturbation about a reference solution. Its coefficients are determined by derivatives of the original nonlinear equation evaluated on that reference solution.

#### Inhomogeneous linear differential equation

↑ **Parent:** [Linear differential equation](#linear-differential-equation)

An inhomogeneous linear differential equation has a nonzero forcing term. Its general solution is one particular solution plus the general solution of the associated homogeneous equation.

### Local existence for a scalar autonomous ordinary differential equation with continuous vector field

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)

For continuous $\phi:\mathbb R\to\mathbb R$, the initial-value problem

$$
f'(t)=\phi(f(t)),
\qquad f(0)=0,
$$

has a local continuously differentiable solution. If $\phi(0)=0$, use the constant solution; otherwise locally invert $F(x)=\int_0^xdu/\phi(u)$.

### Singular perturbation

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Singular_perturbation)

A singular perturbation multiplies a highest derivative or otherwise changes the limiting equation's order when its small parameter is set to zero. It commonly separates fast and slow time scales.

#### Beyond-all-orders boundary-value sensitivity

↑ **Parent:** [Singular perturbation](#singular-perturbation)

A homogeneous mode can be order one inside an interval and exponentially small at an endpoint. Adjusting an endpoint value beyond all algebraic orders can then change the interior solution by order one. In the [nested layers at an essential singular endpoint](#nested-layers-at-an-essential-singular-endpoint) example, the mode $\exp(-x/\epsilon-2\epsilon^2/x)$ has this behavior: prescribed exact endpoint values give a unique solution for each fixed positive $\epsilon$, but leading asymptotic endpoint data do not select a unique bounded family.

#### Adiabatic elimination

↑ **Parent:** [Singular perturbation](#singular-perturbation)

[Adiabatic elimination](#adiabatic-elimination) replaces a rapidly relaxing variable by its instantaneous stable quasistatic value. If $\dot R=-\Gamma(t)R+P(t)$ with $\Gamma>0$, write $R=R_0+\delta R$, $R_0=P/\Gamma$. Then $\dot{\delta R}+\Gamma\delta R=-\dot R_0$. After the transient, $\delta R\simeq-\dot R_0/\Gamma$ when coefficients vary slowly compared with $\Gamma^{-1}$. This gives both the leading reduction and its time-scale error; rapid relaxation alone does not justify an additional Taylor expansion in another parameter.

#### Matched asymptotic expansion

↑ **Parent:** [Singular perturbation](#singular-perturbation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matched_asymptotic_expansion)

A matched asymptotic expansion constructs approximations in regions with different distinguished scalings and determines their free constants by requiring agreement in an overlap region.

##### Endpoint derivative in a negative-drift boundary layer

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

For $\epsilon y''-(1+x)y'+y=0$, $y(0)=1$, $y(1)=1+\epsilon$, the exact outer solution is $1+x$ and the mismatch is at the right endpoint. In $X=(1-x)/\epsilon$, matching gives $Y_0=2-e^{-2X}$ and $Y_1=-X+(1-X-X^2/2)e^{-2X}$. Differentiation at $X=0$ gives the displayed endpoint slope. The order-one term requires the first inner correction; differentiating only the leading boundary layer loses it.

##### Logistic crossover in a weakly nonlinear Euler equation

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

A growing linear mode can make a formally small [derivative](calculus.md#derivative) nonlinearity order one at large distance. After the crossover scaling, the equation $XH''-H'+(H')^2=0$ reduces to a [logistic differential equation](#logistic-differential-equation) in $\log X$ for $H'$. Matching $H\sim X^2/2$ at small $X$ gives $H'=X/(1+X)$ and the displayed primitive with $H(0)=0$. It changes from quadratic growth to linear growth without a finite turning singularity.

###### Nonlinear crossover delayed by a small unstable-mode coefficient

↑ **Parent:** [Logistic crossover in a weakly nonlinear Euler equation](#logistic-crossover-in-a-weakly-nonlinear-euler-equation)

When the early growing solution is $Ax^2$ and the nonlinear coefficient depends on $\varepsilon y'$, its crossover occurs at the displayed scale. If $A$ is order one this is $x=O(\varepsilon^{-1})$; if the initial slope suppresses the leading mode and $A=O(\varepsilon)$, it is delayed to $x=O(\varepsilon^{-2})$. The first nonzero perturbative seed must therefore be computed before constructing the global leading approximation; setting the small parameter to zero can erase the mode that ultimately dominates.

##### Nonlinear endpoint layer with a quadratic reaction

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

For $q>0$, matching $Y\to-q$, $Y'\to0$ fixes the [first integral](#first-integral) to $(Y')^2=(q-2Y)(Y+q)^2/3$. Hence endpoint values above $q/2$ cannot match this outer branch. The upper family is $Y=-q+(3q/2)\operatorname{sech}^2[\sqrt q(\xi-\xi_0)/2]$. An endpoint value strictly between $-q$ and $q/2$ admits two translations, one initially approaching $-q$ and one initially moving towards the turning value $q/2$. Values below $-q$ give the unique lower family $Y=-q-(3q/2)\operatorname{csch}^2[\sqrt q(\xi+\xi_0)/2]$ with $\xi_0>0$. Matching to zero instead gives $(Y')^2=-qY^2-2Y^3/3$, which forbids a nonconstant real approach to zero. These are leading [boundary layer](continuum-mechanics.md#boundary-layer) classifications, not exact multiplicity theorems at degenerate endpoint data.

###### One-third-power scaling at a nonlinear turning endpoint

↑ **Parent:** [Nonlinear endpoint layer with a quadratic reaction](#nonlinear-endpoint-layer-with-a-quadratic-reaction)

In $\epsilon y''+xy+y^2=0$, balancing all three terms where the outer branches $0$ and $-x$ meet gives the displayed [dominant balance](analysis.md#dominant-balance) and the inner equation $Y''+XY+Y^2=0$. Matching to $-X$ and writing $Y=-X+u$ gives $u''-Xu+u^2=0$. Its linearized decaying correction is an [Airy function](#airy-function); the growing correction is excluded. Matching to zero instead gives $Y''+XY=0$, whose nonzero [Airy function](#airy-function) combinations oscillate. Thus the acceptable matching branches differ qualitatively at the turning endpoint.

##### Asymptotic matching condition

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

An asymptotic matching condition requires the [inner expansion](#inner-expansion) and [outer expansion](#outer-expansion), re-expressed in a common overlap region, to agree to the retained order. Both function values and slopes may constrain the free constants. In the [square-root reaction problem with nested boundary layers](#square-root-reaction-problem-with-nested-boundary-layers), the shared small plateau sets the [first integral of a square-root reaction layer](#first-integral-of-a-square-root-reaction-layer), while its large-field fourth-power tail fixes the neighboring broad layer.

##### Square-root reaction problem with nested boundary layers

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

For fixed $k>0$ and endpoint values $y(0)=0$, $y(1)=1$, the [outer solution](#outer-expansion) is $y\sim\varepsilon^2k^2$. The left [boundary layer](continuum-mechanics.md#boundary-layer) has width $\varepsilon$. At the right, a layer of width $\sqrt\varepsilon$ carries the order-one rise, and a translated layer of width $\varepsilon$ connects its inner edge to the small plateau. The [dominant balance](analysis.md#dominant-balance) depends on both amplitude and derivative scale; using the same scale at both ends loses a necessary match.

###### First integral of a square-root reaction layer

↑ **Parent:** [Square-root reaction problem with nested boundary layers](#square-root-reaction-problem-with-nested-boundary-layers)

After $y=\varepsilon^2Y$ and $x=\varepsilon\xi$ or a translated version, the layer equation is $Y''-\sqrt Y+k=0$. Multiplying by $Y'$ and matching $Y=k^2$, $Y'=0$ fixes the energy constant to $k^3/3$ and gives the displayed factorization. The increasing branch below $k^2$ approaches it at positive infinity; the increasing branch above it leaves it at negative infinity and grows like $\xi^4/144$. This supplies both interfaces of the [square-root reaction problem with nested boundary layers](#square-root-reaction-problem-with-nested-boundary-layers).

##### Nested layers at an essential singular endpoint

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

Multiplication by $x^2$ makes this example exactly integrable once: $\epsilon x^2y\prime+(x^2-2\epsilon^3)y=C$. Its homogeneous solution is $\exp(-x/\epsilon-2\epsilon^2/x)$. A solution with $y(1)=\epsilon^3$ that remains uniformly bounded needs $C\sim\epsilon^3$, hence $y(0)\sim-1/2$. The scales $x=O(\epsilon)$ and $x=O(\epsilon^2)$ connect the small outer solution to the order-one endpoint value. Bounded homogeneous contributions remain invisible to algebraic matching at the right boundary.

##### Matched expansion with square-root and logarithmic corrections

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

A decaying algebraic tail in an inner [asymptotic expansion](analysis.md#asymptotic-expansion) can become a fractional-order outer correction after rescaling. For an inner tail proportional to $r^{-1/2}$ and outer variable $x=\epsilon r$, the outer correction is proportional to $\epsilon^{1/2}x^{-1/2}$. If the next outer correction contains $\epsilon\log x$, expressing it in the inner variable produces both $\epsilon\log r$ and $\epsilon\log\epsilon$. Omitting the latter loses a term larger than a plain $O(\epsilon)$ correction. Matching must include all these scales and constants, rather than only the leading algebraic powers.

##### Logarithmic matching in a small-exponent boundary layer

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

In a singular first-order equation with coefficient $x+\epsilon$, an outer correction proportional to $\epsilon\log x$ cannot be evaluated at the endpoint. The inner scale $x=\epsilon X$ changes it to $\epsilon\log\epsilon+\epsilon\log(1+X)$. Matching retains the logarithmic constant, which is larger than a plain order-epsilon correction. For $(x+\epsilon)y'=\epsilon y$, $y(1)=1$, the exact solution $[(x+\epsilon)/(1+\epsilon)]^\epsilon$ verifies the displayed endpoint asymptotic and its remainder.

##### Gaussian interior layer of a conservative drift equation

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

The equation $\epsilon y''+xy'+y=0$ integrates to $\epsilon y'+xy=C$. Equal endpoint data $y(-1)=y(1)=A$ force $C=0$ and give the unique Gaussian solution above. Its central width is $\sqrt\epsilon$, with amplitude $A e^{1/(2\epsilon)}$. The exponentially large central mode is missed by an assumed bounded algebraic [outer expansion](#outer-expansion) $C/x$. Changes of order one relative to either endpoint value occur over distance $O(\epsilon)$ from that endpoint.

##### Oscillatory endpoint with a quadratically vanishing drift

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

For $\epsilon y''+s^2y'+y=0$ on $s\geq0$, removing the drift by $y=e^{-s^3/(6\epsilon)}v$ gives

$$
\epsilon^2v''=(s^4/4+\epsilon s-\epsilon)v.
$$

The transformed potential changes sign at $s_t\sim\sqrt2\epsilon^{1/4}$. [WKB approximation](analysis.md#wkb-approximation) is oscillatory inside and exponential outside this turning region; an [Airy turning-point connection formula](analysis.md#airy-turning-point-connection-formula) applies over width $\epsilon^{5/12}$. At the endpoint the wavelength is $\sqrt\epsilon$, while the physical exponential prefactor changes on the envelope scale $\epsilon^{1/3}$. Balancing only diffusion and drift and declaring a single $\epsilon^{1/3}$ layer misses the zeroth-order term and the turning region. Matching constants may be singular at homogeneous boundary-value resonances.

##### First-order composite expansion for a positive drift

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

For $\epsilon y''+a(x)y'+b(x)y=0$ with smooth $a$ bounded positively away from zero, the first-order equation for the [outer expansion](#outer-expansion) is selected by the right [boundary condition](#boundary-condition). The left mismatch is repaired on the scale $\xi=x/\epsilon$. If $a(0)=a_0>0$, the leading inner transient is $B e^{-a_0\xi}$. Its next equation is $Y_1''+a_0Y_1'=-a'(0)\xi Y_0'-b(0)Y_0$. Matching its constant and linear large-$\xi$ terms to the [outer expansion](#outer-expansion) permits an order-$\epsilon$ composite approximation. A sign reversal of the drift places the transient at the opposite endpoint.

##### Logarithmically enhanced nonlinear boundary layer

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

If a leading [outer expansion](#outer-expansion) diverges as $\log x$ and a [derivative](calculus.md#derivative) coefficient contains $x-\varepsilon z$, balancing that nonlinear correction gives a layer larger than $O(\varepsilon)$. Write $x=\varepsilon L X$ with $L=\log(1/\varepsilon)$ and subtract the large negative constant from $z$. Matching often introduces a $\log L$ correction and yields an endpoint slope of order $1/(\varepsilon L)$. The balance must be derived from the actual equation; logarithmic divergence alone does not fix a universal layer width.

##### Boundary layer around a moving endpoint

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

For $\varepsilon xw''+w'+2xw=0$ with left endpoint $x=\varepsilon$, diffusion there is of size $\varepsilon^2$. The distinguished coordinate is $z=(x-\varepsilon)/\varepsilon^2$, giving $(1+\varepsilon z)W''+W'+2\varepsilon^3(1+\varepsilon z)W=0$. Matching to one with zero left value gives $W=1-e^{-z}-\varepsilon z(z+2)e^{-z}/2+O(\varepsilon^2)$. The layer width is different from the endpoint's distance from zero.

##### Square-root boundary layer at a vanishing drift

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

In $\varepsilon y''+2xy'-2xy=0$, the drift vanishes at the endpoint $x=0$. Balancing diffusion against drift gives the [inner expansion](#inner-expansion) coordinate $z=x/\sqrt\varepsilon$. The leading layer equation is $Y''+2zY'=0$, with a bounded [error function](calculus.md#error-function) profile. A regular outer first-order calculation alone cannot impose both endpoint values.

###### Error-function logarithmic switchback

↑ **Parent:** [Square-root boundary layer at a vanishing drift](#square-root-boundary-layer-at-a-vanishing-drift)

If an [outer expansion](#outer-expansion) contains $-(\varepsilon/2)\log x$ and the layer coordinate is $x=\sqrt\varepsilon z$, its overlap contains $-(\varepsilon/2)\log z-(\varepsilon/4)\log\varepsilon$. Matching forces an [inner expansion](#inner-expansion) term $-(\varepsilon/4)\log\varepsilon\operatorname{erf}z$ when that homogeneous profile tends to one in the overlap and vanishes at the boundary. The logarithm multiplies the matching profile, rather than an arbitrary constant.

##### Overlap region

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

An overlap region is a parameter-dependent range in which two neighboring [asymptotic expansions](analysis.md#asymptotic-expansion) have simultaneously ordered common limits. Between scales $\epsilon^2$ and $\epsilon$, it is $\epsilon^2\ll x\ll\epsilon$: the narrow coordinate tends to infinity while the wider coordinate tends to zero. Matching uses these limiting descriptions, not an assertion that either expansion is uniform at all values of the other's scaled variable.

##### Intermediate asymptotic region

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

An intermediate asymptotic region has a scale between two other scales and provides their connecting [matched asymptotic expansion](#matched-asymptotic-expansion). It can be needed because a coefficient changes its dominant form before the narrowest region's highest-derivative balance is reached. For example, a coefficient $x+\epsilon$ changes near $x=O(\epsilon)$ even when the fast [inner expansion](#inner-expansion) has width $O(\epsilon^2)$. The intermediate solution must be matched at both ends rather than assigned an independent boundary value.

##### Interior layer at a simple zero of advection

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

In $\varepsilon^2y''+a(x)y'+\cdots=f$, a simple zero $a(x_*)=0$, $a'(x_*)\ne0$, balances diffusion and advection on width $\varepsilon$. With $a(x)\simeq2(x-x_*)$, the leading homogeneous inner equation is $Y''+2zY'=0$, whose bounded solutions are constants and the [error function](calculus.md#error-function). Thus distinct order-one [outer solutions](#outer-expansion) can match across an interior transition. Reversing the diffusion sign makes the nonconstant homogeneous solution grow at both ends, changing the matching structure.

###### Endpoint layers for reversed diffusion

↑ **Parent:** [Interior layer at a simple zero of advection](#interior-layer-at-a-simple-zero-of-advection)

For $-\varepsilon^2y''+2(x-x_*)y'+\cdots=f$ on an interval straddling $x_*$, the bounded leading interior solution cannot connect unequal constants. A common bulk value is instead selected by an inner [solvability condition](linear-operator-theory.md#solvability-condition), and width-$\varepsilon^2$ endpoint layers enforce the two boundary values. At endpoints $x=0,2$ with $x_*=1$, their leading decaying factors are $e^{-2x/\varepsilon^2}$ and $e^{-2(2-x)/\varepsilon^2}$. The interior layer still corrects derivative mismatches at smaller amplitude.

##### Distinguished limit

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

A distinguished limit rescales variables so that two or more effects enter the leading asymptotic balance together. It identifies a region whose governing equation differs from the equations in adjacent scales.

##### Inner expansion

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inner_expansion)

An inner expansion resolves a region in which a stretched independent variable makes otherwise small effects enter the leading balance.

###### Square-root-degenerate endpoint layer

↑ **Parent:** [Inner expansion](#inner-expansion)

The [singular perturbation](#singular-perturbation) equation $\epsilon\sqrt x\,u''+u'=0$ balances its derivatives on the width $x=\epsilon^2X$. The inner equation is $\sqrt X\,U''+U'=0$, so $U'=Ce^{-2\sqrt X}$. Its solution with $U(0)=0$ and $U(\infty)=1$ is the displayed $H$, since $\int_0^\infty e^{-2\sqrt q}dq=1/2$. Near zero $H=2X-8X^{3/2}/3+O(X^2)$, so the first derivative is finite while the second is singular. Treat the differential equation on the open interval and impose the endpoint value by continuous extension.

###### Inner variable

↑ **Parent:** [Inner expansion](#inner-expansion)

An inner variable is a stretched coordinate such as $\xi=(x-x_0)/\delta(\epsilon)$ that remains order one inside a thin region of width $\delta(\epsilon)$.

##### Outer expansion

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Outer_expansion)

An outer expansion describes the solution away from a thin or distant inner region and is matched to the inner expansion in their common limit.

##### Additive composite expansion

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

An additive composite expansion combines inner and outer approximations by adding them and subtracting their common overlap. It is uniformly valid across both regions to the retained order.

##### Multiplicative composite expansion

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

When inner and outer approximations share a nonzero multiplicative overlap, a multiplicative composite divides their product by that common part. It is especially convenient when different regions contribute separate exponential or boundary-layer factors.

##### Outflow boundary layer

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

For $\epsilon y''+a(x)y'+b(x)y=0$ with $a>0$, the reduced first-order outer problem takes its boundary condition at the right endpoint. A rapidly decaying exponential in $x/\epsilon$ supplies the otherwise unsatisfied left-end condition, so the layer lies at the outflow end for the fast mode associated with this sign convention.

##### Switchback term

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

A switchback term such as $\epsilon\log\epsilon$ is forced into a matched expansion when logarithms of a stretched coordinate split into parameter-dependent and local pieces in the overlap region.

###### Logarithmic overlap creates a switchback term

↑ **Parent:** [Switchback term](#switchback-term)

If a stretched variable is $x=\epsilon r$ and an [outer expansion](#outer-expansion) contains $\epsilon^2\log x$, its expression in the fixed-$r$ region is $\epsilon^2\log r+\epsilon^2\log\epsilon$. The parameter logarithm must therefore be present in the [inner expansion](#inner-expansion), often multiplying a homogeneous solution selected by a boundary condition. An ansatz containing only integer powers with parameter-independent coefficients misses this [switchback term](#switchback-term). The same reasoning applies to other powers of $\epsilon$ and other stretched-coordinate scalings.

#### Method of multiple scales

↑ **Parent:** [Singular perturbation](#singular-perturbation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Method_of_multiple_scales)

The method of multiple scales treats fast and slow variables such as $t$ and $T=\epsilon t$ as independent, then removes resonant forcing to obtain slow amplitude and phase equations.

##### Slow oscillator damping by a relaxing auxiliary variable

↑ **Parent:** [Method of multiple scales](#method-of-multiple-scales)

For $x''+3\epsilon yx'+x=2(y')^2$ and $y'=\epsilon(1+x-y)$ with leading oscillation $x=A(\tau)\sin t$, $\tau=\epsilon t$, averaging the auxiliary equation gives $Y'=1-Y$. Cancellation of resonant forcing in the oscillator gives $2A'+3YA=0$. With $Y(0)=3$ and $A(0)=1$, $Y=1+2e^{-\tau}$ and the displayed amplitude follows. Bounded oscillatory corrections repair the instantaneous auxiliary equation; secular terms in a fixed-time expansion show why the slow scale is needed.

##### Averaged oscillator damping by a power of velocity

↑ **Parent:** [Method of multiple scales](#method-of-multiple-scales)

For $y''+\epsilon(y')^n+y=0$, the [method of multiple scales](#method-of-multiple-scales) gives no first-order phase drift. If $n$ is odd, the [amplitude](physics.md#wave-amplitude) obeys the displayed damping law with $C_n=2^{-(n+1)}\binom{n+1}{(n+1)/2}$. If $n$ is even, the average is zero and the amplitude is unchanged on the first slow time $T=\epsilon t$. The odd case dissipates [mechanical energy](classical-mechanics.md#mechanical-energy), whereas the even case is reversible and its force is not damping of both velocity signs.

##### Second-order resonance from quadratic oscillator coupling

↑ **Parent:** [Method of multiple scales](#method-of-multiple-scales)

Two fundamental harmonics of [frequency](physics.md#frequency) one multiply into only a constant and second harmonics. The first-order [solvability condition in the method of multiple scales](#solvability-condition-in-the-method-of-multiple-scales) therefore has no amplitude-changing resonant coupling. Their first-order particular corrections can mix back into the fundamental at second order, selecting the possible scale $t=O(\epsilon^{-2})$. Detuning may suppress the resulting [resonance](dynamical-systems.md#resonance), so identifying this scale alone does not prove instability for every initial state.

##### Averaged amplitude for position-dependent damping

↑ **Parent:** [Method of multiple scales](#method-of-multiple-scales)

For $x\prime\prime+\epsilon f(x)x\prime+x=0$, write $x_0=A(T)\cos(t+\theta)$ and $T=\epsilon t$. Removing [secular terms](#secular-term) gives $A_T=-A\langle f(A\cos\psi)\sin^2\psi\rangle$ and $\theta_T=0$, where the brackets mean a period average. This is the first-order [solvability condition in the method of multiple scales](#solvability-condition-in-the-method-of-multiple-scales), with a slowly evolving amplitude and no first-order frequency correction.

###### Absolute-value damping amplitude law

↑ **Parent:** [Averaged amplitude for position-dependent damping](#averaged-amplitude-for-position-dependent-damping)

For $x''+\varepsilon|x|x'+x=0$ and unit initial amplitude, averaging uses $\langle|\cos\psi|\sin^2\psi\rangle=2/(3\pi)$. Thus $A_T=-2A^2/(3\pi)$ and the displayed algebraic envelope follows. The leading phase has no first-order drift. The dissipation is amplitude dependent, so an exponential envelope with a constant decay rate would give the wrong long-time scale.

###### Van der Pol amplitude evolution

↑ **Parent:** [Averaged amplitude for position-dependent damping](#averaged-amplitude-for-position-dependent-damping)

For $x''+\varepsilon(x^2-1)x'+x=0$, the [averaged amplitude for position-dependent damping](#averaged-amplitude-for-position-dependent-damping) has the displayed logistic-type equation. With $A(0)=1$, its positive solution is $A(T)=2/\sqrt{1+3e^{-T}}$. Small amplitudes grow and large ones decay toward the stable value two; the leading oscillation is $A(\varepsilon t)\cos t$.

###### Shifted Van der Pol amplitude evolution

↑ **Parent:** [Van der Pol amplitude evolution](#van-der-pol-amplitude-evolution)

For $x''+\epsilon c(1-x^2)x'+x=k$, use $T=\epsilon t$ and $x=k-r(T)\cos(t+\phi(T))$. Removal of [secular terms](#secular-term) gives $\phi_T=0$ and the displayed [amplitude equation](dynamical-systems.md#amplitude-equation). With $R=r^2$, $R_T=c(k^2-1)R+(c/4)R^2$, which is explicitly integrable. If $c$ is replaced by a slowly varying coefficient $C(T)$, the same solution uses the accumulated time $\int_0^T C(s)\,ds$. The [method of multiple scales](#method-of-multiple-scales) is uniform on bounded slow-time intervals only while its [amplitude](physics.md#wave-amplitude) and correction estimates remain bounded.

###### Odd position-dependent damping has zero first-order amplitude drift

↑ **Parent:** [Averaged amplitude for position-dependent damping](#averaged-amplitude-for-position-dependent-damping)

If $f$ is odd, its average $\langle f(A\cos\psi)\sin^2\psi\rangle$ vanishes under a half-period shift. Hence the [averaged amplitude for position-dependent damping](#averaged-amplitude-for-position-dependent-damping) is constant at first order. Odd-power damping creates only even harmonics when multiplied by the leading oscillator velocity; these do not resonate with the fundamental harmonic. Higher-order drift is still possible.

##### Secular term

↑ **Parent:** [Method of multiple scales](#method-of-multiple-scales)

A secular term grows in a nominal perturbation correction and eventually invalidates an otherwise ordered expansion. In the [method of multiple scales](#method-of-multiple-scales), a solvability condition removes resonant forcing that would generate such growth.

##### Whitham modulation theory

↑ **Parent:** [Method of multiple scales](#method-of-multiple-scales)

Whitham modulation theory averages a variational wave equation over a fast periodic phase and derives slow equations for its local wavenumber, frequency, and amplitude.

###### Averaged Lagrangian

↑ **Parent:** [Whitham modulation theory](#whitham-modulation-theory)

The averaged Lagrangian is the phase average of a Lagrangian evaluated on a periodic wave profile. Variation with respect to profile parameters gives the local dispersion relation, while variation of the slow phase gives a modulation conservation law.

###### Modulated-wave first integral

↑ **Parent:** [Averaged Lagrangian](#averaged-lagrangian)

Multiplying a one-dimensional Euler--Lagrange wave equation by the derivative of its periodic profile with respect to fast phase produces a phase first integral plus slow divergence terms. Phase averaging removes the periodic derivative and yields the slow phase equation.

###### Whitham modulation equation

↑ **Parent:** [Averaged Lagrangian](#averaged-lagrangian)

For local wavenumber $k=\Theta_X$, frequency $\omega=-\Theta_T$, and averaged Lagrangian $\overline L(k,\omega,\ldots)$, slow-phase variation gives

$$
\partial_X\overline L_k-\partial_T\overline L_\omega=0.
$$

###### Wave-action density

↑ **Parent:** [Whitham modulation equation](#whitham-modulation-equation)

For an averaged Lagrangian, the wave-action density is $W=\partial\overline L/\partial\omega$, up to the sign convention used for the fast phase.

###### Wave-action conservation law

↑ **Parent:** [Wave-action density](#wave-action-density)

In a slowly varying conservative medium, wave action obeys a continuity equation with flux equal to wave-action density times group velocity.

##### Amplitude-phase equations for a weakly perturbed oscillator

↑ **Parent:** [Method of multiple scales](#method-of-multiple-scales)

For $u''+u=\epsilon f(u,u',\epsilon t)$, write $u_0=R(T)\cos(t+\phi(T))$ with $T=\epsilon t$. Removing resonant sine and cosine forcing gives

$$
R'=-\langle f\sin(t+\phi)\rangle,
\qquad
R\phi'=-\langle f\cos(t+\phi)\rangle.
$$

###### Oscillator coupled to slow damping feedback

↑ **Parent:** [Amplitude-phase equations for a weakly perturbed oscillator](#amplitude-phase-equations-for-a-weakly-perturbed-oscillator)

For $x''+x=-2\varepsilon yx'$ and $y'=\varepsilon g(x)$, the [method of multiple scales](#method-of-multiple-scales) gives the displayed [amplitude-phase equations](#amplitude-phase-equations-for-a-weakly-perturbed-oscillator), together with constant leading phase. For $g(x)=x$, $Y$ is constant and $R$ changes exponentially. For $g(x)=\log|x|$ and positive amplitude, the integrable phase average is $\log(R/2)$. Thus $L=\log(R/2)$ obeys $L_{TT}+L=0$ with $L_T=-Y$. The identically zero oscillator is inadmissible for logarithmic feedback, whose force is undefined there.

###### Velocity-only forcing in averaged oscillator equations

↑ **Parent:** [Amplitude-phase equations for a weakly perturbed oscillator](#amplitude-phase-equations-for-a-weakly-perturbed-oscillator)

When the weak force depends only on [velocity](classical-mechanics.md#velocity), the phase average is a periodic total [derivative](calculus.md#derivative) and vanishes. The leading phase is constant, while the amplitude evolves according to the remaining average. The sign of that drift determines damping or growth and must be checked from the force, rather than inferred from its [velocity](classical-mechanics.md#velocity) dependence alone.

###### Quadratically damped oscillator

↑ **Parent:** [Velocity-only forcing in averaged oscillator equations](#velocity-only-forcing-in-averaged-oscillator-equations)

For initial amplitude one, the [method of multiple scales](#method-of-multiple-scales) gives $x\simeq A(\epsilon t)\sin t$ with $A_T=-4A^2/(3\pi)$, hence $A=1/(1+4\epsilon t/(3\pi))$. Positive damping causes algebraic decay. Negative damping yields a formal finite-time amplitude pole, but the weak-damping assumption fails before it because $|\epsilon|A$ becomes order one. A leading approximation has order-$|\epsilon|$ displacement error on fixed slow-time intervals away from that pole.

###### Cubic velocity anti-damping

↑ **Parent:** [Velocity-only forcing in averaged oscillator equations](#velocity-only-forcing-in-averaged-oscillator-equations)

For $y''+y=\varepsilon(y')^3$ with positive $\varepsilon$, the oscillator [energy](classical-mechanics.md#energy) increases at rate $\varepsilon(y')^4$. The [amplitude-phase equations](#amplitude-phase-equations-for-a-weakly-perturbed-oscillator) give $R(T)=R_0(1-3R_0^2T/4)^{-1/2}$. The [weakly nonlinear expansion](#weakly-nonlinear-expansion) fails when the growing amplitude makes $\varepsilon R^2$ large, so its formal finite-time divergence does not itself control the exact late-time trajectory.

###### Conservative forcing in averaged oscillator equations

↑ **Parent:** [Amplitude-phase equations for a weakly perturbed oscillator](#amplitude-phase-equations-for-a-weakly-perturbed-oscillator)

For a weak force depending only on [position](classical-mechanics.md#position), the amplitude average is a periodic total [derivative](calculus.md#derivative) and vanishes. The leading harmonic amplitude is constant, while the phase may drift. The [method of multiple scales](#method-of-multiple-scales) agrees with the exact [conservation of energy](physics.md#conservation-of-energy) for bounded orbits in the effective potential. A cubic [position](classical-mechanics.md#position) force on the right side of the oscillator equation lowers the [frequency](physics.md#frequency) at first order when its coefficient is positive.

##### Slow time

↑ **Parent:** [Method of multiple scales](#method-of-multiple-scales)

A slow time resolves evolution occurring over many periods of a faster process. It is treated as an independent variable in the [method of multiple scales](#method-of-multiple-scales).

##### Weakly nonlinear expansion

↑ **Parent:** [Method of multiple scales](#method-of-multiple-scales)

A weakly nonlinear expansion writes a small disturbance as powers of an amplitude parameter while resolving its evolution on a [slow time](#slow-time). Near a critical [eigenvalue](linear-operator-theory.md#eigenvalue), linear detuning and nonlinear interactions enter the same perturbation order. The [Fredholm solvability condition for a self-adjoint operator](linear-operator-theory.md#fredholm-solvability-condition-for-a-self-adjoint-operator), or its adjoint form for a general operator, yields an [amplitude equation](dynamical-systems.md#amplitude-equation) without requiring the full higher-order correction.

###### Quadratic wave interaction

↑ **Parent:** [Weakly nonlinear expansion](#weakly-nonlinear-expansion)

A quadratic product of [plane waves](quantum-mechanics.md#plane-wave) generates sums and differences of their [wavenumbers](wave-equation.md#wavenumber) and [angular frequencies](classical-mechanics.md#angular-frequency). A component drives a [secular term](#secular-term) when its generated pair also satisfies the linear [dispersion relation](wave-equation.md#dispersion-relation). A [solvability condition in the method of multiple scales](#solvability-condition-in-the-method-of-multiple-scales) then determines the coupled [amplitude equations](dynamical-systems.md#amplitude-equation) on a [slow time](#slow-time).

###### Resonant three-wave triad

↑ **Parent:** [Quadratic wave interaction](#quadratic-wave-interaction)

Three [Fourier modes](fourier-analysis.md#fourier-mode) form a spatial resonance when their wavevectors sum to zero. Products of the conjugate second and third modes then force the first mode, with cyclic counterparts. Such terms couple both amplitudes and phases, unlike self-saturation terms proportional only to squared magnitudes. For three equal [wavenumbers](wave-equation.md#wavenumber), the vectors are separated by $120$ degrees and support hexagonal pattern interactions.

###### Detuning of a wave resonance

↑ **Parent:** [Quadratic wave interaction](#quadratic-wave-interaction)

Detuning measures the small mismatch from a [resonance condition](#resonance-condition). When the mismatch and nonlinear forcing are both $O(\epsilon)$, they enter the same [slow time](#slow-time) equation. A small shift of the [wavenumber](wave-equation.md#wavenumber) can therefore balance a quadratic interaction and permit a locked periodic [travelling wave](analysis.md#travelling-wave).

###### Phase matching for a quadratic wave interaction

↑ **Parent:** [Quadratic wave interaction](#quadratic-wave-interaction)

A resonant interaction requires matching both [wavenumber](wave-equation.md#wavenumber) and [angular frequency](classical-mechanics.md#angular-frequency): $k_3=k_1+k_2$ and $\omega_3=\omega_1+\omega_2$ for a sum interaction, with corresponding sign changes for differences. A common [phase velocity](wave-equation.md#phase-velocity) alone does not guarantee that a generated harmonic lies on the [dispersion relation](wave-equation.md#dispersion-relation).

###### Two-to-one resonance of dispersive waves

↑ **Parent:** [Phase matching for a quadratic wave interaction](#phase-matching-for-a-quadratic-wave-interaction)

A fundamental wave and its second harmonic satisfy [phase matching for a quadratic wave interaction](#phase-matching-for-a-quadratic-wave-interaction) when $\omega(2k)=2\omega(k)$. The square of the fundamental drives the second harmonic, while its product with the conjugate second harmonic drives the fundamental. Projecting these terms onto the resonant modes gives coupled [amplitude equations](dynamical-systems.md#amplitude-equation) rather than a uniformly valid correction at fixed amplitude.

###### Explosive two-to-one amplitude system

↑ **Parent:** [Two-to-one resonance of dispersive waves](#two-to-one-resonance-of-dispersive-waves)

For $A_T=-\overline AB/2$ and $B_T=-A^2/4$, write $A=Re^{i\theta}$, $B=Pe^{i\phi}$ and $\delta=\phi-2\theta$. The polar equations are

$$
R_T=-\frac{RP}2\cos\delta,\qquad \theta_T=-\frac P2\sin\delta,\qquad P_T=-\frac{R^2}4\cos\delta,\qquad \phi_T=\frac{R^2}{4P}\sin\delta.
$$

Where the polar phases are defined, direct [differentiation](calculus.md#differentiation) gives the [first integrals](#first-integral) $R^2-2P^2$ and $R^2P\sin\delta$. In particular $R^2\theta_T$ and $P^2\phi_T$ are constant. If $\delta=\pi$ and $R^2-2P^2=C>0$, then $P_T=P^2/2+C/4$, a [Riccati equation](analysis.md#riccati-equation) whose positive solution develops a finite-time pole. This is [finite-time blowup](#finite-time-blowup) of the reduced amplitude system; it does not establish blowup of the full wave equation beyond the domain of the [weakly nonlinear expansion](#weakly-nonlinear-expansion).

##### Harmonic balance

↑ **Parent:** [Method of multiple scales](#method-of-multiple-scales)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Harmonic_balance)

Harmonic balance substitutes a finite [Fourier series](fourier-series.md) into a differential equation and projects the residual onto the retained harmonics. It determines their amplitudes and phases. A nonlinear equation generally generates additional harmonics, so vanishing of the projected residual alone does not make the finite series an exact solution. In a [weakly nonlinear expansion](#weakly-nonlinear-expansion), nonresonant generated harmonics can be found at the next order by solving their linear equations.

##### Solvability condition in the method of multiple scales

↑ **Parent:** [Method of multiple scales](#method-of-multiple-scales)

At each perturbation order, the coefficient of a homogeneous oscillatory mode must vanish from the forcing to prevent secular growth. This solvability condition determines the slow evolution of lower-order amplitudes.

##### Parametric resonance

↑ **Parent:** [Method of multiple scales](#method-of-multiple-scales)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Parametric_resonance)

Parametric resonance occurs when periodic variation of a system parameter couples oscillatory modes and produces exponential amplitude growth. Multiple-scale solvability identifies the instability tongues and their detuning widths.

###### Primary instability tongue of a weak Mathieu oscillator

↑ **Parent:** [Parametric resonance](#parametric-resonance)

For $y''+(\omega^2+\epsilon\cos t)y=0$, use the [method of multiple scales](#method-of-multiple-scales) with $T=\epsilon t$ and $y_0=a(T)\cos(t/2)+b(T)\sin(t/2)$. Removing [secular terms](#secular-term) gives $a_T=(k-1/2)b$ and $b_T=-(k+1/2)a$. The slow [eigenvalues](linear-operator-theory.md#eigenvalue) satisfy $\lambda^2=1/4-k^2$, so an exponentially growing mode exists inside the displayed leading instability interval. At its leading endpoints the slow matrix is nilpotent; higher-order corrections are needed to determine the exact edges. [Floquet theory](#floquet-theory) distinguishes this exponential instability from algebraic growth at a repeated multiplier.

###### Primary parametric resonance of a two-to-one oscillator pair

↑ **Parent:** [Parametric resonance](#parametric-resonance)

For weak quadratic coupling between [frequencies](physics.md#frequency) one and two, the first oscillator's [complex amplitude](physics.md#complex-amplitude) can obey $2iA_T+\alpha A+b\overline A=0$ with a constant real second-oscillator amplitude $b$. In real coordinates this is a linear slow system with squared growth rate $(b^2-\alpha^2)/4$. Exponential amplification occurs when the modulation amplitude exceeds detuning, $|b|>|\alpha|$. The [method of multiple scales](#method-of-multiple-scales) is valid over bounded slow time while the physical amplitudes remain in the weak-coupling regime. At equality the slow matrix can have a [Jordan block](linear-operator-theory.md#jordan-block) and produce linear growth for some initial phases.

###### Second instability tongue of a weak Mathieu oscillator

↑ **Parent:** [Parametric resonance](#parametric-resonance)

For $u''+[1+\epsilon\sin t+\epsilon^2f]u=0$, the second parametric-instability tongue is $-1/12<f<5/12$ to leading order. Outside its closure every leading slow amplitude is oscillatory.

###### Slow amplitudes for the second Mathieu instability tongue

↑ **Parent:** [Second instability tongue of a weak Mathieu oscillator](#second-instability-tongue-of-a-weak-mathieu-oscillator)

For $x''+[1+\epsilon\cos t+f\epsilon^2]x=0$, let $T=\epsilon^2t$ and $x_0=a(T)\cos t+b(T)\sin t$. First-order forcing produces a constant and second harmonics, not a resonant harmonic. Their feedback at second order gives the displayed [solvability condition in the method of multiple scales](#solvability-condition-in-the-method-of-multiple-scales). The slow squared growth rate is $(f+1/12)(5/12-f)/4$. Consequently the leading instability interval is $-1/12<f<5/12$; outside its closure the slow amplitudes oscillate. The endpoints are degenerate and require the [fourth-order edges of the second Mathieu instability tongue](#fourth-order-edges-of-the-second-mathieu-instability-tongue) for exact small-parameter stability.

###### Fourth-order edges of the second Mathieu instability tongue

↑ **Parent:** [Second instability tongue of a weak Mathieu oscillator](#second-instability-tongue-of-a-weak-mathieu-oscillator)

For $u''+[1+k\epsilon^2+\epsilon\cos t]u=0$, set $t=2s$. The [Mathieu equation](#mathieu-equation) has $a=4+4k\epsilon^2$ and $q=-2\epsilon$. Near the value $4$, the orthonormal even [Fourier series](fourier-series.md) basis $1,\cos2s,\cos4s,\cos6s$ gives diagonal entries $0,4,16,36$ and adjacent couplings $\sqrt2q,q,q$. The odd basis $\sin2s,\sin4s,\sin6s$ gives diagonal entries $4,16,36$ and adjacent couplings $q,q$. Higher modes require at least six coupling steps to affect the root near $4$, so these truncations determine its coefficients through $q^4$.

Substituting $a=4+c_2q^2+c_4q^4$ into the two [characteristic polynomials](linear-operator-theory.md#characteristic-polynomial) and equating coefficients yields

$$
a_2=4+\frac5{12}q^2-\frac{763}{13824}q^4+O(q^6),\qquad
b_2=4-\frac1{12}q^2+\frac5{13824}q^4+O(q^6).
$$

Converting back gives the displayed gap edges with remainders $O(\epsilon^4)$ in $k$. In a fixed bounded neighborhood of this [parametric resonance](#parametric-resonance), the true unstable gap is $k_-<k<k_+$. The leading slow-amplitude calculation cannot decide exact stability at $k=-1/12$ or $5/12$; the fourth-order shifts put those fixed values just outside the gap for sufficiently small positive $\epsilon$. This does not provide a bound uniform in $\epsilon$ for their transient amplification.

### Lie point symmetry of an ordinary differential equation

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)

A Lie point symmetry is a local one-parameter transformation of the independent and dependent variables that maps solution graphs of a differential equation to solution graphs.

#### Prolongation of a vector field

↑ **Parent:** [Lie point symmetry of an ordinary differential equation](#lie-point-symmetry-of-an-ordinary-differential-equation)

For $V=\xi(x,u)\partial_x+\eta(x,u)\partial_u$, its prolongation to derivatives through order $n$ is

$$
\operatorname{pr}^{(n)}V
=V+\sum_{j=1}^n\eta^{(j)}\partial_{u^{(j)}},
\qquad
\eta^{(j)}=D_x\eta^{(j-1)}-u^{(j)}D_x\xi.
$$

It generates a symmetry of $\Delta=0$ exactly when $\operatorname{pr}^{(n)}V(\Delta)$ vanishes on the equation manifold.

Prolongation lifts a [vector field](calculus.md#vector-field) to the [jet bundle of maps](differential-geometry.md#jet-bundle-of-maps) so that its flow acts on derivatives of the dependent variables as well as on their values.

##### First prolongation

↑ **Parent:** [Prolongation of a vector field](#prolongation-of-a-vector-field)

For $V=\xi(x,u)\partial_x+\eta(x,u)\partial_u$, the first prolongation is

$$
\operatorname{pr}^{(1)}V
=V+\left[\eta_x+(\eta_u-\xi_x)u'-\xi_u(u')^2\right]\partial_{u'}.
$$

##### Jet space of a scalar ordinary differential equation

↑ **Parent:** [Prolongation of a vector field](#prolongation-of-a-vector-field)

The $n$th jet space for a scalar function $u(x)$ has local coordinates

$$
(x,u,u_x,u_{xx},\ldots,u^{(n)}).
$$

It records the value of a function and its derivatives through order $n$ at one point, allowing an order-$n$ [ordinary differential equation](#ordinary-differential-equation) to be treated as a hypersurface and a point transformation to act through its [prolongation of a vector field](#prolongation-of-a-vector-field).

###### Solution manifold

↑ **Parent:** [Jet space of a scalar ordinary differential equation](#jet-space-of-a-scalar-ordinary-differential-equation)

An ordinary differential equation $\Delta(x,u,u',\ldots,u^{(n)})=0$ defines a solution manifold in [jet space](#jet-space-of-a-scalar-ordinary-differential-equation). The prolonged graph of every classical solution lies in this manifold.

##### Lie-symmetry determining equation for a first-order ordinary differential equation

↑ **Parent:** [Prolongation of a vector field](#prolongation-of-a-vector-field)

For $u'=F(x,u)$, a point-symmetry generator $V=\xi\partial_x+\eta\partial_u$ must satisfy

$$
\eta_x+(\eta_u-\xi_x-F\xi_u)F-\xi F_x-\eta F_u=0.
$$

It follows by applying the [first prolongation](#first-prolongation) to $u'-F=0$ and restricting to its [solution manifold](#solution-manifold).

##### Second prolongation of the rotation generator for plane graphs

↑ **Parent:** [Prolongation of a vector field](#prolongation-of-a-vector-field)

The infinitesimal generator $V=u\partial_x-x\partial_u$ of rotations of the $(x,u)$ plane has second prolongation

$$
\operatorname{pr}^{(2)}V
=u\partial_x-x\partial_u
-(1+u_x^2)\partial_{u_x}
-3u_xu_{xx}\partial_{u_{xx}}.
$$

Consequently it preserves both $u_{xx}=0$ and $u_{xx}=(1+u_x^2)^{3/2}$, the equations for straight lines and consistently oriented unit-circle arcs.

##### Total derivative operator

↑ **Parent:** [Prolongation of a vector field](#prolongation-of-a-vector-field)

On jet coordinates,

$$
D_x=\partial_x+u'\partial_u+u''\partial_{u'}+\cdots.
$$

It differentiates a differential function along prolonged solution graphs.

##### Schwarzian derivative

↑ **Parent:** [Prolongation of a vector field](#prolongation-of-a-vector-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schwarzian_derivative)

For a thrice differentiable function with $u'\ne0$, the Schwarzian derivative is

$$
S[u]=\frac{u'''}{u'}-\frac32\left(\frac{u''}{u'}\right)^2.
$$

It vanishes exactly for fractional linear functions $u(x)=(ax+b)/(cx+d)$ on intervals where the denominator does not vanish. In a [two-dimensional conformal field theory](string-theory.md#two-dimensional-conformal-field-theory), it is the inhomogeneous term in the finite conformal transformation of a stress-energy tensor with nonzero central charge.

###### Prolongations of the projective vector fields on the line

↑ **Parent:** [Schwarzian derivative](#schwarzian-derivative)

For $u_j=u^{(j)}$, the $n$th [prolongations](#prolongation-of-a-vector-field) of the translation, dilation, and special projective generators acting on the independent variable are

$$
\begin{aligned}
\operatorname{pr}^{(n)}(\partial_x)
&=\partial_x,\\
\operatorname{pr}^{(n)}(x\partial_x)
&=x\partial_x-\sum_{j=1}^n j u_j\partial_{u_j},\\
\operatorname{pr}^{(n)}(x^2\partial_x)
&=x^2\partial_x-\sum_{j=1}^n
\bigl(2jx u_j+j(j-1)u_{j-1}\bigr)\partial_{u_j}.
\end{aligned}
$$

###### Projective transformation weights of the Schwarzian derivative

↑ **Parent:** [Schwarzian derivative](#schwarzian-derivative)

For $V_1=\partial_x$, $V_2=x\partial_x$, and $V_3=x^2\partial_x$, direct application of their third [prolongations](#prolongation-of-a-vector-field) gives

$$
\operatorname{pr}^{(3)}V_1(S)=0,
\qquad
\operatorname{pr}^{(3)}V_2(S)=-2S,
\qquad
\operatorname{pr}^{(3)}V_3(S)=-4xS.
$$

Thus the Schwarzian is invariant under translation and has weight minus two under dilation; the third identity is its infinitesimal projective transformation law.

##### Affine-scaling symmetry of u double prime equals u prime squared over u minus u squared

↑ **Parent:** [Prolongation of a vector field](#prolongation-of-a-vector-field)

The vector fields $(cx+d)\partial_x-2cu\partial_u$ generate

$$
(x,u)\longmapsto(\lambda x+a,\lambda^{-2}u).
$$

Their second prolongations multiply the differential equation by $-4c$, so they are infinitesimal Lie symmetries.

### Boundary value problem

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boundary_value_problem)

A boundary value problem asks for a differential-equation solution satisfying conditions at more than one point or boundary component.

#### Neumann boundary-value problem

↑ **Parent:** [Boundary value problem](#boundary-value-problem)

A [boundary value problem](#boundary-value-problem) with prescribed outward [normal derivative](differential-geometry.md#normal-derivative), or the associated weighted flux, on the boundary. Its boundary data are [Neumann boundary data](#neumann-boundary-data). For an elliptic divergence-form operator without a zeroth-order term, integration over the domain imposes a compatibility condition between total source and boundary flux. A connected domain generally leaves a constant undetermined, fixed by a mean or reference value.

#### Boundary trace of a function

↑ **Parent:** [Boundary value problem](#boundary-value-problem)

For a sufficiently regular [function](function.md) on a domain $\Omega$, its boundary trace is the restriction to $\partial\Omega$, using the limit from within the domain when necessary. In a half-line evolution problem, the traces $f_j(t)=\partial_x^ju(0,t)$ are boundary values of the spatial [derivatives](calculus.md#derivative). An initial value does not generally determine every such trace without the [partial differential equation](partial-differential-equation.md) and suitable [boundary conditions](#boundary-condition). The [Sobolev trace operator](sobolev-space.md#trace-operator) extends classical restriction continuously to appropriate [Sobolev spaces](sobolev-space.md), where pointwise values need not be defined.

#### Oblique derivative boundary condition

↑ **Parent:** [Boundary value problem](#boundary-value-problem)

An oblique derivative boundary condition prescribes a linear combination of the outward [normal derivative](differential-geometry.md#normal-derivative) and the tangential [derivative](calculus.md#derivative) on a boundary. Its strictly oblique case has a nonzero normal coefficient; a zero normal coefficient is a limiting tangential condition. Both trace directions must be tracked when constructing a [global relation](#global-relation-for-a-linear-boundary-value-problem). On unbounded domains, regularity at corners and a growth condition at infinity are separate parts of an admissible [boundary value problem](#boundary-value-problem).

##### Corner compatibility for collinear oblique derivative data

↑ **Parent:** [Oblique derivative boundary condition](#oblique-derivative-boundary-condition)

For a solution with a continuous [gradient](calculus.md#gradient) at a quadrant corner, the prescribed derivative directions are $( -\sin\beta_1,\cos\beta_1)$ and $(\cos\beta_2,-\sin\beta_2)$. When $\beta_1+\beta_2=\pi/2$, these vectors are negatives of one another. Their corner data must therefore be opposite. Imposing $h_1(0)=h_2(0)$ as well forces both to vanish. Smooth decay of separate boundary functions alone does not ensure this local [compatibility condition for an overdetermined linear system](integrable-systems.md#compatibility-condition-for-an-overdetermined-linear-system).

// Target: analysis.bigb

##### Rational-angle oblique derivative problem on a quadrant

↑ **Parent:** [Oblique derivative boundary condition](#oblique-derivative-boundary-condition)

For a complex-valued [harmonic function](partial-differential-equation.md#harmonic-function) in the first quadrant, write $\Phi=q_z$ and $\Psi(\bar z)=q_{\bar z}$ as independent [holomorphic functions](complex-analysis.md#holomorphic-function). Prescribe $i(e^{i\beta_1}\Phi-e^{-i\beta_1}\Psi)=g_1$ on the imaginary axis and $e^{-i\beta_2}\Phi+e^{i\beta_2}\Psi=g_2$ on the real axis. If $\beta_1+\beta_2=n\pi/2$, set $\epsilon=(-1)^n$. Reflection into four quadrants produces a scalar [Riemann-Hilbert problem](#riemann-hilbert-problem) with parity $H(-z)=-\epsilon H(z)$ and known jumps. Provided its corner and large-arc contributions vanish, the [Cauchy integral formula](analysis.md#cauchy-integral-formula) gives

$$
\Phi(z)=\frac1{2\pi i}\left[e^{i\beta_2}\int_0^\infty g_2(s)\left(\frac1{s-z}-\frac\epsilon{s+z}\right)ds-e^{-i\beta_1}\int_0^\infty g_1(s)\left(\frac1{is-z}-\frac\epsilon{is+z}\right)ds\right].
$$

Complex boundary data do not justify replacing $q_{\bar z}$ by the conjugate of $q_z$.

###### Quarter-plane oblique boundary spectral functions

↑ **Parent:** [Rational-angle oblique derivative problem on a quadrant](#rational-angle-oblique-derivative-problem-on-a-quadrant)

For real [harmonic](partial-differential-equation.md#harmonic-function) $q$, prescribe $-\sin\beta_1q_x+\cos\beta_1q_y=h_1$ on the vertical axis and $\cos\beta_2q_x-\sin\beta_2q_y=h_2$ on the horizontal axis. Their orthogonal derivatives $j_1,j_2$ determine the missing gradient components. If $H_1,J_1$ use the kernel $e^{ky}$ and $H_2,J_2$ use $e^{-ikx}$, the clockwise spectra $\widehat q_1=\int_0^{i\infty}e^{-ikz}q_z\,dz$, $\widehat q_2=-\int_0^\infty e^{-ikz}q_z\,dz$ have the displayed expressions. Their [global relation](#global-relation-for-a-linear-boundary-value-problem) is $\widehat q_1+\widehat q_2=0$ in the third spectral quadrant.

// Target: analysis.bigb

###### Single-function spectral elimination for a rational-angle quadrant

↑ **Parent:** [Quarter-plane oblique boundary spectral functions](#quarter-plane-oblique-boundary-spectral-functions)

Reality of the boundary derivatives gives $H_1(\bar k)=\overline{H_1(k)}$ and $H_2(-\bar k)=\overline{H_2(k)}$, and the same identities for $J_1,J_2$. The [global relation](#global-relation-for-a-linear-boundary-value-problem) and its conjugate express both [quarter-plane oblique boundary spectral functions](#quarter-plane-oblique-boundary-spectral-functions) in terms of the known $H_1,H_2$ and the single bounded [holomorphic function](complex-analysis.md#holomorphic-function) $\Phi$ in the upper half-plane. For $\gamma=\beta_1+\beta_2\in\{0,\pi/2,\pi\}$, its coefficients on the positive real and positive imaginary reconstruction rays are opposite, because $e^{4i\gamma}=1$. Closing the first-quadrant contour removes $\Phi$ by the [Cauchy integral theorem](complex-analysis.md#cauchy-s-integral-theorem).

// Target: analysis.bigb

###### Homogeneous corner ambiguity in a quadrant Laplace problem

↑ **Parent:** [Rational-angle oblique derivative problem on a quadrant](#rational-angle-oblique-derivative-problem-on-a-quadrant)

For tangential data with $\beta_1=\beta_2=0$, the [harmonic function](partial-differential-equation.md#harmonic-function) $q=xy$ has zero prescribed data on both axes but a growing nonzero derivative. For normal data with $\beta_1=\beta_2=\pi/2$, $q=\log|z|$ also has zero prescribed data, and $q_z=1/(2z)$ decays at infinity but is singular at the corner. Thus decay of the data, and even decay of the solution gradient, does not alone determine the quadrant representation. Requiring the reflected gradient to decay at infinity and satisfy $|z|H(z)\to0$ at the corner removes both examples. Without such conditions, add homogeneous [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) terms obeying the reflection parity.

#### Dirichlet-to-Neumann map

↑ **Parent:** [Boundary value problem](#boundary-value-problem)

Given a uniquely solvable [Dirichlet problem](analysis.md#dirichlet-problem), this map sends prescribed [Dirichlet boundary data](#dirichlet-boundary-data) to the solution's outward [normal derivative](differential-geometry.md#normal-derivative). It depends on the differential operator and domain. Spectral [global relations](#global-relation-for-a-linear-boundary-value-problem) offer one way to compute it numerically from boundary traces, while a finite collocation scheme still requires a rank and conditioning check.

##### Semistrip Dirichlet-to-Neumann sine transforms

↑ **Parent:** [Dirichlet-to-Neumann map](#dirichlet-to-neumann-map)

In the [semistrip Laplace spectral global relation](#semistrip-laplace-spectral-global-relation), reality makes $W(\pm\kappa)$ real for $\kappa>0$. Its imaginary parts at those two arguments remove the unknown vertical-side [normal derivative](differential-geometry.md#normal-derivative). With $G_j^s(\kappa)=\int_0^\infty\sin(\kappa x)g_j(x)\,dx$ and $S_j(\kappa)=\int_0^\infty\sin(\kappa x)q_y(x,j)\,dx$, the result is

$$
S_0=\frac{\kappa[-\cosh(\kappa l)G_0^s+G_l^s+\int_0^l\sinh(\kappa(l-y))h(y)\,dy]}{\sinh(\kappa l)},\qquad
S_l=\frac{\kappa[-G_0^s+\cosh(\kappa l)G_l^s-\int_0^l\sinh(\kappa y)h(y)\,dy]}{\sinh(\kappa l)}.
$$

The lower outward [normal derivative](differential-geometry.md#normal-derivative) is $-q_y$, so its [Dirichlet-to-Neumann map](#dirichlet-to-neumann-map) coefficient is $-S_0$, whereas the upper coefficient is $S_l$.

// Target: analysis.bigb

#### Riemann-Hilbert problem

↑ **Parent:** [Boundary value problem](#boundary-value-problem)

Find functions analytic on the two sides of a contour whose boundary values obey a prescribed jump, with suitable normalization at infinity and other distinguished points. An additive jump $J$ on a counterclockwise closed contour is solved by the [Cauchy integral formula](analysis.md#cauchy-integral-formula) $F(k)=(2\pi i)^{-1}\int J(\zeta)/(\zeta-k)d\zeta$, subject to the normalization and compatibility conditions. The [Sokhotski–Plemelj theorem](complex-analysis.md#sokhotski-plemelj-theorem) verifies the jump.

##### Sectorial half-line mKdV Riemann-Hilbert reconstruction

↑ **Parent:** [Riemann-Hilbert problem](#riemann-hilbert-problem)

Use the bounded columns supplied by [Volterra analyticity sectors for reverse-dispersion mKdV](integrable-systems.md#volterra-analyticity-sectors-for-reverse-dispersion-mkdv) and divide the necessary columns by their determinants. This gives a normalized meromorphic matrix on the six-ray contour $\arg k=m\pi/3$. The constant [scattering data](integrable-systems.md#scattering-data) connection matrices generate its jumps by conjugation with $e^{i(kx-4k^3t)\sigma_3}$. Zeros of column determinants require residue conditions; in a sufficiently small-data, zero-free regime only jumps are needed. The off-diagonal expansion coefficient reconstructs $q=-2i\lim_{k\to\infty}kM_{12}$ for this sign convention.

##### Half-line NLS Riemann-Hilbert reconstruction

↑ **Parent:** [Riemann-Hilbert problem](#riemann-hilbert-problem)

Combine columns of the three normalized [Lax pair](integrable-systems.md#lax-pair) eigenfunctions in their common [Volterra analyticity sectors for a half-line NLS Lax pair](integrable-systems.md#volterra-analyticity-sectors-for-a-half-line-nls-lax-pair), dividing by the relevant determinants $a,d,d^\sharp,a^\sharp$. The resulting matrix is normalized to the identity at infinity and has jumps on the real and imaginary axes. Connection matrices determine each jump explicitly. Zeros of those determinants require residue conditions or local contour deformations.

##### Negative-index scalar Riemann-Hilbert moment conditions

↑ **Parent:** [Riemann-Hilbert problem](#riemann-hilbert-problem)

Suppose a scalar canonical factor has exterior growth $X_-(z)\sim z^q$ with index $-q<0$, and the original exterior unknown must decay as $O(z^{-1})$. Dividing by the canonical factor gives an additive jump $D_+-D_-=g$ with exterior decay $O(z^{-q-1})$. The exterior [Cauchy integral](complex-analysis.md#cauchy-transform) expands in moments $-\int_Lt^jg(t)dt/(2\pi iz^{j+1})$. Its first $q$ coefficients must therefore vanish, yielding the displayed solvability conditions. Under this decay there is no nonzero entire [polynomial](polynomial.md) addition. A nonlocal moment appearing in $g$ must additionally agree with the moment of the reconstructed original jump.

##### Matrix NLS reconstruction from a normalized Riemann-Hilbert problem

↑ **Parent:** [Riemann-Hilbert problem](#riemann-hilbert-problem)

Assume a regular invertible normalized [Riemann-Hilbert problem](#riemann-hilbert-problem) solution $\mu=I+\mu_1/k+\mu_2/k^2+\cdots$ with jump tending to the identity and conjugated by $e^{-i(kx+2k^2t)\sigma_3}$. Residuals of its two differential equations have no jump and vanish at infinity, so [Liouville theorem](complex-analysis.md#liouville-theorem) gives a [Lax pair](integrable-systems.md#lax-pair). Coefficient comparison gives the displayed reconstruction and $A=2Q$; compatibility yields $iQ_t-Q_{xx}\sigma_3+2Q^3\sigma_3=0$. A jump matrix tending to zero instead is inconsistent with the normalization. Recovering the initial jump from a prescribed initial potential still requires direct scattering.

##### Canonical factorization of a rational scalar Riemann-Hilbert jump

↑ **Parent:** [Riemann-Hilbert problem](#riemann-hilbert-problem)

A rational jump with no zeros or poles on the contour can be split into factors analytic and nonvanishing on the two sides. The exterior factor may carry a power of $z$ recording the winding number. For a circle enclosing $0,\pm1$, the jump $G=z/(z^2-1)$ has the canonical factors $X_+=1$, $X_-=z-z^{-1}$. The exterior growth of $X_-$ imposes compatibility conditions when a Cauchy transform is required to vanish at infinity.

#### Wiener-Hopf method

↑ **Parent:** [Boundary value problem](#boundary-value-problem)

The Wiener-Hopf method solves a [boundary value problem](#boundary-value-problem) with complementary half-line traces by [Wiener-Hopf factorization](#wiener-hopf-factorization) and additive splitting into upper- and lower-half-plane analytic functions. Analytic continuation gives a common entire function, whose growth and edge conditions determine its admissible value.

##### Mixed Dirichlet-Neumann half-plane diffraction

↑ **Parent:** [Wiener-Hopf method](#wiener-hopf-method)

For a scalar wave above a line with a Dirichlet half and a Neumann half, the boundary transform factors into $\beta_+(\alpha)=\sqrt{k+\alpha}$ and $\beta_-(\alpha)=\sqrt{k-\alpha}$. For $e^{-i\omega t}$, the [limiting absorption principle](gravity-wave.md#limiting-absorption-principle) puts $-k$ below and $k$ above the inversion contour. With Dirichlet conditions on the negative half-line and incident tangential wavenumber $a$, pole subtraction gives the diffracted trace $U_+=2i\sqrt{k-a}/[(\alpha+a)\sqrt{k+\alpha}]$. Its large-transform decay gives a bounded field with a square-root edge trace. The normal derivative has an inverse-square-root singularity on the Dirichlet half; it is identically zero on the Neumann half.

##### Wiener-Hopf factorization

↑ **Parent:** [Wiener-Hopf method](#wiener-hopf-method)

The plus factor is analytic and nonzero above the transform contour, and the minus factor below it. Their continuations inherit singularities and zeros in the opposite half-planes. Allocation of branch cuts and modal poles must agree with the physical outgoing continuation; no factor may have a zero inside its designated analytic domain.

##### Wiener-Hopf equation

↑ **Parent:** [Wiener-Hopf method](#wiener-hopf-method)

A scalar Wiener-Hopf equation couples two [Half-range Fourier transforms](analysis.md#half-range-fourier-transform) analytic in complementary half-planes. After dividing by a kernel factor, additive splitting separates the known forcing. Source poles, boundary terms and contour prescriptions are part of the problem data.

###### Wiener-Hopf kernel

↑ **Parent:** [Wiener-Hopf equation](#wiener-hopf-equation)

The scalar coefficient multiplying an unknown half-line transform in a [Wiener-Hopf equation](#wiener-hopf-equation) is its kernel. This is a transform-domain [function](function.md), distinct from the [null space](linear-algebra.md#kernel-of-a-linear-map) of a [linear map](vector-space.md#linear-map). Its analytic zeros, [poles](isolated-singularity.md#pole) and [winding number](complex-analysis.md#winding-number) govern [Wiener-Hopf factorization](#wiener-hopf-factorization). For mixed scalar Helmholtz half-plane diffraction a typical kernel is the outgoing vertical [wavenumber](wave-equation.md#wavenumber) $\sqrt{k^2-\alpha^2}$.

###### Pole subtraction in a Wiener-Hopf equation

↑ **Parent:** [Wiener-Hopf equation](#wiener-hopf-equation)

A forcing pole can be split between analytic half-planes by subtracting a factor's value at the pole. For instance,

$$
\frac{L^+(k)}{k+k_0}=\frac{L^+(-k_0)}{k+k_0}
+\frac{L^+(k)-L^+(-k_0)}{k+k_0}.
$$

The second quotient has a removable pole and belongs to the plus expression; the first keeps the prescribed minus-side forcing pole. After [Wiener-Hopf factorization](#wiener-hopf-factorization), analytic continuation identifies an entire remainder, whose value is fixed by growth and edge conditions. The pole prescription must be stated together with the [Fourier transform](analysis.md#fourier-transform) convention.

#### Fokas method

↑ **Parent:** [Boundary value problem](#boundary-value-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fokas_method)

The Fokas method uses a [global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem) between transformed boundary traces, complex spectral symmetries, and [contour integration](complex-analysis.md#contour-integration) to eliminate unknown traces or construct a numerical boundary scheme. The distinction between the domains of analyticity of the transforms and the decay sectors of spectral exponentials controls valid contour deformations.

##### Two-trace half-line cubic dispersion representation

↑ **Parent:** [Fokas method](#fokas-method)

For $q_t+q_x-q_{xxx}=0$ on $x>0$, its [local relation](#local-relation) has flux $(1+k^2)q-ikq_x-q_{xx}$. With $Q_0(k)=\int_0^\infty e^{-ikx}q(x,0)dx$ and $G_j(k,T)=\int_0^T e^{w(k)s}\partial_x^jq(0,s)ds$, its [global relation](#global-relation-for-a-linear-boundary-value-problem) is $e^{wT}\widehat q=Q_0+(1+k^2)G_0-ikG_1-G_2$. In $D_+=\{\operatorname{Im}k>0,\operatorname{Re}w(k)<0\}$, choose the other cubic root $\nu(k)$ in the lower half-plane. Then the known spectral density is $-Q_0(\nu)+(k^2-\nu^2)G_0-i(k-\nu)G_1$. The remaining final-state transform has zero integral around $\partial D_+$ by the [Cauchy integral theorem](complex-analysis.md#cauchy-s-integral-theorem) and exponential decay. The full boundary includes the real axis and the hyperbola $\operatorname{Im}k=\sqrt{1+3(\operatorname{Re}k)^2}$, oriented with the domain on the left.

##### Boundary spectral representation of a holomorphic function on a semistrip

↑ **Parent:** [Fokas method](#fokas-method)

For a [holomorphic function](complex-analysis.md#holomorphic-function) on $x>0$, $0<y<l$, define boundary spectra by counterclockwise traversal: $\rho_L=\int_{il}^0e^{-ikw}f(w)\,dw$, $\rho_B=\int_0^\infty e^{-ikx}f(x)\,dx$, and $\rho_T=-e^{kl}\int_0^\infty e^{-ikx}f(x+il)\,dx$. The displayed reconstruction follows from the [Cauchy integral formula](analysis.md#cauchy-integral-formula) and the ray identity $\int_0^{e^{i\theta}\infty}e^{ik(z-w)}\,dk=i/(z-w)$ whenever that exponential decays. The three rays are selected by the inward normals of the three sides.

// Target: analysis.bigb

##### Quadrant modified Helmholtz spectral reconstruction

↑ **Parent:** [Fokas method](#fokas-method)

For $\lambda>0$, put $a=k-\lambda/k$, $b=k+\lambda/k$. The spectral integral uses the positive real and positive imaginary rays, both oriented outward. On the first ray its density is $\rho_x=i\int_0^\infty e^{-iax}[bq(x,0)-q_y(x,0)]dx$; on the second it is $\rho_y=\int_0^\infty e^{by}[a q(0,y)-i q_x(0,y)]dy$. The [global relation](#global-relation-for-a-linear-boundary-value-problem) $\rho_x+\rho_y=0$ holds in the third spectral quadrant. Primitives from the corner and from each infinite boundary end give an additive [Riemann-Hilbert problem](#riemann-hilbert-problem). Their limits are $-q$ at infinity and $q$ at zero, which explains the factor $1/(4\pi i)$.

##### Neumann spectral formula for half-line constant drift

↑ **Parent:** [Fokas method](#fokas-method)

The reflected [global relation](#global-relation-for-a-linear-boundary-value-problem) expresses the unknown value trace in terms of the prescribed derivative trace. Multiplying the [half-line drift null contour identity](analysis.md#half-line-drift-null-contour-identity) by $(ik+\alpha)/(ik)$ removes the reflected time-dependent transform. Its pole at $k=0$ lies below the contour and is not crossed. The formula concerns the derivative $q_x(0,t)$, rather than the outward derivative $-q_x(0,t)$.

##### Dirichlet spectral formula for half-line constant drift

↑ **Parent:** [Fokas method](#fokas-method)

Let $I_C[F]=(2\pi)^{-1}\int_Ce^{ikx-(k^2-i\alpha k)t}F(k)dk$. The [drift-diffusion half-line global relation](#drift-diffusion-half-line-global-relation) and the [half-line drift null contour identity](analysis.md#half-line-drift-null-contour-identity) give the formula in the secondary title. Its real-space kernel is the difference of two drifted [Gaussian heat kernels](diffusion-equation.md#gaussian-heat-kernel), and its boundary-forcing kernel is $x(2\sqrt\pi t^{3/2})^{-1}\exp[-(x+\alpha t)^2/(4t)]$. This kernel is an [approximate identity](fourier-analysis.md#approximate-identity) in time as $x\downarrow0$, which verifies the [Dirichlet boundary condition](#dirichlet-boundary-condition).

##### Local relation

↑ **Parent:** [Fokas method](#fokas-method)

A spectral-parameter-dependent divergence identity equivalent to a partial differential equation. Integrating it over a space-time region gives a [global relation](#global-relation-for-a-linear-boundary-value-problem) between transformed initial and boundary data. For the half-line free [Schrödinger equation](physics.md#schrodinger-equation), take $P=e^{-ikx+ik^2t}q$ and $Q=e^{-ikx+ik^2t}(-kq+iq_x)$.

##### Dispersion symmetry elimination of a boundary trace

↑ **Parent:** [Fokas method](#fokas-method)

To eliminate an unknown boundary transform by a [dispersion relation](wave-equation.md#dispersion-relation) symmetry, evaluate the [global relation](#global-relation-for-a-linear-boundary-value-problem) at $\nu(k)$ only where the spatial transform remains analytic. Substitute the resulting trace identity into the contour representation. An unwanted transform vanishes only if its transformed argument and exponential admit a valid [contour deformation](complex-analysis.md#contour-deformation) and decay estimate. For constant drift, $\nu(k)=i\alpha-k$ maps the upper domain $\operatorname{Re}(k^2-i\alpha k)<0$ into the lower transform half-plane.

###### Cubic-dispersion elimination of one missing boundary trace

↑ **Parent:** [Dispersion symmetry elimination of a boundary trace](#dispersion-symmetry-elimination-of-a-boundary-trace)

For the [backward-sign Airy half-line global relation](integrable-systems.md#backward-sign-airy-half-line-global-relation), suppose exactly one trace of derivative order $j\in\{0,1,2\}$ is unknown. Its spectral multiplier is a constant times $k^r$, $r=2-j$. Use the [rotated null contours for half-range Fourier inversion](analysis.md#rotated-null-contours-for-half-range-fourier-inversion) with the displayed coefficients. The unknown contribution becomes an integral over the boundary of the middle upper sector $\pi/3<\arg k<2\pi/3$. There $\operatorname{Im}k^3<0$, so

$$
e^{-ik^3t}F_j(k,t)=\int_0^t e^{-ik^3(t-s)}f_j(s)\,ds
$$

is bounded, while $e^{ikx}$ decays exponentially. The [Cauchy integral theorem](complex-analysis.md#cauchy-s-integral-theorem) therefore removes that entire unknown contribution. The resulting solution depends on the initial transform and the two prescribed boundary transforms only.

// Target: analysis.bigb

###### Cubic Stokes dispersion symmetry

↑ **Parent:** [Dispersion symmetry elimination of a boundary trace](#dispersion-symmetry-elimination-of-a-boundary-trace)

For the [linear dispersive Stokes equation](integrable-systems.md#linear-dispersive-stokes-equation), $\omega(\nu)=\omega(k)$ factors as $(\nu-k)(\nu^2+k\nu+k^2-1)=0$. In $D_+=\{\operatorname{Im}k>0,\operatorname{Re}\omega(k)<0\}$ the two displayed other roots lie in the lower half-plane, so both can be used in the [global relation](#global-relation-for-a-linear-boundary-value-problem). To check the root locations, at $k=ib$ they have imaginary part $-b/2$. A root could reach the real axis only where $\operatorname{Re}\omega(k)=0$, so continuity preserves their signs throughout this connected domain. The branch points $\pm2/\sqrt3$ lie outside its closure. The weights $A_1=(k-\nu_2)/(\nu_1-\nu_2)$ and $A_2=(\nu_1-k)/(\nu_1-\nu_2)$ obey $A_1+A_2=1$ and $\nu_j'=-A_j$.

##### Upper-quadrant cancellation of reflected boundary transforms

↑ **Parent:** [Fokas method](#fokas-method)

If $P(k)$ is analytic in the upper half-plane with suitable growth, paired integrals along the positive real and imaginary rays cancel when their exponential is $e^{ik(x+iy)}$ with $x,y>0$. For $0<y<\ell$, the analogous pair along the imaginary and negative real rays cancels with $e^{ik(x+i(y-\ell))}$. These two applications of the [Cauchy integral theorem](complex-analysis.md#cauchy-s-integral-theorem) eliminate reflected unknown transforms from a strip [global relation](#global-relation-for-a-linear-boundary-value-problem); an individual ray integral need not vanish.

#### Global relation for a linear boundary value problem

↑ **Parent:** [Boundary value problem](#boundary-value-problem)

A global relation is an identity connecting transforms or integrals of the boundary traces of a solution. For a formally self-adjoint operator $L=\Delta-k^2$, [Green second identity](partial-differential-equation.md#green-second-identity) gives

$$
\int_{\partial\Omega}(v\partial_nu-u\partial_nv)\,ds=0
$$

for every homogeneous adjoint solution $Lv=0$. Exponential adjoint families turn this into a spectral identity between the [Dirichlet boundary condition](#dirichlet-boundary-condition) and unknown [normal derivative](differential-geometry.md#normal-derivative).

##### Dirichlet spectral formula for Airy flow with negative transport

↑ **Parent:** [Global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem)

Let $F(k)=\int_0^\infty e^{-ikx}q_0(x)dx$ and $G_0(k,t)=\int_0^t e^{w(k)s}g_0(s)ds$. Using the roots of [cubic dispersion symmetry with negative transport](integrable-systems.md#cubic-dispersion-symmetry-with-negative-transport), put $\mathcal T F=[(k-\nu_2)F(\nu_1)+(\nu_1-k)F(\nu_2)]/(\nu_1-\nu_2)$. The [Fokas method](#fokas-method) formula is an initial real-line integral minus an integral over $\partial D_+$ of $e^{ikx-wt}[\mathcal TF+(3k^2+1)G_0]$, both divided by $2\pi$. The boundary is oriented with $D_+$ on the left. Its unknown final-state transform has zero integral by analyticity and upper-half-plane decay.

##### Finite-interval Airy global relation

↑ **Parent:** [Global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem)

For the [Airy equation](integrable-systems.md#airy-equation) $q_t+q_{xxx}=0$ on $0<x<L$, define $F_j=\int_0^t e^{-ik^3s}\partial_x^jq(0,s)ds$ and $G_j$ analogously at $L$. Set $\mathcal F=k^2F_0-ikF_1-F_2$ and $\mathcal G=k^2G_0-ikG_1-G_2$. Integrating the [local relation](#local-relation) with flux $-q_{xx}-ikq_x+k^2q$ proves the displayed [global relation](#global-relation-for-a-linear-boundary-value-problem). The [dispersion relation](wave-equation.md#dispersion-relation) is invariant under multiplication of $k$ by a cube root of unity; the resulting three equations determine the three missing boundary transforms for data $q(0,t),q(L,t),q_x(L,t)$.

###### Finite-interval Airy spectral determinant

↑ **Parent:** [Finite-interval Airy global relation](#finite-interval-airy-global-relation)

Here $\alpha=e^{2\pi i/3}$. The missing-trace matrix has determinant $-\sqrt3k\Delta(k)$. Its nonzero zeros are the [eigenvalues](linear-operator-theory.md#eigenvalue) in the parametrization $Av=ik^3v$ of $A=-d^3/dx^3$ with $v(0)=v(L)=v'(L)=0$. [Integration by parts](calculus.md#integration-by-parts) gives $\operatorname{Re}\langle v,Av\rangle=-|v'(0)|^2/2$. No nonzero zero lies in $\operatorname{Re}(-ik^3)\leq0$: on its boundary the determinant equation reduces, after rotation, to an equality between a unit-modulus exponential and $\cosh u-i\sqrt3\sinh u$, whose modulus exceeds one unless $u=0$. The zero at the origin is removable in the original boundary problem. There are nevertheless infinitely many genuine negative [eigenvalues](linear-operator-theory.md#eigenvalue) of $A$, obtained from $e^{-3s/2}=2\cos(\sqrt3s/2+\pi/3)$, $s>0$, with $k=-is/L$. Absence of contour poles in the [Fokas method](#fokas-method) does not imply absence of [discrete spectrum](functional-analysis.md#discrete-spectrum) of the operator.

##### Semistrip Laplace spectral global relation

↑ **Parent:** [Global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem)

Let $q$ be a real [harmonic function](partial-differential-equation.md#harmonic-function) in a semistrip, $g_0(x)=q(x,0)$, $g_l(x)=q(x,l)$ and $h(y)=q(0,y)$. Let $G_j,N_j$ be the negative-exponential [Half-range Fourier transforms](analysis.md#half-range-fourier-transform) of $g_j$ and $q_y(x,j)$, and put $H(k)=\int_0^l e^{ky}h(y)\,dy$, $W(k)=\int_0^l e^{ky}q_x(0,y)\,dy$. The [closed differential form](differential-form.md#closed-differential-form) $e^{-ikz}q_z\,dz$ has zero boundary integral. [Integration by parts](calculus.md#integration-by-parts) of tangential derivatives cancels all corner values and gives the displayed [global relation](#global-relation-for-a-linear-boundary-value-problem), for $\operatorname{Im}k\leq0$.

// Target: analysis.bigb

##### Drift-diffusion half-line global relation

↑ **Parent:** [Global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem)

For $q_t=q_{xx}+\alpha q_x$ on $x>0$, write $Q(k)=\int_0^\infty e^{-ikx}q(x,0)dx$ and $G_j(k,t)=\int_0^t e^{\omega(k)s}\partial_x^jq(0,s)ds$. Twice integrating by parts gives $e^{\omega(k)t}\widehat q(k,t)=Q(k)-G_1(k,t)-(ik+\alpha)G_0(k,t)$ in the lower transform half-plane. The [dispersion relation](wave-equation.md#dispersion-relation) is invariant under $k\mapsto i\alpha-k$. This [global relation](#global-relation-for-a-linear-boundary-value-problem) eliminates one unknown boundary trace after the symmetry maps the inversion contour into the transform's analytic domain.

##### Half-line linear dispersive Stokes global relation

↑ **Parent:** [Global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem)

For the [linear dispersive Stokes equation](integrable-systems.md#linear-dispersive-stokes-equation) $q_t+q_x+q_{xxx}=0$, let $\omega(k)=i(k-k^3)$. Its [local relation](#local-relation) is obtained with $X=q_{xx}+ikq_x+(1-k^2)q$. Integrating $\partial_t(e^{-ikx+\omega t}q)+\partial_x(e^{-ikx+\omega t}X)=0$ over the half-line gives the displayed [global relation](#global-relation-for-a-linear-boundary-value-problem), with negative-exponential [Half-range Fourier transforms](analysis.md#half-range-fourier-transform) and $G_j(k,t)=\int_0^t e^{\omega(k)s}\partial_x^jq(0,s)\,ds$. The spatial transforms are [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) for $\operatorname{Im}k<0$, whereas the finite-time boundary transforms are [entire functions](complex-analysis.md#entire-function).

###### Dirichlet spectral representation for the linear dispersive Stokes equation

↑ **Parent:** [Half-line linear dispersive Stokes global relation](#half-line-linear-dispersive-stokes-global-relation)

Let $A_j$ be the weights of the [cubic Stokes dispersion symmetry](#cubic-stokes-dispersion-symmetry) and set $F(k)=\sum_jA_j(k)\widehat q_0(\nu_j(k))$. Orient $\partial D_+$ with $D_+$ on its left. Evaluating the [global relation](#global-relation-for-a-linear-boundary-value-problem) at its two lower-half-plane roots and interpolating the linear expression $ikG_1+G_2$ removes both unknown boundary traces. The resulting [Fokas method](#fokas-method) formula is

$$
q(x,t)=\frac1{2\pi}\int_{\mathbb R}e^{ikx-\omega t}\widehat q_0(k)\,dk+\frac1{2\pi}\int_{\partial D_+}e^{ikx-\omega t}\bigl[(1-3k^2)G_0(k,t)-F(k)\bigr]dk.
$$

The discarded transform of the solution is [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) in $D_+$ and has zero [integral](calculus.md#integral) after closing its [contour](complex-analysis.md#complex-integration-contour) for $x>0$. Initial compatibility and sufficient smoothness and spatial decay are required. At the boundary, use a fixed time horizon later than $t$ before [Fourier inversion](fourier-analysis.md#fourier-inversion-theorem), to avoid an endpoint half-value.

##### Half-line Schrodinger boundary-trace elimination

↑ **Parent:** [Global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem)

Orient the upper-quadrant contour from $i\infty$ down to zero and then to $+\infty$. The reflected half-line transform has zero inverse contribution for positive $x$. Adding $c$ times this contribution, and deforming boundary integrands through the second quadrant where $|e^{ikx-ik^2(t-\tau)}|\leq e^{-x\operatorname{Im}k}$, gives boundary coefficients $(1-c)k\widetilde g_0-i(1+c)\widetilde g_1$. Thus $c=-1$ removes the unknown Neumann trace for a prescribed Dirichlet value, while $c=1$ removes the unknown Dirichlet trace for a prescribed Neumann value. The initial reflected term has coefficient $c$ and cannot be discarded after the time-dependent spectral decomposition.

##### Finite-time spectral boundary transform

↑ **Parent:** [Global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem)

A boundary trace transformed over a finite time interval using the [dispersion relation](wave-equation.md#dispersion-relation) of a linear [partial differential equation](partial-differential-equation.md). For integrable trace data and a polynomial dispersion function, it is an [entire function](complex-analysis.md#entire-function) of the complex [spectral parameter](integrable-systems.md#spectral-parameter). Its growth depends on $\operatorname{Re}\omega(k)$; multiplying by $e^{-\omega(k)t}$ changes the integrand to the causal factor $e^{-\omega(k)(t-s)}$.

###### Finite-horizon extension of a boundary transform

↑ **Parent:** [Finite-time spectral boundary transform](#finite-time-spectral-boundary-transform)

In a [Fokas method](#fokas-method) boundary [integral](calculus.md#integral) over $\partial D_+$, where $\operatorname{Re}\omega<0$ inside, the contribution of replacing $G(k,t)$ by $G(k,T)$ is an [integral](calculus.md#integral) of $e^{ikx}\int_t^T e^{\omega(k)(s-t)}g(s)\,ds$ times an [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) coefficient. For $x>0$ it vanishes by the [Cauchy integral theorem](complex-analysis.md#cauchy-s-integral-theorem) and the exponential decay in the upper domain. The transformed amplitude is then independent of the observation time, which simplifies differentiation of the [partial differential equation](partial-differential-equation.md). Temporal inversion at $0<t<T$ recovers the full boundary value rather than the half-value of a truncated transform at its endpoint.

##### Polygonal modified Helmholtz global relation

↑ **Parent:** [Global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem)

For $u_{z\bar z}=\beta^2u$, pull back its spectral [closed differential one-form](differential-form.md#closed-differential-one-form) along each straight side $z=m_j+sh_j$. Under counterclockwise traversal and outward [normal derivatives](differential-geometry.md#normal-derivative) $q_j$, the side density is $i e^{-i\beta(\lambda z-\bar z/\lambda)}[|h_j|q_j+\beta(\lambda h_j+\bar h_j/\lambda)g_j]$, where $g_j$ is the [Dirichlet boundary data](#dirichlet-boundary-data). The [Generalized Stokes theorem](differential-form.md#generalized-stokes-theorem) gives the displayed [global relation](#global-relation-for-a-linear-boundary-value-problem). Clockwise traversal reverses the normal-derivative coefficient; all orientations must be changed consistently.

###### Dirichlet reconstruction in an equilateral triangle

↑ **Parent:** [Polygonal modified Helmholtz global relation](#polygonal-modified-helmholtz-global-relation)

For equal oriented [Dirichlet boundary data](#dirichlet-boundary-data) on all three sides and a uniquely solvable elliptic problem, rotation invariance makes their outward [normal derivatives](differential-geometry.md#normal-derivative) equal. Pairing the global relation with its [Schwarz conjugation of a spectral function](complex-analysis.md#schwarz-conjugation-of-a-spectral-function) at $\ell(k+\lambda/k)=2\pi in$ determines every Fourier coefficient of the common normal trace. The zero mode at $\lambda=0$ follows from zero total flux. At negative parameters, uniqueness and possible removable spectral denominators must be checked rather than assumed.

##### Half-line drift global relation

↑ **Parent:** [Global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem)

For the [advection-diffusion equation](diffusion-equation.md#advection-diffusion-equation) $u_t=u_{xx}+\alpha u_x$ on $x>0$, the spectral [divergence form](analysis.md#divergence-form) uses $\omega=k^2-i\alpha k$ and factor $e^{-ikx+\omega t}$. With negative-exponential [Half-range Fourier transforms](analysis.md#half-range-fourier-transform), integration gives the displayed [global relation](#global-relation-for-a-linear-boundary-value-problem) for $\operatorname{Im}k\le0$. The boundary transform $G_1$ refers to $u_x(0,t)$, the negative of the outward [normal derivative](differential-geometry.md#normal-derivative).

###### Exponential-decay contour for half-line drift diffusion

↑ **Parent:** [Half-line drift global relation](#half-line-drift-global-relation)

For $q_t=q_{xx}+\alpha q_x$ with $\alpha>0$, the [dispersion relation](wave-equation.md#dispersion-relation) is $\omega=k^2-i\alpha k$ and its symmetry is $\nu=i\alpha-k$. On the upper domain $\operatorname{Re}\omega<0$, $\operatorname{Im}k>\alpha$ and therefore $\operatorname{Im}\nu<0$. After removing the unknown trace through the [global relation](#global-relation-for-a-linear-boundary-value-problem), deform the boundary [contour](complex-analysis.md#complex-integration-contour) to the displayed two rays, with $0<\theta<\pi/4$, oriented from left infinity to $i\alpha$ to right infinity. The factor $e^{ikx}$ decays like $e^{-r x\sin\theta}$, while $e^{-\omega t}$ has Gaussian decay for large $r$. Apparent poles introduced by splitting a finite-time forcing transform must be treated as removable singularities of the unsplit expression.

##### Collocation points for a global relation

↑ **Parent:** [Global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem)

These are chosen complex values of a [spectral parameter for a linear boundary value problem](#spectral-parameter-for-a-linear-boundary-value-problem) at which a truncated [global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem) is enforced. Their directions and magnitudes determine which boundary side and which tangential mode are tested. Suitable row combinations can give much better conditioning than arbitrary raw samples.

##### Conjugate global relations for the modified Helmholtz equation

↑ **Parent:** [Global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem)

The two [modified Helmholtz adjoint plane waves](partial-differential-equation.md#modified-helmholtz-adjoint-plane-wave) $v_\lambda$ and $\widetilde v_\lambda=\overline{v_{\overline\lambda}}$ give boundary identities $\mathcal G(\lambda)=0$ and $\widetilde{\mathcal G}(\lambda)=0$. For real solution traces, $\widetilde{\mathcal G}(\lambda)=\overline{\mathcal G(\overline\lambda)}$. Reality is needed for this conjugation argument; the parametrization separately yields the reciprocal identity $\widetilde{\mathcal G}(\lambda)=\mathcal G(1/\lambda)$.

###### Rotationally invariant Neumann reconstruction in an equilateral triangle

↑ **Parent:** [Conjugate global relations for the modified Helmholtz equation](#conjugate-global-relations-for-the-modified-helmholtz-equation)

For the [modified Helmholtz equation](partial-differential-equation.md#modified-helmholtz-equation) $\Delta q-4\lambda q=0$ with identical oriented outward [Neumann boundary data](#neumann-boundary-data) on all sides of an [equilateral triangle](geometry-and-topology.md#equilateral-triangle), uniqueness forces rotation invariance. Put $\chi(k)=l(k+\lambda/k)/2$, $\Psi(k)=\int_{-l/2}^{l/2}e^{(k+\lambda/k)s}f(s)ds$, and $a=e^{2\pi i/3}$. At $\chi(k_n)=i\pi n$, paired [global relations](#global-relation-for-a-linear-boundary-value-problem) give

$$
Q_n=\frac{i[\cosh\chi(\bar a k_n)\Psi(k_n)+(-1)^n\Psi(\bar a k_n)+\Psi(a k_n)]}{(k_n-\lambda/k_n)\sinh\chi(\bar a k_n)}.
$$

For $\lambda>0$ one may choose $k_n=i[\pi n/l+\sqrt{(\pi n/l)^2+\lambda}]$; both denominator factors are nonzero. The derivation retains the tangential-derivative term in each side spectrum. Its endpoint contribution vanishes at these samples because rotation invariance makes all vertex values equal. For $\lambda=0$ the data must have zero total flux and an additive constant remains; negative parameters at [Neumann Laplacian](partial-differential-equation.md#neumann-laplacian) eigenvalues require the [Fredholm solvability condition](analysis.md#fredholm-solvability-condition) and allow homogeneous additions.

###### Sine collocation of square modified Helmholtz global relations

↑ **Parent:** [Conjugate global relations for the modified Helmholtz equation](#conjugate-global-relations-for-the-modified-helmholtz-equation)

On the square $[-1,1]^2$, write normal traces in $\phi_n(s)=\sin[n\pi(s+1)/2]$. Set $p_n=n\pi/2$, $\omega_n=\sqrt{k^2+p_n^2}$, $r_n=(\omega_n+p_n)/k$. Paired spectral samples $\{r_n,r_n^{-1}\}$, $\{-r_n,-r_n^{-1}\}$, $\{ir_n,i/r_n\}$, $\{-ir_n,-i/r_n\}$ give adjoint tests $e^{\mp\omega_ny}\phi_n(x)$ and $e^{\mp\omega_nx}\phi_n(y)$. Each test vanishes on the adjacent sides, removing their unknown [normal derivatives](differential-geometry.md#normal-derivative).

###### Square modified Helmholtz Dirichlet-to-Neumann coefficients

↑ **Parent:** [Sine collocation of square modified Helmholtz global relations](#sine-collocation-of-square-modified-helmholtz-global-relations)

Let $R_{jn}=\int_{\partial\Omega}f\partial_nv_{jn}ds$ for a square sine adjoint test, and put $\rho_{jn}=e^{-\omega_n}R_{jn}$, $\delta_n=e^{-2\omega_n}$. The opposite-side normal-trace coefficients obey

$$
c_{Bn}=\frac{\rho_{Bn}-\delta_n\rho_{Tn}}{1-\delta_n^2},\qquad c_{Tn}=\frac{\rho_{Tn}-\delta_n\rho_{Bn}}{1-\delta_n^2},
$$

with the same formulas for $L,R$. When the known [Dirichlet boundary condition](#dirichlet-boundary-condition) is integrated exactly, these are exact coefficients, since [orthogonality](linear-algebra.md#orthogonal-vectors) eliminates all other unknown modes.

###### Diagonal dominance of paired square global-relation collocation

↑ **Parent:** [Sine collocation of square modified Helmholtz global relations](#sine-collocation-of-square-modified-helmholtz-global-relations)

For [sine collocation of square modified Helmholtz global relations](#sine-collocation-of-square-modified-helmholtz-global-relations), each opposite-side mode has a scaled matrix

$$
\begin{pmatrix}1&\delta_n\\\delta_n&1\end{pmatrix},\qquad\delta_n=e^{-2\sqrt{k^2+(n\pi/2)^2}}<e^{-\pi}.
$$

The assembled system has [strict diagonal dominance](vector-space.md#strictly-diagonally-dominant-matrix), and its [spectral condition number of a positive-definite matrix](linear-algebra.md#spectral-condition-number-of-a-positive-definite-matrix) is below $(1+e^{-\pi})/(1-e^{-\pi})<1.091$. The conclusion concerns the explicit paired sine rows, not arbitrary uncombined complex rows.

#### Spectral parameter for a linear boundary value problem

↑ **Parent:** [Boundary value problem](#boundary-value-problem)

A complex parameter labels auxiliary solutions of a linear [differential equation](differential-equation.md), such as exponential adjoint solutions used in a [global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem). It need not be a discrete [eigenvalue](linear-operator-theory.md#eigenvalue) or a parameter of a nonlinear [Lax pair](integrable-systems.md#lax-pair). Analytic dependence on it allows transformed boundary identities to be sampled or inverted.

#### Boundary lifting

↑ **Parent:** [Boundary value problem](#boundary-value-problem)

Subtract a known function with the required boundary trace so that the remaining unknown has homogeneous [boundary conditions](#boundary-condition). For an interval with [Dirichlet boundary conditions](#dirichlet-boundary-condition) $g(t),h(t)$, $\ell=(1-x/L)g+(x/L)h$ is a simple lifting. In $w_t=w_{xx}-cw$, $z=w-\ell$ has forcing $-\ell_t-c\ell$ and zero endpoint values. This improves [Fourier sine series](fourier-series.md#fourier-sine-series) convergence.

##### Uniform half-line Schrodinger representation by boundary lifting

↑ **Parent:** [Boundary lifting](#boundary-lifting)

For the [free Schrodinger equation](physics.md#free-schrodinger-equation) with compatible smooth initial and boundary data, subtract $g(t)e^{-x}$ before taking a [Fourier sine transform](analysis.md#fourier-sine-transform). The lifted initial datum vanishes at the endpoint, making its sine transform $O(k^{-2})$ if its second derivative is integrable. The transformed forcing is $k(ig-g')/(1+k^2)$; time integration followed by [integration by parts](calculus.md#integration-by-parts) makes its solution contribution uniformly $O(k^{-3})$. An integrable spectral majorant proves [uniform convergence](real-analysis.md#uniform-convergence) even at the compatible initial-boundary corner.

### Boundary condition

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boundary_condition)

A boundary condition prescribes values of an unknown [function](function.md) or its [derivatives](calculus.md#derivative) at the boundary of the domain of a [differential equation](differential-equation.md).

#### Dynamic boundary condition for the heat equation

↑ **Parent:** [Boundary condition](#boundary-condition)

A dynamic [boundary condition](#boundary-condition) includes a time derivative of the boundary trace. For a half-line [heat equation](diffusion-equation.md#heat-equation), $u_t(0,t)+\alpha u_x(0,t)+\beta u(0,t)=f(t)$ gives a separate boundary evolution coupled to the interior flux. Its [Laplace transform](analysis.md#laplace-transform) contains the initial trace $u_0(0)$. The sign of $u_x$ differs from that of the outward [normal derivative](differential-geometry.md#normal-derivative) at a left endpoint.

##### Dirichlet energy dissipation with a dynamic heat boundary condition

↑ **Parent:** [Dynamic boundary condition for the heat equation](#dynamic-boundary-condition-for-the-heat-equation)

For a smooth [heat equation](diffusion-equation.md#heat-equation) solution $w_t=\Delta w$ with $w_t+\alpha\partial_nw=0$ on the [boundary](topology.md#boundary-of-a-set) and nonnegative $\alpha$, [Green's first identity](partial-differential-equation.md#green-s-first-identity) gives the displayed dissipation identity for $E=\int_V|\nabla w|^2$. The outward [normal derivative](differential-geometry.md#normal-derivative) is used. Writing the [boundary](topology.md#boundary-of-a-set) loss as $\alpha(\partial_nw)^2$ avoids division by $\alpha$ and remains valid where $\alpha=0$. A stationary solution is harmonic with $\alpha\partial_nw=0$; it need not be a particular fixed-data [Dirichlet problem](analysis.md#dirichlet-problem) solution.

##### Repeated-root dynamic-boundary heat kernel

↑ **Parent:** [Dynamic boundary condition for the heat equation](#dynamic-boundary-condition-for-the-heat-equation)

For the [dynamic boundary condition for the heat equation](#dynamic-boundary-condition-for-the-heat-equation) with $\alpha=2a$, $\beta=a^2$, the boundary resolvent denominator is $(\sqrt p-a)^2$. With the [principal square root](analysis.md#principal-square-root-of-a-complex-number), its inverse kernel is

$$
J_a(x,t)=(1-ax+2a^2t)e^{-ax+a^2t}\operatorname{erfc}\!\left(\frac{x}{2\sqrt t}-a\sqrt t\right)+2a\sqrt{t/\pi}\,e^{-x^2/(4t)}.
$$

Equivalently, $J_a=\int_0^\infty r e^{ar}P(x+r,t)dr$ using the [Heat Poisson kernel](diffusion-equation.md#heat-poisson-kernel). This representation fixes the repeated-root sign and remains valid for either sign of $a$.

###### Repeated-root unstable heat boundary mode

↑ **Parent:** [Repeated-root dynamic-boundary heat kernel](#repeated-root-dynamic-boundary-heat-kernel)

For $a>0$, the [heat equation](diffusion-equation.md#heat-equation) on a half-line with $u_t+2au_x+a^2u=0$ at the left endpoint admits $u=e^{-ax+a^2t}$. The solution is spatially decaying and temporally growing. The boundary resolvent has a double pole at $p=a^2$, allowing generalized contributions proportional to $t e^{a^2t}$. For $a<0$ the root $\sqrt p=a$ is absent on the [principal square root](analysis.md#principal-square-root-of-a-complex-number) branch.

#### Clamped boundary condition

↑ **Parent:** [Boundary condition](#boundary-condition)

A clamped endpoint of a fourth-order beam or eigenvalue problem imposes both zero displacement and zero slope, $y=y'=0$. These conditions remove the boundary terms produced by integrating a fourth derivative by parts twice.

#### Periodic boundary conditions

↑ **Parent:** [Boundary condition](#boundary-condition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Periodic_boundary_conditions)

A periodic boundary condition identifies opposite ends of a domain by requiring the solution and the derivatives needed by the equation to agree there.

#### Vanishing boundary condition

↑ **Parent:** [Boundary condition](#boundary-condition)

A vanishing boundary condition requires the relevant field, variation, or flux to tend to zero on the boundary. It removes boundary terms produced by [integration by parts](calculus.md#integration-by-parts).

#### Initial condition

↑ **Parent:** [Boundary condition](#boundary-condition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Initial_condition)

An initial condition prescribes the state of a time-dependent problem at a chosen initial time.

##### Initial velocity

↑ **Parent:** [Initial condition](#initial-condition)

Initial velocity specifies the time derivative of the [displacement field](continuum-mechanics.md#displacement-field-mechanics) at the starting time. A second-order [wave equation](wave-equation.md) requires it independently of [initial displacement](#initial-displacement). Both vanish for a causal scattered field before an incident pulse reaches its scatterer.

##### Initial displacement

↑ **Parent:** [Initial condition](#initial-condition)

Initial displacement specifies the configuration of a [wave equation](wave-equation.md) at the starting time. For a second-order evolution equation it is paired with the [initial velocity](#initial-velocity). Specifying only the boundary forcing does not determine these initial data.

#### Dirichlet boundary condition

↑ **Parent:** [Boundary condition](#boundary-condition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dirichlet_boundary_condition)

A Dirichlet boundary condition prescribes the value of the unknown function on the boundary.

##### Dirichlet boundary data

↑ **Parent:** [Dirichlet boundary condition](#dirichlet-boundary-condition)

Dirichlet boundary data prescribe the boundary values of a solution as a function $\varphi$ on the boundary of its domain. Continuity on a polygon requires agreement of the values at corners, but continuity alone does not ensure solvability if the equation loses [uniform ellipticity](elliptic-boundary-value-problem.md#uniformly-elliptic-operator) at a boundary side.

##### Perfectly conducting thermal boundary condition

↑ **Parent:** [Dirichlet boundary condition](#dirichlet-boundary-condition)

In a fixed-temperature [convection](fluid-mechanics.md#convection) problem, the boundary [temperature](thermodynamics.md#temperature) is prescribed, and its perturbation satisfies a thermal [Dirichlet boundary condition](#dirichlet-boundary-condition). A homogeneous condition means the boundary follows the prescribed conductive background [temperature](thermodynamics.md#temperature). This does not necessarily mean a vertical wall has a spatially constant [temperature](thermodynamics.md#temperature); that additional assumption can conflict with a background vertical [gradient](calculus.md#gradient).

#### Neumann boundary condition

↑ **Parent:** [Boundary condition](#boundary-condition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Neumann_boundary_condition)

A Neumann boundary condition prescribes the outward normal derivative of the unknown function on the boundary.

##### Neumann boundary data

↑ **Parent:** [Neumann boundary condition](#neumann-boundary-condition)

[Neumann boundary data](#neumann-boundary-data) are prescribed values of the outward [normal derivative](differential-geometry.md#normal-derivative) of a function on the boundary of a [boundary value problem](#boundary-value-problem). They enter a [Neumann boundary condition](#neumann-boundary-condition) as $\partial_nu=g_N$. Directional derivatives defined using a fixed coordinate direction must be converted to the outward-normal convention: for example, on the bottom of an upper domain, $\partial_nu=-u_y$.

##### Initial incompatibility with a Neumann boundary condition

↑ **Parent:** [Neumann boundary condition](#neumann-boundary-condition)

Initial data whose normal [derivative](calculus.md#derivative) is nonzero at a wall cannot satisfy homogeneous [Neumann boundary conditions](#neumann-boundary-condition) continuously all the way to the initial time. For example, $-\operatorname{erf}(ay)$ has wall [derivative](calculus.md#derivative) $-2ae^{-a^2}/\sqrt\pi$ at $y=\pm1$, which is nonzero for finite $a>0$. A parabolic [mild solution of an abstract Cauchy problem](functional-analysis.md#mild-solution-of-an-abstract-cauchy-problem) can still take those initial data in an integral or square-integrable sense and satisfy the boundary condition for every positive time. An exactly compatible smooth profile is needed for a classical solution on the closed time interval.

##### Neumann eigenfunction

↑ **Parent:** [Neumann boundary condition](#neumann-boundary-condition)

A Neumann eigenfunction is an [eigenfunction](linear-operator-theory.md#eigenfunction) of a spatial [differential operator](analysis.md#differential-operator) whose normal [derivative](calculus.md#derivative) vanishes on the boundary. A [Sturm-Liouville eigenfunction expansion](analysis.md#sturm-liouville-eigenfunction-expansion) in these functions gives a [heat kernel](diffusion-equation.md#heat-kernel) for homogeneous [Neumann boundary conditions](#neumann-boundary-condition).

#### Tangential boundary derivative

↑ **Parent:** [Boundary condition](#boundary-condition)

A tangential boundary derivative differentiates the boundary restriction of a [function](function.md) along a [tangent vector](differential-geometry.md#tangent-vector). Prescribing it fixes the boundary value only up to a constant on each connected boundary component. This differs from a [Neumann boundary condition](#neumann-boundary-condition), which specifies a normal [derivative](calculus.md#derivative).

#### Robin boundary condition

↑ **Parent:** [Boundary condition](#boundary-condition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Robin_boundary_condition)

A Robin boundary condition prescribes a linear combination of a function and its outward normal derivative on the boundary.

##### Poisson uniqueness with a nonnegative Robin normal coefficient

↑ **Parent:** [Robin boundary condition](#robin-boundary-condition)

On a bounded region, two sufficiently regular solutions of the [Poisson equation](partial-differential-equation.md#poisson-equation) with the same forcing and boundary condition $\alpha\partial_n\phi+\phi=\gamma$, where $\alpha\ge0$, have harmonic difference $w$. [Green's first identity](partial-differential-equation.md#green-s-first-identity) gives $\int|\nabla w|^2=\int_{\partial V}w\partial_nw=-\int_{\partial V}\alpha(\partial_nw)^2\le0$. Hence $w$ is constant on each component, and the boundary condition makes that constant zero. The proof never divides by $\alpha$, so it includes variable coefficients and Dirichlet portions where $\alpha=0$.

##### Symmetric Robin strip transform

↑ **Parent:** [Robin boundary condition](#robin-boundary-condition)

For a decaying harmonic function on a semi-infinite strip with equal outward [Robin boundary conditions](#robin-boundary-condition) and reflection-symmetric end data, the top and bottom value traces agree. The [global relation](#global-relation-for-a-linear-boundary-value-problem) and its reflected spectral companion express their transforms through $D(k)$. With $H(k)=\tfrac12\int_0^\ell e^{ky}g(y)dy$, the relation is $\psi(-ik)+\psi(ik)=2H(k)/D(k)$. Real zeros of $D$ require compatible data; unrestricted negative Robin parameters do not guarantee a decaying solution.

###### Solvability of a decaying Robin strip

↑ **Parent:** [Symmetric Robin strip transform](#symmetric-robin-strip-transform)

Let $\lambda_n$ be the transverse [eigenvalues](linear-operator-theory.md#eigenvalue) of a [Sturm-Liouville problem](analysis.md#sturm-liouville-problem) for the two [Robin boundary conditions](#robin-boundary-condition). For a harmonic strip solution decaying in the longitudinal direction, projection of the prescribed end [Neumann boundary condition](#neumann-boundary-condition) onto every nonpositive eigenvalue must vanish. Positive modes give $q_n(x)=-g_ne^{-\sqrt{\lambda_n}x}/\sqrt{\lambda_n}$. Zero modes are affine and negative modes are oscillatory, so neither can contribute to a decaying solution. The condition also establishes uniqueness within the decay class.

##### Weak Robin problem for a uniformly elliptic operator

↑ **Parent:** [Robin boundary condition](#robin-boundary-condition)

For $Lu=-\partial_j(a^{ij}\partial_i u)+b^i\partial_i u+cu$ with smooth coefficients on a bounded smooth domain, the [weak formulation](partial-differential-equation.md#weak-formulation) of $(L+\lambda)u=f$ and conormal [Robin boundary condition](#robin-boundary-condition) $a^{ij}\partial_i u\,\nu_j+\beta u=0$ is

$$
\int_U\bigl(a^{ij}\partial_i u\partial_j v+b^i\partial_i u\,v+(c+\lambda)uv\bigr)
+\int_{\partial U}\beta TuTv=\int_Ufv\qquad(v\in H^1(U)).
$$

The [bilinear form](linear-algebra.md#bilinear-form) is bounded by the [Sobolev trace theorem](sobolev-space.md#sobolev-trace-theorem). If $a^{ij}$ satisfy the positive [uniformly elliptic operator](elliptic-boundary-value-problem.md#uniformly-elliptic-operator) inequality, the [multiplicative trace inequality on a bounded smooth domain](sobolev-space.md#multiplicative-trace-inequality-on-a-bounded-smooth-domain) and the [Young inequality](nonlinear-analysis.md#young-s-inequality-for-products) show that the form is [coercive](linear-algebra.md#coercive-bilinear-form) when $\lambda$ is sufficiently large, even if $\beta$ and $c$ have negative parts. The [Lax-Milgram theorem](functional-analysis.md#lax-milgram-theorem) then gives a unique [weak solution](partial-differential-equation.md#weak-solution) for every $f\in L^2(U)$.

#### Mixed boundary condition

↑ **Parent:** [Boundary condition](#boundary-condition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mixed_boundary_condition)

A mixed boundary condition imposes different kinds of [boundary conditions](#boundary-condition) on different portions of the boundary. A common elliptic example combines a [Dirichlet boundary condition](#dirichlet-boundary-condition) on one portion with a [Neumann boundary condition](#neumann-boundary-condition) on the remainder.

#### Far-field boundary condition

↑ **Parent:** [Boundary condition](#boundary-condition)

A far-field boundary condition prescribes the limiting behavior of a solution as one or more spatial coordinates tend to infinity.

### Sign-decay differential equation

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)

For $y_0>0$, the initial-value problem

$$
y'=-\operatorname{sign}(y),
\qquad y(0)=y_0,
$$

has the continuous piecewise differentiable solution

$$
y(t)=\max\{y_0-t,0\}.
$$

The vector field is not Lipschitz at zero, but the direction on each side prevents any solution from leaving zero, so this solution is unique in the piecewise differentiable class.

#### Explicit Euler method for the sign-decay equation

↑ **Parent:** [Sign-decay differential equation](#sign-decay-differential-equation)

The iteration $y_{n+1}=y_n-h\operatorname{sign}(y_n)$ agrees with the exact linear descent until the first step past zero. It then either remains at zero or alternates between two values of magnitude at most $h$. Consequently its uniform grid-point error is at most $h$ for arbitrarily long finite time intervals.

### Parameter sensitivity equation

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)

Differentiating a parameter-dependent initial-value problem with respect to its parameter gives a linear inhomogeneous equation for the solution sensitivity, with initial data obtained by differentiating the original initial condition.

### Differential inequality

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Differential_inequality)

A differential inequality bounds derivatives rather than specifying them exactly; comparison and integration turn it into bounds on the function.

### Bernoulli differential equation

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bernoulli_differential_equation)

For

$$
y'+P(x)y=Q(x)y^n,\qquad n\ne0,1,
$$

the substitution $z=y^{1-n}$ gives the linear equation

$$
z'+(1-n)Pz=(1-n)Q.
$$

#### Finite-time extinction in a sublinear Bernoulli equation

↑ **Parent:** [Bernoulli differential equation](#bernoulli-differential-equation)

For $y'=y-Ay^p$, $A>0$ and $0<p<1$, put $u=y^{1-p}$ while $y>0$. Then $u'=(1-p)(u-A)$. If $0<y_0<A^{1/(1-p)}$, $u$ decreases to zero at the displayed finite time. The positive branch joins the zero solution with zero first derivative, giving a nonnegative forward solution. The equilibrium at zero is one-sided stable even though the vector field is not locally [Lipschitz continuous](real-analysis.md#lipschitz-continuity) there; the positive equilibrium is unstable.

### Tangent addition functional equation

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)

A differentiable real function satisfying

$$
f(x+y)=\frac{f(x)+f(y)}{1-f(x)f(y)}
$$

on an interval has $f(0)=0$ and $f'=C(1+f^2)$, hence $f(x)=\tan(Cx)$ wherever the tangent remains finite.

### Linear ordinary differential equation

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_ordinary_differential_equation)

A linear ordinary differential equation is linear in the unknown function and its derivatives.

#### Characteristic equation of a constant-coefficient differential equation

↑ **Parent:** [Linear ordinary differential equation](#linear-ordinary-differential-equation)

For the homogeneous [linear ordinary differential equation](#linear-ordinary-differential-equation) $\sum_{j=0}^n a_j y^{(j)}=0$, substitute $y=e^{rx}$. Dividing by the nonzero exponential gives the polynomial equation $P(r)=\sum_j a_jr^j=0$. A simple root gives an exponential solution; a root of multiplicity $m$ gives $x^ke^{rx}$ for $0\le k<m$. Real equations admit real sine and cosine combinations of conjugate roots. These [characteristic roots](#characteristic-root-of-a-constant-coefficient-differential-equation) determine growth, decay and oscillation of the linearized modes.

#### Method of undetermined coefficients

↑ **Parent:** [Linear ordinary differential equation](#linear-ordinary-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Method_of_undetermined_coefficients)

Choose a finite trial family of polynomial-exponential or trigonometric functions for a [particular solution](#particular-solution), substitute it into a constant-coefficient linear equation, and solve for its coefficients. If the forcing exponent is a characteristic root of multiplicity $m$, multiply the ordinary trial by $t^m$ to leave the homogeneous [kernel](linear-algebra.md#kernel-of-a-linear-map). The method is efficient for forcing families preserved by differentiation.

##### Resonant exponential particular solution

↑ **Parent:** [Method of undetermined coefficients](#method-of-undetermined-coefficients)

For a constant-coefficient [linear differential equation](#linear-differential-equation) $P(D)y=e^{rx}$, where $D$ denotes differentiation, a simple root $P(r)=0$ forces a resonant trial. Factor $P(z)=(z-r)Q(z)$; since $(D-r)(xe^{rx})=e^{rx}$, commuting the differential operators gives $P(D)(xe^{rx})=Q(r)e^{rx}=P'(r)e^{rx}$. Thus the displayed expression is a [particular solution](#particular-solution). More generally, if the root has multiplicity $m$, the same factorization gives $P(D)(x^me^{rx})=P^{(m)}(r)e^{rx}$, so $y_p=x^me^{rx}/P^{(m)}(r)$. This is the extra polynomial factor required by [resonance in a differential equation](#resonance-in-a-differential-equation).

#### Weighted energy estimate for two coupled modes

↑ **Parent:** [Linear ordinary differential equation](#linear-ordinary-differential-equation)

Suppose two complex amplitudes satisfy $\partial_t|A|^2\leq2a|A||B|-2d|A|^2$ and $\partial_t|B|^2\leq2c|A||B|-2d|B|^2$, with positive $a,c$ and $d\geq0$. Then $N=c|A|^2+a|B|^2\geq2\sqrt{ac}|A||B|$ gives $\dot N\leq2(\sqrt{ac}-d)N$. A positive weighted norm avoids treating two coupling rates of different size as a single arithmetic sum. This is useful for nonautonomous [linear ordinary differential equations](#linear-ordinary-differential-equation) and the [bounded-modulation alpha-Omega growth estimate](astrophysical-fluid-dynamics.md#bounded-modulation-alpha-omega-growth-estimate).

<h4 id="newton-s-law-of-cooling">Newton's law of cooling</h4>

↑ **Parent:** [Linear ordinary differential equation](#linear-ordinary-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Newton's_law_of_cooling)

Newton's law of cooling models the temperature $T$ of an object in an environment at constant temperature $T_\infty$ by $\dot T=-a(T-T_\infty)$ for a positive cooling rate $a$.

##### Impulse versus finite-duration cooling

↑ **Parent:** [Newton's law of cooling](#newton-s-law-of-cooling)

For equal initial temperatures and the same [Newton's law of cooling](#newton-s-law-of-cooling) coefficient $a>0$, compare a unit [Dirac delta function](distribution-theory.md#dirac-delta-function) cooling impulse at time one with unit-rate cooling on the interval from one to two. The impulse produces a temperature jump of minus one. The finite-duration forcing gives a continuous temperature with change $-(1-e^{-a(t-1)})/a$ while it is active. Relative to the common unforced cooling curve, the impulse contributes $-e^{-a(t-1)}$. Consequently the temperatures cross at $t=1+\log(1+a)/a$, strictly between one and two. After time two the impulse-cooled body is warmer: the later cooling receives less subsequent exponential attenuation.

##### Cumulative thermal destruction under exponential warming and cooling

↑ **Parent:** [Newton's law of cooling](#newton-s-law-of-cooling)

In an ideal linear temperature-dependent destruction model with equal warming and cooling durations, normalized temperature is $1-e^{-\alpha t}$ during warming and $(1-e^{-\alpha T})e^{-\alpha(t-T)}$ during cooling. Integrating the destruction rate gives $D(T)$, the [logarithm](calculus.md#logarithm) of the surviving-count reduction factor. If the endpoint destruction rate and thermal relaxation constant stay fixed, changing the temperature gap alone leaves this integral unchanged. This is a property of the stipulated model.

##### Newton cooling with an instantaneous temperature jump

↑ **Parent:** [Newton's law of cooling](#newton-s-law-of-cooling)

Under [Newton's law of cooling](#newton-s-law-of-cooling) with fixed ambient temperature $T_0$ and $k>0$, an instantaneous jump $\beta$ at $t_*$ sets $T(t_*+)=T(t_*-)+\beta$. The subsequent temperature is $T_0+[T(t_*-)+\beta-T_0]e^{-k(t-t_*)}$. Equivalently, for an initial temperature $T_i$, the full solution is

$$
T(t)=T_0+(T_i-T_0)e^{-kt}+\beta H(t-t_*)e^{-k(t-t_*)}.
$$

This piecewise model has the [distributional derivative](distribution-theory.md#distributional-derivative) equation $T'+k(T-T_0)=\beta\delta(t-t_*)$, with the [Dirac delta distribution](distribution-theory.md#dirac-delta-function) representing the added temperature.

##### Heat transfer coefficient

↑ **Parent:** [Newton's law of cooling](#newton-s-law-of-cooling)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Heat_transfer_coefficient)

A heat transfer coefficient relates [heat flux](thermodynamics.md#heat-flux-density) through a boundary to a temperature difference: $F=\lambda\Delta T$. Its dimensions are power per area per temperature. In a quasistatic ice layer, atmospheric boundary resistance $1/\lambda_A$ and conductive resistance $h/k$ add in series, giving effective conductance $(1/\lambda_A+h/k)^{-1}$.

#### Homogeneous solution

↑ **Parent:** [Linear ordinary differential equation](#linear-ordinary-differential-equation)

A homogeneous solution solves the associated linear equation with zero forcing. The difference of any two solutions to the same forced linear equation is homogeneous.

A homogeneous solution satisfies the associated [homogeneous linear differential equation](#homogeneous-linear-differential-equation), obtained by setting the forcing term to zero. Such solutions form the kernel of the differential operator.

#### Particular solution

↑ **Parent:** [Linear ordinary differential equation](#linear-ordinary-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Particular_solution)

A particular solution is any one solution of a forced linear differential equation. Every solution is the sum of that particular solution and an arbitrary [homogeneous solution](#homogeneous-solution).

#### General solution

↑ **Parent:** [Linear ordinary differential equation](#linear-ordinary-differential-equation)

The general solution of a [differential equation](differential-equation.md) is a family containing every solution, usually parameterized by arbitrary constants or initial data. For a forced [linear ordinary differential equation](#linear-ordinary-differential-equation), it is the sum of one [particular solution](#particular-solution) and the general [homogeneous solution](#homogeneous-solution).

#### Dominant eigenmode in a forced linear system

↑ **Parent:** [Linear ordinary differential equation](#linear-ordinary-differential-equation)

After diagonalising a constant-coefficient system, each eigenmode satisfies a scalar forced equation. The large-time behaviour is determined by the largest exponential rate whose coefficient does not vanish, including rates introduced by the forcing.

#### Second-order linear differential equation

↑ **Parent:** [Linear ordinary differential equation](#linear-ordinary-differential-equation)

A second-order linear equation has the form $y\prime\prime+p(x)y\prime+q(x)y=f(x)$.

##### Quadratic-variable reduction of a singular oscillator

↑ **Parent:** [Second-order linear differential equation](#second-order-linear-differential-equation)

The [chain rule](calculus.md#chain-rule) with $y(x)=Y(x^2)$ gives $xy''-y'=4x^3Y''$ and transforms the equation, away from zero, into $Y''+Y=0$. Thus its solution space is spanned by $\cos(x^2)$ and $\sin(x^2)$. Both extend smoothly through the [regular singular point](complex-analysis.md#regular-singular-point) at zero. Their even [power series](real-analysis.md#power-series) allow the independent data $y(0)$ and $y''(0)$ to select the two solutions; every smooth solution has $y'(0)=0$.

##### Repeated-root constant-coefficient differential equation

↑ **Parent:** [Second-order linear differential equation](#second-order-linear-differential-equation)

The homogeneous equation has [linearly independent](vector-space.md#linear-independence) solutions $e^{rx}$ and $xe^{rx}$, with nonzero [Wronskian](#wronskian) $e^{2rx}$. Setting $y=e^{rx}u$ converts the forced equation to $u''=e^{-rx}f$. For resonant forcing $f=e^{rx}$, the particular response is $x^2e^{rx}/2$. This substitution explains the extra powers of $x$ required by repeated-root resonance.

##### Singular point of a second-order linear ODE

↑ **Parent:** [Second-order linear differential equation](#second-order-linear-differential-equation)

For a normalized second-order equation, a point is singular when its coefficient functions are not both analytic there. If multiplying them by the first and second powers of distance to the point makes them analytic, it is a [regular singular point](complex-analysis.md#regular-singular-point). This classification concerns the equation; some individual solutions may nevertheless extend analytically through the point.

##### Reciprocal-coordinate reduction of a beam-type equation

↑ **Parent:** [Second-order linear differential equation](#second-order-linear-differential-equation)

For $t>0$, the [change of variables](calculus.md#change-of-variables-formula) $\tau=1/t$ and $u(t)=v(\tau)/\tau$ converts $t^4u''+\lambda^2u=0$ into $v''+\lambda^2v=0$. The [chain rule](calculus.md#chain-rule) gives $u'=v-\tau v'$ and $u''=\tau^3v''$. Thus $u=t[A\cos(\lambda/t)+B\sin(\lambda/t)]$. The prefactor cancels the derivative term introduced by inverting the independent variable.

##### Liouville transformation of a second-order equation

↑ **Parent:** [Second-order linear differential equation](#second-order-linear-differential-equation)

A smooth invertible [change of variables](calculus.md#change-of-variables-formula) in $u_{xx}-f(x)u=0$ introduces a first derivative in time. Rescaling by $\dot x^{-1/2}$ removes it. Choosing $\dot x=f^{-1/2}$ locally for $f>0$ produces the constant leading coefficient used in the [WKB approximation](analysis.md#wkb-approximation); negative $f$ requires a complex branch or the corresponding oscillatory real formulation.

##### Power substitution for an oscillatory second-order equation

↑ **Parent:** [Second-order linear differential equation](#second-order-linear-differential-equation)

For $\gamma\ne0$ and $x>0$, the [change of variables](calculus.md#change-of-variables-formula) $u=x^\gamma$ converts

$$
x^{2-2\gamma}y''+(1-\gamma)x^{1-2\gamma}y'+\gamma^2y=0
$$

into $Y_{uu}+Y=0$, where $y(x)=Y(u)$. The [chain rule](calculus.md#chain-rule) cancels the first-derivative terms. Thus $\cos(x^\gamma)$ and $\sin(x^\gamma)$ form a pair of [linearly independent](vector-space.md#linear-independence) solutions, with [Wronskian](#wronskian) $\gamma x^{\gamma-1}$. This is a variable-speed reparametrization of the [harmonic oscillator equation](classical-mechanics.md#simple-harmonic-motion).

##### Mathieu equation

↑ **Parent:** [Second-order linear differential equation](#second-order-linear-differential-equation)

The Mathieu equation is the displayed [linear differential equation](#linear-differential-equation) with periodic coefficients. [Floquet theory](#floquet-theory) describes its bounded and exponentially growing solutions, while its periodic [Mathieu characteristic values](#mathieu-characteristic-value) mark the edges of [parametric resonance](#parametric-resonance) gaps. The forcing normalization matters: replacing $t$ by $t/2$ rescales both the constant and periodic coefficients.

###### Mathieu characteristic value

↑ **Parent:** [Mathieu equation](#mathieu-equation)

The Mathieu characteristic values are the parameter values $a$ for which the [Mathieu equation](#mathieu-equation) has the even periodic mode traditionally denoted $\operatorname{ce}_n$, or the odd periodic mode $\operatorname{se}_n$. They are [eigenvalues](linear-operator-theory.md#eigenvalue) of $-d^2/dt^2+2q\cos2t$ with the corresponding periodic or antiperiodic [boundary conditions](#boundary-condition). Their small-$q$ expansions can be derived by projecting onto a [Fourier series](fourier-series.md) and perturbing the resulting tridiagonal [matrix](vector-space.md#matrix).

##### Airy ordinary differential equation

↑ **Parent:** [Second-order linear differential equation](#second-order-linear-differential-equation)

This second-order [ordinary differential equation](#ordinary-differential-equation) has the independent entire [Airy functions](#airy-function) $\operatorname{Ai}$ and $\operatorname{Bi}$ as a standard basis. It is distinct from the dispersive PDE in [Airy equation](integrable-systems.md#airy-equation). Its general solution is $a_1\operatorname{Ai}(Z)+a_2\operatorname{Bi}(Z)$.

###### Forced Airy boundary-value problem

↑ **Parent:** [Airy ordinary differential equation](#airy-ordinary-differential-equation)

On the unit interval, the weak form is $a(u,v)=\int_0^1fv$, with $a(u,v)=\int_0^1(u'v'+xuv)$ on the [zero-boundary Sobolev space](sobolev-space.md#zero-boundary-sobolev-space). The nonnegative potential makes this form coercive in the derivative [norm](functional-analysis.md#norm), and the [Poincaré inequality](sobolev-space.md#poincare-inequality) makes that [norm](functional-analysis.md#norm) equivalent to the [Sobolev norm](sobolev-space.md#sobolev-norm). The [Lax-Milgram theorem](functional-analysis.md#lax-milgram-theorem) gives a unique solution. A conforming [Ritz method](numerical-analysis.md#rayleigh-ritz-method) minimizes the corresponding strictly convex quadratic energy and produces a symmetric positive-definite [tridiagonal](vector-space.md#tridiagonal-matrix) [matrix](vector-space.md#matrix) for piecewise-linear hats.

###### Airy power-series fundamental pair

↑ **Parent:** [Airy ordinary differential equation](#airy-ordinary-differential-equation)

For the [Airy ordinary differential equation](#airy-ordinary-differential-equation) $y''=xy$, a [power series](real-analysis.md#power-series) obeys $a_2=0$ and $a_{m+3}=a_m/[(m+3)(m+2)]$. Setting its first two coefficients to $(1,0)$ or $(0,1)$ gives

$$
y_1(x)=\sum_{k\geq0}\frac{x^{3k}}{\prod_{j=1}^k(3j)(3j-1)},\qquad
y_2(x)=\sum_{k\geq0}\frac{x^{3k+1}}{\prod_{j=1}^k(3j)(3j+1)}.
$$

Empty products are one. The [ratio test](real-analysis.md#ratio-test) proves convergence on the whole complex plane. Termwise differentiation verifies the equation, and the initial normalization gives [Wronskian](#wronskian) one. By the [Abel identity](#abel-s-identity), the [Wronskian](#wronskian) remains one everywhere, so these solutions span the whole solution space.

###### Airy function

↑ **Parent:** [Airy ordinary differential equation](#airy-ordinary-differential-equation)

The standard Airy functions solve the [Airy ordinary differential equation](#airy-ordinary-differential-equation). Their [Wronskian](#wronskian) is $\operatorname{Ai}(Z)\operatorname{Bi}'(Z)-\operatorname{Ai}'(Z)\operatorname{Bi}(Z)=1/\pi$, so they form a fundamental solution pair, including for complex $Z$.

###### Airy displacement integral

↑ **Parent:** [Airy function](#airy-function)

For $q=e^{i\pi/6}$ define $I_0(C)=\int_0^\infty\operatorname{Ai}(q(s-C))ds$ and $I_1(C)=\int_0^\infty s\operatorname{Ai}(q(s-C))ds$. Both converge by [Airy function](#airy-function) decay. Integrating its differential equation gives $I_1-CI_0=iq\operatorname{Ai}\prime(-qC)$. These moments convert a decaying vorticity profile into its velocity and displacement for [three-layer long-wave shear-flow matching](hydrodynamic-stability.md#three-layer-long-wave-shear-flow-matching).

##### Elimination of the first derivative

↑ **Parent:** [Second-order linear differential equation](#second-order-linear-differential-equation)

For a [second-order linear differential equation](#second-order-linear-differential-equation)

$$
y''+p(x)y'+q(x)y=0,
$$

the substitution $y=u\exp[-\tfrac12\int p(x)\,dx]$ eliminates the first-derivative term and gives

$$
u''+\left(q-\frac12p'-\frac14p^2\right)u=0.
$$

##### Sturm-Picone comparison theorem

↑ **Parent:** [Second-order linear differential equation](#second-order-linear-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sturm–Picone_comparison_theorem)

For two real self-adjoint equations $(p_i y_i\prime)\prime+q_i y_i=0$ with continuous coefficients, $0<p_2\leq p_1$ and $q_1\leq q_2$, between consecutive zeros of a nontrivial first solution a nontrivial second solution either has a zero or is proportional to the first there. This comparison controls oscillation through the coefficients.

###### Sturm comparison theorem

↑ **Parent:** [Sturm-Picone comparison theorem](#sturm-picone-comparison-theorem)

If $q_1\leq q_2$, then between consecutive zeros of a nontrivial solution of

$$
y''+q_1(x)y=0
$$

there is a zero of every nontrivial solution of $y''+q_2(x)y=0$, unless the two coefficients agree throughout that interval.

###### Wronskian proof of Sturm comparison

↑ **Parent:** [Sturm comparison theorem](#sturm-comparison-theorem)

For solutions $\varphi_i''+q_i\varphi_i=0$, the mixed Wronskian

$$
W=\varphi_1'\varphi_2-\varphi_1\varphi_2'
$$

satisfies

$$
W'=(q_2-q_1)\varphi_1\varphi_2.
$$

Its endpoint signs between consecutive zeros of a positive $\varphi_1$ force a zero of $\varphi_2$ unless $q_1=q_2$.

##### Power-series solution of a differential equation

↑ **Parent:** [Second-order linear differential equation](#second-order-linear-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Power-series_solution_of_a_differential_equation)

##### Kummer differential equation

↑ **Parent:** [Second-order linear differential equation](#second-order-linear-differential-equation)

Kummer's equation is

$$
xy''+(b-x)y'-ay=0.
$$

Its solution analytic at zero is the [confluent hypergeometric function of the first kind](#confluent-hypergeometric-function-of-the-first-kind)

$$
M(a,b,x)=\sum_{m=0}^{\infty}
\frac{(a)_m}{(b)_m\,m!}x^m.
$$

When $b$ is not an integer, a second local solution is

$$
x^{1-b}M(a-b+1,2-b,x).
$$

###### Confluent hypergeometric function

↑ **Parent:** [Kummer differential equation](#kummer-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Confluent_hypergeometric_function)

Confluent hypergeometric functions solve the [Kummer differential equation](#kummer-differential-equation) $zy''+(b-z)y'-ay=0$. The regular solution is the [confluent hypergeometric function of the first kind](#confluent-hypergeometric-function-of-the-first-kind); a second standard solution is conventionally denoted $U(a,b,z)$. The family arises by coalescing singular points of the [Gauss hypergeometric equation](complex-analysis.md#gauss-hypergeometric-equation).

###### Confluent hypergeometric function of the first kind

↑ **Parent:** [Confluent hypergeometric function](#confluent-hypergeometric-function)

For $b$ not a nonpositive integer, the regular solution normalized by $M(a,b,0)=1$ has the [power series](real-analysis.md#power-series)

$$
M(a,b,z)=\sum_{n=0}^{\infty}\frac{(a)_n}{(b)_n}\frac{z^n}{n!}.
$$

Here $(a)_n$ is the [rising factorial](combinatorics.md#rising-factorial). Substitution into the [Kummer differential equation](#kummer-differential-equation) proves the coefficient recurrence. This normalization agrees with [NIST's definitions](https://dlmf.nist.gov/13.2).

##### Wronskian

↑ **Parent:** [Second-order linear differential equation](#second-order-linear-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wronskian)

<h6 id="abel-s-identity">Abel's identity</h6>

↑ **Parent:** [Wronskian](#wronskian)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Abel's_identity)

For $y\prime\prime+py\prime+qy=0$, the Wronskian satisfies $W\prime=-pW$.

##### Variation of parameters

↑ **Parent:** [Second-order linear differential equation](#second-order-linear-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Variation_of_parameters)

Variation of parameters replaces the constants in a complementary solution by functions to construct a particular solution.

##### Reduction of order

↑ **Parent:** [Second-order linear differential equation](#second-order-linear-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reduction_of_order)

Given one nonzero solution of a homogeneous second-order linear equation, reduction of order constructs a second by writing it as a variable multiple of the first.

###### First correction to a regular singular solution by reduction of order

↑ **Parent:** [Reduction of order](#reduction-of-order)

Suppose $y''-P(x)y'/x-Q(x)y/x=0$ has analytic $P,Q$ near zero, $P(x)=P_0+P_1x+\cdots$, and a solution $y_1=1+\beta x+\cdots$, with $P_0$ a positive integer. The [indicial roots](#indicial-root) are $0,P_0+1$. The [Abel identity](#abel-s-identity) gives $W=Cx^{P_0}(1+P_1x+\cdots)$. Dividing by $y_1^2$ gives $Cx^{P_0}[1+(P_1-2\beta)x+\cdots]$. Integrating this [reduction of order](#reduction-of-order) expression from zero, multiplying by $y_1$, and choosing $C=P_0+1$ proves the displayed normalized expansion. The integral's zero constant eliminates the added multiple of $y_1$. Its nonzero [Wronskian](#wronskian) proves independence. In this setting the assumed exponent-zero solution prevents a logarithm in the constructed exponent-$P_0+1$ solution.

###### Reduction of order across a zero of the known solution

↑ **Parent:** [Reduction of order](#reduction-of-order)

The integral representation $y_2=y_1\int e^{-\int p}/y_1^2$ is derived where $y_1\ne0$. At a zero, its integral factor may have a pole while the product has a removable singularity. For regular coefficients, continue the actual second solution by its finite initial data and initial-value uniqueness; the [Abel identity](#abel-s-identity) preserves a nonzero [Wronskian](#wronskian). In the degree-one [Legendre differential equation](#legendre-differential-equation), $y_1=x$ and $y_2=x\operatorname{arctanh}x-1$ illustrate this cancellation at zero.

##### Cauchy-Euler equation

↑ **Parent:** [Second-order linear differential equation](#second-order-linear-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cauchy–Euler_equation)

A Cauchy–Euler equation has powers of the independent variable matched to derivative order and is solved using power laws or a logarithmic change of variable.

###### Euler-Cauchy classification from two regular singular points

↑ **Parent:** [Cauchy-Euler equation](#cauchy-euler-equation)

Normalize the second-order equation as $y''+P(z)y'+Q(z)y=0$. If every point other than zero and infinity is ordinary and both exceptions are at worst [regular singular points](complex-analysis.md#regular-singular-point), then $zP$ and $z^2Q$ extend holomorphically across zero and stay bounded at infinity. [Liouville's theorem](complex-analysis.md#liouville-theorem) makes them constants, yielding the displayed [Euler-Cauchy equation](#euler-cauchy-equation). If both exceptions must be genuinely singular, exclude $(A,B)=(0,0)$ and $(2,0)$, which make zero and infinity respectively ordinary.

###### Euler-Cauchy equation

↑ **Parent:** [Cauchy-Euler equation](#cauchy-euler-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euler-Cauchy_equation)

###### General solution of an Euler-Cauchy equation

↑ **Parent:** [Cauchy-Euler equation](#cauchy-euler-equation)

For

$$
z^2w''+azw'+bw=0,
$$

the power ansatz $w=z^\lambda$ gives the indicial equation $\lambda(\lambda-1)+a\lambda+b=0$. Distinct roots give $C_1z^{\lambda_1}+C_2z^{\lambda_2}$; a repeated root $\lambda$ gives $z^\lambda(C_1+C_2\log z)$ on a chosen logarithm branch.

###### Power-law ansatz

↑ **Parent:** [General solution of an Euler-Cauchy equation](#general-solution-of-an-euler-cauchy-equation)

A power-law ansatz assumes that an unknown function is a monomial $y=x^s$. Scale-invariant differential equations then reduce to an algebraic equation for the exponent $s$.

###### Indicial equation

↑ **Parent:** [Power-law ansatz](#power-law-ansatz)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Indicial_equation)

An indicial equation is the algebraic equation for the leading exponent of a power-law or Frobenius solution near a regular singular point.

###### Indicial root

↑ **Parent:** [Indicial equation](#indicial-equation)

An [indicial root](#indicial-root) is a root of the [indicial equation](#indicial-equation) obtained from a [power-law ansatz](#power-law-ansatz). For a [Cauchy-Euler differential equation](#cauchy-euler-equation), such roots give the exponents of its power solutions. Their sign determines which modes remain bounded near a singular endpoint.

###### Indicial exponent

↑ **Parent:** [Indicial equation](#indicial-equation)

An indicial exponent is a root of the [indicial equation](#indicial-equation) at a [regular singular point](complex-analysis.md#regular-singular-point). It gives the leading local power in a [Frobenius method](complex-analysis.md#frobenius-method); resonant roots can require logarithmic terms.

###### Log-periodic oscillation

↑ **Parent:** [Power-law ansatz](#power-law-ansatz)

A log-periodic oscillation is periodic in the logarithm of its argument, for example $\cos(\mu\log x)$. Its successive zeros or extrema therefore occur at radii in a geometric progression.

##### Legendre differential equation

↑ **Parent:** [Second-order linear differential equation](#second-order-linear-differential-equation)

The equation $(1-x^2)y\prime\prime-2xy\prime+\ell(\ell+1)y=0$ has polynomial solutions for nonnegative integer $\ell$.

The equation $(1-x^2)y\prime\prime-2xy\prime+\ell(\ell+1)y=0$ has the [Legendre polynomial](#legendre-polynomial) of degree $\ell$ as its normalized regular polynomial solution when $\ell$ is a nonnegative integer.

###### Associated Legendre differential equation

↑ **Parent:** [Legendre differential equation](#legendre-differential-equation)

This second-order linear differential equation extends the [Legendre differential equation](#legendre-differential-equation) by its order parameter $m$. Its solutions are [associated Legendre functions](#associated-legendre-function). In a degree-one potential problem, with $x=\tanh\eta$, two explicit solutions are $e^{m\eta}(m-\tanh\eta)$ and $e^{-m\eta}(m+\tanh\eta)$. Their [Wronskian](#wronskian) with respect to $\eta$ is $2m(1-m^2)$, so the two formulas are not a fundamental pair at $m=0$ or $m=\pm1$.

###### Associated Legendre function

↑ **Parent:** [Legendre differential equation](#legendre-differential-equation)

Associated Legendre functions solve $(1-x^2)y''-2xy'+[\nu(\nu+1)-\mu^2/(1-x^2)]y=0$. For integers $\ell\geq0$ and $0\leq m\leq\ell$, the regular solution is $P_\ell^m(x)=(-1)^m(1-x^2)^{m/2}(d/dx)^mP_\ell(x)$, using a [Legendre polynomial](#legendre-polynomial). It enters normalized [spherical harmonics](analysis.md#spherical-harmonic). Despite the traditional term associated Legendre polynomial, the factor $(1-x^2)^{m/2}$ is not a polynomial when $m$ is odd. Negative integer orders satisfy $P_\ell^{-m}=(-1)^m(\ell-m)!P_\ell^m/(\ell+m)!$.

###### Legendre polynomial

↑ **Parent:** [Legendre differential equation](#legendre-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Legendre_polynomial)

The polynomial solution of degree l normalized by P\_l(1)=1 is the Legendre polynomial P\_l.

###### Weighted orthogonality of Legendre polynomial derivatives

↑ **Parent:** [Legendre polynomial](#legendre-polynomial)

Differentiating the [Legendre differential equation](#legendre-differential-equation) gives $((1-x^2)^2R_n')'+(n-1)(n+2)(1-x^2)R_n=0$ for $R_n=P_n'$. Multiply the equations for two distinct indices by the opposite polynomial and subtract. The endpoint term vanishes because of $(1-x^2)^2$, giving the displayed weighted [orthogonality](linear-algebra.md#orthogonal-vectors). The zero polynomial $R_0$ is not a nonzero eigenfunction.

###### Generating function and norm of Legendre polynomials

↑ **Parent:** [Legendre polynomial](#legendre-polynomial)

With $P_n(1)=1$, the generating function satisfies $\partial_x(x^2\partial_xG)+\partial_t((1-t^2)\partial_tG)=0$. Expanding in [Legendre polynomials](#legendre-polynomial) gives $x^2a_n''+2xa_n'-n(n+1)a_n=0$. Boundedness at zero removes $x^{-n-1}$, and the value at $t=1$ makes $a_n=x^n$. Orthogonality then gives $\int_{-1}^1G^2dt=\sum_nk_nx^{2n}$. The integral is $x^{-1}\log((1+x)/(1-x))$, so $k_n=2/(2n+1)$. Uniform analyticity on compact subdiscs $|x|<1$ justifies the generating expansion and termwise calculations.

###### Orthogonality of Legendre polynomials

↑ **Parent:** [Legendre polynomial](#legendre-polynomial)

The Legendre polynomials are orthogonal on $[-1,1]$ with unit weight:

$$
\int_{-1}^1P_\ell(x)P_m(x)\,dx
=\frac{2}{2\ell+1}\delta_{\ell m}.
$$

###### Legendre polynomial recurrence relation

↑ **Parent:** [Legendre polynomial](#legendre-polynomial)

The three-term recurrence

$$
(2\ell+1)xP_\ell(x)
=(\ell+1)P_{\ell+1}(x)+\ell P_{\ell-1}(x)
$$

turns multiplication by $x$ into coupling between adjacent Legendre multipoles.

<h6 id="schlafli-contour-integral-for-legendre-polynomials">Schläfli contour integral for Legendre polynomials</h6>

↑ **Parent:** [Legendre polynomial](#legendre-polynomial)

For a contour enclosing $t$,

$$
P_n(t)=\frac1{2^{n+1}\pi i}
\oint\frac{(z^2-1)^n}{(z-t)^{n+1}}\,dz.
$$

###### Debye asymptotic for Legendre polynomials

↑ **Parent:** [Legendre polynomial](#legendre-polynomial)

For fixed $0<\theta<\pi$,

$$
P_n(\cos\theta)
\sim
\sqrt{\frac{2}{\pi n\sin\theta}}
\cos\left(\left(n+\frac12\right)\theta-\frac\pi4\right).
$$

###### Hyperbolic Debye asymptotic for Legendre polynomials

↑ **Parent:** [Debye asymptotic for Legendre polynomials](#debye-asymptotic-for-legendre-polynomials)

For fixed $\xi>0$,

$$
P_n(\cosh\xi)
\sim
\frac{e^{(n+1/2)\xi}}{\sqrt{2\pi n\sinh\xi}}.
$$

###### Legendre boundary layer at x equals one

↑ **Parent:** [Hyperbolic Debye asymptotic for Legendre polynomials](#hyperbolic-debye-asymptotic-for-legendre-polynomials)

The endpoint [Laplace method](analysis.md#laplace-s-method) for a [Legendre polynomial](#legendre-polynomial) ceases to localize when $n\sqrt{x-1}=O(1)$. On the scale $x=1+\nu/n^2$, its real integral representation gives

$$
P_n(1+\nu/n^2)\longrightarrow \frac1\pi\int_0^\pi e^{\sqrt{2\nu}\cos\theta}\,d\theta=I_0(\sqrt{2\nu}).
$$

The [Modified Bessel function of the first kind](analysis.md#modified-bessel-function-of-the-first-kind) equals one at $\nu=0$ and has large-$\nu$ behavior $e^{\sqrt{2\nu}}/\sqrt{2\pi\sqrt{2\nu}}$, matching the [Hyperbolic Debye asymptotic for Legendre polynomials](#hyperbolic-debye-asymptotic-for-legendre-polynomials). This [boundary layer](continuum-mechanics.md#boundary-layer) resolves an increasingly steep function at an endpoint where its value remains fixed.

##### Change of independent variable in a second-order ODE

↑ **Parent:** [Second-order linear differential equation](#second-order-linear-differential-equation)

For $z=z(x)$, the second derivative transforms as $w_{xx}=z_x^2w_{zz}+z_{xx}w_z$.

#### First-order linear differential equation

↑ **Parent:** [Linear ordinary differential equation](#linear-ordinary-differential-equation)

A first-order linear differential equation has the form $y'+p(x)y=q(x)$. Multiplication by an integrating factor $\mu$ satisfying $\mu'=p\mu$ turns it into $(\mu y)'=\mu q$.

##### Causal response of a first-order relaxation equation

↑ **Parent:** [First-order linear differential equation](#first-order-linear-differential-equation)

For $\alpha>0$, the retarded [impulse response](analysis.md#impulse-response) of $\alpha y'+y=f$ is the displayed function, with $H$ the [Heaviside step function](analysis.md#heaviside-step-function). The corresponding [convolution](fourier-analysis.md#convolution) $y(t)=\alpha^{-1}\int_{-\infty}^t e^{-(t-s)/\alpha}f(s)\,ds$ is the unique solution tending to zero in the remote past whenever the integral exists and has that limit. For example, bounded forcing that tends to zero as $t\to-\infty$ satisfies these conditions. A general forcing need not: $f\equiv1$ admits no such solution. A unit-duration pulse with $\alpha=1$ gives $y=0$ before zero, $y=1-e^{-t}$ between zero and one, and $y=(1-e^{-1})e^{-(t-1)}$ thereafter.

##### Resonant exponential forcing in a first-order equation

↑ **Parent:** [First-order linear differential equation](#first-order-linear-differential-equation)

For $y\prime-ay=e^{\lambda x}$, subtracting an appropriate [homogeneous solution](#homogeneous-solution) from the [particular solution](#particular-solution) removes its apparent singularity as $\lambda\to a$. The resulting derivative in the parameter produces the resonant particular solution $xe^{ax}$. The arbitrary constant must be reparametrized before taking the limit.

#### Integrating factor

↑ **Parent:** [Linear ordinary differential equation](#linear-ordinary-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Integrating_factor)

An integrating factor turns a first-order linear equation into an exact derivative.

##### Heaviside forcing in a first-order integrating-factor equation

↑ **Parent:** [Integrating factor](#integrating-factor)

For $y'+a(x)y=H(x)$ with continuous $a$, the [integrating factor](#integrating-factor) $\mu=\exp(\int a)$ gives the displayed solution. It is continuous at the step and solves the [differential equation](differential-equation.md) classically on each side; the derivative jumps by one. The value assigned to the [Heaviside step function](analysis.md#heaviside-step-function) at the single point zero does not affect the integral. A discontinuity in $y$ would instead produce an unintended delta term in its distributional derivative.

##### Integrating factor for a differential one-form

↑ **Parent:** [Integrating factor](#integrating-factor)

For the [differential one-form](differential-form.md#one-form) $f\,dy+g\,dx$, a nonzero integrating factor $\mu$ makes $\mu f\,dy+\mu g\,dx$ an [exact differential form](differential-form.md#exact-differential-form) locally. If it equals $dF$, then $F_y=\mu f$, $F_x=\mu g$, and equality of mixed [partial derivatives](calculus.md#partial-derivative) gives the displayed compatibility condition. Conversely this condition is local sufficiency for smooth coefficients on a small rectangle; global exactness additionally depends on the domain. Zeros of the multiplying factor can change the solution set, so equivalence is asserted only where the factor is nonzero.

##### Bounded solution selected by a terminal condition

↑ **Parent:** [Integrating factor](#integrating-factor)

For a first-order linear equation whose homogeneous solution grows at infinity, boundedness fixes the integration constant by rewriting the particular integral as a tail integral from the current point to infinity.

#### Resonance in a differential equation

↑ **Parent:** [Linear ordinary differential equation](#linear-ordinary-differential-equation)

Resonance occurs when forcing overlaps a homogeneous mode, requiring multiplication of the usual particular ansatz by an extra power or logarithm.

##### Resonance condition

↑ **Parent:** [Resonance in a differential equation](#resonance-in-a-differential-equation)

A resonance condition is the relation between forcing parameters and a homogeneous mode that makes the forcing operator singular on that mode. A repeated inversion then produces algebraic amplitude growth.

##### Resonant forcing

↑ **Parent:** [Resonance in a differential equation](#resonance-in-a-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Resonant_forcing)

When forcing matches a natural frequency, the oscillator response acquires a linearly growing amplitude.

#### Linear system of differential equations

↑ **Parent:** [Linear ordinary differential equation](#linear-ordinary-differential-equation)

A linear differential system has vector form $x\prime=A(t)x+b(t)$.

##### Exponential forcing of a constant-coefficient differential system

↑ **Parent:** [Linear system of differential equations](#linear-system-of-differential-equations)

For $x'-Ax=e^{\lambda t}v$, substituting an exponential particular solution reduces the differential equation to $(\lambda I-A)u=v$. The displayed solution exists whenever $\lambda$ is not an [eigenvalue](linear-operator-theory.md#eigenvalue) of $A$. Resonance can require polynomial factors in time. The general solution adds $e^{tA}c$, expressed using the [matrix exponential](linear-operator-theory.md#matrix-exponential).

##### Cauchy-Euler differential system

↑ **Parent:** [Linear system of differential equations](#linear-system-of-differential-equations)

An [eigenvector](linear-operator-theory.md#eigenvector) of $A$ with [eigenvalue](linear-operator-theory.md#eigenvalue) $\lambda$ gives a homogeneous solution $t^\lambda\mathbf v$ for $t>0$. If $A$ is diagonalizable, these powers form a fundamental system. A constant vector forcing has a particular solution $t(I-A)^{-1}\mathbf b$ when $1$ is not an [eigenvalue](linear-operator-theory.md#eigenvalue). At a resonant [eigenvalue](linear-operator-theory.md#eigenvalue) or a nontrivial Jordan block, logarithmic factors in $t$ can occur, equivalently by changing time to $\log t$ and solving a constant-coefficient linear system.

##### Eigenvector method for a differential equation

↑ **Parent:** [Linear system of differential equations](#linear-system-of-differential-equations)

For a constant coefficient system, eigenvectors split the homogeneous equation into scalar exponential or power-law modes.

##### State transition matrix

↑ **Parent:** [Linear system of differential equations](#linear-system-of-differential-equations)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/State_transition_matrix)

A state transition matrix maps the state of a homogeneous linear system between two times.

##### Complex form of a planar linear system

↑ **Parent:** [Linear system of differential equations](#linear-system-of-differential-equations)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complex_form_of_a_planar_linear_system)

Encoding two planar components as one complex variable turns a rotation-dilation system into a scalar complex equation.

#### Jump condition for an impulse

↑ **Parent:** [Linear ordinary differential equation](#linear-ordinary-differential-equation)

Integrating an equation through a Dirac impulse determines the jump in the derivative or state while nonsingular lower-order terms contribute no jump.

##### Impulse cancellation of a harmonic oscillator

↑ **Parent:** [Jump condition for an impulse](#jump-condition-for-an-impulse)

For the [harmonic oscillator equation](classical-mechanics.md#simple-harmonic-motion) $y''+\omega^2y=J\delta(t-t_*)$, with $\omega>0$, the displacement is continuous and the velocity increases by $J$ at the impulse. If the incoming displacement is zero and $J=-y'(t_*-)$, the outgoing displacement and velocity both vanish. The subsequent [homogeneous solution](#homogeneous-solution) is identically zero. Equivalently, the causal forced response $(J/\omega)H(t-t_*)\sin(\omega(t-t_*))$ cancels the pre-existing oscillation, where $H$ is the [Heaviside step function](analysis.md#heaviside-step-function).

### First integral

↑ **Parent:** [Ordinary differential equation](#ordinary-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/First_integral)

A first integral is a function of time, state, and derivatives that remains constant along every solution.

## ↑ Ancestors (4)

1. [Analysis](analysis.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (59)

- [Boundary condition](#boundary-condition)
- [Classical solution of an abstract Cauchy problem](functional-analysis.md#classical-solution-of-an-abstract-cauchy-problem)
- [Collocation method](numerical-analysis.md#collocation-method)
- [Difference equation](real-analysis.md#difference-equation)
- [Euler discretization of logistic growth](#euler-discretization-of-logistic-growth)
- [General solution](#general-solution)
- [Geodesic reparametrization under projective equivalence](fiber-bundle.md#geodesic-reparametrization-under-projective-equivalence)
- [Heaviside forcing in a first-order integrating-factor equation](#heaviside-forcing-in-a-first-order-integrating-factor-equation)
- [Integral representation](calculus.md#integral-representation)
- [Isocline](#isocline)
- [Jump condition](#jump-condition)
- [Large-argument asymptotic expansion of a modified Bessel function](analysis.md#large-argument-asymptotic-expansion-of-a-modified-bessel-function)
- [Mehrstellen method](finite-difference.md#mehrstellen-method)
- [Mode shape](wave-equation.md#mode-shape)
- [Modified Bessel differential equation](analysis.md#modified-bessel-differential-equation)
- [Normalizable zero mode of a polynomial factorized Hamiltonian](quantum-mechanics.md#normalizable-zero-mode-of-a-polynomial-factorized-hamiltonian)
- [Optimal control](control-theory.md#optimal-control)
- [Painlevé property](#painleve-property)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1.md#11c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-1.md#12c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-2.md#5d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-2.md#6d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-2.md#7d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-26.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-57.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-66.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-28.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-8.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-8.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-2.md#1b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-2.md#5b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-4.md#4a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-4.md#9a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-55.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-76.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-2.md#1b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-2.md#6b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-2.md#15e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-2.md#16b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-83.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-2.md#1b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-2.md#7b/i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-33.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-2.md#34d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-59.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2.md#28b/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2.md#29d/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-1.md#14a/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-336.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-1.md#14b/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#31a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4.md#30e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4.md#7e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-349.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-2.md#17b/a/solution)
- [Solution of a differential equation](#solution-of-a-differential-equation)
- [Spectral parameter for a linear boundary value problem](#spectral-parameter-for-a-linear-boundary-value-problem)
