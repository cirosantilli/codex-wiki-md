# Relativistic quantum field

↑ **Parent:** [Quantum field theory](quantum-field-theory.md)

**Table of contents**

- [Microcausality](#microcausality)
  - [Antiparticle modes and spacelike commutativity](#antiparticle-modes-and-spacelike-commutativity)
- [Massive spin-two field](#massive-spin-two-field)
  - [Light-cone decomposition of a massive spin-two field](#light-cone-decomposition-of-a-massive-spin-two-field)
- [Decay width](#decay-width)
  - [Branching fraction](#branching-fraction)
  - [Decay amplitude](#decay-amplitude)
    - [Absorptive phase of a decay amplitude](#absorptive-phase-of-a-decay-amplitude)
  - [Massive-vector spin average](#massive-vector-spin-average)
  - [Massless semileptonic pseudoscalar decay rate](#massless-semileptonic-pseudoscalar-decay-rate)
  - [Lorentz-invariant phase space](#lorentz-invariant-phase-space)
    - [Two-body Lorentz-invariant phase space](#two-body-lorentz-invariant-phase-space)
      - [Massless two-body scattering flux normalization](#massless-two-body-scattering-flux-normalization)
- [Polarization vector](#polarization-vector)
  - [Longitudinal polarization of a massive vector boson](#longitudinal-polarization-of-a-massive-vector-boson)
  - [Photon polarization completeness relation](#photon-polarization-completeness-relation)
  - [Polarization sum for a massive vector boson](#polarization-sum-for-a-massive-vector-boson)
  - [Timelike photon polarization](#timelike-photon-polarization)
- [Fierz-Pauli equations](#fierz-pauli-equations)
- [Dirac field](#dirac-field)
  - [Dirac fermion number conservation](#dirac-fermion-number-conservation)
  - [Fermion bilinear](#fermion-bilinear)
    - [Vector current](#vector-current)
  - [Mode expansion of a Dirac field](#mode-expansion-of-a-dirac-field)
    - [Particle and antiparticle occupation operators of a Dirac field](#particle-and-antiparticle-occupation-operators-of-a-dirac-field)
    - [Antiparticle](#antiparticle)
      - [Annihilation](#annihilation)
      - [Antimatter](#antimatter)
      - [Dirac sea](#dirac-sea)
    - [Fermionic annihilation operator](#fermionic-annihilation-operator)
    - [Fermionic creation operator](#fermionic-creation-operator)
  - [Dirac equation](#dirac-equation)
    - [Flat-space Dirac factorization](#flat-space-dirac-factorization)
    - [Lichnerowicz spinor-square formula](#lichnerowicz-spinor-square-formula)
      - [Riemann tensor Clifford contraction](#riemann-tensor-clifford-contraction)
      - [Torsion correction to the Dirac square](#torsion-correction-to-the-dirac-square)
      - [Compact harmonic-spinor rigidity under nonnegative scalar curvature](#compact-harmonic-spinor-rigidity-under-nonnegative-scalar-curvature)
        - [Riemannian parallel-spinor Ricci-flatness](#riemannian-parallel-spinor-ricci-flatness)
    - [Lorentz covariance of the Dirac operator](#lorentz-covariance-of-the-dirac-operator)
    - [Adjoint Dirac equation](#adjoint-dirac-equation)
    - [Massless Dirac equation](#massless-dirac-equation)
    - [Mostly-plus Dirac convention](#mostly-plus-dirac-convention)
  - [Dirac adjoint](#dirac-adjoint)
    - [Dirac scalar bilinear](#dirac-scalar-bilinear)
  - [Dirac action](#dirac-action)
  - [Fermion spin sum](#fermion-spin-sum)
  - [Weyl spinor](#weyl-spinor)
    - [Weyl field](#weyl-field)
    - [Weyl sigma matrices](#weyl-sigma-matrices)
    - [Helicity content of a quantized Weyl field](#helicity-content-of-a-quantized-weyl-field)
    - [Left-handed massless plane-wave spinor](#left-handed-massless-plane-wave-spinor)
    - [Opposite Weyl boost generators](#opposite-weyl-boost-generators)
    - [Weyl spinor bilinear exchange identity](#weyl-spinor-bilinear-exchange-identity)
      - [Square of a Weyl spinor bilinear](#square-of-a-weyl-spinor-bilinear)
    - [Chirality (physics)](#chirality-physics)
      - [Chiral projector](#chiral-projector)
        - [Chiral fermion trace contraction](#chiral-fermion-trace-contraction)
      - [Vectorlike gauge spectrum](#vectorlike-gauge-spectrum)
      - [Chiral gauge spectrum](#chiral-gauge-spectrum)
    - [Weyl representation of the gamma matrices](#weyl-representation-of-the-gamma-matrices)
    - [Majorana spinor](#majorana-spinor)
      - [Four-dimensional Majorana bilinear vanishing criterion](#four-dimensional-majorana-bilinear-vanishing-criterion)
      - [Four-dimensional Majorana bilinear interchange](#four-dimensional-majorana-bilinear-interchange)
      - [Majorana-Weyl spinor](#majorana-weyl-spinor)
      - [Majorana Grassmann bilinear interchange](#majorana-grassmann-bilinear-interchange)
      - [Majorana mass term](#majorana-mass-term)
        - [Grassmann variation of a chiral Majorana mass term](#grassmann-variation-of-a-chiral-majorana-mass-term)
  - [Dirac spinor](#dirac-spinor)
    - [Dirac plane waves in the standard representation](#dirac-plane-waves-in-the-standard-representation)
    - [Massless limit of a transverse canonical-spin label](#massless-limit-of-a-transverse-canonical-spin-label)
    - [Hermitian square-root construction of Dirac plane waves](#hermitian-square-root-construction-of-dirac-plane-waves)
    - [Euclidean adjoint Dirac Feynman rules](#euclidean-adjoint-dirac-feynman-rules)
    - [Spinor representation of the Lorentz group](#spinor-representation-of-the-lorentz-group)
      - [Spinor Lorentz generator commutator](#spinor-lorentz-generator-commutator)
      - [Even-dimensional Clifford spinor dimension](#even-dimensional-clifford-spinor-dimension)
      - [Rarita-Schwinger field](#rarita-schwinger-field)
        - [Gamma trace of a vector-spinor](#gamma-trace-of-a-vector-spinor)
        - [Massless Rarita-Schwinger polarization count](#massless-rarita-schwinger-polarization-count)
        - [Massive Rarita-Schwinger constraints](#massive-rarita-schwinger-constraints)
      - [Inverse Lorentz action on gamma matrices](#inverse-lorentz-action-on-gamma-matrices)
      - [Dirac spinor pseudo-unitarity](#dirac-spinor-pseudo-unitarity)
      - [Lorentz-spinor generators from a Clifford algebra](#lorentz-spinor-generators-from-a-clifford-algebra)
      - [Pseudo-unitarity of the spinor Lorentz representation](#pseudo-unitarity-of-the-spinor-lorentz-representation)
      - [Infinitesimal transformation of a Dirac field](#infinitesimal-transformation-of-a-dirac-field)
      - [Spinor sign under a full spatial rotation](#spinor-sign-under-a-full-spatial-rotation)
      - [Lorentz generator from gamma-matrix commutators](#lorentz-generator-from-gamma-matrix-commutators)
    - [Dirac mass term](#dirac-mass-term)
  - [Spin sum](#spin-sum)
    - [Spin average](#spin-average)
    - [Gamma-matrix trace](#gamma-matrix-trace)
- [Gauge field](#gauge-field)
  - [Chern-Simons 5-form](#chern-simons-5-form)
    - [Abelian Chern-Simons five-form field equation](#abelian-chern-simons-five-form-field-equation)
    - [Variation of the Chern-Simons 5-form](#variation-of-the-chern-simons-5-form)
  - [CP transformation of a non-Abelian gauge connection](#cp-transformation-of-a-non-abelian-gauge-connection)
  - [Abelian p-form gauge field](#abelian-p-form-gauge-field)
    - [Massive p-form field](#massive-p-form-field)
      - [Stueckelberg mechanism](#stueckelberg-mechanism)
      - [Massive p-form duality](#massive-p-form-duality)
    - [Massless p-form gauge field](#massless-p-form-gauge-field)
      - [Massless p-form duality](#massless-p-form-duality)
      - [Nondynamical four-dimensional three-form](#nondynamical-four-dimensional-three-form)
      - [Two-form scalar duality](#two-form-scalar-duality)
    - [Bianchi identity for an Abelian p-form](#bianchi-identity-for-an-abelian-p-form)
  - [Two-form gauge field](#two-form-gauge-field)
    - [Gauge-invariant string coupling to a two-form](#gauge-invariant-string-coupling-to-a-two-form)
  - [Gauss law constraint in gauge theory](#gauss-law-constraint-in-gauge-theory)
  - [Gauge boson](#gauge-boson)
    - [Gauge-boson mass matrix](#gauge-boson-mass-matrix)
      - [Gauge-boson mass rank from a real scalar vacuum](#gauge-boson-mass-rank-from-a-real-scalar-vacuum)
  - [Gauge group](#gauge-group)
    - [Gauge generator](#gauge-generator)
    - [Gauge group representation](#gauge-group-representation)
  - [Gauge coupling](#gauge-coupling)
    - [Canonical normalization of a gauge kinetic term](#canonical-normalization-of-a-gauge-kinetic-term)
  - [Wilson line](#wilson-line)
    - [Wilson loop](#wilson-loop)
    - [Wilson-line gauge transformation](#wilson-line-gauge-transformation)
  - [Gauge-field transformation law](#gauge-field-transformation-law)
  - [Gauge field strength](#gauge-field-strength)
    - [Spinor decomposition of gauge curvature](#spinor-decomposition-of-gauge-curvature)
    - [Cross-product convention for an adjoint covariant derivative](#cross-product-convention-for-an-adjoint-covariant-derivative)
    - [CP transformation of non-Abelian field strength](#cp-transformation-of-non-abelian-field-strength)
    - [Scaled right Maurer-Cartan gauge potential](#scaled-right-maurer-cartan-gauge-potential)
      - [Circular curvature zeros for a planar SU2 exponential](#circular-curvature-zeros-for-a-planar-su2-exponential)
    - [Pure gauge potential](#pure-gauge-potential)
    - [Gauge-theory Bianchi identity](#gauge-theory-bianchi-identity)
  - [Flat connection](#flat-connection)
    - [Parallel-frame compatibility criterion](#parallel-frame-compatibility-criterion)
    - [Holonomy representation of a flat connection](#holonomy-representation-of-a-flat-connection)
    - [Framed flat connections and holonomy](#framed-flat-connections-and-holonomy)
  - [Gauge covariant derivative](#gauge-covariant-derivative)
    - [Invariant integration by parts for a gauge covariant derivative](#invariant-integration-by-parts-for-a-gauge-covariant-derivative)
    - [Conjugate gauge covariant derivative](#conjugate-gauge-covariant-derivative)
    - [Gauge covariance of a scalar covariant derivative](#gauge-covariance-of-a-scalar-covariant-derivative)
    - [Adjoint covariant derivative](#adjoint-covariant-derivative)
      - [Adjoint gauge variation for a positive-sign covariant derivative](#adjoint-gauge-variation-for-a-positive-sign-covariant-derivative)
      - [Gauge-covariant integration by parts](#gauge-covariant-integration-by-parts)
  - [Gauge invariance](#gauge-invariance)
    - [Symmetry up to gauge transformation](#symmetry-up-to-gauge-transformation)
    - [Gauge-invariant operator](#gauge-invariant-operator)
    - [Gauge redundancy](#gauge-redundancy)
    - [Gauge orbit](#gauge-orbit)
  - [Abelian gauge theory](#abelian-gauge-theory)
    - [U(1) gauge symmetry](#u-1-gauge-symmetry)
      - [Scalar electrodynamics](#scalar-electrodynamics)
        - [Two-charge scalar gauge potential](#two-charge-scalar-gauge-potential)
      - [Large gauge transformation](#large-gauge-transformation)
  - [Yang-Mills theory](#yang-mills-theory)
    - [Invariant bilinear-form construction of a Yang-Mills action](#invariant-bilinear-form-construction-of-a-yang-mills-action)
    - [Theta vacuum](#theta-vacuum)
      - [Yang-Mills theta term](#yang-mills-theta-term)
        - [Boundary variation of the Yang-Mills theta term](#boundary-variation-of-the-yang-mills-theta-term)
        - [CP parity of the Yang-Mills theta density](#cp-parity-of-the-yang-mills-theta-density)
        - [QCD theta angle](#qcd-theta-angle)
          - [Strong CP problem](#strong-cp-problem)
            - [Peccei–Quinn theory](#peccei-quinn-theory)
              - [Axion](#axion)
        - [Electroweak theta angle](#electroweak-theta-angle)
        - [Chern-Simons current](#chern-simons-current)
    - [Cubic and quartic Yang-Mills self-interactions](#cubic-and-quartic-yang-mills-self-interactions)
    - [Yang-Mills vacuum](#yang-mills-vacuum)
    - [Invariant gauge kinetic form](#invariant-gauge-kinetic-form)
    - [Non-Abelian gauge transformation](#non-abelian-gauge-transformation)
    - [Yang-Mills equations](#yang-mills-equations)
      - [Covariant wave equation for the Yang-Mills field strength](#covariant-wave-equation-for-the-yang-mills-field-strength)
    - [Yang-Mills theory coupled to an arbitrary scalar representation](#yang-mills-theory-coupled-to-an-arbitrary-scalar-representation)
      - [Adjoint Yang-Mills-Higgs trace variation](#adjoint-yang-mills-higgs-trace-variation)
      - [Gauge-invariant scalar potential](#gauge-invariant-scalar-potential)
    - [Killing-form Yang-Mills Lagrangian](#killing-form-yang-mills-lagrangian)
    - [Killing-form Lagrangian for an adjoint scalar](#killing-form-lagrangian-for-an-adjoint-scalar)
    - [SU(2) gauge theory](#su-2-gauge-theory)
      - [SU2 gauge self-interaction vertices](#su2-gauge-self-interaction-vertices)
      - [Complete breaking by an SU2 scalar doublet](#complete-breaking-by-an-su2-scalar-doublet)
        - [Scalar interactions after complete SU2 breaking](#scalar-interactions-after-complete-su2-breaking)
      - [SU(2) gauge theory with an adjoint Higgs field](#su-2-gauge-theory-with-an-adjoint-higgs-field)
        - ['t Hooft electromagnetic tensor](#t-hooft-electromagnetic-tensor)
        - [Physical charged-vector Lagrangian for an adjoint SU2 Higgs model](#physical-charged-vector-lagrangian-for-an-adjoint-su2-higgs-model)
          - [Scalar vertices of an adjoint triplet Higgs model](#scalar-vertices-of-an-adjoint-triplet-higgs-model)
    - [SU(3) gauge theory](#su-3-gauge-theory)
      - [Fundamental-Higgs breaking of SU(3) to SU(2)](#fundamental-higgs-breaking-of-su-3-to-su-2)
    - [Yang-Mills action](#yang-mills-action)
      - [Conformal invariance of four-dimensional Yang-Mills action](#conformal-invariance-of-four-dimensional-yang-mills-action)
      - [Derivative-squared Yang-Mills action](#derivative-squared-yang-mills-action)
      - [Power of the Yang-Mills invariant](#power-of-the-yang-mills-invariant)
    - [Yang-Mills gauge transformation](#yang-mills-gauge-transformation)
      - [Gauge transformation in the derivative-plus-connection convention](#gauge-transformation-in-the-derivative-plus-connection-convention)
      - [Infinitesimal gauge transformation with an anti-Hermitian connection](#infinitesimal-gauge-transformation-with-an-anti-hermitian-connection)
    - [Gluon propagator](#gluon-propagator)
    - [Anomaly (physics)](#anomaly-physics)
      - [Global anomaly](#global-anomaly)
        - [Witten SU(2) anomaly](#witten-su-2-anomaly)
      - [Gauge anomaly](#gauge-anomaly)
        - [Anomaly cancellation](#anomaly-cancellation)
          - [Standard Model anomaly cancellation](#standard-model-anomaly-cancellation)
            - [One-generation hypercharge anomaly traces](#one-generation-hypercharge-anomaly-traces)
        - [Mixed gauge-gravitational anomaly](#mixed-gauge-gravitational-anomaly)
      - [Chiral anomaly](#chiral-anomaly)
        - [Axial current](#axial-current)
          - [Axial charge](#axial-charge)
          - [Axial derivative coupling and parity](#axial-derivative-coupling-and-parity)
          - [Axial-current divergence for scalar and pseudoscalar backgrounds](#axial-current-divergence-for-scalar-and-pseudoscalar-backgrounds)
          - [Axial-current divergence for a pseudoscalar Yukawa interaction](#axial-current-divergence-for-a-pseudoscalar-yukawa-interaction)
          - [Axial-current squared interaction](#axial-current-squared-interaction)
          - [Chiral transformation](#chiral-transformation)
      - ['t Hooft anomaly](#t-hooft-anomaly)
        - ['t Hooft anomaly matching](#t-hooft-anomaly-matching)
  - [Gauge fixing](#gauge-fixing)
    - [R-xi gauge](#r-xi-gauge)
    - [Regular gauge slice](#regular-gauge-slice)
    - [Light cone gauge](#light-cone-gauge)
    - [Gauge-fixed action](#gauge-fixed-action)
    - [Dynamical gauge-fixing parameter](#dynamical-gauge-fixing-parameter)
    - [Nonlinear Abelian gauge fixing](#nonlinear-abelian-gauge-fixing)
      - [Quadratic Abelian gauge fixing](#quadratic-abelian-gauge-fixing)
      - [Complex quadratic Abelian gauge condition](#complex-quadratic-abelian-gauge-condition)
        - [Ghost-scalar determinant cancellation in a complex quadratic gauge](#ghost-scalar-determinant-cancellation-in-a-complex-quadratic-gauge)
        - [Reality obstruction for a complex Euclidean gauge condition](#reality-obstruction-for-a-complex-euclidean-gauge-condition)
    - [Scalar-dependent gauge fixing](#scalar-dependent-gauge-fixing)
      - [Ghost vertex in scalar-dependent gauge fixing](#ghost-vertex-in-scalar-dependent-gauge-fixing)
      - [Free adjoint-scalar propagator in scalar-dependent gauge fixing](#free-adjoint-scalar-propagator-in-scalar-dependent-gauge-fixing)
    - [Zero mode in field theory](#zero-mode-in-field-theory)
      - [Zero mode of a radiation-era massless scalar](#zero-mode-of-a-radiation-era-massless-scalar)
    - [Gribov ambiguity](#gribov-ambiguity)
    - [Covariant gauge](#covariant-gauge)
      - [Gauge-fixed Maxwell kinetic operator](#gauge-fixed-maxwell-kinetic-operator)
      - [Landau gauge (quantum field theory)](#landau-gauge-quantum-field-theory)
        - [Landau gauge photon propagator](#landau-gauge-photon-propagator)
      - [Gauge-fixed Yang-Mills Lagrangian in a covariant gauge](#gauge-fixed-yang-mills-lagrangian-in-a-covariant-gauge)
      - [Inversion of the gauge-fixed Maxwell kinetic operator](#inversion-of-the-gauge-fixed-maxwell-kinetic-operator)
      - [Positive-sign covariant gauge-fixing inverse](#positive-sign-covariant-gauge-fixing-inverse)
        - [Longitudinal gauge propagator contraction](#longitudinal-gauge-propagator-contraction)
      - [Feynman gauge](#feynman-gauge)
        - [Feynman-gauge Maxwell kinetic density after a boundary-term subtraction](#feynman-gauge-maxwell-kinetic-density-after-a-boundary-term-subtraction)
          - [Boundary-induced canonical transformation in Feynman gauge](#boundary-induced-canonical-transformation-in-feynman-gauge)
        - [Gupta-Bleuler formalism](#gupta-bleuler-formalism)
          - [Gupta-Bleuler null-state quotient](#gupta-bleuler-null-state-quotient)
            - [Transverse one-photon physical quotient](#transverse-one-photon-physical-quotient)
          - [Covariant photon Fock space](#covariant-photon-fock-space)
            - [Photon oscillator completeness and canonical brackets](#photon-oscillator-completeness-and-canonical-brackets)
            - [Negative-norm photon state](#negative-norm-photon-state)
      - [Gauge-boson propagator](#gauge-boson-propagator)
        - [Feynman-gauge adjoint propagator](#feynman-gauge-adjoint-propagator)
        - [Feynman-gauge photon propagator](#feynman-gauge-photon-propagator)
        - [Transverse projector of a vector field](#transverse-projector-of-a-vector-field)
        - [Longitudinal projector of a vector field](#longitudinal-projector-of-a-vector-field)
    - [Faddeev-Popov determinant](#faddeev-popov-determinant)
      - [Faddeev-Popov gauge-orbit identity](#faddeev-popov-gauge-orbit-identity)
        - [Finite-dimensional Faddeev-Popov gauge reduction](#finite-dimensional-faddeev-popov-gauge-reduction)
      - [Faddeev-Popov operator](#faddeev-popov-operator)
      - [Faddeev-Popov ghost](#faddeev-popov-ghost)
        - [Ghost propagator](#ghost-propagator)
        - [Ghost propagator for a negative derivative kinetic term](#ghost-propagator-for-a-negative-derivative-kinetic-term)
        - [Ghost-gluon vertex](#ghost-gluon-vertex)
          - [One-loop ghost kinetic counterterm in Feynman gauge](#one-loop-ghost-kinetic-counterterm-in-feynman-gauge)
        - [Faddeev-Popov antighost field](#faddeev-popov-antighost-field)
        - [Ghost number](#ghost-number)
          - [Ghost-number Noether current](#ghost-number-noether-current)
        - [Ghost loop](#ghost-loop)
    - [Axial gauge](#axial-gauge)
      - [Axial-gauge pole prescription](#axial-gauge-pole-prescription)
      - [Axial-gauge propagator](#axial-gauge-propagator)
    - [Temporal gauge](#temporal-gauge)
    - [BRST symmetry](#brst-symmetry)
      - [Grassmann-valued SU(2) adjoint bracket](#grassmann-valued-su-2-adjoint-bracket)
      - [BRST quantization](#brst-quantization)
        - [Point-particle Faddeev–Popov ghost action](#point-particle-faddeev-popov-ghost-action)
      - [BRST nilpotence](#brst-nilpotence)
        - [Off-shell nilpotence of the Yang-Mills BRST quartet](#off-shell-nilpotence-of-the-yang-mills-brst-quartet)
      - [Left-acting BRST differential](#left-acting-brst-differential)
      - [Right-acting BRST differential](#right-acting-brst-differential)
      - [Nakanishi-Lautrup field](#nakanishi-lautrup-field)
        - [Gaussian gauge fixing with an auxiliary field](#gaussian-gauge-fixing-with-an-auxiliary-field)
      - [BRST charge](#brst-charge)
        - [A Hermitian nilpotent BRST charge requires an indefinite auxiliary space](#a-hermitian-nilpotent-brst-charge-requires-an-indefinite-auxiliary-space)
        - [Particle BRST charge and Klein–Gordon constraint](#particle-brst-charge-and-klein-gordon-constraint)
        - [BRST current in derivative-b gauge fixing](#brst-current-in-derivative-b-gauge-fixing)
        - [Yang-Mills BRST Noether current](#yang-mills-brst-noether-current)
        - [BRST Ward identity](#brst-ward-identity)
          - [Gauge-fixing parameter independence from BRST symmetry](#gauge-fixing-parameter-independence-from-brst-symmetry)
            - [Gauge-condition independence of BRST-closed correlation functions](#gauge-condition-independence-of-brst-closed-correlation-functions)
          - [Graded BRST Ward identity](#graded-brst-ward-identity)
      - [Gauge-fixing fermion](#gauge-fixing-fermion)
        - [BRST-exact covariant gauge fixing](#brst-exact-covariant-gauge-fixing)
        - [Covariant gauge-fixing density as a BRST variation](#covariant-gauge-fixing-density-as-a-brst-variation)
        - [Derivative-antighost gauge-fixing fermion](#derivative-antighost-gauge-fixing-fermion)
      - [BRST cohomology](#brst-cohomology)
        - [Positive one-particle BRST cohomology](#positive-one-particle-brst-cohomology)
        - [BRST-closed operator](#brst-closed-operator)
        - [BRST-exact operator](#brst-exact-operator)
          - [BRST-exact insertions in physical correlation functions](#brst-exact-insertions-in-physical-correlation-functions)

## Microcausality

↑ **Parent:** [Relativistic quantum field](relativistic-quantum-field.md)

[Microcausality](#microcausality) requires local bosonic observables at spacelike separation to commute. For a free [real scalar field](scalar-field-theory.md#real-scalar-field), the field [commutator](lie-algebra.md#commutator) is the difference of its two [Wightman functions](quantum-field-theory.md#wightman-function); it vanishes at equal time and, by [Lorentz invariance](special-relativity.md#lorentz-invariance), at every spacelike separation. Nonzero spacelike vacuum correlations do not violate this condition, since a correlation is different from the response to a local intervention. Odd fermionic fields satisfy a corresponding spacelike anticommutation condition, while physical even local observables commute.

### Antiparticle modes and spacelike commutativity

↑ **Parent:** [Microcausality](#microcausality)

For a free [complex scalar field](scalar-field-theory.md#complex-scalar-field), independent particle annihilators and [antiparticle](#antiparticle) creators give

$$
[\Phi(x),\Phi^\dagger(y)]=\int\frac{d^3p}{(2\pi)^3\,2E_p}\left(e^{-ip(x-y)}-e^{ip(x-y)}\right).
$$

The invariant [mass shell](special-relativity.md#mass-shell) integral vanishes at spacelike separation: transform to equal time, then reverse the spatial momentum in one term. Retaining only the particle-annihilation term would leave a [Wightman function](quantum-field-theory.md#wightman-function), which is generally nonzero even at spacelike separation. Thus both frequency branches are needed for a local relativistic field. For a [real scalar field](scalar-field-theory.md#real-scalar-field), the creation term supplies the same cancellation but creates the same self-conjugate particle species.

## Massive spin-two field

↑ **Parent:** [Relativistic quantum field](relativistic-quantum-field.md)

A free massive spin-two field is a [symmetric tensor](linear-algebra.md#symmetric-tensor) obeying a massive [Klein-Gordon equation](wave-equation.md#klein-gordon-equation), vanishing divergence, and vanishing [trace](linear-algebra.md#matrix-trace). Its rest-frame polarizations form the [symmetric traceless square](linear-algebra.md#symmetric-trace-free-square-of-the-defining-orthogonal-representation) of the $SO(D-1)$ vector, with $(D-2)(D+1)/2$ degrees of freedom.

### Light-cone decomposition of a massive spin-two field

↑ **Parent:** [Massive spin-two field](#massive-spin-two-field)

When $\partial_-$ is invertible, divergence determines components with a plus index from $h_{--},h_{-I},h_{IJ}$. The [trace](linear-algebra.md#matrix-trace) constraint fixes the [trace](linear-algebra.md#matrix-trace) of $h_{IJ}$. The remaining transverse [group representations](representation-theory.md#group-representation) are a [symmetric traceless square](linear-algebra.md#symmetric-trace-free-square-of-the-defining-orthogonal-representation), a [vector representation](representation-theory.md#vector-representation), and a scalar.

## Decay width

↑ **Parent:** [Relativistic quantum field](relativistic-quantum-field.md)

In units with $\hbar=1$, the inverse lifetime of an unstable particle. A [neutral meson mixing](physics.md#neutral-meson-mixing) effective [Hamiltonian operator](quantum-mechanics.md#hamiltonian-quantum-mechanics) incorporates decay through its anti-Hermitian part $-i\Gamma/2$.

### Branching fraction

↑ **Parent:** [Decay width](#decay-width)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Branching_fraction)

A [branching fraction](#branching-fraction) is the probability that a decay occurs through a particular mutually exclusive channel, equal to its partial [decay width](#decay-width) divided by the total [decay width](#decay-width). Inclusive channel fractions sum to one. Rounding displayed fractions can make their numerical sum differ from one.

### Decay amplitude

↑ **Parent:** [Decay width](#decay-width)

The invariant decay amplitude is the transition matrix element for one incoming particle and a specified on-shell final state, with the overall momentum delta function factored out. For covariantly normalized states, write the connected [S-matrix](quantum-mechanics.md#s-matrix) element as $i(2\pi)^4\delta^4(p_i-p_f)\mathcal M(i\to f)$. Its overall phase does not affect the [decay width](#decay-width). The rate is $\Gamma=(2M_i)^{-1}\sum_{\rm spins}\int d\Phi_f|\mathcal M|^2$, with the initial spin average included when the initial state is unpolarized. For a spin-zero parent and an angle-independent two-body amplitude, the [two-body Lorentz-invariant phase space](#two-body-lorentz-invariant-phase-space) gives $\Gamma=|\mathbf k|\sum|\mathcal M|^2/(8\pi M_i^2)$. In [leptonic pion decay](standard-model.md#leptonic-pion-decay), contracting the axial hadronic matrix element with the chiral [weak charged current](standard-model.md#charged-current) makes this amplitude proportional to the charged-lepton mass, proving [helicity suppression](standard-model.md#helicity-suppression).

#### Absorptive phase of a decay amplitude

↑ **Parent:** [Decay amplitude](#decay-amplitude)

An [absorptive phase](#absorptive-phase-of-a-decay-amplitude) arises from physical intermediate states or rescattering in a [decay amplitude](#decay-amplitude). For a pair of [CP symmetry](quantum-field-theory.md#cp-symmetry) conjugate reactions with otherwise symmetric dynamics, this phase is the same in both amplitudes, whereas a [weak phase](quantum-field-theory.md#weak-phase-cp-violation) changes sign. Their differing transformation laws allow interference to produce a [direct CP asymmetry](quantum-field-theory.md#direct-cp-asymmetry).

### Massive-vector spin average

↑ **Parent:** [Decay width](#decay-width)

An unpolarized decay of a massive [spin](quantum-mechanics.md#spin)-one particle averages the squared amplitude over three parent [spin](quantum-mechanics.md#spin) states. Its polarization sum is $-\eta_{\mu\nu}+p_\mu p_\nu/m^2$. For a conserved external current the longitudinal $p_\mu p_\nu$ term drops out, but this does not replace the [spin](quantum-mechanics.md#spin) average by $1/2$: the physical massive parent still has three states.

### Massless semileptonic pseudoscalar decay rate

↑ **Parent:** [Decay width](#decay-width)

For a [pseudoscalar meson](physics.md#pseudoscalar-meson) of mass $M$ decaying into a [pseudoscalar meson](physics.md#pseudoscalar-meson) of mass $m$ and two massless leptons through a [weak charged current](standard-model.md#charged-current), the [transverse massless leptonic current](standard-model.md#transverse-massless-leptonic-current) selects $f_+(s)$. With hadronic current normalized as $(p+k)^\mu f_+(s)+(p-k)^\mu f_-(s)$ and flavour coefficient $V$,

$$
\frac{d\Gamma}{ds}=\frac{G_F^2|V|^2}{192\pi^3M^3}\lambda(s,M^2,m^2)^{3/2}|f_+(s)|^2,\qquad 0\leq s\leq(M-m)^2.
$$

The [Källén function](special-relativity.md#kallen-function) has mass dimension four, and the coefficient has mass dimension $-7$. This [decay rate](#decay-width) assumes the stated form-factor normalization and no additional isospin factor. It follows by the [integrated massless leptonic tensor](standard-model.md#integrated-massless-leptonic-tensor) and the pion momentum change of variable in the parent's [centre-of-momentum frame](special-relativity.md#center-of-momentum-frame).

### Lorentz-invariant phase space

↑ **Parent:** [Decay width](#decay-width)

For two outgoing particles the [Lorentz-invariant phase space](#lorentz-invariant-phase-space) is $d\Phi_2=(2\pi)^4\delta^{(4)}(p-k-k')\,d^3k/((2\pi)^32E_k)\,d^3k'/((2\pi)^32E_{k'})$. With massless daughters in their center-of-mass frame, $d\Phi_2=d\Omega/(32\pi^2)$ and $\int d\Phi_2=1/(8\pi)$. This fixes normalization factors in [decay widths](#decay-width) and scattering rates.

#### Two-body Lorentz-invariant phase space

↑ **Parent:** [Lorentz-invariant phase space](#lorentz-invariant-phase-space)

For two distinct massless final particles in their centre-of-momentum frame, integrating the energy-momentum delta function gives $d\Phi_2=d\Omega/(32\pi^2)$. A massless two-particle initial state has flux $2s$, hence $d\sigma/d\cos\theta=\overline{|\mathcal M|^2}/(32\pi s)$. Average only over the initial spin states physically present.

##### Massless two-body scattering flux normalization

↑ **Parent:** [Two-body Lorentz-invariant phase space](#two-body-lorentz-invariant-phase-space)

For two distinct massless final particles, $d\Phi_2/d\Omega=1/(32\pi^2)$ in the centre-of-mass frame. The invariant initial flux is $4p_1\cdot p_2=2s$. Their ratio gives the displayed differential cross-section. Equivalently the denominator is $128\pi^2p_1\cdot p_2$. Initial spins are averaged and final spins and colors summed when defining an inclusive unpolarized cross-section; averaging final colors would change the observable.

## Polarization vector

↑ **Parent:** [Relativistic quantum field](relativistic-quantum-field.md)

A [Lorentz four-vector](special-relativity.md#four-vector) coefficient selecting a spin-one polarization in a [mode expansion of a free field](quantum-field-theory.md#mode-expansion-of-a-free-field). Its allowed components depend on the field equations and [gauge fixing](#gauge-fixing).

### Longitudinal polarization of a massive vector boson

↑ **Parent:** [Polarization vector](#polarization-vector)

A physical polarization of a massive spin-one [gauge boson](#gauge-boson) whose spatial polarization points along its spatial momentum. Together with two transverse polarizations it supplies the three physical spin states. In the [Higgs mechanism](standard-model.md#higgs-mechanism), a broken-direction [Goldstone boson](critical-phenomenon.md#goldstone-boson) supplies this extra state as the [gauge boson](#gauge-boson) acquires mass.

### Photon polarization completeness relation

↑ **Parent:** [Polarization vector](#polarization-vector)

Two orthonormal transverse [polarization vectors](#polarization-vector) span the plane perpendicular to a nonzero momentum. Summing their dyadic products gives the spatial transverse projector. It has trace and rank two and acts as the identity on physical [photon](quantum-mechanics.md#photon) polarizations.

### Polarization sum for a massive vector boson

↑ **Parent:** [Polarization vector](#polarization-vector)

For $m>0$, the three physical [polarization vectors](#polarization-vector) are transverse to $k$ and have norm $-1$ in metric $(+---)$. In the rest frame their sum is $\operatorname{diag}(0,1,1,1)$; [Lorentz covariance](special-relativity.md#lorentz-covariance) then gives the displayed expression for $k^2=m^2$. This includes the longitudinal mode. It cannot be specialized to $m=0$ by setting its denominator to zero.

### Timelike photon polarization

↑ **Parent:** [Polarization vector](#polarization-vector)

A timelike basis polarization in covariant photon quantization has positive [Minkowski metric](special-relativity.md#minkowski-metric) squared length, conventionally $\epsilon^{0\mu}=(1,\mathbf0)$ with signature $(+,-,-,-)$. It is distinct from the spatial [longitudinal polarization](wave-equation.md#longitudinal-polarization) $\epsilon^{3\mu}=(0,\widehat{\mathbf p})$. The extra minus sign in the covariant oscillator [commutator](lie-algebra.md#commutator) makes its one-photon state a [negative-norm photon state](#negative-norm-photon-state). Neither this temporal polarization nor an isolated longitudinal photon survives the [Gupta-Bleuler null-state quotient](#gupta-bleuler-null-state-quotient).

## Fierz-Pauli equations

↑ **Parent:** [Relativistic quantum field](relativistic-quantum-field.md)

The Fierz-Pauli equations describe a free massive spin-two field. A symmetric tensor $h_{\mu\nu}$ obeys the Klein-Gordon equation together with $\partial^\mu h_{\mu\nu}=0$ and $h^\mu{}_{\mu}=0$, leaving five propagating polarizations in four dimensions.

## Dirac field

↑ **Parent:** [Relativistic quantum field](relativistic-quantum-field.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dirac_field)

A free Dirac field has Lagrangian density $\mathcal L=i\bar\psi\gamma^\mu\partial_\mu\psi-m\bar\psi\psi$ and obeys the [Dirac equation](#dirac-equation).

### Dirac fermion number conservation

↑ **Parent:** [Dirac field](#dirac-field)

A [Dirac field](#dirac-field) theory invariant under $\psi\mapsto e^{i\alpha}\psi$, $\bar\psi\mapsto e^{-i\alpha}\bar\psi$ has a conserved global charge, subject to the quantum theory preserving the [symmetry](physics.md#symmetry-physics). In particle language this charge counts particles minus [antiparticles](#antiparticle). When the [S-matrix](quantum-mechanics.md#s-matrix) commutes with it, a [scattering amplitude](quantum-mechanics.md#scattering-amplitude) between states of different charge vanishes. A neutral scalar and a [Yukawa interaction](standard-model.md#yukawa-interaction) preserve the charge, so a process with one incoming Dirac particle and only one outgoing Dirac antiparticle plus neutral particles is forbidden. This net charge is distinct from a sum of positive occupation numbers for all particle and antiparticle modes.

### Fermion bilinear

↑ **Parent:** [Dirac field](#dirac-field)

A local expression containing two [fermion](quantum-mechanics.md#fermion) fields and a matrix acting on [Dirac spinor](#dirac-spinor) indices. The choices $\Gamma=\gamma^\mu$ and $\Gamma=\gamma^\mu\gamma^5$ give the [Dirac current](quantum-field-theory.md#dirac-current) and [axial current](#axial-current).

#### Vector current

↑ **Parent:** [Fermion bilinear](#fermion-bilinear)

A [fermion bilinear](#fermion-bilinear) transforming as a [Lorentz four-vector](special-relativity.md#four-vector). For a single [Dirac field](#dirac-field) this is the [Dirac current](quantum-field-theory.md#dirac-current); distinct flavours can give a charged or flavour-changing current.

### Mode expansion of a Dirac field

↑ **Parent:** [Dirac field](#dirac-field)

The mode expansion of a free Dirac field decomposes it into positive-frequency particle modes and negative-frequency antiparticle modes:

$$
\psi(x)=\sum_s\int d\Pi_p\left[b^s(p)u^s(p)e^{-ip\cdot x}+d^{s\dagger}(p)v^s(p)e^{ip\cdot x}\right].
$$

The operators $b^s$ and $d^s$ obey fermionic anticommutation relations.

#### Particle and antiparticle occupation operators of a Dirac field

↑ **Parent:** [Mode expansion of a Dirac field](#mode-expansion-of-a-dirac-field)

The positive occupation operators are $N_e=\sum_s\int d^3p\,a_{\mathbf p}^{s\dagger}a_{\mathbf p}^s/(2\pi)^3$ and $N_{\bar e}=\sum_s\int d^3p\,b_{\mathbf p}^{s\dagger}b_{\mathbf p}^s/(2\pi)^3$. Both commute with the free Hamiltonian. The [normal-ordered](perturbative-quantum-field-theory.md#normal-ordering) local density integral $\int:\psi^\dagger\psi:\,d^3x$ is their difference, not their sum. It generates the global phase symmetry. For electron charge $-e$, electric charge is $-eQ$. Pair creation can change total occupation while preserving this net charge.

#### Antiparticle

↑ **Parent:** [Mode expansion of a Dirac field](#mode-expansion-of-a-dirac-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Antiparticle)

An antiparticle has the same mass and spin as its particle and opposite additive internal charges. In a relativistic quantum field, antiparticles are created by the negative-frequency part of the field expansion.

##### Annihilation

↑ **Parent:** [Antiparticle](#antiparticle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Annihilation)

[Particle-antiparticle annihilation](#annihilation) converts a particle and its [antiparticle](#antiparticle) into other particles, conserving [energy](classical-mechanics.md#energy) and applicable quantum numbers. Baryon-antibaryon annihilation commonly produces mesons whose subsequent decays can generate radiation.

##### Antimatter

↑ **Parent:** [Antiparticle](#antiparticle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Antimatter)

[Antimatter](#antimatter) is an assembly of [antiparticles](#antiparticle). A cosmological antimatter population is distinct from the small secondary antiparticle populations produced by energetic collisions.

##### Dirac sea

↑ **Parent:** [Antiparticle](#antiparticle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dirac_sea)

The historical interpretation fills the negative-energy electron states of the [Dirac equation](#dirac-equation) and uses the [Pauli exclusion principle](quantum-mechanics.md#pauli-exclusion-principle) to prevent additional electrons from falling into them. Removing an electron of energy $-E$ and charge $-e$ gives a hole of excitation energy $E$ and charge $+e$, interpreted as a positron. A [quantum field theory](quantum-field-theory.md) instead treats negative-frequency field coefficients as independent [antiparticle](#antiparticle) [creation operators](quantum-mechanics.md#creation-operator) in a [Fock space](quantum-field-theory.md#fock-space), with positive excitation energies after [normal ordering](perturbative-quantum-field-theory.md#normal-ordering). No literal infinite material sea is needed. Bosonic [antiparticles](#antiparticle) also exist, although a filled-sea exclusion argument cannot stabilize bosonic negative-energy levels.

#### Fermionic annihilation operator

↑ **Parent:** [Mode expansion of a Dirac field](#mode-expansion-of-a-dirac-field)

A fermionic annihilation operator removes one fermion from a specified one-particle mode. Together with its adjoint it satisfies a canonical anticommutation relation such as $\{b_r,b_s^\dagger\}=\delta_{rs}$.

#### Fermionic creation operator

↑ **Parent:** [Mode expansion of a Dirac field](#mode-expansion-of-a-dirac-field)

A fermionic creation operator is the adjoint of a [fermionic annihilation operator](#fermionic-annihilation-operator) and adds one fermion to a mode. Its square vanishes, implementing the [Pauli exclusion principle](quantum-mechanics.md#pauli-exclusion-principle).

### Dirac equation

↑ **Parent:** [Dirac field](#dirac-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dirac_equation)

The Dirac equation is the relativistic spin-one-half field equation $(i\gamma^\mu\partial_\mu-m)\psi=0$.

#### Flat-space Dirac factorization

↑ **Parent:** [Dirac equation](#dirac-equation)

The [gamma matrix](algebra.md#gamma-matrices) [Clifford algebra](algebra.md#clifford-algebra) and commuting [partial derivatives](calculus.md#partial-derivative) give $(\not\partial)^2=\Box$. Thus every free [Dirac equation](#dirac-equation) solution also solves the [Klein-Gordon equation](wave-equation.md#klein-gordon-equation) componentwise. The converse is false without the first-order [spinor](algebra.md#spinor) constraint: the second-order equation alone allows twice as much independent initial data.

#### Lichnerowicz spinor-square formula

↑ **Parent:** [Dirac equation](#dirac-equation)

With $\{\gamma^\mu,\gamma^\nu\}=2g^{\mu\nu}$ and [spin](quantum-mechanics.md#spin) [curvature](differential-geometry.md#curvature) $[\nabla_\mu,\nabla_\nu]=R_{\mu\nu ab}\gamma^{ab}/4$, the [Dirac equation](#dirac-equation) operator squares to the [rough Laplacian](fiber-bundle.md#rough-laplacian) minus $R/4$. In the [curvature](differential-geometry.md#curvature) contraction the four-gamma term vanishes by the [first Bianchi identity](general-relativity.md#first-bianchi-identity), the two-gamma terms vanish by Ricci symmetry, and the scalar term is $-2R$. In Riemannian signature $i\not\nabla$ is the [self-adjoint](linear-operator-theory.md#self-adjoint-operator) convention and its square is $-\nabla^2+R/4$.

##### Riemann tensor Clifford contraction

↑ **Parent:** [Lichnerowicz spinor-square formula](#lichnerowicz-spinor-square-formula)

The four-gamma product decomposes into fully antisymmetric, two-gamma and scalar parts. The first part vanishes on contraction by the [first Bianchi identity](general-relativity.md#first-bianchi-identity), and the two-gamma parts vanish because they contract symmetric [Ricci curvature](second-fundamental-form.md#ricci-curvature) against antisymmetric gamma matrices. The scalar contractions are $-g^{ac}g^{bd}R_{abcd}+g^{ad}g^{bc}R_{abcd}=-2R$. Here $R=g^{ac}g^{bd}R_{abcd}$ fixes the curvature-slot convention.

// Target: second-fundamental-form.bigb

##### Torsion correction to the Dirac square

↑ **Parent:** [Lichnerowicz spinor-square formula](#lichnerowicz-spinor-square-formula)

For a [metric-compatible connection](fiber-bundle.md#metric-connection) with [torsion tensor](fiber-bundle.md#torsion-tensor) $T^\rho{}_{\mu\nu}=\Gamma^\rho_{\mu\nu}-\Gamma^\rho_{\nu\mu}$, expand the square using Clifford multiplication and the full affine second derivative. Its antisymmetric part is spin curvature minus $T^\rho{}_{\mu\nu}\nabla_\rho$. This gives the displayed formula. The curvature need not have the torsion-free pair symmetry or [first Bianchi identity](general-relativity.md#first-bianchi-identity), so its Clifford contraction need not reduce to a scalar $-R/4$. General torsion produces additional first-order and nonscalar curvature couplings.

##### Compact harmonic-spinor rigidity under nonnegative scalar curvature

↑ **Parent:** [Lichnerowicz spinor-square formula](#lichnerowicz-spinor-square-formula)

On a compact boundaryless Riemannian [spin manifold](riemannian-geometry.md#spin-manifold) with $R\ge0$, integrating the [Lichnerowicz spinor-square formula](#lichnerowicz-spinor-square-formula) against a harmonic spinor gives $\int(|\nabla\psi|^2+R|\psi|^2/4)=0$. Positivity forces the spinor to be parallel. Its norm is constant on each connected component, so a nontrivial solution is nowhere zero there. Strictly positive [scalar curvature](second-fundamental-form.md#scalar-curvature) at any point on such a component excludes nonzero harmonic spinors.

###### Riemannian parallel-spinor Ricci-flatness

↑ **Parent:** [Compact harmonic-spinor rigidity under nonnegative scalar curvature](#compact-harmonic-spinor-rigidity-under-nonnegative-scalar-curvature)

A parallel spinor has zero [spin](quantum-mechanics.md#spin) [curvature](differential-geometry.md#curvature). Contracting the spinorial [Ricci identity](general-relativity.md#curvature-commutator-on-a-covariant-tensor) with a [gamma matrix](algebra.md#gamma-matrices) gives $R_{\mu\nu}\gamma^\nu\psi=0$. For each fixed $\mu$, squaring [Clifford multiplication](algebra.md#clifford-multiplication) by that Ricci row gives $|R_{\mu\cdot}|^2\psi=0$. Riemannian positivity and a nonzero spinor force every row to vanish. This implication is local and does not itself require compactness; the compact hypothesis is used to obtain parallelism from harmonicity.

#### Lorentz covariance of the Dirac operator

↑ **Parent:** [Dirac equation](#dirac-equation)

A spinor Lorentz matrix satisfies $S^{-1}\gamma^\mu S=\Lambda^\mu{}_{\nu}\gamma^\nu$. Combining this identity with the transformed derivative shows that $(i\gamma^\mu\partial'_\mu-m)\Psi'=S(i\gamma^\mu\partial_\mu-m)\Psi$. Thus a [Lorentz transformation](special-relativity.md#lorentz-transformation) carries every solution of the [Dirac equation](#dirac-equation) to another.

#### Adjoint Dirac equation

↑ **Parent:** [Dirac equation](#dirac-equation)

Varying the [Dirac action](#dirac-action) with respect to the spinor, rather than its [Dirac adjoint](#dirac-adjoint), gives the left-acting field equation after integration by parts. Together with the [Dirac equation](#dirac-equation) it proves conservation of the vector current.

#### Massless Dirac equation

↑ **Parent:** [Dirac equation](#dirac-equation)

The massless [Dirac equation](#dirac-equation) is $\gamma^m\partial_m\Psi=0$. The [Clifford algebra](algebra.md#clifford-algebra) makes its square the massless wave equation. Quantization of a worldline spin variable as $\widehat\psi^m=\gamma^m/\sqrt2$ turns its fermionic constraint into this equation.

#### Mostly-plus Dirac convention

↑ **Parent:** [Dirac equation](#dirac-equation)

One consistent [Dirac equation](#dirac-equation) convention uses $\eta=\operatorname{diag}(-1,1,1,1)$, $\{\gamma^a,\gamma^b\}=-2\eta^{ab}$, and $(i\gamma^a\partial_a+m)\psi=0$. Taking the negatives of the standard mostly-minus [gamma matrices](algebra.md#gamma-matrices), and defining the [Dirac adjoint](#dirac-adjoint) with the new $\gamma^0$, gives the same physical [Dirac action](#dirac-action). The positive-frequency plane wave is $e^{ip\cdot x}u(p)$ with $p^0>0$, and its equation is $(\not p-m)u=0$. The [mass shell](special-relativity.md#mass-shell) is $p^2=-m^2$. These signs must be translated together when using a formula stated in another convention.

### Dirac adjoint

↑ **Parent:** [Dirac field](#dirac-field)

The Dirac adjoint of a spinor is $\bar\psi=\psi^\dagger\gamma^0$. It transforms contragrediently, making $\bar\psi\psi$ a Lorentz scalar and $\bar\psi\gamma^\mu\psi$ a Lorentz vector.

#### Dirac scalar bilinear

↑ **Parent:** [Dirac adjoint](#dirac-adjoint)

The [Dirac scalar bilinear](#dirac-scalar-bilinear) is invariant under the simultaneous spinor and adjoint transformations because $\bar\Psi'\Psi'=\bar\Psi S^{-1}S\Psi$. It is the [mass term](quantum-field-theory.md#mass-term) of the [Dirac action](#dirac-action). At fixed coordinates it transforms as a [scalar field](quantum-field-theory.md#scalar-field), with an orbital transport term and no spin term.

### Dirac action

↑ **Parent:** [Dirac field](#dirac-field)

The free Dirac action is

$$
S_D=\int d^4x\,\bar\psi(i\gamma^\mu\partial_\mu-m)\psi.
$$

Its Euler-Lagrange equations are the Dirac equation and its adjoint.

### Fermion spin sum

↑ **Parent:** [Dirac field](#dirac-field)

For on-shell Dirac spinors in standard relativistic normalization,

$$
\sum_ru_r(p)\bar u_r(p)=\not p+m,
\qquad
\sum_rv_r(p)\bar v_r(p)=\not p-m.
$$

These completeness identities turn spin-summed squared amplitudes into gamma-matrix traces.

### Weyl spinor

↑ **Parent:** [Dirac field](#dirac-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weyl_spinor)

A left- or right-handed Weyl spinor transforms in the Lorentz representation $(1/2,0)$ or $(0,1/2)$. Parity exchanges the two chiralities.

#### Weyl field

↑ **Parent:** [Weyl spinor](#weyl-spinor)

A spacetime field valued in one irreducible chiral [spinor](algebra.md#spinor) representation. A free massless left-handed [Weyl field](#weyl-field) obeys $i(\partial_t-\boldsymbol\sigma\cdot\boldsymbol\nabla)\chi_L=0$. The [left-handed massless plane-wave spinor](#left-handed-massless-plane-wave-spinor) and [helicity content of a quantized Weyl field](#helicity-content-of-a-quantized-weyl-field) describe its modes and particle states. Field chirality fixes one spinor representation; it does not give the same particle and antiparticle helicity.

#### Weyl sigma matrices

↑ **Parent:** [Weyl spinor](#weyl-spinor)

For mostly-minus [metric signature](topology.md#metric-signature), the Weyl sigma matrices are $\sigma^\mu=(I,\sigma_1,\sigma_2,\sigma_3)$ and $\bar\sigma^\mu=(I,-\sigma_1,-\sigma_2,-\sigma_3)$, where $\sigma_i$ are the [Pauli matrices](algebra.md#pauli-matrices). The [Pauli matrix multiplication law](algebra.md#pauli-matrix-multiplication-law) proves

$$
\sigma^\mu\bar\sigma^\nu+\sigma^\nu\bar\sigma^\mu=2\eta^{\mu\nu}I.
$$

A real [Lorentz four-vector](special-relativity.md#four-vector) is equivalently a [Hermitian matrix](hilbert-space.md#hermitian-operator) $X=x^0I+x^i\sigma_i$ with $\det X=(x^0)^2-|\mathbf x|^2$. The transformation $X\mapsto MXM^\dagger$ for $M\in\mathrm{SL}(2,\mathbb C)$ preserves this [determinant](linear-algebra.md#determinant) and gives the [Lorentz spinor double cover](special-relativity.md#lorentz-spinor-double-cover). The indices $\sigma^\mu_{\alpha\dot\beta}$ therefore convert a vector index into one undotted and one dotted [Weyl spinor](#weyl-spinor) index. They are the invariant tensors in the mixed [supercharge](supersymmetry.md#supersymmetry-generator) anticommutator $\{Q_\alpha,\bar Q_{\dot\beta}\}=2\sigma^\mu_{\alpha\dot\beta}P_\mu$.

#### Helicity content of a quantized Weyl field

↑ **Parent:** [Weyl spinor](#weyl-spinor)

A left-handed massless [Weyl spinor](#weyl-spinor) has a positive-energy [plane wave](quantum-mechanics.md#plane-wave) transforming by $e^{i\alpha/2}$ under a rotation about its [momentum](classical-mechanics.md#momentum). Its particle has [helicity](special-relativity.md#helicity) $-1/2$. The negative-frequency term multiplies an antiparticle [fermionic creation operator](#fermionic-creation-operator), so its corresponding one-particle state carries the conjugate rotation phase and [helicity](special-relativity.md#helicity) $+1/2$. Thus a left-handed field has one particle and one antiparticle helicity; the right-handed field interchanges the signs. A full massless [Dirac field](#dirac-field) contains both chiral fields and hence both particle helicities.

#### Left-handed massless plane-wave spinor

↑ **Parent:** [Weyl spinor](#weyl-spinor)

In the standard [Weyl representation of the gamma matrices](#weyl-representation-of-the-gamma-matrices) and mostly-minus [metric signature](topology.md#metric-signature), the left [chirality](#chirality-physics) component obeys $i(\partial_t-\boldsymbol\sigma\cdot\boldsymbol\nabla)\chi_L=0$. A [plane wave](quantum-mechanics.md#plane-wave) with $p^0>0$ exists precisely on the massless [mass shell](special-relativity.md#mass-shell) $p^0=|\mathbf p|$. Its coefficient is a negative [helicity](special-relativity.md#helicity) eigenspinor. For direction angles $\vartheta,\varphi$, one normalized choice is

$$
\chi_-=\begin{pmatrix}-e^{-i\varphi}\sin(\vartheta/2)\\\cos(\vartheta/2)\end{pmatrix},\qquad
(\boldsymbol\sigma\cdot\widehat{\mathbf p})\chi_-=-\chi_-.
$$

The nonzero solution is unique up to overall normalization and phase. Different patches are required for a continuous phase choice over all directions; the direction of zero [momentum](classical-mechanics.md#momentum) is undefined.

#### Opposite Weyl boost generators

↑ **Parent:** [Weyl spinor](#weyl-spinor)

With $K_i=M_{0i}$ and $M_{\mu\nu}=i\gamma_{\mu\nu}/2$ in the supplied mostly-minus index convention, the two [Weyl spinor](#weyl-spinor) blocks have equal rotation generators $J_i=\sigma_i/2$ and opposite boost generators. A complex-linear intertwiner must commute with every [SU(2)](topological-group.md#su-2-group) rotation and hence be scalar by the [Schur lemma](representation-theory.md#schur-s-lemma), but no nonzero scalar intertwines the opposite boosts. This proves inequivalence of the two complex representations; parity exchanges them.

#### Weyl spinor bilinear exchange identity

↑ **Parent:** [Weyl spinor](#weyl-spinor)

For odd [Grassmann variables](linear-algebra.md#grassmann-variable), $(\chi\psi)=\chi^\alpha\psi_\alpha$ is symmetric under exchanging the two spinors: the Grassmann sign cancels the sign of the antisymmetric epsilon contraction. With $\epsilon^{12}=1$, lower components $\chi=(a,b)$ and $\psi=(c,d)$ give $(\chi\psi)=bc-ad$. Commuting numerical spinors instead give an antisymmetric contraction.

##### Square of a Weyl spinor bilinear

↑ **Parent:** [Weyl spinor bilinear exchange identity](#weyl-spinor-bilinear-exchange-identity)

For four independent odd [Grassmann variables](linear-algebra.md#grassmann-variable) $a,b,c,d$, $(bc-ad)^2=-2abcd$, whereas $(\psi\psi)(\chi\chi)=(-2cd)(-2ab)=4abcd$. This proves the displayed two-component identity and fixes its sign. It is not valid with the same interpretation for commuting spinors, whose self-contractions vanish.

#### Chirality (physics)

↑ **Parent:** [Weyl spinor](#weyl-spinor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chirality_(physics))

Chirality distinguishes the two irreducible Weyl representations of the proper Lorentz group. For a massless particle it agrees with helicity up to the particle-antiparticle convention, while a mass term couples opposite chiralities.

##### Chiral projector

↑ **Parent:** [Chirality (physics)](#chirality-physics)

The projectors $P_L=(1-\gamma^5)/2$ and $P_R=(1+\gamma^5)/2$ select the two [chirality](#chirality-physics) eigenspaces of a [Dirac field](#dirac-field). They satisfy $P_L+P_R=I$, $P_LP_R=0$, and $P_L^2=P_L$, $P_R^2=P_R$.

###### Chiral fermion trace contraction

↑ **Parent:** [Chiral projector](#chiral-projector)

With [Minkowski metric](special-relativity.md#minkowski-metric) signature $+---$ and $\operatorname{tr}(\gamma^\mu\gamma^\nu\gamma^\rho\gamma^\sigma\gamma_5)=4i\epsilon^{\mu\nu\rho\sigma}$, define $H^{\mu\nu}(a,b)=a^\mu b^\nu+a^\nu b^\mu-g^{\mu\nu}a\cdot b+i\epsilon^{\mu\nu\rho\sigma}a_\rho b_\sigma$. Then $\operatorname{tr}[\not a\gamma^\mu(1-\gamma_5)\not b\gamma^\nu(1-\gamma_5)]=8H^{\mu\nu}(a,b)$. The symmetric-tensor contraction gives twice the sum of the two possible dot-product pairings; the [Levi-Civita symbol](calculus.md#levi-civita-symbol) contraction, including the two factors of $i$, gives twice their difference. Their sum is the displayed identity, explaining the single pairing in left-chiral weak rates.

##### Vectorlike gauge spectrum

↑ **Parent:** [Chirality (physics)](#chirality-physics)

A vectorlike gauge spectrum pairs complex [gauge group representations](#gauge-group-representation) $R$ and $\bar R$ among independent left-handed [Weyl spinors](#weyl-spinor). Such a pair permits a gauge-invariant [fermion](quantum-mechanics.md#fermion) mass and occurs in a full charged [hypermultiplet](supersymmetry.md#hypermultiplet) of four-dimensional $\mathcal N=2$ [extended supersymmetry](supersymmetry.md#extended-supersymmetry).

##### Chiral gauge spectrum

↑ **Parent:** [Chirality (physics)](#chirality-physics)

A chiral gauge spectrum has independent left-handed [Weyl spinors](#weyl-spinor) in complex [gauge group representations](#gauge-group-representation) without an obligatory conjugate pair of left-handed [Weyl spinors](#weyl-spinor). The right-handed antiparticles required by the [CPT theorem](quantum-field-theory.md#cpt-theorem) do not themselves make a spectrum vectorlike.

#### Weyl representation of the gamma matrices

↑ **Parent:** [Weyl spinor](#weyl-spinor)

In the Weyl representation,

$$
\gamma^\mu=\begin{pmatrix}0&\sigma^\mu\\\bar\sigma^\mu&0\end{pmatrix},
\qquad
\gamma^5=\begin{pmatrix}-I&0\\0&I\end{pmatrix}.
$$

A Dirac spinor therefore splits into left- and right-handed two-component spinors.

#### Majorana spinor

↑ **Parent:** [Weyl spinor](#weyl-spinor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Majorana_spinor)

A Majorana spinor equals its charge conjugate. In the Weyl representation it can be written $\psi_M=(u_L,i\sigma^2u_L^*)^T$ from one left-handed Weyl spinor.

##### Four-dimensional Majorana bilinear vanishing criterion

↑ **Parent:** [Majorana spinor](#majorana-spinor)

For a [Majorana spinor](#majorana-spinor) $\lambda$ with odd [Grassmann variables](linear-algebra.md#grassmann-variable) as components, $\lambda^TM\lambda$ sees only the antisymmetric part of $M$. With $C^T=-C$ and $(\gamma^a)^T=-C\gamma^aC^{-1}$, reversing an antisymmetrized gamma product gives the displayed transpose rule. Thus the same-spinor vector and bivector bilinears vanish, whereas scalar, pseudoscalar and three-form bilinears can be nonzero. Four-dimensional [Hodge duality](complex-geometry.md#hodge-duality) gives the same vanishing result for a bivector multiplied by $\gamma_5$. Commuting spinors instead see the symmetric part, so their selection rule is different.

##### Four-dimensional Majorana bilinear interchange

↑ **Parent:** [Majorana spinor](#majorana-spinor)

For Grassmann-odd four-dimensional [Majorana spinors](#majorana-spinor), choose $C^T=-C$ and $(\gamma^a)^T=-C\gamma^aC^{-1}$. Then $C\gamma^a$ is symmetric whereas $C\gamma^{abc}$ is antisymmetric. Swapping Grassmann components therefore changes the sign of a vector bilinear but preserves a three-gamma bilinear. Integration by parts and antisymmetry of the vector indices then make the two spinor variations of the quadratic [Rarita-Schwinger field](#rarita-schwinger-field) action equal. Commuting auxiliary spinors have different interchange signs.

##### Majorana-Weyl spinor

↑ **Parent:** [Majorana spinor](#majorana-spinor)

A Majorana-Weyl spinor satisfies both a [Majorana spinor](#majorana-spinor) reality condition and a [Weyl spinor](#weyl-spinor) chirality condition when dimension and signature permit them. In ten-dimensional Lorentzian spacetime it has sixteen real components off shell and eight physical massless spin-one-half polarizations.

##### Majorana Grassmann bilinear interchange

↑ **Parent:** [Majorana spinor](#majorana-spinor)

For Grassmann-odd spinors in two dimensions with $\bar\psi=\psi^TC$, $C^T=-C$ and $(\gamma^\mu)^TC=-C\gamma^\mu$, moving components past each other gives $\bar\chi\epsilon=\bar\epsilon\chi$ and $\bar\chi\gamma^\mu\gamma^\nu\epsilon=\bar\epsilon\gamma^\nu\gamma^\mu\chi$. The transpose of a two-gamma product reverses its order; the Grassmann sign and the antisymmetry of $C$ cancel. For $\delta\psi=B\gamma^\mu\partial_\mu X\epsilon$, this also gives $\delta\bar\psi=-B\bar\epsilon\gamma^\mu\partial_\mu X$. These identities fix the boundary variation in [worldsheet supersymmetry](string-theory.md#worldsheet-supersymmetry); commuting spinors would not obey the same interchange rule.

##### Majorana mass term

↑ **Parent:** [Majorana spinor](#majorana-spinor)

A Majorana mass term pairs a Weyl field with itself and violates its continuous phase symmetry. Gauge invariance therefore permits it only when the field is neutral under every unbroken gauge charge.

###### Grassmann variation of a chiral Majorana mass term

↑ **Parent:** [Majorana mass term](#majorana-mass-term)

For anticommuting components and an antisymmetric numerical matrix $A$, $\delta(\psi^TA\psi)=2\delta\psi^TA\psi$: move the second varied field past the first and use $A^T=-A$. Applying this to $C^{-1}$ and to $C$ cancels the factor $1/2$ in $\mathcal L=\bar\psi i\not\partial\psi+\tfrac12(m\psi^TC^{-1}\psi-m^*\bar\psi C\bar\psi^T)$. Varying the [Dirac adjoint](#dirac-adjoint) gives the first displayed equation. Integration by parts in the spinor variation gives $i\gamma^{\mu T}\partial_\mu\bar\psi^T+mC^{-1}\psi=0$; multiplication by $C$ gives the second. Squaring the coupled equations yields $(\Box+|m|^2)\psi=0$, so the physical [Majorana fermion](#majorana-spinor) mass is $|m|$.

### Dirac spinor

↑ **Parent:** [Dirac field](#dirac-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dirac_spinor)

A Dirac spinor transforms as $(1/2,0)\oplus(0,1/2)$, so it combines the two [Weyl chiralities](#weyl-spinor) into a parity-invariant representation.

#### Dirac plane waves in the standard representation

↑ **Parent:** [Dirac spinor](#dirac-spinor)

For $g=\operatorname{diag}(1,-1,-1,-1)$ and the block-diagonal standard representation of the [gamma matrices](algebra.md#gamma-matrices), write a positive-energy [Dirac spinor](#dirac-spinor) as $(\xi,\eta)^T$. The [Dirac equation](#dirac-equation) gives $\eta=(\boldsymbol\sigma\cdot\mathbf p)\xi/(E+m)$. Choosing two orthonormal two-spinors $\chi_s$ yields the displayed positive-frequency solutions. Negative-frequency solutions are $v_s=\sqrt{E+m}((\boldsymbol\sigma\cdot\mathbf p)\eta_s/(E+m),\eta_s)^T$ multiplying $e^{ip\cdot x}$. They obey $(\not p+m)v_s=0$. Both have norm $2E$; their [Dirac adjoints](#dirac-adjoint) give $\overline u_ru_s=2m\delta_{rs}$ and $\overline v_rv_s=-2m\delta_{rs}$. Spatial rotations act on each two-spinor with generators $\sigma_j/2$, explaining [spin one-half](quantum-mechanics.md#spin-one-half).

#### Massless limit of a transverse canonical-spin label

↑ **Parent:** [Dirac spinor](#dirac-spinor)

Boost a massive rest [Dirac spinor](#dirac-spinor) labelled by $\xi=(1,1)^T/\sqrt2$ along the third axis and take its [massless limit](quantum-field-theory.md#massless-limit). In the [Weyl representation](algebra.md#chiral-gamma-matrix-representation) the result is the displayed equal superposition of helicities, not an eigenvector of the fixed transverse rotation generator $\Sigma_1/2$. For momentum $(E,0,0,E)$ the positive-energy Hamiltonian is $E\gamma^0\gamma^3$, which anticommutes with $\Sigma_1=\operatorname{diag}(\sigma_1,\sigma_1)$. A nonzero positive-energy solution cannot also be a $\Sigma_1$ eigenvector. Thus a transported canonical spin label must be distinguished from literal transverse spin at zero mass; longitudinal [helicity](special-relativity.md#helicity) remains a good quantum number.

#### Hermitian square-root construction of Dirac plane waves

↑ **Parent:** [Dirac spinor](#dirac-spinor)

In mostly-minus signature and the [Weyl representation](algebra.md#chiral-gamma-matrix-representation), take $p^0=E=\sqrt{|\mathbf p|^2+m^2}>0$. The [Hermitian matrices](hilbert-space.md#hermitian-operator) $A=p\cdot\sigma=E-\mathbf p\cdot\boldsymbol\sigma$ and $B=p\cdot\bar\sigma=E+\mathbf p\cdot\boldsymbol\sigma$ commute and obey $AB=m^2I$. Their positive [square roots of a matrix](linear-algebra.md#square-root-of-a-matrix) therefore obey $\sqrt A\sqrt B=mI$. It follows that $u=(\sqrt A\xi,\sqrt B\xi)^T$ solves $(\not p-m)u=0$ and $v=(\sqrt A\zeta,-\sqrt B\zeta)^T$ solves $(\not p+m)v=0$. They multiply $e^{-ipx}$ and $e^{ipx}$ respectively. For normalized two-spinors, $u^\dagger u=v^\dagger v=2E$. The formula extends by positive-semidefinite square roots to the [massless limit](quantum-field-theory.md#massless-limit).

#### Euclidean adjoint Dirac Feynman rules

↑ **Parent:** [Dirac spinor](#dirac-spinor)

Take Hermitian generators with $[T^a,T^b]=if^{abc}T^c$, $(T^b_{\mathrm{ad}})_{ac}=-if^{bac}$, and $D_\mu=\partial_\mu-igA_\mu^bT^b_{\mathrm{ad}}$. For $S_\psi=\int\bar\psi(\gamma_\mu D_\mu+m)\psi$ and $\{\gamma_\mu,\gamma_\nu\}=2\delta_{\mu\nu}$, the [Dirac propagator](quantum-field-theory.md#dirac-propagator) is $\delta^{ac}(-i\not p+m)/(p^2+m^2)$. Expansion of $e^{-S_\psi}$ gives the fermion-gluon vertex $+ig\gamma_\mu(T^b_{\mathrm{ad}})_{ac}$. There is no two-gluon seagull vertex in this first-order kinetic action, and a closed fermion loop has a minus sign.

#### Spinor representation of the Lorentz group

↑ **Parent:** [Dirac spinor](#dirac-spinor)

With $S^{\mu\nu}=\frac14[\gamma^\mu,\gamma^\nu]$, the spinor representation is

$$
S[\Lambda]=\exp\left(\frac12\Omega_{\mu\nu}S^{\mu\nu}\right).
$$

It obeys $S^{-1}\gamma^\mu S=\Lambda^\mu{}_\nu\gamma^\nu$.

##### Spinor Lorentz generator commutator

↑ **Parent:** [Spinor representation of the Lorentz group](#spinor-representation-of-the-lorentz-group)

Define $\sigma^{\mu\nu}=\frac i2[\gamma^\mu,\gamma^\nu]$ using the [gamma matrix](algebra.md#gamma-matrices) [Clifford algebra](algebra.md#clifford-algebra). Moving $\gamma^\rho$ through the two factors with $\{\gamma^\mu,\gamma^\nu\}=2g^{\mu\nu}$ proves the displayed [operator commutator](vector-space.md#operator-commutator). For real antisymmetric $\omega_{\mu\nu}$ and $S=1-\frac i4\sigma^{\mu\nu}\omega_{\mu\nu}$, it gives $S^{-1}\gamma^\rho S=\gamma^\rho+\omega^\rho{}_{\nu}\gamma^\nu+O(\omega^2)$. This is the infinitesimal [Lorentz covariance](special-relativity.md#lorentz-covariance) identity required by the [Dirac equation](#dirac-equation).

##### Even-dimensional Clifford spinor dimension

↑ **Parent:** [Spinor representation of the Lorentz group](#spinor-representation-of-the-lorentz-group)

After complexification, pair the $D=2n$ [Clifford algebra](algebra.md#clifford-algebra) generators into $n$ fermionic creation and annihilation operators. Their occupation basis has $2^n$ states, giving the irreducible complex Dirac module. The chirality operator separates its even and odd occupation subspaces, each with $2^{n-1}$ states. Majorana reality conditions concern real dimensions and depend on spacetime signature; they must not be imposed in every even dimension indiscriminately.

##### Rarita-Schwinger field

↑ **Parent:** [Spinor representation of the Lorentz group](#spinor-representation-of-the-lorentz-group)

A vector-spinor describes a spin-three-halves field after its lower-spin components are removed by constraints and, in the massless theory, gauge equivalence. The massless equation is invariant under $\psi_\mu\mapsto\psi_\mu+\partial_\mu\eta$. Gamma-trace gauge and the field equation give $\gamma\cdot\psi=\partial\cdot\psi=\not\partial\psi_\mu=0$. Only helicities $\pm3/2$ remain. A four-dimensional Majorana field has two physical polarizations; a complex field also has independent antiparticle modes. The [gravitino](supersymmetry.md#gravitino) is the [supergravity](supersymmetry.md#supergravity) realization of this field.

###### Gamma trace of a vector-spinor

↑ **Parent:** [Rarita-Schwinger field](#rarita-schwinger-field)

The gamma trace contracts the vector index of a [Rarita-Schwinger field](#rarita-schwinger-field) with a [gamma matrix](algebra.md#gamma-matrices), producing an ordinary spinor. In the massive free theory it vanishes by the field equations. In the massless theory a [gauge transformation](electromagnetism.md#gauge-transformation) changes it by $\gamma^\mu\partial_\mu\epsilon$, allowing a gamma-traceless gauge for propagating modes. Together with transversality this removes the unwanted spin-one-half sector.

###### Massless Rarita-Schwinger polarization count

↑ **Parent:** [Rarita-Schwinger field](#rarita-schwinger-field)

Gauge equivalence $\psi_\mu\sim\psi_\mu+\partial_\mu\epsilon$ permits gamma-trace gauge. The [Rarita-Schwinger field](#rarita-schwinger-field) equation then gives transversality and a massless [Dirac equation](#dirac-equation) for each component. For momentum along the third axis, residual gauge removes the temporal and longitudinal components. The remaining constraint is $\psi_2=\gamma^1\gamma^2\psi_1$, with $\psi_1$ in the two-dimensional kernel of $\not p$. Spinor helicity $\pm1/2$ is paired with vector helicity of the same sign, leaving only $\pm3/2$. A [Majorana spinor](#majorana-spinor) reality condition identifies antiparticles; a Dirac vector-spinor has separate antiparticle modes.

###### Massive Rarita-Schwinger constraints

↑ **Parent:** [Rarita-Schwinger field](#rarita-schwinger-field)

For $\gamma^{\mu\nu\rho}\partial_\nu\psi_\rho-m\gamma^{\mu\rho}\psi_\rho=0$ with $m\ne0$, divergence gives $\gamma^{\mu\rho}\partial_\mu\psi_\rho=0$. Gamma contraction then forces $\gamma\cdot\psi=0$, hence $\partial\cdot\psi=0$. The remaining equation is $(\not\partial+m)\psi_\mu=0$ in a mostly-plus convention. In the rest frame the temporal component vanishes, leaving a spatial [vector](vector-space.md#vector) times an on-shell two-component spinor; its gamma trace removes the spin-one-half sector. The remaining spin-three-halves representation has four physical states, including longitudinal helicities $\pm1/2$.

##### Inverse Lorentz action on gamma matrices

↑ **Parent:** [Spinor representation of the Lorentz group](#spinor-representation-of-the-lorentz-group)

With $\{\gamma_\mu,\gamma_\nu\}=2\eta_{\mu\nu}$, $\Omega=\omega^{\mu\nu}\gamma_{\mu\nu}/4$, and $\Lambda=e^\omega$, the [Clifford algebra](algebra.md#clifford-algebra) gives $[\Omega,\gamma^\rho]=-\omega^\rho{}_{\mu}\gamma^\mu$. Exponentiation proves the inverse Lorentz action displayed above, equivalently $S^{-1}\gamma^\rho S=\Lambda^\rho{}_{\mu}\gamma^\mu$. This second order is what combines with $\psi\mapsto S\psi$ and the [Dirac adjoint](#dirac-adjoint) action $\bar\psi\mapsto\bar\psi S^{-1}$ to make the gamma bilinears transform as ordinary contravariant [tensors](linear-algebra.md#tensor).

##### Dirac spinor pseudo-unitarity

↑ **Parent:** [Spinor representation of the Lorentz group](#spinor-representation-of-the-lorentz-group)

The generators in the [Spinor representation of the Lorentz group](#spinor-representation-of-the-lorentz-group) satisfy $M^\dagger\gamma^0+\gamma^0M=0$, so the finite transformation preserves the indefinite form $S^\dagger\gamma^0S=\gamma^0$. This makes $\bar\psi\psi$ a [Lorentz scalar](special-relativity.md#lorentz-scalar) through the [Dirac adjoint](#dirac-adjoint). Boost generators are Hermitian rather than anti-Hermitian: a boost has eigenvalues $e^{\pm\eta/2}$ and is not unitary in the ordinary positive-definite component norm. Rotations are unitary. This component representation is distinct from the unitary [action](classical-mechanics.md#action) on the physical state space.

##### Lorentz-spinor generators from a Clifford algebra

↑ **Parent:** [Spinor representation of the Lorentz group](#spinor-representation-of-the-lorentz-group)

In a real-generator convention, $M^{\rho\sigma}=\frac14[\gamma^\rho,\gamma^\sigma]$ obeys $[M^{\rho\sigma},\gamma^\mu]=g^{\sigma\mu}\gamma^\rho-g^{\rho\mu}\gamma^\sigma$. Applying this identity to the commutator of two gamma matrices proves the [Lorentz algebra](semisimple-lie-algebra.md#lorentz-algebra) relations. With the matching vector generators and real antisymmetric parameters, $S=\exp(\frac12\Omega_{\rho\sigma}M^{\rho\sigma})$ obeys $S^{-1}\gamma^\mu S=\Lambda^\mu{}_{\nu}\gamma^\nu$. A convention using Hermitian Lorentz generators instead must consistently insert factors of $i$.

##### Pseudo-unitarity of the spinor Lorentz representation

↑ **Parent:** [Spinor representation of the Lorentz group](#spinor-representation-of-the-lorentz-group)

The spinor Lorentz matrices preserve the indefinite form defined by $\gamma^0$: $S^\dagger\gamma^0S=\gamma^0$. This follows from the gamma-matrix adjoint identities for infinitesimal generators and extends to finite connected transformations. Consequently the [Dirac adjoint](#dirac-adjoint) transforms with $S^{-1}$, even though a boost matrix is not ordinarily unitary.

##### Infinitesimal transformation of a Dirac field

↑ **Parent:** [Spinor representation of the Lorentz group](#spinor-representation-of-the-lorentz-group)

For $\Lambda=1+\omega$ with antisymmetric lowered parameters, the spin matrix is $S=1-(i/4)\omega_{\mu\nu}\sigma^{\mu\nu}$, where $\sigma^{\mu\nu}=(i/2)[\gamma^\mu,\gamma^\nu]$. At transformed coordinates this is the full component transformation. At fixed coordinates an additional orbital term $-\omega^\mu{}_{\nu}x^\nu\partial_\mu\Psi$ appears.

##### Spinor sign under a full spatial rotation

↑ **Parent:** [Spinor representation of the Lorentz group](#spinor-representation-of-the-lorentz-group)

For a [Dirac spinor](#dirac-spinor) a spatial rotation acts in each chiral block by a [matrix exponential](linear-operator-theory.md#matrix-exponential) $e^{\pm i\theta\mathbf n\cdot\boldsymbol\sigma/2}$, depending on angle orientation. Since $(\mathbf n\cdot\boldsymbol\sigma)^2=I_2$ for a unit axis, the [Pauli matrix multiplication law](algebra.md#pauli-matrix-multiplication-law) gives this exponential as $\cos(\theta/2)I_2\pm i\sin(\theta/2)\mathbf n\cdot\boldsymbol\sigma$. At $\theta=2\pi$ it is $-I_2$, and at $4\pi$ it is $I_2$. A [vector](vector-space.md#vector) returns already at $2\pi$. This describes the lift of the rotation loop to the [Spin group](semisimple-lie-algebra.md#spin-group), rather than a single-valued representation of the ordinary rotation group on spinors.

##### Lorentz generator from gamma-matrix commutators

↑ **Parent:** [Spinor representation of the Lorentz group](#spinor-representation-of-the-lorentz-group)

The [Clifford algebra](algebra.md#clifford-algebra) gives $S^{\mu\nu}=\frac12\gamma^\mu\gamma^\nu-\frac12\eta^{\mu\nu}I$. Reordering one more [gamma matrix](algebra.md#gamma-matrices) gives $[S^{\mu\nu},\gamma^\rho]=\eta^{\nu\rho}\gamma^\mu-\eta^{\mu\rho}\gamma^\nu$. The [commutator derivation identity](lie-algebra.md#commutator-derivation-identity) then gives

$$
[S^{\mu\nu},S^{\rho\sigma}]=\eta^{\nu\rho}S^{\mu\sigma}-\eta^{\mu\rho}S^{\nu\sigma}+\eta^{\nu\sigma}S^{\rho\mu}-\eta^{\mu\sigma}S^{\rho\nu},
$$

so these matrices represent the [Lorentz algebra](semisimple-lie-algebra.md#lorentz-algebra). This convention has no extra factor of $i$; the spatial generators are $-\frac i2\epsilon^{jkl}\operatorname{diag}(\sigma^l,\sigma^l)$.

#### Dirac mass term

↑ **Parent:** [Dirac spinor](#dirac-spinor)

A Dirac mass term pairs left- and right-handed Weyl fields in conjugate Lorentz representations. Gauge invariance requires the two chiral fields to carry matching internal quantum numbers, directly or after multiplication by a scalar field that acquires a vacuum expectation value.

### Spin sum

↑ **Parent:** [Dirac field](#dirac-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spin_sum)

A spin sum adds a squared [scattering amplitude](quantum-mechanics.md#scattering-amplitude) over the unobserved [spins](quantum-mechanics.md#spin) of external particles. For an on-shell [Dirac spinor](#dirac-spinor), the completeness relations $\sum_s u_s(p)\bar u_s(p)=\not p+m$ and $\sum_s v_s(p)\bar v_s(p)=\not p-m$ turn the sum into a [gamma-matrix trace](#gamma-matrix-trace).

#### Spin average

↑ **Parent:** [Spin sum](#spin-sum)

For an unpolarized initial state, average the squared [scattering amplitude](quantum-mechanics.md#scattering-amplitude) over its equally populated spin states. With two incoming spin-one-half particles this gives a factor $1/(2\cdot2)=1/4$. Unobserved final spins are summed rather than averaged.

#### Gamma-matrix trace

↑ **Parent:** [Spin sum](#spin-sum)

A gamma-matrix trace is a [matrix trace](linear-algebra.md#matrix-trace) of products of [gamma matrices](algebra.md#gamma-matrices). In four spacetime dimensions, $\operatorname{tr}(\gamma^\mu\gamma^\nu)=4\eta^{\mu\nu}$ and $\operatorname{tr}(\gamma^\mu\gamma^\nu\gamma^\rho\gamma^\sigma)=4(\eta^{\mu\nu}\eta^{\rho\sigma}-\eta^{\mu\rho}\eta^{\nu\sigma}+\eta^{\mu\sigma}\eta^{\nu\rho})$.

## Gauge field

↑ **Parent:** [Relativistic quantum field](relativistic-quantum-field.md)

A [gauge field](#gauge-field) is a connection associated with a local symmetry in a [gauge theory](quantum-field-theory.md#gauge-theory). Its [gauge potential](#gauge-field) defines the internal-symmetry contribution to a [covariant derivative](general-relativity.md#covariant-derivative). For an Abelian [gauge field](#gauge-field), the [gauge field strength](#gauge-field-strength) is $F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu$.

### Chern-Simons 5-form

↑ **Parent:** [Gauge field](#gauge-field)

For a matrix-valued [gauge field](#gauge-field) $A$, let $F=dA+A\wedge A$ be its [gauge field strength](#gauge-field-strength); products below combine matrix multiplication with the [wedge product of differential forms](differential-form.md#wedge-product-of-differential-forms). The five-form can be written $Q_5=\operatorname{Tr}(A(dA)^2+\tfrac32A^3dA+\tfrac35A^5)$. Applying the [exterior derivative](differential-form.md#exterior-derivative), using its graded product rule and the graded cyclic property of the [matrix trace](linear-algebra.md#matrix-trace), gives $dQ_5=\operatorname{Tr}(F^3)$. The six-form is an invariant polynomial in the [gauge curvature](#gauge-field-strength), while its local potential depends on the connection.

#### Abelian Chern-Simons five-form field equation

↑ **Parent:** [Chern-Simons 5-form](#chern-simons-5-form)

For $F=dA$ on a five-dimensional oriented spacetime, the action $S=-\frac12\int F\wedge *F+c\int A\wedge F\wedge F$ has bulk variation $\int\delta A\wedge(-d*F+3cF\wedge F)$. Two integrations by parts make the three variations of the [Chern-Simons 5-form](#chern-simons-5-form) contribute equally. Under $A\mapsto A+d\lambda$, the extra action is $c\int d(\lambda F\wedge F)$, a boundary term by the [Generalized Stokes theorem](differential-form.md#generalized-stokes-theorem). Its bulk field equation is gauge invariant. The Chern-Simons term is metric-independent and has no bulk contribution to the [stress-energy tensor](general-relativity.md#stress-energy-tensor) when the differential-form field is held fixed in metric variation.

#### Variation of the Chern-Simons 5-form

↑ **Parent:** [Chern-Simons 5-form](#chern-simons-5-form)

The boundary four-form is $\Theta=\operatorname{Tr}[\delta A\,(FA+AF-\tfrac12A^3)]$. To derive the identity, put $B=dA$ and $a=\delta A$. The variations of the three polynomial terms in $Q_5$ are respectively $3\operatorname{Tr}(aB^2)+d\operatorname{Tr}[a(BA+AB)]$, $3\operatorname{Tr}[a(A^2B+BA^2)]+\tfrac32d\operatorname{Tr}(aA^3)$, and $3\operatorname{Tr}(aA^4)$. Their sum gives the identity because $F=B+A^2$. For variations in a [Lie algebra](lie-algebra.md) with basis $T_\alpha$, the bulk field equations are $\operatorname{Tr}(T_\alpha F^2)=0$, not necessarily the unprojected matrix equation $F^2=0$. Conjugation of both the Lie algebra and the [gauge curvature](#gauge-field-strength) proves covariance of these equations under [Yang-Mills gauge transformations](#yang-mills-gauge-transformation).

### CP transformation of a non-Abelian gauge connection

↑ **Parent:** [Gauge field](#gauge-field)

For vector coupling to a Dirac [fermion](quantum-mechanics.md#fermion), write the Hermitian color connection $\mathcal A_\mu=A_\mu^aT^a$. [Charge conjugation](quantum-field-theory.md#charge-conjugation) reverses the vector current and transposes its color matrix, requiring $\mathcal A_\mu^C=-\mathcal A_\mu^T$. Combining with [parity](quantum-mechanics.md#parity) gives $\mathcal A_\mu^{CP}(x)=-P_\mu{}^\nu\mathcal A_\nu^T(x_P)$, where $P=\operatorname{diag}(1,-1,-1,-1)$. The transpose acts only on color indices; intrinsic [fermion](quantum-mechanics.md#fermion) phases cancel in the bilinear.

### Abelian p-form gauge field

↑ **Parent:** [Gauge field](#gauge-field)

An Abelian $p$-form gauge potential $A_p$ is an antisymmetric tensor field with gauge equivalence $A_p\mapsto A_p+d\Lambda_{p-1}$ and field strength $F_{p+1}=dA_p$. Its field strength obeys the [Bianchi identity for an Abelian p-form](#bianchi-identity-for-an-abelian-p-form). The potential can have global gauge data even when its local field strength vanishes.

#### Massive p-form field

↑ **Parent:** [Abelian p-form gauge field](#abelian-p-form-gauge-field)

A free massive $p$-form obeys the displayed equation, with the divergence constraint following by applying the [codifferential](differential-form.md#codifferential). For $m>0$ and $0\le p\le D-1$, a rest frame leaves an antisymmetric tensor on $D-1$ spatial directions, giving $\binom{D-1}{p}$ physical polarizations. The mass term removes the ordinary gauge invariance, unless a [Stueckelberg mechanism](#stueckelberg-mechanism) restores a redundant description.

// Target: quantum-field-theory.bigb

##### Stueckelberg mechanism

↑ **Parent:** [Massive p-form field](#massive-p-form-field)

For $p\ge1$, introduce a $(p-1)$-form $C$ and replace the mass term of a [massive p-form field](#massive-p-form-field) by one built from $A-m^{-1}dC$. The transformations $A\mapsto A+d\Lambda$, $C\mapsto C+m\Lambda$ leave this combination and $dA$ invariant. Gauge fixing $C=0$ recovers the original massive theory. Its massless-component counts add as $\binom{D-2}{p}+\binom{D-2}{p-1}=\binom{D-1}{p}$, explaining the longitudinal degrees of freedom and the corresponding assembly of nonzero [Kaluza-Klein modes](physics.md#kaluza-klein-mode).

##### Massive p-form duality

↑ **Parent:** [Massive p-form field](#massive-p-form-field)

For a free [massive p-form field](#massive-p-form-field), the displayed dual has degree $D-p-1$. The massive field equation reconstructs $A$ locally from $m^{-1}*dB$ with the signature-dependent sign. It also gives $\delta B=0$ and $\delta dB+m^2B=0$. The polarization counts agree because $\binom{D-1}{p}=\binom{D-1}{D-p-1}$. The construction depends on nonzero mass and therefore differs from [massless p-form duality](#massless-p-form-duality) by one potential rank.

// Target: physics.bigb

#### Massless p-form gauge field

↑ **Parent:** [Abelian p-form gauge field](#abelian-p-form-gauge-field)

A massless Abelian $p$-form in $D$-dimensional flat spacetime transforms on shell as an antisymmetric rank-$p$ tensor of the rotational [little group](special-relativity.md#little-group) $SO(D-2)$. Its physical state count is $\binom{D-2}{p}$. A compatible real self-duality constraint halves this count. A four-dimensional three-form has no local propagating polarization.

##### Massless p-form duality

↑ **Parent:** [Massless p-form gauge field](#massless-p-form-gauge-field)

For a free [massless p-form gauge field](#massless-p-form-gauge-field) with $0\le p\le D-2$, its field equation makes $*dA$ closed. The [Poincaré lemma](differential-form.md#poincare-lemma) writes it locally as $dB$, giving a dual potential of degree $D-p-2$. The original [Bianchi identity for an Abelian p-form](#bianchi-identity-for-an-abelian-p-form) becomes the dual field equation, and the original equation becomes the dual Bianchi identity. The two descriptions have equal [little group](special-relativity.md#little-group) counts $\binom{D-2}{p}$. Global fluxes and top forms require separate treatment.

// Target: quantum-field-theory.bigb

##### Nondynamical four-dimensional three-form

↑ **Parent:** [Massless p-form gauge field](#massless-p-form-gauge-field)

A three-form potential in four dimensions has no local massless polarizations. Its four-form field strength can be a constant multiple of the spacetime volume form. The equation $d(g_3^{-2}*F_4)=0$ leaves a constant flux parameter, which can affect vacuum energy despite supplying no local wave.

##### Two-form scalar duality

↑ **Parent:** [Massless p-form gauge field](#massless-p-form-gauge-field)

Locally in four dimensions, a massless two-form is dual to one real [scalar field](quantum-field-theory.md#scalar-field). In signature $(-+++)$, the first-order density $-H^2/(12g_B^2)+\epsilon^{\mu\nu\rho\sigma}H_{\mu\nu\rho}\partial_\sigma a/6$ gives $H^{\mu\nu\rho}=g_B^2\epsilon^{\mu\nu\rho\sigma}\partial_\sigma a$. Eliminating $H$ in both terms produces $-g_B^2(\partial a)^2/2$, so the fixed-normalization kinetic coefficient is inverted. Global flux sectors and scalar periodicities need separate treatment.

#### Bianchi identity for an Abelian p-form

↑ **Parent:** [Abelian p-form gauge field](#abelian-p-form-gauge-field)

For an [Abelian p-form gauge field](#abelian-p-form-gauge-field) with local field strength $F=dA$, the [exterior derivative](differential-form.md#exterior-derivative) identity $d^2=0$ gives $dF=0$. In a first-order duality formulation, this identity can be enforced with a Lagrange multiplier, whose elimination restores the local gauge potential.

### Two-form gauge field

↑ **Parent:** [Gauge field](#gauge-field)

An antisymmetric tensor potential $B$ has gauge transformation $B\mapsto B+d\alpha$, where $\alpha$ is a one-form. Its field strength is the three-form $H=dB$, invariant because $d^2=0$. The [Kalb–Ramond field](string-theory.md#kalb-ramond-field) is the string-theory example.

#### Gauge-invariant string coupling to a two-form

↑ **Parent:** [Two-form gauge field](#two-form-gauge-field)

The coupling $q\int_\Sigma X^*B$ integrates the pullback of the [two-form gauge field](#two-form-gauge-field) over the [string worldsheet](string-theory.md#worldsheet). Its gauge variation is $q\int_{\partial\Sigma}X^*\alpha$, by [Stokes theorem](calculus.md#stokes-theorem). It therefore vanishes for a closed worldsheet, while an open surface requires suitable boundary fields or boundary-state transformations.

### Gauss law constraint in gauge theory

↑ **Parent:** [Gauge field](#gauge-field)

The time component of a gauge field's equation of motion constrains the spatial fields and their momenta. In a [Yang-Mills theory](#yang-mills-theory) it has the covariant form $D_iE_i=\rho$; its Abelian form is [Gauss's law](electromagnetism.md#gauss-s-law). Time-dependent [collective coordinates](classical-field-theory-soliton.md#collective-coordinate-of-a-soliton) of a [gauge-theory soliton](classical-field-theory-soliton.md#gauge-theory-soliton) require a temporal gauge field, or an equivalent horizontal projection, that satisfies this constraint before the kinetic metric is read from the action.

### Gauge boson

↑ **Parent:** [Gauge field](#gauge-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gauge_boson)

A gauge boson is a spin-one quantum excitation of a gauge field. Each generator of the gauge group supplies one gauge-boson species before symmetry breaking.

#### Gauge-boson mass matrix

↑ **Parent:** [Gauge boson](#gauge-boson)

With canonically normalized [gauge field](#gauge-field) [kinetic terms](quantum-field-theory.md#kinetic-term), a gauge-boson mass matrix is the real symmetric matrix of coefficients in the displayed quadratic mass term. Its [eigenvalues](linear-operator-theory.md#eigenvalue) are squared physical [gauge boson](#gauge-boson) masses. For a complex [scalar field](quantum-field-theory.md#scalar-field) vacuum $\Phi_0$ in the [Higgs mechanism](standard-model.md#higgs-mechanism), $(M^2)_{ab}=2\operatorname{Re}[(g_aT_a\Phi_0)^\dagger(g_bT_b\Phi_0)]$. Thus for real $x_a$, $x^TM^2x=2\|\sum_a x_ag_aT_a\Phi_0\|^2\geq0$: it is a [Gram matrix](linear-algebra.md#gram-matrix) and a [positive semidefinite matrix](linear-algebra.md#positive-semidefinite-matrix). An unbroken generator annihilates the [vacuum expectation value](quantum-field-theory.md#vacuum-expectation-value) and lies in its null space. Diagonalizing the matrix identifies the massive and massless field combinations.

##### Gauge-boson mass rank from a real scalar vacuum

↑ **Parent:** [Gauge-boson mass matrix](#gauge-boson-mass-matrix)

With positive canonical kinetic terms and nonzero coupling $g$, expansion of the covariant scalar kinetic term gives the displayed [gauge-boson mass matrix](#gauge-boson-mass-matrix). It is a [Gram matrix](linear-algebra.md#gram-matrix): for real $c_a$, $c^TM_A^2c=g^2|\sum_ac_aT_a\phi_0|^2$. Its kernel is the [Lie algebra](lie-algebra.md) of the [stabilizer subgroup](group-theory.md#stabilizer-subgroup) of the vacuum. Thus its rank is $\dim G-\dim H$, and exactly that many gauge-field combinations acquire nonzero squared masses. Removal of these gauge-orbit directions does not remove accidental zero eigenvalues of the [scalar mass matrix](quantum-field-theory.md#scalar-mass-matrix) on the transverse complement.

### Gauge group

↑ **Parent:** [Gauge field](#gauge-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gauge_group)

The gauge group is the group of local internal symmetries. Its [Lie algebra](lie-algebra.md) labels the gauge-boson species, while a matter field carries a representation of the group.

#### Gauge generator

↑ **Parent:** [Gauge group](#gauge-group)

A [gauge generator](#gauge-generator) is the representation [matrix](vector-space.md#matrix) of a basis element of the [Lie algebra](lie-algebra.md) of a continuous [gauge group](#gauge-group) on a specified set of fields. For Hermitian generators $T^a$, an infinitesimal transformation is $\delta\phi=i\alpha^aT^a\phi$, and $[T^a,T^b]=if^{ab}{}_cT^c$. [Gauge invariance](#gauge-invariance) of a [superpotential](supersymmetry.md#superpotential) consequently requires $W_i(T^a)^i{}_j\phi^j=0$ for each generator.

#### Gauge group representation

↑ **Parent:** [Gauge group](#gauge-group)

A gauge group representation specifies how a matter field transforms under a [gauge group](#gauge-group). It fixes the gauge charges and whether gauge-invariant mass terms can pair a field with a field in the conjugate [group representation](representation-theory.md#group-representation).

### Gauge coupling

↑ **Parent:** [Gauge field](#gauge-field)

A gauge coupling is the constant multiplying the gauge potential in the [gauge covariant derivative](#gauge-covariant-derivative). Its normalization depends on that of the Lie-algebra generators; each simple or Abelian factor of a gauge algebra may have an independent coupling.

#### Canonical normalization of a gauge kinetic term

↑ **Parent:** [Gauge coupling](#gauge-coupling)

For $\mathcal L=-\mathcal N F^a_{\mu\nu}F^{a\mu\nu}/4$ with $\mathcal N>0$, rescale $\mathcal A^a=\sqrt{\mathcal N}A^a$ and $g_c=g/\sqrt{\mathcal N}$. The [gauge field strength](#gauge-field-strength) then has canonical component normalization. Masses inferred from matter couplings must use $g_c$, not an unnormalized coefficient. A matrix-trace convention $\operatorname{Tr}(t^at^b)=\mathcal N\delta^{ab}$ fixes this factor.

### Wilson line

↑ **Parent:** [Gauge field](#gauge-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wilson_line)

A Wilson line is the path-ordered parallel transporter

$$
U(y,x)=\mathcal P\exp\left(ig\int_x^y A_\mu(z)\,dz^\mu\right).
$$

Under a gauge transformation $V$, it transforms as $U(y,x)\mapsto V(y)U(y,x)V(x)^{-1}$.

#### Wilson loop

↑ **Parent:** [Wilson line](#wilson-line)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wilson_loop)

With [gauge covariant derivative](#gauge-covariant-derivative) $D=d+A$, a Wilson loop is the [matrix trace](linear-algebra.md#matrix-trace) in a specified [group representation](representation-theory.md#group-representation) of [parallel transport](fiber-bundle.md#parallel-transport) around a closed curve. The [holonomy of a connection](fiber-bundle.md#holonomy) changes by conjugation under [gauge equivalence of principal connections](fiber-bundle.md#gauge-equivalence-of-principal-connections), so its trace is gauge-invariant. It detects global connection data even when the local [gauge curvature](#gauge-field-strength) is zero.

#### Wilson-line gauge transformation

↑ **Parent:** [Wilson line](#wilson-line)

Expanding a short [Wilson line](#wilson-line) determines the inhomogeneous gauge-potential transformation. For $V=1+i\alpha$ and Hermitian generators,

$$
A_\mu\mapsto A_\mu+\frac1g\partial_\mu\alpha+i[\alpha,A_\mu].
$$

### Gauge-field transformation law

↑ **Parent:** [Gauge field](#gauge-field)

For $D_\mu=\partial_\mu+A_\mu$ and a matter field transforming as $\phi\mapsto g\phi$, covariance of $D_\mu\phi$ requires

$$
A_\mu\mapsto gA_\mu g^{-1}-(\partial_\mu g)g^{-1}.
$$

### Gauge field strength

↑ **Parent:** [Gauge field](#gauge-field)

The curvature of a non-Abelian gauge field is $F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu+[A_\mu,A_\nu]$. It satisfies $[D_\mu,D_\nu]=F_{\mu\nu}$ and transforms as $F_{\mu\nu}\mapsto gF_{\mu\nu}g^{-1}$.

#### Spinor decomposition of gauge curvature

↑ **Parent:** [Gauge field strength](#gauge-field-strength)

In complexified four-dimensional space-time, antisymmetry gives

$$
F_{AA'BB'}=\epsilon_{AB}\varphi_{A'B'}+\epsilon_{A'B'}\varphi_{AB},
$$

where both [gauge curvature](#gauge-field-strength) [two-component spinors](connection-1-form.md#two-component-spinor) are symmetric. The two summands are the two duality components. In the convention where the primed symmetric part is self-dual, the [Anti-self-dual Yang-Mills equations](classical-field-theory-soliton.md#anti-self-dual-yang-mills-equations) are $\varphi_{A'B'}=0$. Equivalently $\pi^{A'}\pi^{B'}F_{AA'BB'}=0$ for every primed [two-component spinor](connection-1-form.md#two-component-spinor) $\pi$, since a quadratic polynomial vanishing for every [two-component spinor](connection-1-form.md#two-component-spinor) has all symmetric coefficients zero.

#### Cross-product convention for an adjoint covariant derivative

↑ **Parent:** [Gauge field strength](#gauge-field-strength)

For the ordinary three-dimensional cross product, $D_\mu\Phi=\partial_\mu\Phi+eA_\mu\times\Phi$ requires $F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu+eA_\mu\times A_\nu$. This follows from $[A\times,B\times]=(A\times B)\times$. The same curvature then transforms covariantly under local rotations. Using a minus sign in its quadratic term while retaining the plus sign in $D$ breaks local gauge invariance: a pure gauge for $D$ has $F_+=0$ but generally $F_-=-2eA_\mu\times A_\nu\ne0$. Reversing both signs is an alternative consistent convention.

#### CP transformation of non-Abelian field strength

↑ **Parent:** [Gauge field strength](#gauge-field-strength)

For $\mathcal F_{\mu\nu}=\partial_\mu\mathcal A_\nu-\partial_\nu\mathcal A_\mu+ig[\mathcal A_\mu,\mathcal A_\nu]$, the [CP transformation of a non-Abelian gauge connection](#cp-transformation-of-a-non-abelian-gauge-connection) gives $\mathcal F_{\mu\nu}^{CP}(x)=-P_\mu{}^\alpha P_\nu{}^\beta\mathcal F_{\alpha\beta}^T(x_P)$. The commutator term transforms with the same sign as the derivative terms because $[X^T,Y^T]=-[X,Y]^T$. A simple component check is $F_{0i}\mapsto+F_{0i}^T$ and $F_{ij}\mapsto-F_{ij}^T$, evaluated at the reflected point.

#### Scaled right Maurer-Cartan gauge potential

↑ **Parent:** [Gauge field strength](#gauge-field-strength)

Write $B_i=(\partial_i g)g^{-1}$ and use $D=d+A$. The right [Maurer-Cartan equation](lie-theory.md#maurer-cartan-equation) gives $\partial_xB_y-\partial_yB_x=[B_x,B_y]$. Thus $A_i=\alpha B_i$ has the displayed [gauge curvature](#gauge-field-strength). Both $\alpha=0$ and $\alpha=-1$ are universally flat; the latter is a [pure gauge potential](#pure-gauge-potential). Commuting $B_x,B_y$ give additional flat cases. For the opposite convention $D=d-A$, the corresponding component formula instead has $\alpha(1-\alpha)$.

##### Circular curvature zeros for a planar SU2 exponential

↑ **Parent:** [Scaled right Maurer-Cartan gauge potential](#scaled-right-maurer-cartan-gauge-potential)

For $g=\exp(-i(x\sigma_1+y\sigma_2)/2)$, write $r=\sqrt{x^2+y^2}$ and $n=(x/r,y/r,0)$. The [Pauli matrix multiplication law](algebra.md#pauli-matrix-multiplication-law) gives $g=\cos(r/2)I-i\sin(r/2)n\cdot\sigma$. On the circles $r=2\pi k$, the angular derivative is zero, so the two Cartesian right logarithmic derivatives are proportional to the same radial generator. They commute, giving zero [gauge curvature](#gauge-field-strength) for every scaling constant. At the origin their [commutator](lie-algebra.md#commutator) is $-i\sigma_3/2$, which need not vanish.

#### Pure gauge potential

↑ **Parent:** [Gauge field strength](#gauge-field-strength)

With [gauge covariant derivative](#gauge-covariant-derivative) $D=d+A$, transforming the zero connection by a smooth group-valued map $g$ gives $A=-dg\,g^{-1}$. This potential has zero [gauge curvature](#gauge-field-strength). A flat potential is locally of this form; global reconstruction can also depend on topology and holonomy. The sign changes when the definition of the covariant derivative changes.

#### Gauge-theory Bianchi identity

↑ **Parent:** [Gauge field strength](#gauge-field-strength)

The [Jacobi identity](lie-algebra.md#jacobi-identity) for [gauge covariant derivatives](#gauge-covariant-derivative) gives $D_{[\mu}F_{\nu\rho]}=0$. In four dimensions this is $D_\mu\widetilde F^{\mu\nu}=0$, with $\widetilde F^{\mu\nu}=\frac12\varepsilon^{\mu\nu\rho\sigma}F_{\rho\sigma}$. It holds independently of the [Yang-Mills equations](#yang-mills-equations).

### Flat connection

↑ **Parent:** [Gauge field](#gauge-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Flat_connection)

A flat connection has vanishing curvature. On a simply connected patch it is gauge equivalent to the zero connection, because the parallel-transport equation has path-independent solutions.

#### Parallel-frame compatibility criterion

↑ **Parent:** [Flat connection](#flat-connection)

For $D_i=\partial_i+A_i$, compatibility for arbitrary initial vectors is equivalent to zero [gauge curvature](#gauge-field-strength). An invertible parallel [bundle frame](fiber-bundle.md#frame-of-a-vector-bundle) $S$ obeys $D_iS=0$, so $[D_i,D_j]S=F_{ij}S=0$ forces $F_{ij}=0$. Conversely, solve the two ordinary transport equations along one coordinate axis and then along parallel lines. The unused transport residual solves a homogeneous transport equation with zero initial value when the [gauge curvature](#gauge-field-strength) is zero; it therefore vanishes. Thus $A_i=-(\partial_iS)S^{-1}=g^{-1}\partial_i g$ with $g=S^{-1}$. One particular parallel vector requires only $F_{ij}v=0$, a weaker condition.

#### Holonomy representation of a flat connection

↑ **Parent:** [Flat connection](#flat-connection)

The [holonomy](fiber-bundle.md#holonomy) of a [flat connection](#flat-connection) is invariant under based homotopy of loops, giving a [group homomorphism](group-theory.md#group-homomorphism) from the [fundamental group](algebraic-topology.md#fundamental-group) into the structure group after choosing a frame at the base point. Changing that frame conjugates the representation. Its associated bundle is constructed from the universal cover and this monodromy. It differs from the natural representation of a Riemannian holonomy group on a tangent fiber.

#### Framed flat connections and holonomy

↑ **Parent:** [Flat connection](#flat-connection)

For a connected base and a chosen frame at one point, a [flat connection](#flat-connection) gives a representation of the [fundamental group](algebraic-topology.md#fundamental-group) by parallel transport. Conversely, $(\widetilde X\times G)/\pi_1(X)$ with monodromy representation has a flat product connection. Based gauge classes correspond to representations, and unbased classes to conjugacy classes. On a fixed underlying bundle only representations whose associated flat bundle has that bundle type are allowed.

// Destination: geometry-and-topology.bigb

### Gauge covariant derivative

↑ **Parent:** [Gauge field](#gauge-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gauge_covariant_derivative)

A gauge covariant derivative combines an ordinary derivative with a [gauge field](#gauge-field) so that differentiating a field preserves its gauge-transformation law. In a matrix representation one common convention is $D_\mu=\partial_\mu-igA_\mu$.

#### Invariant integration by parts for a gauge covariant derivative

↑ **Parent:** [Gauge covariant derivative](#gauge-covariant-derivative)

For the [Killing form](lie-algebra.md#killing-form) or another [invariant bilinear form on a Lie algebra](lie-algebra.md#invariant-bilinear-form-on-a-lie-algebra),

$$
\partial_\mu\kappa(X,Y)=\kappa(D_\mu X,Y)+\kappa(X,D_\mu Y).
$$

The connection terms cancel by invariance. Thus, for compactly supported variations, a [gauge covariant derivative](#gauge-covariant-derivative) can be moved to the other factor in an integral with a minus sign, just as an ordinary derivative.

// Target: quantum-field-theory.bigb

#### Conjugate gauge covariant derivative

↑ **Parent:** [Gauge covariant derivative](#gauge-covariant-derivative)

If a [complex scalar field](scalar-field-theory.md#complex-scalar-field) uses $D_\mu\phi=(\partial_\mu+ieA_\mu)\phi$, its conjugate uses $(D_\mu\phi)^*=(\partial_\mu-ieA_\mu)\phi^*$. Under $\phi\mapsto e^{-ie\alpha}\phi$ and $A\mapsto A+d\alpha$, the two derivatives transform with opposite phases. Their product is gauge invariant. Applying the same plus-charge operator to both factors leaves an unwanted term proportional to $\partial_\mu\alpha$ and fails [gauge invariance](#gauge-invariance).

#### Gauge covariance of a scalar covariant derivative

↑ **Parent:** [Gauge covariant derivative](#gauge-covariant-derivative)

With $D_\mu=\partial_\mu+R(A_\mu)$ and $\delta_X A_\mu=-\epsilon\partial_\mu X+\epsilon[X,A_\mu]$, the derivative terms in $\delta_X(D_\mu\phi)$ cancel. The remaining terms combine using $R([X,A_\mu])=[R(X),R(A_\mu)]$, so the covariant derivative transforms in the same [Lie algebra representation](lie-algebra.md#lie-algebra-representation) as the scalar. This convention absorbs the gauge coupling into the connection.

#### Adjoint covariant derivative

↑ **Parent:** [Gauge covariant derivative](#gauge-covariant-derivative)

On an adjoint-valued field $X$, the covariant derivative is $D_\mu X=\partial_\mu X+[A_\mu,X]$. If $X\mapsto gXg^{-1}$, then $D_\mu X\mapsto g(D_\mu X)g^{-1}$.

##### Adjoint gauge variation for a positive-sign covariant derivative

↑ **Parent:** [Adjoint covariant derivative](#adjoint-covariant-derivative)

Choose the [gauge covariant derivative](#gauge-covariant-derivative) $D_\mu=\partial_\mu+igA_\mu$ and matter transformation $\phi'=h\phi$. Covariance $D'_\mu\phi'=hD_\mu\phi$ forces $A'_\mu=hA_\mu h^{-1}+(i/g)(\partial_\mu h)h^{-1}$. For $h=1-ig\omega+O(\omega^2)$, expansion gives the displayed [adjoint covariant derivative](#adjoint-covariant-derivative) variation. With an orthonormal Hermitian Lie-algebra basis, $\delta A^a_\mu=\partial_\mu\omega^a-gf^{abc}A^b_\mu\omega^c$. Thus Lorenz-gauge variation is $\delta(\partial\cdot A)=\partial\cdot\mathscr D\omega$. Choosing the [Faddeev-Popov operator](#faddeev-popov-operator) as $\mathcal M=-\partial\cdot\mathscr D$, with its field-independent sign absorbed in normalization, gives ghost action $-\bar c\partial\cdot\mathscr D c$; consistent propagator and vertex signs follow from this choice.

##### Gauge-covariant integration by parts

↑ **Parent:** [Adjoint covariant derivative](#adjoint-covariant-derivative)

For Lie-algebra-valued fields and a constant [invariant bilinear form on a Lie algebra](lie-algebra.md#invariant-bilinear-form-on-a-lie-algebra), the connection terms in the displayed identity cancel. Indeed, invariance gives $\kappa([A,Y],Z)+\kappa(Y,[A,Z])=0$. Ordinary [integration by parts](calculus.md#integration-by-parts) then yields $\int\kappa(D_\mu Y,Z)=-\int\kappa(Y,D_\mu Z)$ when boundary terms vanish, for example for compactly supported variations. This preserves covariance in variational calculations of [Yang-Mills equations](#yang-mills-equations).

### Gauge invariance

↑ **Parent:** [Gauge field](#gauge-field)

Gauge invariance is invariance under local changes of gauge representative. Gauge-invariant observables depend only on the physical gauge orbit.

A [gauge theory](quantum-field-theory.md#gauge-theory) uses this redundancy to describe the same physical state by different field representatives.

#### Symmetry up to gauge transformation

↑ **Parent:** [Gauge invariance](#gauge-invariance)

A spatial transformation is a symmetry of a gauge-field configuration when its pullback lies in the [gauge orbit](#gauge-orbit) of the original configuration. It need not fix a particular representative. For a planar vortex, rotation changes its winding phase and a constant $U(1)$ transformation compensates. For a [hedgehog ansatz for a monopole](classical-field-theory-soliton.md#hedgehog-ansatz-for-a-monopole), a spatial rotation is compensated by the corresponding internal adjoint $SU(2)$ rotation. Gauge-invariant densities remain invariant without choosing a special gauge.

#### Gauge-invariant operator

↑ **Parent:** [Gauge invariance](#gauge-invariance)

A local field combination is a gauge-invariant operator when its gauge representations and charges combine to a singlet. In an [effective field theory](quantum-field-theory.md#effective-field-theory), such operators may be multiplied by [Wilson coefficients](quantum-field-theory.md#wilson-coefficient) and inverse powers of a heavy scale. Multiplication by $\phi^\dagger\phi$ preserves the invariance of an existing Higgs Yukawa operator.

#### Gauge redundancy

↑ **Parent:** [Gauge invariance](#gauge-invariance)

Gauge redundancy means that multiple field configurations or polarization representatives describe the same physical state. Physical amplitudes must be unchanged when an external polarization is shifted by a pure-gauge component.

#### Gauge orbit

↑ **Parent:** [Gauge invariance](#gauge-invariance)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gauge_orbit)

A gauge orbit is the set of all field configurations related by gauge transformations. Every point on one orbit represents the same physical gauge configuration.

### Abelian gauge theory

↑ **Parent:** [Gauge field](#gauge-field)

An Abelian gauge theory has a commutative [gauge group](#gauge-group). Its [gauge field strength](#gauge-field-strength) has no commutator term, so the pure gauge Lagrangian has no cubic or quartic gauge-boson self-interactions.

<h4 id="u-1-gauge-symmetry">U(1) gauge symmetry</h4>

↑ **Parent:** [Abelian gauge theory](#abelian-gauge-theory)

For $D_\mu=\partial_\mu+ieA_\mu$, the local U(1) transformation is

$$
\psi\mapsto e^{ie\chi}\psi,
\qquad
A_\mu\mapsto A_\mu-\partial_\mu\chi.
$$

##### Scalar electrodynamics

↑ **Parent:** [U(1) gauge symmetry](#u-1-gauge-symmetry)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Scalar_electrodynamics)

A [charged scalar field](quantum-field-theory.md#charged-scalar-field) coupled to an Abelian [gauge field](#gauge-field) through $D_\mu=\partial_\mu-iea_\mu$. Under $\phi\mapsto e^{i\alpha}\phi$ and $a_\mu\mapsto a_\mu+e^{-1}\partial_\mu\alpha$, its [gauge covariant derivative](#gauge-covariant-derivative) transforms with the same phase. The potential determines whether the perturbative spectrum has a massless [photon](quantum-mechanics.md#photon) or exhibits the [Higgs mechanism](standard-model.md#higgs-mechanism).

###### Two-charge scalar gauge potential

↑ **Parent:** [Scalar electrodynamics](#scalar-electrodynamics)

With scalar charges $e$ and $2e$, both $\psi$ and $\phi^2$ transform with phase $e^{2i\alpha}$. Therefore $M^2|\psi-b\phi^2|^2$ is a gauge-invariant potential term. It contains a nonzero direct cubic interaction $-M^2(b\psi^*\phi^2+\mathrm{h.c.})$. Adding positive quadratic and quartic modulus terms gives a real bounded-below potential. All expanded interactions have field degree at most four.

##### Large gauge transformation

↑ **Parent:** [U(1) gauge symmetry](#u-1-gauge-symmetry)

A large gauge transformation does not approach the identity at the relevant spatial or asymptotic boundary. Although it leaves the local field strength unchanged, its boundary charge can act nontrivially on physical states and constrain soft limits through a [Ward identity](perturbative-quantum-field-theory.md#ward-identity).

### Yang-Mills theory

↑ **Parent:** [Gauge field](#gauge-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Yang-Mills_theory)

Yang-Mills theory is the non-Abelian gauge theory with field strength

$$
F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu-ig[A_\mu,A_\nu].
$$

Under an infinitesimal gauge transformation it transforms covariantly as $\delta F_{\mu\nu}=-ig[F_{\mu\nu},\alpha]$.

#### Invariant bilinear-form construction of a Yang-Mills action

↑ **Parent:** [Yang-Mills theory](#yang-mills-theory)

If a [Lie algebra](lie-algebra.md) has an invariant symmetric nondegenerate form $h$, its curvature $F$ transforms in the [Adjoint representation](lie-algebra.md#adjoint-representation-of-a-lie-algebra) and $\mathcal L=-h(F_{\mu\nu},F^{\mu\nu})/4$ is gauge invariant. Infinitesimal invariance follows from $h([\theta,X],Y)+h(X,[\theta,Y])=0$. For compact generators with $\operatorname{tr}(T^aT^b)=\delta^{ab}/2$, this gives $-\operatorname{tr}(F_{\mu\nu}F^{\mu\nu})/2=-F^a_{\mu\nu}F^{a\mu\nu}/4$. An arbitrary index contraction is not gauge invariant for an arbitrary [Lie algebra](lie-algebra.md).

#### Theta vacuum

↑ **Parent:** [Yang-Mills theory](#yang-mills-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Theta_vacuum)

A theta vacuum is a coherent state $|\theta\rangle=\sum_n e^{in\theta}|n\rangle$ formed from gauge vacua of different winding numbers. Large gauge transformations shift $n$ and act on this state by a phase. The [Yang-Mills theta term](#yang-mills-theta-term) gives the corresponding weighting of spacetime topological sectors.

##### Yang-Mills theta term

↑ **Parent:** [Theta vacuum](#theta-vacuum)

In four dimensions the Yang-Mills theta term is proportional to $\theta\,\operatorname{Tr}(F_{\mu\nu}{}^\star F^{\mu\nu})$. Its density is a total derivative, but nontrivial gauge-field topology can make its spacetime integral physically relevant in the quantum theory.

The term weights topological sectors and supplies the angle labeling a [theta vacuum](#theta-vacuum).

###### Boundary variation of the Yang-Mills theta term

↑ **Parent:** [Yang-Mills theta term](#yang-mills-theta-term)

For $F=dA+A\wedge A$, the [gauge-theory Bianchi identity](#gauge-theory-bianchi-identity) is $DF=0$ and the variation is $\delta F=D\delta A$. The graded product rule for the [covariant exterior derivative](fiber-bundle.md#exterior-covariant-derivative) gives the displayed boundary integral. Thus a constant-coefficient [Yang-Mills theta term](#yang-mills-theta-term) leaves the bulk [Yang-Mills equations](#yang-mills-equations) unchanged, but can change the boundary variational condition. Its four-form density is exactly [gauge-invariant](#gauge-invariance) by conjugation of $F$ and cyclicity of the [matrix trace](linear-algebra.md#matrix-trace), even if the gauge parameter is nonzero on the boundary. Gauge changes of a local [Chern-Simons 3-form](geometry-and-topology.md#chern-simons-3-form) must not be confused with gauge changes of this globally defined curvature density.

###### CP parity of the Yang-Mills theta density

↑ **Parent:** [Yang-Mills theta term](#yang-mills-theta-term)

The color-contracted density $\epsilon^{\mu\nu\rho\sigma}F^a_{\mu\nu}F^a_{\rho\sigma}$ is even under [charge conjugation](quantum-field-theory.md#charge-conjugation) and odd under [parity](quantum-mechanics.md#parity). In matrix form the two charge-conjugation signs cancel and transposition leaves the [trace](linear-algebra.md#matrix-trace) of the product unchanged. [Parity](quantum-mechanics.md#parity) contributes its orientation-reversing determinant to the four-index [Levi-Civita symbol](calculus.md#levi-civita-symbol). Thus the density is [CP](quantum-field-theory.md#cp-symmetry) odd. A generic fixed coefficient violates [CP symmetry](quantum-field-theory.md#cp-symmetry); being a local total derivative does not eliminate effects from nontrivial gauge topology.

###### QCD theta angle

↑ **Parent:** [Yang-Mills theta term](#yang-mills-theta-term)

The physical QCD theta angle is $\bar\theta=\theta_{\rm QCD}+\arg\det(M_uM_d)$. An anomalous chiral quark rotation shifts the two terms oppositely, so only their sum is invariant.

###### Strong CP problem

↑ **Parent:** [QCD theta angle](#qcd-theta-angle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Strong_CP_problem)

The strong CP problem asks why the physical QCD theta angle is smaller than roughly $10^{-10}$ even though no Standard Model symmetry requires this small value.

<h6 id="peccei-quinn-theory">Peccei–Quinn theory</h6>

↑ **Parent:** [Strong CP problem](#strong-cp-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Peccei–Quinn_theory)

Peccei–Quinn theory promotes the physical QCD theta angle to a dynamical field through an anomalous global $U(1)$ symmetry. Nonperturbative QCD drives its vacuum expectation value to a CP-conserving minimum.

###### Axion

↑ **Parent:** [Peccei–Quinn theory](#peccei-quinn-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Axion)

The axion is the pseudo-Goldstone boson of spontaneously broken Peccei–Quinn symmetry. Its QCD-generated potential dynamically relaxes the physical theta angle toward zero.

###### Electroweak theta angle

↑ **Parent:** [Yang-Mills theta term](#yang-mills-theta-term)

The electroweak theta angle multiplies the $SU(2)_L$ topological density. In the renormalizable Standard Model it is unphysical because an anomalous baryon-plus-lepton rephasing shifts it, but explicit baryon-plus-lepton violation can make an invariant combination observable.

###### Chern-Simons current

↑ **Parent:** [Yang-Mills theta term](#yang-mills-theta-term)

The Chern-Simons current satisfies $\partial_\mu K^\mu=\operatorname{Tr}(F_{\mu\nu}{}^\star F^{\mu\nu})$. It is not gauge invariant even though its divergence is.

In four dimensions this current is dual to the degree-three [Chern-Simons form](geometry-and-topology.md#chern-simons-form).

#### Cubic and quartic Yang-Mills self-interactions

↑ **Parent:** [Yang-Mills theory](#yang-mills-theory)

With $D_\mu=\partial_\mu+igA_\mu$ and $[T^a,T^b]=if_{abc}T^c$, the [Yang-Mills field strength](#gauge-field-strength) has the sign $F_{\mu\nu}^a=G_{\mu\nu}^a-gf_{abc}A_\mu^bA_\nu^c$. Expanding $-F^a_{\mu\nu}F^{a\mu\nu}/4$ gives a cross term $(g/2)G^a_{\mu\nu}f_{abc}A^{b\mu}A^{c\nu}$; antisymmetry makes its two derivative terms equal, proving the cubic expression. Squaring the nonlinear term gives the quartic expression. Both vertices arise from the same [gauge coupling](#gauge-coupling), rather than independent free parameters.

#### Yang-Mills vacuum

↑ **Parent:** [Yang-Mills theory](#yang-mills-theory)

A classical zero-energy Yang-Mills vacuum has vanishing spatial gauge curvature. On simply connected space it is pure gauge, $A=h^{-1}dh$. If gauge transformations approach the identity at spatial infinity, the boundary-normalized gauge maps on compactified space $S^3$ have integer winding, recorded by the [Chern-Simons number of a gauge field](geometry-and-topology.md#chern-simons-number-of-a-gauge-field). Transformations of nonzero winding relate these representatives; quantum theta states encode their tunnelling and large-gauge-transformation phases.

#### Invariant gauge kinetic form

↑ **Parent:** [Yang-Mills theory](#yang-mills-theory)

In $\mathcal L=-g_{ab}F^a_{\mu\nu}F^{b\mu\nu}/4$, only the symmetric part of $g$ contributes. A constant symmetric [bilinear form](linear-algebra.md#bilinear-form) gives local [gauge invariance](#gauge-invariance) precisely when it is an [invariant bilinear form on a Lie algebra](lie-algebra.md#invariant-bilinear-form-on-a-lie-algebra), because the [gauge field strength](#gauge-field-strength) transforms in the [Adjoint representation](lie-algebra.md#adjoint-representation-of-a-lie-algebra). A nondegenerate kinetic term requires a [nondegenerate bilinear form](linear-algebra.md#nondegenerate-bilinear-form); positivity of the Hamiltonian is an additional condition. For a compact simple real [Lie algebra](lie-algebra.md), $-\kappa$ is positive definite, and a positive multiple supplies the usual positive-energy convention with Minkowski signature $(+---)$.

#### Non-Abelian gauge transformation

↑ **Parent:** [Yang-Mills theory](#yang-mills-theory)

For the convention $D_\mu=\partial_\mu+gA_\mu$, a [gauge group](#gauge-group) transformation $\Phi\mapsto R\Phi$ acts on the [gauge potential](#gauge-field) by $A_\mu\mapsto RA_\mu R^{-1}-g^{-1}(\partial_\mu R)R^{-1}$. The [gauge field strength](#gauge-field-strength) transforms by conjugation. This makes $D_\mu\Phi$ transform in the same [gauge group representation](#gauge-group-representation) as $\Phi$.

#### Yang-Mills equations

↑ **Parent:** [Yang-Mills theory](#yang-mills-theory)

Stationarity of the [Yang-Mills action](#yang-mills-action) in the absence of sources gives $D_\mu F^{\mu\nu}=0$, using the adjoint [gauge covariant derivative](#gauge-covariant-derivative). This dynamical equation differs from the geometric [gauge-theory Bianchi identity](#gauge-theory-bianchi-identity).

##### Covariant wave equation for the Yang-Mills field strength

↑ **Parent:** [Yang-Mills equations](#yang-mills-equations)

Apply $D^\rho$ to the [gauge-theory Bianchi identity](#gauge-theory-bianchi-identity) and commute it through the other derivatives using $[D_\mu,D_\nu]X=[F_{\mu\nu},X]$. The [Yang-Mills equations](#yang-mills-equations) remove the differentiated divergences. The two remaining [commutator](lie-algebra.md#commutator) terms both equal $[F_\mu{}^\rho,F_{\nu\rho}]$, proving the displayed nonlinear [covariant wave equation for the Yang-Mills field strength](#covariant-wave-equation-for-the-yang-mills-field-strength) on flat spacetime.

// Target: special-relativity.bigb

#### Yang-Mills theory coupled to an arbitrary scalar representation

↑ **Parent:** [Yang-Mills theory](#yang-mills-theory)

For a compact simple [gauge group](#gauge-group), use $B=-\kappa$ on its algebra and an averaged positive invariant [Hermitian form](linear-algebra.md#hermitian-form) $h$ on any supplied finite-dimensional complex representation. With anti-Hermitian connection and signature $(+---)$, $\mathcal L=-B(\mathcal F_{\mu\nu},\mathcal F^{\mu\nu})/(4g^2)+h(D_\mu\Phi,D^\mu\Phi)-V(\Phi)$ is [gauge-invariant](#gauge-invariance) whenever $V$ is invariant. A real scalar representation instead has a symmetric form and kinetic prefactor $1/2$.

##### Adjoint Yang-Mills-Higgs trace variation

↑ **Parent:** [Yang-Mills theory coupled to an arbitrary scalar representation](#yang-mills-theory-coupled-to-an-arbitrary-scalar-representation)

Take $D_\mu X=\partial_\mu X+[A_\mu,X]$, signature $(+---)$ and the [trace](linear-algebra.md#matrix-trace) [Lagrangian density](quantum-field-theory.md#lagrangian-density) $\operatorname{Tr}(F_{\mu\nu}F^{\mu\nu})/4-\operatorname{Tr}(D_\mu\Phi D^\mu\Phi)/2+m^2\operatorname{Tr}(\Phi^2)/2$. The variation of the [gauge curvature](#gauge-field-strength) is $D_\mu\delta A_\nu-D_\nu\delta A_\mu$. Cyclicity of the [trace](linear-algebra.md#matrix-trace) and covariant [integration by parts](calculus.md#integration-by-parts) give gauge coefficient $-D_\mu F^{\mu\nu}+[D^\nu\Phi,\Phi]$ and scalar coefficient $D_\mu D^\mu\Phi+m^2\Phi$. Their vanishing gives the displayed [Euler-Lagrange field equations](quantum-field-theory.md#euler-lagrange-field-equation). In static [temporal gauge](#temporal-gauge) at zero mass they reduce to $D_jF_{ji}=[\Phi,D_i\Phi]$ and $D_iD_i\Phi=0$.

// Destination: integrable-systems.bigb

##### Gauge-invariant scalar potential

↑ **Parent:** [Yang-Mills theory coupled to an arbitrary scalar representation](#yang-mills-theory-coupled-to-an-arbitrary-scalar-representation)

A real potential $V$ for a [scalar field](quantum-field-theory.md#scalar-field) is invariant when $V(R(U)\Phi)=V(\Phi)$ for every gauge transformation. In a unitary representation, $m^2h(\Phi,\Phi)+\lambda h(\Phi,\Phi)^2$ is always an example. Particular representations may admit additional invariant interactions.

#### Killing-form Yang-Mills Lagrangian

↑ **Parent:** [Yang-Mills theory](#yang-mills-theory)

For a real compact semisimple algebra, $B=-\kappa$ is a positive internal metric. With signature $(+---)$ and connection $D_\mu=\partial_\mu+A_\mu$, the healthy Lagrangian is $\mathcal L=-B(F_{\mu\nu},F^{\mu\nu})/(4g^2)=\kappa(F_{\mu\nu},F^{\mu\nu})/(4g^2)$. [Gauge invariance](#gauge-invariance) follows from Killing-form invariance and $\delta_XF=\epsilon[X,F]$. The physical [Hamiltonian](classical-mechanics.md#hamiltonian) density is $[B(E_i,E_i)+B(B_i,B_i)]/(2g^2)$ after imposing the [Gauss law constraint in gauge theory](#gauss-law-constraint-in-gauge-theory) and treating the spatial boundary flux appropriately. An Abelian factor needs a separate positive invariant metric because its [Killing form](lie-algebra.md#killing-form) vanishes.

#### Killing-form Lagrangian for an adjoint scalar

↑ **Parent:** [Yang-Mills theory](#yang-mills-theory)

An adjoint scalar has [adjoint covariant derivative](#adjoint-covariant-derivative) $D_\mu\phi=\partial_\mu\phi+[A_\mu,\phi]$. A symmetric [invariant bilinear form on a Lie algebra](lie-algebra.md#invariant-bilinear-form-on-a-lie-algebra) contracts the [gauge field strength](#gauge-field-strength) and scalar kinetic terms to give [gauge invariance](#gauge-invariance). On a [compact real form](semisimple-lie-algebra.md#compact-real-form-of-a-complex-semisimple-lie-algebra) the positive internal metric is $-\kappa$, because the [Killing form](lie-algebra.md#killing-form) itself is negative definite; complex scalar components require the associated Hermitian pairing. The Killing form is degenerate on Abelian factors, where another invariant metric is needed for a nondegenerate kinetic term.

<h4 id="su-2-gauge-theory">SU(2) gauge theory</h4>

↑ **Parent:** [Yang-Mills theory](#yang-mills-theory)

An SU(2) gauge theory is a [Yang-Mills theory](#yang-mills-theory) with gauge group $SU(2)$. In its defining representation the generators are $T^a=\sigma^a/2$, and its structure constants are the Levi-Civita symbols $\epsilon^{abc}$.

##### SU2 gauge self-interaction vertices

↑ **Parent:** [SU(2) gauge theory](#su-2-gauge-theory)

For field strength $F^a_{\mu\nu}=f^a_{\mu\nu}-g\epsilon^{abc}A_\mu^bA_\nu^c$, the square produces $\mathcal L_3=g\epsilon^{abc}(\partial_\mu A_\nu^a)A^{b\mu}A^{c\nu}$ and $\mathcal L_4=-g^2\epsilon^{abc}\epsilon^{ade}A_\mu^bA_\nu^cA^{d\mu}A^{e\nu}/4$. The cubic [Feynman vertex](perturbative-quantum-field-theory.md#interaction-vertex) has one derivative; the quartic one has none. No higher pure-gauge vertex occurs.

##### Complete breaking by an SU2 scalar doublet

↑ **Parent:** [SU(2) gauge theory](#su-2-gauge-theory)

A nonzero complex fundamental doublet has trivial stabilizer in the gauged $SU(2)$. Its three angular directions are gauge directions, absorbed by the [Higgs mechanism](standard-model.md#higgs-mechanism). For vacuum $\phi_0=(0,v/\sqrt2)^T$, the three gauge bosons have equal mass $gv/2$; one radial scalar remains. There is no unbroken photon-like gauge generator in this theory.

###### Scalar interactions after complete SU2 breaking

↑ **Parent:** [Complete breaking by an SU2 scalar doublet](#complete-breaking-by-an-su2-scalar-doublet)

In [unitary gauge](standard-model.md#unitary-gauge), $\phi=(0,(v+h)/\sqrt2)^T$ gives $\frac{g^2}{8}(v+h)^2A_\mu^aA^{a\mu}$. With potential $\frac{\lambda}{2}(\phi^\dagger\phi-v^2/2)^2$, the physical scalar has $m_h^2=\lambda v^2$ and interactions $-\lambda vh^3/2-\lambda h^4/8$. This normalization matters when extracting both masses and identical-leg [Feynman vertices](perturbative-quantum-field-theory.md#interaction-vertex).

<h5 id="su-2-gauge-theory-with-an-adjoint-higgs-field">SU(2) gauge theory with an adjoint Higgs field</h5>

↑ **Parent:** [SU(2) gauge theory](#su-2-gauge-theory)

A real [scalar field](quantum-field-theory.md#scalar-field) in the [Adjoint representation](lie-algebra.md#adjoint-representation-of-a-lie-algebra) can have a nonzero [vacuum expectation value](quantum-field-theory.md#vacuum-expectation-value), leaving one massless and two massive [gauge bosons](#gauge-boson). This breaking differs from [electroweak symmetry breaking](standard-model.md#electroweak-symmetry-breaking) by a complex [Higgs doublet](standard-model.md#higgs-field).

###### 't Hooft electromagnetic tensor

↑ **Parent:** [SU(2) gauge theory with an adjoint Higgs field](#su-2-gauge-theory-with-an-adjoint-higgs-field)

For a nonvanishing adjoint [Higgs field](standard-model.md#higgs-field), put $n=\Phi/|\Phi|$. If an oriented orthonormal internal basis satisfies $[e_a,e_b]=\kappa\varepsilon_{abc}e_c$, the displayed tensor is gauge invariant. In a gauge with $n=e_3$, write $A_j=a_j^ae_a$; the transverse quadratic terms cancel, leaving $\mathcal F_{jk}=\partial_ja_k^3-\partial_ka_j^3$. Hence it is a [closed differential form](differential-form.md#closed-differential-form) wherever $\Phi\ne0$. Under [trace normalization of su(2)](lie-algebra.md#trace-normalization-of-su-2) with $-\operatorname{tr}(XY)$, $\kappa^2=2$ and the commutator term has coefficient $1/2$. With $-2\operatorname{tr}(XY)$, its coefficient is one. Omitting this normalization factor generally destroys closure.

###### Physical charged-vector Lagrangian for an adjoint SU2 Higgs model

↑ **Parent:** [SU(2) gauge theory with an adjoint Higgs field](#su-2-gauge-theory-with-an-adjoint-higgs-field)

For a real triplet potential $\lambda(|\phi|^2-v^2)^2/8$ and canonical gauge coupling $g_c$, [unitary gauge](standard-model.md#unitary-gauge) gives one neutral [Higgs mode](quantum-field-theory.md#higgs-mode), two oppositely charged massive vectors and one massless Abelian vector. The scalar kinetic contribution is $\tfrac12(\partial\eta)^2+g_c^2(v+\eta)^2W^+W^-$, and its potential is $\lambda v^2\eta^2/2+\lambda v\eta^3/2+\lambda\eta^4/8$. This potential convention is distinct from using $\lambda(|\phi|^2-v^2)^2/4$.

###### Scalar vertices of an adjoint triplet Higgs model

↑ **Parent:** [Physical charged-vector Lagrangian for an adjoint SU2 Higgs model](#physical-charged-vector-lagrangian-for-an-adjoint-su2-higgs-model)

For a real triplet with potential $\lambda(\Phi^2-v^2)^2/8$, unitary gauge gives $\Phi=(0,0,v+h)$ and scalar interaction terms $-\lambda vh^3/2-\lambda h^4/8+2e^2vhW^+W^-+e^2h^2W^+W^-$. Functional differentiation, including identical-field multiplicities, gives vertices $-3i\lambda v$, $-3i\lambda$, $2ie^2v g_{\mu\nu}$ and $2ie^2g_{\mu\nu}$ respectively. The physical scalar is neutral under the residual U(1), so there are no $hAA$ or $hhAA$ vertices.

<h4 id="su-3-gauge-theory">SU(3) gauge theory</h4>

↑ **Parent:** [Yang-Mills theory](#yang-mills-theory)

An SU(3) gauge theory has eight gauge fields, one for each generator of $SU(3)$. A vacuum expectation value of one scalar in the [fundamental representation](semisimple-lie-algebra.md#fundamental-representation) generically leaves an $SU(2)$ subgroup unbroken.

<h5 id="fundamental-higgs-breaking-of-su-3-to-su-2">Fundamental-Higgs breaking of SU(3) to SU(2)</h5>

↑ **Parent:** [SU(3) gauge theory](#su-3-gauge-theory)

For a complex fundamental scalar with vacuum expectation value proportional to $(0,0,v)$, the stabilizer is the $SU(2)$ acting on the first two components. Five broken generators produce five massive vector bosons, while three gauge bosons remain massless and one radial scalar remains physical.

#### Yang-Mills action

↑ **Parent:** [Yang-Mills theory](#yang-mills-theory)

On an oriented Riemannian four-manifold, one positive Euclidean convention is

$$
S_{\rm YM}=-\frac1{g_{\rm YM}^2}
\int\operatorname{Tr}(F\wedge{}^\star F)
$$

for anti-Hermitian gauge fields.

##### Conformal invariance of four-dimensional Yang-Mills action

↑ **Parent:** [Yang-Mills action](#yang-mills-action)

Under $g\mapsto\Omega^2g$ in dimension $d$, the [Hodge star](differential-form.md#hodge-star-operator) on $p$-forms scales by $\Omega^{d-2p}$. For gauge [gauge curvature](#gauge-field-strength), $d=4,p=2$, so the star and the action $-g_{\rm YM}^{-2}\int\operatorname{tr}(F\wedge *F)$ are unchanged. Dilation therefore changes the [instanton size modulus](classical-field-theory-soliton.md#instanton-size-modulus) without changing the classical action. Quantum running of the coupling can break this classical scale invariance.

##### Derivative-squared Yang-Mills action

↑ **Parent:** [Yang-Mills action](#yang-mills-action)

This [gauge-invariant](#gauge-invariance) higher-derivative density has equation

$$
2D_\mu D_\lambda D^\lambda F^{\mu\nu}+[F_{\rho\sigma},D^\nu F^{\rho\sigma}]=0.
$$

The extra commutator comes from varying the connection inside the [adjoint covariant derivative](#adjoint-covariant-derivative): $\delta(D_\mu F_{\nu\rho})=D_\mu\delta F_{\nu\rho}+[\delta A_\mu,F_{\nu\rho}]$. Two uses of [gauge-covariant integration by parts](#gauge-covariant-integration-by-parts) give the first term, and Killing-form invariance gives the second. In an abelian limit it reduces to $\Box\partial_\mu F^{\mu\nu}=0$. Keeping the covariant derivative order is essential because their commutator is curvature.

##### Power of the Yang-Mills invariant

↑ **Parent:** [Yang-Mills action](#yang-mills-action)

For a semisimple gauge algebra and positive integer $p$, this [gauge-invariant](#gauge-invariance) density yields $D_\mu(s^{p-1}F^{\mu\nu})=0$. The curvature variation $\delta F_{\mu\nu}=D_\mu\delta A_\nu-D_\nu\delta A_\mu$ gives $\delta s=4\kappa(D_\mu\delta A_\nu,F^{\mu\nu})$, and [gauge-covariant integration by parts](#gauge-covariant-integration-by-parts) proves the equation. More generally a density $f(s)$ gives $D_\mu(f'(s)F^{\mu\nu})=0$. The product form retains the equation at zeros of $s$; dividing by $s$ can discard solutions.

#### Yang-Mills gauge transformation

↑ **Parent:** [Yang-Mills theory](#yang-mills-theory)

For $D_\mu=\partial_\mu-igA_\mu$ and matter transforming as $\psi\mapsto U\psi$, a Yang-Mills connection transforms inhomogeneously while its curvature transforms by conjugation, $F_{\mu\nu}\mapsto UF_{\mu\nu}U^{-1}$.

##### Gauge transformation in the derivative-plus-connection convention

↑ **Parent:** [Yang-Mills gauge transformation](#yang-mills-gauge-transformation)

For $D_\mu=\partial_\mu+A_\mu$ and $\delta\phi=\Lambda\phi$, covariance requires $\delta A_\mu=-\partial_\mu\Lambda+[\Lambda,A_\mu]$. Expanding $[D_\mu,D_\nu]$ gives $F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu+[A_\mu,A_\nu]$, and operator Jacobi gives $\delta F_{\mu\nu}=[\Lambda,F_{\mu\nu}]$. An invariant internal quadratic form makes its Yang-Mills kinetic contraction gauge invariant. Couplings and factors of i are absorbed into the connection in this convention.

##### Infinitesimal gauge transformation with an anti-Hermitian connection

↑ **Parent:** [Yang-Mills gauge transformation](#yang-mills-gauge-transformation)

With $D_\mu=\partial_\mu+\rho(\mathcal A_\mu)$ and $\Phi\mapsto R(U)\Phi$, a local $U=1+\epsilon$ gives $\delta\mathcal A_\mu=-\partial_\mu\epsilon+[\epsilon,\mathcal A_\mu]$, $\delta\Phi=\rho(\epsilon)\Phi$ and $\delta\mathcal F_{\mu\nu}=[\epsilon,\mathcal F_{\mu\nu}]$. Derivative terms cancel in $\delta(D_\mu\Phi)=\rho(\epsilon)D_\mu\Phi$. Here the [gauge coupling](#gauge-coupling) is absorbed into the connection.

#### Gluon propagator

↑ **Parent:** [Yang-Mills theory](#yang-mills-theory)

A gluon propagator is the inverse of the gauge-fixed quadratic Yang-Mills operator. It carries Lorentz and adjoint color indices and depends on the gauge-fixing condition, while gauge-invariant observables do not.

#### Anomaly (physics)

↑ **Parent:** [Yang-Mills theory](#yang-mills-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Anomaly_(physics))

A quantum anomaly is the failure of a classical symmetry to survive quantization because the functional measure or regulator cannot preserve it.

##### Global anomaly

↑ **Parent:** [Anomaly (physics)](#anomaly-physics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Global_anomaly)

A global anomaly obstructs invariance of a quantum theory under a topologically nontrivial symmetry transformation even when infinitesimal local anomaly tests vanish. The [Witten SU(2) anomaly](#witten-su-2-anomaly) is one example; global gravitational anomalies are another class.

<h6 id="witten-su-2-anomaly">Witten SU(2) anomaly</h6>

↑ **Parent:** [Global anomaly](#global-anomaly)

The Witten SU(2) anomaly is a four-dimensional global gauge anomaly present for an odd number of left-handed Weyl fermion doublets. A consistent SU(2) gauge theory must have an even number modulo the corresponding representation index.

##### Gauge anomaly

↑ **Parent:** [Anomaly (physics)](#anomaly-physics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gauge_anomaly)

A gauge anomaly destroys a gauge redundancy needed to remove unphysical states and makes the quantum gauge theory inconsistent unless the anomaly cancels.

###### Anomaly cancellation

↑ **Parent:** [Gauge anomaly](#gauge-anomaly)

Anomaly cancellation is the vanishing of every gauge and mixed gauge-gravitational anomaly after summing over all chiral fermions. It is a consistency condition for a quantum gauge theory.

###### Standard Model anomaly cancellation

↑ **Parent:** [Anomaly cancellation](#anomaly-cancellation)

In each Standard Model generation, quark and lepton hypercharges cancel the $SU(3)_c^3$, $SU(3)_c^2U(1)_Y$, $SU(2)_L^2U(1)_Y$, $U(1)_Y^3$, and mixed gauge-gravitational anomalies. The four left-handed $SU(2)_L$ doublets also avoid the global Witten anomaly.

###### One-generation hypercharge anomaly traces

↑ **Parent:** [Standard Model anomaly cancellation](#standard-model-anomaly-cancellation)

In normalization $Q=T_3+Y$, one [Standard Model](standard-model.md) generation has left quark and lepton doublet hypercharges $1/6$ and $-1/2$, and right singlet hypercharges $2/3,-1/3,-1$. Including colour multiplicity, $\operatorname{tr}_LY=6/6-2/2=0$. On every left doublet $T_3^2=I/4$, and all right fields have $T_3=0$, so the mixed weak-hypercharge [gauge anomaly](#gauge-anomaly) vanishes. The cubic left trace is $6(1/6)^3+2(-1/2)^3=-2/9$, and the right trace is $3(2/3)^3+3(-1/3)^3+(-1)^3=-2/9$. Their difference is zero, proving generation-by-generation cancellation of these two anomalies.

###### Mixed gauge-gravitational anomaly

↑ **Parent:** [Gauge anomaly](#gauge-anomaly)

A mixed gauge-gravitational anomaly has one gauge-current insertion and two stress-tensor insertions. For a four-dimensional $U(1)$ symmetry its coefficient is the sum of the left-handed Weyl-fermion charges, with right-handed fermions counted as left-handed conjugates.

##### Chiral anomaly

↑ **Parent:** [Anomaly (physics)](#anomaly-physics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chiral_anomaly)

The chiral anomaly is the quantum nonconservation of a classically conserved axial current in a gauge-field background.

###### Axial current

↑ **Parent:** [Chiral anomaly](#chiral-anomaly)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Axial_current)

For massless Dirac fermions, the classical axial current is $J_A^\mu=\bar\psi\gamma^\mu\gamma^5\psi$. The chiral anomaly makes its divergence proportional to $F_{\mu\nu}{}^\star F^{\mu\nu}$.

###### Axial charge

↑ **Parent:** [Axial current](#axial-current)

An [axial charge](#axial-charge) is the spatial integral of the time component of an [axial current](#axial-current). For a [Dirac field](#dirac-field) and an internal generator $t$, it is $\int\psi^\dagger\gamma_5t\psi\,d^3x$. Its canonical action rotates left- and right-handed fields oppositely. It is conserved only when the current divergence and flux at infinity vanish; [Dirac masses](#dirac-mass-term) and a [chiral anomaly](#chiral-anomaly) can obstruct conservation. The nonsinglet [quark](standard-model.md#quark) generators have no color anomaly and obey the [nonsinglet axial charge algebra of quark densities](standard-model.md#nonsinglet-axial-charge-algebra-of-quark-densities).

###### Axial derivative coupling and parity

↑ **Parent:** [Axial current](#axial-current)

For an ordinary [scalar field](quantum-field-theory.md#scalar-field), its derivative is a polar covector, while the [axial current](#axial-current) is a pseudovector. Their contraction is invariant under the [Proper orthochronous Lorentz group](special-relativity.md#proper-orthochronous-lorentz-group) but changes sign under [parity](quantum-mechanics.md#parity). If the field is a [pseudoscalar](quantum-mechanics.md#pseudoscalar), the extra transformation sign makes this coupling parity even. In four spacetime dimensions its [mass dimension](perturbative-quantum-field-theory.md#mass-dimension) is five, so Lorentz invariance alone does not imply power-counting [renormalizability](perturbative-quantum-field-theory.md#renormalizable-quantum-field-theory).

###### Axial-current divergence for scalar and pseudoscalar backgrounds

↑ **Parent:** [Axial current](#axial-current)

For $\mathcal L=\bar\psi(i\not\partial-S+iP\gamma^5)\psi$, with real scalar backgrounds $S,P$, the [Dirac equation](#dirac-equation) is $(i\not\partial-S+iP\gamma^5)\psi=0$ and the [adjoint Dirac equation](#adjoint-dirac-equation) is $i(\partial_\mu\bar\psi)\gamma^\mu+S\bar\psi-iP\bar\psi\gamma^5=0$. Use $\{\gamma^5,\gamma^\mu\}=0$ and $(\gamma^5)^2=1$ in the derivative of $j_5^\mu=\bar\psi\gamma^\mu\gamma^5\psi$ to obtain the displayed classical identity. Taking $S=m+g\phi$ and $P=G\Phi$ includes both scalar and [Hermitian](hilbert-space.md#hermitian-operator) pseudoscalar [Yukawa couplings](standard-model.md#yukawa-interaction).

###### Axial-current divergence for a pseudoscalar Yukawa interaction

↑ **Parent:** [Axial current](#axial-current)

For $\mathcal L_{\rm int}=-g\phi\bar\psi\gamma^5\psi$, the variational [Dirac equation](#dirac-equation) and [adjoint Dirac equation](#adjoint-dirac-equation) are $(i\not\partial-m-g\phi\gamma^5)\psi=0$ and $i(\partial_\mu\bar\psi)\gamma^\mu+m\bar\psi+g\phi\bar\psi\gamma^5=0$. Substitute these into the [derivative](calculus.md#derivative) of $j_5^\mu=\bar\psi\gamma^\mu\gamma^5\psi$. Anticommuting the chirality matrix past $\gamma^\mu$ gives two identical mass terms and two identical interaction terms, proving the displayed identity. These are classical field equations; the formula does not assert an unrenormalized quantum composite-operator identity. With Hermitian coupling $g=i g_P$, the second term is $-2g_P\phi\bar\psi\psi$.

###### Axial-current squared interaction

↑ **Parent:** [Axial current](#axial-current)

Since the [chirality matrix](algebra.md#chirality-matrix) commutes with spinor Lorentz generators, $j_5^\mu=\bar\psi\gamma^\mu\gamma^5\psi$ transforms as a vector under proper [Lorentz transformations](special-relativity.md#lorentz-transformation) and as a [pseudovector](vector-space.md#pseudovector) under [parity](quantum-mechanics.md#parity). Contracting two copies gives the [Lorentz scalar](special-relativity.md#lorentz-scalar) $j_{5\mu}j_5^\mu$; the extra [parity](quantum-mechanics.md#parity) signs cancel. [Lorentz invariance](special-relativity.md#lorentz-invariance) of this interaction does not require current conservation.

###### Chiral transformation

↑ **Parent:** [Axial current](#axial-current)

A chiral transformation rotates a Dirac field by $\psi\mapsto e^{i\alpha\gamma^5}\psi$. A massless Dirac kinetic term is invariant under a global rotation, while a mass term is not.

##### 't Hooft anomaly

↑ **Parent:** [Anomaly (physics)](#anomaly-physics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/'t_Hooft_anomaly)

A 't Hooft anomaly is an obstruction to gauging a global symmetry. It is preserved by renormalization-group flow and constrains possible infrared phases.

###### 't Hooft anomaly matching

↑ **Parent:** ['t Hooft anomaly](#t-hooft-anomaly)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/'t_Hooft_anomaly_matching)

't Hooft anomaly matching requires the massless infrared degrees of freedom, topological sector, or symmetry-breaking pattern to reproduce every anomaly of an unbroken global symmetry measured in the ultraviolet theory.

### Gauge fixing

↑ **Parent:** [Gauge field](#gauge-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gauge_fixing)

Gauge fixing removes the degeneracy among gauge-equivalent field configurations so that the kinetic operator has an inverse propagator.

#### R-xi gauge

↑ **Parent:** [Gauge fixing](#gauge-fixing)

For the Abelian [Higgs mechanism](standard-model.md#higgs-mechanism) with scalar phase $\chi$ and vector mass $m$, take $\mathcal L_{\rm gf}=-(\partial\cdot A+\xi m\chi)^2/(2\xi)$ when the scalar kinetic mixing is $-mA_\mu\partial^\mu\chi$. The cross term cancels this mixing after integration by parts. The resulting vector [propagator](quantum-field-theory.md#propagator) is

$$
D_{\mu\nu}(k)=\frac{-i}{k^2-m^2+i0}\left(g_{\mu\nu}-(1-\xi)\frac{k_\mu k_\nu}{k^2-\xi m^2+i0}\right).
$$

At fixed finite $\xi$ it decays as $1/k^2$. Would-be [Goldstone bosons](critical-phenomenon.md#goldstone-boson) and the required [Faddeev-Popov ghosts](#faddeev-popov-ghost) remain in intermediate calculations; [BRST symmetry](#brst-symmetry) identifies the physical states and ensures cancellation of unphysical modes. The limit $\xi\to\infty$ gives the [unitary gauge](standard-model.md#unitary-gauge) propagator and is not uniform in ultraviolet momentum.

#### Regular gauge slice

↑ **Parent:** [Gauge fixing](#gauge-fixing)

A gauge condition $F(x)=0$ is regular at a representative $x_0$ if its derivative along the [gauge orbit](#gauge-orbit) is an invertible [matrix](vector-space.md#matrix). The [inverse function theorem](calculus.md#inverse-function-theorem) then makes the gauge-condition values valid local coordinates along that orbit. A unique zero without this regularity is insufficient: the translation action on the line with $F(x)=x^3$ has a unique zero but a zero derivative there. Multiple regular intersections give a [Gribov ambiguity](#gribov-ambiguity) rather than a globally unique slice.

#### Light cone gauge

↑ **Parent:** [Gauge fixing](#gauge-fixing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Light_cone_gauge)

In gauge field theory its standard form is $A^+=n_\mu A^\mu=0$ for a fixed null direction $n$. A light-cone gauge uses [light-cone coordinates](special-relativity.md#light-cone-coordinates) to fix a longitudinal variable, often choosing $x^+$ as the evolution parameter for a [relativistic particle phase-space action](classical-mechanics.md#relativistic-particle-phase-space-action). Related field gauges set selected minus components to zero when a field has the required [gauge invariance](#gauge-invariance). A massive field without that gauge freedom must instead eliminate dependent components through its equations of motion.

#### Gauge-fixed action

↑ **Parent:** [Gauge fixing](#gauge-fixing)

A [gauge-fixed action](#gauge-fixed-action) supplements a gauge-invariant action with a term imposing the gauge condition and with [Faddeev-Popov ghost fields](#faddeev-popov-ghost) representing the [Faddeev-Popov determinant](#faddeev-popov-determinant). A local gauge condition gives local differential operators and a local action.

#### Dynamical gauge-fixing parameter

↑ **Parent:** [Gauge fixing](#gauge-fixing)

If a real nonzero field $\xi(x)$ appears in the Lorentzian density $-F_{ab}F^{ab}/4+(\partial_aA^a)^2/(2\xi)$ and is varied, its algebraic [Euler-Lagrange equation](analysis.md#euler-lagrange-equation) is $-(\partial_aA^a)^2/(2\xi^2)=0$. Hence it imposes the [Lorenz gauge](electromagnetism.md#lorenz-gauge-condition) condition on real classical fields. Varying $A_b$ gives $\partial_aF^{ab}-\partial^b[(\partial\cdot A)/\xi]=0$, including derivatives of $\xi$. This constrained field theory differs from holding the gauge parameter fixed in a [Gaussian functional integral](quantum-field-theory.md#gaussian-functional-integral).

#### Nonlinear Abelian gauge fixing

↑ **Parent:** [Gauge fixing](#gauge-fixing)

For an [Abelian gauge theory](#abelian-gauge-theory) with $A_\mu\mapsto A_\mu+\partial_\mu\alpha$, a nonlinear gauge functional $F[A]$ has [Faddeev-Popov determinant](#faddeev-popov-determinant) $\det(\delta F[A+\partial\alpha]/\delta\alpha)$. This operator can depend on $A$ even though the [Adjoint representation](lie-algebra.md#adjoint-representation-of-a-lie-algebra) of $U(1)$ is trivial. Consequently [Faddeev-Popov ghost fields](#faddeev-popov-ghost) need not decouple in a nonlinear Abelian gauge, unlike a field-independent linear gauge condition.

##### Quadratic Abelian gauge fixing

↑ **Parent:** [Nonlinear Abelian gauge fixing](#nonlinear-abelian-gauge-fixing)

For $\delta A_\mu=\partial_\mu\omega$, the real quadratic gauge functional varies by $(\Box+2A\cdot\partial)\omega$. Its [Faddeev-Popov operator](#faddeev-popov-operator) depends on the [gauge field](#gauge-field), producing a ghost-gauge vertex even in an [Abelian gauge theory](#abelian-gauge-theory). With $\Psi=\int\bar c(F[A]+\xi h/2)$, a consistent left [BRST symmetry](#brst-symmetry) convention gives $s\Psi=hF+\xi h^2/2-\bar c(\Box+2A\cdot\partial)c$. The auxiliary-field integral at $\xi=0$ imposes the exact condition; finite $\xi$ gives a weighted gauge condition. This real functional is distinct from a [complex quadratic Abelian gauge condition](#complex-quadratic-abelian-gauge-condition).

##### Complex quadratic Abelian gauge condition

↑ **Parent:** [Nonlinear Abelian gauge fixing](#nonlinear-abelian-gauge-fixing)

The formal variation of this condition is $\delta F=(\partial^2+2iA\cdot\partial)\alpha$. Thus its [Faddeev-Popov ghost field](#faddeev-popov-ghost) operator can be chosen as $\mathcal O_A=-\partial^2-2iA\cdot\partial$. With $D_\mu=\partial_\mu+iA_\mu$, one has $D^2=\partial^2+2iA\cdot\partial+iF[A]$, so $\mathcal O_A=-D^2$ on the formal gauge slice. The [reality obstruction for a complex Euclidean gauge condition](#reality-obstruction-for-a-complex-euclidean-gauge-condition) prevents interpreting this slice as an ordinary real Euclidean [gauge fixing](#gauge-fixing) without an additional complex-contour prescription.

###### Ghost-scalar determinant cancellation in a complex quadratic gauge

↑ **Parent:** [Complex quadratic Abelian gauge condition](#complex-quadratic-abelian-gauge-condition)

A massless complex bosonic [charged scalar field](quantum-field-theory.md#charged-scalar-field) with $D_\mu=\partial_\mu+iA_\mu$ contributes $[\det(-D^2)]^{-1}$ to a Gaussian background-field integral. A [Faddeev-Popov ghost field](#faddeev-popov-ghost) pair contributes $\det\mathcal O_A$. On the formal [complex quadratic Abelian gauge condition](#complex-quadratic-abelian-gauge-condition), $\mathcal O_A=-D^2$, so the two determinants cancel and their effective-action contributions sum to zero. Use matching regulators, boundary conditions and removed zero modes. This is a formal cancellation of closed loops; the [reality obstruction for a complex Euclidean gauge condition](#reality-obstruction-for-a-complex-euclidean-gauge-condition) precludes deducing that physical [scalar quantum electrodynamics](#scalar-electrodynamics) has no quantum effects.

###### Reality obstruction for a complex Euclidean gauge condition

↑ **Parent:** [Complex quadratic Abelian gauge condition](#complex-quadratic-abelian-gauge-condition)

For real $A_\mu$ in positive-definite Euclidean signature, $\partial\cdot A$ is real and $A_\mu A_\mu\ge0$. Therefore $\partial\cdot A+iA^2=0$ forces $A^2=0$, and hence $A=0$. Its only real gauge orbit is the zero-field orbit; a field with nonzero electromagnetic curvature cannot be gauge-transformed to zero. Consequently this complex equation is not an admissible [gauge fixing](#gauge-fixing) for general Hermitian Euclidean [U(1) gauge symmetry](#u-1-gauge-symmetry) configurations. A formal complexified treatment needs a specified contour and cannot be justified by a real delta-functional insertion.

#### Scalar-dependent gauge fixing

↑ **Parent:** [Gauge fixing](#gauge-fixing)

##### Ghost vertex in scalar-dependent gauge fixing

↑ **Parent:** [Scalar-dependent gauge fixing](#scalar-dependent-gauge-fixing)

The [Faddeev-Popov ghost field](#faddeev-popov-ghost) couples to both the [gauge field](#gauge-field) and the [adjoint scalar field](quantum-field-theory.md#adjoint-scalar-field). In a convention with $D_\mu=\partial_\mu+[A_\mu,\cdot]$, the ghost action after [integration by parts](calculus.md#integration-by-parts) contains $f^{abc}(\partial_\mu\bar c^a)A_\mu^b c^c$ and $f^{abc}(n\cdot\partial\bar c^a)\phi^b c^c/\sqrt2$.

##### Free adjoint-scalar propagator in scalar-dependent gauge fixing

↑ **Parent:** [Scalar-dependent gauge fixing](#scalar-dependent-gauge-fixing)

For [gauge fixing](#gauge-fixing) with $F^a=\partial\cdot A^a+(n\cdot\partial\phi^a)/\sqrt2$, integrating out the [Nakanishi-Lautrup field](#nakanishi-lautrup-field) produces gauge-scalar mixing. The [Schur complement](linear-algebra.md#schur-complement) of the free gauge-field kernel cancels the extra $(n\cdot p)^2/2$ in the scalar kernel, leaving $\langle\phi^a(p)\phi^b(-p)\rangle=\delta^{ab}/p^2$. This is independent of the gauge vector $n$, but still depends on the full momentum $p$.

#### Zero mode in field theory

↑ **Parent:** [Gauge fixing](#gauge-fixing)

A zero mode of a quadratic field operator is a nonzero field variation that the operator maps to zero. Infinitesimal pure-gauge variations are zero modes of an unfixed gauge kinetic operator, preventing it from having an inverse propagator.

##### Zero mode of a radiation-era massless scalar

↑ **Parent:** [Zero mode in field theory](#zero-mode-in-field-theory)

For a minimally coupled [massless scalar field](scalar-field-theory.md#massless-scalar-field) in a flat radiation-dominated universe, [conformal time](cosmology.md#conformal-time) gives $a=\alpha\tau$ and $(a\phi)''-\nabla^2(a\phi)=0$. Every nonzero [Fourier mode](fourier-analysis.md#fourier-mode) is therefore a free oscillator divided by $a$. The zero-wavenumber equation instead gives $a\phi_0=A+B\tau$, hence the displayed constant-plus-decaying solution. Substituting $k=0$ into a fixed-amplitude oscillatory formula retains only the $1/a$ term and loses the constant field solution. A truly general solution must include this zero mode or explicitly exclude a homogeneous background.

#### Gribov ambiguity

↑ **Parent:** [Gauge fixing](#gauge-fixing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gribov_ambiguity)

The Gribov ambiguity is the nonperturbative failure of a local gauge condition to intersect every gauge orbit exactly once. Distinct gauge-equivalent fields satisfying the same condition are Gribov copies.

#### Covariant gauge

↑ **Parent:** [Gauge fixing](#gauge-fixing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Covariant_gauge)

Adding $-(\partial_\mu A^\mu)^2/(2\alpha)$ gives a family of Lorentz-covariant gauges; $\alpha=1$ is [Feynman gauge](#feynman-gauge).

##### Gauge-fixed Maxwell kinetic operator

↑ **Parent:** [Covariant gauge](#covariant-gauge)

The Fourier-space quadratic Maxwell kernel after adding $-(\partial_\mu A^\mu)^2/(2\xi)$. For nonzero $\xi$ and non-null [four-momentum](special-relativity.md#four-momentum), its [transverse and longitudinal momentum projectors](quantum-field-theory.md#transverse-and-longitudinal-momentum-projectors) give $K=-k^2(P_T+\xi^{-1}P_L)$ and its inverse is $-(P_T+\xi P_L)/k^2$. The [inversion of the gauge-fixed Maxwell kinetic operator](#inversion-of-the-gauge-fixed-maxwell-kinetic-operator) supplies the [photon propagator](quantum-field-theory.md#photon-propagator) with its vacuum boundary prescription.

##### Landau gauge (quantum field theory)

↑ **Parent:** [Covariant gauge](#covariant-gauge)

The $\xi\to0$ limit of [covariant gauge](#covariant-gauge) fixing by $-(\partial_\mu A^\mu)^2/(2\xi)$. It imposes the divergence condition sharply and gives a transverse [photon propagator](quantum-field-theory.md#photon-propagator). This is distinct from the vector-potential choice called [Landau gauge for a uniform magnetic field](quantum-theory.md#landau-gauge-for-a-uniform-magnetic-field) when computing [Landau levels](quantum-theory.md#landau-level).

###### Landau gauge photon propagator

↑ **Parent:** [Landau gauge (quantum field theory)](#landau-gauge-quantum-field-theory)

The [covariant Landau gauge](#landau-gauge-quantum-field-theory) propagator is the transverse limit of the [inversion of the gauge-fixed Maxwell kinetic operator](#inversion-of-the-gauge-fixed-maxwell-kinetic-operator). Contracting with $k^\mu$ gives zero away from the pole. The [Lorenz gauge](electromagnetism.md#lorenz-gauge-condition) condition still has residual transformations satisfying $\Box\chi=0$, so boundary conditions and the pole prescription complete the choice.

##### Gauge-fixed Yang-Mills Lagrangian in a covariant gauge

↑ **Parent:** [Covariant gauge](#covariant-gauge)

Use $F^a_{\mu\nu}=\partial_\mu A^a_\nu-\partial_\nu A^a_\mu+g f^{abc}A^b_\mu A^c_\nu$ and $(D_\mu c)^a=\partial_\mu c^a+g f^{abc}A^b_\mu c^c$. The [Faddeev-Popov gauge-orbit identity](#faddeev-popov-gauge-orbit-identity) with [Lorenz gauge](electromagnetism.md#lorenz-gauge-condition) function $G^a=\partial^\mu A^a_\mu$, followed by Gaussian averaging of $G^a=f^a$, supplies the quadratic gauge-fixing term. Represent the determinant of $-\partial^\mu D_\mu$ using a [Grassmann Gaussian integral](quantum-field-theory.md#grassmann-gaussian-integral) over a [Faddeev-Popov ghost field](#faddeev-popov-ghost) and [antighost field](#faddeev-popov-antighost-field) to obtain the ghost term. The minus sign in this operator differs by a field-independent determinant factor from the direct gauge-condition Jacobian; it is a consistent antighost convention.

The ghost term equals $(\partial^\mu\bar c^a)(D_\mu c)^a$ up to a boundary term. Thus it contains a [ghost-gluon vertex](#ghost-gluon-vertex) with the sign matching this kinetic convention. An equivalent auxiliary-field form replaces the gauge-fixing term by $B^aG^a+\xi B^aB^a/2$. The [Nakanishi-Lautrup field](#nakanishi-lautrup-field) equation gives $B^a=-G^a/\xi$ and recovers the displayed Lagrangian. With left-acting [BRST transformations](#brst-symmetry) $sA=Dc$, $sc=-g[c,c]/2$, $s\bar c=B$, and $sB=0$, the gauge-fixing and ghost terms together are $s[\bar c^a(G^a+\xi B^a/2)]$.

##### Inversion of the gauge-fixed Maxwell kinetic operator

↑ **Parent:** [Covariant gauge](#covariant-gauge)

[Gauge fixing](#gauge-fixing) removes the noninvertible longitudinal direction of the Maxwell quadratic action. In a gauge with parameter $\xi$, the Fourier kernel is $-k^2\eta^{\mu\nu}+(1-\xi^{-1})k^\mu k^\nu$. Multiplying its inverse by $i$ gives the [photon propagator](quantum-field-theory.md#photon-propagator), with the [Feynman i-epsilon prescription](quantum-field-theory.md#feynman-i-epsilon-prescription). At $\xi=1$ the answer is $-i\eta_{\mu\nu}/(k^2+i0)$.

##### Positive-sign covariant gauge-fixing inverse

↑ **Parent:** [Covariant gauge](#covariant-gauge)

For fixed $\xi\ne0$, the Lorentzian quadratic density $-F^2/4+(\partial\cdot A)^2/(2\xi)$ has momentum kernel $K^{ab}=-p^2\eta^{ab}+(1+1/\xi)p^ap^b$. At $p^2\ne0$ its inverse, defined by $K^{ac}G_{cb}=\delta^a_b$, is $G_{ab}=-\eta_{ab}/p^2+(1+\xi)p_ap_b/(p^2)^2$. A vacuum [photon propagator](quantum-field-theory.md#photon-propagator) is $iG$ with the appropriate [Feynman i-epsilon prescription](quantum-field-theory.md#feynman-i-epsilon-prescription). The usual parameter in the negative-sign [covariant gauge](#covariant-gauge) term is $\alpha=-\xi$, so [Feynman gauge](#feynman-gauge) is $\xi=-1$.

###### Longitudinal gauge propagator contraction

↑ **Parent:** [Positive-sign covariant gauge-fixing inverse](#positive-sign-covariant-gauge-fixing-inverse)

For the [positive-sign covariant gauge-fixing inverse](#positive-sign-covariant-gauge-fixing-inverse), $p^aG_{ab}=\xi p_b/p^2$. It is not identically zero for fixed $\xi\ne0$ and is a nonzero vector at a nonzero non-null [four-momentum](special-relativity.md#four-momentum). Null [momenta](classical-mechanics.md#momentum) require the chosen pole prescription, and individual zero components are possible. The [covariant Landau gauge](#landau-gauge-quantum-field-theory) limit suppresses this longitudinal part. The [Ward identity](perturbative-quantum-field-theory.md#ward-identity) removes longitudinal contributions from physical conserved-current amplitudes.

##### Feynman gauge

↑ **Parent:** [Covariant gauge](#covariant-gauge)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Feynman_gauge)

###### Feynman-gauge Maxwell kinetic density after a boundary-term subtraction

↑ **Parent:** [Feynman gauge](#feynman-gauge)

With $D=\partial_\mu A^\mu$, expand the [Maxwell Lagrangian](electromagnetism.md#maxwell-lagrangian) and its [Feynman gauge](#feynman-gauge) term to find

$$
-\frac14F_{\mu\nu}F^{\mu\nu}-\frac12D^2
=-\frac12\partial_\mu A_\nu\partial^\mu A^\nu+\partial_\mu K^\mu,
\qquad K^\mu=\frac12(A_\nu\partial^\nu A^\mu-A^\mu D).
$$

Commuting [partial derivatives](calculus.md#partial-derivative) verifies the divergence identity. Both densities give $\Box A^\mu=0$ under the usual variational [boundary conditions](differential-equation.md#boundary-condition). Their [canonical momentum](classical-mechanics.md#canonical-momentum) components differ: the original density gives $-F^{0\nu}-\eta^{0\nu}D$, whereas the subtracted density gives $-\dot A^\nu$. Thus a free-photon [momentum](classical-mechanics.md#momentum) expansion using the latter requires a stated boundary-term convention.

###### Boundary-induced canonical transformation in Feynman gauge

↑ **Parent:** [Feynman-gauge Maxwell kinetic density after a boundary-term subtraction](#feynman-gauge-maxwell-kinetic-density-after-a-boundary-term-subtraction)

In mostly-minus signature, adding the [boundary term](calculus.md#boundary-term) $\partial_\mu K^\mu$ with $K^\mu=\frac12(A_\nu\partial^\nu A^\mu-A^\mu\partial_\nu A^\nu)$ to the subtracted [Feynman gauge](#feynman-gauge) density changes $\widetilde\pi^\mu=-\dot A^\mu$ to the displayed [canonical momenta](classical-mechanics.md#canonical-momentum). For fields with vanishing spatial boundary terms, $\int K^0d^3x=\int A_0\partial_iA_i\,d^3x$, whose functional derivatives are these momentum shifts. They depend only on coordinates, so $[A_\mu,\pi^\nu]=i\delta_\mu{}^\nu\delta^3$ is unchanged. The only potentially nonzero mixed momentum bracket is $[\pi^0(x),\pi^i(y)]=i(\partial_{y^i}+\partial_{x^i})\delta^3(x-y)=0$. Thus both density representatives define [canonical commutation relations](quantum-mechanics.md#canonical-commutation-relation), although their momenta must not be equated componentwise.

###### Gupta-Bleuler formalism

↑ **Parent:** [Feynman gauge](#feynman-gauge)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gupta–Bleuler_formalism)

Gupta-Bleuler quantization keeps Lorentz covariance by first quantizing all four photon polarizations in an indefinite inner-product space. The condition $(\partial_\mu A^\mu)^{(+)}|\mathrm{phys}\rangle=0$, followed by quotienting null states, leaves the two transverse physical polarizations.

###### Gupta-Bleuler null-state quotient

↑ **Parent:** [Gupta-Bleuler formalism](#gupta-bleuler-formalism)

Choose $C_{\mathbf p}=a^0_{\mathbf p}-a^3_{\mathbf p}$ with the standard temporal and longitudinal [polarization vectors](#polarization-vector). The physical pre-space is the common kernel of all $C_{\mathbf p}$. In each regulated mode, $a^0$ acts on creator [polynomials](polynomial.md) as $-\partial_{a^{0\dagger}}$ and $a^3$ as $\partial_{a^{3\dagger}}$, so the constraint kernel consists of transverse creator [polynomials](polynomial.md) and [polynomials](polynomial.md) in $C^\dagger=a^{0\dagger}-a^{3\dagger}$. Since $[C,C^\dagger]=0$, these latter excitations remain constrained. They are orthogonal to every constrained state because $\langle\Phi|C^\dagger=\langle C\Phi|=0$. Quotienting this [radical of a Hermitian form](linear-algebra.md#radical-of-a-hermitian-form) leaves only the transverse [bosonic Fock space](quantum-field-theory.md#bosonic-fock-space) with a positive [inner product](linear-algebra.md#inner-product). The constraint alone gives a [positive semidefinite Hermitian form](linear-algebra.md#positive-semidefinite-hermitian-form); quotienting removes its null directions. If starting from finite-particle creator [polynomials](polynomial.md), take the [Hilbert space completion](hilbert-space.md#hilbert-space-completion) of this positive quotient to obtain the physical [Hilbert space](hilbert-space.md).

###### Transverse one-photon physical quotient

↑ **Parent:** [Gupta-Bleuler null-state quotient](#gupta-bleuler-null-state-quotient)

Choose a temporal [polarization vector](#polarization-vector), two transverse [polarization vectors](#polarization-vector) and a spatial longitudinal [polarization vector](#polarization-vector). The [Gupta-Bleuler quantization](#gupta-bleuler-formalism) condition is $(a^0-a^3)|\chi\rangle=0$. Applied to $\sum_\lambda c_\lambda a^{\lambda\dagger}|0\rangle$, it gives $c_3=-c_0$. The remaining temporal-longitudinal excitation $a^{0\dagger}-a^{3\dagger}$ has zero norm and is orthogonal to every constrained state. Its field wavefunction is proportional to the null [four-momentum](special-relativity.md#four-momentum), hence is pure gauge. Quotienting this direction leaves the two positive transverse [photon](quantum-mechanics.md#photon) states. Use [wave packets](wave-equation.md#wave-packet) or a box normalization to avoid treating continuum momentum eigenstates as normalizable vectors.

###### Covariant photon Fock space

↑ **Parent:** [Gupta-Bleuler formalism](#gupta-bleuler-formalism)

The covariant free-photon oscillator construction uses four [polarization vectors](#polarization-vector) and $[a^\lambda,a^{\lambda'\dagger}]=-\eta^{\lambda\lambda'}$. Starting from a positive [Fock vacuum](quantum-field-theory.md#fock-vacuum), it induces an [indefinite Hermitian form](linear-algebra.md#indefinite-hermitian-form) on the multiparticle state space: the temporal oscillator has negative norm while the three spatial oscillators have positive norm. It is therefore not the physical positive [Hilbert space](hilbert-space.md). The [Gupta-Bleuler null-state quotient](#gupta-bleuler-null-state-quotient) selects a positive physical space with two transverse photon polarizations. Continuum [momentum](classical-mechanics.md#momentum) oscillators and their states are understood after smearing or finite-volume regularization.

###### Photon oscillator completeness and canonical brackets

↑ **Parent:** [Covariant photon Fock space](#covariant-photon-fock-space)

With real complete [polarization vectors](#polarization-vector), the [covariant photon Fock space](#covariant-photon-fock-space) oscillator [commutators](lie-algebra.md#commutator) and $\sum_{\lambda,\lambda'}\epsilon_\mu^\lambda\epsilon^{\nu\lambda'}\eta_{\lambda\lambda'}=\delta_\mu{}^\nu$ imply the equal-time [canonical commutation relations](quantum-mechanics.md#canonical-commutation-relation) $[A_\mu(\mathbf x),-\dot A^\nu(\mathbf y)]=i\delta_\mu{}^\nu\delta^3(\mathbf x-\mathbf y)$. The two mixed creation-annihilation terms add; the two coordinate-coordinate or momentum-momentum terms cancel after their polarization sums. The sign of the time-component oscillator is essential to the identity. [Boundary-induced canonical transformation in Feynman gauge](#boundary-induced-canonical-transformation-in-feynman-gauge) explains the momenta for the unsubtracted density.

###### Negative-norm photon state

↑ **Parent:** [Covariant photon Fock space](#covariant-photon-fock-space)

For a temporal [photon](quantum-mechanics.md#photon) [wave packet](wave-equation.md#wave-packet) $|f,0\rangle=\int d^3p\,f(\mathbf p)a_{\mathbf p}^{0\dagger}|0\rangle/(2\pi)^3$, the oscillator [commutator](lie-algebra.md#commutator) gives $\langle f,0|f,0\rangle=-\int d^3p\,|f(\mathbf p)|^2/(2\pi)^3<0$ when $f\ne0$. This is the negative direction of the [indefinite Hermitian form](linear-algebra.md#indefinite-hermitian-form), not the divergent normalization of an unsmeared [momentum eigenstate](quantum-mechanics.md#momentum-eigenstate). It is excluded by the physical condition in [Gupta-Bleuler quantization](#gupta-bleuler-formalism).

##### Gauge-boson propagator

↑ **Parent:** [Covariant gauge](#covariant-gauge)

For the Euclidean covariant gauge term $(\partial_\mu A^\mu)^2/(2\xi)$, the free gauge-boson propagator is

$$
D_{\mu\nu}(k)=\frac1{k^2}\left(\delta_{\mu\nu}+(\xi-1)\frac{k_\mu k_\nu}{k^2}\right).
$$

###### Feynman-gauge adjoint propagator

↑ **Parent:** [Gauge-boson propagator](#gauge-boson-propagator)

With a mostly-plus [metric signature](topology.md#metric-signature), $e^{iS}$, and gauge-fixing term $-(\partial\cdot A)^2/2$, the free adjoint gauge-field kernel is $-p^2\eta_{\mu\nu}\delta_{ab}$. Inverting it gives the displayed [Feynman propagator](quantum-field-theory.md#feynman-propagator). This convention uses the same denominator and sign as a massless real [scalar propagator](scalar-field-theory.md#scalar-propagator).

###### Feynman-gauge photon propagator

↑ **Parent:** [Gauge-boson propagator](#gauge-boson-propagator)

At $\xi=1$, the Euclidean photon propagator is $D_{\mu\nu}(k)=\delta_{\mu\nu}/k^2$. Its Lorentz-index contraction simplifies loop numerators in [quantum electrodynamics](perturbative-quantum-field-theory.md#quantum-electrodynamics).

###### Transverse projector of a vector field

↑ **Parent:** [Gauge-boson propagator](#gauge-boson-propagator)

At a nonzero Euclidean [momentum](classical-mechanics.md#momentum) $k$, the [transverse projector of a vector field](#transverse-projector-of-a-vector-field) is $P_T^{ab}=\delta^{ab}-k^ak^b/k^2$. In a Lorentzian [Minkowski metric](special-relativity.md#minkowski-metric), its mixed-index form is $(P_T)^a{}_b=\delta^a_b-p^ap_b/p^2$, defined for $p^2\ne0$. It obeys $P_Tp=0$ and $P_T^2=P_T$. A nonzero null [four-momentum](special-relativity.md#four-momentum) is insufficient for this particular decomposition because the denominator vanishes.

###### Longitudinal projector of a vector field

↑ **Parent:** [Gauge-boson propagator](#gauge-boson-propagator)

At a nonzero Euclidean [momentum](classical-mechanics.md#momentum) $k$, the [longitudinal projector of a vector field](#longitudinal-projector-of-a-vector-field) is $P_L^{ab}=k^ak^b/k^2$. Its Lorentzian mixed-index form is $(P_L)^a{}_b=p^ap_b/p^2$ for non-null [four-momentum](special-relativity.md#four-momentum). Together with the [transverse projector of a vector field](#transverse-projector-of-a-vector-field), it obeys $P_T+P_L=I$, $P_TP_L=0$, $P_T^2=P_T$, and $P_L^2=P_L$. This formula is not a pointwise decomposition at null [four-momentum](special-relativity.md#four-momentum).

#### Faddeev-Popov determinant

↑ **Parent:** [Gauge fixing](#gauge-fixing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Faddeev-Popov_determinant)

The Faddeev-Popov determinant is the functional Jacobian

$$
\Delta_{\mathrm{FP}}[A]=\det\left(\frac{\delta G(A^\alpha)}{\delta\alpha}\right)_{G=0}
$$

that compensates for the change from integration along a gauge orbit to a gauge-fixing condition $G(A)=0$. It can be represented by a path integral over a [Faddeev-Popov ghost field](#faddeev-popov-ghost) pair.

##### Faddeev-Popov gauge-orbit identity

↑ **Parent:** [Faddeev-Popov determinant](#faddeev-popov-determinant)

Suppose a [gauge fixing](#gauge-fixing) condition intersects each [gauge orbit](#gauge-orbit) once in the local region under consideration, and its linearized [Faddeev-Popov operator](#faddeev-popov-operator) has no residual zero modes after boundary conditions are imposed. The [functional Jacobian](quantum-field-theory.md#functional-jacobian) for changing from the [gauge transformation](electromagnetism.md#gauge-transformation) parameter to the gauge condition gives the displayed identity. Inserting it in a [gauge-invariant](#gauge-invariance) [functional integral](quantum-field-theory.md#functional-measure) allows the integration along the [gauge orbit](#gauge-orbit) to factor out and cancel the formal gauge-group volume. In a perturbative neighborhood the Jacobian's sign or phase is fixed; a field-independent determinant factor is absorbed into normalization. The [Gribov ambiguity](#gribov-ambiguity) prevents treating this local identity as a globally unique gauge choice without further qualifications.

###### Finite-dimensional Faddeev-Popov gauge reduction

↑ **Parent:** [Faddeev-Popov gauge-orbit identity](#faddeev-popov-gauge-orbit-identity)

Assume an invariant volume measure, an invariant integrand and one [regular gauge slice](#regular-gauge-slice) representative per orbit. At that representative, let $M$ be the [Jacobian matrix](calculus.md#jacobian-matrix) of $F$ along the group coordinates, whose [Haar measure](measure-theory.md#haar-measure) is normalized to ordinary coordinate measure at the identity. Changing coordinates from the group parameter to $F$ gives $\int_Gd\mu(g)\,\delta(F(x_g))=1/|\det M(x_0)|$. Multiply by its reciprocal and insert this identity into the original integral. Invariance permits a change of variables $x\mapsto x_g$ for each $g$, factoring out the group volume. The absolute determinant is required for ordinary unoriented real integration; a consistently positive orientation permits writing $\det M$. Infinite group volume is divided out formally or treated with a regulator.

##### Faddeev-Popov operator

↑ **Parent:** [Faddeev-Popov determinant](#faddeev-popov-determinant)

For a gauge condition $\chi[A]=0$, the linearization of $\chi[A+D\omega]$ in the gauge parameter is the Faddeev-Popov operator. Its determinant is represented by [Faddeev-Popov ghost fields](#faddeev-popov-ghost).

##### Faddeev-Popov ghost

↑ **Parent:** [Faddeev-Popov determinant](#faddeev-popov-determinant)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Faddeev–Popov_ghost)

A Faddeev-Popov ghost field is a Grassmann-valued scalar field whose Gaussian functional integral represents the [Faddeev-Popov determinant](#faddeev-popov-determinant). Ghosts occur only on internal lines and cancel unphysical gauge-field contributions.

###### Ghost propagator

↑ **Parent:** [Faddeev-Popov ghost](#faddeev-popov-ghost)

A [ghost propagator](#ghost-propagator) is the two-point function $\langle Tc(x)\bar c(y)\rangle$ of a [Faddeev-Popov ghost field](#faddeev-popov-ghost) and its independent [Faddeev-Popov antighost field](#faddeev-popov-antighost-field). For quadratic action $\int\bar c M c$ and source ordering consistent with that field ordering, the [Grassmann integral](quantum-mechanics.md#berezin-integral) gives $G_c=iM_F^{-1}$. The subscript specifies the causal pole prescription. For the negative derivative kinetic term $-\int\partial\bar c\cdot\partial c$, the Fourier kernel is $M=-p^2$. With signature $(-,+,+,+)$ this gives $G_c=-i/(p^2-i0)$. Field normalization multiplies the inverse kernel accordingly, while an antighost sign redefinition changes propagator and vertex signs together. Anticommuting statistics and loop signs do not turn these auxiliary fields into physical asymptotic particles.

###### Ghost propagator for a negative derivative kinetic term

↑ **Parent:** [Faddeev-Popov ghost](#faddeev-popov-ghost)

With signature $(+---)$ and action $-\int\partial^\mu\bar c\,\partial_\mu c$, integration by parts gives the quadratic kernel $K_c=\Box$, or $-p^2$ in Fourier space. The [Grassmann Gaussian integral](quantum-field-theory.md#grassmann-gaussian-integral) with odd sources gives $Z=\exp[-i\bar\eta K_{c,F}^{-1}\eta]$. Left and right source derivatives, including their insertion factors, yield $\langle Tc\bar c\rangle=iK_{c,F}^{-1}$ and hence the displayed sign. Replacing $\bar c$ by $-\bar c$ changes this propagator and the [ghost-gluon vertex](#ghost-gluon-vertex) together; it is a convention change, not a physical discrepancy.

###### Ghost-gluon vertex

↑ **Parent:** [Faddeev-Popov ghost](#faddeev-popov-ghost)

Expanding the ghost covariant derivative in [Yang-Mills theory](#yang-mills-theory) produces an interaction between the [Faddeev-Popov ghost field](#faddeev-popov-ghost), [Faddeev-Popov antighost field](#faddeev-popov-antighost-field), and gauge boson. For the displayed kinetic convention, Fourier factors $e^{-ipx}$ and all momenta incoming give vertex $-g f^{abc}k_\mu$, where $k$ is the antighost momentum. The [structure constants](algebra.md#structure-constant) encode the [Adjoint representation](lie-algebra.md#adjoint-representation-of-a-lie-algebra). Propagator, vertex, Fourier, and ghost-order conventions must be chosen consistently.

###### One-loop ghost kinetic counterterm in Feynman gauge

↑ **Parent:** [Ghost-gluon vertex](#ghost-gluon-vertex)

For canonically normalized fields with action $-\int[\tfrac14F^2+\tfrac12(\partial\cdot A)^2+\partial\bar c\cdot Dc]$, use signature $(-,+,+,+)$ and incoming Fourier modes $e^{ipx}$. The [ghost-gluon vertex](#ghost-gluon-vertex) is $gp_\mu f_{abc}$ and the [ghost propagator](#ghost-propagator) is $-i/(p^2-i0)$. The open ghost-line [one-particle-irreducible two-point vertex](perturbative-quantum-field-theory.md#one-particle-irreducible-two-point-vertex) at one loop is $ig^2C I_d(p)$, where

$$
I_d(p)=\frac1i\int\frac{d^dk}{(2\pi)^d}\frac{p\cdot k}{[(p-k)^2-i0][k^2-i0]},\qquad I_d(p)\big|_{\mathrm{pole}}=\frac{p^2}{16\pi^2(4-d)}.
$$

A [counterterm](perturbative-quantum-field-theory.md#counterterm) $\mathcal L_{\mathrm{ct}}=-\delta Z_c\,\partial\bar c\cdot\partial c$ inserts $-i\delta Z_c p^2$ and cancels this pole. Equivalently, writing $d=4-2\epsilon$ gives $\delta Z_c=g^2C/(32\pi^2\epsilon)$. There is no closed ghost-loop sign for this open-line graph. The [Feynman i-epsilon prescription](quantum-field-theory.md#feynman-i-epsilon-prescription), Fourier convention and antighost sign must be kept consistent throughout.

###### Faddeev-Popov antighost field

↑ **Parent:** [Faddeev-Popov ghost](#faddeev-popov-ghost)

The Grassmann-odd partner of the [Faddeev-Popov ghost field](#faddeev-popov-ghost) in the gauge-fixing determinant representation. In an auxiliary-field [BRST symmetry](#brst-symmetry) description it obeys $sb=h$, where $h$ is the [Nakanishi-Lautrup field](#nakanishi-lautrup-field). Its ordinary spacetime derivative remains odd, which matters when moving an anticommuting BRST parameter past it.

###### Ghost number

↑ **Parent:** [Faddeev-Popov ghost](#faddeev-popov-ghost)

The additive grading assigns ghost number $+1$ to $c$ and $-1$ to $\bar c$. Physical observables have ghost number zero. This grading is distinct from spin or the [Adjoint representation](lie-algebra.md#adjoint-representation-of-a-lie-algebra).

###### Ghost-number Noether current

↑ **Parent:** [Ghost number](#ghost-number)

For ghost term $-(\partial^\mu\bar c)\cdot D_\mu c$ and the current convention $\delta S=-\int(\partial_\mu\theta)j_G^\mu$, localize $\delta c=\theta c$, $\delta\bar c=-\theta\bar c$. The two differentiated parameters give this current. Its [Noether charge](quantum-field-theory.md#noether-charge) grades ghosts by $+1$ and antighosts by $-1$, up to the corresponding overall generator normalization.

###### Ghost loop

↑ **Parent:** [Faddeev-Popov ghost](#faddeev-popov-ghost)

A ghost loop is a closed cycle of ghost propagators in a [Feynman diagram](perturbative-quantum-field-theory.md#feynman-diagram). Its Grassmann statistics contribute an additional minus sign.

#### Axial gauge

↑ **Parent:** [Gauge fixing](#gauge-fixing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Axial_gauge)

An axial gauge imposes $n^\mu A_\mu=0$ for a fixed vector $n^\mu$. Its Faddeev-Popov operator is $n^\mu D_\mu$; on the strict gauge slice its gauge-field-dependent part vanishes, so its ghosts decouple.

##### Axial-gauge pole prescription

↑ **Parent:** [Axial gauge](#axial-gauge)

The inverse of $n\cdot\partial$ and the [axial-gauge propagator](#axial-gauge-propagator) are singular when $n\cdot k=0$. A pole prescription and residual-gauge boundary conditions specify these inverses. They must be compatible throughout a calculation; formal ghost decoupling alone does not specify them.

##### Axial-gauge propagator

↑ **Parent:** [Axial gauge](#axial-gauge)

In strict [axial gauge](#axial-gauge), the [gauge-boson propagator](#gauge-boson-propagator) obeys $n^\mu D_{\mu\nu}(k)=0$ and contains poles at $n\cdot k=0$. Its contraction with conserved external currents removes the gauge-choice terms. Consistent calculations require an [axial-gauge pole prescription](#axial-gauge-pole-prescription).

#### Temporal gauge

↑ **Parent:** [Gauge fixing](#gauge-fixing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Temporal_gauge)

Temporal gauge sets the time component of a gauge potential to zero, $A_0=0$. The mixed curvature components then reduce to time derivatives of the spatial connection, $F_{0i}=\partial_0A_i$.

#### BRST symmetry

↑ **Parent:** [Gauge fixing](#gauge-fixing)

BRST symmetry is a nilpotent fermionic symmetry of a gauge-fixed action. Its differential $s$ replaces an infinitesimal gauge parameter by the ghost field and satisfies $s^2=0$.

<h5 id="grassmann-valued-su-2-adjoint-bracket">Grassmann-valued SU(2) adjoint bracket</h5>

↑ **Parent:** [BRST symmetry](#brst-symmetry)

For adjoint fields whose coefficients have [Grassmann parity](linear-algebra.md#grassmann-parity), $X\times Y=-(-1)^{|X||Y|}Y\times X$. Thus two odd ghost fields have a symmetric adjoint bracket, and $c\times c$ need not vanish. The [graded Jacobi identity](lie-algebra.md#graded-jacobi-identity) and this symmetry are the algebraic mechanisms behind [BRST nilpotence](#brst-nilpotence).

##### BRST quantization

↑ **Parent:** [BRST symmetry](#brst-symmetry)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/BRST_quantization)

A gauge quantization prescription using a nilpotent [BRST charge](#brst-charge) on the gauge-fixed state space. Physical states are represented by its [BRST cohomology](#brst-cohomology), usually at [ghost number](#ghost-number) zero. Exact states decouple under suitable invariant-measure, boundary and positivity assumptions. Nilpotence alone does not prove positivity of the quotient or select its physical ghost-number sector.

<h6 id="point-particle-faddeev-popov-ghost-action">Point-particle Faddeev–Popov ghost action</h6>

↑ **Parent:** [BRST quantization](#brst-quantization)

For a relativistic particle, the [Hamiltonian](classical-mechanics.md#hamiltonian) gauge parameter changes the [worldline einbein](classical-mechanics.md#worldline-einbein) by its time derivative. Fixing the einbein to a constant therefore gives a [Faddeev-Popov determinant](#faddeev-popov-determinant) of $\partial_t$, represented by anticommuting [FP ghosts](#faddeev-popov-ghost). Gauge zero modes and the [proper-time modulus](classical-mechanics.md#proper-time-modulus) are treated separately. The displayed phase convention gives the odd canonical bracket $\{b,c\}=-i$.

##### BRST nilpotence

↑ **Parent:** [BRST symmetry](#brst-symmetry)

A [BRST charge](#brst-charge) is nilpotent when $Q^2=0$, making [BRST cohomology](#brst-cohomology) well-defined. For the critical [bosonic string theory](string-theory.md#bosonic-string-theory), the matter and ghost [central charges](string-theory.md#central-charge) cancel, $D-26=0$, and the intercept is one. In a ghost convention with a zero-mode linear shift, the shifted total constraint generators, rather than the unshifted ones, obey the centerless [Witt algebra](lie-algebra.md#witt-algebra).

###### Off-shell nilpotence of the Yang-Mills BRST quartet

↑ **Parent:** [BRST nilpotence](#brst-nilpotence)

Using the [graded Leibniz rule](commutative-algebra.md#graded-leibniz-rule), $s^2A=D(sc)+g(Dc)\times c=0$ because $D(c\times c)=2(Dc)\times c$. The [graded Jacobi identity](lie-algebra.md#graded-jacobi-identity) gives $s^2c=g^2(c\times c)\times c/2=0$. [BRST nilpotence](#brst-nilpotence) on the antighost and [Nakanishi-Lautrup field](#nakanishi-lautrup-field) is immediate. No field equations are required.

##### Left-acting BRST differential

↑ **Parent:** [BRST symmetry](#brst-symmetry)

Writing a transformation as $\delta\Phi=\epsilon s\Phi$ with the odd parameter on the left defines this graded derivation convention. For Yang-Mills fields, $sA=Dc$, $sc=-[c,c]/2$, $sb=h$, and $sh=0$. The [Jacobi identity](lie-algebra.md#jacobi-identity) supplies nilpotence; the placement of the odd parameter controls signs in a [Noether current](quantum-field-theory.md#noether-current).

##### Right-acting BRST differential

↑ **Parent:** [BRST symmetry](#brst-symmetry)

A [right-acting BRST differential](#right-acting-brst-differential) obeys the right [graded Leibniz rule](commutative-algebra.md#graded-leibniz-rule). This convention permits $Q\phi=[c,\phi]$ together with $Qc=-[c,c]/2$. Using a left [graded Leibniz rule](commutative-algebra.md#graded-leibniz-rule) with those same two signs does not give a [nilpotent operator](linear-operator-theory.md#nilpotent-linear-map); one of the signs must change.

##### Nakanishi-Lautrup field

↑ **Parent:** [BRST symmetry](#brst-symmetry)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nakanishi-Lautrup_field)

The Nakanishi-Lautrup field is an auxiliary bosonic field used to write gauge fixing as a BRST-exact term. Its algebraic field equation produces the usual quadratic gauge-fixing term.

###### Gaussian gauge fixing with an auxiliary field

↑ **Parent:** [Nakanishi-Lautrup field](#nakanishi-lautrup-field)

Complete the square as $bF+\xi b^2/2=\xi(b+F/\xi)^2/2-F^2/(2\xi)$. Translation of the [Gaussian functional integral](quantum-field-theory.md#gaussian-functional-integral) gives the displayed identity for nonzero $\xi$, with the appropriate oscillatory contour prescription. At $\xi=0$, the [Nakanishi-Lautrup field](#nakanishi-lautrup-field) is a [Lagrange multiplier](mathematical-optimization.md#lagrange-multiplier) imposing the gauge-condition delta functional. This field has no kinetic term and no independent propagating degree of freedom.

##### BRST charge

↑ **Parent:** [BRST symmetry](#brst-symmetry)

The [BRST charge](#brst-charge) generates [BRST transformations](#brst-symmetry). It has odd [Grassmann parity](linear-algebra.md#grassmann-parity) and is nilpotent, $Q^2=0$.

###### A Hermitian nilpotent BRST charge requires an indefinite auxiliary space

↑ **Parent:** [BRST charge](#brst-charge)

On a positive-definite Hilbert space, these two identities imply $\|Q\psi\|^2=\langle\psi,Q^2\psi\rangle=0$, hence $Q=0$ on its invariant domain. A nontrivial covariant [BRST charge](#brst-charge) therefore acts before reduction on an indefinite-inner-product gauge/ghost space. Exact vectors are null and orthogonal to closed vectors, and [BRST cohomology](#brst-cohomology) quotients them out. Positivity of the reduced physical space requires the additional gauge-theory structure; it does not follow from abstract nilpotence alone.

<h6 id="particle-brst-charge-and-klein-gordon-constraint">Particle BRST charge and Klein–Gordon constraint</h6>

↑ **Parent:** [BRST charge](#brst-charge)

The [FP ghost](#faddeev-popov-ghost) square vanishes, so this [BRST charge](#brst-charge) is nilpotent. On a ghost-number-zero wavefunction, [BRST cohomology](#brst-cohomology) implements the [Klein-Gordon equation](wave-equation.md#klein-gordon-equation). Closure of an unrestricted ghost-extended wavefunction does not independently constrain every component: a pure [FP ghost](#faddeev-popov-ghost) component can lie in the kernel without satisfying the same scalar equation. The [FP ghost](#faddeev-popov-ghost) sector is part of the physical prescription.

###### BRST current in derivative-b gauge fixing

↑ **Parent:** [BRST charge](#brst-charge)

Use gauge-fixing term $(\partial^\mu b)\cdot A_\mu$, ghost term $-(\partial^\mu\bar c)\cdot D_\mu c$, and the [left-acting BRST differential](#left-acting-brst-differential) with $s\bar c=b$. Localizing the odd parameter on the left yields $\delta S=-\int(\partial_\mu\epsilon)j_B^\mu$. Moving it through the antighost derivative determines the last sign. Changing the overall Noether convention reverses this current; rewriting gauge fixing by integration by parts changes its improvement term. Every summand has [ghost number](#ghost-number) one.

###### Yang-Mills BRST Noether current

↑ **Parent:** [BRST charge](#brst-charge)

For the left-parameter convention and ghost kinetic term $(\partial b)Dc$, localization of the [BRST symmetry](#brst-symmetry) yields this conserved [Noether current](quantum-field-theory.md#noether-current). Subtract the total-derivative contribution $K^\mu=h^a(D^\mu c)^a$ in the Lagrangian variation. The [BRST charge](#brst-charge) is the spatial integral of $j^0$. The antighost term has the displayed sign because the parameter and [antighost field](#faddeev-popov-antighost-field) derivative anticommute.

###### BRST Ward identity

↑ **Parent:** [BRST charge](#brst-charge)

For a BRST-invariant action and functional measure, the expectation of a BRST-exact insertion vanishes: $\langle QX\rangle=0$, subject to anomaly and boundary qualifications.

###### Gauge-fixing parameter independence from BRST symmetry

↑ **Parent:** [BRST Ward identity](#brst-ward-identity)

For auxiliary-field covariant gauge fixing, varying the parameter inserts a [BRST-exact operator](#brst-exact-operator). Its correlations with separated physical [BRST-closed](#brst-closed-operator) operators vanish by the [BRST Ward identity](#brst-ward-identity). Normalized physical correlators are therefore independent of the parameter under the invariant-measure and boundary assumptions.

###### Gauge-condition independence of BRST-closed correlation functions

↑ **Parent:** [Gauge-fixing parameter independence from BRST symmetry](#gauge-fixing-parameter-independence-from-brst-symmetry)

For an admissible family of [gauge-fixing fermions](#gauge-fixing-fermion), variation inserts a [BRST-exact operator](#brst-exact-operator) into normalized correlations. If the measured operators are [BRST-closed](#brst-closed-operator), the [graded BRST Ward identity](#graded-brst-ward-identity) makes that insertion vanish. This extends gauge-parameter independence to changes of the gauge functional itself, provided the action and measure preserve [BRST symmetry](#brst-symmetry) and the change produces no boundary contribution. It is the perturbative statement; global gauge-orbit problems require additional analysis.

###### Graded BRST Ward identity

↑ **Parent:** [BRST Ward identity](#brst-ward-identity)

An invariant path-integral measure and [BRST symmetry](#brst-symmetry) action imply this identity when every separated insertion $G_i$ is [BRST-closed](#brst-closed-operator). The bracket is the [graded commutator](commutative-algebra.md#graded-commutator), so it becomes an anticommutator for an odd $\mathcal O$. The arbitrary operator need not itself be closed. Exact insertions therefore decouple from physical correlators.

##### Gauge-fixing fermion

↑ **Parent:** [BRST symmetry](#brst-symmetry)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gauge-fixing_fermion)

A gauge-fixing fermion is a Grassmann-odd functional whose [BRST transformation](#brst-symmetry) $s\Psi$ supplies the gauge-fixing and ghost terms. Nilpotence gives $s(s\Psi)=0$ immediately.

###### BRST-exact covariant gauge fixing

↑ **Parent:** [Gauge-fixing fermion](#gauge-fixing-fermion)

For a left [left-acting BRST differential](#left-acting-brst-differential) with $sA=Dc$, $s\bar c=b$, $sb=0$, choose $\Psi=\bar c^a(\partial\cdot A^a+\xi b^a/2)$. The [graded Leibniz rule](commutative-algebra.md#graded-leibniz-rule) gives $s\Psi=b\partial\cdot A+\xi b^2/2-\bar c\partial\cdot Dc$. Integrating the auxiliary Gaussian yields $-(\partial\cdot A)^2/(2\xi)-\bar c\partial\cdot Dc$. At $\xi=1$ this is [Feynman gauge](#feynman-gauge). Opposite antighost or exact-action sign conventions require a corresponding change of fermion.

// Target: relativistic-quantum-field.bigb

###### Covariant gauge-fixing density as a BRST variation

↑ **Parent:** [Gauge-fixing fermion](#gauge-fixing-fermion)

For the left [graded Leibniz rule](commutative-algebra.md#graded-leibniz-rule) and $s\bar c=-b$, $sb=0$, the displayed [gauge-fixing fermion](#gauge-fixing-fermion) gives $b\,\partial\cdot A+\xi b^2/2+\bar c\,\partial\cdot Dc$. The ghost signs follow from odd parity. [BRST nilpotence](#brst-nilpotence) implies invariance of this density without using field equations. Eliminating the [Nakanishi-Lautrup field](#nakanishi-lautrup-field) gives $-(\partial\cdot A)^2/(2\xi)$ for nonzero $\xi$.

###### Derivative-antighost gauge-fixing fermion

↑ **Parent:** [Gauge-fixing fermion](#gauge-fixing-fermion)

For the convention $s\bar c=-b$, the [action](classical-mechanics.md#action) $S_{\mathrm{YM}}-s\Psi$ contains $-b\,\partial\cdot A+\xi b^2/2-\bar c\,\partial\cdot Dc$ after [integration by parts](calculus.md#integration-by-parts). Integrating the [Nakanishi-Lautrup field](#nakanishi-lautrup-field) gives $-(\partial\cdot A)^2/(2\xi)$. The [Grassmann Gaussian integral](quantum-field-theory.md#grassmann-gaussian-integral) represents the [Faddeev-Popov determinant](#faddeev-popov-determinant).

##### BRST cohomology

↑ **Parent:** [BRST symmetry](#brst-symmetry)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/BRST_cohomology)

BRST cohomology identifies physical states and observables with BRST-closed objects modulo BRST-exact ones. A change of gauge-fixing fermion changes the action by a BRST-exact term and therefore leaves BRST-cohomology classes unchanged when the measure has no BRST anomaly.

###### Positive one-particle BRST cohomology

↑ **Parent:** [BRST cohomology](#brst-cohomology)

For a nonzero null momentum and a nontrivial [BRST charge](#brst-charge) on the gauge/ghost one-particle sector, closed vector states obey $k\cdot\varepsilon=0$ and exact vector states have polarization proportional to $k$. The [Faddeev-Popov ghost field](#faddeev-popov-ghost) state is exact and the [antighost field](#faddeev-popov-antighost-field) state is not closed. With mostly-plus [Minkowski metric](special-relativity.md#minkowski-metric), choose $k=(\omega,0,0,\omega)$; closure sets $\varepsilon^3=\varepsilon^0$, so the norm is $|\varepsilon^1|^2+|\varepsilon^2|^2$. Quotienting by the null longitudinal polarization leaves two positive-norm transverse polarizations per group index. Self-adjointness and nilpotence alone do not establish positivity on an arbitrary state space: the nonzero momentum, nontrivial charge and stated indefinite inner products are essential here.

###### BRST-closed operator

↑ **Parent:** [BRST cohomology](#brst-cohomology)

A BRST-closed operator $O$ satisfies $QO=0$. It represents a physical observable when it is not also BRST exact.

###### BRST-exact operator

↑ **Parent:** [BRST cohomology](#brst-cohomology)

A BRST-exact operator has the form $O=QX$. It is BRST closed by nilpotence and represents the zero class in BRST cohomology.

###### BRST-exact insertions in physical correlation functions

↑ **Parent:** [BRST-exact operator](#brst-exact-operator)

When separated operators $G_i$ are [BRST-closed](#brst-closed-operator), the [graded BRST Ward identity](#graded-brst-ward-identity) makes an exact insertion vanish. This is the correlator form of identifying closed representatives that differ by exact terms in [BRST cohomology](#brst-cohomology). The statement presupposes an invariant measure and suitable boundary conditions.

## ↑ Ancestors (4)

1. [Quantum field theory](quantum-field-theory.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (4)

- [Intrinsic charge-conjugation phase](quantum-field-theory.md#intrinsic-charge-conjugation-phase)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-305.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-305.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-305.md#1/e/solution)
