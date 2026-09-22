# Stochastic process

↑ **Parent:** [Probability theory](probability-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stochastic_process)

A stochastic process is a family of random variables indexed by time or another ordered parameter.

**Table of contents**

- [Skorokhod problem](#skorokhod-problem)
  - [Skorokhod reflection map on the half-line](#skorokhod-reflection-map-on-the-half-line)
- [Self-similarity of a stochastic process](#self-similarity-of-a-stochastic-process)
- [Random field](#random-field)
- [Locally bounded process](#locally-bounded-process)
- [Branching process](#branching-process)
  - [Multitype Poisson branching process](#multitype-poisson-branching-process)
    - [Spectral survival criterion for multitype Poisson branching](#spectral-survival-criterion-for-multitype-poisson-branching)
- [Unnormalized time autocorrelation](#unnormalized-time-autocorrelation)
  - [Intrawell phase autocorrelation](#intrawell-phase-autocorrelation)
- [Sample path](#sample-path)
- [Bounded increments](#bounded-increments)
  - [Bounded-increment martingale convergence-or-oscillation dichotomy](#bounded-increment-martingale-convergence-or-oscillation-dichotomy)
    - [Oscillation of a bounded centered iid random walk](#oscillation-of-a-bounded-centered-iid-random-walk)
- [Locally defined stochastic process](#locally-defined-stochastic-process)
  - [Local solution of a stochastic differential equation](#local-solution-of-a-stochastic-differential-equation)
- [Stochastic interval](#stochastic-interval)
- [Modification of a stochastic process](#modification-of-a-stochastic-process)
  - [Càdlàg modification](#cadlag-modification)
  - [Continuous modification](#continuous-modification)
- [Linear fluctuating interface](#linear-fluctuating-interface)
  - [Stationary spectrum of a linear fluctuating interface](#stationary-spectrum-of-a-linear-fluctuating-interface)
  - [Brownian zero mode of a fluctuating interface](#brownian-zero-mode-of-a-fluctuating-interface)
- [Path probability](#path-probability)
- [Langevin dynamics](#langevin-dynamics)
- [Interacting particle system](#interacting-particle-system)
  - [Voter model](#voter-model)
    - [Voter-model duality](#voter-model-duality)
      - [Finite-seed local extinction in the voter model](#finite-seed-local-extinction-in-the-voter-model)
      - [Invariant measures of the two-dimensional voter model](#invariant-measures-of-the-two-dimensional-voter-model)
  - [Exclusion process](#exclusion-process)
    - [Symmetric simple exclusion process](#symmetric-simple-exclusion-process)
      - [Bernoulli invariant laws of finite symmetric exclusion](#bernoulli-invariant-laws-of-finite-symmetric-exclusion)
      - [Stirring representation of symmetric exclusion](#stirring-representation-of-symmetric-exclusion)
        - [Product self-duality of symmetric exclusion](#product-self-duality-of-symmetric-exclusion)
          - [Exchangeable invariant laws of symmetric exclusion](#exchangeable-invariant-laws-of-symmetric-exclusion)
  - [Contact process](#contact-process)
    - [Exponential cardinality supermartingale for the contact process on a tree](#exponential-cardinality-supermartingale-for-the-contact-process-on-a-tree)
    - [Extremal invariant measures of the contact process](#extremal-invariant-measures-of-the-contact-process)
    - [Branching bound for contact-process survival](#branching-bound-for-contact-process-survival)
    - [Graphical representation of the contact process](#graphical-representation-of-the-contact-process)
      - [Independent oriented-percolation comparison for the contact process](#independent-oriented-percolation-comparison-for-the-contact-process)
      - [Dimension comparison for the contact process](#dimension-comparison-for-the-contact-process)
      - [Additivity of the contact process](#additivity-of-the-contact-process)
      - [Duality of the contact process](#duality-of-the-contact-process)
    - [Survival probability of the contact process](#survival-probability-of-the-contact-process)
      - [Local survival threshold of the contact process](#local-survival-threshold-of-the-contact-process)
        - [Height-weighted local extinction bound for the contact process](#height-weighted-local-extinction-bound-for-the-contact-process)
      - [Global survival threshold of the contact process](#global-survival-threshold-of-the-contact-process)
        - [Two-vertex branching comparison for contact-process survival](#two-vertex-branching-comparison-for-contact-process-survival)
- [Telegraph process](#telegraph-process)
  - [Diffusion limit of the telegraph process](#diffusion-limit-of-the-telegraph-process)
- [Stationary increments](#stationary-increments)
- [Independent increments](#independent-increments)
- [Finite-dimensional distribution](#finite-dimensional-distribution)
  - [Kolmogorov extension theorem](#kolmogorov-extension-theorem)
- [Covariance function](#covariance-function)
- [Kolmogorov continuity theorem](#kolmogorov-continuity-theorem)
  - [Dyadic increment chaining](#dyadic-increment-chaining)
- [Brownian snake](#brownian-snake)
  - [Hölder regularity of the Brownian snake](#holder-regularity-of-the-brownian-snake)
- [Schramm–Loewner evolution](#schramm-loewner-evolution)
  - [Cardy boundary crossing formula](#cardy-boundary-crossing-formula)
  - [Chordal SLE4](#chordal-sle4)
  - [Radial Schramm–Loewner evolution](#radial-schramm-loewner-evolution)
    - [Radial SLE2](#radial-sle2)
  - [Scale-and-domain-Markov characterization of SLE](#scale-and-domain-markov-characterization-of-sle)
  - [SLE angle process](#sle-angle-process)
    - [Dirichlet boundary values of the SLE angle process](#dirichlet-boundary-values-of-the-sle-angle-process)
    - [Logarithmic martingale for SLE4](#logarithmic-martingale-for-sle4)
      - [Fixed-interior-point avoidance of SLE4](#fixed-interior-point-avoidance-of-sle4)
    - [SLE4 angle martingale](#sle4-angle-martingale)
    - [SLE interior-point martingale](#sle-interior-point-martingale)
  - [Compact H-hull](#compact-h-hull)
    - [Mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull)
      - [Monotonicity of boundary derivatives of mapping-out functions](#monotonicity-of-boundary-derivatives-of-mapping-out-functions)
      - [Differentiability estimate for a mapping-out function](#differentiability-estimate-for-a-mapping-out-function)
      - [High-level escape representation of a mapping-out height](#high-level-escape-representation-of-a-mapping-out-height)
      - [Height contraction of a hydrodynamically normalized mapping-out function](#height-contraction-of-a-hydrodynamically-normalized-mapping-out-function)
      - [Inverse-at-infinity criterion for local boundedness of a mapping-out function](#inverse-at-infinity-criterion-for-local-boundedness-of-a-mapping-out-function)
      - [Mapping-out function of a vertical slit](#mapping-out-function-of-a-vertical-slit)
      - [Real boundary bounds for a unit-disc H-hull](#real-boundary-bounds-for-a-unit-disc-h-hull)
        - [Sharp displacement bound for a compact H-hull](#sharp-displacement-bound-for-a-compact-h-hull)
          - [Nearly closed semicircular slit](#nearly-closed-semicircular-slit)
      - [Hydrodynamic normalization at infinity](#hydrodynamic-normalization-at-infinity)
      - [Half-plane capacity](#half-plane-capacity)
        - [Half-plane capacity versus harmonic hull capacity](#half-plane-capacity-versus-harmonic-hull-capacity)
        - [Half-plane capacity of a half-disc](#half-plane-capacity-of-a-half-disc)
        - [Conformal change of half-plane capacity](#conformal-change-of-half-plane-capacity)
          - [Conformal conjugacy derivative for the chordal Loewner equation](#conformal-conjugacy-derivative-for-the-chordal-loewner-equation)
            - [Boundary derivative diffusion under conformal Loewner conjugacy](#boundary-derivative-diffusion-under-conformal-loewner-conjugacy)
            - [Transformed SLE driving function](#transformed-sle-driving-function)
        - [Half-plane capacity of a vertical slit](#half-plane-capacity-of-a-vertical-slit)
        - [Scaling and translation of half-plane capacity](#scaling-and-translation-of-half-plane-capacity)
        - [Monotonicity of half-plane capacity](#monotonicity-of-half-plane-capacity)
          - [Half-plane-capacity composition rule](#half-plane-capacity-composition-rule)
        - [Brownian representation of half-plane capacity](#brownian-representation-of-half-plane-capacity)
        - [Half-plane capacity is bounded by squared diameter](#half-plane-capacity-is-bounded-by-squared-diameter)
        - [Half-plane capacity of a low rectangle](#half-plane-capacity-of-a-low-rectangle)
        - [Half-plane-capacity parameterization](#half-plane-capacity-parameterization)
      - [Boundary degeneration under a mapping-out function](#boundary-degeneration-under-a-mapping-out-function)
  - [Loewner chain](#loewner-chain)
    - [Domain Markov property of a chordal Loewner chain](#domain-markov-property-of-a-chordal-loewner-chain)
      - [Simplicity of SLE from boundary-avoiding restarts](#simplicity-of-sle-from-boundary-avoiding-restarts)
    - [Capacity-parametrized scale invariance of a Loewner chain](#capacity-parametrized-scale-invariance-of-a-loewner-chain)
    - [Trace of a Loewner chain](#trace-of-a-loewner-chain)
      - [Boundary extension of the inverse map for a continuous Loewner trace](#boundary-extension-of-the-inverse-map-for-a-continuous-loewner-trace)
    - [Loewner local growth property](#loewner-local-growth-property)
      - [Loewner correspondence theorem](#loewner-correspondence-theorem)
    - [Loewner differential equation](#loewner-differential-equation)
      - [Chordal Loewner equation](#chordal-loewner-equation)
        - [Loewner variation of the Dirichlet Green function](#loewner-variation-of-the-dirichlet-green-function)
        - [Boundary-point swallowing time for a Loewner chain](#boundary-point-swallowing-time-for-a-loewner-chain)
          - [SLE boundary swallowing criterion](#sle-boundary-swallowing-criterion)
        - [Interior-point swallowing time for a Loewner chain](#interior-point-swallowing-time-for-a-loewner-chain)
        - [Loewner driving function](#loewner-driving-function)
          - [Continuity estimate for the Loewner driving function](#continuity-estimate-for-the-loewner-driving-function)
          - [Driving-function reconstruction for a chordal Loewner chain](#driving-function-reconstruction-for-a-chordal-loewner-chain)
          - [Composition rule for chordal Loewner driving functions](#composition-rule-for-chordal-loewner-driving-functions)
          - [Square-root Loewner driving function generates a straight slit](#square-root-loewner-driving-function-generates-a-straight-slit)
          - [Boundary derivative of a chordal Loewner chain](#boundary-derivative-of-a-chordal-loewner-chain)
  - [Scaling invariance of SLE](#scaling-invariance-of-sle)
    - [SLE reaches every positive height](#sle-reaches-every-positive-height)
  - [Conformal Markov property of SLE](#conformal-markov-property-of-sle)
    - [Characterization of the SLE driving function](#characterization-of-the-sle-driving-function)
  - [Conformal invariance of SLE](#conformal-invariance-of-sle)
    - [Chordal SLE in a specified scale](#chordal-sle-in-a-specified-scale)
    - [Chordal restriction property](#chordal-restriction-property)
      - [Restriction exponent of a chordal filling](#restriction-exponent-of-a-chordal-filling)
      - [Chordal filling](#chordal-filling)
        - [Avoidance probabilities determine a chordal filling law](#avoidance-probabilities-determine-a-chordal-filling-law)
      - [Derivative avoidance criterion for chordal restriction](#derivative-avoidance-criterion-for-chordal-restriction)
      - [Avoidance probabilities determine a simple chordal curve law](#avoidance-probabilities-determine-a-simple-chordal-curve-law)
      - [SLE eight-thirds restriction martingale](#sle-eight-thirds-restriction-martingale)
    - [Locality property of SLE](#locality-property-of-sle)
      - [Locality of a chord law under conformal changes of neighborhoods](#locality-of-a-chord-law-under-conformal-changes-of-neighborhoods)
      - [Target-change locality of SLE6](#target-change-locality-of-sle6)
        - [Target-dependent continuation of SLE6](#target-dependent-continuation-of-sle6)
  - [Phase classification of the SLE trace](#phase-classification-of-the-sle-trace)
    - [Space-filling SLE above parameter eight](#space-filling-sle-above-parameter-eight)
    - [SLE Green-function estimate](#sle-green-function-estimate)
    - [SLE4 left-passage probability](#sle4-left-passage-probability)
    - [Boundary-intersection threshold for SLE](#boundary-intersection-threshold-for-sle)
      - [Positive boundary-interval hitting probability for SLE above parameter four](#positive-boundary-interval-hitting-probability-for-sle-above-parameter-four)
  - [Transience of chordal SLE](#transience-of-chordal-sle)
  - [Reverse Loewner flow](#reverse-loewner-flow)
    - [Reverse SLE derivative martingale](#reverse-sle-derivative-martingale)
      - [Reverse SLE derivative bound above the space-filling threshold](#reverse-sle-derivative-bound-above-the-space-filling-threshold)
  - [Boundary-point Bessel flow for SLE](#boundary-point-bessel-flow-for-sle)
    - [Boundary approach forces a small SLE Bessel gap](#boundary-approach-forces-a-small-sle-bessel-gap)
    - [SLE two-boundary-point ratio diffusion](#sle-two-boundary-point-ratio-diffusion)
      - [Strict ordering threshold for SLE boundary swallowing](#strict-ordering-threshold-for-sle-boundary-swallowing)
        - [Real-line visitation from strict SLE swallowing order](#real-line-visitation-from-strict-sle-swallowing-order)
    - [SLE boundary-point logarithmic separation diffusion](#sle-boundary-point-logarithmic-separation-diffusion)
      - [SLE does not hit a fixed nonzero boundary point](#sle-does-not-hit-a-fixed-nonzero-boundary-point)
    - [Two-sided SLE boundary swallowing probability](#two-sided-sle-boundary-swallowing-probability)
- [Infinitesimal generator (stochastic processes)](#infinitesimal-generator-stochastic-processes)
  - [Dynkin's formula](#dynkin-s-formula)
  - [Diffusion generator](#diffusion-generator)
    - [Dynkin formula for a diffusion](#dynkin-formula-for-a-diffusion)
- [Filtration (probability theory)](#filtration-probability-theory)
  - [Dyadic filtration](#dyadic-filtration)
  - [Filtered probability space](#filtered-probability-space)
    - [Usual conditions for a filtration](#usual-conditions-for-a-filtration)
  - [Left-limit sigma-algebra](#left-limit-sigma-algebra)
- [Natural filtration](#natural-filtration)
- [Adapted process](#adapted-process)
  - [Adaptedness of a stopped right-continuous process](#adaptedness-of-a-stopped-right-continuous-process)
  - [Progressive measurability](#progressive-measurability)
    - [Almost sure path regularity does not ensure progressive measurability](#almost-sure-path-regularity-does-not-ensure-progressive-measurability)
    - [Right-continuous adapted processes are progressively measurable](#right-continuous-adapted-processes-are-progressively-measurable)
- [Uniform convergence on compacts in probability](#uniform-convergence-on-compacts-in-probability)
  - [Uniform convergence on compacts in probability under an absolutely continuous measure change](#uniform-convergence-on-compacts-in-probability-under-an-absolutely-continuous-measure-change)
- [Càdlàg process](#cadlag-process)
- [Time change of a continuous process](#time-change-of-a-continuous-process)
  - [Optional time-change theorem](#optional-time-change-theorem)
- [Indistinguishability of stochastic processes](#indistinguishability-of-stochastic-processes)
  - [Càdlàg versions are indistinguishable](#cadlag-versions-are-indistinguishable)
- [Stochastic calculus](stochastic-calculus.md)
  - [Itô process](stochastic-calculus.md#ito-process)
  - [Stochastic Fubini theorem](stochastic-calculus.md#stochastic-fubini-theorem)
  - [Semimartingale](stochastic-calculus.md#semimartingale)
    - [Continuous semimartingale](stochastic-calculus.md#continuous-semimartingale)
    - [Semimartingale stability under an absolutely continuous measure change](stochastic-calculus.md#semimartingale-stability-under-an-absolutely-continuous-measure-change)
      - [Stochastic integral under an absolutely continuous measure change](stochastic-calculus.md#stochastic-integral-under-an-absolutely-continuous-measure-change)
    - [Bichteler-Dellacherie theorem](stochastic-calculus.md#bichteler-dellacherie-theorem)
    - [Finite-variation process](stochastic-calculus.md#finite-variation-process)
      - [Total-variation process](stochastic-calculus.md#total-variation-process)
        - [Càdlàg regularity of finite total variation](stochastic-calculus.md#cadlag-regularity-of-finite-total-variation)
    - [Semimartingale decomposition](stochastic-calculus.md#semimartingale-decomposition)
      - [Continuous semimartingale decomposition](stochastic-calculus.md#continuous-semimartingale-decomposition)
        - [Initial-value integrability in normalized semimartingale decompositions](stochastic-calculus.md#initial-value-integrability-in-normalized-semimartingale-decompositions)
  - [Quadratic variation](stochastic-calculus.md#quadratic-variation)
    - [Predictable quadratic variation](stochastic-calculus.md#predictable-quadratic-variation)
    - [Uniqueness of an increasing square compensator](stochastic-calculus.md#uniqueness-of-an-increasing-square-compensator)
    - [Dyadic quadratic variation of a bounded continuous martingale](stochastic-calculus.md#dyadic-quadratic-variation-of-a-bounded-continuous-martingale)
    - [Finite-variation terms do not change quadratic variation](stochastic-calculus.md#finite-variation-terms-do-not-change-quadratic-variation)
    - [Localization and patching of quadratic variation](stochastic-calculus.md#localization-and-patching-of-quadratic-variation)
    - [Quadratic variation from completed grid increments](stochastic-calculus.md#quadratic-variation-from-completed-grid-increments)
    - [Weighted realized variance](stochastic-calculus.md#weighted-realized-variance)
      - [Spot variance](stochastic-calculus.md#spot-variance)
    - [Quadratic variation obstruction to Hölder regularity](stochastic-calculus.md#quadratic-variation-obstruction-to-holder-regularity)
    - [Dyadic quadratic variation of Brownian motion](stochastic-calculus.md#dyadic-quadratic-variation-of-brownian-motion)
    - [Dyadic power variation of a continuous local martingale](stochastic-calculus.md#dyadic-power-variation-of-a-continuous-local-martingale)
    - [Quadratic covariation](stochastic-calculus.md#quadratic-covariation)
      - [Quadratic covariations of an analytic Brownian image](stochastic-calculus.md#quadratic-covariations-of-an-analytic-brownian-image)
      - [Covariance identity for continuous square-integrable martingales](stochastic-calculus.md#covariance-identity-for-continuous-square-integrable-martingales)
      - [Weakly orthogonal continuous martingales](stochastic-calculus.md#weakly-orthogonal-continuous-martingales)
      - [Orthogonal continuous local martingales](stochastic-calculus.md#orthogonal-continuous-local-martingales)
        - [Knight theorem for orthogonal martingales](stochastic-calculus.md#knight-theorem-for-orthogonal-martingales)
        - [Complex exponential of two orthogonal Brownian motions](stochastic-calculus.md#complex-exponential-of-two-orthogonal-brownian-motions)
      - [Quadratic covariation under an absolutely continuous measure change](stochastic-calculus.md#quadratic-covariation-under-an-absolutely-continuous-measure-change)
        - [Quadratic variation under an absolutely continuous measure change](stochastic-calculus.md#quadratic-variation-under-an-absolutely-continuous-measure-change)
      - [Martingale product identity](stochastic-calculus.md#martingale-product-identity)
      - [Kunita-Watanabe inequality](stochastic-calculus.md#kunita-watanabe-inequality)
      - [Realized absolute covariation](stochastic-calculus.md#realized-absolute-covariation)
    - [Pathwise quadratic variation distinguishes Brownian speeds](stochastic-calculus.md#pathwise-quadratic-variation-distinguishes-brownian-speeds)
  - [Stochastic integral](stochastic-calculus.md#stochastic-integral)
    - [Semimartingale integration by parts](stochastic-calculus.md#semimartingale-integration-by-parts)
    - [Stochastic dominated convergence theorem](stochastic-calculus.md#stochastic-dominated-convergence-theorem)
    - [Left-endpoint approximation of a continuous semimartingale integral](stochastic-calculus.md#left-endpoint-approximation-of-a-continuous-semimartingale-integral)
    - [Stopping-time shift of a stochastic integral](stochastic-calculus.md#stopping-time-shift-of-a-stochastic-integral)
    - [Conditionally Gaussian stochastic integral with an independent integrator](stochastic-calculus.md#conditionally-gaussian-stochastic-integral-with-an-independent-integrator)
    - [Stratonovich integral](stochastic-calculus.md#stratonovich-integral)
      - [Stratonovich chain rule](stochastic-calculus.md#stratonovich-chain-rule)
    - [Itô integral](stochastic-calculus.md#ito-integral)
      - [Gaussianity of deterministic Brownian stochastic integrals](stochastic-calculus.md#gaussianity-of-deterministic-brownian-stochastic-integrals)
      - [Gaussian coordinates of deterministic orthonormal Wiener integrands](stochastic-calculus.md#gaussian-coordinates-of-deterministic-orthonormal-wiener-integrands)
      - [Recovery of a continuous Brownian integrand from short increments](stochastic-calculus.md#recovery-of-a-continuous-brownian-integrand-from-short-increments)
    - [Associativity of stochastic integration](stochastic-calculus.md#associativity-of-stochastic-integration)
    - [Itô isometry](stochastic-calculus.md#ito-isometry)
      - [Square-integrable stochastic integrand](stochastic-calculus.md#square-integrable-stochastic-integrand)
      - [Fractional-moment control of Brownian increment ratios](stochastic-calculus.md#fractional-moment-control-of-brownian-increment-ratios)
      - [Conditional bracket isometry for stopped martingale increments](stochastic-calculus.md#conditional-bracket-isometry-for-stopped-martingale-increments)
      - [Quadratic-variation measure](stochastic-calculus.md#quadratic-variation-measure)
    - [Quadratic variation of a stochastic integral](stochastic-calculus.md#quadratic-variation-of-a-stochastic-integral)
      - [Localized isometry proof of stochastic-integral quadratic variation](stochastic-calculus.md#localized-isometry-proof-of-stochastic-integral-quadratic-variation)
  - [Itô's lemma](stochastic-calculus.md#ito-s-lemma)
    - [Polynomial Itô formula from integration by parts](stochastic-calculus.md#polynomial-ito-formula-from-integration-by-parts)
    - [Itô formula for semimartingales with jumps](stochastic-calculus.md#ito-formula-for-semimartingales-with-jumps)
    - [Itô product rule](stochastic-calculus.md#ito-product-rule)
    - [Tanaka's formula](stochastic-calculus.md#tanaka-s-formula)
      - [Smooth convex approximation proof of the Tanaka formula](stochastic-calculus.md#smooth-convex-approximation-proof-of-the-tanaka-formula)
      - [Discrete Tanaka formula](stochastic-calculus.md#discrete-tanaka-formula)
  - [Local time (mathematics)](stochastic-calculus.md#local-time-mathematics)
    - [Local time of a semimartingale](stochastic-calculus.md#local-time-of-a-semimartingale)
      - [Brownian local time](stochastic-calculus.md#brownian-local-time)
        - [Occupation approximations for Brownian local time](stochastic-calculus.md#occupation-approximations-for-brownian-local-time)
          - [Ratio-one interpolation for shrinking-window occupation integrals](stochastic-calculus.md#ratio-one-interpolation-for-shrinking-window-occupation-integrals)
      - [Right local time of a continuous semimartingale](stochastic-calculus.md#right-local-time-of-a-continuous-semimartingale)
  - [Stochastic differential equation](stochastic-calculus.md#stochastic-differential-equation)
    - [Bounded diffusion coefficient gives square martingales](stochastic-calculus.md#bounded-diffusion-coefficient-gives-square-martingales)
    - [Bernoulli stochastic differential equation](stochastic-calculus.md#bernoulli-stochastic-differential-equation)
      - [Explosion threshold for a Bernoulli stochastic differential equation](stochastic-calculus.md#explosion-threshold-for-a-bernoulli-stochastic-differential-equation)
    - [Brownian rotation in the plane](stochastic-calculus.md#brownian-rotation-in-the-plane)
    - [Stroock-Varadhan support theorem](stochastic-calculus.md#stroock-varadhan-support-theorem)
    - [Square-root branching diffusion](stochastic-calculus.md#square-root-branching-diffusion)
      - [Cutoff construction of an absorbed square-root diffusion](stochastic-calculus.md#cutoff-construction-of-an-absorbed-square-root-diffusion)
      - [Addition law for square-root branching diffusions](stochastic-calculus.md#addition-law-for-square-root-branching-diffusions)
    - [Strict order preservation for scalar Lipschitz diffusions](stochastic-calculus.md#strict-order-preservation-for-scalar-lipschitz-diffusions)
      - [Reciprocal barrier proof of scalar diffusion comparison](stochastic-calculus.md#reciprocal-barrier-proof-of-scalar-diffusion-comparison)
    - [Global existence theorem for stochastic differential equations with Lipschitz coefficients](stochastic-calculus.md#global-existence-theorem-for-stochastic-differential-equations-with-lipschitz-coefficients)
    - [Tanaka equation](stochastic-calculus.md#tanaka-equation)
    - [Itô diffusion](stochastic-calculus.md#ito-diffusion)
      - [Exponential small-noise concentration for a Lipschitz diffusion](stochastic-calculus.md#exponential-small-noise-concentration-for-a-lipschitz-diffusion)
      - [Generator of an SDE diffusion](stochastic-calculus.md#generator-of-an-sde-diffusion)
      - [Initial mean and variance derivatives of an Itô diffusion](stochastic-calculus.md#initial-mean-and-variance-derivatives-of-an-ito-diffusion)
      - [Wright–Fisher diffusion](stochastic-calculus.md#wright-fisher-diffusion)
        - [Wright–Fisher binomial sampling chain](stochastic-calculus.md#wright-fisher-binomial-sampling-chain)
      - [Diffusion with hyperbolic tangent drift](stochastic-calculus.md#diffusion-with-hyperbolic-tangent-drift)
      - [Diffusion amplitude](stochastic-calculus.md#diffusion-amplitude)
      - [Diffusion occupation time](stochastic-calculus.md#diffusion-occupation-time)
      - [Power diffusion](stochastic-calculus.md#power-diffusion)
        - [Finite lifetime threshold for a power diffusion](stochastic-calculus.md#finite-lifetime-threshold-for-a-power-diffusion)
      - [Lamperti transform (diffusion)](stochastic-calculus.md#lamperti-transform-diffusion)
      - [Drift coefficient](stochastic-calculus.md#drift-coefficient)
        - [Drift estimator](stochastic-calculus.md#drift-estimator)
      - [Geometric Brownian motion](stochastic-calculus.md#geometric-brownian-motion)
        - [Killed geometric Brownian heat kernel](stochastic-calculus.md#killed-geometric-brownian-heat-kernel)
    - [Invariant distribution of an Itô diffusion](stochastic-calculus.md#invariant-distribution-of-an-ito-diffusion)
    - [Underdamped Langevin dynamics](stochastic-calculus.md#underdamped-langevin-dynamics)
      - [Inertial Brownian displacement with zero initial velocity](stochastic-calculus.md#inertial-brownian-displacement-with-zero-initial-velocity)
    - [Overdamped Langevin dynamics](stochastic-calculus.md#overdamped-langevin-dynamics)
      - [Isothermal diffusion with position-dependent drag](stochastic-calculus.md#isothermal-diffusion-with-position-dependent-drag)
      - [Tilted washboard potential](stochastic-calculus.md#tilted-washboard-potential)
      - [Kramers escape rate](stochastic-calculus.md#kramers-escape-rate)
    - [Euler-Maruyama method](stochastic-calculus.md#euler-maruyama-method)
      - [Milstein method](stochastic-calculus.md#milstein-method)
    - [Strong convergence of a stochastic numerical method](stochastic-calculus.md#strong-convergence-of-a-stochastic-numerical-method)
    - [Weak convergence of a stochastic numerical method](stochastic-calculus.md#weak-convergence-of-a-stochastic-numerical-method)
    - [Markov diffusion](stochastic-calculus.md#markov-diffusion)
      - [Driftless square-root diffusion](stochastic-calculus.md#driftless-square-root-diffusion)
        - [Compound Poisson transition law of a driftless square-root diffusion](stochastic-calculus.md#compound-poisson-transition-law-of-a-driftless-square-root-diffusion)
      - [Diffusion limit](stochastic-calculus.md#diffusion-limit)
      - [Speed density of a one-dimensional diffusion](stochastic-calculus.md#speed-density-of-a-one-dimensional-diffusion)
        - [Finite-interval diffusion exit Green kernel](stochastic-calculus.md#finite-interval-diffusion-exit-green-kernel)
    - [Maximal local solution of a stochastic differential equation](stochastic-calculus.md#maximal-local-solution-of-a-stochastic-differential-equation)
      - [Existence and pathwise uniqueness theorem for a stochastic differential equation](stochastic-calculus.md#existence-and-pathwise-uniqueness-theorem-for-a-stochastic-differential-equation)
        - [Linear growth condition for an SDE](stochastic-calculus.md#linear-growth-condition-for-an-sde)
          - [Maximal second-moment bound under linear growth](stochastic-calculus.md#maximal-second-moment-bound-under-linear-growth)
    - [Scale function (stochastic processes)](stochastic-calculus.md#scale-function-stochastic-processes)
      - [Arctangent transform of a two-noise affine diffusion](stochastic-calculus.md#arctangent-transform-of-a-two-noise-affine-diffusion)
        - [Endpoint convergence of a bounded angle diffusion](stochastic-calculus.md#endpoint-convergence-of-a-bounded-angle-diffusion)
      - [Scale transform for an additive-noise diffusion](stochastic-calculus.md#scale-transform-for-an-additive-noise-diffusion)
        - [Strong well-posedness of additive-noise equations with bounded continuous drift](stochastic-calculus.md#strong-well-posedness-of-additive-noise-equations-with-bounded-continuous-drift)
        - [Zero extension of a scale diffusion coefficient at finite endpoints](stochastic-calculus.md#zero-extension-of-a-scale-diffusion-coefficient-at-finite-endpoints)
      - [Boundary hitting probability from a diffusion scale function](stochastic-calculus.md#boundary-hitting-probability-from-a-diffusion-scale-function)
        - [Hypotheses for a diffusion scale hitting formula](stochastic-calculus.md#hypotheses-for-a-diffusion-scale-hitting-formula)
    - [Weak solution of a stochastic differential equation](stochastic-calculus.md#weak-solution-of-a-stochastic-differential-equation)
      - [Weak existence and uniqueness in law for an additive-noise SDE with bounded drift](stochastic-calculus.md#weak-existence-and-uniqueness-in-law-for-an-additive-noise-sde-with-bounded-drift)
    - [Strong solution of a stochastic differential equation](stochastic-calculus.md#strong-solution-of-a-stochastic-differential-equation)
      - [Strong existence](stochastic-calculus.md#strong-existence)
      - [Strong existence theorem for additive-noise SDEs with bounded measurable drift](stochastic-calculus.md#strong-existence-theorem-for-additive-noise-sdes-with-bounded-measurable-drift)
    - [Pathwise uniqueness](stochastic-calculus.md#pathwise-uniqueness)
    - [Uniqueness in law](stochastic-calculus.md#uniqueness-in-law)
    - [Kolmogorov backward equation](stochastic-calculus.md#kolmogorov-backward-equation)
      - [Bounded backward-equation stochastic representation](stochastic-calculus.md#bounded-backward-equation-stochastic-representation)
      - [Feynman-Kac formula](stochastic-calculus.md#feynman-kac-formula)
        - [Critical quadratic potential for the Ornstein-Uhlenbeck generator](stochastic-calculus.md#critical-quadratic-potential-for-the-ornstein-uhlenbeck-generator)
        - [Elliptic Feynman-Kac formula](stochastic-calculus.md#elliptic-feynman-kac-formula)
        - [Parabolic Feynman-Kac formula with a source](stochastic-calculus.md#parabolic-feynman-kac-formula-with-a-source)
        - [Discounted boundary-hitting representation](stochastic-calculus.md#discounted-boundary-hitting-representation)
        - [Feynman-Kac formula with a bounded potential](stochastic-calculus.md#feynman-kac-formula-with-a-bounded-potential)
          - [Soft killing limit for Brownian nonnegative survival](stochastic-calculus.md#soft-killing-limit-for-brownian-nonnegative-survival)
          - [Zero-noise limit with a bounded potential](stochastic-calculus.md#zero-noise-limit-with-a-bounded-potential)
          - [Positive-potential growth from Brownian recurrence](stochastic-calculus.md#positive-potential-growth-from-brownian-recurrence)
    - [Martingale problem](stochastic-calculus.md#martingale-problem)
      - [Martingale problem for Brownian motion](stochastic-calculus.md#martingale-problem-for-brownian-motion)
      - [Diffusion approximation theorem](stochastic-calculus.md#diffusion-approximation-theorem)
      - [Well-posed martingale problem](stochastic-calculus.md#well-posed-martingale-problem)
      - [Diffusion martingale problem](stochastic-calculus.md#diffusion-martingale-problem)
        - [Bounded-domain harmonic uniqueness for a diffusion](stochastic-calculus.md#bounded-domain-harmonic-uniqueness-for-a-diffusion)
        - [Projection unboundedness of a uniformly elliptic diffusion](stochastic-calculus.md#projection-unboundedness-of-a-uniformly-elliptic-diffusion)
        - [Time-dependent test functions for a diffusion martingale problem](stochastic-calculus.md#time-dependent-test-functions-for-a-diffusion-martingale-problem)
  - [Doléans-Dade exponential](stochastic-calculus.md#doleans-dade-exponential)
    - [Pathwise uniqueness for a multiplicative martingale equation](stochastic-calculus.md#pathwise-uniqueness-for-a-multiplicative-martingale-equation)
    - [Stochastic logarithm](stochastic-calculus.md#stochastic-logarithm)
      - [Divergent logarithmic clock for a positive local martingale tending to zero](stochastic-calculus.md#divergent-logarithmic-clock-for-a-positive-local-martingale-tending-to-zero)
    - [Kazamaki's condition](stochastic-calculus.md#kazamaki-s-condition)
    - [Terminal scaling inequality for stochastic exponentials](stochastic-calculus.md#terminal-scaling-inequality-for-stochastic-exponentials)
    - [Hölder factorization of stochastic exponentials](stochastic-calculus.md#holder-factorization-of-stochastic-exponentials)
      - [Half-threshold for the exponential-martingale Hölder bound](stochastic-calculus.md#half-threshold-for-the-exponential-martingale-holder-bound)
    - [Novikov's condition](stochastic-calculus.md#novikov-s-condition)
      - [Bounded-bracket criterion for a stochastic exponential](stochastic-calculus.md#bounded-bracket-criterion-for-a-stochastic-exponential)
      - [Dambis-Dubins-Schwarz proof of the Novikov condition](stochastic-calculus.md#dambis-dubins-schwarz-proof-of-the-novikov-condition)
    - [Girsanov theorem](stochastic-calculus.md#girsanov-theorem)
      - [Ornstein-Uhlenbeck likelihood relative to Wiener measure](stochastic-calculus.md#ornstein-uhlenbeck-likelihood-relative-to-wiener-measure)
      - [Bounded Girsanov density for exit of an unstable linear diffusion](stochastic-calculus.md#bounded-girsanov-density-for-exit-of-an-unstable-linear-diffusion)
      - [Semimartingale invariance under equivalent measures](stochastic-calculus.md#semimartingale-invariance-under-equivalent-measures)
      - [Finite-horizon drift replacement by a change of measure](stochastic-calculus.md#finite-horizon-drift-replacement-by-a-change-of-measure)
      - [Girsanov density for a stopped Bessel process](stochastic-calculus.md#girsanov-density-for-a-stopped-bessel-process)
        - [Brownian conditioning by a stopped Bessel density](stochastic-calculus.md#brownian-conditioning-by-a-stopped-bessel-density)
      - [Martingale transfer under a density process](stochastic-calculus.md#martingale-transfer-under-a-density-process)
        - [Initial integrability under a density change](stochastic-calculus.md#initial-integrability-under-a-density-change)
        - [Bounded-process density-product criterion](stochastic-calculus.md#bounded-process-density-product-criterion)
- [Stochastic continuity](#stochastic-continuity)
- [Lévy process](#levy-process)
  - [Continuous Lévy process](#continuous-levy-process)
  - [Atomic compound Poisson process with drift](#atomic-compound-poisson-process-with-drift)
  - [Closure of Lévy processes under locally controlled convergence in probability](#closure-of-levy-processes-under-locally-controlled-convergence-in-probability)
  - [Cauchy process](#cauchy-process)
    - [Self-similarity of a Cauchy process](#self-similarity-of-a-cauchy-process)
  - [Characteristic exponent of a Lévy process](#characteristic-exponent-of-a-levy-process)
    - [Exponential martingale of a Lévy process](#exponential-martingale-of-a-levy-process)
    - [Exponential form of Lévy characteristic functions](#exponential-form-of-levy-characteristic-functions)
    - [Continuity of Lévy characteristic functions](#continuity-of-levy-characteristic-functions)
  - [Subordination of a Lévy process](#subordination-of-a-levy-process)
  - [Subordinator](#subordinator)
    - [Brownian first-passage subordinator](#brownian-first-passage-subordinator)
      - [Countable dense jumps of the Brownian first-passage subordinator](#countable-dense-jumps-of-the-brownian-first-passage-subordinator)
  - [Lévy measure](#levy-measure)
    - [Lévy measure of a symmetric Laplace time-one law](#levy-measure-of-a-symmetric-laplace-time-one-law)
  - [Compound Poisson process](#compound-poisson-process)
    - [Independent compound Poisson jumps cannot cancel](#independent-compound-poisson-jumps-cannot-cancel)
    - [Grid-sampled compound Poisson workload bound](#grid-sampled-compound-poisson-workload-bound)
    - [Exponential Laplace martingale of a compound Poisson process](#exponential-laplace-martingale-of-a-compound-poisson-process)
    - [Difference of independent Poisson processes](#difference-of-independent-poisson-processes)
    - [Continuous-time symmetric simple random walk](#continuous-time-symmetric-simple-random-walk)
      - [Scaling classification of a continuous-time symmetric simple random walk](#scaling-classification-of-a-continuous-time-symmetric-simple-random-walk)
    - [Martingale compound Poisson process](#martingale-compound-poisson-process)
    - [Independent coordinates of a compound Poisson process](#independent-coordinates-of-a-compound-poisson-process)
  - [Lévy–Khintchine formula](#levy-khintchine-formula)
    - [Uncompensated Lévy–Khintchine formula](#uncompensated-levy-khintchine-formula)
    - [Lévy–Itô decomposition](#levy-ito-decomposition)
      - [Path and moment criteria from a Lévy triplet](#path-and-moment-criteria-from-a-levy-triplet)
  - [Centered square-integrable Lévy martingale](#centered-square-integrable-levy-martingale)
- [Gaussian process](#gaussian-process)
  - [Gaussian exponential martingale with deterministic variance](#gaussian-exponential-martingale-with-deterministic-variance)
  - [Covariance criterion for a stationary Gaussian Markov process](#covariance-criterion-for-a-stationary-gaussian-markov-process)
  - [Gaussian process construction from square-summable features](#gaussian-process-construction-from-square-summable-features)
  - [Canonical pseudometric of a Gaussian process](#canonical-pseudometric-of-a-gaussian-process)
  - [Fractional Brownian motion](#fractional-brownian-motion)
    - [Hurst exponent](#hurst-exponent)
  - [Sudakov-Fernique inequality](#sudakov-fernique-inequality)
  - [Slepian's lemma](#slepian-s-lemma)
  - [Mean-square derivative of a Gaussian process](#mean-square-derivative-of-a-gaussian-process)
    - [Differentiable modification of a stationary Gaussian process](#differentiable-modification-of-a-stationary-gaussian-process)
    - [Mean-square fundamental theorem of calculus](#mean-square-fundamental-theorem-of-calculus)
  - [Gaussian process classification](#gaussian-process-classification)
  - [Periodic covariance function](#periodic-covariance-function)
    - [Periodic Gaussian process with zero period average](#periodic-gaussian-process-with-zero-period-average)
  - [Gaussian-process marginal likelihood](#gaussian-process-marginal-likelihood)
  - [Gaussian concentration inequality](#gaussian-concentration-inequality)
    - [Brownian martingale proof of Gaussian concentration](#brownian-martingale-proof-of-gaussian-concentration)
    - [Gaussian rotation interpolation inequality](#gaussian-rotation-interpolation-inequality)
  - [Dudley entropy integral](#dudley-entropy-integral)
  - [Borell-TIS inequality](#borell-tis-inequality)
  - [Isonormal Gaussian process](#isonormal-gaussian-process)
    - [Exponential tilting of an isonormal Gaussian process](#exponential-tilting-of-an-isonormal-gaussian-process)
  - [Gaussian white noise](#gaussian-white-noise)
    - [Gaussian white noise model](#gaussian-white-noise-model)
    - [White-noise likelihood for a square-integrable shift](#white-noise-likelihood-for-a-square-integrable-shift)
    - [Gaussian sequence model](#gaussian-sequence-model)
      - [Bernstein-von Mises theorem](#bernstein-von-mises-theorem)
      - [Gaussian net test](#gaussian-net-test)
      - [Gaussian least-squares contrast](#gaussian-least-squares-contrast)
  - [Independent increments of a Gaussian martingale](#independent-increments-of-a-gaussian-martingale)
    - [Gaussian continuous martingale](#gaussian-continuous-martingale)
      - [Deterministic quadratic variation characterizes a Gaussian continuous local martingale](#deterministic-quadratic-variation-characterizes-a-gaussian-continuous-local-martingale)
  - [Exponential covariance function](#exponential-covariance-function)
  - [Gaussian random field](#gaussian-random-field)
    - [Brownian sheet](#brownian-sheet)
    - [Gaussian marginals do not imply a Gaussian random field](#gaussian-marginals-do-not-imply-a-gaussian-random-field)
    - [Centered quadratic Gaussian transformation](#centered-quadratic-gaussian-transformation)
    - [Exponential moment of a Gaussian linear functional](#exponential-moment-of-a-gaussian-linear-functional)
      - [Gaussian quadratic exponential moment](#gaussian-quadratic-exponential-moment)
    - [Stationary Gaussian random field](#stationary-gaussian-random-field)
      - [Autocorrelation function of a random field](#autocorrelation-function-of-a-random-field)
        - [Covariance of a squared random field](#covariance-of-a-squared-random-field)
    - [Novikov's theorem](#novikov-s-theorem)
    - [Markov approximation for a random medium](#markov-approximation-for-a-random-medium)
    - [Gaussian free field](#gaussian-free-field)
      - [Discrete Gaussian free field](#discrete-gaussian-free-field)
        - [Gaussian free field with Dirichlet boundary condition](#gaussian-free-field-with-dirichlet-boundary-condition)
          - [Gibbs-Markov property of the discrete Gaussian free field](#gibbs-markov-property-of-the-discrete-gaussian-free-field)
          - [Spatial Markov property of the Gaussian free field](#spatial-markov-property-of-the-gaussian-free-field)
      - [Continuum Gaussian free field](#continuum-gaussian-free-field)
        - [Conformal invariance of the two-dimensional Gaussian free field](#conformal-invariance-of-the-two-dimensional-gaussian-free-field)
        - [Zero-boundary Gaussian free field](#zero-boundary-gaussian-free-field)
          - [SLE4 coupling with a Gaussian free field](#sle4-coupling-with-a-gaussian-free-field)
            - [Gaussian characteristic-function martingale from covariance loss](#gaussian-characteristic-function-martingale-from-covariance-loss)
            - [Gaussian free field level line](#gaussian-free-field-level-line)
          - [Test-function pairing with a Gaussian free field](#test-function-pairing-with-a-gaussian-free-field)
          - [Green-kernel expansion in the Dirichlet space](#green-kernel-expansion-in-the-dirichlet-space)
            - [Finite-Green-energy measure pairing with a Gaussian free field](#finite-green-energy-measure-pairing-with-a-gaussian-free-field)
          - [Domain Markov property of the Gaussian free field](#domain-markov-property-of-the-gaussian-free-field)
            - [Local set of a Gaussian free field](#local-set-of-a-gaussian-free-field)
          - [Circle-average process of the Gaussian free field](#circle-average-process-of-the-gaussian-free-field)
            - [Circle-average process of the Gaussian free field is Brownian motion](#circle-average-process-of-the-gaussian-free-field-is-brownian-motion)
      - [Green energy](#green-energy)
      - [Pinned Gaussian free field](#pinned-gaussian-free-field)
  - [Gaussian zero-one law for measurable linear subspaces](#gaussian-zero-one-law-for-measurable-linear-subspaces)
  - [Gaussian measure](#gaussian-measure)
    - [Fernique's theorem](#fernique-s-theorem)
    - [First Gaussian chaos](#first-gaussian-chaos)
    - [Gaussian random variable in a Banach space](#gaussian-random-variable-in-a-banach-space)
      - [Strict increase of a Gaussian norm distribution](#strict-increase-of-a-gaussian-norm-distribution)
    - [Cameron-Martin theorem for a Gaussian measure](#cameron-martin-theorem-for-a-gaussian-measure)
      - [Symmetric Gaussian translation lower bound](#symmetric-gaussian-translation-lower-bound)
    - [Cameron-Martin space of a Gaussian measure](#cameron-martin-space-of-a-gaussian-measure)
      - [Cameron-Martin space of a Gaussian random variable in a Banach space](#cameron-martin-space-of-a-gaussian-random-variable-in-a-banach-space)
    - [Covariance operator of a Gaussian measure](#covariance-operator-of-a-gaussian-measure)
      - [Hilbert-space Gaussian series](#hilbert-space-gaussian-series)
    - [Bayesian inverse problem](#bayesian-inverse-problem)
      - [Bayes formula for a dominated observation model](#bayes-formula-for-a-dominated-observation-model)
      - [Well-posed Bayesian inverse problem in total variation](#well-posed-bayesian-inverse-problem-in-total-variation)
      - [Well-posed Bayesian inverse problem in Hellinger distance](#well-posed-bayesian-inverse-problem-in-hellinger-distance)
  - [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process)
    - [Stationary drift saturation](#stationary-drift-saturation)
      - [Same-noise stationary Ornstein-Uhlenbeck processes](#same-noise-stationary-ornstein-uhlenbeck-processes)
    - [Exponential Brownian time change to a stationary Ornstein-Uhlenbeck process](#exponential-brownian-time-change-to-a-stationary-ornstein-uhlenbeck-process)
    - [Ornstein-Uhlenbeck stochastic differential equation](#ornstein-uhlenbeck-stochastic-differential-equation)
    - [Ornstein-Uhlenbeck multiplicative amplification](#ornstein-uhlenbeck-multiplicative-amplification)
      - [Tilted Ornstein-Uhlenbeck oscillator transformation](#tilted-ornstein-uhlenbeck-oscillator-transformation)
    - [Integrated Ornstein-Uhlenbeck displacement](#integrated-ornstein-uhlenbeck-displacement)
    - [Explicit Ornstein-Uhlenbeck solution](#explicit-ornstein-uhlenbeck-solution)
      - [Zero-start Ornstein-Uhlenbeck covariance](#zero-start-ornstein-uhlenbeck-covariance)
    - [Multivariate Ornstein-Uhlenbeck process](#multivariate-ornstein-uhlenbeck-process)
      - [Ornstein-Uhlenbeck power spectrum](#ornstein-uhlenbeck-power-spectrum)
    - [Colored noise](#colored-noise)
- [Counting process](#counting-process)
  - [Counting-process intensity](#counting-process-intensity)
  - [Counting-process intensity in survival analysis](#counting-process-intensity-in-survival-analysis)
  - [Compensator of a counting process](#compensator-of-a-counting-process)
    - [Counting-process martingale](#counting-process-martingale)
- [Brownian motion](brownian-motion.md)
  - [Strict comparison of one-sided and absolute Brownian maxima](brownian-motion.md#strict-comparison-of-one-sided-and-absolute-brownian-maxima)
  - [Brownian sign transform](brownian-motion.md#brownian-sign-transform)
  - [Cylindrical Brownian motion](brownian-motion.md#cylindrical-brownian-motion)
  - [Brownian motion under a quadratic time change](brownian-motion.md#brownian-motion-under-a-quadratic-time-change)
  - [Rotational invariance of Brownian motion](brownian-motion.md#rotational-invariance-of-brownian-motion)
  - [Brownian moment recursion](brownian-motion.md#brownian-moment-recursion)
    - [Centered Brownian powers need not be martingales](brownian-motion.md#centered-brownian-powers-need-not-be-martingales)
  - [Planar Brownian motion avoids a fixed point](brownian-motion.md#planar-brownian-motion-avoids-a-fixed-point)
  - [Lévy area](brownian-motion.md#levy-area)
  - [Projection criterion for Brownian avoidance of affine subspaces](brownian-motion.md#projection-criterion-for-brownian-avoidance-of-affine-subspaces)
  - [Wiener sausage](brownian-motion.md#wiener-sausage)
    - [Survival among independently moving Poisson traps](brownian-motion.md#survival-among-independently-moving-poisson-traps)
  - [Blumenthal zero-one law](brownian-motion.md#blumenthal-zero-one-law)
  - [Brownian increment](brownian-motion.md#brownian-increment)
  - [Brownian fluctuations exceed the square-root scale](brownian-motion.md#brownian-fluctuations-exceed-the-square-root-scale)
  - [Integrated Brownian motion](brownian-motion.md#integrated-brownian-motion)
  - [Integrated square of Brownian motion](brownian-motion.md#integrated-square-of-brownian-motion)
    - [Laplace transform of the integrated square of Brownian motion](brownian-motion.md#laplace-transform-of-the-integrated-square-of-brownian-motion)
  - [Brownian time reversal on a finite interval](brownian-motion.md#brownian-time-reversal-on-a-finite-interval)
    - [Independent Brownian arms at a deterministic time](brownian-motion.md#independent-brownian-arms-at-a-deterministic-time)
  - [Longitudinal Brownian field with transverse covariance](brownian-motion.md#longitudinal-brownian-field-with-transverse-covariance)
  - [Local maximum of Brownian motion](brownian-motion.md#local-maximum-of-brownian-motion)
  - [Nowhere monotonicity of Brownian motion](brownian-motion.md#nowhere-monotonicity-of-brownian-motion)
  - [Brownian hitting of lattice spheres](brownian-motion.md#brownian-hitting-of-lattice-spheres)
  - [Brownian paths are not uniformly continuous on the half-line](brownian-motion.md#brownian-paths-are-not-uniformly-continuous-on-the-half-line)
  - [Brownian filtration](brownian-motion.md#brownian-filtration)
    - [Natural Brownian filtration](brownian-motion.md#natural-brownian-filtration)
  - [Martingale representation theorem](brownian-motion.md#martingale-representation-theorem)
    - [Brownian martingale representation theorem](brownian-motion.md#brownian-martingale-representation-theorem)
      - [Clark-Ocone formula for a smooth Brownian terminal payoff](brownian-motion.md#clark-ocone-formula-for-a-smooth-brownian-terminal-payoff)
  - [Exponential martingale for Brownian motion](brownian-motion.md#exponential-martingale-for-brownian-motion)
  - [Integral of Brownian motion](brownian-motion.md#integral-of-brownian-motion)
    - [Brownian motion transform by three times its running average](brownian-motion.md#brownian-motion-transform-by-three-times-its-running-average)
  - [Diffusion coefficient](brownian-motion.md#diffusion-coefficient)
    - [Solutal diffusivity](brownian-motion.md#solutal-diffusivity)
  - [Orthogonal invariance of Brownian motion](brownian-motion.md#orthogonal-invariance-of-brownian-motion)
  - [Meeting time of two independent Brownian motions](brownian-motion.md#meeting-time-of-two-independent-brownian-motions)
  - [Wiener measure](brownian-motion.md#wiener-measure)
    - [Wiener theorem](brownian-motion.md#wiener-theorem)
    - [Cameron-Martin space of Wiener measure](brownian-motion.md#cameron-martin-space-of-wiener-measure)
      - [Cameron-Martin theorem](brownian-motion.md#cameron-martin-theorem)
        - [Cameron-Martin shifts on infinite Wiener path space](brownian-motion.md#cameron-martin-shifts-on-infinite-wiener-path-space)
        - [Cameron-Martin theorem for a linear drift](brownian-motion.md#cameron-martin-theorem-for-a-linear-drift)
          - [First-passage density of Brownian motion with positive drift](brownian-motion.md#first-passage-density-of-brownian-motion-with-positive-drift)
  - [Brownian Hölder regularity](brownian-motion.md#brownian-holder-regularity)
  - [Brownian zero set](brownian-motion.md#brownian-zero-set)
  - [Reflection invariance of Brownian motion](brownian-motion.md#reflection-invariance-of-brownian-motion)
  - [Critical exponential moment of a drifted Brownian hitting time](brownian-motion.md#critical-exponential-moment-of-a-drifted-brownian-hitting-time)
  - [Bessel process](brownian-motion.md#bessel-process)
    - [Two-dimensional Bessel transition law](brownian-motion.md#two-dimensional-bessel-transition-law)
    - [Squared Bessel process](brownian-motion.md#squared-bessel-process)
      - [Additivity of independently driven squared Bessel processes](brownian-motion.md#additivity-of-independently-driven-squared-bessel-processes)
    - [Oppositely driven Bessel exit probability](brownian-motion.md#oppositely-driven-bessel-exit-probability)
    - [Truncation construction of a positive Bessel strong solution](brownian-motion.md#truncation-construction-of-a-positive-bessel-strong-solution)
    - [Three-dimensional Bessel process](brownian-motion.md#three-dimensional-bessel-process)
      - [Logarithmic escape rate of three-dimensional Brownian motion](brownian-motion.md#logarithmic-escape-rate-of-three-dimensional-brownian-motion)
    - [Beta integral for strict ordering of coupled Bessel lifetimes](brownian-motion.md#beta-integral-for-strict-ordering-of-coupled-bessel-lifetimes)
    - [Reciprocal three-dimensional Bessel strict local martingale](brownian-motion.md#reciprocal-three-dimensional-bessel-strict-local-martingale)
    - [Bessel power local martingale](brownian-motion.md#bessel-power-local-martingale)
      - [Stopped inverse radial power martingale classification](brownian-motion.md#stopped-inverse-radial-power-martingale-classification)
      - [All-time minimum of a transient Bessel process](brownian-motion.md#all-time-minimum-of-a-transient-bessel-process)
    - [Hitting-zero classification for a Bessel process](brownian-motion.md#hitting-zero-classification-for-a-bessel-process)
      - [Finite-time access to zero for Bessel dimensions below two](brownian-motion.md#finite-time-access-to-zero-for-bessel-dimensions-below-two)
    - [Scaling invariance of a Bessel process](brownian-motion.md#scaling-invariance-of-a-bessel-process)
    - [Exponential Brownian-to-Bessel time change](brownian-motion.md#exponential-brownian-to-bessel-time-change)
      - [Logarithmic growth of an exponential Brownian clock with positive drift](brownian-motion.md#logarithmic-growth-of-an-exponential-brownian-clock-with-positive-drift)
    - [Power time change of a Bessel process](brownian-motion.md#power-time-change-of-a-bessel-process)
  - [Reflected Brownian motion](brownian-motion.md#reflected-brownian-motion)
    - [Reflected Brownian motion with negative drift](brownian-motion.md#reflected-brownian-motion-with-negative-drift)
      - [Stationary law of negatively drifted reflected Brownian motion](brownian-motion.md#stationary-law-of-negatively-drifted-reflected-brownian-motion)
  - [Brownian occupation time](brownian-motion.md#brownian-occupation-time)
    - [Infinite occupation time of one-dimensional Brownian motion](brownian-motion.md#infinite-occupation-time-of-one-dimensional-brownian-motion)
      - [Divergence of a driftless Brownian exponential clock](brownian-motion.md#divergence-of-a-driftless-brownian-exponential-clock)
    - [Occupation-times formula](brownian-motion.md#occupation-times-formula)
  - [Planar Brownian motion](brownian-motion.md#planar-brownian-motion)
    - [Area of a planar Brownian path](brownian-motion.md#area-of-a-planar-brownian-path)
    - [Logarithmic radius of planar Brownian motion](brownian-motion.md#logarithmic-radius-of-planar-brownian-motion)
      - [Winding at logarithmic radial passage levels](brownian-motion.md#winding-at-logarithmic-radial-passage-levels)
    - [Planar Brownian stochastic area](brownian-motion.md#planar-brownian-stochastic-area)
      - [Orthogonality of the radial martingale and planar Brownian area](brownian-motion.md#orthogonality-of-the-radial-martingale-and-planar-brownian-area)
        - [Common-clock Brownian representation of radius and area](brownian-motion.md#common-clock-brownian-representation-of-radius-and-area)
    - [Brownian excursion in the upper half-plane](brownian-motion.md#brownian-excursion-in-the-upper-half-plane)
      - [Restriction probability of a Brownian half-plane excursion](brownian-motion.md#restriction-probability-of-a-brownian-half-plane-excursion)
        - [Boundary derivative is an excursion avoidance probability](brownian-motion.md#boundary-derivative-is-an-excursion-avoidance-probability)
    - [Conformal invariance of planar Brownian motion](brownian-motion.md#conformal-invariance-of-planar-brownian-motion)
      - [Small-radius Brownian winding law](brownian-motion.md#small-radius-brownian-winding-law)
      - [Cauchy exit law from a Brownian half-plane](brownian-motion.md#cauchy-exit-law-from-a-brownian-half-plane)
      - [Complex exponential construction of planar Brownian motion](brownian-motion.md#complex-exponential-construction-of-planar-brownian-motion)
      - [Power-map reduction for Brownian exit from a wedge](brownian-motion.md#power-map-reduction-for-brownian-exit-from-a-wedge)
        - [Brownian wedge-exit probability](brownian-motion.md#brownian-wedge-exit-probability)
      - [Conformal Brownian clock](brownian-motion.md#conformal-brownian-clock)
        - [Finite exit from a conformal image of a bounded planar domain](brownian-motion.md#finite-exit-from-a-conformal-image-of-a-bounded-planar-domain)
    - [Rotational invariance of planar Brownian motion](brownian-motion.md#rotational-invariance-of-planar-brownian-motion)
    - [Recurrence of planar Brownian motion](brownian-motion.md#recurrence-of-planar-brownian-motion)
      - [Polar point for planar Brownian motion](brownian-motion.md#polar-point-for-planar-brownian-motion)
      - [Divergence of a positive planar Brownian occupation integral](brownian-motion.md#divergence-of-a-positive-planar-brownian-occupation-integral)
    - [Brownian reflection coupling](brownian-motion.md#brownian-reflection-coupling)
    - [Harmonic measure](brownian-motion.md#harmonic-measure)
      - [Brownian exit law from a quadrant](brownian-motion.md#brownian-exit-law-from-a-quadrant)
      - [Harmonic capacity from infinity in the upper half-plane](brownian-motion.md#harmonic-capacity-from-infinity-in-the-upper-half-plane)
        - [Reflection lower bound for harmonic hull capacity](brownian-motion.md#reflection-lower-bound-for-harmonic-hull-capacity)
        - [Radius gives no positive lower bound for disconnected harmonic hull capacity](brownian-motion.md#radius-gives-no-positive-lower-bound-for-disconnected-harmonic-hull-capacity)
        - [Subadditivity of harmonic hull capacity](brownian-motion.md#subadditivity-of-harmonic-hull-capacity)
      - [Harmonic-measure asymptotic at infinity](brownian-motion.md#harmonic-measure-asymptotic-at-infinity)
      - [Möbius calculation of circular Brownian exit](brownian-motion.md#mobius-calculation-of-circular-brownian-exit)
      - [Reflection identity for Brownian exit from a half-disc](brownian-motion.md#reflection-identity-for-brownian-exit-from-a-half-disc)
      - [Bottom-boundary harmonic measure of a strip](brownian-motion.md#bottom-boundary-harmonic-measure-of-a-strip)
      - [Upper-half-plane harmonic measure of the positive half-axis](brownian-motion.md#upper-half-plane-harmonic-measure-of-the-positive-half-axis)
      - [Planar Brownian annulus hitting probability](brownian-motion.md#planar-brownian-annulus-hitting-probability)
      - [Brownian entrance law to a disc from infinity](brownian-motion.md#brownian-entrance-law-to-a-disc-from-infinity)
  - [Coordinatewise coalescing coupling of Brownian motions](brownian-motion.md#coordinatewise-coalescing-coupling-of-brownian-motions)
  - [Strong law for Brownian motion](brownian-motion.md#strong-law-for-brownian-motion)
  - [Brownian loop measure](brownian-motion.md#brownian-loop-measure)
    - [Pinned Brownian loop measure at an interior point](brownian-motion.md#pinned-brownian-loop-measure-at-an-interior-point)
    - [Conformal restriction measure on simple loops](brownian-motion.md#conformal-restriction-measure-on-simple-loops)
      - [Recovery of a loop measure from conformal deficits](brownian-motion.md#recovery-of-a-loop-measure-from-conformal-deficits)
  - [Nowhere differentiability of Brownian motion](brownian-motion.md#nowhere-differentiability-of-brownian-motion)
  - [Lévy characterization of Brownian motion](brownian-motion.md#levy-characterization-of-brownian-motion)
    - [Lévy characterization of multidimensional Brownian motion](brownian-motion.md#levy-characterization-of-multidimensional-brownian-motion)
  - [Brownian scaling](brownian-motion.md#brownian-scaling)
  - [Recurrence of one-dimensional Brownian motion](brownian-motion.md#recurrence-of-one-dimensional-brownian-motion)
  - [Transience of Brownian motion in dimension at least three](brownian-motion.md#transience-of-brownian-motion-in-dimension-at-least-three)
    - [Brownian sphere-hitting probability in dimension three](brownian-motion.md#brownian-sphere-hitting-probability-in-dimension-three)
      - [Last visit to a bounded ball for three-dimensional Brownian motion](brownian-motion.md#last-visit-to-a-bounded-ball-for-three-dimensional-brownian-motion)
  - [Brownian exit time](brownian-motion.md#brownian-exit-time)
    - [Brownian hitting probability of a ball](brownian-motion.md#brownian-hitting-probability-of-a-ball)
      - [Small-ball Brownian hitting asymptotic](brownian-motion.md#small-ball-brownian-hitting-asymptotic)
    - [Brownian exit-time expectation in an orthant](brownian-motion.md#brownian-exit-time-expectation-in-an-orthant)
    - [Uniform ball sampling by Brownian stopping](brownian-motion.md#uniform-ball-sampling-by-brownian-stopping)
      - [Brownian exit-time ball averaging identity](brownian-motion.md#brownian-exit-time-ball-averaging-identity)
        - [Finiteness propagation of Brownian mean exit times](brownian-motion.md#finiteness-propagation-of-brownian-mean-exit-times)
    - [Brownian exit from an interval](brownian-motion.md#brownian-exit-from-an-interval)
      - [Asymmetric Brownian interval-exit transform](brownian-motion.md#asymmetric-brownian-interval-exit-transform)
      - [Brownian exit-time skeleton](brownian-motion.md#brownian-exit-time-skeleton)
        - [Gaussian limit of a Brownian exit skeleton](brownian-motion.md#gaussian-limit-of-a-brownian-exit-skeleton)
        - [Brownian exit-skeleton clock convergence](brownian-motion.md#brownian-exit-skeleton-clock-convergence)
      - [Laplace transform of symmetric Brownian interval-exit time](brownian-motion.md#laplace-transform-of-symmetric-brownian-interval-exit-time)
      - [Brownian symmetric interval-exit moments](brownian-motion.md#brownian-symmetric-interval-exit-moments)
      - [Conditional Brownian interval-exit time](brownian-motion.md#conditional-brownian-interval-exit-time)
    - [Dynkin formula for Brownian motion](brownian-motion.md#dynkin-formula-for-brownian-motion)
  - [Brownian bridge](brownian-motion.md#brownian-bridge)
    - [Time reversal of a Brownian bridge](brownian-motion.md#time-reversal-of-a-brownian-bridge)
    - [Stochastic integral representation of a Brownian bridge](brownian-motion.md#stochastic-integral-representation-of-a-brownian-bridge)
    - [F-Brownian bridge](brownian-motion.md#f-brownian-bridge)
    - [Brownian bridge independence from its endpoint](brownian-motion.md#brownian-bridge-independence-from-its-endpoint)
    - [Brownian-bridge crossing probability](brownian-motion.md#brownian-bridge-crossing-probability)
  - [Exponential Brownian martingale](brownian-motion.md#exponential-brownian-martingale)
    - [Parameter derivative of the exponential Brownian martingale](brownian-motion.md#parameter-derivative-of-the-exponential-brownian-martingale)
  - [Gaussian-process characterization of Brownian motion](brownian-motion.md#gaussian-process-characterization-of-brownian-motion)
  - [Time inversion of Brownian motion](brownian-motion.md#time-inversion-of-brownian-motion)
  - [Brownian motion with drift](brownian-motion.md#brownian-motion-with-drift)
    - [Drifted Brownian interval-exit probability](brownian-motion.md#drifted-brownian-interval-exit-probability)
    - [Infinite-horizon singularity of Brownian motion with constant drift](brownian-motion.md#infinite-horizon-singularity-of-brownian-motion-with-constant-drift)
    - [Finite-horizon maximum of Brownian motion with negative drift](brownian-motion.md#finite-horizon-maximum-of-brownian-motion-with-negative-drift)
    - [Infinite-horizon crossing probability for Brownian motion with negative drift](brownian-motion.md#infinite-horizon-crossing-probability-for-brownian-motion-with-negative-drift)
    - [Last passage time above a level for Brownian motion with negative drift](brownian-motion.md#last-passage-time-above-a-level-for-brownian-motion-with-negative-drift)
  - [Reflection principle (Wiener process)](brownian-motion.md#reflection-principle-wiener-process)
    - [Brownian terminal-to-maximum ratio](brownian-motion.md#brownian-terminal-to-maximum-ratio)
    - [Brownian reflection at a stopping time](brownian-motion.md#brownian-reflection-at-a-stopping-time)
    - [Brownian running maximum](brownian-motion.md#brownian-running-maximum)
      - [Gaussian maximal bound for Brownian motion](brownian-motion.md#gaussian-maximal-bound-for-brownian-motion)
      - [Atomless maxima on separated Brownian intervals](brownian-motion.md#atomless-maxima-on-separated-brownian-intervals)
      - [Finite-horizon maximum of Brownian motion with drift](brownian-motion.md#finite-horizon-maximum-of-brownian-motion-with-drift)
        - [Joint endpoint and maximum law for drifted Brownian motion](brownian-motion.md#joint-endpoint-and-maximum-law-for-drifted-brownian-motion)
      - [Integral lower envelope for the Brownian maximum](brownian-motion.md#integral-lower-envelope-for-the-brownian-maximum)
      - [Brownian barrier survival asymptotic](brownian-motion.md#brownian-barrier-survival-asymptotic)
      - [Maximum before a lower Brownian barrier](brownian-motion.md#maximum-before-a-lower-brownian-barrier)
      - [Joint distribution of Brownian motion and its running maximum](brownian-motion.md#joint-distribution-of-brownian-motion-and-its-running-maximum)
      - [Lévy identity for Brownian motion](brownian-motion.md#levy-identity-for-brownian-motion)
      - [Time of the Brownian maximum](brownian-motion.md#time-of-the-brownian-maximum)
        - [Brownian motion shifted at its finite-horizon maximum](brownian-motion.md#brownian-motion-shifted-at-its-finite-horizon-maximum)
  - [Brownian transition semigroup](brownian-motion.md#brownian-transition-semigroup)
    - [Brownian transition density](brownian-motion.md#brownian-transition-density)
      - [Killed Brownian transition density](brownian-motion.md#killed-brownian-transition-density)
    - [Brownian compensator martingale](brownian-motion.md#brownian-compensator-martingale)
  - [Exponential test-function characterization of Brownian motion](brownian-motion.md#exponential-test-function-characterization-of-brownian-motion)
    - [Conditional characteristic-function criterion for Brownian increments](brownian-motion.md#conditional-characteristic-function-criterion-for-brownian-increments)

## Skorokhod problem

↑ **Parent:** [Stochastic process](stochastic-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Skorokhod_problem)

Find a constrained path and a boundary regulator which together modify a given driving path. In the half-line case, write $x=g+k\ge0$, require $k(0)=0$ and $k$ nondecreasing, and require its increases to occur only where $x=0$. For multidimensional orthants the regulator acts through a specified reflection matrix. The [Skorokhod reflection map on the half-line](#skorokhod-reflection-map-on-the-half-line) solves the one-dimensional continuous-path case explicitly.

### Skorokhod reflection map on the half-line

↑ **Parent:** [Skorokhod problem](#skorokhod-problem)

For a [continuous](calculus.md#continuous-function) driving path with $g(0)\ge0$, the running supremum supplies the minimal nondecreasing regulator keeping the path nonnegative. It increases only at a new negative running minimum, where the reflected path is zero. Any regulator satisfying the [Skorokhod problem](#skorokhod-problem) constraints must coincide with it. On a finite time interval, $\|\Gamma(g)-\Gamma(h)\|_\infty\le2\|g-h\|_\infty$, so the map is continuous and transfers a [functional central limit theorem](convergence-of-random-variables.md#donsker-s-theorem) to reflected workloads.

## Self-similarity of a stochastic process

↑ **Parent:** [Stochastic process](stochastic-process.md)

A process $Z$ is self-similar with exponent $H$ if $Z(a\,\cdot)$ and $a^HZ$ have the same finite-dimensional distributions for every $a>0$, or the same path law when the process is considered as a random path. [Fractional Brownian motion](#fractional-brownian-motion) has this property with its [Hurst exponent](#hurst-exponent). It converts dilation of time to deterministic scaling of amplitude: $Z(N\,\cdot)/N\overset d=N^{H-1}Z$. Consequently a small-noise [large deviation principle](convergence-of-random-variables.md#large-deviation-principle) with inverse-variance speed produces the [large-deviation speed](convergence-of-random-variables.md#large-deviation-speed) $N^{2(1-H)}$ for those rescaled paths.

## Random field

↑ **Parent:** [Stochastic process](stochastic-process.md)

A random field is a family of [random variables](random-variable.md) indexed by points of a spatial domain, or more generally by a multi-dimensional parameter set. Its componentwise [covariance function](#covariance-function) and [spectral tensor](probability-and-statistics.md#spectral-tensor) describe second-order dependence. A [Gaussian random field](#gaussian-random-field) has jointly Gaussian finite-dimensional distributions; a general random field need not be Gaussian.

## Locally bounded process

↑ **Parent:** [Stochastic process](stochastic-process.md)

A process is locally bounded if there are stopping times $\tau_n\uparrow\infty$ and finite deterministic constants $K_n$ bounding it on the stopped intervals. A locally bounded predictable process is integrable against a semimartingale. Continuous adapted processes are locally bounded by stopping their magnitudes and time.

// Target: probability-and-statistics.bigb

## Branching process

↑ **Parent:** [Stochastic process](stochastic-process.md)

A [stochastic process](stochastic-process.md) in which individuals independently produce offspring according to specified distributions. It models growing populations and gives an approximation to sparse [percolation clusters](bond-percolation.md#percolation-cluster) when collisions between branches can be neglected. On a lattice, loops and overlapping branches prevent this approximation from being an exact identity.

### Multitype Poisson branching process

↑ **Parent:** [Branching process](#branching-process)

A particle of type $i$ has independently a [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) of type-$j$ offspring with [mean](probability-theory.md#expected-value) $\lambda_{ij}$. Different particles reproduce independently. If $p^{(t)}_i$ is the [probability](probability-theory.md#probability) generation $t$ is nonempty from one type-$i$ ancestor, then $p^{(0)}=\mathbf1$ and $p^{(t+1)}=T(p^{(t)})$, where $T_i(x)=1-\exp[-(\Lambda x)_i]$. This iteration decreases to the [survival probability of a branching process](probability-and-statistics.md#survival-probability-of-a-branching-process), the greatest nonnegative [fixed point](function.md#fixed-point) of $T$. The expected type-count row [vector](vector-space.md#vector) in generation $t$ is $e_i^T\Lambda^t$.

#### Spectral survival criterion for multitype Poisson branching

↑ **Parent:** [Multitype Poisson branching process](#multitype-poisson-branching-process)

This criterion holds even for reducible [nonnegative matrices](vector-space.md#nonnegative-matrix). If a [fixed point](function.md#fixed-point) $p\ne0$ exists, $1-e^{-z}<z$ for $z>0$ gives $(\Lambda p)_i>p_i$ on its support. Some $\alpha>1$ therefore satisfies $\Lambda p\ge\alpha p$, forcing the [spectral radius](analysis.md#spectral-radius) above one by the [Perron–Frobenius theorem](vector-space.md#perron-frobenius-theorem). Conversely take $v\ge0$, $v\ne0$, with $\Lambda v=\rho v$ and $\rho>1$. For sufficiently small $\eta>0$, $1-e^{-\eta\rho v_i}\ge\eta v_i$. Thus $\eta v$ is a subsolution; monotone iteration under $T$ gives a positive [fixed point](function.md#fixed-point) below $\mathbf1$. Strictness of $1-e^{-z}<z$ excludes survival at the critical value for this Poisson offspring law.

## Unnormalized time autocorrelation

↑ **Parent:** [Stochastic process](stochastic-process.md)

The raw same-observable time correlation $C(t,\tau)=\langle X(t)X(t+\tau)\rangle$. For a stationary process, it equals $\langle X\rangle^2+\operatorname{Cov}(X(t),X(t+\tau))$. Its connected part is the [autocovariance](time-series.md#autocovariance); unlike the normalized statistical [autocorrelation](time-series.md#autocorrelation), no division by the [variance](variance.md) is imposed. The distinction matters for fluctuations around a nonzero [equilibrium point](dynamical-systems.md#equilibrium-point-of-a-dynamical-system).

### Intrawell phase autocorrelation

↑ **Parent:** [Unnormalized time autocorrelation](#unnormalized-time-autocorrelation)

Near the stable [Adler phase equation](dynamical-systems.md#adler-phase-equation) point $\alpha=\arcsin(\omega/\epsilon)$, linearized noise obeys an [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process) with relaxation rate $\kappa=\sqrt{\epsilon^2-\omega^2}$. Its harmonic-model raw correlation is $\alpha^2+(T_{\rm eff}/\kappa)e^{-\kappa|\tau|}$. Nonlinear drift also shifts the local mean at order $T_{
m eff}$. This describes times after relaxation but before appreciable [phase slips](dynamical-systems.md#phase-slip); it is not a stationary infinite-time correlation of the unwrapped phase at fixed nonzero noise.

## Sample path

↑ **Parent:** [Stochastic process](stochastic-process.md)

For a [stochastic process](stochastic-process.md) $X_t$ and a fixed sample outcome $\omega$, its [sample path](#sample-path) is the function $t\mapsto X_t(\omega)$. Statements about continuous, [càdlàg](calculus.md#cadlag) or [Hölder continuous function](sobolev-space.md#holder-condition) [sample paths](#sample-path) concern these functions simultaneously in time; they differ from assertions made only at each fixed deterministic time. A probability-one path property can be checked using countable dense times when the appropriate continuity is available.

## Bounded increments

↑ **Parent:** [Stochastic process](stochastic-process.md)

A discrete-time [stochastic process](stochastic-process.md) has [bounded increments](#bounded-increments) if a single deterministic $C<\infty$ satisfies $|X_{n+1}-X_n|\leq C$ almost surely for every $n$. The constant is uniform in time and sample outcome; bounding each increment by a different constant does not suffice. This property applies to differences, so it does not require the process itself to stay bounded.

### Bounded-increment martingale convergence-or-oscillation dichotomy

↑ **Parent:** [Bounded increments](#bounded-increments)

A discrete-time [martingale](martingale.md) with a common deterministic bound on all increments either converges finitely or has $\liminf X_n=-\infty$ and $\limsup X_n=+\infty$, [almost surely](convergence-of-random-variables.md#almost-sure-convergence). Stopping on first crossing below $-A$ gives a lower bound $-A-M$ on the overshoot. Adding $A+M+X_0^-$ produces a nonnegative [martingale](martingale.md), so the [martingale convergence theorem](martingale.md#martingale-convergence-theorem) forces finite convergence on the event of never crossing. Apply the same argument to $-X$.

#### Oscillation of a bounded centered iid random walk

↑ **Parent:** [Bounded-increment martingale convergence-or-oscillation dichotomy](#bounded-increment-martingale-convergence-or-oscillation-dichotomy)

Let $S_n=\sum_{j=1}^nX_j$, where the increments are nonconstant [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables) with zero [expected value](probability-theory.md#expected-value) and $|X_j|\leq c$. Then the [random walk](markov-process.md#random-walk) oscillates between arbitrarily large positive and negative levels [almost surely](convergence-of-random-variables.md#almost-sure-convergence). For $T_a=\inf\{n:S_n\geq a\}$, the [stopped martingale](martingale.md#stopped-martingale) $a+c-S_{n\wedge T_a}$ is nonnegative. The [martingale convergence theorem](martingale.md#martingale-convergence-theorem) implies that $S_n$ converges finitely on $\{T_a=\infty\}$. However, some $\delta>0$ has $\mathbb P(|X_1|>\delta)>0$, and the [Borel-Cantelli lemmas](probability-theory.md#borel-cantelli-lemmas) imply $|X_n|>\delta$ infinitely often. Hence finite convergence is impossible. Apply this to every positive integer $a$ and to $-S_n$.

The [bounded increments](#bounded-increments) also imply infinitely many visits to $[-c/2,c/2]$: a path cannot cross from above $c/2$ to below $-c/2$ without entering this interval. Identical distribution cannot simply be dropped. For independent symmetric signs $\varepsilon_j$, the increments $X_j=c4^{-(j-1)}\varepsilon_j$ satisfy $|S_n|\geq2c/3$ for every $n$, even though they are nonzero, independent, symmetric and uniformly bounded.

## Locally defined stochastic process

↑ **Parent:** [Stochastic process](stochastic-process.md)

A continuous locally defined process is a pair $(X,T)$ specified on the [stochastic interval](#stochastic-interval) $[0,T)$, with a lifetime [stopping time](martingale.md#stopping-time) $T$ approached by an [announcing sequence for a stopping time](martingale.md#announcing-sequence-for-a-stopping-time) $T_n$. Each stopped process is an ordinary continuous [adapted process](#adapted-process). This is the convention used for continuous local differential equations; no value at $T$ is required. Restricting a globally defined process gives examples, but finite lifetimes also allow approach to a domain boundary or explosion.

### Local solution of a stochastic differential equation

↑ **Parent:** [Locally defined stochastic process](#locally-defined-stochastic-process)

A local solution is a [locally defined stochastic process](#locally-defined-stochastic-process) taking values in a specified open domain $U$ and satisfying the [stochastic differential equation](stochastic-calculus.md#stochastic-differential-equation) on every stopped interval before its lifetime. For $dX=b(X)dt+\sigma(X)dB$, the integral equation holds after each announcing stop, with the requisite local drift and noise integrability. A [maximal local solution of a stochastic differential equation](stochastic-calculus.md#maximal-local-solution-of-a-stochastic-differential-equation) cannot be extended while remaining in $U$; a finite lifetime can be a boundary hit rather than divergence to infinity.

## Stochastic interval

↑ **Parent:** [Stochastic process](stochastic-process.md)

For a [stopping time](martingale.md#stopping-time) $T$, the stochastic interval $[0,T)$ means the subset $\{(\omega,t):0\leq t<T(\omega)\}$ of sample-time space. Its endpoint varies with the sample. A [locally defined stochastic process](#locally-defined-stochastic-process) on it has no prescribed value at the endpoint. This notation is distinct from an ordinary deterministic interval.

## Modification of a stochastic process

↑ **Parent:** [Stochastic process](stochastic-process.md)

Processes $X,Y$ on the same probability space and index set are modifications of each other if $\mathbb P(X_t=Y_t)=1$ for each fixed index $t$. This differs from [indistinguishability of stochastic processes](#indistinguishability-of-stochastic-processes), which requires equality at all indices on a single [event](probability-theory.md#event) of probability one. Equality at a countable dense set upgrades to indistinguishability when both processes have continuous paths.

<h3 id="cadlag-modification">Càdlàg modification</h3>

↑ **Parent:** [Modification of a stochastic process](#modification-of-a-stochastic-process)

A [càdlàg modification](#cadlag-modification) of a [stochastic process](stochastic-process.md) is a [modification of a stochastic process](#modification-of-a-stochastic-process) whose paths are [càdlàg](calculus.md#cadlag) on one event of probability one. Equality [almost surely](convergence-of-random-variables.md#almost-sure-convergence) at every separately fixed time does not imply [indistinguishability of stochastic processes](#indistinguishability-of-stochastic-processes) when the original process lacks path regularity. A [stochastic process](stochastic-process.md) starting at zero, with [independent increments](#independent-increments), [stationary increments](#stationary-increments), and [stochastic continuity](#stochastic-continuity), has a [càdlàg modification](#cadlag-modification) and is a [Lévy process](#levy-process) under the intrinsic definition.

### Continuous modification

↑ **Parent:** [Modification of a stochastic process](#modification-of-a-stochastic-process)

A continuous modification of a [stochastic process](stochastic-process.md) is a [modification of a stochastic process](#modification-of-a-stochastic-process) whose paths are continuous outside a single null [event](probability-theory.md#event). For a process originally given only on a countable dense set, the analogous construction gives a continuous extension agreeing simultaneously at all original indices. The [Kolmogorov continuity theorem](#kolmogorov-continuity-theorem) and [dyadic increment chaining](#dyadic-increment-chaining) are standard ways to obtain it.

## Linear fluctuating interface

↑ **Parent:** [Stochastic process](stochastic-process.md)

A linear fluctuating interface smooths height gradients by diffusion and receives additive [Gaussian white noise](#gaussian-white-noise). With periodic or [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition), its nonzero [Fourier modes](fourier-analysis.md#fourier-mode) are independent [Ornstein-Uhlenbeck processes](#ornstein-uhlenbeck-process) if the noise is diagonal in that basis. The unconstrained uniform height is a [Brownian zero mode of a fluctuating interface](#brownian-zero-mode-of-a-fluctuating-interface).

### Stationary spectrum of a linear fluctuating interface

↑ **Parent:** [Linear fluctuating interface](#linear-fluctuating-interface)

For a nonzero [Fourier mode](fourier-analysis.md#fourier-mode) satisfying $dh_q=-\alpha q^2h_q\,dt+\sigma\,dW_q$ with $\alpha>0$, the [explicit Ornstein-Uhlenbeck solution](#explicit-ornstein-uhlenbeck-solution) and [Itô isometry](stochastic-calculus.md#ito-isometry) give the stationary [second moment](probability-theory.md#second-moment) $\sigma^2/(2\alpha q^2)$. The prefactor depends on the normalization of the mode noise, while the inverse-square dependence follows from diffusive relaxation.

### Brownian zero mode of a fluctuating interface

↑ **Parent:** [Linear fluctuating interface](#linear-fluctuating-interface)

An unpinned uniform height driven by [Gaussian white noise](#gaussian-white-noise) is [Brownian motion](brownian-motion.md). Its [variance](variance.md) grows as $\sigma^2t$ and it has no [stationary distribution](markov-process.md#stationary-distribution) on the real height axis for $\sigma>0$. Indeed, a stationary [characteristic function](probability-theory.md#characteristic-function) would obey $\widehat\mu(k)=\widehat\mu(k)e^{-\sigma^2k^2t/2}$, incompatible with continuity at zero. Quotienting out the uniform height can still leave stationary shape fluctuations.

## Path probability

↑ **Parent:** [Stochastic process](stochastic-process.md)

A path probability is a [probability measure](probability-theory.md#probability-measure), or a density relative to a specified reference measure, on histories of a [stochastic process](stochastic-process.md). A formal [Onsager--Machlup path probability](critical-phenomenon.md#onsager-machlup-path-probability) must be interpreted with its discretization and initial-state conditioning specified; conditioning on both endpoints produces a separately normalized bridge measure.

## Langevin dynamics

↑ **Parent:** [Stochastic process](stochastic-process.md)

[Langevin dynamics](#langevin-dynamics) describes a dynamical variable driven by deterministic forces and random noise. [Underdamped Langevin dynamics](stochastic-calculus.md#underdamped-langevin-dynamics) retains inertia, whereas [overdamped Langevin dynamics](stochastic-calculus.md#overdamped-langevin-dynamics) neglects it. At [thermal equilibrium](thermodynamics.md#thermal-equilibrium), the [fluctuation-dissipation relation for a Langevin particle](thermodynamics.md#fluctuation-dissipation-relation-for-a-langevin-particle) relates [Gaussian white noise](#gaussian-white-noise) strength to drag and [temperature](thermodynamics.md#temperature).

## Interacting particle system

↑ **Parent:** [Stochastic process](stochastic-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Interacting_particle_system)

An interacting particle system is a [stochastic process](stochastic-process.md) whose local states evolve through random transitions whose rates depend on nearby states.

### Voter model

↑ **Parent:** [Interacting particle system](#interacting-particle-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Voter_model)

At each site, a rate-one clock rings and the site copies the state of a randomly chosen neighbor. The model is a [Markov process](markov-process.md) on [Ising spin](statistical-physics.md#ising-spin-variable) configurations, interpreted through its local update [infinitesimal generator](#infinitesimal-generator-stochastic-processes). All constant configurations are [absorbing state](markov-process.md#absorbing-state). Tracing copying arrows backwards gives the [voter-model duality](#voter-model-duality) with [coalescing random walks](markov-process.md#coalescing-random-walks).

#### Voter-model duality

↑ **Parent:** [Voter model](#voter-model)

Independent [Poisson process](probability-theory.md#poisson-process) copying arrows construct the [voter model](#voter-model). A backward ancestral line from a site follows a [continuous-time random walk](markov-process.md#continuous-time-random-walk); lines that meet then coincide. Thus a finite collection of [Ising spins](statistical-physics.md#ising-spin-variable) at time $t$ equals initial [Ising spins](statistical-physics.md#ising-spin-variable) at the positions of [coalescing random walks](markov-process.md#coalescing-random-walks). In particular $E_\eta\xi_t(x)=\sum_zp_t(x,z)\eta(z)$, and the [probability](probability-theory.md#probability) of disagreement at two sites is bounded by the [probability](probability-theory.md#probability) their ancestral walks have not yet coalesced.

##### Finite-seed local extinction in the voter model

↑ **Parent:** [Voter-model duality](#voter-model-duality)

If the initial one-spin set $F$ is finite on the [square lattice](graph.md#square-lattice), [voter-model duality](#voter-model-duality) gives $P(\xi_t(x)=1)=\sum_{z\in F}p_t(x,z)\to0$. The [transition probabilities](markov-process.md#transition-probability) tend to zero on this infinite [lattice](mathematical-logic.md#lattice); their [Fourier transform](analysis.md#fourier-transform) also proves the [limit of a sequence](real-analysis.md#limit-of-a-sequence) by [dominated convergence](measure-theory.md#dominated-convergence-theorem). A [union bound](probability-inequality.md#boole-s-inequality) on any finite set of observation sites then proves [weak convergence of probability measures](convergence-of-random-variables.md#weak-convergence-of-probability-measures) to the all-zero point mass in the [product topology](geometry-and-topology.md#product-topology).

##### Invariant measures of the two-dimensional voter model

↑ **Parent:** [Voter-model duality](#voter-model-duality)

In a nearest-neighbor [voter model](#voter-model) on the [square lattice](graph.md#square-lattice), any two ancestral [coalescing random walks](markov-process.md#coalescing-random-walks) meet almost surely. For an [invariant probability measure of a Markov process](markov-process.md#invariant-probability-law-of-a-markov-process), the disagreement [probability](probability-theory.md#probability) is constant in time but bounded by the vanishing [probability](probability-theory.md#probability) of noncoalescence. Hence every pair of sites agrees almost surely. Countability concentrates the measure on the two constant configurations; both are [absorbing state](markov-process.md#absorbing-state), so every mixture of their [Dirac measures](measure-theory.md#dirac-measure) is invariant. [Translation invariance](physics.md#translation-invariance) need not be assumed.

### Exclusion process

↑ **Parent:** [Interacting particle system](#interacting-particle-system)

Particles on a countable lattice attempt jumps at the rates $p(x,y)$, and an attempt into an occupied site is suppressed. Thus each site contains at most one particle and the number of particles is conserved when finite. Here $\eta^{xy}$ interchanges the occupations at $x$ and $y$. Bounded nearest-neighbour rates give a well-defined [Markov process](markov-process.md). A symmetric jump kernel gives the [symmetric simple exclusion process](#symmetric-simple-exclusion-process); an unequal left-right kernel gives the [asymmetric simple exclusion process](mathematical-biology.md#asymmetric-simple-exclusion-process).

#### Symmetric simple exclusion process

↑ **Parent:** [Exclusion process](#exclusion-process)

On $\mathbb Z$, put independent rate-$c$ [Poisson processes](probability-theory.md#poisson-process) on unoriented nearest-neighbour [edges](graph-theory.md#edge-of-a-graph), and exchange their endpoint occupations at each mark. Its generator on cylinder functions is $Lf(\eta)=c\sum_x[f(\eta^{x,x+1})-f(\eta)]$. Equal occupations do not change the state, and a particle next to a vacancy jumps across at rate $c$. The [stirring representation of symmetric exclusion](#stirring-representation-of-symmetric-exclusion) constructs it for arbitrary initial configurations. The simple occupation-product [product self-duality of symmetric exclusion](#product-self-duality-of-symmetric-exclusion) requires symmetry and is not the ordinary duality of an asymmetric process.

##### Bernoulli invariant laws of finite symmetric exclusion

↑ **Parent:** [Symmetric simple exclusion process](#symmetric-simple-exclusion-process)

On a finite [graph](graph.md) with symmetric [edge](graph-theory.md#edge-of-a-graph)-swap rates, the [stirring representation of symmetric exclusion](#stirring-representation-of-symmetric-exclusion) transports the occupations by a random [permutation](combinatorics.md#permutation). An independent identically distributed [Bernoulli distribution](discrete-probability-distribution.md#bernoulli-distribution) occupation field is invariant under every deterministic [permutation](combinatorics.md#permutation), and hence under this random [permutation](combinatorics.md#permutation) when it is independent of the initial field. Therefore the displayed [product measure](probability-theory.md#product-measure) is invariant, including densities zero and one. Equivalently, an [edge](graph-theory.md#edge-of-a-graph) swap preserves the number of particles and has the same reverse rate, giving [detailed balance](markov-process.md#detailed-balance).

##### Stirring representation of symmetric exclusion

↑ **Parent:** [Symmetric simple exclusion process](#symmetric-simple-exclusion-process)

Give every site a distinct label and interchange labels at the edge marks defining the [symmetric simple exclusion process](#symmetric-simple-exclusion-process). Each forward or backward label path makes only finitely many jumps in a bounded time interval, since its total rate is $2c$. Occupations are transported along these paths. The backward ancestors of a finite set have the law of the finite-particle [symmetric exclusion process](#symmetric-simple-exclusion-process), by time reversal of the Poisson marks. This proves the [product self-duality of symmetric exclusion](#product-self-duality-of-symmetric-exclusion).

###### Product self-duality of symmetric exclusion

↑ **Parent:** [Stirring representation of symmetric exclusion](#stirring-representation-of-symmetric-exclusion)

For finite $A\subset\mathbb Z$ put $D(\eta,A)=\prod_{x\in A}\eta(x)$, with empty product one. Interchanging occupations gives $D(\eta^{xy},A)=D(\eta,A^{xy})$, where $A^{xy}$ interchanges membership of the two sites. The edge-swap generators therefore agree on $D$. The [stirring representation of symmetric exclusion](#stirring-representation-of-symmetric-exclusion) proves the displayed identity at all times by tracing the ancestors of $A$ backwards. A general asymmetric jump kernel does not satisfy this product self-duality.

###### Exchangeable invariant laws of symmetric exclusion

↑ **Parent:** [Product self-duality of symmetric exclusion](#product-self-duality-of-symmetric-exclusion)

If the probability of occupation at every site in a finite set depends only on its cardinality, the law is exchangeable. The [product self-duality of symmetric exclusion](#product-self-duality-of-symmetric-exclusion) and conservation of the finite dual particle count imply that all these occupation-product moments are unchanged by evolution. [Inclusion-exclusion principle](combinatorics.md#inclusion-exclusion-principle) reconstructs every finite cylinder probability from them, proving invariance. This direct argument does not require a representation theorem for exchangeable laws.

### Contact process

↑ **Parent:** [Interacting particle system](#interacting-particle-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Contact_process)

In the contact process, infected vertices recover at rate $\mu$, while each oriented nearest-neighbour edge transmits infection at rate $\lambda$. The empty configuration is absorbing.

#### Exponential cardinality supermartingale for the contact process on a tree

↑ **Parent:** [Contact process](#contact-process)

For the [contact process](#contact-process) with per-[edge](graph-theory.md#edge-of-a-graph) infection rate $\lambda$ and recovery rate one on a degree-$(d+1)$ [regular tree](combinatorics.md#regular-tree), the [infinitesimal generator](#infinitesimal-generator-stochastic-processes) gives $L\nu_\rho(A)=(1-\rho)\nu_\rho(A)(|A|/\rho-\lambda|\partial_E A|)$. The [edge boundary of a finite forest in a regular tree](combinatorics.md#edge-boundary-of-a-finite-forest-in-a-regular-tree) implies $L\nu_\rho\le0$ whenever $\rho\lambda(d-1)\ge1$, including the absorbing empty state where the generator is zero. Thus the displayed functional is a bounded [supermartingale](martingale.md#supermartingale), and the extinction [probability](probability-theory.md#probability) from $A$ is at most $\rho^{|A|}$.

#### Extremal invariant measures of the contact process

↑ **Parent:** [Contact process](#contact-process)

The [graphical representation of the contact process](#graphical-representation-of-the-contact-process) preserves coordinatewise order. Its law from the all-infected state decreases in [stochastic domination](probability-and-statistics.md#stochastic-domination-of-probability-measures) with time, and its limit is invariant by the [Feller semigroup](functional-analysis.md#feller-semigroup) property. The all-healthy state is absorbing. Any invariant probability law lies between these two laws. [Duality of the contact process](#duality-of-the-contact-process) gives $\overline\nu(\eta(x)=1)=\theta(\lambda)$ when the recovery rate is one. Consequently the two extremal laws coincide exactly when the [survival probability of the contact process](#survival-probability-of-the-contact-process) is zero.

#### Branching bound for contact-process survival

↑ **Parent:** [Contact process](#contact-process)

With recovery rate one, the number of infected sites in a nearest-neighbour [contact process](#contact-process) has death rate equal to its size and birth rate at most $2d\lambda$ times its size. It is dominated by a linear birth-death [branching process](#branching-process) with these per-particle rates. In particular, from one infection its expected size is at most $e^{(2d\lambda-1)t}$, so its survival probability is zero when $2d\lambda<1$. This proves the displayed lower bound on the critical rate.

#### Graphical representation of the contact process

↑ **Parent:** [Contact process](#contact-process)

Place recovery marks at each vertex according to independent rate-$\mu$ [Poisson processes](probability-theory.md#poisson-process) and infection arrows on each oriented nearest-neighbour edge according to independent rate-$\lambda$ Poisson processes. A vertex is infected at time $t$ exactly when a time-directed path from an initially infected vertex reaches it while following arrows and avoiding recovery marks.

##### Independent oriented-percolation comparison for the contact process

↑ **Parent:** [Graphical representation of the contact process](#graphical-representation-of-the-contact-process)

For the one-dimensional [contact process](#contact-process) with recovery rate one and per-neighbour infection rate $\lambda$, use parity sites $(x,n)$ with $x+n$ even. Call a site good if $x$ has no recovery in $[(n-1)\delta,(n+1)\delta]$ and sends an arrow to each neighbour during $[n\delta,(n+1)\delta]$. The goodness indicators are independent: recovery intervals for successive parity sites at the same spatial point only touch at endpoints, and all outgoing-arrow intervals and clocks are disjoint. Their common probability is the displayed $q$. A path of good sites carries infection from each time layer to the next, because both its source and target avoid recovery during the transmitting interval. Taking $\delta=\lambda^{-1/2}$ makes $q\to1$. The [incoming-edge coupling of site and bond percolation](probability-theory.md#incoming-edge-coupling-of-site-and-bond-percolation) and $p_c^{\mathrm{bond}}<1$ imply $p_c^{\mathrm{site}}<1$, so this proves a finite critical infection rate.

##### Dimension comparison for the contact process

↑ **Parent:** [Graphical representation of the contact process](#graphical-representation-of-the-contact-process)

Map a site $x\in\mathbb Z^d$ to its height $h(x)=\sum_i x_i$. Maintain one infected representative in height $n$ for every infected site of an auxiliary one-dimensional [contact process](#contact-process). The representative's death makes that auxiliary site recover. Its $d$ outgoing arrows to each neighbouring height, each of rate $\lambda$, make an auxiliary infection at total rate $d\lambda$, using the arrow's target as the new representative. Arrows to an already infected auxiliary height do nothing there. Distinct active representatives use distinct death and outgoing-arrow clocks, so their conditional rates are exactly those of the one-dimensional process. Every auxiliary infection has a live representative upstairs, proving the survival comparison.

##### Additivity of the contact process

↑ **Parent:** [Graphical representation of the contact process](#graphical-representation-of-the-contact-process)

Reachability in the graphical representation gives

$$
\xi_t^{A\cup B}=\xi_t^A\cup\xi_t^B.
$$

##### Duality of the contact process

↑ **Parent:** [Graphical representation of the contact process](#graphical-representation-of-the-contact-process)

Time reversal of the Poisson graphical representation, together with reversal of every infection arrow, gives

$$
\mathbb P(\xi_t^A\cap B\ne\varnothing)
=\mathbb P(\xi_t^B\cap A\ne\varnothing).
$$

#### Survival probability of the contact process

↑ **Parent:** [Contact process](#contact-process)

The survival probability is the probability that the contact process begun from one infected vertex never reaches its absorbing empty state. Its critical infection rate is $\lambda_c(\mu)=\inf\{\lambda:\theta(\lambda,\mu)>0\}$.

##### Local survival threshold of the contact process

↑ **Parent:** [Survival probability of the contact process](#survival-probability-of-the-contact-process)

Local survival means repeated infection of a fixed [vertex](graph.md#vertex-graph-theory) at arbitrarily large times in the [contact process](#contact-process). It implies global survival, but infection can survive by moving away from every fixed [vertex](graph.md#vertex-graph-theory) on an infinite [graph](graph.md). On a transitive [graph](graph.md) the threshold is independent of the chosen [vertex](graph.md#vertex-graph-theory), and $\lambda_1\le\lambda_2$, with $\lambda_1$ the [global survival threshold of the contact process](#global-survival-threshold-of-the-contact-process).

###### Height-weighted local extinction bound for the contact process

↑ **Parent:** [Local survival threshold of the contact process](#local-survival-threshold-of-the-contact-process)

Orient a degree-$(d+1)$ [regular tree](combinatorics.md#regular-tree) towards one end, and let height $g$ decrease along the unique parent [edge](graph-theory.md#edge-of-a-graph) and increase along the $d$ child [edges](graph-theory.md#edge-of-a-graph). For $w_\rho(A)=\sum_{x\in A}\rho^{g(x)}$, suppressing the occupied-target constraint only increases births, so its [infinitesimal generator](#infinitesimal-generator-stochastic-processes) satisfies $Lw_\rho\le[-1+\lambda(\rho^{-1}+d\rho)]w_\rho$. For $d>1$, choose $\rho=d^{-1/2}$. If $\lambda<1/(2\sqrt d)$, the expected weight and the infection [probability](probability-theory.md#probability) at each fixed site decay exponentially. The expected number of recoveries there equals its expected total occupation time, which is finite. Each infection episode ends almost surely at a recovery, so infinitely late infection is impossible. For $d=1$, take $\rho<1$ sufficiently close to one for each $\lambda<1/2$.

##### Global survival threshold of the contact process

↑ **Parent:** [Survival probability of the contact process](#survival-probability-of-the-contact-process)

This is the critical infection rate for the [contact process](#contact-process) started from one infected site to avoid its absorbing empty state forever. It concerns infection somewhere in the [graph](graph.md) at all times, rather than repeated infection of a fixed site. On a transitive [graph](graph.md) it is independent of the starting site. Infection-arrow inclusion couples different rates monotonically.

###### Two-vertex branching comparison for contact-process survival

↑ **Parent:** [Global survival threshold of the contact process](#global-survival-threshold-of-the-contact-process)

Inside a rooted $d$-ary subtree of a degree-$(d+1)$ [regular tree](combinatorics.md#regular-tree), pair each cell root with one distinguished child. Keep reinfection inside each pair, suppress infection back into its parent cell, and allow each child cell to be activated only once. Offspring counts of different cells are independent and identically distributed, so cell genealogies form a [Galton-Watson process](probability-and-statistics.md#galton-watson-process). A cell root has $d-1$ outgoing child-cell [edges](graph-theory.md#edge-of-a-graph) and its paired [vertex](graph.md#vertex-graph-theory) has $d$. Starting at the root, the [probabilities](probability-theory.md#probability) to send an arrow along one specified outgoing [edge](graph-theory.md#edge-of-a-graph) from these two [vertices](graph.md#vertex-graph-theory) before internal extinction are respectively

$$
a=\frac{2\lambda^3+3\lambda^2+2\lambda}{D},\qquad b=\frac{2\lambda^3+2\lambda^2}{D},\qquad D=2\lambda^3+4\lambda^2+5\lambda+2.
$$

They follow by first-step equations on the three nonempty pair states. The offspring mean is $M=(d-1)a+db$, and

$$
M\bigl(1/(d-1)\bigr)-1=\frac{2(d-1)}{2d^3-d^2+1}>0.
$$

Continuity makes $M>1$ at some strictly smaller positive rate. The [branching-process extinction criterion](probability-and-statistics.md#branching-process-extinction-criterion) then gives positive survival [probability](probability-theory.md#probability) for the suppressed process, hence for the original [contact process](#contact-process).

## Telegraph process

↑ **Parent:** [Stochastic process](stochastic-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Telegraph_process)

The telegraph process moves at one of two opposite constant velocities and reverses direction at Poisson event times. Its position has finite propagation speed and persistent increments.

### Diffusion limit of the telegraph process

↑ **Parent:** [Telegraph process](#telegraph-process)

If speed $s$ and reversal rate $\lambda$ tend to infinity with $s^2/(2\lambda)=D$ fixed, the integrated telegraph velocity converges to Brownian motion with diffusivity $D$.

## Stationary increments

↑ **Parent:** [Stochastic process](stochastic-process.md)

A stochastic process has stationary increments when the distribution of $X_{t+s}-X_t$ depends only on $s$.

## Independent increments

↑ **Parent:** [Stochastic process](stochastic-process.md)

A stochastic process has independent increments when its increments over pairwise disjoint time intervals are [independent random variables](random-variable.md#independent-random-variables).

## Finite-dimensional distribution

↑ **Parent:** [Stochastic process](stochastic-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finite-dimensional_distribution)

For times $t_1,\ldots,t_n$, the corresponding finite-dimensional distribution of a [stochastic process](stochastic-process.md) $X$ is the [joint probability distribution](probability-theory.md#joint-probability-distribution) of the [random vector](random-variable.md#random-vector) $(X_{t_1},\ldots,X_{t_n})$. The collection of these distributions records every finite set of coordinates of the process.

### Kolmogorov extension theorem

↑ **Parent:** [Finite-dimensional distribution](#finite-dimensional-distribution)

Consistent probability distributions on finite collections of coordinates in standard Borel spaces determine a unique probability measure on the product cylinder $\sigma$-algebra. In particular repeated products of a fixed distribution construct an [independent and identically distributed](random-variable.md#independent-and-identically-distributed-random-variables) sequence.

## Covariance function

↑ **Parent:** [Stochastic process](stochastic-process.md)

The covariance function of a second-order [stochastic process](stochastic-process.md) $(X_t)$ is

$$
C(s,t)=\operatorname{Cov}(X_s,X_t).
$$

It is a [positive-semidefinite kernel](probability-and-statistics.md#positive-semidefinite-kernel) and determines the [finite-dimensional distributions](#finite-dimensional-distribution) of a centered [Gaussian process](#gaussian-process).

## Kolmogorov continuity theorem

↑ **Parent:** [Stochastic process](stochastic-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kolmogorov_continuity_theorem)

If a [stochastic process](stochastic-process.md) indexed by a subset of $\mathbb R^d$ satisfies

$$
\mathbb E|X_t-X_s|^p\leq C|t-s|^{d+\beta}
$$

for some $p,\beta>0$, then it has a continuous modification. More precisely, that modification is locally $\gamma$-Hölder continuous for every $\gamma<\beta/p$.

### Dyadic increment chaining

↑ **Parent:** [Kolmogorov continuity theorem](#kolmogorov-continuity-theorem)

For a function on the [dyadic rationals](arithmetic.md#dyadic-rational) in $[0,1]$, let $A_n$ be its largest absolute adjacent increment on the level-$n$ grid. If $K_\alpha<\infty$ for $\alpha>0$, the function extends uniquely to a [Hölder continuous function](sobolev-space.md#holder-condition) with

$$
|X_t-X_s|\leq K_\alpha|t-s|^\alpha.
$$

Choose $n$ with $2^{-n}\leq|t-s|<2^{1-n}$. The level-$n$ left approximations differ by at most two grid steps, and each finer approximation adds at most one level increment. Thus the difference is bounded by $2\sum_{j\geq n}A_j\leq2^{-n\alpha}K_\alpha$. For a [stochastic process](stochastic-process.md) with $\|\xi_t-\xi_s\|_p\leq C|t-s|^\beta$, the bound $\|A_n\|_p\leq C2^{-n(\beta-1/p)}$ makes this series converge in the [Lp norm](real-analysis.md#lp-norm) for $0<\alpha<\beta-1/p$.

## Brownian snake

↑ **Parent:** [Stochastic process](stochastic-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Brownian_snake)

For a nonnegative [continuous function](calculus.md#continuous-function) $g$ on $[0,1]$ that vanishes at both endpoints, the head of the Brownian snake driven by $g$ is the centered [Gaussian process](#gaussian-process) $(Z_t)_{0\leq t\leq1}$ with [covariance function](#covariance-function)

$$
\mathbb E[Z_sZ_t]=m_g(s,t)
=\inf_{r\in[s\wedge t,s\vee t]}g(r).
$$

Consequently $\mathbb E[(Z_t-Z_s)^2]=d_g(s,t)$, the [pseudometric](topological-analysis.md#pseudometric) used by the [real tree encoded by an excursion](topological-analysis.md#real-tree-encoded-by-an-excursion).

<h3 id="holder-regularity-of-the-brownian-snake">Hölder regularity of the Brownian snake</h3>

↑ **Parent:** [Brownian snake](#brownian-snake)

If the driving function $g$ is $\alpha$-Hölder continuous, then its [Brownian snake](#brownian-snake) has a modification that is $\gamma$-Hölder continuous for every $\gamma<\alpha/2$. Indeed,

$$
\mathbb E|Z_t-Z_s|^p=C_p d_g(s,t)^{p/2}
\leq C'_p|t-s|^{\alpha p/2},
$$

and the conclusion follows from the [Kolmogorov continuity theorem](#kolmogorov-continuity-theorem) by taking $p$ arbitrarily large.

<h2 id="schramm-loewner-evolution">Schramm–Loewner evolution</h2>

↑ **Parent:** [Stochastic process](stochastic-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schramm–Loewner_evolution)

Chordal Schramm–Loewner evolution in the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) from $0$ to $\infty$ is the random [Loewner chain](#loewner-chain) driven by $U_t=\sqrt\kappa B_t$, where $B$ is standard [Brownian motion](brownian-motion.md) and $\kappa\geq0$.

### Cardy boundary crossing formula

↑ **Parent:** [Schramm–Loewner evolution](#schramm-loewner-evolution)

For critical planar percolation in a conformal quadrilateral, Cardy's boundary-crossing probability is $I_\theta(1/3,1/3)$, where $\theta\in(0,1)$ is its conformal cross-ratio and $I$ is the regularized incomplete beta function. This conformally invariant crossing law is associated with [Schramm–Loewner evolution](#schramm-loewner-evolution) at parameter six.

The conformally invariant critical percolation crossing probability can be expressed in an appropriate ordered boundary cross ratio $\theta\in[0,1]$ as

$$
\frac{\int_0^\theta[u(1-u)]^{-2/3}\,du}{\int_0^1[u(1-u)]^{-2/3}\,du}.
$$

For the corresponding [SLE](#schramm-loewner-evolution) exploration at parameter six, it arises from the [beta integral for strict ordering of coupled Bessel lifetimes](brownian-motion.md#beta-integral-for-strict-ordering-of-coupled-bessel-lifetimes) with $a=1/3$. In the upper-half-plane configuration $0<x<y$, the strict-swallowing probability is this function at $\theta=1-x/y$. Exchanging the two relevant boundary arcs exchanges the probability with its complement. This is a crossing probability, not the probability of visiting a fixed boundary point.

### Chordal SLE4

↑ **Parent:** [Schramm–Loewner evolution](#schramm-loewner-evolution)

Chordal [SLE](#schramm-loewner-evolution) at parameter four has driver $2\beta_t$ in half-plane-capacity time. The [Itô formula](stochastic-calculus.md#ito-s-lemma) makes the imaginary part of $\log(g_t(z)-W_t)$ drift-free, a feature used in the [SLE4 coupling with a Gaussian free field](#sle4-coupling-with-a-gaussian-free-field). The trace is simple and avoids fixed nonzero boundary points.

<h3 id="radial-schramm-loewner-evolution">Radial Schramm–Loewner evolution</h3>

↑ **Parent:** [Schramm–Loewner evolution](#schramm-loewner-evolution)

Radial [SLE](#schramm-loewner-evolution) grows from a boundary point to an interior target. In the unit disc from $1$ to $0$, its conformal-radius parameterization satisfies

$$
\partial_tg_t(z)=g_t(z)\frac{e^{i\sqrt\kappa\beta_t}+g_t(z)}{e^{i\sqrt\kappa\beta_t}-g_t(z)},\qquad g_t'(0)=e^t.
$$

The target remains in the remaining simply connected component; the time parameter records its decreasing [conformal radius](geometry-and-topology.md#conformal-radius).

#### Radial SLE2

↑ **Parent:** [Radial Schramm–Loewner evolution](#radial-schramm-loewner-evolution)

For radial [SLE](#schramm-loewner-evolution) at parameter two, the normalized slit-domain [Poisson kernel](partial-differential-equation.md#poisson-kernel-for-the-upper-half-plane) at the growing tip is a [local martingale](martingale.md#local-martingale). This observable provides the coupling to [loop-erasure of planar Brownian motion](markov-process.md#loop-erasure-of-planar-brownian-motion), oriented from the boundary point to the interior target. Its discrete counterpart is a [loop-erased random walk](markov-process.md#loop-erased-random-walk).

### Scale-and-domain-Markov characterization of SLE

↑ **Parent:** [Schramm–Loewner evolution](#schramm-loewner-evolution)

Among [Loewner chains](#loewner-chain) with capacity $2t$, continuous real driver and initial driver zero, scale invariance and the centered [domain Markov property of a chordal Loewner chain](#domain-markov-property-of-a-chordal-loewner-chain) characterize [Schramm–Loewner evolution](#schramm-loewner-evolution) with some $\kappa\geq0$. [Driving-function reconstruction for a chordal Loewner chain](#driving-function-reconstruction-for-a-chordal-loewner-chain) turns the hull properties into stationary independent increments and Brownian scaling for the driver. The [continuous Lévy process](#continuous-levy-process) classification then gives $U_t=bt+\sqrt\kappa W_t$, and scaling eliminates $b$. Regularity and parametrization are essential hypotheses of this characterization.

### SLE angle process

↑ **Parent:** [Schramm–Loewner evolution](#schramm-loewner-evolution)

With the upper-half-plane branch, $\theta_t\in(0,\pi)$ before the [Loewner swallowing time](#interior-point-swallowing-time-for-a-loewner-chain). Write $Z_t=X_t+iY_t$. The [Itô formula](stochastic-calculus.md#ito-s-lemma) and the [Chordal Loewner equation](#chordal-loewner-equation) give

$$
d\theta_t=(\kappa-4)\frac{X_tY_t}{|Z_t|^4}\,dt+\sqrt\kappa\frac{Y_t}{|Z_t|^2}\,dB_t.
$$

At parameter four its drift vanishes. At other parameters the drift describes the competition between the deterministic conformal evolution and the Brownian driver.

#### Dirichlet boundary values of the SLE angle process

↑ **Parent:** [SLE angle process](#sle-angle-process)

For the [SLE angle process](#sle-angle-process), the bounded [Dirichlet problem](analysis.md#dirichlet-problem) on the unbounded surviving domain has data $\pi$ on the intrinsic boundary mapped to the left of the [Loewner driving function](#loewner-driving-function) and zero on the boundary mapped to its right. For a simple [Loewner trace](#trace-of-a-loewner-chain) these are its left and right banks, with the negative and positive real rays respectively. The tip is a discontinuity point of the boundary data.

#### Logarithmic martingale for SLE4

↑ **Parent:** [SLE angle process](#sle-angle-process)

For [Schramm–Loewner evolution](#schramm-loewner-evolution) with $\kappa=4$ and $Z_t=g_t(z)-2W_t$, the [Itô formula](stochastic-calculus.md#ito-s-lemma) for the [complex logarithm](analysis.md#complex-logarithm) gives $d\log Z_t=-2Z_t^{-1}dW_t$ before swallowing. The drift cancels exactly at this parameter. Its real part is $\log|Z_t|$ and its imaginary part is the [SLE4 angle martingale](#sle4-angle-martingale). The real-part [quadratic variation](stochastic-calculus.md#quadratic-variation) is $4\int X_t^2/|Z_t|^4\,dt$, which also gives a direct non-swallowing argument.

##### Fixed-interior-point avoidance of SLE4

↑ **Parent:** [Logarithmic martingale for SLE4](#logarithmic-martingale-for-sle4)

Every fixed $z\in\mathbb H$ has infinite [interior-point swallowing time for a Loewner chain](#interior-point-swallowing-time-for-a-loewner-chain) under [Schramm–Loewner evolution](#schramm-loewner-evolution) at $\kappa=4$. The centered flow is bounded on any finite horizon, making $\log|Z_t|$ bounded above. The [one-sided bound criterion for a martingale clock](martingale.md#one-sided-bound-criterion-for-a-martingale-clock) gives a finite logarithmic limit at any putative finite swallowing time. Thus $|Z_t|$ stays away from zero and the imaginary coordinate remains positive, so the differential equation extends, a contradiction. In particular the trace misses each fixed interior point almost surely.

#### SLE4 angle martingale

↑ **Parent:** [SLE angle process](#sle-angle-process)

For a fixed [interior](topology.md#interior-topology) point and parameter four, the [SLE angle process](#sle-angle-process) has zero drift and satisfies $\theta_t=\arg z+2\int_0^tY_s|Z_s|^{-2}\,dB_s$. Its values in $(0,\pi)$ make this continuous [local martingale](martingale.md#local-martingale) a true bounded [martingale](martingale.md). The identity $\log(\Upsilon_t/\Upsilon_0)=-[\theta]_t$, together with the [Dambis-Dubins-Schwarz theorem](martingale.md#dambis-dubins-schwarz-theorem), prevents its [Loewner conformal radius](geometry-and-topology.md#conformal-radius-under-a-chordal-loewner-flow) from vanishing at a finite lifetime. Since the parameter-four trace is simple and does not meet the real [boundary](topology.md#boundary-of-a-set) at positive times, finite swallowing would require a visit to the point and vanishing radius. Thus its [Loewner swallowing time](#interior-point-swallowing-time-for-a-loewner-chain) is infinite almost surely. This gives a global continuous bounded [martingale](martingale.md), not just one defined before swallowing.

#### SLE interior-point martingale

↑ **Parent:** [SLE angle process](#sle-angle-process)

For $\kappa>0$, $\rho>0$, let $J_t=|g_t'(z)|$, $S_t=\sin\theta_t$ and $\Upsilon_t=Y_t/J_t$. Then

$$
M_t=J_t^{(8-\kappa+\rho)\rho/(4\kappa)}\Upsilon_t^{\rho(\rho+8)/(8\kappa)}S_t^{-\rho/\kappa}
$$

is a positive continuous [local martingale](martingale.md#local-martingale) before the [Loewner swallowing time](#interior-point-swallowing-time-for-a-loewner-chain). Indeed the [Itô formula](stochastic-calculus.md#ito-s-lemma) gives $d\log J_t=-2(X_t^2-Y_t^2)|Z_t|^{-4}dt$, $d\log\Upsilon_t=-4Y_t^2|Z_t|^{-4}dt$, and

$$
d\log S_t=\frac{(\kappa/2-4)X_t^2-\kappa Y_t^2/2}{|Z_t|^4}\,dt+\sqrt\kappa\frac{X_t}{|Z_t|^2}\,dB_t.
$$

Combining the exponents cancels the drift of $M_t$, including the quadratic-variation correction, leaving $dM_t/M_t=-\rho X_t/(\sqrt\kappa|Z_t|^2)\,dB_t$.

### Compact H-hull

↑ **Parent:** [Schramm–Loewner evolution](#schramm-loewner-evolution)

A compact H-hull is a bounded relatively closed subset $A$ of the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) $\mathbb H$ such that $\mathbb H\setminus A$ is a [simply connected domain](complex-analysis.md#simply-connected-domain).

#### Mapping-out function of a compact H-hull

↑ **Parent:** [Compact H-hull](#compact-h-hull)

The mapping-out function is the unique [conformal map](geometry-and-topology.md#conformal-map) $g_A:\mathbb H\setminus A\to\mathbb H$ with [hydrodynamic normalization at infinity](#hydrodynamic-normalization-at-infinity)

$$
g_A(z)=z+\frac{a}{z}+O(|z|^{-2}).
$$

##### Monotonicity of boundary derivatives of mapping-out functions

↑ **Parent:** [Mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull)

For nested [compact H-hulls](#compact-h-hull) whose closures avoid $x\in\mathbb R$, the [boundary derivative is an excursion avoidance probability](brownian-motion.md#boundary-derivative-is-an-excursion-avoidance-probability). Avoiding the larger hull is a subset of avoiding the smaller one, which proves the derivative inequality. For a hull contained in $\{|z|\leq R\}$ and $|x|>R$, comparison with the filled half-disc gives the sharp bound $1-R^2/x^2\leq g_A'(x)\leq1$, since that half-disc has [mapping-out function](#mapping-out-function-of-a-compact-h-hull) $z+R^2/z$. The empty hull and filled half-disc attain the two bounds.

##### Differentiability estimate for a mapping-out function

↑ **Parent:** [Mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull)

If a [compact H-hull](#compact-h-hull) lies in a disc of radius $r$ centred at $\xi\in\mathbb R$, the displayed estimate holds for $|z-\xi|>2r$, with an absolute constant $C$. It refines the Laurent expansion uniformly in the hull and supplies the first-order increment needed to derive the [Chordal Loewner equation](#chordal-loewner-equation) from the [Loewner local growth property](#loewner-local-growth-property).

##### High-level escape representation of a mapping-out height

↑ **Parent:** [Mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull)

Let $D=\mathbb H\setminus K$ and stop [planar Brownian motion](brownian-motion.md#planar-brownian-motion) from $z\in D$ on reaching height $R$ or leaving $D$. Then $\operatorname{Im}g_K(z)=\lim_{R\to\infty}R\mathbb P_z(\operatorname{Im}B_{\tau_R}=R)$. The stopped harmonic height is a bounded [martingale](martingale.md). The bounded difference $g_K(z)-z$ makes its top-boundary value differ from $R$ by a uniform constant, while optional stopping of the imaginary coordinate bounds the top exit probability by $\operatorname{Im}z/R$. Killing on the hull is essential.

##### Height contraction of a hydrodynamically normalized mapping-out function

↑ **Parent:** [Mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull)

For a [compact H-hull](#compact-h-hull), $v(z)=\operatorname{Im}g_K(z)$ is harmonic and satisfies $0<v(z)\leq\operatorname{Im}z$. Local boundedness and the interior continuity of $g_K^{-1}$ show that $v$ tends to zero at every finite boundary point. The [maximum principle for harmonic functions](partial-differential-equation.md#maximum-principle-for-harmonic-functions) applied to $v-\operatorname{Im}z$, with an exhaustion controlling infinity through the Laurent expansion, proves the inequality without boundary smoothness.

##### Inverse-at-infinity criterion for local boundedness of a mapping-out function

↑ **Parent:** [Mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull)

The inverse of a hydrodynamically normalized [mapping-out function](#mapping-out-function-of-a-compact-h-hull) has expansion $f(w)=w+O(1/w)$ at infinity. If bounded-domain points $z_n$ had unbounded images $w_n=g(z_n)$, then $z_n=f(w_n)=w_n+O(1/w_n)$ would be unbounded, a contradiction. Thus $g$ is bounded even near finite rough boundary points. Its own expansion at infinity then makes $g(z)-z$ uniformly bounded throughout the domain. Reflection is needed only near infinity, not along the entire hull boundary.

##### Mapping-out function of a vertical slit

↑ **Parent:** [Mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull)

For the [compact H-hull](#compact-h-hull) $(x,x+ih]$, the square-root branch asymptotic to $z-x$ gives the [hydrodynamic normalization at infinity](#hydrodynamic-normalization-at-infinity) of its [mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull). Its expansion has coefficient $h^2/2$, the [half-plane capacity of a vertical slit](#half-plane-capacity-of-a-vertical-slit).

##### Real boundary bounds for a unit-disc H-hull

↑ **Parent:** [Mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull)

If a [compact H-hull](#compact-h-hull) lies in the unit disc, compare its tail [harmonic measure](brownian-motion.md#harmonic-measure) with that of the empty hull and filled half-disc. The [Poisson kernel for the upper half-plane](partial-differential-equation.md#poisson-kernel-for-the-upper-half-plane) turns the inclusion of Brownian exit events into $x\leq g_K(x)\leq x+1/x$ for $x>1$. Reflection gives $x+1/x\leq g_K(x)\leq x$ for $x<-1$.

###### Sharp displacement bound for a compact H-hull

↑ **Parent:** [Real boundary bounds for a unit-disc H-hull](#real-boundary-bounds-for-a-unit-disc-h-hull)

For a [compact H-hull](#compact-h-hull) inside the disc of radius $r$ centred at a real point, its [mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull) displaces every point of its domain by at most $3r$. After scaling and translation, the [real boundary bounds for a unit-disc H-hull](#real-boundary-bounds-for-a-unit-disc-h-hull) put the corresponding inverse boundary interval inside $[-2,2]$. Boundary cluster points of the inverse over this interval lie in the unit disc. The [maximum modulus principle](complex-analysis.md#maximum-modulus-principle) applied to $w-g_K^{-1}(w)$ gives the bound without assuming [local connectedness](topology.md#locally-connected-space) of the hull. The [nearly closed semicircular slit](#nearly-closed-semicircular-slit) makes the constant three sharp.

###### Nearly closed semicircular slit

↑ **Parent:** [Sharp displacement bound for a compact H-hull](#sharp-displacement-bound-for-a-compact-h-hull)

With $m(z)=(z+1)/(1-z)$, the [compact H-hull](#compact-h-hull) $K_L=m^{-1}(i(0,L])$ is a unit semicircular arc attached at $-1$, with a narrow passage near $1$. As $L\to\infty$, its normalized [mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull) tends to $2$ at each fixed point of the interior bay. Points in that bay tending to $-1$ therefore have displacement approaching three. The order of these two limits is important.

##### Hydrodynamic normalization at infinity

↑ **Parent:** [Mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull)

A conformal map from an upper-half-plane domain has hydrodynamic normalization when $g(z)-z\to0$ at infinity. For a compact H-hull this normalization makes its [mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull) unique.

##### Half-plane capacity

↑ **Parent:** [Mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Half-plane_capacity)

The half-plane capacity of a [compact H-hull](#compact-h-hull) is the nonnegative coefficient $a$ in

$$
g_A(z)=z+\frac{a}{z}+O(|z|^{-2}).
$$

###### Half-plane capacity versus harmonic hull capacity

↑ **Parent:** [Half-plane capacity](#half-plane-capacity)

The [Brownian representation of half-plane capacity](#brownian-representation-of-half-plane-capacity) is $\operatorname{hcap}(K)=\lim_{y\to\infty}y\mathbb E_{iy}\operatorname{Im}B_T$. The [harmonic capacity from infinity in the upper half-plane](brownian-motion.md#harmonic-capacity-from-infinity-in-the-upper-half-plane) uses $\operatorname{cap}(K)=\lim_{y\to\infty}\pi y\mathbb P_{iy}(B_T\in K)$. Since $0\leq\operatorname{Im}B_T\leq\operatorname{rad}(K)\mathbf1_{\{B_T\in K\}}$, the displayed bound follows. The normalization factor $\pi$ cannot be omitted. Independently, enclosure in a half-disc and [monotonicity of half-plane capacity](#monotonicity-of-half-plane-capacity) give the sharp bound $\operatorname{hcap}(K)\leq\operatorname{rad}(K)^2$.

###### Half-plane capacity of a half-disc

↑ **Parent:** [Half-plane capacity](#half-plane-capacity)

For $x\in\mathbb R$ and $R>0$, the filled half-disc $K=\{z\in\mathbb H:|z-x|\leq R\}$ is a [compact H-hull](#compact-h-hull). Its [mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull) is $g_K(z)=z+R^2/(z-x)$. On the semicircle the image is real, and the inverse branch asymptotic to the identity maps the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) onto the exterior half-disc. Its [Laurent series](analysis.md#laurent-series) has coefficient $R^2/z$, so $\boxed{\operatorname{hcap}(K)=R^2}$. Using an open half-disc instead requires taking its relative [closure](topology.md#closure-topology) first.

###### Conformal change of half-plane capacity

↑ **Parent:** [Half-plane capacity](#half-plane-capacity)

Suppose a capacity-parameterized [Loewner chain](#loewner-chain) lies in a domain on which $\psi$ is a [conformal map](geometry-and-topology.md#conformal-map). For its image chain set $\psi_t=\widetilde g_t\circ\psi\circ g_t^{-1}$. Then the image [Loewner driving function](#loewner-driving-function) is $\widetilde U_t=\psi_t(U_t)$ and

$$
d\operatorname{hcap}(\widetilde A_t)=2\psi_t'(U_t)^2\,dt.
$$

The derivative is real by the [Schwarz reflection principle](complex-analysis.md#schwarz-reflection-principle). Cancellation of the pole in the differentiated conjugacy identity proves the squared-derivative rule.

###### Conformal conjugacy derivative for the chordal Loewner equation

↑ **Parent:** [Conformal change of half-plane capacity](#conformal-change-of-half-plane-capacity)

For conjugated [Loewner chains](#loewner-chain), $\phi_t=\widetilde g_t\circ\phi\circ g_t^{-1}$ and $\widetilde\xi_t=\phi_t(\xi_t)$. The image capacity speed is $2\phi_t'(\xi_t)^2$. Differentiating this identity gives $\dot\phi_t(z)=2\phi_t'(\xi_t)^2/(\phi_t(z)-\phi_t(\xi_t))-2\phi_t'(z)/(z-\xi_t)$. The removable singularity at the driver has value $-3\phi_t''(\xi_t)$.

###### Boundary derivative diffusion under conformal Loewner conjugacy

↑ **Parent:** [Conformal conjugacy derivative for the chordal Loewner equation](#conformal-conjugacy-derivative-for-the-chordal-loewner-equation)

Let $h_t$ intertwine two [Loewner chains](#loewner-chain), with driver $\xi_t=\sqrt\kappa B_t$, and set $a_t=h_t'(\xi_t)$, $b_t=h_t''(\xi_t)$, $c_t=h_t'''(\xi_t)$. Expanding the conjugacy equation at the driver gives $\partial_t h_t'(\xi_t)=b_t^2/(2a_t)-4c_t/3$; the [Itô formula](stochastic-calculus.md#ito-s-lemma) gives the displayed diffusion. For a real exponent $p$, the drift of $a_t^p$ is $p[1+\kappa(p-1)]a_t^{p-2}b_t^2/2+p(\kappa/2-4/3)a_t^{p-1}c_t$. At $\kappa=8/3$, $p=5/8$ cancels both terms and yields the [SLE eight-thirds restriction martingale](#sle-eight-thirds-restriction-martingale).

###### Transformed SLE driving function

↑ **Parent:** [Conformal conjugacy derivative for the chordal Loewner equation](#conformal-conjugacy-derivative-for-the-chordal-loewner-equation)

Apply the [Itô formula](stochastic-calculus.md#ito-s-lemma) to the transformed [Loewner driving function](#loewner-driving-function) $\widetilde\xi_t=\phi_t(\sqrt\kappa W_t)$. The [conformal conjugacy derivative for the chordal Loewner equation](#conformal-conjugacy-derivative-for-the-chordal-loewner-equation) cancels the Itô drift exactly when $\kappa=6$. Its [quadratic variation](stochastic-calculus.md#quadratic-variation) is $\kappa\int_0^t\phi_s'(\xi_s)^2ds$.

###### Half-plane capacity of a vertical slit

↑ **Parent:** [Half-plane capacity](#half-plane-capacity)

For a vertical slit of height $h>0$ attached at $x\in\mathbb R$, the [mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull) is $g(z)=x+\sqrt{(z-x)^2+h^2}$, with the branch asymptotic to $z-x$ at infinity. Its [half-plane capacity](#half-plane-capacity) is $h^2/2$.

###### Scaling and translation of half-plane capacity

↑ **Parent:** [Half-plane capacity](#half-plane-capacity)

For $\lambda>0$ and $x\in\mathbb R$,

$$
g_{\lambda A+x}(z)=x+\lambda g_A\!\left(\frac{z-x}{\lambda}\right),
\qquad
\operatorname{hcap}(\lambda A+x)=\lambda^2\operatorname{hcap}(A).
$$

###### Monotonicity of half-plane capacity

↑ **Parent:** [Half-plane capacity](#half-plane-capacity)

If compact H-hulls satisfy $A\subseteq C$, then

$$
\operatorname{hcap}(A)\leq\operatorname{hcap}(C).
$$

This follows from the [Brownian representation of half-plane capacity](#brownian-representation-of-half-plane-capacity) or from composition of their mapping-out functions.

###### Half-plane-capacity composition rule

↑ **Parent:** [Monotonicity of half-plane capacity](#monotonicity-of-half-plane-capacity)

If compact H-hulls satisfy $A\subseteq C$ and $D$ is the bounded filling of $g_A(C\setminus A)$, then

$$
g_C=g_D\circ g_A,
\qquad
\operatorname{hcap}(C)
=\operatorname{hcap}(A)+\operatorname{hcap}(D).
$$

In particular, inclusion is strict exactly when the capacity increase is positive.

###### Brownian representation of half-plane capacity

↑ **Parent:** [Half-plane capacity](#half-plane-capacity)

If $\tau$ is the first exit time of planar [Brownian motion](brownian-motion.md) from $\mathbb H\setminus A$, then

$$
\operatorname{hcap}(A)=\lim_{y\to\infty}y\,\mathbb E_{iy}[\operatorname{Im}B_\tau].
$$

It follows by applying the [optional sampling theorem for a supermartingale](martingale.md#optional-sampling-theorem-for-a-supermartingale) to the harmonic function $\operatorname{Im}(z-g_A(z))$.

###### Half-plane capacity is bounded by squared diameter

↑ **Parent:** [Half-plane capacity](#half-plane-capacity)

There is a universal constant $C$ such that every compact H-hull satisfies

$$
\operatorname{hcap}(A)\leq C\operatorname{diam}(A)^2.
$$

Translate and scale so the hull lies in a unit half-disc, then use the [Brownian representation of half-plane capacity](#brownian-representation-of-half-plane-capacity) and the $O(y^{-1})$ [harmonic measure](brownian-motion.md#harmonic-measure) of that half-disc as viewed from $iy$.

###### Half-plane capacity of a low rectangle

↑ **Parent:** [Half-plane capacity](#half-plane-capacity)

For $R_r=[-r,r]\times(0,1]$ with $r\geq1$,

$$
\operatorname{hcap}(R_r)\leq Cr.
$$

Indeed, the imaginary part at the Brownian exit point is at most one and the probability of reaching the radius-$O(r)$ neighbourhood containing the rectangle from $iy$ is $O(r/y)$. Consequently $r^{-1}R_r=[-1,1]\times(0,r^{-1}]$ has capacity $O(r^{-1})$ although its diameter tends to two.

###### Half-plane-capacity parameterization

↑ **Parent:** [Half-plane capacity](#half-plane-capacity)

A growing hull is parameterized by half-plane capacity when $\operatorname{hcap}(K_t)=2t$. The factor two makes its [Chordal Loewner equation](#chordal-loewner-equation) take the conventional form $\partial_tg_t=2/(g_t-U_t)$.

##### Boundary degeneration under a mapping-out function

↑ **Parent:** [Mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull)

If $z_n\in\mathbb H\setminus A$ approaches a point of a compact H-hull $A$, then

$$
\operatorname{Im}g_A(z_n)\longrightarrow0.
$$

The real part need not converge: the two sides of a vertical slit have distinct real boundary values under its mapping-out function.

### Loewner chain

↑ **Parent:** [Schramm–Loewner evolution](#schramm-loewner-evolution)

A chordal Loewner chain is an increasing family of compact H-hulls, usually parameterized by [half-plane capacity](#half-plane-capacity), whose mapping-out functions evolve according to the [Chordal Loewner equation](#chordal-loewner-equation).

#### Domain Markov property of a chordal Loewner chain

↑ **Parent:** [Loewner chain](#loewner-chain)

Conditionally on the entire past up to $t$, the future domains mapped and centered by $g_t-U_t$ have the original chain law and are independent of that past. For [Schramm–Loewner evolution](#schramm-loewner-evolution) this follows from independent stationary [Brownian motion](brownian-motion.md) increments and the [composition rule for chordal Loewner driving functions](#composition-rule-for-chordal-loewner-driving-functions). The [Strong Markov property](markov-process.md#strong-markov-property) gives the version at almost surely finite stopping times.

##### Simplicity of SLE from boundary-avoiding restarts

↑ **Parent:** [Domain Markov property of a chordal Loewner chain](#domain-markov-property-of-a-chordal-loewner-chain)

Suppose a chordal [SLE](#schramm-loewner-evolution) trace stays in the open [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) at every positive time almost surely. For every deterministic rational time $s$, the [domain Markov property of a chordal Loewner chain](#domain-markov-property-of-a-chordal-loewner-chain) makes its mapped and centered future a fresh SLE, so its positive-time future stays in the open half-plane as well. The inverse [mapping-out function](#mapping-out-function-of-a-compact-h-hull) then places that future outside the entire old hull. Intersecting these probability-one events over rational $s$ rules out every self-intersection: if two times $u<v$ shared a trace point, choose rational $s$ strictly between them. This proves simplicity using the allowed boundary-avoidance assertion for $0<\kappa\leq4$.

#### Capacity-parametrized scale invariance of a Loewner chain

↑ **Parent:** [Loewner chain](#loewner-chain)

For a [Loewner chain](#loewner-chain) with [half-plane capacity](#half-plane-capacity) $2t$, scale invariance means $(\lambda^{-1}K_{\lambda^2t})_{t\geq0}$ has the original law for every $\lambda>0$. Its mapping-out maps are $\lambda^{-1}g_{\lambda^2t}(\lambda z)$ and its [Loewner driving function](#loewner-driving-function) is $\lambda^{-1}U_{\lambda^2t}$. This follows by differentiating the [Chordal Loewner equation](#chordal-loewner-equation). [Brownian scaling](brownian-motion.md#brownian-scaling) gives this property for [Schramm–Loewner evolution](#schramm-loewner-evolution).

#### Trace of a Loewner chain

↑ **Parent:** [Loewner chain](#loewner-chain)

When the indicated limit exists continuously and the hulls are generated by its past, it defines the trace of the [Loewner chain](#loewner-chain). The hull $K_t$ includes the curve up to time $t$ and any regions it disconnects from infinity. Therefore swallowing a point by $K_t$ is different from visiting that point by the [Loewner trace](#trace-of-a-loewner-chain). For [SLE](#schramm-loewner-evolution), the continuous trace is part of its basic existence theory.

##### Boundary extension of the inverse map for a continuous Loewner trace

↑ **Parent:** [Trace of a Loewner chain](#trace-of-a-loewner-chain)

For a continuous [Loewner trace](#trace-of-a-loewner-chain) generating its hulls, the inverse [mapping-out function of a compact H-hull](#mapping-out-function-of-a-compact-h-hull) $g_t^{-1}$ extends continuously to the closed [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis). The finite trace is a [continuous map](topology.md#continuous-map) image of an interval, and the [boundary](topology.md#boundary-of-a-set) of its unbounded complementary component has [local connectedness](topology.md#locally-connected-space); the [Caratheodory boundary extension theorem](complex-analysis.md#caratheodory-boundary-extension-theorem) gives the extension. In particular $g_t^{-1}(U_t)=\gamma(t)$, while $g_t^{-1}$ maps the open [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) into $D_t$. This is the deterministic boundary-extension input of [Rohde and Schramm, Theorem 4.1](https://annals.math.princeton.edu/wp-content/uploads/annals-v161-n2-p07.pdf). Under a [Conformal Markov property of SLE](#conformal-markov-property-of-sle) restart, this relates [boundary](topology.md#boundary-of-a-set) contacts of the mapped future to contacts with the old hull, without assuming the old trace is simple.

#### Loewner local growth property

↑ **Parent:** [Loewner chain](#loewner-chain)

The local growth property says that, after mapping out the hull at time $t$, the new hull grown during a short interval has diameter tending uniformly to zero with the interval length. It ensures that the growth is described by one continuous boundary point.

##### Loewner correspondence theorem

↑ **Parent:** [Loewner local growth property](#loewner-local-growth-property)

An increasing family of [compact H-hulls](#compact-h-hull) of [half-plane capacity](#half-plane-capacity) $2t$ with the [Loewner local growth property](#loewner-local-growth-property) corresponds uniquely to a continuous real [Loewner driving function](#loewner-driving-function). Its [mapping-out functions](#mapping-out-function-of-a-compact-h-hull) solve the [Chordal Loewner equation](#chordal-loewner-equation) up to the maximal lifetime of each point. Conversely each continuous driver generates that hull family. A continuous [Loewner trace](#trace-of-a-loewner-chain) is an additional property, not a consequence for every continuous driver. For [SLE](#schramm-loewner-evolution) it is supplied by the trace-existence theorem.

#### Loewner differential equation

↑ **Parent:** [Loewner chain](#loewner-chain)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Loewner_differential_equation)

The Loewner differential equation describes a growing family of simply connected planar domains through ordinary differential equations for their normalized conformal maps.

##### Chordal Loewner equation

↑ **Parent:** [Loewner differential equation](#loewner-differential-equation)

For a capacity-parameterized locally growing hull family,

$$
\partial_tg_t(z)=\frac2{g_t(z)-U_t},
\qquad g_0(z)=z,
$$

where the continuous real function $U$ is the [Loewner driving function](#loewner-driving-function).

###### Loewner variation of the Dirichlet Green function

↑ **Parent:** [Chordal Loewner equation](#chordal-loewner-equation)

With [half-plane capacity](#half-plane-capacity) $2t$, $f_t=g_t-W_t$ and $G_{\mathbb H}(z,w)=\log|(z-\overline w)/(z-w)|$, differentiating $G_{D_t}(z,w)=G_{\mathbb H}(f_t(z),f_t(w))$ gives the displayed identity. The translation by the driver cancels in the Green function. This rank-one [covariance](variance.md#covariance) loss balances the quadratic covariation of the harmonic mean in the [SLE4 coupling with a Gaussian free field](#sle4-coupling-with-a-gaussian-free-field).

###### Boundary-point swallowing time for a Loewner chain

↑ **Parent:** [Chordal Loewner equation](#chordal-loewner-equation)

For a real point $b$ away from the initial driver, this is the maximal lifetime of the real solution $\partial_tg_t(b)=2/(g_t(b)-\xi_t)$. At finite lifetime its centred image collides with the [Loewner driving function](#loewner-driving-function). A point may be visited or separated from infinity by the hull, so swallowing is not the same as an individual trace visit.

###### SLE boundary swallowing criterion

↑ **Parent:** [Boundary-point swallowing time for a Loewner chain](#boundary-point-swallowing-time-for-a-loewner-chain)

For a continuous chordal [SLE](#schramm-loewner-evolution) trace started at zero, hitting the real interval $[b,\infty)$ is equivalent to finite [boundary-point swallowing time for a Loewner chain](#boundary-point-swallowing-time-for-a-loewner-chain) at $b>0$. A boundary crosscut may swallow all points between its endpoints without visiting them individually. The [Boundary-point Bessel flow for SLE](#boundary-point-bessel-flow-for-sle) determines the probability of this event.

###### Interior-point swallowing time for a Loewner chain

↑ **Parent:** [Chordal Loewner equation](#chordal-loewner-equation)

For a continuous [Loewner driving function](#loewner-driving-function) $U$, $T_z$ is the maximal lifetime of $g_t(z)$ in the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) under the [Chordal Loewner equation](#chordal-loewner-equation). A finite lifetime has $\operatorname{Im}g_t(z)\to0$ as $t\uparrow T_z$: otherwise the continuous driver and the [ordinary differential equation](differential-equation.md#ordinary-differential-equation) continue the solution. A swallowed point need not have been visited by the [Loewner trace](#trace-of-a-loewner-chain); it may lie in a disconnected pocket of the filled hull.

###### Loewner driving function

↑ **Parent:** [Chordal Loewner equation](#chordal-loewner-equation)

The Loewner driving function $U_t$ is the real boundary point at which the mapped-out hull grows. Scaling the hulls by $a^{-1}$ and time by $a^2$ transforms it to $a^{-1}U_{a^2t}$.

###### Continuity estimate for the Loewner driving function

↑ **Parent:** [Loewner driving function](#loewner-driving-function)

Suppose the mapped increments $K_{s,t}$ have real-centred enclosing radii bounded by a nondecreasing modulus $\omega(t-s)\to0$. Nested closures define the unique growing real point $\xi_s$. For $v\in K_{t,t+h}$, its preimage $z=g_{K_{s,t}}^{-1}(v)$ belongs to $K_{s,t+h}$. The uniform displacement estimate for a [mapping-out function](#mapping-out-function-of-a-compact-h-hull) gives $|v-z|\leq C\omega(t-s)$, while $|z-\xi_s|\leq2\omega(t-s+h)$. Letting $h\downarrow0$ with $h\leq t-s$ proves the displayed estimate. It proves uniform [continuity](calculus.md#continuous-function) of the [Loewner transform](#loewner-driving-function) on each bounded time interval without evaluating a conformal map on a rough boundary.

###### Driving-function reconstruction for a chordal Loewner chain

↑ **Parent:** [Loewner driving function](#loewner-driving-function)

The domains of a capacity-parametrized [Loewner chain](#loewner-chain) determine their hydrodynamically normalized [mapping-out functions of compact H-hulls](#mapping-out-function-of-a-compact-h-hull). At a surviving point, the [Chordal Loewner equation](#chordal-loewner-equation) gives $U_t=g_t(z)-2/\partial_tg_t(z)$. For a continuous driver and $t>0$, the left derivative uses only the hull past. High points $in$, $n\in\mathbb N$, survive up to any fixed finite time for sufficiently large $n$, making this a countable local reconstruction of the driver and its past filtration.

###### Composition rule for chordal Loewner driving functions

↑ **Parent:** [Loewner driving function](#loewner-driving-function)

After time $t$, map remaining domains by $g_t-U_t$. The new [mapping-out function](#mapping-out-function-of-a-compact-h-hull) at elapsed time $s$ is $\widehat g_s(z)=g_{t+s}(g_t^{-1}(z+U_t))-U_t$. Direct differentiation of the [Chordal Loewner equation](#chordal-loewner-equation) proves that its driver is $U_{t+s}-U_t$, and its [half-plane capacity](#half-plane-capacity) is $2s$. Defining transformed hulls as complements of transformed domains avoids ambiguity at the old hull boundary.

###### Square-root Loewner driving function generates a straight slit

↑ **Parent:** [Loewner driving function](#loewner-driving-function)

For the [Chordal Loewner equation](#chordal-loewner-equation) driven by $U_t=a\sqrt t$, the hull is a straight slit whose endpoint is proportional to $\sqrt t$. Put $r_\pm=(a\pm\sqrt{a^2+16})/2$ and $\alpha=-r_-/(r_+-r_-)\in(0,1)$. Its inverse map is

$$
f_t(w)=(w-r_+\sqrt t)^\alpha(w-r_-\sqrt t)^{1-\alpha},
$$

using upper-half-plane branches. The interval between the two real roots maps onto the two sides of a segment of argument $\pi\alpha$.

###### Boundary derivative of a chordal Loewner chain

↑ **Parent:** [Loewner driving function](#loewner-driving-function)

For a real $x$ before its swallowing time,

$$
g_t'(x)=\exp\left(
-\int_0^t\frac{2\,ds}{(g_s(x)-U_s)^2}\right).
$$

It lies in $(0,1]$ and decreases with time.

### Scaling invariance of SLE

↑ **Parent:** [Schramm–Loewner evolution](#schramm-loewner-evolution)

For every $a>0$, if $(K_t)$ is $\operatorname{SLE}_\kappa$, then $(a^{-1}K_{a^2t})$ has the same law. Its driving function is $a^{-1}U_{a^2t}$, which has the same law as $U_t$ by [Brownian scaling](brownian-motion.md#brownian-scaling).

#### SLE reaches every positive height

↑ **Parent:** [Scaling invariance of SLE](#scaling-invariance-of-sle)

For a chordal [SLE](#schramm-loewner-evolution) trace $\gamma$, the [Scaling invariance of SLE](#scaling-invariance-of-sle) makes $\mathbb P(\sup_t\operatorname{Im}\gamma(t)>r)$ independent of $r>0$. The trace must enter the upper half-plane because its positive-time hull has positive [half-plane capacity](#half-plane-capacity). Letting $r\downarrow0$ therefore makes this probability one, and continuity implies that every positive height is reached. This argument does not assume [Transience of chordal SLE](#transience-of-chordal-sle).

### Conformal Markov property of SLE

↑ **Parent:** [Schramm–Loewner evolution](#schramm-loewner-evolution)

Conditionally on an $\operatorname{SLE}_\kappa$ initial segment through time $t$, mapping out that segment by $g_t-U_t$ turns the future into an independent $\operatorname{SLE}_\kappa$ in $(\mathbb H,0,\infty)$. This follows because its driving function is $U_{t+s}-U_t$, and [Brownian motion](brownian-motion.md) has [stationary increments](#stationary-increments) and [independent increments](#independent-increments).

#### Characterization of the SLE driving function

↑ **Parent:** [Conformal Markov property of SLE](#conformal-markov-property-of-sle)

The conformal Markov property gives the continuous Loewner driver stationary independent increments. Scale invariance removes its deterministic drift. Therefore

$$
U_t=\sqrt\kappa B_t
$$

for a standard Brownian motion and a constant $\kappa\geq0$.

### Conformal invariance of SLE

↑ **Parent:** [Schramm–Loewner evolution](#schramm-loewner-evolution)

Chordal [SLE](#schramm-loewner-evolution) is defined on any simply connected domain with two marked boundary points by applying a [conformal map](geometry-and-topology.md#conformal-map) from the upper half-plane. Its law is independent of the chosen map, up to a deterministic change of parameterization.

#### Chordal SLE in a specified scale

↑ **Parent:** [Conformal invariance of SLE](#conformal-invariance-of-sle)

A scale is a [conformal bijection](complex-analysis.md#biholomorphism) sending a marked starting boundary point to zero and target boundary point to infinity in the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis). A curve is [SLE](#schramm-loewner-evolution) in that scale when its image is ordinary [SLE](#schramm-loewner-evolution) using the [half-plane-capacity parameterization](#half-plane-capacity-parameterization) of that image.

#### Chordal restriction property

↑ **Parent:** [Conformal invariance of SLE](#conformal-invariance-of-sle)

A random curve $\gamma$ from $0$ to infinity in the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) has the chordal restriction property when, for every admissible compact H-hull $A$ avoiding zero, the conditional law of $\psi_A(\gamma)$ given $\gamma\cap A=\varnothing$ equals the original law of $\gamma$. Here $\psi_A:\mathbb H\setminus A\to\mathbb H$ fixes zero and has derivative one at infinity.

##### Restriction exponent of a chordal filling

↑ **Parent:** [Chordal restriction property](#chordal-restriction-property)

A conformally invariant random [chordal filling](#chordal-filling) has exponent $\alpha$ when its avoidance probability for every admissible hull $A$ is the displayed power, where $\Phi_A$ fixes zero and has derivative one at infinity. Composition of two hull-removing maps and the chain rule make conditional image avoidance probabilities the same as unconditional ones. The [avoidance probabilities determine a chordal filling law](#avoidance-probabilities-determine-a-chordal-filling-law) principle therefore implies the [chordal restriction property](#chordal-restriction-property). Independent unions followed by filling add exponents, since avoidance probabilities multiply.

##### Chordal filling

↑ **Parent:** [Chordal restriction property](#chordal-restriction-property)

A chordal filling is the closed connected set obtained from a proper boundary-to-boundary path by adding complementary pockets disconnected from both boundary arcs between its marked endpoints. In $(\mathbb H,0,\infty)$ it meets the boundary only at zero and infinity and leaves two complementary simply connected sides, adjacent to the negative and positive real axes. Equivalently it is full with respect to the two marked boundary arcs. This definition uses the [prime ends](geometry-and-topology.md#prime-end) of a general simply connected domain and is preserved by [conformal maps](geometry-and-topology.md#conformal-map).

###### Avoidance probabilities determine a chordal filling law

↑ **Parent:** [Chordal filling](#chordal-filling)

The probabilities that a random [chordal filling](#chordal-filling) avoids each admissible [compact H-hull](#compact-h-hull) away from zero determine its law as an unparameterized closed set. Each point of its complement can be joined to the relevant real boundary arc through the complement and lies in a thin rational polygonal tube attached to that arc. These countably many hull tests recover the complement. Their joint avoidance events are tested by filled finite unions; if a union separates zero from infinity, the joint avoidance event is empty. Otherwise connectedness makes avoidance of the union equivalent to avoidance of its filled hull. Thus individual hull probabilities give every finite joint indicator distribution and determine the random complement.

##### Derivative avoidance criterion for chordal restriction

↑ **Parent:** [Chordal restriction property](#chordal-restriction-property)

Suppose a random proper [simple curve](topology.md#simple-curve) from zero to infinity has the displayed avoidance probability for every admissible [compact H-hull](#compact-h-hull) $A$, with fixed $\alpha>0$. Put $\psi_A=g_A-g_A(0)$. For another admissible hull $B$ in the image [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis), map composition and the [chain rule](calculus.md#chain-rule) give $g_C'(0)=g_B'(0)g_A'(0)$ for $C=A\cup\psi_A^{-1}(B)$. The conditional image curve therefore has avoidance probabilities $g_B'(0)^\alpha$, exactly those of the original. Since [avoidance probabilities determine a simple chordal curve law](#avoidance-probabilities-determine-a-simple-chordal-curve-law), the conditional image law agrees with the original. This is the [chordal restriction property](#chordal-restriction-property).

##### Avoidance probabilities determine a simple chordal curve law

↑ **Parent:** [Chordal restriction property](#chordal-restriction-property)

For random proper [simple curves](topology.md#simple-curve) from $0$ to infinity in the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis), the probabilities of avoiding every [compact H-hull](#compact-h-hull) whose [closure](topology.md#closure-topology) excludes zero determine the unparameterized trace law. Every point off a simple chordal curve can be [connected](geometry-and-topology.md#connected-space) to a real [boundary](topology.md#boundary-of-a-set) interval away from zero within one side of its complement. A countable collection of thin rational polygonal tubes attached to that interval therefore recovers the complement from its avoidance indicators. Joint avoidance of finitely many tubes reduces to avoidance of their filled union. If the union blocks every path from zero to infinity the joint event is empty; otherwise filling pockets does not change the avoidance event. The [inclusion-exclusion principle](combinatorics.md#inclusion-exclusion-principle) gives all finite indicator distributions. These determine the random complement and hence the trace. Simplicity and properness are hypotheses; the assertion is not a general determination theorem for arbitrary random closed sets.

##### SLE eight-thirds restriction martingale

↑ **Parent:** [Chordal restriction property](#chordal-restriction-property)

For chordal $\operatorname{SLE}_{8/3}$ and an admissible hull $A$, let $\psi_t$ map out the image of $A$ after removing the SLE hull. Then

$$
M_t=\psi_t'(U_t)^{5/8}
$$

stopped when the trace meets $A$ is a bounded martingale. Its terminal value yields the avoidance probability

$$
\mathbb P(\gamma\cap A=\varnothing)=\psi_A'(0)^{5/8}.
$$

#### Locality property of SLE

↑ **Parent:** [Conformal invariance of SLE](#conformal-invariance-of-sle)

The locality property says that an [SLE](#schramm-loewner-evolution) does not detect a hull lying away from its starting point until the curve reaches that hull. Among chordal Schramm-Loewner evolutions, this property holds for $\operatorname{SLE}_6$.

##### Locality of a chord law under conformal changes of neighborhoods

↑ **Parent:** [Locality property of SLE](#locality-property-of-sle)

A scale-invariant law of unparameterized chords from zero to infinity in the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) is local when a boundary-preserving [conformal map](geometry-and-topology.md#conformal-map) between neighborhoods of zero, fixing zero, transports its curve stopped on leaving the first neighborhood to the same-law curve stopped on leaving the second. Equality concerns the stopped curves up to increasing reparameterization. For [SLE](#schramm-loewner-evolution) with parameter six, the [transformed SLE driving function](#transformed-sle-driving-function) is a [continuous local martingale](martingale.md#continuous-local-martingale) with bracket six times the image capacity clock. The [Lévy characterization of Brownian motion](brownian-motion.md#levy-characterization-of-brownian-motion) makes that driver Brownian in the new clock, proving the local stopped-curve invariance.

##### Target-change locality of SLE6

↑ **Parent:** [Locality property of SLE](#locality-property-of-sle)

Changing the target boundary point by a [conformal automorphism of the upper half-plane](complex-analysis.md#conformal-automorphism-of-the-upper-half-plane) preserves the local chordal [SLE](#schramm-loewner-evolution) law at parameter six, up to a capacity time change and until the relevant boundary point is swallowed. The [transformed SLE driving function](#transformed-sle-driving-function) has zero drift at six; the [Dambis-Dubins-Schwarz theorem](martingale.md#dambis-dubins-schwarz-theorem) makes it Brownian in image capacity time.

###### Target-dependent continuation of SLE6

↑ **Parent:** [Target-change locality of SLE6](#target-change-locality-of-sle6)

At parameter six, changing a boundary target preserves the initial unparameterized [SLE](#schramm-loewner-evolution) law until the growing hull separates the two possible targets. After separation, each curve continues in the complementary component whose boundary contains its own target. A curve targeted at infinity follows the unbounded component, whereas a finite separated target lies on a different component. The [target-change locality of SLE6](#target-change-locality-of-sle6) proof no longer applies: its [conformal automorphism of the upper half-plane](complex-analysis.md#conformal-automorphism-of-the-upper-half-plane) conjugates corresponding surviving domains only before this separation. A zero drift before contact does not give equality of complete curve laws afterwards.

### Phase classification of the SLE trace

↑ **Parent:** [Schramm–Loewner evolution](#schramm-loewner-evolution)

The trace of $\operatorname{SLE}_\kappa$ is [simple](topology.md#simple-curve) for $0<\kappa\leq4$, has self-intersections without being [space-filling](topology.md#space-filling-curve) for $4<\kappa<8$, and is space-filling for $\kappa\geq8$. The thresholds arise from the [Boundary-point Bessel flow for SLE](#boundary-point-bessel-flow-for-sle) and estimates for the [Loewner chain](#loewner-chain) near its driving point.

#### Space-filling SLE above parameter eight

↑ **Parent:** [Phase classification of the SLE trace](#phase-classification-of-the-sle-trace)

For $\kappa>8$, the [Loewner trace](#trace-of-a-loewner-chain) visits every point of the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis) almost surely. Choose $\rho=\kappa-8$ in the [SLE interior-point martingale](#sle-interior-point-martingale) to obtain $M_t=\Upsilon_t^{(\kappa-8)/8}S_t^{-(\kappa-8)/\kappa}$. The [maximal inequality for a nonnegative supermartingale](martingale.md#maximal-inequality-for-a-nonnegative-supermartingale) bounds its running supremum. If a fixed [interior](topology.md#interior-topology) ball were avoided, its center would have $\Upsilon_t\geq c_1>0$ before swallowing, forcing $S_t\geq c_2>0$. But the [Chordal Loewner equation](#chordal-loewner-equation) gives $dY_t^2/dt=-4S_t^2$, forcing a finite lifetime with $Y_t\to0$, and $d\log\Upsilon_t/d\log Y_t=2S_t^2$ then forces $\Upsilon_t\to0$, a contradiction. Countably many rational balls give a dense trace; [continuity](calculus.md#continuous-function) and [Transience of chordal SLE](#transience-of-chordal-sle) make its image relatively closed, so it is all of the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis). This argument does not cover the critical parameter eight.

#### SLE Green-function estimate

↑ **Parent:** [Phase classification of the SLE trace](#phase-classification-of-the-sle-trace)

For $0<\kappa<8$, the probability that chordal $\operatorname{SLE}_\kappa$ approaches an interior point $z$ to conformal radius at most $\epsilon$ is, on compact subsets of $\mathbb H$, comparable to

$$
G_\kappa(z)\epsilon^{1-\kappa/8},
$$

where $G_\kappa$ is the SLE Green function. The positive exponent implies that the trace has zero planar [Lebesgue measure](measure-theory.md#lebesgue-measure).

#### SLE4 left-passage probability

↑ **Parent:** [Phase classification of the SLE trace](#phase-classification-of-the-sle-trace)

For chordal $\operatorname{SLE}_4$ in $(\mathbb H,0,\infty)$,

$$
\mathbb P(\gamma\text{ passes to the right of }z)
=\frac{\arg z}{\pi}.
$$

Indeed, $\arg(g_t(z)-U_t)$ is a bounded martingale whose terminal value is zero or $\pi$ according to the side on which the trace passes.

#### Boundary-intersection threshold for SLE

↑ **Parent:** [Phase classification of the SLE trace](#phase-classification-of-the-sle-trace)

Chordal $\operatorname{SLE}_\kappa$ intersects the domain boundary away from its endpoints exactly when $\kappa>4$. The centered image of a boundary point is a Bessel process of dimension $1+4/\kappa$, which hits zero exactly below dimension two.

##### Positive boundary-interval hitting probability for SLE above parameter four

↑ **Parent:** [Boundary-intersection threshold for SLE](#boundary-intersection-threshold-for-sle)

For $\kappa>4$, the [Boundary-point Bessel flow for SLE](#boundary-point-bessel-flow-for-sle) and the [SLE boundary swallowing criterion](#sle-boundary-swallowing-criterion) imply that the full [Loewner trace](#trace-of-a-loewner-chain) hits the positive real axis almost surely. Every fixed open interval in that axis has positive hitting probability: its countably many dilates cover the axis, while [Scaling invariance of SLE](#scaling-invariance-of-sle) makes all their hitting probabilities equal. Reflection gives the corresponding negative-axis statement. Together with the [domain Markov property of a chordal Loewner chain](#domain-markov-property-of-a-chordal-loewner-chain), this produces visits to the old [Loewner trace](#trace-of-a-loewner-chain) boundary in a mapped future domain.

### Transience of chordal SLE

↑ **Parent:** [Schramm–Loewner evolution](#schramm-loewner-evolution)

The chordal [SLE](#schramm-loewner-evolution) [Loewner trace](#trace-of-a-loewner-chain) eventually leaves every bounded subset of the [complex upper half-plane](complex-analysis.md#upper-half-plane-complex-analysis). For $0<\kappa<4$, its time-one [compact H-hull](#compact-h-hull) is a simple slit and does not contain a half-disc. Instead, the [boundary approach forces a small SLE Bessel gap](#boundary-approach-forces-a-small-sle-bessel-gap) estimate shows that every fixed nonzero real point is outside the closure of the full [Loewner trace](#trace-of-a-loewner-chain). After mapping out the initial simple slit, the starting point has two distinct real [prime end](geometry-and-topology.md#prime-end) images. A fresh independent [SLE](#schramm-loewner-evolution) avoids approaching either image, so the original future stays a positive distance from its starting point. [Scaling invariance of SLE](#scaling-invariance-of-sle) gives $\inf_{t\geq T}|\gamma(t)|\overset d=\sqrt T\inf_{t\geq1}|\gamma(t)|$, and decreasing-event continuity proves escape from every fixed disc. The separate argument based on a swallowed half-disc at positive time applies in the nonsimple regime $\kappa>4$; it must not be applied to a simple slit. The critical parameters require their own limiting or trace-existence arguments.

### Reverse Loewner flow

↑ **Parent:** [Schramm–Loewner evolution](#schramm-loewner-evolution)

For a continuous driver $U$ and terminal time $T$, the reverse Loewner flow solves

$$
\partial_sh_s(z)=-\frac2{h_s(z)-(U_{T-s}-U_T)},
\qquad h_0(z)=z.
$$

It satisfies $h_T(z)=g_T^{-1}(U_T+z)-U_T$.

#### Reverse SLE derivative martingale

↑ **Parent:** [Reverse Loewner flow](#reverse-loewner-flow)

For the reverse $\operatorname{SLE}_\kappa$ flow, write $X_s+iY_s=h_s(z)-(U_{T-s}-U_T)$. Then

$$
M_s=|h_s'(z)|^2\left(1+\frac{X_s^2}{Y_s^2}\right)^{4/\kappa}
$$

is a nonnegative [local martingale](martingale.md#local-martingale) and hence a [supermartingale](martingale.md#supermartingale).

##### Reverse SLE derivative bound above the space-filling threshold

↑ **Parent:** [Reverse SLE derivative martingale](#reverse-sle-derivative-martingale)

If $\kappa>8$, then for every $0<\alpha<(1-8/\kappa)/2$ and fixed $T$, there is an almost surely finite random $C$ such that

$$
|h_T'(x+iy)|\leq Cy^{-1+\alpha}
$$

for $|x|\leq1$ and $0<y\leq1$. The proof combines the derivative martingale, [Markov inequality](probability-inequality.md#markov-inequality), a dyadic lattice, the [Borel-Cantelli lemmas](probability-theory.md#borel-cantelli-lemmas), and the [Koebe distortion theorem](complex-analysis.md#koebe-distortion-theorem).

### Boundary-point Bessel flow for SLE

↑ **Parent:** [Schramm–Loewner evolution](#schramm-loewner-evolution)

For chordal $\operatorname{SLE}_\kappa$, the centered image of a real boundary point, divided by $\sqrt\kappa$, evolves as a [Bessel process](brownian-motion.md#bessel-process) of dimension

$$
d=1+\frac4\kappa.
$$

Its first hit of zero is the time at which the point is swallowed by the Loewner hull.

#### Boundary approach forces a small SLE Bessel gap

↑ **Parent:** [Boundary-point Bessel flow for SLE](#boundary-point-bessel-flow-for-sle)

For $0<\kappa<4$ and $x>0$, stop the simple chordal [SLE](#schramm-loewner-evolution) trace on first entering the radius-$r$ half-disc about $x$, with $r<x/4$. A crosscut from its tip to $x$ separates the positive-side boundary arc containing $x/2$ from infinity. [Harmonic measure](brownian-motion.md#harmonic-measure) comparison with the half-disc bounds the length of that arc's mapped interval, $g_t(x/2)-\xi_t$, by a universal constant times $r$. This centered boundary image is a positive [Bessel process](brownian-motion.md#bessel-process) of dimension $1+4/\kappa>2$ and has a strictly positive all-time minimum. Hence the full trace stays a positive distance from each fixed nonzero real point. Reflection gives the negative-side version.

#### SLE two-boundary-point ratio diffusion

↑ **Parent:** [Boundary-point Bessel flow for SLE](#boundary-point-bessel-flow-for-sle)

For $0<x<y$, let $D_t=g_t(y)-g_t(x)$. Before the first [boundary-point swallowing time for a Loewner chain](#boundary-point-swallowing-time-for-a-loewner-chain), the ratio obeys

$$
dZ_t=-\frac{\sqrt\kappa}{D_t}d\beta_t+\frac2{D_t^2}\left(\frac1{Z_t}+\frac1{Z_t-1}\right)dt.
$$

The clock $u=\int D_t^{-2}dt$ removes the denominator. An increasing [scale function of a one-dimensional diffusion](stochastic-calculus.md#scale-function-stochastic-processes) is $s_\kappa(z)=\int_1^z[v(v-1)]^{-4/\kappa}dv$. For $\kappa>4$ the endpoint $1$ represents strict swallowing; escape at infinite clock represents simultaneous swallowing.

##### Strict ordering threshold for SLE boundary swallowing

↑ **Parent:** [SLE two-boundary-point ratio diffusion](#sle-two-boundary-point-ratio-diffusion)

For $\kappa\geq8$, almost surely the positive-boundary swallowing times satisfy $T(x)<T(y)$ simultaneously for every $0<x<y$. The [SLE two-boundary-point ratio diffusion](#sle-two-boundary-point-ratio-diffusion) has unbounded scale, ruling out escape before hitting $1$. For $4<\kappa<8$, its total scale $S_\kappa$ is finite, and the simultaneous-swallowing probability is $s_\kappa(y/(y-x))/S_\kappa$. At $\kappa=4$, fixed positive points have infinite swallowing times.

###### Real-line visitation from strict SLE swallowing order

↑ **Parent:** [Strict ordering threshold for SLE boundary swallowing](#strict-ordering-threshold-for-sle-boundary-swallowing)

A continuous capacity-parameterized [Loewner trace](#trace-of-a-loewner-chain) with finite, strictly ordered positive swallowing times visits every positive real point. An unvisited swallowed point has an interval disjoint from the compact trace up to its swallowing time; that interval is swallowed simultaneously, contradicting strict order. Reflection yields the negative-axis conclusion for chordal [SLE](#schramm-loewner-evolution) at $\kappa\geq8$.

#### SLE boundary-point logarithmic separation diffusion

↑ **Parent:** [Boundary-point Bessel flow for SLE](#boundary-point-bessel-flow-for-sle)

For two boundary points $1<r$, let $V_t^x=g_t(x)-U_t$ and set $Z_t=\log(V_t^r-V_t^1)-\log V_t^1$. After the clock $q(u)=\int_0^u(V_s^1)^{-2}ds$, the [Dambis-Dubins-Schwarz theorem](martingale.md#dambis-dubins-schwarz-theorem) gives

$$
d\widetilde Z_t=\sqrt\kappa\,dW_t+\left(\frac{\kappa-4}{2}-\frac2{1+e^{\widetilde Z_t}}\right)dt.
$$

This one-dimensional [diffusion process](stochastic-calculus.md#markov-diffusion) compares the swallowing times of nearby boundary points.

##### SLE does not hit a fixed nonzero boundary point

↑ **Parent:** [SLE boundary-point logarithmic separation diffusion](#sle-boundary-point-logarithmic-separation-diffusion)

For every $x\in\mathbb R\setminus\{0\}$, the probability that a chordal $\operatorname{SLE}_\kappa$ trace in $(\mathbb H,0,\infty)$ passes through $x$ is zero. The [SLE boundary-point logarithmic separation diffusion](#sle-boundary-point-logarithmic-separation-diffusion) shows that the chance for $x$ to be swallowed strictly before a nearby point tends to zero as that point approaches $x$; [Scaling invariance of SLE](#scaling-invariance-of-sle) and reflection then handle every nonzero $x$.

#### Two-sided SLE boundary swallowing probability

↑ **Parent:** [Boundary-point Bessel flow for SLE](#boundary-point-bessel-flow-for-sle)

For $1<d<2$, couple Bessel flows $X>0>Y$ with the same Brownian motion and let $v=x/y<0$. Then

$$
\mathbb P(\tau_x>\tau_y)=\frac{\displaystyle\int_v^0\frac{du}{(-u)^{d-1}(1-u)^{4-2d}}}{\displaystyle\int_{-\infty}^0\frac{du}{(-u)^{d-1}(1-u)^{4-2d}}}.
$$

It is the probability that the SLE hull swallows the chosen point on the negative side before the point on the positive side.

## Infinitesimal generator (stochastic processes)

↑ **Parent:** [Stochastic process](stochastic-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Infinitesimal_generator_(stochastic_processes))

For a Markov process with transition semigroup $(P_t)$, its infinitesimal generator is the operator

$$
Lf=\lim_{t\downarrow0}\frac{P_tf-f}{t}
$$

on the functions for which this limit exists.

<h3 id="dynkin-s-formula">Dynkin's formula</h3>

↑ **Parent:** [Infinitesimal generator (stochastic processes)](#infinitesimal-generator-stochastic-processes)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dynkin's_formula)

For a [Markov process](markov-process.md) with [infinitesimal generator](#infinitesimal-generator-stochastic-processes) $L$ and a suitable test function $f$, the displayed process is a [local martingale](martingale.md#local-martingale). With integrability it is a true [martingale](martingale.md) and yields the corresponding expectation identity at admissible stopping times. For bounded $f,Lf$ in the semigroup generator domain, $P_tf-f=\int_0^tP_sLf\,ds$. The [Markov property](markov-process.md#markov-property) applies this identity conditionally over each interval, proving the martingale increments have zero conditional expectation. Localization gives the local version. For a continuous diffusion, these identities are the [martingale problem](stochastic-calculus.md#martingale-problem) for $L$.

### Diffusion generator

↑ **Parent:** [Infinitesimal generator (stochastic processes)](#infinitesimal-generator-stochastic-processes)

For the one-dimensional Itô equation $dX=b(X)dt+\sigma(X)dW$, the infinitesimal generator on smooth test functions is $L=b\partial_x+\sigma^2\partial_{xx}/2$. The [Kolmogorov backward equation](stochastic-calculus.md#kolmogorov-backward-equation) is $u_t=Lu$, while its formal adjoint produces the [Fokker-Planck equation](probability-theory.md#fokker-planck-equation).

#### Dynkin formula for a diffusion

↑ **Parent:** [Diffusion generator](#diffusion-generator)

For a [diffusion process](stochastic-calculus.md#markov-diffusion) with [diffusion generator](#diffusion-generator) $L$, the [Itô formula](stochastic-calculus.md#ito-s-lemma) makes $\varphi(X_t)-\varphi(X_0)-\int_0^tL\varphi(X_s)ds$ a local martingale. Under stopping and integrability conditions making it a true martingale, taking expectations gives the displayed identity. For [Brownian motion](brownian-motion.md), $L=\tfrac12\Delta$, recovering the usual Brownian formula.

## Filtration (probability theory)

↑ **Parent:** [Stochastic process](stochastic-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Filtration_(probability_theory))

A filtration is an increasing family of sigma-algebras: $\mathcal F_s\subseteq\mathcal F_t$ whenever $s\leq t$. It represents the information available as time passes.

### Dyadic filtration

↑ **Parent:** [Filtration (probability theory)](#filtration-probability-theory)

On $(0,1]^d$, the dyadic [filtration](#filtration-probability-theory) is generated by the partitions into half-open cubes of side $2^{-n}$. The [conditional expectation](measure-theory.md#conditional-expectation) of an integrable function is its average on each atom. The increasing partitions generate the Borel sigma-algebra. Step functions on these partitions are dense in $L^1$; approximation and the [Doob maximal inequality](martingale.md#doob-maximal-inequality-for-a-nonnegative-submartingale) show that their conditional averages converge in $L^1$ and [almost everywhere](measure-theory.md#almost-everywhere) to the original function.

### Filtered probability space

↑ **Parent:** [Filtration (probability theory)](#filtration-probability-theory)

A filtered probability space is a [probability space](probability-theory.md#probability-space) together with an increasing family of [sigma-algebras](measure-theory.md#sigma-algebra) $\mathcal F_t\subseteq\mathcal F$ describing the information available by time $t$.

#### Usual conditions for a filtration

↑ **Parent:** [Filtered probability space](#filtered-probability-space)

The usual conditions are completeness and right continuity of a [filtration](#filtration-probability-theory): $\mathcal F_0$ contains all subsets of null events in the ambient [probability space](probability-theory.md#probability-space), and $\mathcal F_t=\bigcap_{s>t}\mathcal F_s$. They allow the standard continuous-time [martingale](martingale.md), [stopping time](martingale.md#stopping-time) and stochastic integration theorems to be used without repeated augmentation qualifications. An [absolute continuity of measures](measure-theory.md#absolute-continuity-of-measures) change preserves old null sets but can introduce new ones; the usual completion under the new measure may therefore be understood when needed.

### Left-limit sigma-algebra

↑ **Parent:** [Filtration (probability theory)](#filtration-probability-theory)

For a [filtration](#filtration-probability-theory) $(\mathcal F_t)$, the information strictly before time $t$ is

$$
\mathcal F_{t-}=\sigma\!\left(\bigcup_{s<t}\mathcal F_s\right).
$$

A [predictable process](martingale.md#predictable-process) evaluated at a deterministic positive time $t$ is $\mathcal F_{t-}$-measurable.

## Natural filtration

↑ **Parent:** [Stochastic process](stochastic-process.md)

The natural filtration of a stochastic process $X$ records its history:

$$
\mathcal F_t^X=\sigma(X_s:0\leq s\leq t),
$$

possibly completed and made right-continuous when the usual conditions are required.

## Adapted process

↑ **Parent:** [Stochastic process](stochastic-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Adapted_process)

A stochastic process $X$ is adapted to a [filtration](#filtration-probability-theory) $(\mathcal F_t)$ when $X_t$ is $\mathcal F_t$-measurable at every time $t$. Its present value therefore depends only on information already available.

### Adaptedness of a stopped right-continuous process

↑ **Parent:** [Adapted process](#adapted-process)

For an [adapted process](#adapted-process) with right-continuous paths and a [stopping time](martingale.md#stopping-time) $T$, $X^T_t=X_{t\wedge T}$ is [adapted](#adapted-process). At fixed $t$, round $t\wedge T$ upward on finite partitions of $[0,t]$. Every approximating value is $\mathcal F_t$-[measurable](measure-theory.md#measurability), and right continuity gives the limit. Completeness handles a null exceptional set if right continuity holds only [almost surely](convergence-of-random-variables.md#almost-sure-convergence). A [martingale](martingale.md) assumption and boundedness of $T$ are unnecessary.

### Progressive measurability

↑ **Parent:** [Adapted process](#adapted-process)

A process $H$ is progressively measurable when, for every $T$, its restriction to $[0,T]\times\Omega$ is measurable for $\mathcal B([0,T])\otimes\mathcal F_T$. Continuous [adapted processes](#adapted-process) are progressively measurable, and a Borel function of such a process remains so. A progressively measurable square-integrable Brownian integrand has an equivalent predictable integrand for the [Itô integral](stochastic-calculus.md#ito-integral), up to equality for $dt\,d\mathbb P$.

#### Almost sure path regularity does not ensure progressive measurability

↑ **Parent:** [Progressive measurability](#progressive-measurability)

Let a probability space have two sample points, one of probability zero and one of probability one, and give it the complete power-set sigma-algebra at every time. Let $A\subseteq[0,1]$ be non-Borel. Assign the [stochastic process](stochastic-process.md) the path $\mathbf1_A(t)$ at the null sample point and the zero path at the other point. Each fixed-time variable is measurable and the paths are [càdlàg](calculus.md#cadlag) [almost surely](convergence-of-random-variables.md#almost-sure-convergence), but the [stochastic process](stochastic-process.md) is not [progressively measurable](#progressive-measurability): a section in the time variable of a product-measurable function must be Borel measurable at every sample point. The zero [stochastic process](stochastic-process.md) is an [indistinguishable](#indistinguishability-of-stochastic-processes) [progressively measurable](#progressive-measurability) version. Completing the filtration does not complete the time-product sigma-algebra or remove this distinction.

#### Right-continuous adapted processes are progressively measurable

↑ **Parent:** [Progressive measurability](#progressive-measurability)

For an [adapted process](#adapted-process) with pathwise [right continuity](calculus.md#right-continuous-function), fix $T$ and approximate its time argument by the next endpoint of a deterministic partition of $[0,T]$. Every approximation is jointly measurable for the terminal [product sigma-algebra](probability-theory.md#product-sigma-algebra) because all sampled values are $\mathcal F_T$-measurable. [Right continuity](calculus.md#right-continuous-function) makes them converge pointwise, proving [progressive measurability](#progressive-measurability). Sampling from the right need not preserve adaptedness at intermediate times, but that is not required in this proof.

## Uniform convergence on compacts in probability

↑ **Parent:** [Stochastic process](stochastic-process.md)

Processes $X_n$ converge uniformly on compacts in probability to $X$ when, for every $T<\infty$ and $\varepsilon>0$,

$$
\mathbb P\!\left(\sup_{t\leq T}|X_n(t)-X(t)|>\varepsilon\right)\to0.
$$

### Uniform convergence on compacts in probability under an absolutely continuous measure change

↑ **Parent:** [Uniform convergence on compacts in probability](#uniform-convergence-on-compacts-in-probability)

If $Q\ll P$, [uniform convergence on compacts in probability](#uniform-convergence-on-compacts-in-probability) under $P$ implies the same convergence under $Q$. Indeed, let $Z=dQ/dP$ be the [Radon-Nikodym derivative](measure-theory.md#radon-nikodym-derivative). For every event $E$,

$$
Q(E)\leq K P(E)+\mathbb E_P[Z\mathbf1_{\{Z>K\}}].
$$

Integrability makes the second term arbitrarily small for large $K$. Thus $P(E_n)\to0$ implies $Q(E_n)\to0$; apply this to each event where the supremum on $[0,T]$ exceeds a fixed tolerance. Only [absolute continuity of measures](measure-theory.md#absolute-continuity-of-measures) is needed, not equivalence.

<h2 id="cadlag-process">Càdlàg process</h2>

↑ **Parent:** [Stochastic process](stochastic-process.md)

A càdlàg process has sample paths that are [càdlàg functions](calculus.md#cadlag): they are right-continuous and have a finite left limit at every positive time.

## Time change of a continuous process

↑ **Parent:** [Stochastic process](stochastic-process.md)

If $X$ has continuous paths and $\tau_s$ is a finite continuous increasing family of random times, then $X_{\tau_s}$ also has continuous paths. A strictly increasing continuous clock that tends to infinity has a continuous inverse.

### Optional time-change theorem

↑ **Parent:** [Time change of a continuous process](#time-change-of-a-continuous-process)

Let $M$ be a [continuous local martingale](martingale.md#continuous-local-martingale) and let $(\tau_s)$ be an increasing continuous family of finite [stopping times](martingale.md#stopping-time). Under the usual compatibility conditions, $M_{\tau_s}$ is a continuous local martingale for the time-changed filtration $\mathcal F_{\tau_s}$. A finite-variation process remains of finite variation after the same time change.

## Indistinguishability of stochastic processes

↑ **Parent:** [Stochastic process](stochastic-process.md)

Two stochastic processes $X,Y$ are indistinguishable when

$$
\mathbb P(X_t=Y_t\text{ for every }t)=1.
$$

This is stronger than equality almost surely at each fixed time, though the two notions agree for continuous processes after checking equality on a countable dense set.

<h3 id="cadlag-versions-are-indistinguishable">Càdlàg versions are indistinguishable</h3>

↑ **Parent:** [Indistinguishability of stochastic processes](#indistinguishability-of-stochastic-processes)

If two [versions of a stochastic process](#modification-of-a-stochastic-process) both have [càdlàg](calculus.md#cadlag) paths on an event of probability one, equality at every rational time holds simultaneously outside one null event. Approaching an arbitrary time by rationals from the right then gives equality at every time on the same event. Thus the [stochastic processes](stochastic-process.md) are [indistinguishable](#indistinguishability-of-stochastic-processes). [Right continuity](calculus.md#right-continuous-function) suffices; left limits are unnecessary for this conclusion.

## Stochastic calculus

↑ **Parent:** [Stochastic process](stochastic-process.md)

[This section is present in another page, follow this link to view it.](stochastic-calculus.md)

## Stochastic continuity

↑ **Parent:** [Stochastic process](stochastic-process.md)

A stochastic process $X$ is stochastically continuous when $X_s\to X_t$ in probability as $s\to t$.

<h2 id="levy-process">Lévy process</h2>

↑ **Parent:** [Stochastic process](stochastic-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lévy_process)

A Lévy process starts at zero, has independent stationary increments, is stochastically continuous, and is conventionally taken to have càdlàg paths.

<h3 id="continuous-levy-process">Continuous Lévy process</h3>

↑ **Parent:** [Lévy process](#levy-process)

A real [Lévy process](#levy-process) with continuous paths is [Brownian motion](brownian-motion.md) with deterministic linear drift: $X_t=bt+\sigma W_t$. Continuity forces the jump measure in the [Lévy–Khintchine formula](#levy-khintchine-formula) to vanish, leaving characteristic function $\exp(t(ibu-\sigma^2u^2/2))$. If its law is also invariant under $X_t\mapsto\lambda^{-1}X_{\lambda^2t}$ for every $\lambda>0$, then $b=0$. The zero-variance case is included.

### Atomic compound Poisson process with drift

↑ **Parent:** [Lévy process](#levy-process)

With finitely many nonzero marks $z_j$ and independent [Poisson processes](probability-theory.md#poisson-process) $N^j$ of rates $\lambda_j$, the displayed process is a [Lévy process](#levy-process) with no Gaussian component. Its [Lévy measure](#levy-measure) is $\sum_j\lambda_j\delta_{z_j}$, its mean is $t(\gamma+\sum_j\lambda_jz_j)$, and its [variance](variance.md) is $t\sum_j\lambda_jz_j^2$. Its paths have finitely many jumps on every bounded interval and deterministic slope $\gamma$ between jumps. Coincident mark sizes combine their rates; zero marks have no effect. The drift here uses the uncompensated finite-sum convention, which differs from the drift parameter in a compensated [Lévy–Khintchine formula](#levy-khintchine-formula).

<h3 id="closure-of-levy-processes-under-locally-controlled-convergence-in-probability">Closure of Lévy processes under locally controlled convergence in probability</h3>

↑ **Parent:** [Lévy process](#levy-process)

Suppose [Lévy processes](#levy-process) $X^n$ converge to $X$ in probability at every fixed time, and

$$
\lim_{n\to\infty}\limsup_{t\downarrow0}\mathbb P(|X_t^n-X_t|>\varepsilon)=0\qquad(\varepsilon>0).
$$

Then $X$ starts at zero, has [independent increments](#independent-increments) and [stationary increments](#stationary-increments), and has [stochastic continuity](#stochastic-continuity). Finite increment vectors inherit their independent laws by [convergence in distribution](convergence-of-random-variables.md#convergence-in-distribution); the near-zero estimate supplies continuity at zero. Hence $X$ has a [càdlàg modification](#cadlag-modification) that is a [Lévy process](#levy-process). The hypotheses alone cannot assert that the original version has [càdlàg](calculus.md#cadlag) paths.

### Cauchy process

↑ **Parent:** [Lévy process](#levy-process)

The standard symmetric [Cauchy process](#cauchy-process) is the [Lévy process](#levy-process) with [Lévy characteristic exponent](#characteristic-exponent-of-a-levy-process) $\Psi(u)=|u|$. Its time-$t$ distribution for $t>0$ is the [Cauchy distribution](probability-theory.md#cauchy-distribution) of location zero and scale $t$. It can be constructed by [subordination of a Lévy process](#subordination-of-a-levy-process): evaluate an independent standard [Brownian motion](brownian-motion.md) at the [Brownian first-passage subordinator](#brownian-first-passage-subordinator), whose Laplace exponent is $\sqrt{2\lambda}$.

#### Self-similarity of a Cauchy process

↑ **Parent:** [Cauchy process](#cauchy-process)

For a standard [Cauchy process](#cauchy-process), the increment [characteristic function](probability-theory.md#characteristic-function) is $\exp[-(t-s)|u|]$. Scaling space by $\alpha^{-1}$ and time by $\alpha$ leaves this expression unchanged and preserves [independent increments](#independent-increments), proving equality of all [finite-dimensional distributions](#finite-dimensional-distribution). Equivalently, $\alpha X_{t/\alpha}$ has the original process law. Scaling both space and time by $\alpha$ instead changes the exponent by $\alpha^2$ and is not an invariance unless $\alpha=1$.

<h3 id="characteristic-exponent-of-a-levy-process">Characteristic exponent of a Lévy process</h3>

↑ **Parent:** [Lévy process](#levy-process)

Use the convention

$$
\mathbb E e^{iuX_t}=e^{-t\Psi(u)}.
$$

Then $\Psi$ is the characteristic exponent of the [Lévy process](#levy-process). Some authors instead write $e^{t\psi(u)}$, with $\psi=-\Psi$. The sign convention should always be specified. The [Lévy–Khintchine formula](#levy-khintchine-formula) describes all possible exponents.

<h4 id="exponential-martingale-of-a-levy-process">Exponential martingale of a Lévy process</h4>

↑ **Parent:** [Characteristic exponent of a Lévy process](#characteristic-exponent-of-a-levy-process)

With the convention $\mathbb E e^{iuX_t}=e^{t\psi(u)}$, this complex process is a [martingale](martingale.md) for each real $u$. Its absolute value is the deterministic finite number $e^{-t\operatorname{Re}\psi(u)}$. Conditioning on the past at time $s$ and using [independent increments](#independent-increments) multiplies $e^{iuX_s-t\psi(u)}$ by $e^{(t-s)\psi(u)}$, giving $M_s^u$. Under the opposite exponent convention the sign of the compensating term reverses.

<h4 id="exponential-form-of-levy-characteristic-functions">Exponential form of Lévy characteristic functions</h4>

↑ **Parent:** [Characteristic exponent of a Lévy process](#characteristic-exponent-of-a-levy-process)

[Independent increments](#independent-increments) and [stationary increments](#stationary-increments) make a [Lévy process](#levy-process)'s [characteristic functions](probability-theory.md#characteristic-function) multiplicative in time. Together with [continuity of Lévy characteristic functions](#continuity-of-levy-characteristic-functions) and the value one at time zero, this forces an exponential. A continuous local [complex logarithm](analysis.md#complex-logarithm) is additive: its failure of additivity would be a continuous integer multiple of $2\pi i$, hence zero. The [Cauchy functional equation](analysis.md#cauchy-s-functional-equation) and subdivision then give the exponential at every time. This construction of the [characteristic exponent of a Lévy process](#characteristic-exponent-of-a-levy-process) precedes the [Lévy–Khintchine formula](#levy-khintchine-formula) describing the exponent's possible form.

<h4 id="continuity-of-levy-characteristic-functions">Continuity of Lévy characteristic functions</h4>

↑ **Parent:** [Characteristic exponent of a Lévy process](#characteristic-exponent-of-a-levy-process)

For a [Lévy process](#levy-process), [stochastic continuity](#stochastic-continuity) gives continuity of its [characteristic function](probability-theory.md#characteristic-function) in time at every fixed frequency. The elementary estimate $|\varphi_{X_s}(u)-\varphi_{X_t}(u)|\leq |u|\delta+2\mathbb P(|X_s-X_t|>\delta)$ proves this by first taking $s\to t$ and then $\delta\downarrow0$. The argument works for any stochastically continuous [stochastic process](stochastic-process.md) and needs no finite-moment assumption.

<h3 id="subordination-of-a-levy-process">Subordination of a Lévy process</h3>

↑ **Parent:** [Lévy process](#levy-process)

If $X$ is a [Lévy process](#levy-process) and $T$ an independent [subordinator](#subordinator), then $Y_t=X_{T_t}$ is a [Lévy process](#levy-process). Conditional on the clock, increments of $X$ over disjoint clock intervals are independent; averaging over the independent [stationary increments](#stationary-increments) of the clock gives the same properties for $Y$. If $\mathbb Ee^{iuX_s}=e^{-s\Psi(u)}$, its [characteristic function](probability-theory.md#characteristic-function) is $\mathbb E e^{-T_t\Psi(u)}$. For standard [Brownian motion](brownian-motion.md), $\Psi(u)=u^2/2$, so this is the clock's [Laplace transform](analysis.md#laplace-transform) at $u^2/2$.

### Subordinator

↑ **Parent:** [Lévy process](#levy-process)

A subordinator is a [Lévy process](#levy-process) with nondecreasing paths. Its nonnegative [stationary increments](#stationary-increments) have a [Laplace transform](analysis.md#laplace-transform) of the form

$$
\mathbb E e^{-\lambda T_t}=e^{-t\Phi(\lambda)},\qquad\lambda\geq0,
$$

where $\Phi$ is called its Laplace exponent. Its standard path convention is [càdlàg](calculus.md#cadlag). Subordinators provide random clocks for [subordination of a Lévy process](#subordination-of-a-levy-process).

#### Brownian first-passage subordinator

↑ **Parent:** [Subordinator](#subordinator)

For standard [Brownian motion](brownian-motion.md) started at zero, the strict first-passage times form a [subordinator](#subordinator) in the level parameter $a$. The [Strong Markov property](markov-process.md#strong-markov-property) gives [independent increments](#independent-increments) and [stationary increments](#stationary-increments); the strict inverse of the continuous running maximum has [càdlàg](calculus.md#cadlag) paths. The [Brownian first-passage Laplace transform](markov-process.md#brownian-first-passage-laplace-transform) gives Laplace exponent $\Phi(\lambda)=\sqrt{2\lambda}$, so the process is strictly stable of index $1/2$. Choosing the non-strict hitting times preserves each fixed-level law but generally loses right continuity at random levels, as in the [fixed-level versus simultaneous Brownian passage-time equality](markov-process.md#fixed-level-versus-simultaneous-brownian-passage-time-equality).

##### Countable dense jumps of the Brownian first-passage subordinator

↑ **Parent:** [Brownian first-passage subordinator](#brownian-first-passage-subordinator)

The [Brownian first-passage subordinator](#brownian-first-passage-subordinator) has a countable dense set of jump levels almost surely, and is continuous at every other level. Its paths are finite [nondecreasing functions](calculus.md#nondecreasing-function), so on a bounded level interval there can be only finitely many jumps larger than any fixed positive size; a countable union proves countability. For density, suppose its path were continuous throughout an open level interval. It is strictly increasing, since the original continuous Brownian path takes different values at different passage times. Its continuous inverse on that interval would parametrize a positive-length time interval on which the Brownian path increases monotonically. This contradicts [nowhere monotonicity of Brownian motion](brownian-motion.md#nowhere-monotonicity-of-brownian-motion). Thus every level interval contains a jump. In particular dense discontinuities do not mean that the path is nowhere continuous: it is continuous at every level outside a countable random set.

<h3 id="levy-measure">Lévy measure</h3>

↑ **Parent:** [Lévy process](#levy-process)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lévy_measure)

The Lévy measure $\nu$ of a [Lévy process](#levy-process) records the intensity of its jumps: for every measurable set $A$ bounded away from zero, $\nu(A)$ is the expected number per unit time of jumps whose sizes lie in $A$. It satisfies

$$
\nu(\{0\})=0,
\qquad
\int_{\mathbb R^d}(1\wedge |x|^2)\,\nu(dx)<\infty.
$$

<h4 id="levy-measure-of-a-symmetric-laplace-time-one-law">Lévy measure of a symmetric Laplace time-one law</h4>

↑ **Parent:** [Lévy measure](#levy-measure)

For $\alpha>0$, the [Lévy process](#levy-process) with [characteristic function](probability-theory.md#characteristic-function) $\mathbb E e^{iuX_t}=(1+u^2/\alpha^2)^{-t}$ has zero Gaussian coefficient, zero uncompensated drift, and the displayed [Lévy measure](#levy-measure). Indeed, the symmetric jump integral is $2\int_0^\infty(\cos(uy)-1)e^{-\alpha y}dy/y$. Differentiating in $u$ gives $-2u/(\alpha^2+u^2)$, and integrating back from zero gives $-\log(1+u^2/\alpha^2)$. The time-one law is the [Laplace distribution](continuous-probability-distribution.md#laplace-distribution) of rate $\alpha$. The jump activity is infinite, since $K$ has infinite mass near zero, but the jump variation is finite because $\int(1\wedge|y|)K(dy)<\infty$.

### Compound Poisson process

↑ **Parent:** [Lévy process](#levy-process)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Compound_Poisson_process)

A compound Poisson process has the form

$$
X_t=\sum_{n=1}^{N_t}Y_n,
$$

where $N$ is a [Poisson process](probability-theory.md#poisson-process) and the independent identically distributed marks $Y_n$ are independent of $N$. It is a [Lévy process](#levy-process) with a finite Lévy measure.

#### Independent compound Poisson jumps cannot cancel

↑ **Parent:** [Compound Poisson process](#compound-poisson-process)

Let $Y$ be a [Compound Poisson process](#compound-poisson-process) with nonzero jump marks and positive rate, [independent](random-variable.md#independent-random-variables) of a [càdlàg](calculus.md#cadlag) process $Z$. Conditional on the path of $Z$, its discontinuities form a [countable set](set-theory.md#countable-set). The Poisson jump times have continuous distributions and avoid that set almost surely. At every jump of $Y$, the sum $Y+Z$ therefore has the same nonzero jump. In particular a [continuous Lévy process](#continuous-levy-process) cannot have a positive-rate [independent](random-variable.md#independent-random-variables) compound Poisson component. Applying this to each truncation of its [Lévy measure](#levy-measure) proves that its jump measure is zero.

#### Grid-sampled compound Poisson workload bound

↑ **Parent:** [Compound Poisson process](#compound-poisson-process)

For nondecreasing compound Poisson input U, let $W=\sup_{t\geq0}(U(t)-Ct)$ and $W_\delta=\sup_{k\geq0}(U(k\delta)-Ck\delta)$. The second [supremum](real-analysis.md#supremum) is bounded above by the first. For each t, the next grid point is at most delta later, its input is at least U(t), and it offers at most an extra $C\delta$ service. Hence $W\leq W_\delta+C\delta$. This supplies explicit stationary-tail brackets and shows that time discretization preserves the workload's exponential tail rate.

#### Exponential Laplace martingale of a compound Poisson process

↑ **Parent:** [Compound Poisson process](#compound-poisson-process)

Let $Y_t=\sum_{j=1}^{N_t}X_j$ for a rate-$\lambda$ [Poisson process](probability-theory.md#poisson-process) and [independent and identically distributed](random-variable.md#independent-and-identically-distributed-random-variables) nonnegative marks independent of that process, with $\phi(q)=\mathbb E e^{-qX_1}$. The [Laplace transform of a nonnegative random variable](probability-theory.md#laplace-transform-of-a-nonnegative-random-variable) for the increment over $[s,t]$ is $\exp[\lambda(t-s)(\phi(q)-1)]$. That increment is independent of the past of $Y$, so the displayed nonnegative process has mean one and satisfies $\mathbb E[Z_t\mid\sigma(Y_u:u\leq s)]=Z_s$. No finite first moment of the marks is needed for this [martingale](martingale.md) when $q\geq0$.

#### Difference of independent Poisson processes

↑ **Parent:** [Compound Poisson process](#compound-poisson-process)

For independent [Poisson processes](probability-theory.md#poisson-process) with rates $r_+,r_-\geq0$, their difference is a [Lévy process](#levy-process) with [characteristic function](probability-theory.md#characteristic-function) $\exp(t[r_+(e^{iu}-1)+r_-(e^{-iu}-1)])$. When the combined rate is positive, its jumps occur at rate $r_++r_-$, with direction probabilities proportional to the two rates. Equal unit rates give $\exp(2t(\cos u-1))$ and a rate-two [Compound Poisson process](#compound-poisson-process) with [Rademacher distribution](probability-theory.md#rademacher-distribution) jumps. Its paths are integer-valued, [càdlàg](calculus.md#cadlag), and of [finite variation](real-analysis.md#total-variation-of-a-function) on compact intervals.

#### Continuous-time symmetric simple random walk

↑ **Parent:** [Compound Poisson process](#compound-poisson-process)

At unit jump rate, this is $X_t=\sum_{k=1}^{N_t}\xi_k$, where $N$ is a rate-one [Poisson process](probability-theory.md#poisson-process) and the independent marks are uniform signs. Equivalently it is the difference of two independent rate-$1/2$ Poisson processes. It is a [Lévy process](#levy-process) with characteristic function $\exp\{t(\cos\theta-1)\}$, mean zero, [variance](variance.md) $t$, and [Lévy characteristic exponent](#characteristic-exponent-of-a-levy-process) $1-\cos\theta$ in the negative-exponent convention. A general total jump rate rescales time.

##### Scaling classification of a continuous-time symmetric simple random walk

↑ **Parent:** [Continuous-time symmetric simple random walk](#continuous-time-symmetric-simple-random-walk)

For the unit-rate [continuous-time symmetric simple random walk](#continuous-time-symmetric-simple-random-walk), the processes $n^{-\alpha}X_{nt}$ have three finite-dimensional regimes. For $0<\alpha<1/2$ no probability limit is possible, because the one-time characteristic functions tend to zero off the origin and are discontinuous there. At $\alpha=1/2$ the limit is standard [Brownian motion](brownian-motion.md). For $\alpha>1/2$ it is the identically zero [Lévy process](#levy-process). This follows from $n(1-\cos(n^{-\alpha}\theta))\sim(\theta^2/2)n^{1-2\alpha}$ and independent increments. Thus a nonzero limit uniquely determines the exponent, whereas merely asking for a Lévy limit does not.

#### Martingale compound Poisson process

↑ **Parent:** [Compound Poisson process](#compound-poisson-process)

A compound Poisson process with rate $\lambda$ and mark $Y$ is a [martingale](martingale.md) exactly when $\mathbb E|Y|<\infty$ and $\mathbb E Y=0$.

#### Independent coordinates of a compound Poisson process

↑ **Parent:** [Compound Poisson process](#compound-poisson-process)

The coordinates of a vector-valued [Compound Poisson process](#compound-poisson-process) are independent exactly when its [Lévy measure](#levy-measure) is supported on the union of the coordinate axes. For marks $(g_1(U),g_2(U))$ with $U$ uniform on $[0,1]$ and continuous $g_i$, this is equivalent to

$$
g_1(y)g_2(y)=0
$$

for every $y\in[0,1]$.

<h3 id="levy-khintchine-formula">Lévy–Khintchine formula</h3>

↑ **Parent:** [Lévy process](#levy-process)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lévy–Khintchine_formula)

Every real Lévy process has a unique triplet $(a,b,K)$ with $b\geq0$ and $\int(1\wedge x^2)K(dx)<\infty$ such that

$$
\mathbb E e^{iuX_t}=\exp\left\{t\left(iua-\frac12bu^2+\int_{\mathbb R\setminus\{0\}}(e^{iux}-1-iux\mathbf1_{\{|x|\leq1\}})K(dx)\right)\right\}.
$$

<h4 id="uncompensated-levy-khintchine-formula">Uncompensated Lévy–Khintchine formula</h4>

↑ **Parent:** [Lévy–Khintchine formula](#levy-khintchine-formula)

If a [Lévy measure](#levy-measure) satisfies $\int_{|y|\le1}|y|K(dy)<\infty$, the jump integral in the [Lévy–Khintchine formula](#levy-khintchine-formula) can be written without compensation: $\mathbb E e^{iuX_t}=e^{t\psi(u)}$, with the displayed exponent. Its integral is absolutely convergent because $|e^{iuy}-1|\le|u||y|$ near zero and is at most $2$ elsewhere. If the compensated formula uses drift $\gamma$, the uncompensated drift is $b=\gamma-\int_{|y|\le1}yK(dy)$. The Gaussian coefficient is still $\sigma^2\ge0$.

<h4 id="levy-ito-decomposition">Lévy–Itô decomposition</h4>

↑ **Parent:** [Lévy–Khintchine formula](#levy-khintchine-formula)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lévy–Itô_decomposition)

Given a Brownian motion $B$ and an independent Poisson random measure $N$ with intensity $dt\,K(dx)$, a Lévy process with triplet $(a,b,K)$ is

$$
X_t=at+\sqrt b B_t
+\int_0^t\!\int_{|x|\leq1}x\,\widetilde N(ds,dx)
+\int_0^t\!\int_{|x|>1}x\,N(ds,dx).
$$

<h5 id="path-and-moment-criteria-from-a-levy-triplet">Path and moment criteria from a Lévy triplet</h5>

↑ **Parent:** [Lévy–Itô decomposition](#levy-ito-decomposition)

For the convention in the [Lévy–Khintchine formula](#levy-khintchine-formula), a Lévy process has almost surely differentiable paths exactly when $b=0$ and $K=0$, and continuous paths exactly when $K=0$. It is integrable exactly when $\int_{|x|>1}|x|K(dx)<\infty$, and it has a finite second moment exactly when $\int x^2K(dx)<\infty$.

<h3 id="centered-square-integrable-levy-martingale">Centered square-integrable Lévy martingale</h3>

↑ **Parent:** [Lévy process](#levy-process)

If a Lévy process has mean zero and $\operatorname{Var}(X_1)=\sigma^2<\infty$, then $\operatorname{Var}(X_t)=t\sigma^2$ and $X_t^2-t\sigma^2$ is a martingale.

## Gaussian process

↑ **Parent:** [Stochastic process](stochastic-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaussian_process)

A Gaussian process is a [stochastic process](stochastic-process.md) whose every finite vector of values has a [multivariate normal distribution](probability-and-statistics.md#multivariate-normal-distribution). Its law is determined by its mean and covariance functions.

### Gaussian exponential martingale with deterministic variance

↑ **Parent:** [Gaussian process](#gaussian-process)

Let $X_0=0$ and let $X$ be a centered [Gaussian process](#gaussian-process) whose increments are independent of the past [filtration](#filtration-probability-theory), with deterministic variance $v(t)$. Its displayed exponential is a positive [martingale](martingale.md). Indeed, $X_t-X_s$ is a centered [Gaussian random variable](probability-theory.md#gaussian-random-variable) with variance $v(t)-v(s)$, so the [Gaussian moment-generating function](probability-theory.md#moment-generating-function-of-a-normal-distribution) gives

$$
\mathbb E[M_t\mid\mathcal F_s]=M_s\mathbb E\exp(X_t-X_s-(v(t)-v(s))/2)=M_s.
$$

The sign-reversed process has the same variance and the same conclusion. Continuity of paths is unnecessary for this conditional-expectation argument.

### Covariance criterion for a stationary Gaussian Markov process

↑ **Parent:** [Gaussian process](#gaussian-process)

A centered continuous stationary scalar [Gaussian process](#gaussian-process) of positive variance can be [Markov](markov-process.md#markov-property) only if its covariance satisfies the displayed equation for $s,t\geq0$. Gaussian conditioning makes the future conditional mean $C(t)X_s/C(0)$; the [Markov property](markov-process.md#markov-property) then forces the equation by conditioning a future observation on the present and past. Conversely this equation makes the Gaussian residual future independent of the past, proving the [Markov property](markov-process.md#markov-property). In the nondegenerate decaying case the covariance is a single exponential. A sum $c_1e^{-a_1|t|}+c_2e^{-a_2|t|}$ with positive coefficients and distinct positive decay rates fails the equation and hence is not scalar Markov.

### Gaussian process construction from square-summable features

↑ **Parent:** [Gaussian process](#gaussian-process)

For independent standard normal variables $\xi_i$ and $\sum_i k_i(t)^2<\infty$ at each fixed time, the series defines $X_t$ in $L^2$. Every finite linear combination is an $L^2$ limit of Gaussian variables and is Gaussian. Thus this constructs a [Gaussian process](#gaussian-process) with the Gram [covariance kernel](random-variable.md#covariance-kernel) $K$. It supplies no sample-path continuity without additional assumptions.

### Canonical pseudometric of a Gaussian process

↑ **Parent:** [Gaussian process](#gaussian-process)

The canonical distance is the [L2 norm](real-analysis.md#l2-norm) of an increment of a [Gaussian process](#gaussian-process). It is a [pseudometric](topological-analysis.md#pseudometric), since distinct parameters may represent equal [random variables](random-variable.md) almost surely. Its [metric covering number](topological-analysis.md#metric-covering-number) appears in the [Dudley entropy integral](#dudley-entropy-integral). For standard [fractional Brownian motion](#fractional-brownian-motion), $d(s,t)=|s-t|^H$; a normalization with twice the [covariance function](#covariance-function) multiplies this distance by $\sqrt2$.

### Fractional Brownian motion

↑ **Parent:** [Gaussian process](#gaussian-process)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fractional_Brownian_motion)

A fractional Brownian motion with [Hurst exponent](#hurst-exponent) $H\in(0,1)$ is a centered [Gaussian process](#gaussian-process) with the displayed standard [covariance function](#covariance-function) and a [continuous modification](#continuous-modification). Its increment [variance](variance.md) is $|s-t|^{2H}$. Some sources omit the factor $1/2$, multiplying the process by $\sqrt2$; the corresponding increment [variance](variance.md) is then $2|s-t|^{2H}$. Its [canonical pseudometric of a Gaussian process](#canonical-pseudometric-of-a-gaussian-process) is proportional to $|s-t|^H$, which gives finite [expected value](probability-theory.md#expected-value) of its absolute [supremum](real-analysis.md#supremum) on compact intervals through the [Dudley entropy integral](#dudley-entropy-integral).

#### Hurst exponent

↑ **Parent:** [Fractional Brownian motion](#fractional-brownian-motion)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hurst_exponent)

For [fractional Brownian motion](#fractional-brownian-motion), $H\in(0,1)$ controls the [variance](variance.md) $|t-s|^{2H}$ of increments and the scaling of its [finite-dimensional distributions](#finite-dimensional-distribution). Larger $H$ means smaller increment [variance](variance.md) on intervals shorter than one and greater sample-path [Hölder continuity](sobolev-space.md#holder-condition).

### Sudakov-Fernique inequality

↑ **Parent:** [Gaussian process](#gaussian-process)

For centered [multivariate normal distributions](probability-and-statistics.md#multivariate-normal-distribution), if $\mathbb E(U_i-U_j)^2\leq\mathbb E(V_i-V_j)^2$ for every pair, then the displayed comparison holds. For a quick proof, make $U,V$ [independent](random-variable.md#independent-random-variables) and set $Z_r=\sqrt{1-r}U+\sqrt rV$. Apply [Gaussian integration by parts](probability-theory.md#stein-s-lemma-probability) to $F_\tau(z)=\tau^{-1}\log\sum_i e^{\tau z_i}$. With [softmax function](statistical-learning.md#softmax-function) weights $p_i$ and $D=\operatorname{Cov}(V)-\operatorname{Cov}(U)$, the derivative of $\mathbb EF_\tau(Z_r)$ is $\tfrac\tau4\mathbb E\sum_{i,j}p_ip_j(D_{ii}+D_{jj}-2D_{ij})\geq0$. Since $\max z_i\leq F_\tau(z)\leq\max z_i+\tau^{-1}\log n$, let $\tau\to\infty$. Singular [covariance matrices](variance.md#covariance-matrix) follow by adding identical small [independent](random-variable.md#independent-random-variables) [normal](probability-theory.md#normal-distribution) noise to both vectors and taking a limit.

<h3 id="slepian-s-lemma">Slepian's lemma</h3>

↑ **Parent:** [Gaussian process](#gaussian-process)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Slepian's_lemma)

For centered [multivariate normal distributions](probability-and-statistics.md#multivariate-normal-distribution) represented by vectors $U,V$ with equal corresponding [variances](variance.md) and $\mathbb E[U_iU_j]\geq\mathbb E[V_iV_j]$ for all distinct indices, $\mathbb P(U_i\leq u_i\text{ for all }i)\geq\mathbb P(V_i\leq u_i\text{ for all }i)$ for every threshold vector. In particular the [supremum](real-analysis.md#supremum) of $U$ is stochastically smaller than the [supremum](real-analysis.md#supremum) of $V$. Equal corresponding [variances](variance.md) are essential to this formulation. The related [Sudakov-Fernique inequality](#sudakov-fernique-inequality) compares [expected values](probability-theory.md#expected-value) of maxima using [variances](variance.md) of increments and does not require equal pointwise [variances](variance.md).

### Mean-square derivative of a Gaussian process

↑ **Parent:** [Gaussian process](#gaussian-process)

A [Gaussian process](#gaussian-process) has a mean-square derivative at $t$ when its difference quotients converge in [L2 space](measure-theory.md#l2-space-is-a-hilbert-space). The [mean-square convergence](convergence-of-random-variables.md#convergence-in-l2) need not give differentiable sample paths. For a centered [stationary process](time-series.md#stationary-process) with twice continuously differentiable [covariance function](#covariance-function) $K(t-s)$, the difference quotients are Cauchy in [L2 space](measure-theory.md#l2-space-is-a-hilbert-space), since their [covariance](variance.md#covariance) is a rectangular average of $-K''$. Their limits form a [Gaussian process](#gaussian-process) with [covariance function](#covariance-function) $\mathbb E[Y(s)Y(t)]=-K''(s-t)$.

#### Differentiable modification of a stationary Gaussian process

↑ **Parent:** [Mean-square derivative of a Gaussian process](#mean-square-derivative-of-a-gaussian-process)

For a centered [Gaussian process](#gaussian-process) with [covariance function](#covariance-function) $K(s-t)$, twice continuous differentiability of $K$ and differentiability of $K''$ at zero imply a differentiable [modification of a stochastic process](#modification-of-a-stochastic-process) on compact intervals. The [even function](calculus.md#even-function) $K''$ satisfies $K'''(0)=0$, so the mean-square derivative $Y$ has [variance](variance.md) of increments $2(K''(h)-K''(0))=o(|h|)$. A [normal distribution](probability-theory.md#normal-distribution) has fourth absolute moment three times the square of its [variance](variance.md), so [Kolmogorov continuity theorem](#kolmogorov-continuity-theorem) gives a [continuous modification](#continuous-modification) of $Y$. The [mean-square fundamental theorem of calculus](#mean-square-fundamental-theorem-of-calculus) identifies its path integral with a [modification of a stochastic process](#modification-of-a-stochastic-process) of $X$. This argument does not require integrability of $K$ or continuity of $K'''$.

#### Mean-square fundamental theorem of calculus

↑ **Parent:** [Mean-square derivative of a Gaussian process](#mean-square-derivative-of-a-gaussian-process)

If an [L2 space](measure-theory.md#l2-space-is-a-hilbert-space)-valued map $X$ has a continuous mean-square derivative $Y$, then its increments equal the [Bochner integral](measure-theory.md#bochner-integral) of $Y$. To see this, for each partition interval $[t_j,t_{j+1}]$, continuous linear observations and the scalar mean-value bound give $\|X(t_{j+1})-X(t_j)-(t_{j+1}-t_j)Y(t_j)\|_2\leq(t_{j+1}-t_j)\sup_{u\in[t_j,t_{j+1}]}\|Y(u)-Y(t_j)\|_2$. Sum these errors. Uniform continuity of $Y$ makes the total error tend to zero as the mesh tends to zero, while the [Riemann sums](real-analysis.md#riemann-sum) converge to the [Bochner integral](measure-theory.md#bochner-integral). This proves the [fundamental theorem of calculus](calculus.md#fundamental-theorem-of-calculus) in [L2 space](measure-theory.md#l2-space-is-a-hilbert-space). If a [Gaussian process](#gaussian-process) derivative also has a [continuous modification](#continuous-modification), its anchored path integral $X(s)+\int_s^t\widetilde Y(u)\,du$ therefore produces a differentiable [modification of a stochastic process](#modification-of-a-stochastic-process) of the original [Gaussian process](#gaussian-process).

### Gaussian process classification

↑ **Parent:** [Gaussian process](#gaussian-process)

[Gaussian process classification](#gaussian-process-classification) links [latent variables](statistical-modelling.md#latent-variable) from a [Gaussian process](#gaussian-process) to class [probabilities](probability-theory.md#probability). A binary [probit regression](statistical-modelling.md#probit-model) likelihood is $\prod_i\Phi((2y_i-1)f_i)$ under [conditional independence](random-variable.md#conditional-independence). The [posterior distribution](statistical-inference.md#bayesian-posterior) of the latent values is not a [normal distribution](probability-theory.md#normal-distribution).

### Periodic covariance function

↑ **Parent:** [Gaussian process](#gaussian-process)

This [covariance function](#covariance-function) is periodic with period $P>0$. Map time to the circle $u(t)=(\cos(2\pi t/P),\sin(2\pi t/P))$ and pull back a [Gaussian kernel](probability-and-statistics.md#gaussian-kernel); since $\|u(t)-u(t')\|^2=4\sin^2(\pi(t-t')/P)$, this proves positive semidefiniteness. A [Gaussian process](#gaussian-process) with this kernel has $\operatorname{Var}(f(t+P)-f(t))=0$ and therefore repeats at every fixed phase. Replacing the inner $\pi$ by $2\pi$ changes the actual period to $P/2$.

#### Periodic Gaussian process with zero period average

↑ **Parent:** [Periodic covariance function](#periodic-covariance-function)

A zero-mean [Gaussian process](#gaussian-process) need not have zero average in each realization. For the [periodic covariance function](#periodic-covariance-function), the constant Fourier component is

$$
c_0=\frac1P\int_0^Pk_P(t,u)\,du=A^2e^{-\ell^{-2}}I_0(\ell^{-2}),
$$

where $I_0$ is a [modified Bessel function](analysis.md#modified-bessel-function). Replacing $f(t)$ by $f(t)-P^{-1}\int_0^Pf(u)\,du$ gives a Gaussian process with kernel $k_P(t,t')-c_0$. This is a [positive-semidefinite kernel](probability-and-statistics.md#positive-semidefinite-kernel) because it is a covariance after a linear transformation, and each sample has zero period average. The [real integral representation of the modified Bessel function I0](analysis.md#real-integral-representation-of-the-modified-bessel-function-i0) yields the displayed constant.

### Gaussian-process marginal likelihood

↑ **Parent:** [Gaussian process](#gaussian-process)

For Gaussian-process latent values with mean vector $m$ and covariance matrix $K$, observed with independent Gaussian noise covariance $E$, integrating out the latent values gives the marginal distribution $N(m,K+E)$. Its density as a function of the mean and kernel parameters is the Gaussian-process marginal likelihood.

### Gaussian concentration inequality

↑ **Parent:** [Gaussian process](#gaussian-process)

A Lipschitz function of a Gaussian vector has sub-Gaussian deviations from its mean, with scale controlled by the covariance operator and the Lipschitz constant. In particular, if the covariance operator norm is at most one and $f$ is one-Lipschitz, then universal constants $c,C>0$ give

$$
\mathbb P(f(X)>\mathbb Ef(X)+u)\leq C e^{-cu^2}.
$$

#### Brownian martingale proof of Gaussian concentration

↑ **Parent:** [Gaussian concentration inequality](#gaussian-concentration-inequality)

For a standard Gaussian vector $G$ and a smooth [Lipschitz function](real-analysis.md#lipschitz-continuity) with $\lVert\nabla f\rVert\le K$, represent its centered value as the terminal [martingale](martingale.md) $P_{1-t}f(B_t)-P_1f(0)$. The [Itô formula](stochastic-calculus.md#ito-s-lemma) gives gradient integrand $P_{1-t}\nabla f$, whose norm is at most $K$. Its terminal [quadratic variation](stochastic-calculus.md#quadratic-variation) is therefore at most $K^2$. The [Dambis-Dubins-Schwarz theorem](martingale.md#dambis-dubins-schwarz-theorem) bounds the terminal deviation by a maximum of [Brownian motion](brownian-motion.md) over $[0,K^2]$. Symmetry, the [Brownian reflection principle](brownian-motion.md#reflection-principle-wiener-process), and the [Gaussian tail bound](probability-and-statistics.md#gaussian-tail-bound) give the displayed inequality. The square on the Lipschitz constant is essential by scaling.

#### Gaussian rotation interpolation inequality

↑ **Parent:** [Gaussian concentration inequality](#gaussian-concentration-inequality)

For [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables) $X,Y$ with a centered [multivariate normal distribution](probability-and-statistics.md#multivariate-normal-distribution), a [continuously differentiable function](calculus.md#continuously-differentiable-function) $f$ with bounded [gradient](calculus.md#gradient), and a [convex function](real-analysis.md#convex-function) $\Psi$ for which the expressions are integrable, the displayed inequality holds. First apply [Jensen inequality](real-analysis.md#jensen-s-inequality) conditionally to $f(X)-f(Y)$. For the [Gaussian rotation of independent copies](probability-and-statistics.md#gaussian-rotation-of-independent-copies), the [chain rule](calculus.md#chain-rule) gives $f(X)-f(Y)=\int_0^{\pi/2}\langle\nabla f(U_\theta),V_\theta\rangle\,d\theta$. A second application of [Jensen inequality](real-analysis.md#jensen-s-inequality) to the uniform measure on $[0,\pi/2]$, followed by the [Gaussian rotation of independent copies](probability-and-statistics.md#gaussian-rotation-of-independent-copies), proves the inequality. The useful choice $\Psi(v)=e^{\lambda|v|}$ yields a [Gaussian concentration inequality](#gaussian-concentration-inequality) through an [exponential moment of an absolute standard normal variable](probability-theory.md#exponential-moment-of-an-absolute-standard-normal-variable).

### Dudley entropy integral

↑ **Parent:** [Gaussian process](#gaussian-process)

For a centered Gaussian process $(X_t)_{t\in T}$ with canonical pseudometric $d(s,t)^2=\mathbb E|X_s-X_t|^2$,

$$
\mathbb E\sup_{t\in T}X_t
\leq C\int_0^{\operatorname{diam}(T)}
\sqrt{\log N(\epsilon,T,d)}\,d\epsilon,
$$

where $N(\epsilon,T,d)$ is the covering number.

### Borell-TIS inequality

↑ **Parent:** [Gaussian process](#gaussian-process)

If a centered separable Gaussian process has finite expected supremum $m$ and $\sigma^2=\sup_t\operatorname{Var}(X_t)$, then

$$
\mathbb P\left(\sup_tX_t>m+u\right)
\leq e^{-u^2/(2\sigma^2)}.
$$

### Isonormal Gaussian process

↑ **Parent:** [Gaussian process](#gaussian-process)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Isonormal_Gaussian_process)

An isonormal Gaussian process over a real [Hilbert space](hilbert-space.md) $H$ is a centered [Gaussian process](#gaussian-process) $(W(h))_{h\in H}$ satisfying

$$
\mathbb E[W(f)W(g)]=\langle f,g\rangle_H.
$$

It turns the geometry of $H$ into the [covariance](variance.md#covariance) structure of a Gaussian family.

#### Exponential tilting of an isonormal Gaussian process

↑ **Parent:** [Isonormal Gaussian process](#isonormal-gaussian-process)

For an [isonormal Gaussian process](#isonormal-gaussian-process) $X$ on a real [Hilbert space](hilbert-space.md) $H$ and $k\in H$, the positive density $\exp(X(k)-\|k\|^2/2)$ has expectation one and defines an [equivalent probability measure](measure-theory.md#equivalent-probability-measure). Under this measure, $X(h)$ has mean $\langle h,k\rangle$ and the same [covariance](variance.md#covariance) as before. The shifted family $X(h)-\langle h,k\rangle$ is again an [isonormal Gaussian process](#isonormal-gaussian-process). This follows by evaluating the joint Gaussian exponential formula for any finite collection of arguments. It is the Hilbert-space version of [exponential tilting](probability-theory.md#exponential-tilting).

### Gaussian white noise

↑ **Parent:** [Gaussian process](#gaussian-process)

Gaussian white noise is a generalized Gaussian process with zero mean and covariance proportional to a [Dirac delta function](distribution-theory.md#dirac-delta-function) in time, and possibly in space. It is the formal time derivative of [Brownian motion](brownian-motion.md) and has independent fluctuations on disjoint time intervals.

#### Gaussian white noise model

↑ **Parent:** [Gaussian white noise](#gaussian-white-noise)

Observe $Y(t)=\int_0^tf(s)\,ds+\sigma W(t)$ on $[0,1]$, where $f\in L^2[0,1]$ is an unknown deterministic drift and $W$ is standard [Brownian motion](brownian-motion.md). The observation against a deterministic test [function](function.md) is $Y(h)=\langle f,h\rangle+\sigma W(h)$, with [covariance](variance.md#covariance) $\sigma^2\langle h,g\rangle$. [Gaussian white noise](#gaussian-white-noise) is represented by an [isonormal Gaussian process](#isonormal-gaussian-process) on test [functions](function.md) rather than a pointwise noise [function](function.md). Taking $\sigma=n^{-1/2}$ is the usual statistical scaling.

#### White-noise likelihood for a square-integrable shift

↑ **Parent:** [Gaussian white noise](#gaussian-white-noise)

Generalized [Gaussian white noise](#gaussian-white-noise) over a real [Hilbert space](hilbert-space.md) $H=L^2$ is an [isonormal Gaussian process](#isonormal-gaussian-process) $W(h)$ with covariance $\langle h,g\rangle_H$. Its law $P_0$ is carried on a larger observation space; the identity is not the covariance of an infinite-dimensional $H$-valued [Gaussian measure](#gaussian-measure) because it is not a [trace-class operator](compact-operator.md#trace-class-operator). A deterministic signal $h\in H$ defines a translated observation law $P_h$ with [Radon-Nikodym derivative](measure-theory.md#radon-nikodym-derivative)

$$
\frac{dP_h}{dP_0}(m)=\exp\left(W_m(h)-\tfrac12\|h\|_H^2\right).
$$

In an [orthonormal basis](linear-algebra.md#orthonormal-basis), $W_m(h)=\sum_jm_jh_j$ is a stochastic series with total [variance](variance.md) $\|h\|_H^2$, not an inner product of two $H$-valued observations. The formula follows from the [Cameron-Martin theorem for a Gaussian measure](#cameron-martin-theorem-for-a-gaussian-measure) in its generalized white-noise version, or from finite-dimensional Gaussian likelihood ratios. On $\mathbb R^2$, generalized noise can be realized on [tempered distributions](fourier-analysis.md#tempered-distribution); an unweighted global negative [Sobolev space](sobolev-space.md) is not automatically a suitable almost-sure support on an unbounded domain. The stochastic series avoids imposing that unsupported regularity.

#### Gaussian sequence model

↑ **Parent:** [Gaussian white noise](#gaussian-white-noise)

The Gaussian sequence model observes

$$
Y_k=\theta_k+n^{-1/2}g_k,
\qquad k\geq1,
$$

where the $g_k$ are independent standard normal variables and the unknown signal commonly lies in $\ell^2$. It is the coordinate representation of a Gaussian white-noise experiment.

##### Bernstein-von Mises theorem

↑ **Parent:** [Gaussian sequence model](#gaussian-sequence-model)

A Bernstein-von Mises theorem says that a suitably centered and scaled posterior distribution converges to the normal distribution prescribed by the local likelihood. For a fixed linear functional in a Gaussian sequence model and a prior with locally flat positive density, the limiting posterior variance is the squared $\ell^2$ norm of the functional's coefficient vector.

##### Gaussian net test

↑ **Parent:** [Gaussian sequence model](#gaussian-sequence-model)

A Gaussian net test covers a composite alternative by finitely many metric balls and takes the maximum of the likelihood-ratio tests against their centers. Gaussian tail bounds control each test, while a union bound costs the logarithm of the covering number.

##### Gaussian least-squares contrast

↑ **Parent:** [Gaussian sequence model](#gaussian-sequence-model)

Because Gaussian white noise is not an $\ell^2$ vector, least squares over $\Theta\subset\ell^2$ is defined by maximizing

$$
2\langle Y,\theta\rangle-\lVert\theta\rVert_2^2
$$

over $\theta\in\Theta$, with the noise pairing interpreted through an [isonormal Gaussian process](#isonormal-gaussian-process). Differences of this contrast equal the formal differences of squared residual norms.

### Independent increments of a Gaussian martingale

↑ **Parent:** [Gaussian process](#gaussian-process)

A centered continuous [Gaussian process](#gaussian-process) that is also a [martingale](martingale.md) has independent increments. Every future increment has zero [covariance](variance.md#covariance) with every finite vector of past values by the martingale property; [uncorrelated jointly normal variables are independent](probability-and-statistics.md#uncorrelated-jointly-normal-variables-are-independent).

#### Gaussian continuous martingale

↑ **Parent:** [Independent increments of a Gaussian martingale](#independent-increments-of-a-gaussian-martingale)

Every centered continuous Gaussian martingale starting at zero is a deterministic time change of [Brownian motion](brownian-motion.md). Its clock is the continuous increasing function $f(t)=\mathbb E[M_t^2]$, and $[M]_t=f(t)$.

##### Deterministic quadratic variation characterizes a Gaussian continuous local martingale

↑ **Parent:** [Gaussian continuous martingale](#gaussian-continuous-martingale)

If a continuous local martingale starts at zero and has deterministic continuous [quadratic variation](stochastic-calculus.md#quadratic-variation) $[M]_t=f(t)$, the [Dambis-Dubins-Schwarz theorem](martingale.md#dambis-dubins-schwarz-theorem) gives $M_t=B_{f(t)}$. It is therefore a centered [Gaussian process](#gaussian-process). The converse follows from [independent increments of a Gaussian martingale](#independent-increments-of-a-gaussian-martingale).

### Exponential covariance function

↑ **Parent:** [Gaussian process](#gaussian-process)

The stationary exponential covariance function is

$$
k(s,t)=R\exp(-|t-s|/\tau).
$$

The corresponding [Gaussian process](#gaussian-process) is Markov and is a stationary [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process).

### Gaussian random field

↑ **Parent:** [Gaussian process](#gaussian-process)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaussian_random_field)

A Gaussian random field is a spatially indexed [Gaussian process](#gaussian-process); its law is determined by its mean and covariance kernel.

#### Brownian sheet

↑ **Parent:** [Gaussian random field](#gaussian-random-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Brownian_sheet)

A centered [Gaussian random field](#gaussian-random-field) with the displayed covariance. It has independent increments over disjoint rectangles. At fixed positive $T$, $W(t,T)/\sqrt T$ is standard [Brownian motion](brownian-motion.md) in $t$. It provides one possible maturity-correlated Gaussian noise for a [Gaussian forward-rate field](mathematical-finance.md#gaussian-forward-rate-field); the forward-rate drift must still satisfy the [Heath-Jarrow-Morton model](mathematical-finance.md#heath-jarrow-morton-model) restriction.

#### Gaussian marginals do not imply a Gaussian random field

↑ **Parent:** [Gaussian random field](#gaussian-random-field)

Let $X$ be a standard [Gaussian random variable](probability-theory.md#gaussian-random-variable) and $S_j$ independent symmetric signs, independent of $X$. The stationary sequence $W_j=S_jX$ has standard Gaussian marginals and identity covariance, but is not jointly Gaussian. For two coordinates its [moment-generating function](probability-theory.md#moment-generating-function) is $(1+e^{2t^2})/2$, rather than $e^{t^2}$. Consequently a field's Gaussian one-point densities and two-point covariance alone do not justify an [exponential moment of a Gaussian linear functional](#exponential-moment-of-a-gaussian-linear-functional).

#### Centered quadratic Gaussian transformation

↑ **Parent:** [Gaussian random field](#gaussian-random-field)

If $G$ is a centered [Gaussian random field](#gaussian-random-field), the transformation $G+\alpha(G^2-\langle G^2\rangle)$ retains zero mean and introduces a three-point [connected correlation function](critical-phenomenon.md#connected-correlation-function) at first order in $\alpha$. [Wick contractions](perturbative-quantum-field-theory.md#wick-contraction) give $2\alpha$ times the sum of products of two covariances. The corresponding local cosmological model uses $\alpha=3f_{\mathrm{NL}}/5$.

#### Exponential moment of a Gaussian linear functional

↑ **Parent:** [Gaussian random field](#gaussian-random-field)

If a linear functional $Z=\int a(\mathbf r)V(\mathbf r)\,d\mathbf r$ of a real [Gaussian random field](#gaussian-random-field) exists in mean square, it is a [Gaussian random variable](probability-theory.md#gaussian-random-variable). Completing the square in its density gives

$$
\mathbb E e^Z=\exp\left(\mathbb EZ+\frac12\operatorname{Var}Z\right),\qquad \operatorname{Var}Z=\iint a(\mathbf r)a(\mathbf r')\operatorname{Cov}[V(\mathbf r),V(\mathbf r')]\,d\mathbf r\,d\mathbf r'.
$$

For a complex linear functional $\phi$, apply this to $Z=2\operatorname{Re}\phi$; then $\tfrac12\operatorname{Var}Z=\mathbb E|\phi-\mathbb E\phi|^2+\operatorname{Re}\mathbb E(\phi-\mathbb E\phi)^2$.

##### Gaussian quadratic exponential moment

↑ **Parent:** [Exponential moment of a Gaussian linear functional](#exponential-moment-of-a-gaussian-linear-functional)

For a real standard [Gaussian random vector](probability-and-statistics.md#gaussian-random-vector) $Z$, a real symmetric matrix $Q$, and $I-2Q$ strictly positive,

$$
\mathbb E e^{b^TZ+Z^TQZ}=\det(I-2Q)^{-1/2}\exp\left[\frac12b^T(I-2Q)^{-1}b\right].
$$

Diagonalize $Q$ and complete the square in each coordinate. Failure of strict positivity makes the positive exponential integral divergent. The same formula extends to a self-adjoint trace-class quadratic form of an isonormal [Gaussian process](#gaussian-process), with square-summable linear coefficients and a [Fredholm determinant](compact-operator.md#fredholm-determinant). A linear-plus-quadratic [Gaussian random field](#gaussian-random-field) functional is reduced to this form by its covariance square root.

#### Stationary Gaussian random field

↑ **Parent:** [Gaussian random field](#gaussian-random-field)

A stationary Gaussian random field has Gaussian finite-dimensional distributions invariant under common spatial translations. Its mean is constant and its two-point covariance depends only on the separation of the points.

##### Autocorrelation function of a random field

↑ **Parent:** [Stationary Gaussian random field](#stationary-gaussian-random-field)

For a zero-mean [stationary Gaussian random field](#stationary-gaussian-random-field) $V(\mathbf r)$, the autocorrelation function is

$$
C_V(\mathbf s)
=\mathbb E[V(\mathbf r)V(\mathbf r+\mathbf s)],
$$

which is independent of $\mathbf r$. Its [Fourier transform](analysis.md#fourier-transform) is the spatial power spectral density.

###### Covariance of a squared random field

↑ **Parent:** [Autocorrelation function of a random field](#autocorrelation-function-of-a-random-field)

For $W=n^2-\langle n^2\rangle$, the [covariance function](#covariance-function) is $\langle n^2n'^2\rangle-\langle n^2\rangle\langle n'^2\rangle$. It involves fourth moments and is not determined by the two-point correlation of $n$ in general. For a centered Gaussian pair the fourth-moment identity reduces it to $2\langle nn'\rangle^2$. This extra Gaussian hypothesis must be stated before using that reduction.

<h4 id="novikov-s-theorem">Novikov's theorem</h4>

↑ **Parent:** [Gaussian random field](#gaussian-random-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Novikov's_theorem)

For a centered [Gaussian random field](#gaussian-random-field) $W$ with covariance $C$ and a sufficiently regular functional $F[W]$, the Furutsu--Novikov formula is the functional [integration by parts](calculus.md#integration-by-parts) identity

$$
\mathbb E[W(x)F[W]]
=\int C(x,y)\mathbb E\left[\frac{\delta F}{\delta W(y)}\right]dy.
$$

It closes moment equations for systems driven multiplicatively by Gaussian fluctuations.

#### Markov approximation for a random medium

↑ **Parent:** [Gaussian random field](#gaussian-random-field)

When a random medium's longitudinal correlation length is much shorter than the scale on which a propagating envelope changes, the Markov approximation replaces the longitudinal covariance by white noise with the same integrated covariance. Field-moment equations then become local in propagation distance.

#### Gaussian free field

↑ **Parent:** [Gaussian random field](#gaussian-random-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaussian_free_field)

The Gaussian free field is a centered [Gaussian random field](#gaussian-random-field) whose covariance is the Green kernel of a Laplace operator. It has discrete versions on graphs and continuum versions as a random generalized function on a domain.

##### Discrete Gaussian free field

↑ **Parent:** [Gaussian free field](#gaussian-free-field)

The discrete Gaussian free field on a transient weighted graph is the centered [Gaussian random field](#gaussian-random-field) whose covariance kernel is the random-walk [Green function of a transient weighted graph](markov-process.md#green-function-of-a-transient-weighted-graph).

###### Gaussian free field with Dirichlet boundary condition

↑ **Parent:** [Discrete Gaussian free field](#discrete-gaussian-free-field)

A Gaussian free field with Dirichlet boundary condition is fixed to zero on a boundary set and has density proportional to the exponential of minus one half of its discrete Dirichlet energy on the remaining vertices.

###### Gibbs-Markov property of the discrete Gaussian free field

↑ **Parent:** [Gaussian free field with Dirichlet boundary condition](#gaussian-free-field-with-dirichlet-boundary-condition)

Conditionally on all other values, a discrete Gaussian free field value is Gaussian with mean equal to the weighted average of its neighbors and variance equal to the reciprocal local precision.

###### Spatial Markov property of the Gaussian free field

↑ **Parent:** [Gaussian free field with Dirichlet boundary condition](#gaussian-free-field-with-dirichlet-boundary-condition)

Conditioning a Gaussian free field on its values along a boundary leaves an independent zero-boundary Gaussian free field plus the harmonic extension of those boundary values in each remaining component.

##### Continuum Gaussian free field

↑ **Parent:** [Gaussian free field](#gaussian-free-field)

The continuum Gaussian free field on a planar domain $D$ is a centered [Gaussian process](#gaussian-process) indexed by finite-energy [measures](measure-theory.md#measure) or [test functions](distribution-theory.md#test-function), with [covariance](variance.md#covariance) given by the [Green function of the Laplacian](partial-differential-equation.md#green-function-of-the-laplacian) on $D$.

###### Conformal invariance of the two-dimensional Gaussian free field

↑ **Parent:** [Continuum Gaussian free field](#continuum-gaussian-free-field)

If $\phi:D\to\widetilde D$ is a [conformal map](geometry-and-topology.md#conformal-map), pulling back a zero-boundary Gaussian free field on $\widetilde D$ gives a zero-boundary Gaussian free field on $D$. This follows from the conformal invariance of the planar Dirichlet Green function.

###### Zero-boundary Gaussian free field

↑ **Parent:** [Continuum Gaussian free field](#continuum-gaussian-free-field)

For finite Borel measures $\rho,\nu$ of finite Green energy, the zero-boundary Gaussian free field $h$ on $D$ is characterized by

$$
\mathbb E[(h,\rho)(h,\nu)]=\iint_{D\times D}G_D(x,y)\rho(dx)\nu(dy),
$$

where $G_D$ is the zero-Dirichlet [Green function of the Laplacian](partial-differential-equation.md#green-function-of-the-laplacian).

###### SLE4 coupling with a Gaussian free field

↑ **Parent:** [Zero-boundary Gaussian free field](#zero-boundary-gaussian-free-field)

For a [Gaussian free field](#gaussian-free-field) with boundary heights $-\lambda$ and $+\lambda$ on the two sides of the starting point, its distinguished zero-height interface has chordal $\operatorname{SLE}_4$ law. Conditional on an initial curve segment, the field is a zero-boundary field in the slit domain plus $m_t(z)=\lambda-(2\lambda/\pi)\arg(g_t(z)-W_t)$. Its mean bracket equals minus the variation of its conditional Green [covariance](variance.md#covariance). Subtracting the initial [harmonic function](partial-differential-equation.md#harmonic-function) gives the corresponding coupling to a zero-boundary field.

###### Gaussian characteristic-function martingale from covariance loss

↑ **Parent:** [SLE4 coupling with a Gaussian free field](#sle4-coupling-with-a-gaussian-free-field)

If a continuous mean [martingale](martingale.md) $M$ and a nonnegative finite-variation process $V$ satisfy $d\langle M\rangle=-dV$, then the [Itô formula](stochastic-calculus.md#ito-s-lemma) shows $\exp(iM-V/2)$ is a bounded complex [martingale](martingale.md). Its terminal expectation establishes an entire [Gaussian distribution](probability-theory.md#normal-distribution) with the initial mean and variance. This is stronger than matching only the first two moments in a random-domain field construction.

###### Gaussian free field level line

↑ **Parent:** [SLE4 coupling with a Gaussian free field](#sle4-coupling-with-a-gaussian-free-field)

A continuum field level line is specified by the harmonic boundary heights it creates and the conditional zero-boundary field remaining on each side. Since a [Continuum Gaussian free field](#continuum-gaussian-free-field) is a random distribution, this is not the pointwise set of its zeros. For the height jump appropriate to the Green-function normalization, the zero-height line between opposite Dirichlet heights is chordal $\operatorname{SLE}_4$.

###### Test-function pairing with a Gaussian free field

↑ **Parent:** [Zero-boundary Gaussian free field](#zero-boundary-gaussian-free-field)

For a [test function](distribution-theory.md#test-function) $\phi$ on $D$, let $f_\phi=-2\pi\Delta^{-1}\phi\in H_0^1(D)$. The pairing

$$
(h,\phi):=(h,f_\phi)_\nabla
$$

is a centered [Gaussian random variable](probability-theory.md#gaussian-random-variable) with variance

$$
\iint_{D\times D}\phi(x)G_D(x,y)\phi(y)\,dx\,dy.
$$

###### Green-kernel expansion in the Dirichlet space

↑ **Parent:** [Zero-boundary Gaussian free field](#zero-boundary-gaussian-free-field)

For an [orthonormal basis](linear-algebra.md#orthonormal-basis) $(e_n)$ of $H_0^1(D)$, the zero-Dirichlet [Green function of the Laplacian](partial-differential-equation.md#green-function-of-the-laplacian) is the weak kernel represented by

$$
G_D(x,y)=\sum_{n\geq1}e_n(x)e_n(y).
$$

Consequently, whenever the terms are defined and the right side is finite,

$$
\sum_{n\geq1}\left(\int_De_n\,d\rho\right)^2
=\iint_{D\times D}G_D(x,y)\rho(dx)\rho(dy).
$$

###### Finite-Green-energy measure pairing with a Gaussian free field

↑ **Parent:** [Green-kernel expansion in the Dirichlet space](#green-kernel-expansion-in-the-dirichlet-space)

If a measure $\rho$ has finite [Green energy](#green-energy), then

$$
(h,\rho)=\sum_{n\geq1}\xi_n\int_De_n\,d\rho
$$

converges in $L^2$ for any [orthonormal basis](linear-algebra.md#orthonormal-basis) $(e_n)$ of $H_0^1(D)$ and independent standard normal coefficients $\xi_n$. The limit is centered Gaussian with variance equal to the Green energy of $\rho$ and does not depend on the chosen basis.

###### Domain Markov property of the Gaussian free field

↑ **Parent:** [Zero-boundary Gaussian free field](#zero-boundary-gaussian-free-field)

For an open $U\subset D$, the field decomposes as $h=h_U+h^{D\setminus U}$, where $h_U$ is an independent zero-boundary Gaussian free field on $U$ and $h^{D\setminus U}$ is harmonic on $U$ and agrees with the outside field in the distributional sense.

###### Local set of a Gaussian free field

↑ **Parent:** [Domain Markov property of the Gaussian free field](#domain-markov-property-of-the-gaussian-free-field)

A random set is local for a [Gaussian free field](#gaussian-free-field) if, conditionally on the set and its associated [harmonic function](partial-differential-equation.md#harmonic-function), the remaining field is an independent zero-boundary field in its complement. This extends the deterministic [Domain Markov property of the Gaussian free field](#domain-markov-property-of-the-gaussian-free-field) to appropriate random revealed domains. Arbitrary field-dependent random sets need not have this property.

###### Circle-average process of the Gaussian free field

↑ **Parent:** [Zero-boundary Gaussian free field](#zero-boundary-gaussian-free-field)

Let $\rho_t$ be uniform measure on the circle of radius $e^{-t}$ around the origin in the unit disc. The process $X_t=(h,\rho_t)$ is the circle-average process. The [Domain Markov property of the Gaussian free field](#domain-markov-property-of-the-gaussian-free-field) and the [mean value property for harmonic functions](partial-differential-equation.md#mean-value-property-for-harmonic-functions) imply that its increments are independent and stationary.

###### Circle-average process of the Gaussian free field is Brownian motion

↑ **Parent:** [Circle-average process of the Gaussian free field](#circle-average-process-of-the-gaussian-free-field)

The circle-average process of a zero-boundary Gaussian free field in the unit disc has the law of a constant multiple of [Brownian motion](brownian-motion.md). It is a continuous centered [Gaussian process](#gaussian-process) with [stationary increments](#stationary-increments) and [independent increments](#independent-increments) and starts at zero.

##### Green energy

↑ **Parent:** [Gaussian free field](#gaussian-free-field)

For a measure $\mu$ and Green kernel $G$, its Green energy is

$$
I_G(\mu)=\iint G(x,y)d\mu(x)d\mu(y).
$$

Finite Green energy is the variance condition needed to pair a Gaussian free field with $\mu$.

##### Pinned Gaussian free field

↑ **Parent:** [Gaussian free field](#gaussian-free-field)

Pinning a Gaussian free field at a vertex $o$ gives the field with value zero at $o$ and covariance

$$
g^{\{o\}^c}(x,y)=g(x,y)-\frac{g(x,o)g(o,y)}{g(o,o)}.
$$

It is independent of the removed scalar Gaussian mode at $o$.

### Gaussian zero-one law for measurable linear subspaces

↑ **Parent:** [Gaussian process](#gaussian-process)

Every linear subspace that is measurable for the [cylinder sigma-algebra](probability-theory.md#cylinder-sigma-algebra) has probability zero or one under a centered Gaussian process.

### Gaussian measure

↑ **Parent:** [Gaussian process](#gaussian-process)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaussian_measure)

A Gaussian measure on a real topological vector space is a Borel probability measure whose image under every continuous linear functional is a one-dimensional normal distribution.

<h4 id="fernique-s-theorem">Fernique's theorem</h4>

↑ **Parent:** [Gaussian measure](#gaussian-measure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fernique's_theorem)

A [Gaussian random variable in a Banach space](#gaussian-random-variable-in-a-banach-space) taking values in a [separable Banach space](banach-space.md#separable-banach-space) satisfies the displayed exponential-integrability bound for some positive $a$. In particular every finite power of its [norm](functional-analysis.md#norm) has a finite [expected value](probability-theory.md#expected-value). The value of $a$ depends on the [Gaussian measure](#gaussian-measure); the theorem does not assert this for every positive $a$.

#### First Gaussian chaos

↑ **Parent:** [Gaussian measure](#gaussian-measure)

For a centered [Gaussian random variable in a Banach space](#gaussian-random-variable-in-a-banach-space), its first Gaussian chaos is the closed [linear subspace](vector-space.md#vector-subspace) of [L2 space](measure-theory.md#l2-space-is-a-hilbert-space) generated by its continuous linear observations. Every element is a centered [Gaussian random variable](probability-theory.md#gaussian-random-variable), and every finite collection has a [multivariate normal distribution](probability-and-statistics.md#multivariate-normal-distribution): approximate in [L2 space](measure-theory.md#l2-space-is-a-hilbert-space) and pass to the [characteristic function](probability-theory.md#characteristic-function). The first Gaussian chaos supplies the scalar coordinates of its [Cameron-Martin space of a Gaussian random variable in a Banach space](#cameron-martin-space-of-a-gaussian-random-variable-in-a-banach-space).

#### Gaussian random variable in a Banach space

↑ **Parent:** [Gaussian measure](#gaussian-measure)

A random variable $X$ in a real [separable Banach space](banach-space.md#separable-banach-space) $B$ is Gaussian when $\ell(X)$ has a [normal distribution](probability-theory.md#normal-distribution) for every [continuous linear functional](topological-vector-space.md#continuous-linear-functional) $\ell\in B^*$. It is centered when all these [expected values](probability-theory.md#expected-value) vanish. Its [probability law](probability-theory.md#probability-distribution) is a [Gaussian measure](#gaussian-measure). Degenerate [normal distributions](probability-theory.md#normal-distribution) are allowed.

##### Strict increase of a Gaussian norm distribution

↑ **Parent:** [Gaussian random variable in a Banach space](#gaussian-random-variable-in-a-banach-space)

Suppose $B$ is a nonzero [separable Banach space](banach-space.md#separable-banach-space), the [Cameron-Martin space of a Gaussian random variable in a Banach space](#cameron-martin-space-of-a-gaussian-random-variable-in-a-banach-space) is a [dense subset](topology.md#dense-set) of $B$, and every centered ball of positive radius has positive [probability](probability-theory.md#probability). Then $t\mapsto\mathbb P(\|X\|_B\leq t)$ is strictly increasing on $(0,\infty)$. For $0<a<b$, choose $h$ in that [Cameron-Martin space of a Gaussian random variable in a Banach space](#cameron-martin-space-of-a-gaussian-random-variable-in-a-banach-space) with $\|h\|_B=(a+b)/2$ and $0<\delta<(b-a)/2$. The closed ball of radius $\delta$ centered at $h$ lies in the annulus $a<\|x\|_B<b$ and has positive [probability](probability-theory.md#probability) by the [symmetric Gaussian translation lower bound](#symmetric-gaussian-translation-lower-bound). The nonzero assumption is necessary: on $B=\{0\}$ the distribution function equals one everywhere.

#### Cameron-Martin theorem for a Gaussian measure

↑ **Parent:** [Gaussian measure](#gaussian-measure)

For $\mu=\mathcal N(0,\Sigma)$ with injective [covariance operator of a Gaussian measure](#covariance-operator-of-a-gaussian-measure), its translated law $\mu_h=\mathcal N(h,\Sigma)$ is an [equivalent probability measure](measure-theory.md#equivalent-probability-measure) to $\mu$ if and only if $h\in E_\mu$, the [Cameron-Martin space of a Gaussian measure](#cameron-martin-space-of-a-gaussian-measure). For such $h$,

$$
\frac{d\mu_h}{d\mu}(x)=\exp\left(\ell_h(x)-\tfrac12\|h\|_{E_\mu}^2\right),\qquad
\ell_h(x)=\sum_j\frac{h_jx_j}{\lambda_j}.
$$

The series has [mean-square convergence](convergence-of-random-variables.md#convergence-in-l2) and converges [almost surely](convergence-of-random-variables.md#almost-sure-convergence) under $\mu$, with [normal distribution](probability-theory.md#normal-distribution) $\mathcal N(0,\|h\|_{E_\mu}^2)$. Its exponential density has [expected value](probability-theory.md#expected-value) one by the [moment-generating function of a normal distribution](probability-theory.md#moment-generating-function-of-a-normal-distribution). Finite-dimensional projections give the formula by ratios of [multivariate normal densities](probability-and-statistics.md#multivariate-normal-density); convergence of these likelihood ratios gives the infinite-dimensional result. The expression $\langle h,x\rangle_{E_\mu}$ is only formal when the sample is outside $E_\mu$. For $h\notin E_\mu$, translation gives [mutually singular measures](measure-theory.md#mutually-singular-measures).

##### Symmetric Gaussian translation lower bound

↑ **Parent:** [Cameron-Martin theorem for a Gaussian measure](#cameron-martin-theorem-for-a-gaussian-measure)

For a centered [Gaussian random variable in a Banach space](#gaussian-random-variable-in-a-banach-space), a [Borel set](measure-theory.md#borel-set) $C=-C$, and $h$ in its [Cameron-Martin space of a Gaussian random variable in a Banach space](#cameron-martin-space-of-a-gaussian-random-variable-in-a-banach-space), the [Cameron-Martin theorem for a Gaussian measure](#cameron-martin-theorem-for-a-gaussian-measure) gives the translated density $e^{-\widehat h(X)-\|h\|_H^2/2}$. The joint law of $(X,\widehat h(X))$ is invariant under simultaneous negation. Averaging the two density formulas therefore replaces $e^{-\widehat h(X)}$ by $\cosh\widehat h(X)\geq1$, proving the lower bound. No [convexity](real-analysis.md#convex-function) of $C$ is required.

#### Cameron-Martin space of a Gaussian measure

↑ **Parent:** [Gaussian measure](#gaussian-measure)

For a centered [Gaussian measure](#gaussian-measure) on a real [Hilbert space](hilbert-space.md) with injective [covariance operator of a Gaussian measure](#covariance-operator-of-a-gaussian-measure) $\Sigma$, its Cameron-Martin space is $E_\mu=\operatorname{Ran}\Sigma^{1/2}$, with [inner product](linear-algebra.md#inner-product) $\langle h,g\rangle_{E_\mu}=\langle\Sigma^{-1/2}h,\Sigma^{-1/2}g\rangle$. In an [orthonormal basis](linear-algebra.md#orthonormal-basis) satisfying $\Sigma e_j=\lambda_je_j$, it consists of exactly the vectors $h$ for which $\sum_jh_j^2/\lambda_j<\infty$. It is complete in this stronger norm even if its range is not closed in the ambient norm. Its importance is that it describes precisely the translations that preserve the null sets of the [Gaussian measure](#gaussian-measure), as in the [Cameron-Martin theorem for a Gaussian measure](#cameron-martin-theorem-for-a-gaussian-measure). For generalized [Gaussian white noise](#gaussian-white-noise) over $L^2$, the corresponding Cameron-Martin space is [L2 space](measure-theory.md#l2-space-is-a-hilbert-space) itself.

##### Cameron-Martin space of a Gaussian random variable in a Banach space

↑ **Parent:** [Cameron-Martin space of a Gaussian measure](#cameron-martin-space-of-a-gaussian-measure)

Let $\mathcal G$ be the [first Gaussian chaos](#first-gaussian-chaos) of a centered [Gaussian random variable in a Banach space](#gaussian-random-variable-in-a-banach-space). By [Fernique's theorem](#fernique-s-theorem), $Sg=\mathbb E[Xg]$ is a [Bochner integral](measure-theory.md#bochner-integral) in $B$. The map $S$ is injective, because $Sg=0$ implies $\mathbb E[g\ell(X)]=0$ for every [continuous linear functional](topological-vector-space.md#continuous-linear-functional) $\ell$, hence $g=0$. Its range becomes a [Hilbert space](hilbert-space.md) under $\langle Sg,Sv\rangle_H=\mathbb E[gv]$. The embedding in $B$ is continuous by [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality). Its [reproducing property](probability-and-statistics.md#reproducing-property) is $\langle h,S\ell(X)\rangle_H=\ell(h)$. Thus this is the [Reproducing kernel Hilbert space](probability-and-statistics.md#reproducing-kernel-hilbert-space) of the random variable, including degenerate laws. For $h=Sg$, the scalar coordinate $\widehat h(X)=g$ has [variance](variance.md) $\|h\|_H^2$; it is generally a measurable linear coordinate rather than a continuous functional on $B$.

#### Covariance operator of a Gaussian measure

↑ **Parent:** [Gaussian measure](#gaussian-measure)

The covariance operator $K$ of a Gaussian measure on a real Hilbert space satisfies $\langle Kh,g\rangle=\operatorname{Cov}(\langle U,h\rangle,\langle U,g\rangle)$. A positive self-adjoint operator is the covariance of a Hilbert-space-valued Gaussian random variable exactly when it is trace class.

##### Hilbert-space Gaussian series

↑ **Parent:** [Covariance operator of a Gaussian measure](#covariance-operator-of-a-gaussian-measure)

If $Ke_j=\lambda_je_j$ with $\lambda_j\geq0$ and $\sum_j\lambda_j<\infty$, then

$$
U=m+\sum_j\sqrt{\lambda_j}\,\xi_je_j
$$

converges in mean square and almost surely in the Hilbert space, and has Gaussian law $N(m,K)$.

#### Bayesian inverse problem

↑ **Parent:** [Gaussian measure](#gaussian-measure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bayesian_inverse_problem)

A Bayesian inverse problem combines a prior measure $\mu_0$ on an unknown $u$ with a likelihood for observed data $y$. When the likelihood is proportional to $e^{-\Phi(u;y)}$, Bayes' formula gives

$$
\frac{d\mu^y}{d\mu_0}(u)=\frac1{Z(y)}e^{-\Phi(u;y)}.
$$

##### Bayes formula for a dominated observation model

↑ **Parent:** [Bayesian inverse problem](#bayesian-inverse-problem)

Suppose an unknown has [prior distribution](statistical-inference.md#prior-probability) $\Pi$ and its conditional observation law $P_u$ has jointly measurable [Radon-Nikodym derivative](measure-theory.md#radon-nikodym-derivative) $L(u,m)$ relative to a fixed observation law $P_0$. If $L>0$ for $\Pi(du)P_0(dm)$-almost every pair, then

$$
Z(m)=\int L(u,m)\Pi(du),\qquad
\frac{d\Pi^m}{d\Pi}(u)=\frac{L(u,m)}{Z(m)}
$$

defines the [posterior distribution](statistical-inference.md#bayesian-posterior) for almost every observation. Indeed, $\int L(u,m)P_0(dm)=1$ for almost every $u$, so [Tonelli theorem](measure-theory.md#tonelli-theorem) gives $\int Z(m)P_0(dm)=1$. Hence $Z$ is finite almost everywhere, and positivity of $L$ and [Fubini's theorem](measure-theory.md#fubini-s-theorem) give $Z>0$ almost everywhere. The data law is $ZP_0$, and integration of the proposed posterior against this data law recovers the joint law. This proves the [conditional distribution](probability-theory.md#conditional-distribution) property and also shows that the data law is an [equivalent probability measure](measure-theory.md#equivalent-probability-measure) to $P_0$.

##### Well-posed Bayesian inverse problem in total variation

↑ **Parent:** [Bayesian inverse problem](#bayesian-inverse-problem)

A Bayesian inverse problem is well posed in total variation when a unique posterior exists for every datum and the map from data to posterior is continuous in [total variation distance](probability-and-statistics.md#total-variation-distance).

##### Well-posed Bayesian inverse problem in Hellinger distance

↑ **Parent:** [Bayesian inverse problem](#bayesian-inverse-problem)

A Bayesian inverse problem is well posed in Hellinger distance when every datum determines a unique posterior and the posterior depends continuously on the data in [Hellinger distance](probability-and-statistics.md#hellinger-distance). Since posterior measures are dominated by the prior and squared Hellinger distance is at most twice [total variation distance](probability-and-statistics.md#total-variation-distance), total-variation well-posedness implies Hellinger well-posedness.

### Ornstein-Uhlenbeck process

↑ **Parent:** [Gaussian process](#gaussian-process)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ornstein–Uhlenbeck_process)

A stationary Ornstein-Uhlenbeck process is a Gaussian Markov process with exponential covariance $K(s,t)=A^2e^{-|t-s|/\tau}$.

#### Stationary drift saturation

↑ **Parent:** [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process)

For an adapted [stationary process](time-series.md#stationary-process) with the displayed bounds, the [Itô formula](stochastic-calculus.md#ito-s-lemma) and stationarity give $\int_0^t(\mathbb E[Z_sg_s]+\lambda)ds=0$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) makes each integrand nonnegative, so equality holds almost everywhere. Then $\mathbb E(g_s+\lambda Z_s)^2\le0$, proving $g=-\lambda Z$ for almost every time and outcome. Thus the process solves the [Ornstein-Uhlenbeck stochastic differential equation](#ornstein-uhlenbeck-stochastic-differential-equation) and its initial value, rather than stationarity alone, determines its coupling with W.

##### Same-noise stationary Ornstein-Uhlenbeck processes

↑ **Parent:** [Stationary drift saturation](#stationary-drift-saturation)

Two [Ornstein-Uhlenbeck processes](#ornstein-uhlenbeck-process) with the same driving [Brownian motion](brownian-motion.md) have the displayed difference. If $Y_0$ is standard normal and independent of future Brownian increments, replacing it by $-Y_0$ produces another [stationary process](time-series.md#stationary-process) with the same covariance and second moment, but a different pathwise coupling. Equal initial values are necessary for [indistinguishability of stochastic processes](#indistinguishability-of-stochastic-processes).

#### Exponential Brownian time change to a stationary Ornstein-Uhlenbeck process

↑ **Parent:** [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process)

For $\lambda>0$, set $\mathcal G_t=\mathcal F_{e^{2\lambda t}}$ and $W_t=(2\lambda)^{-1/2}\int_1^{e^{2\lambda t}}u^{-1/2}dB_u$. This is a [Brownian motion](brownian-motion.md) in the new [filtration](#filtration-probability-theory); its independent Gaussian increments have variance equal to elapsed time. The [Itô product rule](stochastic-calculus.md#ito-product-rule) gives $dY=\sqrt{2\lambda}\,dW-\lambda Y\,dt$. Its initial value is $B_1$, independent of future W increments, and its [covariance function](#covariance-function) is $e^{-\lambda|t-s|}$. Consequently it is a stationary [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process). The quadratic variation of the unscaled time change is $e^{2\lambda t}-1$, not $e^{2\lambda t}$.

#### Ornstein-Uhlenbeck stochastic differential equation

↑ **Parent:** [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process)

The linear [stochastic differential equation](stochastic-calculus.md#stochastic-differential-equation) has the explicit solution $Y_t=e^{-\lambda t}Y_0+\sigma\int_0^te^{-\lambda(t-s)}dW_s$. Its integrating factor is $e^{\lambda t}$. For $\lambda>0$, an independent initial normal variable of variance $\sigma^2/(2\lambda)$ makes its zero-mean [Gaussian process](#gaussian-process) stationary.

#### Ornstein-Uhlenbeck multiplicative amplification

↑ **Parent:** [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process)

Let $d\sigma=-\sigma\,dt/\tau+\sqrt\kappa\,dW$, $\sigma_0=0$, and $\dot B=\sigma B$, $B_0>0$. The logarithm $\log(B_t/B_0)=\int_0^t\sigma_sds$ is a centered [Gaussian random variable](probability-theory.md#gaussian-random-variable) of [variance](variance.md) $V(t)=\kappa\tau^2[t-2\tau(1-e^{-t/\tau})+\tau(1-e^{-2t/\tau})/2]$. Squaring the stochastic kernel $\sqrt\kappa\tau[1-e^{-(t-u)/\tau}]$ and integrating proves this formula. The [exponential moment of a Gaussian linear functional](#exponential-moment-of-a-gaussian-linear-functional) gives $\mathbb E B_t^n=B_0^ne^{n^2V(t)/2}$ and the displayed long-time growth exponent. Positive moment growth with zero mean strain reflects the breadth of the [log-normal distribution](probability-theory.md#log-normal-distribution); it does not imply positive growth of the mean logarithm.

##### Tilted Ornstein-Uhlenbeck oscillator transformation

↑ **Parent:** [Ornstein-Uhlenbeck multiplicative amplification](#ornstein-uhlenbeck-multiplicative-amplification)

The weighted strain density in [Ornstein-Uhlenbeck multiplicative amplification](#ornstein-uhlenbeck-multiplicative-amplification) evolves under $\mathcal L_np=(\kappa/2)p''+\tau^{-1}(\sigma p)'+n\sigma p$. Setting $p=e^{-\sigma^2/(2\kappa\tau)}\psi$ eliminates its first derivative. Shifting and scaling to $x=(\sigma-\kappa n\tau^2)/\sqrt{\kappa\tau}$ gives $\psi_{xx}+[1+\kappa n^2\tau^3-2\gamma\tau-x^2]\psi=0$. The [quantum harmonic oscillator](quantum-mechanics.md#quantum-harmonic-oscillator) levels yield the displayed [eigenvalues](linear-operator-theory.md#eigenvalue). Its [ground state](quantum-mechanics.md#ground-state) is the dominant positive mode; higher sign-changing modes may occur in a transient expansion.

#### Integrated Ornstein-Uhlenbeck displacement

↑ **Parent:** [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process)

For a thermal inertial [Langevin equation](#langevin-dynamics) conditioned on fixed initial position and velocity, the centered displacement is $R_i=\zeta^{-1}\int_0^t[1-e^{-\zeta(t-s)}]A_i(s)ds$. With the [fluctuation-dissipation relation for a Langevin particle](thermodynamics.md#fluctuation-dissipation-relation-for-a-langevin-particle), $D=k_BT/(m\zeta)$ and integrating the squared kernel gives the displayed [variance](variance.md). At short times it is $2D\zeta^2t^3/3$ per component; at long times it is $2Dt+O(1)$. Averaging initial velocity over thermal equilibrium adds a ballistic contribution and gives $2D[t-(1-e^{-\zeta t})/\zeta]$ per component.

#### Explicit Ornstein-Uhlenbeck solution

↑ **Parent:** [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process)

The solution of

$$
dX_t=-\lambda X_t\,dt+dB_t,\qquad X_0=x,
$$

is

$$
X_t=xe^{-\lambda t}+\int_0^te^{-\lambda(t-s)}\,dB_s.
$$

It has variance $(1-e^{-2\lambda t})/(2\lambda)$. Starting from $N(0,(2\lambda)^{-1})$ makes it stationary with covariance $e^{-\lambda|t-s|}/(2\lambda)$.

##### Zero-start Ornstein-Uhlenbeck covariance

↑ **Parent:** [Explicit Ornstein-Uhlenbeck solution](#explicit-ornstein-uhlenbeck-solution)

For $d\sigma=-\sigma\,dt/\tau+\sqrt\kappa\,dW$ with $\sigma_0=0$, the explicit [stochastic integral](stochastic-calculus.md#stochastic-integral) is $\sigma_t=\sqrt\kappa\int_0^te^{-(t-u)/\tau}dW_u$. The [Itô isometry](stochastic-calculus.md#ito-isometry) on the overlap of the two integration intervals gives the displayed [covariance](variance.md#covariance). The second exponential records the zero initial condition; removing it gives the stationary [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process) covariance.

#### Multivariate Ornstein-Uhlenbeck process

↑ **Parent:** [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process)

A multivariate Ornstein-Uhlenbeck process obeys $dX=-AX\,dt+b\,dW$. If every eigenvalue of $A$ has positive real part, its stationary covariance $\Sigma$ is the unique solution of $A\Sigma+\Sigma A^T=bb^T$.

##### Ornstein-Uhlenbeck power spectrum

↑ **Parent:** [Multivariate Ornstein-Uhlenbeck process](#multivariate-ornstein-uhlenbeck-process)

The stationary spectral-density matrix of $dX=-AXdt+b\,dW$ is

$$
S(\omega)=(A+i\omega I)^{-1}bb^T(A^T-i\omega I)^{-1}.
$$

#### Colored noise

↑ **Parent:** [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Colored_noise)

Colored noise has nonzero temporal correlation away from equal times. An Ornstein-Uhlenbeck noise has exponential covariance and approaches white noise when its correlation time tends to zero at fixed integrated covariance.

## Counting process

↑ **Parent:** [Stochastic process](stochastic-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Counting_process)

A counting process is an integer-valued stochastic process that starts at zero and increases by recording the cumulative number of events up to each time.

### Counting-process intensity

↑ **Parent:** [Counting process](#counting-process)

A predictable intensity $\lambda(t)$ is the derivative of an absolutely continuous [compensator of a counting process](#compensator-of-a-counting-process): $N(t)-\int_0^t\lambda(u)\,du$ is a [local martingale](martingale.md#local-martingale). It represents the conditional event rate given the immediately preceding history. In [survival analysis](survival-analysis.md) the individual intensity is an at-risk indicator multiplied by its [hazard function](survival-analysis.md#hazard-function).

### Counting-process intensity in survival analysis

↑ **Parent:** [Counting process](#counting-process)

An observed event [counting process](#counting-process) has conditional increment $\mathbb E(dN_i(t)\mid\mathcal H_{t-})=Y_i(t)h_i(t)\,dt$, where $Y_i$ is the [at-risk process](survival-analysis.md#at-risk-process). The [filtration](#filtration-probability-theory) records the past observed events, censoring, and [covariates](statistical-model.md#covariate); the integral of $Y_i h_i$ is the [compensator of a counting process](#compensator-of-a-counting-process).

### Compensator of a counting process

↑ **Parent:** [Counting process](#counting-process)

The compensator of a [counting process](#counting-process) $N(t)$ is a predictable increasing process $\Lambda(t)$ such that $N(t)-\Lambda(t)$ is a [local martingale](martingale.md#local-martingale). For an observed event process with [at-risk process](survival-analysis.md#at-risk-process) $Y(t)$ and [hazard function](survival-analysis.md#hazard-function) $h(t)$, it is $\Lambda(t)=\int_0^tY(u)h(u)\,du$ under [independent censoring](survival-analysis.md#independent-censoring). It is cumulative intensity, rather than an event probability.

#### Counting-process martingale

↑ **Parent:** [Compensator of a counting process](#compensator-of-a-counting-process)

If a [counting process](#counting-process) $N$ has predictable conditional intensity $\lambda$, subtracting its [compensator of a counting process](#compensator-of-a-counting-process) gives the associated martingale $M$. Conditional expected event increments and compensator increments agree, so their difference is conditionally centered. With the necessary integrability, $M$ is a mean-zero [martingale](martingale.md); for a simple no-ties process its predictable quadratic variation is $\int_0^t\lambda(u)du$. A predictable weighted martingale integral has mean zero and variance determined by the square of its weights. In [survival analysis](survival-analysis.md), $\lambda=Yh$ produces the event-minus-expected representation used to derive the [Nelson–Aalen estimator](survival-analysis.md#nelson-aalen-estimator).

## Brownian motion

↑ **Parent:** [Stochastic process](stochastic-process.md)

[This section is present in another page, follow this link to view it.](brownian-motion.md)

## ↑ Ancestors (5)

1. [Probability theory](probability-theory.md)
2. [Probability and statistics](probability-and-statistics.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (47)

- [Almost sure path regularity does not ensure progressive measurability](#almost-sure-path-regularity-does-not-ensure-progressive-measurability)
- [Bounded increments](#bounded-increments)
- [Branching process](#branching-process)
- [Brownian bridge independence from its endpoint](brownian-motion.md#brownian-bridge-independence-from-its-endpoint)
- [Càdlàg modification](#cadlag-modification)
- [Càdlàg versions are indistinguishable](#cadlag-versions-are-indistinguishable)
- [Continuity of Lévy characteristic functions](#continuity-of-levy-characteristic-functions)
- [Continuous modification](#continuous-modification)
- [Correlation time](time-series.md#correlation-time)
- [Covariance function](#covariance-function)
- [Dyadic increment chaining](#dyadic-increment-chaining)
- [Finite-dimensional distribution](#finite-dimensional-distribution)
- [Fluid limit](queueing-theory.md#fluid-limit)
- [Gaussian process](#gaussian-process)
- [Interacting particle system](#interacting-particle-system)
- [Kolmogorov continuity theorem](#kolmogorov-continuity-theorem)
- [Laplace transform of symmetric Brownian interval-exit time](brownian-motion.md#laplace-transform-of-symmetric-brownian-interval-exit-time)
- [Local time (mathematics)](stochastic-calculus.md#local-time-mathematics)
- [Markov process](markov-process.md)
- [Measurability](measure-theory.md#measurability)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-28.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-34.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-34.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-24.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-24.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-24.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-24.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-24.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-24.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-29.md#6/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-201.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-201.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-201.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-201.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-202.md#5/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#6/ii/solution)
- [Path probability](#path-probability)
- [Sample path](#sample-path)
- [Spot volatility](mathematical-finance.md#spot-volatility)
- [Stock](mathematical-finance.md#stock)
- [Stopped process](martingale.md#stopped-process)
