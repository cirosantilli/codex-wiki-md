# Quantum theory

↑ **Parent:** [Branches of physics](physics.md#branches-of-physics)

**Table of contents**

- [Hadamard transform](#hadamard-transform)
  - [Hadamard gate](#hadamard-gate)
    - [Photon-number reference for a Hadamard gate](#photon-number-reference-for-a-hadamard-gate)
    - [Uniform quantum superposition](#uniform-quantum-superposition)
  - [Walsh-Hadamard transform](#walsh-hadamard-transform)
  - [Hadamard basis](#hadamard-basis)
- [Minimal coupling](#minimal-coupling)
  - [Magnetic minimal coupling](#magnetic-minimal-coupling)
- [Quantum fluctuation](#quantum-fluctuation)
- [Gauge covariance of the Schrödinger equation](#gauge-covariance-of-the-schrodinger-equation)
- [Measurement in quantum mechanics](quantum-measurement.md)
  - [Elitzur-Vaidman bomb tester](quantum-measurement.md#elitzur-vaidman-bomb-tester)
    - [Repeated weak-rotation bomb-test efficiency](quantum-measurement.md#repeated-weak-rotation-bomb-test-efficiency)
  - [Measurement backaction](quantum-measurement.md#measurement-backaction)
  - [Perfect discrimination of pure states requires orthogonality](quantum-measurement.md#perfect-discrimination-of-pure-states-requires-orthogonality)
  - [Quantum nondemolition measurement](quantum-measurement.md#quantum-nondemolition-measurement)
    - [Entanglement-assisted statistical singlet verification](quantum-measurement.md#entanglement-assisted-statistical-singlet-verification)
    - [Bell-pair cost of exact nondemolition singlet verification](quantum-measurement.md#bell-pair-cost-of-exact-nondemolition-singlet-verification)
    - [Entanglement-assisted nondemolition parity measurement](quantum-measurement.md#entanglement-assisted-nondemolition-parity-measurement)
  - [Antidistinguishable quantum states](quantum-measurement.md#antidistinguishable-quantum-states)
  - [Postselection](quantum-measurement.md#postselection)
    - [Aharonov-Bergmann-Lebowitz rule](quantum-measurement.md#aharonov-bergmann-lebowitz-rule)
      - [Context dependence of pre- and post-selected measurements](quantum-measurement.md#context-dependence-of-pre-and-post-selected-measurements)
        - [N-box pre- and post-selection paradox](quantum-measurement.md#n-box-pre-and-post-selection-paradox)
  - [Measurement interaction](quantum-measurement.md#measurement-interaction)
  - [Generalized measurement postulate](quantum-measurement.md#generalized-measurement-postulate)
    - [Nonselective quantum measurement](quantum-measurement.md#nonselective-quantum-measurement)
    - [Selective quantum measurement](quantum-measurement.md#selective-quantum-measurement)
    - [Positive operator-valued measure](quantum-measurement.md#positive-operator-valued-measure)
      - [POVM–ensemble duality for the maximally mixed state](quantum-measurement.md#povm-ensemble-duality-for-the-maximally-mixed-state)
      - [Pure positive operator-valued measure](quantum-measurement.md#pure-positive-operator-valued-measure)
      - [Trine qubit POVM](quantum-measurement.md#trine-qubit-povm)
      - [Informationally complete POVM](quantum-measurement.md#informationally-complete-povm)
        - [Tetrahedral qubit POVM](quantum-measurement.md#tetrahedral-qubit-povm)
      - [Binary rank-one qubit POVM](quantum-measurement.md#binary-rank-one-qubit-povm)
  - [Projective measurement](quantum-measurement.md#projective-measurement)
    - [Completeness forces orthogonality of measurement projections](quantum-measurement.md#completeness-forces-orthogonality-of-measurement-projections)
    - [Equatorial qubit measurement](quantum-measurement.md#equatorial-qubit-measurement)
      - [Equatorial measurement relabeling at Clifford angles](quantum-measurement.md#equatorial-measurement-relabeling-at-clifford-angles)
    - [Lüders rule](quantum-measurement.md#luders-rule)
      - [Post-measurement state](quantum-measurement.md#post-measurement-state)
      - [Nonselective projective measurement](quantum-measurement.md#nonselective-projective-measurement)
        - [Pinching map](quantum-measurement.md#pinching-map)
        - [Rank-one dephasing](quantum-measurement.md#rank-one-dephasing)
          - [Relative-entropy identity for rank-one dephasing](quantum-measurement.md#relative-entropy-identity-for-rank-one-dephasing)
          - [Support inclusion under rank-one dephasing](quantum-measurement.md#support-inclusion-under-rank-one-dephasing)
  - [Quantum state tomography](quantum-measurement.md#quantum-state-tomography)
    - [Interferometric polarization tomography](quantum-measurement.md#interferometric-polarization-tomography)
    - [Single-qubit process tomography](quantum-measurement.md#single-qubit-process-tomography)
  - [No information without disturbance](quantum-measurement.md#no-information-without-disturbance)
    - [Quantum instrument](quantum-measurement.md#quantum-instrument)
      - [Unitary dilation of a measurement instrument](quantum-measurement.md#unitary-dilation-of-a-measurement-instrument)
      - [POVM does not determine the post-measurement state](quantum-measurement.md#povm-does-not-determine-the-post-measurement-state)
      - [Local quantum operation](quantum-measurement.md#local-quantum-operation)
- [Amplitude amplification](#amplitude-amplification)
  - [Nearest-integer stopping for amplitude amplification](#nearest-integer-stopping-for-amplitude-amplification)
  - [Two-dimensional matrix for phase amplitude amplification](#two-dimensional-matrix-for-phase-amplitude-amplification)
  - [Exact amplitude amplification](#exact-amplitude-amplification)
    - [Known-state success dilution for exact amplitude amplification](#known-state-success-dilution-for-exact-amplitude-amplification)
    - [Phase-matched amplitude amplification](#phase-matched-amplitude-amplification)
  - [Geometric amplitude-amplification schedule](#geometric-amplitude-amplification-schedule)
- [Reflection operator](#reflection-operator)
  - [Projector phase rotation](#projector-phase-rotation)
  - [Selective phase rotation](#selective-phase-rotation)
- [HHL algorithm](#hhl-algorithm)
  - [HHL controlled reciprocal rotation](#hhl-controlled-reciprocal-rotation)
  - [Cost of exact phase estimation on a dyadic spectrum](#cost-of-exact-phase-estimation-on-a-dyadic-spectrum)
- [Density matrix](#density-matrix)
  - [Quantum state population](#quantum-state-population)
  - [Quantum coherence in a specified basis](#quantum-coherence-in-a-specified-basis)
  - [Two-qubit Werner state](#two-qubit-werner-state)
    - [Single-copy Werner filtering normalization bound](#single-copy-werner-filtering-normalization-bound)
      - [Single-copy Werner filtering cannot increase concurrence](#single-copy-werner-filtering-cannot-increase-concurrence)
    - [Concurrence of a two-qubit Werner state](#concurrence-of-a-two-qubit-werner-state)
    - [Bell twirling followed by triplet symmetrization](#bell-twirling-followed-by-triplet-symmetrization)
  - [Extreme points of the density-operator state space](#extreme-points-of-the-density-operator-state-space)
  - [Unitary orbit of a density operator](#unitary-orbit-of-a-density-operator)
  - [Quantum state ensemble](#quantum-state-ensemble)
    - [Convex roof extension](#convex-roof-extension)
      - [Monotonicity of a convex roof under a quantum instrument](#monotonicity-of-a-convex-roof-under-a-quantum-instrument)
  - [Pauli correlation tensor](#pauli-correlation-tensor)
  - [Maximally mixed state](#maximally-mixed-state)
    - [Obstruction to uniform probability lowering by a unitary](#obstruction-to-uniform-probability-lowering-by-a-unitary)
  - [Mixed state](#mixed-state)
  - [Von Neumann equation](#von-neumann-equation)
  - [Purification of a density operator](#purification-of-a-density-operator)
    - [Purity decouples a subsystem from its purification](#purity-decouples-a-subsystem-from-its-purification)
    - [Flagged purification of a quantum ensemble](#flagged-purification-of-a-quantum-ensemble)
    - [Unitary freedom of purification](#unitary-freedom-of-purification)
    - [Hughston–Jozsa–Wootters theorem](#hughston-jozsa-wootters-theorem)
      - [Isometry parametrization of a density-matrix ensemble](#isometry-parametrization-of-a-density-matrix-ensemble)
    - [Uhlmann's theorem](#uhlmann-s-theorem)
  - [Trace distance](#trace-distance)
    - [Trace-distance contraction under quantum channels](#trace-distance-contraction-under-quantum-channels)
    - [Trace distance for qubit dephasing](#trace-distance-for-qubit-dephasing)
    - [Pure-target upper bound on trace distance](#pure-target-upper-bound-on-trace-distance)
    - [Spectral-parts formula for trace distance](#spectral-parts-formula-for-trace-distance)
    - [Pure-target lower bound on trace distance](#pure-target-lower-bound-on-trace-distance)
    - [Variational characterization of trace distance](#variational-characterization-of-trace-distance)
      - [Trace-distance-preserving binary measurement](#trace-distance-preserving-binary-measurement)
  - [Von Neumann entropy](von-neumann-entropy.md)
    - [Entropy continuity from Jordan decomposition](von-neumann-entropy.md#entropy-continuity-from-jordan-decomposition)
    - [Entropy of an orthogonal quantum mixture](von-neumann-entropy.md#entropy-of-an-orthogonal-quantum-mixture)
    - [Entropy of a binary diagonal qubit mixture](von-neumann-entropy.md#entropy-of-a-binary-diagonal-qubit-mixture)
    - [Entropy bound from overlap with a pure state](von-neumann-entropy.md#entropy-bound-from-overlap-with-a-pure-state)
    - [Maximum entropy of a quantum state](von-neumann-entropy.md#maximum-entropy-of-a-quantum-state)
    - [Entropy increase under nonselective projective measurement](von-neumann-entropy.md#entropy-increase-under-nonselective-projective-measurement)
      - [Relative entropy of a pinched state](von-neumann-entropy.md#relative-entropy-of-a-pinched-state)
    - [Entanglement entropy](von-neumann-entropy.md#entanglement-entropy)
      - [Average monotonicity of pure-state entanglement entropy](von-neumann-entropy.md#average-monotonicity-of-pure-state-entanglement-entropy)
      - [Schmidt decomposition](von-neumann-entropy.md#schmidt-decomposition)
        - [Operator Schmidt rank](von-neumann-entropy.md#operator-schmidt-rank)
          - [Local Kraus rank bound from an entangled resource](von-neumann-entropy.md#local-kraus-rank-bound-from-an-entangled-resource)
        - [Schmidt-basis Pauli correlation tensor](von-neumann-entropy.md#schmidt-basis-pauli-correlation-tensor)
        - [Schmidt coefficient](von-neumann-entropy.md#schmidt-coefficient)
        - [Schmidt rank](von-neumann-entropy.md#schmidt-rank)
          - [Schmidt-rank contraction under product operators](von-neumann-entropy.md#schmidt-rank-contraction-under-product-operators)
          - [Monotonicity of Schmidt rank under LOCC](von-neumann-entropy.md#monotonicity-of-schmidt-rank-under-locc)
          - [Maximally entangled overlap bound from Schmidt rank](von-neumann-entropy.md#maximally-entangled-overlap-bound-from-schmidt-rank)
      - [Schmidt number](von-neumann-entropy.md#schmidt-number)
    - [Subadditivity of Von Neumann entropy](von-neumann-entropy.md#subadditivity-of-von-neumann-entropy)
      - [Araki–Lieb inequality](von-neumann-entropy.md#araki-lieb-inequality)
      - [Strong subadditivity of quantum entropy](von-neumann-entropy.md#strong-subadditivity-of-quantum-entropy)
        - [Strong subadditivity from relative-entropy monotonicity](von-neumann-entropy.md#strong-subadditivity-from-relative-entropy-monotonicity)
        - [Weak monotonicity of quantum entropy](von-neumann-entropy.md#weak-monotonicity-of-quantum-entropy)
    - [Concavity of Von Neumann entropy](von-neumann-entropy.md#concavity-of-von-neumann-entropy)
      - [Strict concavity of Von Neumann entropy](von-neumann-entropy.md#strict-concavity-of-von-neumann-entropy)
      - [Entropy bounds for a quantum mixture](von-neumann-entropy.md#entropy-bounds-for-a-quantum-mixture)
      - [Entropy bound for a binary mixture](von-neumann-entropy.md#entropy-bound-for-a-binary-mixture)
    - [Quantum conditional entropy](von-neumann-entropy.md#quantum-conditional-entropy)
      - [Pure-state negative conditional entropy criterion](von-neumann-entropy.md#pure-state-negative-conditional-entropy-criterion)
      - [Concavity of quantum conditional entropy](von-neumann-entropy.md#concavity-of-quantum-conditional-entropy)
      - [Continuity bound for quantum conditional entropy](von-neumann-entropy.md#continuity-bound-for-quantum-conditional-entropy)
      - [Dimension bound for quantum conditional entropy](von-neumann-entropy.md#dimension-bound-for-quantum-conditional-entropy)
    - [Quantum relative entropy](von-neumann-entropy.md#quantum-relative-entropy)
      - [Relative entropy of classically flagged states](von-neumann-entropy.md#relative-entropy-of-classically-flagged-states)
      - [Nonnegativity of quantum relative entropy](von-neumann-entropy.md#nonnegativity-of-quantum-relative-entropy)
        - [Eigenbasis proof of quantum relative entropy nonnegativity](von-neumann-entropy.md#eigenbasis-proof-of-quantum-relative-entropy-nonnegativity)
      - [Quantum Pinsker inequality](von-neumann-entropy.md#quantum-pinsker-inequality)
      - [Donald's identity](von-neumann-entropy.md#donald-s-identity)
        - [Relative-entropy barycenter of a quantum ensemble](von-neumann-entropy.md#relative-entropy-barycenter-of-a-quantum-ensemble)
      - [Data-processing inequality for quantum relative entropy](von-neumann-entropy.md#data-processing-inequality-for-quantum-relative-entropy)
      - [Additivity of quantum relative entropy](von-neumann-entropy.md#additivity-of-quantum-relative-entropy)
      - [Superadditivity of quantum relative entropy](von-neumann-entropy.md#superadditivity-of-quantum-relative-entropy)
        - [Multipartite superadditivity of quantum relative entropy](von-neumann-entropy.md#multipartite-superadditivity-of-quantum-relative-entropy)
          - [Lower asymptotic semicontinuity of quantum relative entropy](von-neumann-entropy.md#lower-asymptotic-semicontinuity-of-quantum-relative-entropy)
      - [Quantum mutual information](von-neumann-entropy.md#quantum-mutual-information)
        - [Quantum conditional mutual information](von-neumann-entropy.md#quantum-conditional-mutual-information)
        - [Data processing for quantum mutual information](von-neumann-entropy.md#data-processing-for-quantum-mutual-information)
          - [Postselection can increase conditional quantum mutual information](von-neumann-entropy.md#postselection-can-increase-conditional-quantum-mutual-information)
          - [Mutual-information loss as conditional mutual information](von-neumann-entropy.md#mutual-information-loss-as-conditional-mutual-information)
        - [Quantum mutual information balance identity](von-neumann-entropy.md#quantum-mutual-information-balance-identity)
      - [Variational characterization of quantum conditional entropy](von-neumann-entropy.md#variational-characterization-of-quantum-conditional-entropy)
  - [Purity of a density operator](#purity-of-a-density-operator)
  - [Reduced density operator of a weakly coupled oscillator pair](#reduced-density-operator-of-a-weakly-coupled-oscillator-pair)
  - [Bloch vector](#bloch-vector)
    - [Bloch ball](#bloch-ball)
      - [Antipodal eigenprojectors of a qubit density matrix](#antipodal-eigenprojectors-of-a-qubit-density-matrix)
    - [Generalized Bloch representation](#generalized-bloch-representation)
      - [Hamiltonian rotations of Bloch vectors](#hamiltonian-rotations-of-bloch-vectors)
      - [Purity bound for generalized Bloch vectors](#purity-bound-for-generalized-bloch-vectors)
      - [Affine Bloch equation](#affine-bloch-equation)
        - [Transverse relaxation](#transverse-relaxation)
        - [Population relaxation](#population-relaxation)
        - [Steady states of an affine Bloch equation](#steady-states-of-an-affine-bloch-equation)
    - [Bloch sphere](#bloch-sphere)
      - [Pure-qubit overlap identity](#pure-qubit-overlap-identity)
      - [Uniform pure-qubit average](#uniform-pure-qubit-average)
    - [Informationally complete three-observable qubit tomography](#informationally-complete-three-observable-qubit-tomography)
- [Quantum no-signalling](#quantum-no-signalling)
  - [Remote preparation in conjugate bases](#remote-preparation-in-conjugate-bases)
    - [Perfect two-basis discrimination would allow superluminal signalling](#perfect-two-basis-discrimination-would-allow-superluminal-signalling)
      - [Exact pure-state overlap readout would allow superluminal signalling](#exact-pure-state-overlap-readout-would-allow-superluminal-signalling)
  - [Relativistic causality constraint on an ideal nonlocal measurement](#relativistic-causality-constraint-on-an-ideal-nonlocal-measurement)
    - [Controlled-basis measurement causality obstruction](#controlled-basis-measurement-causality-obstruction)
    - [Singlet-triplet measurement causality obstruction](#singlet-triplet-measurement-causality-obstruction)
- [Quantum cloning](#quantum-cloning)
  - [Cloning failure bound from trace-distance contraction](#cloning-failure-bound-from-trace-distance-contraction)
  - [Copy-number trace-distance obstruction](#copy-number-trace-distance-obstruction)
  - [No-cloning theorem](#no-cloning-theorem)
  - [No-cloning theorem for two pure states](#no-cloning-theorem-for-two-pure-states)
  - [Clone-assisted asymptotic state discrimination](#clone-assisted-asymptotic-state-discrimination)
  - [Perfect discrimination implies cloning for a known state family](#perfect-discrimination-implies-cloning-for-a-known-state-family)
- [Environment-assisted two-state pure-state transformation](#environment-assisted-two-state-pure-state-transformation)
- [Helstrom-Holevo bound](#helstrom-holevo-bound)
  - [Helstrom measurement for two pure states](#helstrom-measurement-for-two-pure-states)
    - [Helstrom measurement for the zero and plus states](#helstrom-measurement-for-the-zero-and-plus-states)
  - [Perfect distinguishability of pure states](#perfect-distinguishability-of-pure-states)
  - [Unambiguous quantum state discrimination](#unambiguous-quantum-state-discrimination)
    - [Reciprocal-state construction of unambiguous discrimination](#reciprocal-state-construction-of-unambiguous-discrimination)
- [Unitary gate discrimination](#unitary-gate-discrimination)
  - [Single-use perfect discrimination of two unitary gates](#single-use-perfect-discrimination-of-two-unitary-gates)
  - [Numerical range](#numerical-range)
    - [Numerical range of a normal matrix](#numerical-range-of-a-normal-matrix)
  - [Unit-circle spectrum of a unitary operator](#unit-circle-spectrum-of-a-unitary-operator)
  - [Spectral arc length of a unitary operator](#spectral-arc-length-of-a-unitary-operator)
    - [Spectral arc length of a phase gate](#spectral-arc-length-of-a-phase-gate)
    - [Origin in the convex hull of unit-circle points](#origin-in-the-convex-hull-of-unit-circle-points)
      - [Spectral-arc criterion for perfect unitary discrimination](#spectral-arc-criterion-for-perfect-unitary-discrimination)
- [Robertson uncertainty principle](#robertson-uncertainty-principle)
  - [Heisenberg uncertainty relation](#heisenberg-uncertainty-relation)
  - [Quadratic-norm proof of the Heisenberg uncertainty relation](#quadratic-norm-proof-of-the-heisenberg-uncertainty-relation)
  - [Equality case of the Heisenberg uncertainty relation](#equality-case-of-the-heisenberg-uncertainty-relation)
- [Gaussian eigenstate for a quadratic potential](#gaussian-eigenstate-for-a-quadratic-potential)
- [Coherent state](#coherent-state)
  - [Coherent-state resolution of identity](#coherent-state-resolution-of-identity)
  - [Unnormalized bosonic coherent state](#unnormalized-bosonic-coherent-state)
  - [Fermionic coherent state](#fermionic-coherent-state)
    - [Fermionic coherent-state trace](#fermionic-coherent-state-trace)
- [Born approximation](#born-approximation)
- [Toffoli gate](#toffoli-gate)
- [Modular-addition quantum oracle](#modular-addition-quantum-oracle)
  - [Modular-oracle inversion by negation](#modular-oracle-inversion-by-negation)
- [Boolean quantum oracle](#boolean-quantum-oracle)
  - [Phase kickback](#phase-kickback)
    - [Quadratic Boolean phase cancellation](#quadratic-boolean-phase-cancellation)
    - [Bernstein-Vazirani phase kickback](#bernstein-vazirani-phase-kickback)
      - [Qutrit linear-function identification](#qutrit-linear-function-identification)
      - [Bernstein-Vazirani decoding controlled by a quantum register](#bernstein-vazirani-decoding-controlled-by-a-quantum-register)
    - [Marked-state phase oracle](#marked-state-phase-oracle)
      - [Marked-state phase oracle from a single faulty identity-oracle query](#marked-state-phase-oracle-from-a-single-faulty-identity-oracle-query)
  - [Compute-phase-uncompute construction](#compute-phase-uncompute-construction)
  - [Uncomputation](#uncomputation)
- [Quantum circuit](quantum-circuit.md)
  - [Quantum circuit gate-error telescoping bound](quantum-circuit.md#quantum-circuit-gate-error-telescoping-bound)
  - [Depth-first quantum circuit path summation](quantum-circuit.md#depth-first-quantum-circuit-path-summation)
  - [Stoquastic circuit](quantum-circuit.md#stoquastic-circuit)
    - [Stoquastic acceptance floor](quantum-circuit.md#stoquastic-acceptance-floor)
  - [Computational history state](quantum-circuit.md#computational-history-state)
    - [Feynman-Kitaev Hamiltonian](quantum-circuit.md#feynman-kitaev-hamiltonian)
      - [Gap above a degenerate history ground space](quantum-circuit.md#gap-above-a-degenerate-history-ground-space)
      - [Input penalty of a history Hamiltonian](quantum-circuit.md#input-penalty-of-a-history-hamiltonian)
    - [Nonlocal quantum clock](quantum-circuit.md#nonlocal-quantum-clock)
    - [Unary quantum clock](quantum-circuit.md#unary-quantum-clock)
      - [History-subspace propagation Hamiltonian](quantum-circuit.md#history-subspace-propagation-hamiltonian)
        - [Gershgorin gap bound for an adiabatic history path](quantum-circuit.md#gershgorin-gap-bound-for-an-adiabatic-history-path)
        - [Spectrum of a path propagation Hamiltonian](quantum-circuit.md#spectrum-of-a-path-propagation-hamiltonian)
  - [Quantum logic gate](quantum-circuit.md#quantum-logic-gate)
    - [Two-qubit gate](quantum-circuit.md#two-qubit-gate)
      - [Diagonal two-qubit phase entanglement criterion](quantum-circuit.md#diagonal-two-qubit-phase-entanglement-criterion)
      - [Cartan decomposition of a two-qubit gate](quantum-circuit.md#cartan-decomposition-of-a-two-qubit-gate)
  - [Measurement-based quantum computation](quantum-circuit.md#measurement-based-quantum-computation)
    - [Three-vertex graph-state wire](quantum-circuit.md#three-vertex-graph-state-wire)
    - [Five-vertex graph-state circuit simulation](quantum-circuit.md#five-vertex-graph-state-circuit-simulation)
    - [Four-cycle graph-state simulation of an entangle-and-measure circuit](quantum-circuit.md#four-cycle-graph-state-simulation-of-an-entangle-and-measure-circuit)
    - [Measurement pattern](quantum-circuit.md#measurement-pattern)
      - [Logical depth of a measurement pattern](quantum-circuit.md#logical-depth-of-a-measurement-pattern)
        - [Two-layer measurement pattern for CNOT and x-axis rotations](quantum-circuit.md#two-layer-measurement-pattern-for-cnot-and-x-axis-rotations)
        - [Nonadaptive Clifford measurement pattern](quantum-circuit.md#nonadaptive-clifford-measurement-pattern)
          - [Nonadaptive Hadamard–CNOT measurement pattern](quantum-circuit.md#nonadaptive-hadamard-cnot-measurement-pattern)
  - [Quantum register](quantum-circuit.md#quantum-register)
  - [Rotation gate](quantum-circuit.md#rotation-gate)
    - [Rotation about the x-axis](quantum-circuit.md#rotation-about-the-x-axis)
    - [Rotation about the y-axis](quantum-circuit.md#rotation-about-the-y-axis)
    - [Rotation about the z-axis](quantum-circuit.md#rotation-about-the-z-axis)
  - [Universal quantum gate set](quantum-circuit.md#universal-quantum-gate-set)
    - [Solovay--Kitaev theorem](quantum-circuit.md#solovay-kitaev-theorem)
  - [Quantum state preparation](quantum-circuit.md#quantum-state-preparation)
    - [Uniform coprime state for a semiprime](quantum-circuit.md#uniform-coprime-state-for-a-semiprime)
    - [Uniform superposition state](quantum-circuit.md#uniform-superposition-state)
    - [Hierarchical probability-distribution state preparation](quantum-circuit.md#hierarchical-probability-distribution-state-preparation)
  - [Quantum arithmetic](quantum-circuit.md#quantum-arithmetic)
  - [Pauli group](quantum-circuit.md#pauli-group)
    - [Pauli-string commutation parity](quantum-circuit.md#pauli-string-commutation-parity)
    - [Binary phase representation of a Pauli string](quantum-circuit.md#binary-phase-representation-of-a-pauli-string)
      - [Binary symplectic space of Pauli labels](quantum-circuit.md#binary-symplectic-space-of-pauli-labels)
        - [Isotropic subspace of a binary symplectic space](quantum-circuit.md#isotropic-subspace-of-a-binary-symplectic-space)
      - [Controlled-Z update in the binary phase representation](quantum-circuit.md#controlled-z-update-in-the-binary-phase-representation)
    - [Pauli frame](quantum-circuit.md#pauli-frame)
    - [Pauli operator](quantum-circuit.md#pauli-operator)
      - [Pauli decomposition of a qubit-environment isometry](quantum-circuit.md#pauli-decomposition-of-a-qubit-environment-isometry)
      - [Weight of a Pauli operator](quantum-circuit.md#weight-of-a-pauli-operator)
      - [Pauli expansion of a quantum error](quantum-circuit.md#pauli-expansion-of-a-quantum-error)
      - [Pauli gate](quantum-circuit.md#pauli-gate)
      - [Pauli correlator](quantum-circuit.md#pauli-correlator)
    - [Stabilizer group](quantum-circuit.md#stabilizer-group)
      - [Balanced spectrum of a nonidentity stabilizer](quantum-circuit.md#balanced-spectrum-of-a-nonidentity-stabilizer)
      - [Stabilizer generator](quantum-circuit.md#stabilizer-generator)
      - [Stabilizer state](quantum-circuit.md#stabilizer-state)
        - [Stabilizer-state preparation](quantum-circuit.md#stabilizer-state-preparation)
        - [Stabilizer tableau](quantum-circuit.md#stabilizer-tableau)
        - [Graph state](quantum-circuit.md#graph-state)
          - [Equatorial measurement of a graph-state leaf](quantum-circuit.md#equatorial-measurement-of-a-graph-state-leaf)
          - [Computational-basis measurement of a graph-state vertex](quantum-circuit.md#computational-basis-measurement-of-a-graph-state-vertex)
          - [Graph-state stabilizer generator](quantum-circuit.md#graph-state-stabilizer-generator)
          - [Local complementation of a graph state](quantum-circuit.md#local-complementation-of-a-graph-state)
      - [Stabilizer subspace](quantum-circuit.md#stabilizer-subspace)
        - [Stabilizer-projector formula](quantum-circuit.md#stabilizer-projector-formula)
    - [Clifford gate](quantum-circuit.md#clifford-gate)
      - [Clifford circuit](quantum-circuit.md#clifford-circuit)
        - [Gottesman--Knill theorem](quantum-circuit.md#gottesman-knill-theorem)
          - [Extended Gottesman--Knill theorem](quantum-circuit.md#extended-gottesman-knill-theorem)
        - [Clifford frame](quantum-circuit.md#clifford-frame)
      - [Local Clifford operation](quantum-circuit.md#local-clifford-operation)
      - [Strong classical simulation of a quantum circuit](quantum-circuit.md#strong-classical-simulation-of-a-quantum-circuit)
        - [Heisenberg propagation of a Pauli observable through a Clifford circuit](quantum-circuit.md#heisenberg-propagation-of-a-pauli-observable-through-a-clifford-circuit)
          - [Backward Pauli updates for Hadamard and phase gates](quantum-circuit.md#backward-pauli-updates-for-hadamard-and-phase-gates)
      - [Weak classical simulation of a quantum circuit](quantum-circuit.md#weak-classical-simulation-of-a-quantum-circuit)
- [Lieb-Robinson bound](#lieb-robinson-bound)
  - [Full-evolution comparison for truncated dynamics](#full-evolution-comparison-for-truncated-dynamics)
  - [Lieb-Robinson interaction-chain expansion](#lieb-robinson-interaction-chain-expansion)
  - [Interaction distance](#interaction-distance)
  - [Lieb-Robinson localization by Haar twirling](#lieb-robinson-localization-by-haar-twirling)
  - [Finite-depth local quantum circuit](#finite-depth-local-quantum-circuit)
    - [Backward light cone of a local quantum circuit](#backward-light-cone-of-a-local-quantum-circuit)
    - [GHZ-state circuit-depth lower bound](#ghz-state-circuit-depth-lower-bound)
- [Grover's algorithm](#grover-s-algorithm)
  - [First half-success time in Grover search](#first-half-success-time-in-grover-search)
  - [Continuous-time quantum search](#continuous-time-quantum-search)
  - [Grover search with a nonzero reflection label](#grover-search-with-a-nonzero-reflection-label)
  - [Verified Grover promise test](#verified-grover-promise-test)
  - [Marked density under a permutation](#marked-density-under-a-permutation)
    - [Permutation-preimage quantum search](#permutation-preimage-quantum-search)
  - [Known-subset Grover search](#known-subset-grover-search)
    - [Clean subset superposition preparation](#clean-subset-superposition-preparation)
  - [Grover diffusion operator](#grover-diffusion-operator)
    - [Inversion about the mean](#inversion-about-the-mean)
  - [Grover rotation angle](#grover-rotation-angle)
    - [First half-probability Grover iterate](#first-half-probability-grover-iterate)
    - [First successful Grover iterate](#first-successful-grover-iterate)
    - [Exact Grover search on four entries](#exact-grover-search-on-four-entries)
- [Computational basis](#computational-basis)
  - [Quantum measurement in the computational basis](#quantum-measurement-in-the-computational-basis)
    - [Computational-basis state](#computational-basis-state)
- [Deutsch-Jozsa algorithm](#deutsch-jozsa-algorithm)
  - [Deutsch algorithm](#deutsch-algorithm)
    - [Deutsch algorithm with pure dephasing](#deutsch-algorithm-with-pure-dephasing)
  - [Opposite-pair elimination for exact quantum balance testing](#opposite-pair-elimination-for-exact-quantum-balance-testing)
  - [Deutsch-Jozsa test with an arbitrary uniform-state unitary](#deutsch-jozsa-test-with-an-arbitrary-uniform-state-unitary)
- [Quantum Fourier transform](#quantum-fourier-transform)
  - [Dyadic quantum Fourier transform circuit](#dyadic-quantum-fourier-transform-circuit)
  - [Product decomposition of a Fourier phase state](#product-decomposition-of-a-fourier-phase-state)
  - [Fourier sample](#fourier-sample)
  - [Quantum Fourier transform over a finite abelian group](#quantum-fourier-transform-over-a-finite-abelian-group)
  - [Square of the quantum Fourier transform](#square-of-the-quantum-fourier-transform)
  - [Quantum Fourier transform of a periodic coset state](#quantum-fourier-transform-of-a-periodic-coset-state)
  - [Quantum period finding](#quantum-period-finding)
    - [Exact period recovery from a Fourier sample](#exact-period-recovery-from-a-fourier-sample)
      - [Two-sample exact period recovery](#two-sample-exact-period-recovery)
      - [Heralded exact quantum period finding when the period divides the register size](#heralded-exact-quantum-period-finding-when-the-period-divides-the-register-size)
        - [Quantum Fourier sampling of powers of three modulo ten](#quantum-fourier-sampling-of-powers-of-three-modulo-ten)
  - [Hidden subgroup problem](#hidden-subgroup-problem)
    - [Discrete-logarithm Fourier sampling](#discrete-logarithm-fourier-sampling)
      - [Linear congruence from a discrete-logarithm Fourier sample](#linear-congruence-from-a-discrete-logarithm-fourier-sample)
    - [Coset state](#coset-state)
      - [Periodic coset state](#periodic-coset-state)
    - [Group shift operator](#group-shift-operator)
    - [Abelian hidden-subgroup Fourier sampling](#abelian-hidden-subgroup-fourier-sampling)
    - [Simon's problem](#simon-s-problem)
      - [Classical collision query bound for Simon's problem](#classical-collision-query-bound-for-simon-s-problem)
      - [Simon's algorithm](#simon-s-algorithm)
        - [Expected query count for Simon sampling](#expected-query-count-for-simon-sampling)
        - [Single-sample distribution in Simon's algorithm](#single-sample-distribution-in-simon-s-algorithm)
        - [Orthogonal complement over the binary field](#orthogonal-complement-over-the-binary-field)
    - [Stabilizer as a hidden subgroup](#stabilizer-as-a-hidden-subgroup)
  - [Cyclic shift operator](#cyclic-shift-operator)
    - [Cyclic shift diagonalization by the quantum Fourier transform](#cyclic-shift-diagonalization-by-the-quantum-fourier-transform)
  - [Quantum phase estimation](#quantum-phase-estimation)
    - [Quantum phase estimation tail bound](#quantum-phase-estimation-tail-bound)
    - [Near-grid quantum phase estimation](#near-grid-quantum-phase-estimation)
    - [Parallel phase multiplication by coherent fanout](#parallel-phase-multiplication-by-coherent-fanout)
    - [Quantum phase estimation with a maximally mixed target](#quantum-phase-estimation-with-a-maximally-mixed-target)
    - [Nearest-integer success bound for quantum phase estimation](#nearest-integer-success-bound-for-quantum-phase-estimation)
    - [Dyadic phase-gate identification](#dyadic-phase-gate-identification)
    - [Tensor-product eigenphase amplification](#tensor-product-eigenphase-amplification)
    - [Positive-phase fractional power of a unitary operator](#positive-phase-fractional-power-of-a-unitary-operator)
    - [Quantum spectral filtering](#quantum-spectral-filtering)
      - [Singular obstruction to normalized quantum matrix multiplication](#singular-obstruction-to-normalized-quantum-matrix-multiplication)
      - [Success probability of positive quantum spectral filtering](#success-probability-of-positive-quantum-spectral-filtering)
    - [Exact quantum phase estimation](#exact-quantum-phase-estimation)
- [BB84](#bb84)
  - [Bit error rate](#bit-error-rate)
- [Breidbart basis](#breidbart-basis)
- [Bell state](bell-state.md)
  - [Local flag correction of a Bell-state phase mixture](bell-state.md#local-flag-correction-of-a-bell-state-phase-mixture)
  - [Bell pair](bell-state.md#bell-pair)
  - [Dephased Bell-state mixture](bell-state.md#dephased-bell-state-mixture)
  - [Bell-basis measurement](bell-state.md#bell-basis-measurement)
    - [Bell-state nondemolition measurement](bell-state.md#bell-state-nondemolition-measurement)
  - [Superdense coding](bell-state.md#superdense-coding)
  - [Spin singlet state](bell-state.md#spin-singlet-state)
    - [Collective-unitary covariance of the two-qubit singlet](bell-state.md#collective-unitary-covariance-of-the-two-qubit-singlet)
  - [Reduced density matrix](bell-state.md#reduced-density-matrix)
    - [No-communication theorem](bell-state.md#no-communication-theorem)
      - [Remote state invariance under a local trace-preserving operation](bell-state.md#remote-state-invariance-under-a-local-trace-preserving-operation)
    - [Product state](bell-state.md#product-state)
      - [Two-qubit product-state determinant criterion](bell-state.md#two-qubit-product-state-determinant-criterion)
    - [Entangled state](bell-state.md#entangled-state)
      - [Entanglement distillation](bell-state.md#entanglement-distillation)
      - [Entanglement dilution](bell-state.md#entanglement-dilution)
        - [Exact dilution obstruction from Schmidt rank](bell-state.md#exact-dilution-obstruction-from-schmidt-rank)
        - [Deterministic two-qubit entanglement dilution](bell-state.md#deterministic-two-qubit-entanglement-dilution)
      - [Entanglement monotone](bell-state.md#entanglement-monotone)
        - [Relative entropy of entanglement](bell-state.md#relative-entropy-of-entanglement)
        - [Schmidt-tail entanglement monotone](bell-state.md#schmidt-tail-entanglement-monotone)
      - [Concurrence](bell-state.md#concurrence)
        - [Mixed-state concurrence of two qubits](bell-state.md#mixed-state-concurrence-of-two-qubits)
          - [Concurrence scaling under invertible local filters](bell-state.md#concurrence-scaling-under-invertible-local-filters)
      - [Entanglement criterion for a two-term correlated state](bell-state.md#entanglement-criterion-for-a-two-term-correlated-state)
      - [Entanglement concentration](bell-state.md#entanglement-concentration)
        - [Schmidt projection entanglement concentration](bell-state.md#schmidt-projection-entanglement-concentration)
          - [Tripartite Schmidt projection entanglement concentration](bell-state.md#tripartite-schmidt-projection-entanglement-concentration)
    - [Local indistinguishability of Bell-state phase](bell-state.md#local-indistinguishability-of-bell-state-phase)
  - [Local operations and classical communication](bell-state.md#local-operations-and-classical-communication)
    - [Two-outcome LOCC dilution of a Bell pair](bell-state.md#two-outcome-locc-dilution-of-a-bell-pair)
    - [Deterministic reduction of maximally entangled Schmidt rank](bell-state.md#deterministic-reduction-of-maximally-entangled-schmidt-rank)
    - [Asymptotic pure-state entanglement conversion rate](bell-state.md#asymptotic-pure-state-entanglement-conversion-rate)
      - [Collective advantage over independent two-qubit filtering](bell-state.md#collective-advantage-over-independent-two-qubit-filtering)
    - [Optimal stochastic conversion of a two-qubit pure state](bell-state.md#optimal-stochastic-conversion-of-a-two-qubit-pure-state)
    - [Local unitary operation](bell-state.md#local-unitary-operation)
      - [Local-unitary invariance of reduced-state spectra](bell-state.md#local-unitary-invariance-of-reduced-state-spectra)
    - [Nielsen's pure-state conversion theorem](bell-state.md#nielsen-s-pure-state-conversion-theorem)
    - [LOCC discrimination of two Bell states](bell-state.md#locc-discrimination-of-two-bell-states)
    - [Quantum teleportation](bell-state.md#quantum-teleportation)
      - [Dicke-resource telecloning](bell-state.md#dicke-resource-telecloning)
      - [Exact teleportation resource criterion](bell-state.md#exact-teleportation-resource-criterion)
      - [Entanglement swapping](bell-state.md#entanglement-swapping)
      - [Qudit teleportation](bell-state.md#qudit-teleportation)
      - [Teleportation as an identity channel on a reference](bell-state.md#teleportation-as-an-identity-channel-on-a-reference)
      - [One-bit teleportation](bell-state.md#one-bit-teleportation)
        - [Pauli-frame propagation along a measurement wire](bell-state.md#pauli-frame-propagation-along-a-measurement-wire)
        - [Graph-state preparation of a computational-basis input](bell-state.md#graph-state-preparation-of-a-computational-basis-input)
        - [Heralded Pauli X correction using controlled-Z and measurements](bell-state.md#heralded-pauli-x-correction-using-controlled-z-and-measurements)
        - [J gate in measurement-based quantum computation](bell-state.md#j-gate-in-measurement-based-quantum-computation)
          - [J-gate phase-error operator norm](bell-state.md#j-gate-phase-error-operator-norm)
      - [Bell-basis teleportation identity](bell-state.md#bell-basis-teleportation-identity)
      - [No-programming theorem](bell-state.md#no-programming-theorem)
      - [Teleportation with the psi-plus Bell state](bell-state.md#teleportation-with-the-psi-plus-bell-state)
  - [Quantum dense coding](bell-state.md#quantum-dense-coding)
- [Variational method](#variational-method)
  - [Nodeless theorem for a one-dimensional ground state](#nodeless-theorem-for-a-one-dimensional-ground-state)
  - [Exact ground state of a solvable sextic potential](#exact-ground-state-of-a-solvable-sextic-potential)
  - [Gaussian variational estimate for a solvable sextic potential](#gaussian-variational-estimate-for-a-solvable-sextic-potential)
  - [Ground-state energy monotonicity under potential ordering](#ground-state-energy-monotonicity-under-potential-ordering)
  - [Quantum virial identity from scaling](#quantum-virial-identity-from-scaling)
    - [Fall to the centre for a supercritical inverse-power potential](#fall-to-the-centre-for-a-supercritical-inverse-power-potential)
  - [Exact variational solution in a two-level system](#exact-variational-solution-in-a-two-level-system)
    - [Level repulsion in a two-level Hamiltonian](#level-repulsion-in-a-two-level-hamiltonian)
- [Landau level](#landau-level)
  - [Ground-state filling of two spin-degenerate Landau levels](#ground-state-filling-of-two-spin-degenerate-landau-levels)
  - [Lowest Landau level](#lowest-landau-level)
  - [Cyclotron frequency](#cyclotron-frequency)
  - [Landau gauge for a uniform magnetic field](#landau-gauge-for-a-uniform-magnetic-field)
  - [Degeneracy of a Landau level](#degeneracy-of-a-landau-level)
  - [Spin splitting of Landau levels](#spin-splitting-of-landau-levels)
  - [Landau levels in crossed electric and magnetic fields](#landau-levels-in-crossed-electric-and-magnetic-fields)
    - [Electric-cross-magnetic-field drift](#electric-cross-magnetic-field-drift)
    - [Electric-field splitting of a Landau level in a rectangle](#electric-field-splitting-of-a-landau-level-in-a-rectangle)
  - [Symmetric gauge](#symmetric-gauge)
    - [Kinetic momentum and magnetic pseudomomentum](#kinetic-momentum-and-magnetic-pseudomomentum)
      - [Kinetic momentum](#kinetic-momentum)
      - [Magnetic translation](#magnetic-translation)
        - [Magnetic translation algebra](#magnetic-translation-algebra)
          - [Magnetic flux quantum](#magnetic-flux-quantum)
            - [Fluxoid and flux quantization in a superconductor](#fluxoid-and-flux-quantization-in-a-superconductor)
- [Bloch's theorem](#bloch-s-theorem)
  - [Particle in a one-dimensional lattice](#particle-in-a-one-dimensional-lattice)
    - [Kronig-Penney model](#kronig-penney-model)
      - [Floquet discriminant of the delta-comb Kronig-Penney model](#floquet-discriminant-of-the-delta-comb-kronig-penney-model)
      - [Attractive delta-comb Kronig-Penney model](#attractive-delta-comb-kronig-penney-model)
        - [Negative-energy band of an attractive delta comb](#negative-energy-band-of-an-attractive-delta-comb)
      - [Scattering-amplitude equations for one-dimensional band edges](#scattering-amplitude-equations-for-one-dimensional-band-edges)
  - [Electronic band structure](#electronic-band-structure)
    - [Energy band](#energy-band)
      - [Impurity level in a crystal](#impurity-level-in-a-crystal)
      - [Band effective mass](#band-effective-mass)
      - [Allowed energy band](#allowed-energy-band)
      - [Band gap](#band-gap)
        - [Avoided crossing](#avoided-crossing)
      - [Band filling](#band-filling)
        - [Band insulator](#band-insulator)
          - [Overlapping energy bands prevent a band insulator](#overlapping-energy-bands-prevent-a-band-insulator)
  - [Bloch oscillation](#bloch-oscillation)
  - [Translation-character proof of Bloch theorem](#translation-character-proof-of-bloch-theorem)
  - [Bloch state](#bloch-state)
    - [Crystal momentum](#crystal-momentum)
  - [Periodic potential](#periodic-potential)
  - [Nearly-free electron model](#nearly-free-electron-model)
    - [Nearly-free electron dispersion near a one-dimensional band gap](#nearly-free-electron-dispersion-near-a-one-dimensional-band-gap)
  - [Floquet matrix for a one-dimensional periodic potential](#floquet-matrix-for-a-one-dimensional-periodic-potential)
    - [Floquet discriminant and energy bands](#floquet-discriminant-and-energy-bands)
  - [Tight binding](#tight-binding)
    - [Dilute-hopping lattice propagator](#dilute-hopping-lattice-propagator)
    - [Harmonic approximation near a potential minimum](#harmonic-approximation-near-a-potential-minimum)
    - [Finite periodic tight-binding ring](#finite-periodic-tight-binding-ring)
    - [Two-direction nearest-neighbour tight-binding dispersion](#two-direction-nearest-neighbour-tight-binding-dispersion)
  - [Brillouin zone](#brillouin-zone)
    - [Bragg point](#bragg-point)
    - [Brillouin zone of a two-dimensional triangular lattice](#brillouin-zone-of-a-two-dimensional-triangular-lattice)
- [Pauli Z gate](#pauli-z-gate)
- [Pauli Y gate](#pauli-y-gate)
- [Pauli X gate](#pauli-x-gate)
- [Phase gate](#phase-gate)
  - [Phase-gate discretization error](#phase-gate-discretization-error)
  - [Controlled phase gate](#controlled-phase-gate)
    - [Controlled-Z gate](#controlled-z-gate)
  - [Probabilistic phase-gate injection](#probabilistic-phase-gate-injection)
- [Inverse quantum circuit](#inverse-quantum-circuit)
- [Controlled unitary gate](#controlled-unitary-gate)
  - [Quantum variable rotation](#quantum-variable-rotation)
    - [Binary-angle implementation of a quantum variable rotation](#binary-angle-implementation-of-a-quantum-variable-rotation)
  - [Fredkin gate](#fredkin-gate)
  - [Controlled-NOT gate](#controlled-not-gate)
    - [CNOT control reversal in the Hadamard basis](#cnot-control-reversal-in-the-hadamard-basis)
      - [Measurement direction of a CNOT interaction](#measurement-direction-of-a-cnot-interaction)
    - [SWAP gate](#swap-gate)
      - [Three-CNOT decomposition of the SWAP gate](#three-cnot-decomposition-of-the-swap-gate)
    - [Greenberger–Horne–Zeilinger state](#greenberger-horne-zeilinger-state)
      - [Localizing a Bell pair from a GHZ state](#localizing-a-bell-pair-from-a-ghz-state)
      - [GHZ preparation with Hadamard and controlled-Z gates](#ghz-preparation-with-hadamard-and-controlled-z-gates)
      - [Bell measurement on one qubit and one leg of a GHZ state](#bell-measurement-on-one-qubit-and-one-leg-of-a-ghz-state)
      - [Quantum circuit preparation of a three-qubit GHZ state](#quantum-circuit-preparation-of-a-three-qubit-ghz-state)
      - [Three-party dense coding with a GHZ state](#three-party-dense-coding-with-a-ghz-state)
      - [GHZ theorem](#ghz-theorem)
        - [GHZ contradiction for N congruent to 3 modulo 4](#ghz-contradiction-for-n-congruent-to-3-modulo-4)
  - [Hadamard test](#hadamard-test)
    - [Mixed-state Hadamard-test quadratures](#mixed-state-hadamard-test-quadratures)
      - [Trace estimation by a maximally mixed Hadamard test](#trace-estimation-by-a-maximally-mixed-hadamard-test)
    - [Eigenphase Hadamard-test probability](#eigenphase-hadamard-test-probability)
    - [Imaginary-part Hadamard test](#imaginary-part-hadamard-test)
  - [Swap test](#swap-test)
- [Parallel quantum gates](#parallel-quantum-gates)
- [Measurement of a Pauli observable](#measurement-of-a-pauli-observable)
  - [Ancilla-assisted Pauli measurement](#ancilla-assisted-pauli-measurement)
  - [Pauli-based computation](#pauli-based-computation)
- [Born rule for a product-basis measurement](#born-rule-for-a-product-basis-measurement)
  - [Matching-outcome projector](#matching-outcome-projector)
  - [Product-state factorization of measurement probabilities](#product-state-factorization-of-measurement-probabilities)
- [Maximally entangled state](#maximally-entangled-state)
  - [Generalized Bell basis](#generalized-bell-basis)
    - [Bell basis](#bell-basis)
      - [Bell-basis conversion circuit](#bell-basis-conversion-circuit)
      - [Bell parity and phase observables](#bell-parity-and-phase-observables)
        - [LOCC discrimination of four Bell states using two copies](#locc-discrimination-of-four-bell-states-using-two-copies)
    - [Generalized Bell state](#generalized-bell-state)
  - [Orthogonal-basis invariance of a real Bell state](#orthogonal-basis-invariance-of-a-real-bell-state)
  - [Bell-state correlation in two real bases](#bell-state-correlation-in-two-real-bases)
- [Shor's algorithm](#shor-s-algorithm)
  - [Candidate-denominator gcd post-processing](#candidate-denominator-gcd-post-processing)
  - [Factor extraction from an even modular order](#factor-extraction-from-an-even-modular-order)
    - [Probability of a useful unit in Shor factorization](#probability-of-a-useful-unit-in-shor-factorization)
  - [Quantum order finding](#quantum-order-finding)
    - [Modular multiplication eigenstates](#modular-multiplication-eigenstates)
    - [Quantum Fourier sampling bound for order finding](#quantum-fourier-sampling-bound-for-order-finding)
    - [Quantum modular exponentiation](#quantum-modular-exponentiation)
    - [Fourier transform of a finite periodic comb](#fourier-transform-of-a-finite-periodic-comb)
      - [Finite geometric Fourier amplitude](#finite-geometric-fourier-amplitude)
    - [Continued-fraction recovery in quantum order finding](#continued-fraction-recovery-in-quantum-order-finding)
      - [Uniqueness of a rational approximation with bounded denominator](#uniqueness-of-a-rational-approximation-with-bounded-denominator)
- [Quantum information theory](quantum-information-theory.md)
  - [Quantum random access code](quantum-information-theory.md#quantum-random-access-code)
    - [Optimal three-to-one qubit random access code](quantum-information-theory.md#optimal-three-to-one-qubit-random-access-code)
  - [Classical communication](quantum-information-theory.md#classical-communication)
  - [Remote state preparation](quantum-information-theory.md#remote-state-preparation)
    - [Asymptotic remote state preparation by block indexing](quantum-information-theory.md#asymptotic-remote-state-preparation-by-block-indexing)
    - [Heralded remote preparation of an arbitrary qubit](quantum-information-theory.md#heralded-remote-preparation-of-an-arbitrary-qubit)
      - [One-bit heralding of a remote state preparation block](quantum-information-theory.md#one-bit-heralding-of-a-remote-state-preparation-block)
    - [Two-bit remote state preparation on a graph-state path](quantum-information-theory.md#two-bit-remote-state-preparation-on-a-graph-state-path)
    - [One-bit remote preparation of real qubit states](quantum-information-theory.md#one-bit-remote-preparation-of-real-qubit-states)
  - [Schumacher compression](quantum-information-theory.md#schumacher-compression)
    - [Memoryless quantum information source](quantum-information-theory.md#memoryless-quantum-information-source)
    - [Quantum typical subspace](quantum-information-theory.md#quantum-typical-subspace)
      - [Typical subspace theorem](quantum-information-theory.md#typical-subspace-theorem)
    - [Reliable quantum source compression](quantum-information-theory.md#reliable-quantum-source-compression)
      - [Typical-subspace compression with a failure flag](quantum-information-theory.md#typical-subspace-compression-with-a-failure-flag)
        - [Average pure-source fidelity after typical projection](quantum-information-theory.md#average-pure-source-fidelity-after-typical-projection)
      - [Finite-dimensional quantum compression converse](quantum-information-theory.md#finite-dimensional-quantum-compression-converse)
  - [Classical-quantum state](quantum-information-theory.md#classical-quantum-state)
    - [Entropy of a classical-quantum state](quantum-information-theory.md#entropy-of-a-classical-quantum-state)
    - [Holevo quantity](quantum-information-theory.md#holevo-quantity)
      - [Holevo quantity under a quantum channel](quantum-information-theory.md#holevo-quantity-under-a-quantum-channel)
      - [Holevo's theorem](quantum-information-theory.md#holevo-s-theorem)
        - [One-shot classical-quantum coding converse](quantum-information-theory.md#one-shot-classical-quantum-coding-converse)
  - [Measure-and-prepare channel](quantum-information-theory.md#measure-and-prepare-channel)
    - [Measurement channel](quantum-information-theory.md#measurement-channel)
      - [Conditional input ensemble after a local measurement](quantum-information-theory.md#conditional-input-ensemble-after-a-local-measurement)
  - [Fidelity of quantum states](quantum-information-theory.md#fidelity-of-quantum-states)
    - [Pure-state trace distance and fidelity identity](quantum-information-theory.md#pure-state-trace-distance-and-fidelity-identity)
    - [Unitary invariance of trace distance and fidelity](quantum-information-theory.md#unitary-invariance-of-trace-distance-and-fidelity)
    - [Squared quantum fidelity](quantum-information-theory.md#squared-quantum-fidelity)
    - [Joint concavity of quantum fidelity](quantum-information-theory.md#joint-concavity-of-quantum-fidelity)
    - [Monotonicity of quantum fidelity under partial trace](quantum-information-theory.md#monotonicity-of-quantum-fidelity-under-partial-trace)
    - [Pure-state gentle measurement bound](quantum-information-theory.md#pure-state-gentle-measurement-bound)
  - [Coherent information](quantum-information-theory.md#coherent-information)
    - [Mutual information and coherent information identity](quantum-information-theory.md#mutual-information-and-coherent-information-identity)
    - [Coherent information upper bound by input entropy](quantum-information-theory.md#coherent-information-upper-bound-by-input-entropy)
    - [Coherent information as an environment conditional entropy](quantum-information-theory.md#coherent-information-as-an-environment-conditional-entropy)
    - [Data-processing inequality for coherent information](quantum-information-theory.md#data-processing-inequality-for-coherent-information)
    - [Anti-degradable quantum channel](quantum-information-theory.md#anti-degradable-quantum-channel)
  - [Joint convexity of quantum relative entropy](quantum-information-theory.md#joint-convexity-of-quantum-relative-entropy)
  - [Quantum ancilla](quantum-information-theory.md#quantum-ancilla)
    - [Ancilla qubit](quantum-information-theory.md#ancilla-qubit)
  - [Positive linear map](quantum-information-theory.md#positive-linear-map)
    - [Positivity (linear maps)](quantum-information-theory.md#positivity-linear-maps)
    - [Decomposable positive map](quantum-information-theory.md#decomposable-positive-map)
      - [Størmer-Woronowicz decomposability theorem](quantum-information-theory.md#stormer-woronowicz-decomposability-theorem)
    - [k-reduction map](quantum-information-theory.md#k-reduction-map)
    - [Completely positive map](quantum-information-theory.md#completely-positive-map)
      - [Quantum operation](quantum-information-theory.md#quantum-operation)
      - [Stinespring representation of a completely positive map](quantum-information-theory.md#stinespring-representation-of-a-completely-positive-map)
      - [Kraus representation](quantum-information-theory.md#kraus-representation)
        - [Trace-preserving and unital Kraus conditions](quantum-information-theory.md#trace-preserving-and-unital-kraus-conditions)
        - [Kraus operator](quantum-information-theory.md#kraus-operator)
      - [Choi matrix](quantum-information-theory.md#choi-matrix)
        - [Spectral Kraus decomposition](quantum-information-theory.md#spectral-kraus-decomposition)
        - [Choi state](quantum-information-theory.md#choi-state)
        - [Choi reconstruction formula](quantum-information-theory.md#choi-reconstruction-formula)
      - [Quantum channel](quantum-information-theory.md#quantum-channel)
        - [Memoryless quantum channel](quantum-information-theory.md#memoryless-quantum-channel)
          - [Quantum erasure channel](quantum-information-theory.md#quantum-erasure-channel)
            - [Entanglement-assisted capacity of a quantum erasure channel](quantum-information-theory.md#entanglement-assisted-capacity-of-a-quantum-erasure-channel)
          - [Entanglement-assisted classical capacity](quantum-information-theory.md#entanglement-assisted-classical-capacity)
        - [Amplitude damping channel](quantum-information-theory.md#amplitude-damping-channel)
          - [Unitary dilation of amplitude damping](quantum-information-theory.md#unitary-dilation-of-amplitude-damping)
          - [Entanglement fidelity of amplitude damping](quantum-information-theory.md#entanglement-fidelity-of-amplitude-damping)
          - [Bloch-vector map of amplitude damping](quantum-information-theory.md#bloch-vector-map-of-amplitude-damping)
            - [Repeated amplitude damping limit](quantum-information-theory.md#repeated-amplitude-damping-limit)
        - [Holevo capacity](quantum-information-theory.md#holevo-capacity)
          - [Superadditivity of Holevo capacity](quantum-information-theory.md#superadditivity-of-holevo-capacity)
          - [Additivity of Holevo capacity](quantum-information-theory.md#additivity-of-holevo-capacity)
            - [Holevo-capacity additivity for entanglement-breaking channels](quantum-information-theory.md#holevo-capacity-additivity-for-entanglement-breaking-channels)
          - [Product-input classical-capacity converse](quantum-information-theory.md#product-input-classical-capacity-converse)
        - [Classical capacity of a quantum channel](quantum-information-theory.md#classical-capacity-of-a-quantum-channel)
          - [Holevo-Schumacher-Westmoreland theorem](quantum-information-theory.md#holevo-schumacher-westmoreland-theorem)
        - [Random unitary channel](quantum-information-theory.md#random-unitary-channel)
          - [Heisenberg-Weyl operator](quantum-information-theory.md#heisenberg-weyl-operator)
            - [Heisenberg-Weyl twirling channel](quantum-information-theory.md#heisenberg-weyl-twirling-channel)
          - [Pauli channel](quantum-information-theory.md#pauli-channel)
            - [Quantum bit-flip channel](quantum-information-theory.md#quantum-bit-flip-channel)
              - [Average pure-qubit fidelity of a bit-flip channel](quantum-information-theory.md#average-pure-qubit-fidelity-of-a-bit-flip-channel)
            - [Quantum depolarizing channel](quantum-information-theory.md#quantum-depolarizing-channel)
              - [Entanglement-assisted capacity of a qubit depolarizing channel](quantum-information-theory.md#entanglement-assisted-capacity-of-a-qubit-depolarizing-channel)
                - [High-noise capacity ratio for qubit depolarization](quantum-information-theory.md#high-noise-capacity-ratio-for-qubit-depolarization)
              - [Depolarizing noise weight above one](quantum-information-theory.md#depolarizing-noise-weight-above-one)
              - [Pauli-mixture parametrization of qubit depolarization](quantum-information-theory.md#pauli-mixture-parametrization-of-qubit-depolarization)
              - [Holevo capacity of a qubit depolarizing channel](quantum-information-theory.md#holevo-capacity-of-a-qubit-depolarizing-channel)
                - [Product-input block bound for a qubit depolarizing channel](quantum-information-theory.md#product-input-block-bound-for-a-qubit-depolarizing-channel)
            - [Phase-flip channel](quantum-information-theory.md#phase-flip-channel)
              - [Iterated phase-flip channel](quantum-information-theory.md#iterated-phase-flip-channel)
            - [Dephasing channel](quantum-information-theory.md#dephasing-channel)
              - [Complex environment overlap in qubit dephasing](quantum-information-theory.md#complex-environment-overlap-in-qubit-dephasing)
        - [Unital quantum channel](quantum-information-theory.md#unital-quantum-channel)
          - [Eigenvalue mixing matrix of a unital quantum channel](quantum-information-theory.md#eigenvalue-mixing-matrix-of-a-unital-quantum-channel)
            - [Spectral majorization under a unital quantum channel](quantum-information-theory.md#spectral-majorization-under-a-unital-quantum-channel)
          - [Werner–Holevo channel](quantum-information-theory.md#werner-holevo-channel)
        - [Strictly contractive quantum channel](quantum-information-theory.md#strictly-contractive-quantum-channel)
        - [Primitive quantum channel](quantum-information-theory.md#primitive-quantum-channel)
        - [Stinespring dilation](quantum-information-theory.md#stinespring-dilation)
        - [Entanglement fidelity](quantum-information-theory.md#entanglement-fidelity)
          - [Entanglement fidelity bound by state fidelity](quantum-information-theory.md#entanglement-fidelity-bound-by-state-fidelity)
          - [Quantum Fano inequality](quantum-information-theory.md#quantum-fano-inequality)
          - [Kraus formula for entanglement fidelity](quantum-information-theory.md#kraus-formula-for-entanglement-fidelity)
          - [Operation fidelity](quantum-information-theory.md#operation-fidelity)
        - [Lindblad equation](quantum-information-theory.md#lindblad-equation)
          - [Lindblad dissipator](quantum-information-theory.md#lindblad-dissipator)
          - [Lindblad operator](quantum-information-theory.md#lindblad-operator)
          - [Lindbladian](quantum-information-theory.md#lindbladian)
            - [Finite-dimensional Lindbladians have stationary states](quantum-information-theory.md#finite-dimensional-lindbladians-have-stationary-states)
            - [Lindbladian gap](quantum-information-theory.md#lindbladian-gap)
            - [Unique stationary state of a Lindbladian](quantum-information-theory.md#unique-stationary-state-of-a-lindbladian)
          - [Quantum Trajectory Theory](quantum-information-theory.md#quantum-trajectory-theory)
            - [Dark state of a Lindblad equation](quantum-information-theory.md#dark-state-of-a-lindblad-equation)
  - [Quantum de Finetti theorem](quantum-information-theory.md#quantum-de-finetti-theorem)
    - [Mean-field ansatz from the quantum de Finetti theorem](quantum-information-theory.md#mean-field-ansatz-from-the-quantum-de-finetti-theorem)
  - [Separable quantum state](quantum-information-theory.md#separable-quantum-state)
    - [Separable positive operator](quantum-information-theory.md#separable-positive-operator)
    - [Positive-map separability criterion](quantum-information-theory.md#positive-map-separability-criterion)
    - [Entanglement witness](quantum-information-theory.md#entanglement-witness)
    - [Partial transpose](quantum-information-theory.md#partial-transpose)
      - [Partial transpose of a maximally entangled projector](quantum-information-theory.md#partial-transpose-of-a-maximally-entangled-projector)
      - [Positive partial transpose](quantum-information-theory.md#positive-partial-transpose)
        - [PPT maximally entangled overlap bound](quantum-information-theory.md#ppt-maximally-entangled-overlap-bound)
      - [Trace-adjoint identity for partial transpose](quantum-information-theory.md#trace-adjoint-identity-for-partial-transpose)
    - [Positive partial transpose criterion](quantum-information-theory.md#positive-partial-transpose-criterion)
    - [Entanglement-breaking channel](quantum-information-theory.md#entanglement-breaking-channel)
      - [Separable Choi-state criterion for entanglement breaking](quantum-information-theory.md#separable-choi-state-criterion-for-entanglement-breaking)
      - [Rank-one Kraus representation of an entanglement-breaking channel](quantum-information-theory.md#rank-one-kraus-representation-of-an-entanglement-breaking-channel)
  - [Isotropic quantum state](quantum-information-theory.md#isotropic-quantum-state)
  - [Swap operator](quantum-information-theory.md#swap-operator)
  - [Pretty good measurement](quantum-information-theory.md#pretty-good-measurement)
  - [Quantum state discrimination](quantum-information-theory.md#quantum-state-discrimination)
  - [Quantum binary hypothesis testing](quantum-information-theory.md#quantum-binary-hypothesis-testing)
    - [Binary test for quantum decoding success](quantum-information-theory.md#binary-test-for-quantum-decoding-success)
    - [Quantum channel discrimination](quantum-information-theory.md#quantum-channel-discrimination)
      - [Diamond norm of the transposition map](quantum-information-theory.md#diamond-norm-of-the-transposition-map)
    - [Holevo–Helstrom theorem](quantum-information-theory.md#holevo-helstrom-theorem)
      - [Equal-prior discrimination of qubit states](quantum-information-theory.md#equal-prior-discrimination-of-qubit-states)
  - [Entanglement monogamy](quantum-information-theory.md#entanglement-monogamy)
    - [Coffman--Kundu--Wootters inequality](quantum-information-theory.md#coffman-kundu-wootters-inequality)
    - [Entanglement area law](quantum-information-theory.md#entanglement-area-law)
      - [Tensor-network area-law bound](quantum-information-theory.md#tensor-network-area-law-bound)
  - [Werner state](quantum-information-theory.md#werner-state)
  - [Ancilla bit](quantum-information-theory.md#ancilla-bit)
- [Quantum decoherence](#quantum-decoherence)
  - [Zurek spin-bath model](#zurek-spin-bath-model)
    - [Random-coupling spin-bath decoherence](#random-coupling-spin-bath-decoherence)
      - [Short-time Gaussian spin-bath decoherence](#short-time-gaussian-spin-bath-decoherence)
      - [Ensemble spin-bath coherence](#ensemble-spin-bath-coherence)
    - [Finite spin-bath coherence recurrence](#finite-spin-bath-coherence-recurrence)
  - [Decoherence factor](#decoherence-factor)
    - [Conditional environment overlap](#conditional-environment-overlap)
      - [Single-qubit interference with conditional environment states](#single-qubit-interference-with-conditional-environment-states)
  - [Quantum recoherence](#quantum-recoherence)
  - [Measurement problem](#measurement-problem)
- [Foundations of quantum mechanics](#foundations-of-quantum-mechanics)
  - [Einstein–Podolsky–Rosen paradox](#einstein-podolsky-rosen-paradox)
    - [Einstein–Podolsky–Rosen criterion of reality](#einstein-podolsky-rosen-criterion-of-reality)
  - [Superselection rule](#superselection-rule)
  - [EPR criterion of reality](#epr-criterion-of-reality)
  - [de Broglie-Bohm theory](#de-broglie-bohm-theory)
    - [Bohmian circulation of an angular-momentum eigenstate](#bohmian-circulation-of-an-angular-momentum-eigenstate)
    - [Quantum potential](#quantum-potential)
    - [Guidance equation](#guidance-equation)
      - [Quantum equilibrium equivariance](#quantum-equilibrium-equivariance)
  - [Ontological model of a quantum system](#ontological-model-of-a-quantum-system)
    - [Pusey-Barrett-Rudolph theorem](#pusey-barrett-rudolph-theorem)
      - [Tensor-power reduction of PBR overlap](#tensor-power-reduction-of-pbr-overlap)
      - [PBR exclusion measurement for zero and plus](#pbr-exclusion-measurement-for-zero-and-plus)
    - [Preparation independence](#preparation-independence)
    - [Psi-epistemic model](#psi-epistemic-model)
    - [Psi-ontic model](#psi-ontic-model)
  - [Bell theorem](#bell-theorem)
    - [Bell inequality](#bell-inequality)
    - [Chained modular Bell inequality](#chained-modular-bell-inequality)
      - [Coplanar qubit realization of the chained Bell inequality](#coplanar-qubit-realization-of-the-chained-bell-inequality)
    - [Local hidden-variable theory](#local-hidden-variable-theory)
      - [Setting-independent heralding preserves Bell locality](#setting-independent-heralding-preserves-bell-locality)
      - [Outcome independence](#outcome-independence)
      - [Bell local causality](#bell-local-causality)
      - [Deterministic local hidden-variable model](#deterministic-local-hidden-variable-model)
      - [Outcome determinism](#outcome-determinism)
      - [Parameter independence](#parameter-independence)
      - [Measurement independence](#measurement-independence)
    - [CHSH inequality](#chsh-inequality)
      - [CHSH optimum from the correlation tensor](#chsh-optimum-from-the-correlation-tensor)
      - [Gisin's theorem](#gisin-s-theorem)
        - [CHSH axes for an entangled pure two-qubit state](#chsh-axes-for-an-entangled-pure-two-qubit-state)
      - [No-signalling box](#no-signalling-box)
        - [Popescu–Rohrlich box](#popescu-rohrlich-box)
          - [One-bit computation using Popescu–Rohrlich boxes](#one-bit-computation-using-popescu-rohrlich-boxes)
  - [Objective-collapse theory](#objective-collapse-theory)
    - [Ghirardi-Rimini-Weber theory](#ghirardi-rimini-weber-theory)
      - [GRW localization operator](#grw-localization-operator)
        - [GRW collapse-centre event probabilities](#grw-collapse-centre-event-probabilities)
      - [GRW amplification mechanism](#grw-amplification-mechanism)
        - [GRW branch persistence versus geometric containment](#grw-branch-persistence-versus-geometric-containment)
      - [GRW spontaneous heating](#grw-spontaneous-heating)
    - [Local quantum state under objective collapse](#local-quantum-state-under-objective-collapse)
      - [Quantum state readout device](#quantum-state-readout-device)
      - [Proper mixed state](#proper-mixed-state)
      - [Improper mixed state](#improper-mixed-state)
- [Quantum gravity](#quantum-gravity)
  - [Two-dimensional quantum gravity](#two-dimensional-quantum-gravity)
  - [Graviton](#graviton)
  - [Semiclassical gravity](#semiclassical-gravity)
    - [Semiclassical Einstein equation](#semiclassical-einstein-equation)
      - [Page–Geilker experiment](#page-geilker-experiment)
  - [Gravitationally induced entanglement](#gravitationally-induced-entanglement)
    - [Bose--Marletto--Vedral experiment](#bose-marletto-vedral-experiment)
- [Pure state](#pure-state)
  - [Relative state of a bipartite vector](#relative-state-of-a-bipartite-vector)
    - [Index state](#index-state)
      - [Conjugate index vector](#conjugate-index-vector)
- [Partial trace](#partial-trace)
  - [Partial trace positivity from product vectors](#partial-trace-positivity-from-product-vectors)
  - [Haar twirling conditional expectation](#haar-twirling-conditional-expectation)
- [Adiabatic theorem](#adiabatic-theorem)
  - [Adiabatic preparation of a computational history state](#adiabatic-preparation-of-a-computational-history-state)
- [Topological quantum matter](topological-quantum-matter.md)
  - [Topological quantum order](topological-quantum-matter.md#topological-quantum-order)
    - [Backward preservation of local indistinguishability](topological-quantum-matter.md#backward-preservation-of-local-indistinguishability)
  - [Local indistinguishability](topological-quantum-matter.md#local-indistinguishability)
  - [Abelian Chern--Simons theory](topological-quantum-matter.md#abelian-chern-simons-theory)
    - [Chern-Simons source stress convention](topological-quantum-matter.md#chern-simons-source-stress-convention)
    - [K-matrix](topological-quantum-matter.md#k-matrix)
      - [Anyon lattice of an Abelian Chern--Simons theory](topological-quantum-matter.md#anyon-lattice-of-an-abelian-chern-simons-theory)
      - [Chern--Simons flux attachment](topological-quantum-matter.md#chern-simons-flux-attachment)
      - [Lagrangian subgroup of Abelian anyons](topological-quantum-matter.md#lagrangian-subgroup-of-abelian-anyons)
    - [Torus ground-state degeneracy of an Abelian Chern--Simons theory](topological-quantum-matter.md#torus-ground-state-degeneracy-of-an-abelian-chern-simons-theory)
      - [Wilson-loop algebra of an Abelian Chern--Simons theory](topological-quantum-matter.md#wilson-loop-algebra-of-an-abelian-chern-simons-theory)
  - [Anyon](topological-quantum-matter.md#anyon)
    - [Topological spin](topological-quantum-matter.md#topological-spin)
    - [Charge-flux composite](topological-quantum-matter.md#charge-flux-composite)
      - [Aharonov-Bohm effect](topological-quantum-matter.md#aharonov-bohm-effect)
      - [Aharonov-Casher effect](topological-quantum-matter.md#aharonov-casher-effect)
    - [Mutual semion](topological-quantum-matter.md#mutual-semion)
    - [Anyon condensation at a boundary](topological-quantum-matter.md#anyon-condensation-at-a-boundary)
      - [Electric and magnetic boundaries of the surface code](topological-quantum-matter.md#electric-and-magnetic-boundaries-of-the-surface-code)
  - [Topological superconductor](topological-quantum-matter.md#topological-superconductor)
    - [Quadratic fermion Hamiltonian](topological-quantum-matter.md#quadratic-fermion-hamiltonian)
      - [Bogoliubov--de Gennes Hamiltonian](topological-quantum-matter.md#bogoliubov-de-gennes-hamiltonian)
        - [Particle-hole symmetry of a Bogoliubov--de Gennes Hamiltonian](topological-quantum-matter.md#particle-hole-symmetry-of-a-bogoliubov-de-gennes-hamiltonian)
      - [Majorana fermion operator](topological-quantum-matter.md#majorana-fermion-operator)
        - [Majorana zero mode](topological-quantum-matter.md#majorana-zero-mode)
          - [Majorana zero mode at a mass domain wall](topological-quantum-matter.md#majorana-zero-mode-at-a-mass-domain-wall)
            - [Continuum p-wave Majorana interface mode](topological-quantum-matter.md#continuum-p-wave-majorana-interface-mode)
          - [Dense encoding with Majorana zero modes](topological-quantum-matter.md#dense-encoding-with-majorana-zero-modes)
          - [Local indistinguishability of separated Majorana zero modes](topological-quantum-matter.md#local-indistinguishability-of-separated-majorana-zero-modes)
          - [Majorana braiding operator](topological-quantum-matter.md#majorana-braiding-operator)
            - [Measurement-only Majorana braiding](topological-quantum-matter.md#measurement-only-majorana-braiding)
              - [Forced Majorana parity measurement](topological-quantum-matter.md#forced-majorana-parity-measurement)
      - [Fermion parity](topological-quantum-matter.md#fermion-parity)
        - [Fermion-parity measurement](topological-quantum-matter.md#fermion-parity-measurement)
    - [Chiral Majorana edge mode](topological-quantum-matter.md#chiral-majorana-edge-mode)
      - [Boundary condition of a chiral Majorana edge mode](topological-quantum-matter.md#boundary-condition-of-a-chiral-majorana-edge-mode)
    - [Kitaev chain](topological-quantum-matter.md#kitaev-chain)
  - [Topological equivalence of gapped Hamiltonians](topological-quantum-matter.md#topological-equivalence-of-gapped-hamiltonians)
    - [Quasi-adiabatic continuation](topological-quantum-matter.md#quasi-adiabatic-continuation)
    - [Winding number of a one-dimensional Bogoliubov--de Gennes Hamiltonian](topological-quantum-matter.md#winding-number-of-a-one-dimensional-bogoliubov-de-gennes-hamiltonian)
  - [Symmetry-protected topological phase](topological-quantum-matter.md#symmetry-protected-topological-phase)
    - [Projective virtual symmetry of a matrix product state](topological-quantum-matter.md#projective-virtual-symmetry-of-a-matrix-product-state)
      - [Protected edge state of a symmetry-protected topological phase](topological-quantum-matter.md#protected-edge-state-of-a-symmetry-protected-topological-phase)
    - [Cluster state](topological-quantum-matter.md#cluster-state)
  - [Intrinsic topological order](topological-quantum-matter.md#intrinsic-topological-order)
  - [Kramers--Wannier duality](topological-quantum-matter.md#kramers-wannier-duality)
    - [Kramers--Wannier intertwiner](topological-quantum-matter.md#kramers-wannier-intertwiner)
    - [Kramers--Wannier projected entangled pair operator](topological-quantum-matter.md#kramers-wannier-projected-entangled-pair-operator)
  - [One-form symmetry](topological-quantum-matter.md#one-form-symmetry)
- [Quantum error correction](quantum-error-correction.md)
  - [Quantum error-correcting code](quantum-error-correction.md#quantum-error-correcting-code)
  - [Logical qubit](quantum-error-correction.md#logical-qubit)
  - [Concatenated quantum error-correcting code](quantum-error-correction.md#concatenated-quantum-error-correcting-code)
    - [Five-qubit concatenation threshold](quantum-error-correction.md#five-qubit-concatenation-threshold)
  - [Five-qubit error correcting code](quantum-error-correction.md#five-qubit-error-correcting-code)
    - [Five-qubit stabilizer syndrome table](quantum-error-correction.md#five-qubit-stabilizer-syndrome-table)
  - [Quantum error detection](quantum-error-correction.md#quantum-error-detection)
    - [Correction implies detection at twice the weight](quantum-error-correction.md#correction-implies-detection-at-twice-the-weight)
  - [Nondegenerate quantum error-correcting code](quantum-error-correction.md#nondegenerate-quantum-error-correcting-code)
    - [Quantum Hamming bound](quantum-error-correction.md#quantum-hamming-bound)
      - [Perfect quantum error-correcting code](quantum-error-correction.md#perfect-quantum-error-correcting-code)
  - [Distance of a quantum error-correcting code](quantum-error-correction.md#distance-of-a-quantum-error-correcting-code)
    - [Correctable Pauli error radius](quantum-error-correction.md#correctable-pauli-error-radius)
    - [Quantum Singleton bound](quantum-error-correction.md#quantum-singleton-bound)
    - [Quantum erasure correction](quantum-error-correction.md#quantum-erasure-correction)
  - [Linearity of coherent quantum error correction](quantum-error-correction.md#linearity-of-coherent-quantum-error-correction)
  - [Knill--Laflamme condition](quantum-error-correction.md#knill-laflamme-condition)
    - [Necessity of the Knill-Laflamme condition](quantum-error-correction.md#necessity-of-the-knill-laflamme-condition)
    - [Constructive recovery from the Knill-Laflamme condition](quantum-error-correction.md#constructive-recovery-from-the-knill-laflamme-condition)
  - [Stabilizer code](quantum-error-correction.md#stabilizer-code)
    - [Symplectic representation of a stabilizer code](quantum-error-correction.md#symplectic-representation-of-a-stabilizer-code)
    - [CSS code](quantum-error-correction.md#css-code)
      - [Nested-code CSS syndrome recovery](quantum-error-correction.md#nested-code-css-syndrome-recovery)
    - [Centralizer of a stabilizer group](quantum-error-correction.md#centralizer-of-a-stabilizer-group)
    - [Local correctability of a stabilizer code](quantum-error-correction.md#local-correctability-of-a-stabilizer-code)
      - [Pauli error criterion for a stabilizer code](quantum-error-correction.md#pauli-error-criterion-for-a-stabilizer-code)
    - [Dressed stabilizer under a weak local perturbation](quantum-error-correction.md#dressed-stabilizer-under-a-weak-local-perturbation)
    - [Distance of a stabilizer code](quantum-error-correction.md#distance-of-a-stabilizer-code)
    - [Error syndrome](quantum-error-correction.md#error-syndrome)
      - [Stabilizer-syndrome coset](quantum-error-correction.md#stabilizer-syndrome-coset)
    - [Phase-flip repetition code](quantum-error-correction.md#phase-flip-repetition-code)
      - [Logical Hadamard convention for a phase-flip repetition code](quantum-error-correction.md#logical-hadamard-convention-for-a-phase-flip-repetition-code)
      - [Logical failure of the three-qubit phase-flip repetition code](quantum-error-correction.md#logical-failure-of-the-three-qubit-phase-flip-repetition-code)
      - [Phase-flip protection by Hadamard conjugation](quantum-error-correction.md#phase-flip-protection-by-hadamard-conjugation)
      - [Majority-vote decoding of a repetition code](quantum-error-correction.md#majority-vote-decoding-of-a-repetition-code)
    - [Bit-flip repetition code](quantum-error-correction.md#bit-flip-repetition-code)
      - [Coherent syndrome extraction for the three-qubit repetition code](quantum-error-correction.md#coherent-syndrome-extraction-for-the-three-qubit-repetition-code)
        - [Timed bit flip during repetition-code syndrome extraction](quantum-error-correction.md#timed-bit-flip-during-repetition-code-syndrome-extraction)
          - [Exact encoded-state failure with a faulty parity check](quantum-error-correction.md#exact-encoded-state-failure-with-a-faulty-parity-check)
    - [Concatenated phase-and-bit-flip repetition code](quantum-error-correction.md#concatenated-phase-and-bit-flip-repetition-code)
      - [Shor code](quantum-error-correction.md#shor-code)
        - [Shor-code phase-flip syndrome](quantum-error-correction.md#shor-code-phase-flip-syndrome)
    - [Steane code](quantum-error-correction.md#steane-code)
      - [Nondegenerate phase-flip correction in the Steane code](quantum-error-correction.md#nondegenerate-phase-flip-correction-in-the-steane-code)
    - [Color code](quantum-error-correction.md#color-code)
      - [String operator in a topological code](quantum-error-correction.md#string-operator-in-a-topological-code)
    - [Surface code](quantum-error-correction.md#surface-code)
      - [Surface code on a chain of spheres](quantum-error-correction.md#surface-code-on-a-chain-of-spheres)
      - [Surface-code decoding as a random-bond Ising model](quantum-error-correction.md#surface-code-decoding-as-a-random-bond-ising-model)
      - [Ground-state splitting of a surface-code cylinder](quantum-error-correction.md#ground-state-splitting-of-a-surface-code-cylinder)
      - [Toric code](quantum-error-correction.md#toric-code)
        - [Surface-code anyon model](quantum-error-correction.md#surface-code-anyon-model)
- [Tensor network state](#tensor-network-state)
  - [Matrix product state](#matrix-product-state)
    - [Matrix product state as an unravelling of a completely positive map](#matrix-product-state-as-an-unravelling-of-a-completely-positive-map)
    - [Matrix product state transfer map](#matrix-product-state-transfer-map)
    - [Injective matrix product state](#injective-matrix-product-state)
      - [Blocking a matrix product state](#blocking-a-matrix-product-state)
      - [Uniform matrix product state](#uniform-matrix-product-state)
      - [Fundamental theorem of matrix product states](#fundamental-theorem-of-matrix-product-states)
        - [Gauge equivalence of injective matrix product state tensors](#gauge-equivalence-of-injective-matrix-product-state-tensors)
      - [Affleck--Kennedy--Lieb--Tasaki state](#affleck-kennedy-lieb-tasaki-state)
        - [Pauli-matrix representation of the Affleck--Kennedy--Lieb--Tasaki state](#pauli-matrix-representation-of-the-affleck-kennedy-lieb-tasaki-state)
          - [Two-site support of the Pauli-matrix Affleck--Kennedy--Lieb--Tasaki tensor](#two-site-support-of-the-pauli-matrix-affleck-kennedy-lieb-tasaki-tensor)
        - [Affleck--Kennedy--Lieb--Tasaki parent Hamiltonian](#affleck-kennedy-lieb-tasaki-parent-hamiltonian)
        - [Symmetry-protected equivalence of the Affleck--Kennedy--Lieb--Tasaki state and cluster state](#symmetry-protected-equivalence-of-the-affleck-kennedy-lieb-tasaki-state-and-cluster-state)
    - [Entanglement spectrum of a matrix product state](#entanglement-spectrum-of-a-matrix-product-state)
    - [Parent Hamiltonian of a matrix product state](#parent-hamiltonian-of-a-matrix-product-state)
  - [Matrix product operator](#matrix-product-operator)
  - [Projected entangled pair state](#projected-entangled-pair-state)
  - [Projected entangled pair operator](#projected-entangled-pair-operator)
- [Hamiltonian simulation](#hamiltonian-simulation)
  - [Commuting local Hamiltonian simulation](#commuting-local-hamiltonian-simulation)
  - [Local Hamiltonian](#local-hamiltonian)
    - [Operator support](#operator-support)
    - [Stoquastic Hamiltonian](#stoquastic-hamiltonian)
    - [Spectral filtering of Hamiltonian terms](#spectral-filtering-of-hamiltonian-terms)
      - [Almost-exponential locality of filtered Hamiltonian terms](#almost-exponential-locality-of-filtered-hamiltonian-terms)
      - [Filtering preserves existing frustration freeness](#filtering-preserves-existing-frustration-freeness)
      - [Commuting with a ground projector does not imply frustration freeness](#commuting-with-a-ground-projector-does-not-imply-frustration-freeness)
      - [Telescoping local-shell decomposition](#telescoping-local-shell-decomposition)
    - [Local Hamiltonian problem](#local-hamiltonian-problem)
      - [Local-energy measurement verification](#local-energy-measurement-verification)
    - [Diagonal Hamiltonian](#diagonal-hamiltonian)
    - [Frustration-free quantum Hamiltonian](#frustration-free-quantum-hamiltonian)
      - [Detectability lemma](#detectability-lemma)
        - [Local projector cone in a frustration-free chain](#local-projector-cone-in-a-frustration-free-chain)
          - [Exponential clustering from layered projectors](#exponential-clustering-from-layered-projectors)
      - [Frustration freeness](#frustration-freeness)
    - [k-local Hamiltonian](#k-local-hamiltonian)
  - [Product-formula Hamiltonian simulation](#product-formula-hamiltonian-simulation)
    - [First-order two-local Hamiltonian simulation](#first-order-two-local-hamiltonian-simulation)
    - [Second-order product formula](#second-order-product-formula)
  - [Simulation of a computable diagonal Hamiltonian](#simulation-of-a-computable-diagonal-hamiltonian)
    - [Pauli-string phase by parity computation](#pauli-string-phase-by-parity-computation)
- [Block encoding](#block-encoding)

## Hadamard transform

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hadamard_transform)

The normalized Hadamard transform maps a vector indexed by binary strings through entries $2^{-n/2}(-1)^{x\cdot y}$. It is its own inverse and an orthogonal transform. The [Hadamard gate](#hadamard-gate) is the $n=1$ quantum case, and the [Hadamard basis](#hadamard-basis) is the image of its computational basis. The [Walsh-Hadamard transform](#walsh-hadamard-transform) gives the same tensor-power construction.

### Hadamard gate

↑ **Parent:** [Hadamard transform](#hadamard-transform)

The Hadamard gate maps

$$
|0\rangle\mapsto\frac{|0\rangle+|1\rangle}{\sqrt2},
\qquad
|1\rangle\mapsto\frac{|0\rangle-|1\rangle}{\sqrt2}.
$$

#### Photon-number reference for a Hadamard gate

↑ **Parent:** [Hadamard gate](#hadamard-gate)

A flat reference over $k$ adjacent [Fock states](quantum-field-theory.md#fock-state) has overlap $r_k$ with a one-photon shift and $s_k$ with a two-photon shift. These overlaps, obtained by counting shared number states, determine the reduced [qubit](quantum-mechanics.md#qubit) channel of a number-conserving Hadamard interaction. For $k\ge2$, its squared fidelity with the desired pure output is $1-(1+xz)/(2k)$ for input [Bloch vector](#bloch-vector) $(x,y,z)$. Its worst-case infidelity is $3/(4k)$ because $|xz|\le1/2$. At $k=1$ the two-shift overlap is zero, not $-1$, and the fidelity is $1/2+(y^2-xz)/4$. Broad coherent number support, rather than merely a large fixed [photon](quantum-mechanics.md#photon) number, suppresses distinguishability of the outgoing field states.

#### Uniform quantum superposition

↑ **Parent:** [Hadamard gate](#hadamard-gate)

The uniform superposition of all $n$-bit strings is

$$
\frac1{\sqrt{2^n}}\sum_{x\in\{0,1\}^n}|x\rangle
=H^{\otimes n}|0\rangle^{\otimes n}.
$$

### Walsh-Hadamard transform

↑ **Parent:** [Hadamard transform](#hadamard-transform)

On $n$ qubits, the Walsh-Hadamard transform satisfies

$$
H^{\otimes n}|x\rangle
=2^{-n/2}\sum_{y\in\{0,1\}^n}(-1)^{x\cdot y}|y\rangle,
$$

where the dot product is evaluated modulo two.

This is the [Hadamard transform](#hadamard-transform) acting on the computational basis of $n$ qubits.

### Hadamard basis

↑ **Parent:** [Hadamard transform](#hadamard-transform)

The qubit Hadamard basis consists of $|+\rangle=(|0\rangle+|1\rangle)/\sqrt2$ and $|-\rangle=(|0\rangle-|1\rangle)/\sqrt2$.

## Minimal coupling

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Minimal_coupling)

Minimal coupling introduces a gauge potential through a covariant derivative, or replaces canonical momentum by $p-qA$. The associated scalar potential supplies the electric coupling. [Magnetic minimal coupling](#magnetic-minimal-coupling) is the magnetic-only nonrelativistic case.

### Magnetic minimal coupling

↑ **Parent:** [Minimal coupling](#minimal-coupling)

For a particle of charge $q$ in a vector potential $\mathbf A$, the canonical momentum in the free Hamiltonian is replaced by $\mathbf p-q\mathbf A$, giving

$$
H=\frac1{2m}(-i\hbar\nabla-q\mathbf A)^2.
$$

## Quantum fluctuation

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_fluctuation)

A [quantum fluctuation](#quantum-fluctuation) is a nonzero variance of an observable in a quantum state, even when its mean vanishes. A vacuum field mode has such zero-point variance. In an inflationary background, the expanding geometry transfers short-wavelength vacuum field fluctuations into [primordial perturbations](cosmic-inflation.md#primordial-perturbation) as their wavelengths cross the [Hubble radius](cosmology.md#hubble-radius).

<h2 id="gauge-covariance-of-the-schrodinger-equation">Gauge covariance of the Schrödinger equation</h2>

↑ **Parent:** [Quantum theory](quantum-theory.md)

For a particle of charge $-e$, the changes $A\mapsto A+\nabla f$ and $\phi\mapsto\phi-\partial_t f$ leave the minimally coupled Schrödinger equation invariant when $\psi\mapsto e^{-ief/\hbar}\psi$.

<h2 id="quantum-measurement">Measurement in quantum mechanics</h2>

↑ **Parent:** [Quantum theory](quantum-theory.md)

[This section is present in another page, follow this link to view it.](quantum-measurement.md)

## Amplitude amplification

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Amplitude_amplification)

If a state has good amplitude $\sin\theta$, the product of the reflection in the bad axis and the reflection in the state line rotates its good-bad plane by $2\theta$. After $k$ iterations the good probability is

$$
\sin^2((2k+1)\theta),
$$

so $O(1/\sin\theta)$ iterations raise a small good amplitude close to one.

### Nearest-integer stopping for amplitude amplification

↑ **Parent:** [Amplitude amplification](#amplitude-amplification)

For known initial success probability $p\in(0,1)$, this choice of iteration count ensures $|(2r+1)\theta-\pi/2|\leq\theta$. Hence the success probability after [amplitude amplification](#amplitude-amplification) is at least $\cos^2\theta=1-p$. Counting initial state preparation and the forward and inverse preparation in each iterate gives $2r+1$ preparation-unitary applications, asymptotic to $\pi/(2\sqrt p)$ as $p\to0$.

### Two-dimensional matrix for phase amplitude amplification

↑ **Parent:** [Amplitude amplification](#amplitude-amplification)

If the state-preparation unitary sends $|0\rangle$ to $|\psi\rangle=\sin\chi|g\rangle+\cos\chi|b\rangle$, use the orthonormal good/bad basis. The marked-space phase is diagonal there, and conjugating a phase on $|0\rangle$ gives the rank-one phase in the displayed formula. Their product is unitary. An arbitrary preparation unitary not sending zero to this state need not preserve this particular two-dimensional subspace. Matrices in unnormalized good/bad vectors must not be described as unitary in the ordinary Euclidean [inner product](linear-algebra.md#inner-product).

### Exact amplitude amplification

↑ **Parent:** [Amplitude amplification](#amplitude-amplification)

If the initial good amplitude $p=\sin\theta$ is known, an ancillary qubit can reduce it to $\sin\theta'=p c$ with $\theta'=\pi/(4k+2)$ and $0<c\leq1$. After $k$ ordinary amplitude-amplification iterations the good amplitude is $\sin((2k+1)\theta')=1$, so the target state is prepared exactly.

#### Known-state success dilution for exact amplitude amplification

↑ **Parent:** [Exact amplitude amplification](#exact-amplitude-amplification)

For known good probability $p=\sin^2\theta$, choose $j=\lceil\pi/(4\theta)-1/2\rceil$. A known reversible preparation of one state with good probability $p_*$ permits $j$ ordinary [amplitude amplification](#amplitude-amplification) iterations to reach the good subspace exactly. With ancillary marking access, prepare a flag with one-probability $q=p_*/p$ and define joint success as good data and flag one. Reflection about the prepared product state is known, while the joint phase test requires a controlled marking oracle or a computed Boolean output. This changes the success projector and enlarges the state space; it does not evade the [obstruction to uniform probability lowering by a unitary](#obstruction-to-uniform-probability-lowering-by-a-unitary). Query costs of preparation, its inverse and marking must all be counted.

#### Phase-matched amplitude amplification

↑ **Parent:** [Exact amplitude amplification](#exact-amplitude-amplification)

Phase-matched amplitude amplification replaces the two sign-flip reflections by selective phase rotations. Choosing their phases from the known initial overlap can rotate the state exactly onto the target even when an integer number of ordinary Grover rotations would overshoot it.

### Geometric amplitude-amplification schedule

↑ **Parent:** [Amplitude amplification](#amplitude-amplification)

A geometric amplitude-amplification schedule tries iteration counts $1,2,4,8,\ldots$ when the initial good amplitude is unknown. It reaches the unknown optimal scale with only a geometric-series overhead.

## Reflection operator

↑ **Parent:** [Quantum theory](quantum-theory.md)

For a unit vector $|\psi\rangle$, the reflection $I-2|\psi\rangle\langle\psi|$ negates the component parallel to $|\psi\rangle$ and fixes its orthogonal complement.

### Projector phase rotation

↑ **Parent:** [Reflection operator](#reflection-operator)

For an [orthogonal projection](hilbert-space.md#orthogonal-projection), $P^k=P$ for $k\geq1$. Summing the exponential series proves the displayed identity. At $\theta=\pi$, the operator is $I-2P$, which changes the sign on the range and fixes its orthogonal complement. In [Grover search algorithm](#grover-s-algorithm), the marked-state reflection and the uniform-state reflection compose to the search iterate up to an irrelevant [global phase](quantum-mechanics.md#global-phase).

### Selective phase rotation

↑ **Parent:** [Reflection operator](#reflection-operator)

For a unit vector $|\psi\rangle$ and real $\phi$,

$$
R_\psi^\phi=I-(1-e^{i\phi})|\psi\rangle\langle\psi|
$$

multiplies the component parallel to $|\psi\rangle$ by $e^{i\phi}$ and fixes its orthogonal complement. The case $\phi=\pi$ is a [reflection operator](#reflection-operator).

A reflection operator is a unitary involution that changes sign on one orthogonal subspace and fixes its orthogonal complement. For a unit vector $|\psi\rangle$, $I-2|\psi\rangle\langle\psi|$ reflects in the hyperplane perpendicular to $|\psi\rangle$.

## HHL algorithm

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/HHL_algorithm)

The HHL algorithm prepares a quantum state proportional to $A^{-1}b$ for a sparse, efficiently accessible, well-conditioned linear system $Ax=b$, provided that $|b\rangle$ can be prepared efficiently. Its runtime depends polynomially on the sparsity, condition number, inverse precision, and $\log N$.

### HHL controlled reciprocal rotation

↑ **Parent:** [HHL algorithm](#hhl-algorithm)

On a positive [eigenvalue](linear-operator-theory.md#eigenvalue) label $\lambda$ and a clean [quantum ancilla](quantum-information-theory.md#quantum-ancilla), the [HHL algorithm](#hhl-algorithm) applies a [quantum variable rotation](#quantum-variable-rotation) with angle $\theta_\lambda=\arcsin(c/\lambda)$, where $0<c\leq\lambda_{\min}$:

$$
|\lambda\rangle|0\rangle\longmapsto|\lambda\rangle\left(\sqrt{1-c^2/\lambda^2}|0\rangle+\frac c\lambda|1\rangle\right).
$$

[Uncomputation](#uncomputation) of the eigenvalue register followed by conditioning on flag one multiplies each input [eigenvector](linear-operator-theory.md#eigenvector) amplitude by $c/\lambda$. If $|b\rangle$ is normalized, the success probability is $c^2\|A^{-1}|b\rangle\|^2$. Choosing $c=\lambda_{\max}/\kappa$ from a valid [condition number](linear-algebra.md#condition-number) bound gives success probability at least $1/\kappa^2$.

### Cost of exact phase estimation on a dyadic spectrum

↑ **Parent:** [HHL algorithm](#hhl-algorithm)

If the [eigenvalues](linear-operator-theory.md#eigenvalue) of $A$ are $\ell/2^n$ with $0\leq\ell<2^n$, [exact quantum phase estimation](#exact-quantum-phase-estimation) on $U=e^{2\pi iA}$ uses $n$ controlled powers $U^{2^j}$. Their [Hamiltonian simulation](#hamiltonian-simulation) times reach $2\pi2^{n-1}$. Counting each supplied controlled power as one oracle query is valid in that oracle model, but does not prove a [polynomial time](computer-science.md#polynomial-time) implementation from generic sparse-matrix access. In the ordinary [HHL algorithm](#hhl-algorithm), one instead chooses finite precision appropriate to the output error and the [condition number](linear-algebra.md#condition-number), or exploits additional structure giving efficient access to the needed powers.

## Density matrix

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Density_matrix)

A finite-dimensional density operator is Hermitian, positive semidefinite, and has trace one. In dimension $N$ it has $N^2-1$ real parameters. Schrödinger evolution is

$$
\rho_S(t)=U(t)\rho_HU(t)^\dagger
$$

when $\rho_H$ denotes the time-independent Heisenberg-picture state.

### Quantum state population

↑ **Parent:** [Density matrix](#density-matrix)

For a chosen normalized level state $|k\rangle$, its population is the [probability](probability-theory.md#probability) $\langle k|\rho|k\rangle=\operatorname{Tr}(|k\rangle\langle k|\rho)$ of finding the system in that state. In an orthonormal level basis these diagonal entries are nonnegative and sum to one. Off-diagonal [quantum coherence](#quantum-coherence-in-a-specified-basis) contains information absent from the population vector, so matching all level populations need not prepare a specified coherent superposition.

### Quantum coherence in a specified basis

↑ **Parent:** [Density matrix](#density-matrix)

For a chosen [orthonormal basis](linear-algebra.md#orthonormal-basis), the off-diagonal entries of a [density operator](#density-matrix) encode quantum coherence between distinct basis states. A diagonal density operator is an incoherent mixture in that basis. This property is basis-dependent: diagonalizing the operator does not imply that it lacked coherence in the measurement or energy basis of interest. Relative phases affect these entries, while a global wavefunction phase cancels from the density operator. Dephasing damps the entries and can spoil [stimulated Raman adiabatic passage](control-theory.md#stimulated-raman-adiabatic-passage) by removing the ground-state interference that maintains the dark state.

### Two-qubit Werner state

↑ **Parent:** [Density matrix](#density-matrix)

This collective-unitary-invariant two-qubit state has singlet weight $p$ and equal weights on the three triplet [Bell states](bell-state.md). With $P_s$ the [spin singlet state](bell-state.md#spin-singlet-state) projector, its [partial transpose](quantum-information-theory.md#partial-transpose) has eigenvalues $(1-2p)/2$ once and $(1+2p)/6$ three times. It is entangled exactly when $p>1/2$. At $p=1/2$, it is the equally weighted mixture of six antiparallel product states along the three Pauli axes. In the interval $1/4\leq p\leq1/2$, convex mixing of this boundary state with $I/4$ explicitly proves separability. The weight $p$ here is the singlet probability, not the alternative coefficient multiplying a pure singlet in a white-noise mixture.

#### Single-copy Werner filtering normalization bound

↑ **Parent:** [Two-qubit Werner state](#two-qubit-werner-state)

Write $W_F=(I\otimes I-w\sum_j\sigma_j\otimes\sigma_j)/4$, with $w=(4F-1)/3\in(1/3,1]$. For positive matrices $X=A^\dagger A=a_0I+a\cdot\sigma$ and $Y=B^\dagger B=b_0I+b\cdot\sigma$, the success probability is $p=a_0b_0-w a\cdot b$. It is at least $a_0b_0-|a||b|\geq\sqrt{(a_0^2-|a|^2)(b_0^2-|b|^2)}=|\det A\det B|$. Squaring the middle comparison leaves $(a_0|b|-b_0|a|)^2\geq0$.

##### Single-copy Werner filtering cannot increase concurrence

↑ **Parent:** [Single-copy Werner filtering normalization bound](#single-copy-werner-filtering-normalization-bound)

Combine the [single-copy Werner filtering normalization bound](#single-copy-werner-filtering-normalization-bound) with [concurrence scaling under invertible local filters](bell-state.md#concurrence-scaling-under-invertible-local-filters). Every complete classical record of [local operations and classical communication](bell-state.md#local-operations-and-classical-communication) has a product filter $A\otimes B$; singular branches are separable. Thus every retained branch has [concurrence](bell-state.md#concurrence) at most that of the input. Coarse-graining successful records preserves the bound by convexity. Since [concurrence of a two-qubit Werner state](#concurrence-of-a-two-qubit-werner-state) increases strictly with $F$, no successful single-copy protocol can output a Werner state with larger $F$. Several input copies permit collective distillation and are outside this statement.

#### Concurrence of a two-qubit Werner state

↑ **Parent:** [Two-qubit Werner state](#two-qubit-werner-state)

For any normalized pure two-[qubit](quantum-mechanics.md#qubit) vector, its squared overlap with a [maximally entangled state](#maximally-entangled-state) is at most $(1+C)/2$: in a [Schmidt decomposition](von-neumann-entropy.md#schmidt-decomposition) the overlap is bounded by $(\sqrt\lambda+\sqrt{1-\lambda})/\sqrt2$. Averaging gives $C(W_F)\geq2F-1$. Equality follows from the six-state ensemble $\sqrt F\,|\Psi_-\rangle\pm\sqrt{1-F}\,|t_j\rangle$, with equal weights, where $t_1=\Psi_+$, $t_2=\Phi_-$ and $t_3=i\Phi_+$. The coherences cancel and each coefficient determinant gives pure concurrence $2F-1$.

#### Bell twirling followed by triplet symmetrization

↑ **Parent:** [Two-qubit Werner state](#two-qubit-werner-state)

Average the four correlated local Pauli operations to remove coherences in the [Bell states](bell-state.md) basis. A one-party Pauli operation can permute the largest of the four resulting weights into the singlet sector; that weight is at least $1/4$. Correlated common local unitaries then permute the three triplet projectors, while [collective-unitary covariance of the two-qubit singlet](bell-state.md#collective-unitary-covariance-of-the-two-qubit-singlet) keeps the singlet projector unchanged. Averaging all six permutations makes the triplet weights equal, producing a [two-qubit Werner state](#two-qubit-werner-state). Shared randomness or [local operations and classical communication](bell-state.md#local-operations-and-classical-communication) coordinates these local operations. Common unitaries alone cannot increase an initially small singlet weight, because that weight is invariant under them.

### Extreme points of the density-operator state space

↑ **Parent:** [Density matrix](#density-matrix)

The [density operators](#density-matrix) on a finite-dimensional [Hilbert space](hilbert-space.md) form a convex set. Its [extreme points](mathematical-optimization.md#extreme-point) are exactly the rank-one projectors, hence exactly the [pure states](#pure-state). To prove this, suppose $|\psi\rangle\langle\psi|=\sum_i a_i\rho_i$ with $a_i>0$ and $\rho_i$ [positive semidefinite](linear-algebra.md#positive-semidefinite-matrix). For $w\perp\psi$, $0=\sum_i a_i\langle w|\rho_i|w\rangle$ is a sum of nonnegative numbers, so every term vanishes. Diagonalizing $\rho_i$ shows that $\langle w|\rho_i|w\rangle=0$ implies $\rho_iw=0$. Thus each $\rho_i$ is supported on the line spanned by $\psi$, and its unit [trace](linear-algebra.md#matrix-trace) forces $\rho_i=|\psi\rangle\langle\psi|$.

Conversely, a [density operator](#density-matrix) of [rank](linear-algebra.md#rank-one-quadratic-form) at least two has a [spectral decomposition](linear-operator-theory.md#spectral-decomposition) with at least two positive [eigenvalues](linear-operator-theory.md#eigenvalue). If $\lambda$ is one of them, $0<\lambda<1$ and $\rho=\lambda|e\rangle\langle e|+(1-\lambda)\sigma$, where $\sigma$ is the normalized remainder. These are distinct [density operators](#density-matrix), proving that $\rho$ is not an [extreme point](mathematical-optimization.md#extreme-point).

### Unitary orbit of a density operator

↑ **Parent:** [Density matrix](#density-matrix)

The unitary orbit consists exactly of [density operators](#density-matrix) with the same spectrum. If distinct eigenvalues have multiplicities $n_j$, its stabilizer is $\prod_jU(n_j)$ and its real dimension is $N^2-\sum_jn_j^2$. A reachable compact group with [Lie algebra](lie-algebra.md) $\mathfrak g$ is transitive on this orbit exactly when $\dim\mathfrak g-\dim(\mathfrak g\cap\{X:[X,\rho]=0\})$ equals the orbit dimension. Global phases act trivially by conjugation.

### Quantum state ensemble

↑ **Parent:** [Density matrix](#density-matrix)

A quantum state ensemble specifies a random preparation: normalized [pure states](#pure-state) $|\psi_i\rangle$ are selected with [probabilities](probability-theory.md#probability) $p_i\geq0$, $\sum_i p_i=1$. Without an accessible preparation label, its measurement statistics are those of the [density operator](#density-matrix) $\rho=\sum_i p_i|\psi_i\rangle\langle\psi_i|$. Indeed every [POVM](quantum-measurement.md#positive-operator-valued-measure) effect $E$ has probability $\sum_i p_i\langle\psi_i|E|\psi_i\rangle=\operatorname{Tr}(E\rho)$. Different ensembles can therefore have identical operational statistics: equal mixtures of computational-basis qubits or Hadamard-basis qubits both have density operator $I/2$. The ensemble decomposition contains information about the preparation, not additional information accessible from the system alone.

#### Convex roof extension

↑ **Parent:** [Quantum state ensemble](#quantum-state-ensemble)

A convex roof extension extends a function $\mu$ on [pure states](#pure-state) to arbitrary [density operators](#density-matrix) by minimizing its ensemble average over all [pure state](#pure-state) decompositions. It agrees with $\mu$ on [pure states](#pure-state): every positive-weight state in a decomposition of a rank-one [density operator](#density-matrix) has the same one-dimensional support. Concatenating nearly minimizing ensembles proves that $F$ is a [convex function](real-analysis.md#convex-function). Moreover, every [convex function](real-analysis.md#convex-function) that is no larger than $\mu$ on [pure states](#pure-state) is no larger than $F$, by applying convexity to each decomposition. Infima need not be attained; an arbitrarily small additive error suffices when $F$ is finite.

##### Monotonicity of a convex roof under a quantum instrument

↑ **Parent:** [Convex roof extension](#convex-roof-extension)

If a [convex roof extension](#convex-roof-extension) is non-increasing on average for every pure input to a [quantum instrument](quantum-measurement.md#quantum-instrument), then it is non-increasing on average for mixed inputs too. For an input ensemble $\{p_j,\pi_j\}$, let $q_{k|j}$ and $\sigma_{jk}$ be its conditional outcome probabilities and states. Linearity of each unnormalized outcome map gives $P_k\rho_k=\sum_jp_jq_{k|j}\sigma_{jk}$. Convexity gives $\sum_kP_kF(\rho_k)\leq\sum_{j,k}p_jq_{k|j}F(\sigma_{jk})\leq\sum_jp_j\mu(\pi_j)$. Taking the [infimum](real-analysis.md#infimum) over input ensembles proves the result, even when conditional outputs of pure inputs are mixed, provided the averages are well defined.

### Pauli correlation tensor

↑ **Parent:** [Density matrix](#density-matrix)

For a two-qubit [density operator](#density-matrix), the real three-by-three [matrix](vector-space.md#matrix) $T$ encodes the spin-product [expectation values](quantum-mechanics.md#expectation-value): unit measurement axes $\mathbf a,\mathbf b$ have $E(\mathbf a,\mathbf b)=\mathbf a^TT\mathbf b$. The tensor does not include local Bloch-vector data and alone need not specify the complete [density operator](#density-matrix). The [CHSH optimum from the correlation tensor](#chsh-optimum-from-the-correlation-tensor) depends on the two largest [eigenvalues](linear-operator-theory.md#eigenvalue) of $T^TT$.

### Maximally mixed state

↑ **Parent:** [Density matrix](#density-matrix)

The maximally mixed [density operator](#density-matrix) on an $N$-dimensional [Hilbert space](hilbert-space.md) assigns equal weights to every vector of any [orthonormal basis](linear-algebra.md#orthonormal-basis). It is invariant under every [unitary operator](vector-space.md#unitary-operator). Its purity is $\operatorname{Tr}(\rho_*^2)=1/N$, the minimum possible because the nonnegative [eigenvalues](linear-operator-theory.md#eigenvalue) sum to one and obey the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality). For $N>1$ it is a [mixed state](#mixed-state); for $N=1$ it is the sole pure state. A rank-$k$ projector has probability $k/N$ in this state.

#### Obstruction to uniform probability lowering by a unitary

↑ **Parent:** [Maximally mixed state](#maximally-mixed-state)

Let $P$ be a rank-$k$ projector with $0<k<N$. No [unitary operator](vector-space.md#unitary-operator) can map every pure state whose $P$ probability equals $k/N$ to a state with the same fixed smaller probability. Average $\sqrt{k/N}|g\rangle\pm\sqrt{1-k/N}|b\rangle$ over good and bad basis vectors and both signs. The average [density operator](#density-matrix) is the [maximally mixed state](#maximally-mixed-state), so every unitary preserves its average $P$ probability. This contradicts a strictly smaller probability for all states in the ensemble. A preparation tailored to one known starting state is a different resource and is used in [exact amplitude amplification](#exact-amplitude-amplification).

### Mixed state

↑ **Parent:** [Density matrix](#density-matrix)

A mixed state is a [density operator](#density-matrix) that is not a rank-one projector. In finite dimension it is characterized by $\operatorname{Tr}(\rho^2)<1$.

### Von Neumann equation

↑ **Parent:** [Density matrix](#density-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Von_Neumann_equation)

The density operator of a closed quantum system obeys

$$
i\hbar\dot\rho=[H,\rho].
$$

### Purification of a density operator

↑ **Parent:** [Density matrix](#density-matrix)

A purification of a density operator $\rho_A$ is a pure state $|\Psi\rangle_{AE}$ on a larger system such that $\operatorname{Tr}_E|\Psi\rangle\langle\Psi|=\rho_A$. A [spectral decomposition](linear-operator-theory.md#spectral-decomposition) $\rho_A=\sum_jp_j|j\rangle\langle j|$ gives the canonical construction $|\Psi\rangle=\sum_j\sqrt{p_j}|j\rangle_A|j\rangle_E$.

#### Purity decouples a subsystem from its purification

↑ **Parent:** [Purification of a density operator](#purification-of-a-density-operator)

If subsystem $S$ has [pure state](#pure-state) $|u\rangle\langle u|$ in a normalized joint pure vector $|\Omega\rangle_{SE}$, then $|\Omega\rangle_{SE}=|u\rangle_S\otimes|e\rangle_E$. Indeed, for an [orthonormal basis](linear-algebra.md#orthonormal-basis) $\{v_j\}$ of $u^\perp$, each squared norm $\|(\langle v_j|\otimes I)|\Omega\rangle\|^2=\langle v_j|\rho_S|v_j\rangle$ is zero. Therefore the joint vector has no component outside $\mathbb Cu\otimes\mathcal H_E$. In particular, if Alice and Bob share a known pure [entangled state](bell-state.md#entangled-state), an adversary holding a purifying system has no correlations with it. This does not make every pure bipartite state useful for key distribution: a pure [product state](bell-state.md#product-state) has no shared random correlations.

#### Flagged purification of a quantum ensemble

↑ **Parent:** [Purification of a density operator](#purification-of-a-density-operator)

For $\rho=\sum_xp_x\rho_x$, choose component purifications $|u_x\rangle_{AR}$ and an orthonormal flag register. The vector $|U\rangle=\sum_x\sqrt{p_x}|u_x\rangle|x\rangle$ is normalized and reduces to $\rho$ after tracing out $R$ and the flag. Orthogonal labels remove the cross terms. This construction turns mixture identities into pure-state overlap arguments and proves [joint concavity of quantum fidelity](quantum-information-theory.md#joint-concavity-of-quantum-fidelity).

#### Unitary freedom of purification

↑ **Parent:** [Purification of a density operator](#purification-of-a-density-operator)

Any two purifications of the same density operator on sufficiently large reference spaces differ by an isometry on the reference system, and by a unitary when the reference spaces have the same dimension.

<h4 id="hughston-jozsa-wootters-theorem">Hughston–Jozsa–Wootters theorem</h4>

↑ **Parent:** [Purification of a density operator](#purification-of-a-density-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hughston–Jozsa–Wootters_theorem)

The Hughston--Jozsa--Wootters theorem says that two pure-state ensembles represent the same density operator exactly when their subnormalized state vectors are related by an isometry, or by a unitary after padding the shorter ensemble with zero vectors.

##### Isometry parametrization of a density-matrix ensemble

↑ **Parent:** [Hughston–Jozsa–Wootters theorem](#hughston-jozsa-wootters-theorem)

For the nonzero spectral decomposition $\rho=\sum_{a=1}^r\lambda_a|e_a\rangle\langle e_a|$, every pure-state [quantum state ensemble](#quantum-state-ensemble) of $\rho$ is specified by the displayed column [linear isometry](hilbert-space.md#linear-isometry-of-hilbert-spaces). To prove this, write $w_j=\sqrt{p_j}\phi_j$. Positivity forces each $w_j$ into the support of $\rho$, and the coefficients $U_{ja}=\langle e_a|w_j\rangle/\sqrt{\lambda_a}$ have orthonormal columns because $\sum_j|w_j\rangle\langle w_j|=\rho$. Conversely this column identity reconstructs $\rho$; the squared vector norms are the [probabilities](probability-theory.md#probability) and sum to one. Complete the columns to unitary bases after adding zero ensemble vectors to obtain the usual unitary-mixing formulation.

<h4 id="uhlmann-s-theorem">Uhlmann's theorem</h4>

↑ **Parent:** [Purification of a density operator](#purification-of-a-density-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Uhlmann's_theorem)

Uhlmann's theorem states that the fidelity of two density operators is the maximum absolute overlap between their purifications on a common reference space.

### Trace distance

↑ **Parent:** [Density matrix](#density-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Trace_distance)

The trace distance between [density operators](#density-matrix) is

$$
D(\rho,\sigma)=\frac12\lVert\rho-\sigma\rVert_1.
$$

Every [quantum channel](quantum-information-theory.md#quantum-channel), including the [partial trace](#partial-trace), contracts trace distance.

#### Trace-distance contraction under quantum channels

↑ **Parent:** [Trace distance](#trace-distance)

By the [variational characterization of trace distance](#variational-characterization-of-trace-distance), maximize $\operatorname{Tr}[P\mathcal E(\rho-\sigma)]$ over $0\leq P\leq I$. The adjoint of a [quantum channel](quantum-information-theory.md#quantum-channel) is positive and unital, so $0\leq\mathcal E^*(P)\leq I$. Moving the channel onto $P$ therefore restricts, rather than enlarges, the effects available in the input variational problem. This proves the displayed bound for every pair of [density operators](#density-matrix).

#### Trace distance for qubit dephasing

↑ **Parent:** [Trace distance](#trace-distance)

For the pure [qubit](quantum-mechanics.md#qubit) $\alpha|0\rangle+\beta|1\rangle$, subtracting the output of [dephasing channel](quantum-information-theory.md#dephasing-channel) leaves a Hermitian matrix with zero diagonal and off-diagonal modulus $|\alpha\beta|\,|1-c|$. Its two [eigenvalues](linear-operator-theory.md#eigenvalue) are that number and its negative, giving the displayed [trace distance](#trace-distance). For real $c=1-2p$, this is $2p|\alpha\beta|$.

#### Pure-target upper bound on trace distance

↑ **Parent:** [Trace distance](#trace-distance)

For two normalized [pure states](#pure-state), the difference of their projectors has two [eigenvalues](linear-operator-theory.md#eigenvalue) $\pm\sqrt{1-|\langle u|v\rangle|^2}$, giving that [trace distance](#trace-distance). Write a mixed [density operator](#density-matrix) as $\rho=\sum_jq_j|u_j\rangle\langle u_j|$. Convexity of the [trace norm](functional-analysis.md#trace-norm) and weighted [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) give $D(\rho,|v\rangle\langle v|)\leq\sum_jq_j\sqrt{1-|\langle u_j|v\rangle|^2}\leq\sqrt{1-\langle v|\rho|v\rangle}$. Thus a small [probability](probability-theory.md#probability) of failing the pure-state projector test forces trace-distance proximity, including for correlated multipartite outputs.

#### Spectral-parts formula for trace distance

↑ **Parent:** [Trace distance](#trace-distance)

For the Hermitian difference $X=\rho-\sigma$, define its [positive part of a Hermitian operator](hilbert-space.md#positive-part-of-a-hermitian-operator) $Q=X_+$ and [negative part of a Hermitian operator](hilbert-space.md#negative-part-of-a-hermitian-operator) $R=X_-$. Their supports are orthogonal and $|X|=Q+R$. Equal traces give $\operatorname{Tr}Q=\operatorname{Tr}R$, so the [trace distance](#trace-distance) is both $\tfrac12(\operatorname{Tr}Q+\operatorname{Tr}R)$ and $\operatorname{Tr}Q$. This explains why the positive spectral projector attains the [variational characterization of trace distance](#variational-characterization-of-trace-distance).

#### Pure-target lower bound on trace distance

↑ **Parent:** [Trace distance](#trace-distance)

For a [density operator](#density-matrix) $\rho$ and [pure state](#pure-state) $P=|\psi\rangle\langle\psi|$, the [diagonal absolute-sum bound for the trace norm](functional-analysis.md#diagonal-absolute-sum-bound-for-the-trace-norm) in a basis containing $|\psi\rangle$ gives $D(\rho,P)\geq1-\langle\psi|\rho|\psi\rangle=1-F(\rho,P)^2$. The [quantum fidelity](quantum-information-theory.md#fidelity-of-quantum-states) is unsquared. Block-diagonal states with respect to the target and its complement attain equality.

#### Variational characterization of trace distance

↑ **Parent:** [Trace distance](#trace-distance)

For density operators $\rho,\sigma$,

$$
D(\rho,\sigma)=\max_{0\leq P\leq I}\operatorname{Tr}[P(\rho-\sigma)].
$$

The maximum is attained by the projector onto the positive spectral subspace of $\rho-\sigma$.

##### Trace-distance-preserving binary measurement

↑ **Parent:** [Variational characterization of trace distance](#variational-characterization-of-trace-distance)

For two [density operators](#density-matrix) $\rho,\sigma$, let $P_+$ project onto the positive spectral subspace of $\rho-\sigma$. The binary [POVM](quantum-measurement.md#positive-operator-valued-measure) $\{P_+,I-P_+\}$ has output probability difference $(D,-D)$, where $D=D(\rho,\sigma)$. Its [measurement channel](quantum-information-theory.md#measurement-channel) therefore preserves this pair's [trace distance](#trace-distance) exactly. The optimizing [measurement in quantum mechanics](quantum-measurement.md) depends on the pair; a single fixed measurement need not preserve every pair's distance.

### Von Neumann entropy

↑ **Parent:** [Density matrix](#density-matrix)

[This section is present in another page, follow this link to view it.](von-neumann-entropy.md)

### Purity of a density operator

↑ **Parent:** [Density matrix](#density-matrix)

The purity of a density operator is $\operatorname{Tr}(\rho^2)$. It equals one exactly for a pure state; in finite dimension $d$ it lies between $1/d$ and $1$.

### Reduced density operator of a weakly coupled oscillator pair

↑ **Parent:** [Density matrix](#density-matrix)

If a weak interaction changes $|0,0\rangle$ to a normalized state proportional to $|0,0\rangle-g|1,1\rangle$, tracing out either oscillator gives eigenvalues $1/(1+g^2)$ and $g^2/(1+g^2)$.

### Bloch vector

↑ **Parent:** [Density matrix](#density-matrix)

Every qubit state has the unique form

$$
\rho=\frac12(I+r_x\sigma_x+r_y\sigma_y+r_z\sigma_z),
\qquad |r|\leq1.
$$

It is pure exactly when $|r|=1$, and  
$r_i=2\langle S_i\rangle/\hbar$.

Unit-length Bloch vectors form the [Bloch sphere](#bloch-sphere); mixed-state vectors occupy the ball’s interior.

#### Bloch ball

↑ **Parent:** [Bloch vector](#bloch-vector)

The qubit [density operators](#density-matrix) $\rho=(I+\mathbf s\cdot\boldsymbol\sigma)/2$ correspond exactly to the closed unit ball: their [eigenvalues](linear-operator-theory.md#eigenvalue) are $(1\pm|\mathbf s|)/2$, so positivity is equivalent to $|\mathbf s|\leq1$. The boundary is the [Bloch sphere](#bloch-sphere) of pure states, and the centre is $I/2$. A [depolarizing channel](quantum-information-theory.md#quantum-depolarizing-channel) scales this ball isotropically, possibly with a sign reversal in the larger completely positive parameter interval.

##### Antipodal eigenprojectors of a qubit density matrix

↑ **Parent:** [Bloch ball](#bloch-ball)

For a qubit [density matrix](#density-matrix) $\rho=(I+n\cdot\sigma)/2$ with nonzero [Bloch vector](#bloch-vector), $\widehat n=n/\|n\|$ and the multiplication rule for the [Pauli matrices](algebra.md#pauli-matrices) give these orthogonal rank-one [spectral projectors](hilbert-space.md#spectral-projector), with eigenvalues $(1\pm\|n\|)/2$. Their [Bloch vectors](#bloch-vector) are opposite unit vectors $\pm\widehat n$. At $n=0$ the state is maximally mixed and the direction is undefined; any orthonormal eigenbasis gives an antipodal pair, but no pair is distinguished by the state.

#### Generalized Bloch representation

↑ **Parent:** [Bloch vector](#bloch-vector)

Choose a [Hilbert-Schmidt inner product](compact-operator.md#hilbert-schmidt-inner-product) orthonormal Hermitian operator basis with final element $I/\sqrt N$. A [density operator](#density-matrix) has real coefficients $r_k=\operatorname{Tr}(\sigma_k\rho)$ and fixed final coefficient $1/\sqrt N$. The remaining coefficients form its generalized [Bloch vector](#bloch-vector). Positivity restricts these real vectors to a compact convex body; for $N>2$ this body is not the entire Euclidean ball allowed by a purity bound.

##### Hamiltonian rotations of Bloch vectors

↑ **Parent:** [Generalized Bloch representation](#generalized-bloch-representation)

In a Hilbert-Schmidt orthonormal operator basis, the generator $-i[H,\cdot]$ is represented on the traceless Hermitian subspace by a real [skew-symmetric matrix](linear-algebra.md#skew-symmetric-matrix). Its propagator is therefore in the [special orthogonal group](linear-algebra.md#special-orthogonal-group) and preserves the [purity of a density operator](#purity-of-a-density-operator). For $N>2$, these rotations form the adjoint image of the accessible unitary group, generally a proper subgroup of the full Euclidean rotation group; preservation of the full [spectrum](linear-operator-theory.md#spectrum-functional-analysis) of the [density operator](#density-matrix) imposes further constraints.

##### Purity bound for generalized Bloch vectors

↑ **Parent:** [Generalized Bloch representation](#generalized-bloch-representation)

For a Hilbert-Schmidt orthonormal traceless Hermitian basis, the [Generalized Bloch representation](#generalized-bloch-representation) gives the displayed identity by orthogonality. Nonnegative [eigenvalues](linear-operator-theory.md#eigenvalue) of a [density operator](#density-matrix) sum to one, so their squared sum is at most one, with equality precisely for a rank-one projector. For $N>2$, the radius bound alone does not guarantee positivity: $(2/N)I-P$ for a rank-one projector $P$ has [trace](linear-algebra.md#matrix-trace) one and squared norm one, but one negative [eigenvalue](linear-operator-theory.md#eigenvalue).

##### Affine Bloch equation

↑ **Parent:** [Generalized Bloch representation](#generalized-bloch-representation)

A time-independent [Lindblad equation](quantum-information-theory.md#lindblad-equation) becomes an affine linear equation for the [Generalized Bloch representation](#generalized-bloch-representation). If $\mathcal L(I)=\sum_d[V_d,V_d^\dagger]$, then $A_{mn}=\operatorname{Tr}(\sigma_m\mathcal L(\sigma_n))$ and $c_m=\operatorname{Tr}(\sigma_m\mathcal L(I))/N$ for traceless basis indices. The offset vanishes exactly when the dynamics are unital. Equilibria solve $As_*=-c$, and deviations evolve as $s(t)-s_*=e^{At}(s(0)-s_*)$.

###### Transverse relaxation

↑ **Parent:** [Affine Bloch equation](#affine-bloch-equation)

Decay of the off-diagonal coherence of a two-level [density operator](#density-matrix). Population relaxation contributes half its total rate; additional [dephasing](quantum-information-theory.md#dephasing-channel) contributes $\gamma_\phi\geq0$ in the usual completely positive two-level model. Thus transverse relaxation should not automatically be identified with pure dephasing alone.

###### Population relaxation

↑ **Parent:** [Affine Bloch equation](#affine-bloch-equation)

For a two-level [density operator](#density-matrix), rates $\gamma_{12}$ from level one to two and $\gamma_{21}$ in the reverse direction give $\dot p_1=-\gamma_{12}p_1+\gamma_{21}p_2$. Their sum sets the longitudinal population relaxation rate, and their ratio fixes the stationary population imbalance. If both rates vanish, populations are conserved.

###### Steady states of an affine Bloch equation

↑ **Parent:** [Affine Bloch equation](#affine-bloch-equation)

An arbitrary real affine equation has [steady states](dynamical-systems.md#steady-state) exactly when $\operatorname{rank}A=\operatorname{rank}[A\mid-c]$. Its solution set is $s_*+\ker A$. For a finite-dimensional time-independent [Lindblad equation](quantum-information-theory.md#lindblad-equation), physical stationary states always exist by time averaging trajectories. If $A$ is invertible the [steady state](dynamical-systems.md#steady-state) is unique. Conversely, a nonzero traceless Hermitian stationary direction can be decomposed into the difference of two equally weighted [density operators](#density-matrix); time averaging their trajectories yields two distinct stationary [density operators](#density-matrix). Thus singularity of the physical Bloch matrix also obstructs physical uniqueness.

#### Bloch sphere

↑ **Parent:** [Bloch vector](#bloch-vector)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bloch_sphere)

The [Bloch sphere](#bloch-sphere) is the unit sphere of [Bloch vectors](#bloch-vector), corresponding to pure [qubit](quantum-mechanics.md#qubit) states through $\rho=(I+\mathbf r\cdot\boldsymbol\sigma)/2$. A local unitary change of qubit basis induces a rotation of this sphere, with its common phase physically irrelevant. Mixed states occupy the interior of the unit ball.

##### Pure-qubit overlap identity

↑ **Parent:** [Bloch sphere](#bloch-sphere)

Write each pure [density matrix](#density-matrix) as $(I+r\cdot\sigma)/2$. The [trace](linear-algebra.md#matrix-trace) identities of the [Pauli matrices](algebra.md#pauli-matrices), $\operatorname{Tr}\sigma_i=0$ and $\operatorname{Tr}(\sigma_i\sigma_j)=2\delta_{ij}$, make the [trace](linear-algebra.md#matrix-trace) of their product equal to the displayed overlap. Antipodal unit vectors represent [orthogonal](linear-algebra.md#orthogonal-vectors) states; vectors at right angles correspond to squared overlap one half. For mixed states the same [trace](linear-algebra.md#matrix-trace) formula gives Hilbert–Schmidt overlap, not in general quantum fidelity.

##### Uniform pure-qubit average

↑ **Parent:** [Bloch sphere](#bloch-sphere)

The rotation-invariant average of pure [qubit](quantum-mechanics.md#qubit) states is uniform area measure on the [Bloch sphere](#bloch-sphere), induced by [Haar measure](measure-theory.md#haar-measure) on unitary transformations. For a uniformly distributed unit [Bloch vector](#bloch-vector) $r$, rotational symmetry gives $\mathbb Er_i=0$ and $\mathbb Er_ir_j=\delta_{ij}/3$. Uniform polar angle without the factor $\sin\theta$ is a different distribution.

#### Informationally complete three-observable qubit tomography

↑ **Parent:** [Bloch vector](#bloch-vector)

Three Hermitian expectation values determine an arbitrary qubit state exactly when the traceless parts of the three observables span the three-dimensional space generated by the Pauli matrices. Mere linear independence as Hermitian matrices is insufficient: $I,\sigma_x,\sigma_z$ are independent but cannot detect the sign or magnitude of the Bloch $y$ component.

## Quantum no-signalling

↑ **Parent:** [Quantum theory](quantum-theory.md)

An uncommunicated local trace-preserving operation cannot change the other subsystem's reduced state.

### Remote preparation in conjugate bases

↑ **Parent:** [Quantum no-signalling](#quantum-no-signalling)

A [projective measurement](quantum-measurement.md#projective-measurement) on one half of a [Bell state](bell-state.md) prepares the complex-conjugate basis on the other half, conditional on the outcome. Measuring Alice in the columns of $U^*$ prepares Bob in the columns of $U$. Ignoring the equally likely outcomes leaves Bob's [reduced density matrix](bell-state.md#reduced-density-matrix) equal to $I/2$ in either basis.

#### Perfect two-basis discrimination would allow superluminal signalling

↑ **Parent:** [Remote preparation in conjugate bases](#remote-preparation-in-conjugate-bases)

Suppose two orthonormal [qubit](quantum-mechanics.md#qubit) bases have disjoint physical rays. Alice chooses which conjugate basis to measure on her half of a [Bell state](bell-state.md). A device that perfectly labels Bob's individual member of either basis would reveal Alice's choice without her outcome being communicated. Spacelike operation would therefore violate relativistic causality, even though ordinary [projective measurements](quantum-measurement.md#projective-measurement) see the same [reduced density matrix](bell-state.md#reduced-density-matrix) $I/2$.

##### Exact pure-state overlap readout would allow superluminal signalling

↑ **Parent:** [Perfect two-basis discrimination would allow superluminal signalling](#perfect-two-basis-discrimination-would-allow-superluminal-signalling)

With a fixed reference $|0\rangle$, exact overlap readout on Bob's remotely prepared state distinguishes the computational basis from the diagonal basis in one use, by the displayed disjoint squared-overlap sets. This would reveal Alice's spacelike basis choice. The argument rules out even deterministic exact overlap magnitude, avoiding the additional unphysical global-phase dependence of a raw complex inner product.

### Relativistic causality constraint on an ideal nonlocal measurement

↑ **Parent:** [Quantum no-signalling](#quantum-no-signalling)

The nonselective channel of a hypothetical spacelike nonlocal [measurement in quantum mechanics](quantum-measurement.md) must not allow a distant input change to alter local output statistics. For a rank-one measurement in the rotated even and odd two-qubit bases with angle $\theta$, Alice's output satisfies

$$
\langle Z_A\rangle_{\rm out}=\cos^2(2\theta)\langle Z_A\rangle_{\rm in}+\sin2\theta\cos2\theta\langle X_AX_B\rangle_{\rm in}.
$$

Bob can change the last correlation using only his local [Pauli Z gate](#pauli-z-gate) while Alice keeps the input $|+\rangle$. The resulting signal excludes $0<\theta<\pi/4$. Degenerate observables that do not distinguish this basis are not covered by the rank-one argument. Locally recording a jointly encoded result, which is decoded later by [local operations and classical communication](bell-state.md#local-operations-and-classical-communication), is compatible with [quantum no-signalling](#quantum-no-signalling).

#### Controlled-basis measurement causality obstruction

↑ **Parent:** [Relativistic causality constraint on an ideal nonlocal measurement](#relativistic-causality-constraint-on-an-ideal-nonlocal-measurement)

A rank-one [projective measurement](quantum-measurement.md#projective-measurement) whose Bob basis is computational when Alice is zero and rotated by $\theta$ when Alice is one can signal. Bob starts in zero. Alice zero leaves Bob zero; Alice one dephases Bob in the rotated basis, giving the displayed nonzero flip probability for $0<\theta\leq\pi/4$. This violates [quantum no-signalling](#quantum-no-signalling). The conclusion applies to a measurement distinguishing the four product-basis states, rather than a degenerate observable that does not resolve them.

#### Singlet-triplet measurement causality obstruction

↑ **Parent:** [Relativistic causality constraint on an ideal nonlocal measurement](#relativistic-causality-constraint-on-an-ideal-nonlocal-measurement)

The binary [Lüders rule](quantum-measurement.md#luders-rule) measurement of singlet versus triplet preserves the entire triplet subspace, but its nonselective channel permits signalling. Starting with $|00\rangle$, Bob retains $|0\rangle$. If Alice instead applies a local [Pauli X gate](#pauli-x-gate), the input is $|10\rangle$ and the channel outputs the equal mixture of $|\Psi^+\rangle$ and $|\Psi^-\rangle$; Bob has [reduced density matrix](bell-state.md#reduced-density-matrix) $I/2$. Thus no spacelike local implementation can realize this channel. A [Bell-state nondemolition measurement](bell-state.md#bell-state-nondemolition-measurement) has a finer triplet readout and a different nonselective channel, so this obstruction does not exclude it.

## Quantum cloning

↑ **Parent:** [Quantum theory](quantum-theory.md)

A cloning operation for a family of pure states would map

$$
|\psi\rangle|0\rangle\longmapsto|\psi\rangle|\psi\rangle
$$

for every state in that family. A single physical operation cannot clone every unknown quantum state.

The [no-cloning theorem](#no-cloning-theorem) forbids a universal unknown-state cloning operation, while orthogonal families can be cloned.

### Cloning failure bound from trace-distance contraction

↑ **Parent:** [Quantum cloning](#quantum-cloning)

For two [pure states](#pure-state) of overlap $0<c<1$, a [quantum channel](quantum-information-theory.md#quantum-channel) attempts to turn $M$ copies into $N>M$ copies. Let $e_i$ be the failure probability of the all-copies projector test on input $i$. The [pure-state trace distance and fidelity identity](quantum-information-theory.md#pure-state-trace-distance-and-fidelity-identity), [trace-distance contraction under quantum channels](#trace-distance-contraction-under-quantum-channels), [pure-target upper bound on trace distance](#pure-target-upper-bound-on-trace-distance) and [triangle inequality](topological-analysis.md#triangle-inequality) give the displayed strictly positive gap $\Delta$. Hence $\max_i e_i\geq\Delta^2/4$, and for positive priors $\pi_0+\pi_1=1$, weighted [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $\pi_0e_0+\pi_1e_1\geq\pi_0\pi_1\Delta^2$. No positive state-by-state bound holds: preparing one candidate perfectly makes its own conditional failure probability zero.

### Copy-number trace-distance obstruction

↑ **Parent:** [Quantum cloning](#quantum-cloning)

Let distinct nonorthogonal [pure states](#pure-state) have overlap magnitude $0<c<1$, and let one [quantum channel](quantum-information-theory.md#quantum-channel) take $n$ identical inputs to $m$ outputs. Let $\epsilon_u,\epsilon_v$ be the respective [probabilities](probability-theory.md#probability) that a test for the ideal $m$-copy [pure state](#pure-state) fails. [Trace distance](#trace-distance) contraction, its triangle inequality and the [pure-target upper bound on trace distance](#pure-target-upper-bound-on-trace-distance) give $\sqrt{1-c^{2m}}\leq\sqrt{\epsilon_u}+\sqrt{1-c^{2n}}+\sqrt{\epsilon_v}$. Squaring with the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives the displayed strategy-independent positive bound. It establishes both a worst-case bound and an equal-prior average bound. Averaging rotated pairs establishes a positive Haar-average bound for unknown qubit inputs, without assuming independent clone errors.

### No-cloning theorem

↑ **Parent:** [Quantum cloning](#quantum-cloning)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/No-cloning_theorem)

No deterministic quantum operation can make two perfect copies of every unknown [pure state](#pure-state). For a proposed [unitary operator](vector-space.md#unitary-operator) acting with a fixed blank and environment, preservation of inner products gives $c=c^2 e$, where $c$ is the input overlap and $|e|\leq1$ is the overlap of final environment states. Nonorthogonal distinct states have $0<|c|<1$, contradicting this equality. The [no-cloning theorem for two pure states](#no-cloning-theorem-for-two-pure-states) is its elementary two-state form.

### No-cloning theorem for two pure states

↑ **Parent:** [Quantum cloning](#quantum-cloning)

No [unitary operator](vector-space.md#unitary-operator) $U$ can satisfy

$$
U|c_j\rangle|0\rangle=|c_j\rangle|c_j\rangle,
\qquad j=0,1,
$$

for two distinct nonorthogonal pure states. Taking the inner product of these two equations would require

$$
\langle c_0|c_1\rangle
=\langle c_0|c_1\rangle^2,
$$

which is impossible when $0<|\langle c_0|c_1\rangle|<1$.

### Clone-assisted asymptotic state discrimination

↑ **Parent:** [Quantum cloning](#quantum-cloning)

If a device produces arbitrarily many copies of either of two distinct pure-state rays, their $N$-copy overlap is

$$
|\langle\phi|\psi\rangle|^N\longrightarrow0.
$$

The Helstrom measurement on the copies therefore distinguishes the alternatives with success probability tending to one.

### Perfect discrimination implies cloning for a known state family

↑ **Parent:** [Quantum cloning](#quantum-cloning)

If a device perfectly identifies which member of a known finite state family was supplied, its classical output can control state-preparation unitaries that prepare any requested number of fresh copies. The discrimination may destroy the supplied system.

## Environment-assisted two-state pure-state transformation

↑ **Parent:** [Quantum theory](quantum-theory.md)

There are a unitary $U$ and normalized environment states $|e_i\rangle$ satisfying

$$
U|\phi_i\rangle|0\rangle=|\psi_i\rangle|e_i\rangle,
\qquad i=0,1,
$$

exactly when

$$
|\langle\phi_0|\phi_1\rangle|
\leq|\langle\psi_0|\psi_1\rangle|.
$$

Necessity follows from preservation of inner products. For sufficiency, choose $\langle e_0|e_1\rangle$ to make the input and output inner products equal; equal two-vector Gram matrices define an isometry that extends to a unitary.

## Helstrom-Holevo bound

↑ **Parent:** [Quantum theory](quantum-theory.md)

Equiprobable pure states of overlap magnitude $c$ have optimal discrimination probability $\frac12(1+\sqrt{1-c^2})$.

### Helstrom measurement for two pure states

↑ **Parent:** [Helstrom-Holevo bound](#helstrom-holevo-bound)

For $\rho_j=|\alpha_j\rangle\langle\alpha_j|$, projecting onto the positive and negative eigenspaces of $\rho_0-\rho_1$ attains

$$
P_s^{\rm opt}=\frac12+\frac14\|\rho_0-\rho_1\|_1
=\frac12\left(1+\sqrt{1-|\langle\alpha_0|\alpha_1\rangle|^2}\right).
$$

#### Helstrom measurement for the zero and plus states

↑ **Parent:** [Helstrom measurement for two pure states](#helstrom-measurement-for-two-pure-states)

For equiprobable states $|0\rangle$ and

$$
|+\rangle=\frac{|0\rangle+|1\rangle}{\sqrt2},
$$

the orthonormal measurement basis at angle $\beta=-\pi/8$ to the computational basis attains

$$
P_s=\frac12\left(1+\frac1{\sqrt2}\right).
$$

### Perfect distinguishability of pure states

↑ **Parent:** [Helstrom-Holevo bound](#helstrom-holevo-bound)

Two pure states can be distinguished with certainty in one measurement exactly when their inner product is zero.

### Unambiguous quantum state discrimination

↑ **Parent:** [Helstrom-Holevo bound](#helstrom-holevo-bound)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Unambiguous_quantum_state_discrimination)

Unambiguous quantum state discrimination allows an inconclusive outcome but forbids a wrong conclusive identification. Two distinct pure states admit such a measurement, whereas two full-rank density operators on the same support do not.

#### Reciprocal-state construction of unambiguous discrimination

↑ **Parent:** [Unambiguous quantum state discrimination](#unambiguous-quantum-state-discrimination)

For normalized linearly independent [pure states](#pure-state), their [Gram matrix](linear-algebra.md#gram-matrix) $G_{ij}=\langle\psi_i|\psi_j\rangle$ is positive definite. The displayed reciprocal vectors satisfy $\langle\chi_i|\psi_j\rangle=\delta_{ij}$. The operator $R=\sum_i|\chi_i\rangle\langle\chi_i|$ has nonzero [eigenvalues](linear-operator-theory.md#eigenvalue) equal to those of $G^{-1}$: use the polar factorization of the matrix whose columns are $\psi_i$. Choosing $0<\epsilon\leq\lambda_{\min}(G)$ gives the [POVM](quantum-measurement.md#positive-operator-valued-measure) effects $E_i$ and $E_?=I-\epsilon R$. Each conclusive outcome has [probability](probability-theory.md#probability) $\epsilon$ on its own state and zero on every other input. The inconclusive effect preserves positivity, so the construction is a physical [measurement in quantum mechanics](quantum-measurement.md).

## Unitary gate discrimination

↑ **Parent:** [Quantum theory](quantum-theory.md)

To distinguish two gates in one use without an ancilla, choose an input $|\psi\rangle$ and discriminate the output states $U_1|\psi\rangle$ and $U_2|\psi\rangle$.

### Single-use perfect discrimination of two unitary gates

↑ **Parent:** [Unitary gate discrimination](#unitary-gate-discrimination)

Perfect discrimination is possible exactly when some unit vector satisfies

$$
\langle\psi|U_2^\dagger U_1|\psi\rangle=0.
$$

### Numerical range

↑ **Parent:** [Unitary gate discrimination](#unitary-gate-discrimination)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Numerical_range)

The numerical range of an operator $A$ is

$$
N(A)=\{\langle\psi|A|\psi\rangle:\|\psi\|=1\}.
$$

#### Numerical range of a normal matrix

↑ **Parent:** [Numerical range](#numerical-range)

For a finite-dimensional normal matrix, the numerical range is the convex hull of its eigenvalues.

### Unit-circle spectrum of a unitary operator

↑ **Parent:** [Unitary gate discrimination](#unitary-gate-discrimination)

If $Uv=\lambda v$ and $U$ is unitary, norm preservation gives $|\lambda|=1$.

### Spectral arc length of a unitary operator

↑ **Parent:** [Unitary gate discrimination](#unitary-gate-discrimination)

The spectral arc length $\theta(U)$ is the length of the shortest closed unit-circle arc containing every eigenvalue of $U$.

#### Spectral arc length of a phase gate

↑ **Parent:** [Spectral arc length of a unitary operator](#spectral-arc-length-of-a-unitary-operator)

For $U_\gamma=\operatorname{diag}(1,e^{i\gamma})$ with $0\leq\gamma<2\pi$,

$$
\theta(U_\gamma)=\min\{\gamma,2\pi-\gamma\}.
$$

#### Origin in the convex hull of unit-circle points

↑ **Parent:** [Spectral arc length of a unitary operator](#spectral-arc-length-of-a-unitary-operator)

The convex hull of finitely many unit-circle points contains zero exactly when the points do not lie in any open semicircle, equivalently when their shortest containing arc has length at least $\pi$.

##### Spectral-arc criterion for perfect unitary discrimination

↑ **Parent:** [Origin in the convex hull of unit-circle points](#origin-in-the-convex-hull-of-unit-circle-points)

Two unitary gates are perfectly distinguishable in one use exactly when

$$
\theta(U_2^\dagger U_1)\geq\pi.
$$

## Robertson uncertainty principle

↑ **Parent:** [Quantum theory](quantum-theory.md)

$\Delta A\,\Delta B\ge\frac12|\langle[A,B]\rangle|$.

### Heisenberg uncertainty relation

↑ **Parent:** [Robertson uncertainty principle](#robertson-uncertainty-principle)

For a normalized state with the required position and momentum moments, $[x,p]=i\hbar$ and the [Robertson uncertainty principle](#robertson-uncertainty-principle) give $\Delta x\,\Delta p\geq\hbar/2$. In a [quantum harmonic oscillator](quantum-mechanics.md#quantum-harmonic-oscillator), the [arithmetic-geometric mean inequality](mathematical-optimization.md#arithmetic-geometric-mean-inequality) then bounds the variance contribution to energy below by $\hbar\omega/2$.

### Quadratic-norm proof of the Heisenberg uncertainty relation

↑ **Parent:** [Robertson uncertainty principle](#robertson-uncertainty-principle)

For a state with zero position and momentum means, positivity of $\lVert(p-isx)\psi\rVert^2$ for every real $s$ gives

$$
(\Delta p)^2+s^2(\Delta x)^2-s\hbar\geq0.
$$

The discriminant is nonpositive, hence $\Delta x\,\Delta p\geq\hbar/2$.

### Equality case of the Heisenberg uncertainty relation

↑ **Parent:** [Robertson uncertainty principle](#robertson-uncertainty-principle)

Equality requires the centred vectors $x'\psi$ and $p'\psi$ to be imaginary scalar multiples. Thus, for some $s>0$,

$$
(p-p_0)\psi=is(x-x_0)\psi.
$$

In the position representation this is a first-order differential equation, whose normalizable solutions are

$$
\psi(x)=C\exp\left(\frac{ip_0x}{\hbar}-\frac{s(x-x_0)^2}{2\hbar}\right).
$$

Hence the states saturating the position-momentum uncertainty relation are Gaussian wave packets, up to translation, modulation, and phase.

## Gaussian eigenstate for a quadratic potential

↑ **Parent:** [Quantum theory](quantum-theory.md)

For $U(x)=kx^2$ and $k>0$, the ansatz $\psi=Ce^{-\alpha x^2}$ solves the stationary Schrödinger equation when

$$
\alpha=\frac1\hbar\sqrt{\frac{mk}{2}},
\qquad
E=\hbar\sqrt{\frac{k}{2m}},
\qquad
C=\left(\frac{2\alpha}{\pi}\right)^{1/4}.
$$

It has $\Delta x=1/(2\sqrt\alpha)$ and $\Delta p=\hbar\sqrt\alpha$, so it saturates the Heisenberg bound.

## Coherent state

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coherent_state)

$|\alpha\rangle=D(\alpha)|0\rangle$ is normalized, satisfies $A|\alpha\rangle=\alpha|\alpha\rangle$, and evolves to a phase times $|\alpha e^{-i\omega t}\rangle$.

### Coherent-state resolution of identity

↑ **Parent:** [Coherent state](#coherent-state)

For an [unnormalized bosonic coherent state](#unnormalized-bosonic-coherent-state), the measure is $d^2\psi/\pi$ over the complex plane. Gaussian moments $\int d^2\psi\,e^{-|\psi|^2}\psi^n\bar\psi^m/\pi=n!\delta_{nm}$ recover the identity in the [Fock state](quantum-field-theory.md#fock-state) basis. For a [fermionic coherent state](#fermionic-coherent-state), use independent [Grassmann variables](linear-algebra.md#grassmann-variable) and an ordered [Berezin integral](quantum-mechanics.md#berezin-integral) with $\int d\bar\psi\,d\psi\,\bar\psi\psi=-1$. The coefficient of $-\bar\psi\psi$ in the weighted projector is the identity. Products of these one-mode measures give the finite-mode result.

### Unnormalized bosonic coherent state

↑ **Parent:** [Coherent state](#coherent-state)

An [unnormalized bosonic coherent state](#unnormalized-bosonic-coherent-state) is $|\psi\rangle=e^{\psi a^\dagger}|0\rangle$ for a complex label $\psi$. The [canonical commutation relation](quantum-mechanics.md#canonical-commutation-relation) gives $a|\psi\rangle=\psi|\psi\rangle$ and overlap $\langle\psi|\psi'\rangle=e^{\bar\psi\psi'}$. Multiplication by $e^{-|\psi|^2/2}$ produces a normalized [coherent state](#coherent-state). The unnormalized form makes the [coherent-state resolution of identity](#coherent-state-resolution-of-identity) and thermal time slicing particularly simple.

### Fermionic coherent state

↑ **Parent:** [Coherent state](#coherent-state)

For a single [fermionic annihilation operator](relativistic-quantum-field.md#fermionic-annihilation-operator) $a$ and an independent odd [Grassmann variable](linear-algebra.md#grassmann-variable) $\theta$, a [fermionic coherent state](#fermionic-coherent-state) is an extended state obeying $a|\theta\rangle=\theta|\theta\rangle$. With $\{a,\theta\}=0$ one may take $|\theta\rangle=\exp(-\theta a^\dagger)|0\rangle$. Its overlap is exponential in the Grassmann labels. A resolution of identity with a [Berezin integral](quantum-mechanics.md#berezin-integral) gives the time-slice construction of a [fermionic path integral](quantum-mechanics.md#fermionic-path-integral). These formal eigenstates use Grassmann-valued coefficients.

#### Fermionic coherent-state trace

↑ **Parent:** [Fermionic coherent state](#fermionic-coherent-state)

The ordinary trace of an even fermionic operator requires $-\psi$ in the bra of its [fermionic coherent state](#fermionic-coherent-state) kernel. In one mode the diagonal matrix elements give $\langle-\psi|A|\psi\rangle=A_{00}-\bar\psi\psi A_{11}$, whose Gaussian [Berezin integral](quantum-mechanics.md#berezin-integral) is $A_{00}+A_{11}$. An untwisted bra gives $A_{00}-A_{11}$, the [supertrace](quantum-mechanics.md#supertrace). This distinction produces the antiperiodic [coherent-state thermal boundary conditions](quantum-field-theory.md#coherent-state-thermal-boundary-conditions).

## Born approximation

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Born_approximation)

The Born approximation replaces the unknown total field inside a scattering integral by the known incident field, thereby retaining only single scattering. In nonrelativistic quantum mechanics, first-order Lippmann-Schwinger iteration gives

$$
f(\mathbf k',\mathbf k)=-\frac{m}{2\pi\hbar^2}\widetilde V(\mathbf k'-\mathbf k).
$$

## Toffoli gate

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Toffoli_gate)

The Toffoli, or controlled-controlled-NOT, gate maps $|x_1x_2y\rangle$ to $|x_1x_2,y\mathbin\oplus x_1x_2\rangle$.

## Modular-addition quantum oracle

↑ **Parent:** [Quantum theory](quantum-theory.md)

For $h:\mathbb Z_N\to\mathbb Z_M$, its modular-addition oracle is the [unitary operator](vector-space.md#unitary-operator)

$$
U_h|x,y\rangle=|x,y+h(x)\bmod M\rangle.
$$

For each fixed $x$, [addition](arithmetic.md#addition) by $h(x)$ permutes the answer register's [computational basis](#computational-basis). This preserves [inner products](linear-algebra.md#inner-product), even when $h$ is not injective.

### Modular-oracle inversion by negation

↑ **Parent:** [Modular-addition quantum oracle](#modular-addition-quantum-oracle)

Let $S_M|y\rangle=|-y\bmod M\rangle$. The [modular-addition quantum oracle](#modular-addition-quantum-oracle) obeys

$$
U_h^{-1}=(I\otimes S_M)U_h(I\otimes S_M).
$$

The three steps replace $y$ by $-y$, then $-y+h(x)$, then $y-h(x)$. Thus a query to the inverse costs one forward query and two known [unitary operators](vector-space.md#unitary-operator). The negation operator is a [permutation matrix](vector-space.md#permutation-matrix) with $S_M^2=I$.

## Boolean quantum oracle

↑ **Parent:** [Quantum theory](quantum-theory.md)

For a Boolean function $f$, its standard oracle acts by

$$
U_f|x\rangle|y\rangle=|x\rangle|y\mathbin\oplus f(x)\rangle.
$$

### Phase kickback

↑ **Parent:** [Boolean quantum oracle](#boolean-quantum-oracle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Phase_kickback)

Because $X| -\rangle=-| -\rangle$, a Boolean oracle with answer qubit $| -\rangle$ acts as

$$
U_f|x\rangle| -\rangle=(-1)^{f(x)}|x\rangle| -\rangle.
$$

#### Quadratic Boolean phase cancellation

↑ **Parent:** [Phase kickback](#phase-kickback)

For a two-variable [Boolean quantum oracle](#boolean-quantum-oracle), [quantum phase kickback](#phase-kickback) produces the phase $(-1)^{axy+bx+cy+d}$ on $|xy\rangle$. If the quadratic coefficient $a$ is known, apply the [Controlled-Z gate](#controlled-z-gate) to the power $a$: its phase $(-1)^{axy}$ cancels the quadratic term. A [Walsh-Hadamard transform](#walsh-hadamard-transform) then maps the remaining phase state to $(-1)^d|bc\rangle$. The constant term is only a [global phase](quantum-mechanics.md#global-phase), and both linear coefficients are read in one [quantum measurement in the computational basis](#quantum-measurement-in-the-computational-basis).

#### Bernstein-Vazirani phase kickback

↑ **Parent:** [Phase kickback](#phase-kickback)

For $f(x)=a\mathbin\cdot x\mathbin\oplus b$, phase kickback followed by a Walsh-Hadamard transform maps the uniform phase state to

$$
(-1)^b|a\rangle.
$$

The hidden linear string $a$ is therefore recovered with certainty.

##### Qutrit linear-function identification

↑ **Parent:** [Bernstein-Vazirani phase kickback](#bernstein-vazirani-phase-kickback)

A [modular-addition quantum oracle](#modular-addition-quantum-oracle) for a linear [function](function.md) over the three-element [finite field](algebra.md#finite-field) reveals its two coefficients in one query. Prepare the answer [qutrit](quantum-mechanics.md#qutrit) in $\operatorname{QFT}_3|2\rangle$, whose unit shift [eigenvalue](linear-operator-theory.md#eigenvalue) is $e^{2\pi i/3}$. [Quantum phase kickback](#phase-kickback) produces a product of Fourier states labelled by the coefficients; inverse [quantum Fourier transforms](#quantum-fourier-transform) read both coefficients exactly.

##### Bernstein-Vazirani decoding controlled by a quantum register

↑ **Parent:** [Bernstein-Vazirani phase kickback](#bernstein-vazirani-phase-kickback)

For a [Boolean quantum oracle](#boolean-quantum-oracle) whose function is $g(x,y)=a_y\cdot x$, place its target in $|{-}\rangle$. Conjugating the oracle by a [Walsh-Hadamard transform](#walsh-hadamard-transform) on the $x$ register translates that register by $a_y$. This is [Bernstein-Vazirani phase kickback](#bernstein-vazirani-phase-kickback) without measuring its output, so the index $y$ may remain in an arbitrary quantum superposition. A second application undoes the translation. A phase evaluation between the two calls therefore transfers a hidden-label-dependent phase to the index register while [uncomputation](#uncomputation) returns the decoding register to zero.

#### Marked-state phase oracle

↑ **Parent:** [Phase kickback](#phase-kickback)

If $f$ marks only $x_0$, phase kickback realizes $I_{x_0}=I-2|x_0\rangle\langle x_0|$ on the search register.

##### Marked-state phase oracle from a single faulty identity-oracle query

↑ **Parent:** [Marked-state phase oracle](#marked-state-phase-oracle)

Suppose $U_f$ agrees with the reversible identity-function oracle except at $x_0$, where its answer differs by a fixed one-bit string $a$. Composing $U_f$ with the known identity oracle and preparing the affected answer qubit in $|-\rangle$ kicks back the phase $-1$ exactly on $|x_0\rangle$, using one query to $U_f$.

### Compute-phase-uncompute construction

↑ **Parent:** [Boolean quantum oracle](#boolean-quantum-oracle)

Starting the answer qubit in $|0\rangle$, the sequence

$$
U_f,\qquad Z,\qquad U_f
$$

maps $|x\rangle|0\rangle$ to $(-1)^{f(x)}|x\rangle|0\rangle$. It realizes a phase oracle with two standard-oracle queries while returning the answer register to its initial state.

### Uncomputation

↑ **Parent:** [Boolean quantum oracle](#boolean-quantum-oracle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Uncomputation)

Uncomputation applies the inverse of a reversible computation after its result has been used. It returns workspace registers to a fixed state, removing unwanted entanglement without erasing the information irreversibly.

## Quantum circuit

↑ **Parent:** [Quantum theory](quantum-theory.md)

[This section is present in another page, follow this link to view it.](quantum-circuit.md)

## Lieb-Robinson bound

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lieb-Robinson_bound)

A Lieb-Robinson bound limits the commutator of initially separated local observables by $\lVert[A(t),B]\rVert\leq C\lVert A\rVert\lVert B\rVert e^{-\mu(d-v|t|)}$. It gives local lattice dynamics an effective causal cone with Lieb-Robinson velocity $v$.

### Full-evolution comparison for truncated dynamics

↑ **Parent:** [Lieb-Robinson bound](#lieb-robinson-bound)

A Duhamel comparison can bound truncation error using [commutators](lie-algebra.md#commutator) evolved under the full Hamiltonian. This avoids assuming that a black-box [Lieb-Robinson bound](#lieb-robinson-bound) for $H$ also holds for every truncation. Polynomial shell weights and exponential distance suppression make the sum over omitted shells convergent. Comparing two truncations through the full evolution bounds their difference.

### Lieb-Robinson interaction-chain expansion

↑ **Parent:** [Lieb-Robinson bound](#lieb-robinson-bound)

Iterating the integral [commutator](lie-algebra.md#commutator) inequality gives ordered interaction chains with factors $(2|t|)^n/n!$. A per-site interaction weight at most $se^{-\mu}$ bounds each successive chain extension by $ks e^{-\mu}$. No chain shorter than the [interaction distance](#interaction-distance) connects separated supports. Reversing chains supplies the smaller support prefactor, producing the [Lieb-Robinson bound](#lieb-robinson-bound). Overlapping supports require retaining the equal-time [commutator](lie-algebra.md#commutator) term.

### Interaction distance

↑ **Parent:** [Lieb-Robinson bound](#lieb-robinson-bound)

The [interaction distance](#interaction-distance) between disjoint supports can count the minimum number of interacting hyperedges in a chain connecting them. Overlapping supports have distance zero in the usual support convention. Distances between interaction terms can instead assign shell zero only to the central term and positive shells to distinct terms. The convention must be specified when using a truncated neighborhood Hamiltonian: ordinary zero support distance includes distinct overlapping terms.

### Lieb-Robinson localization by Haar twirling

↑ **Parent:** [Lieb-Robinson bound](#lieb-robinson-bound)

Apply [Haar twirling conditional expectation](#haar-twirling-conditional-expectation) to the complement of a neighbourhood around the initial operator support. A [Lieb-Robinson bound](#lieb-robinson-bound) on commutators with arbitrary complement-supported unitaries then bounds the approximation error without summing over sites. For a bound proportional to $e^{-\mu d}(e^{2kst}-1)$, choosing $v=4ks/\mu$ gives an error at most $\mu vt\,|X|\|A_X\|e^{-\mu l/2}$ outside radius $vt+l$.

### Finite-depth local quantum circuit

↑ **Parent:** [Lieb-Robinson bound](#lieb-robinson-bound)

A depth-$D$ circuit of gates with range at most $r$ expands the support of a local observable by at most $rD$. States connected by a depth bounded independently of system size are regarded as belonging to the same short-range-entangled phase when no required symmetry is violated.

#### Backward light cone of a local quantum circuit

↑ **Parent:** [Finite-depth local quantum circuit](#finite-depth-local-quantum-circuit)

The backward light cone of an output observable is the set of input degrees of freedom that can influence it. In a depth-$D$ circuit with gate range at most $r$, it lies within distance $rD$ of the observable's output support.

#### GHZ-state circuit-depth lower bound

↑ **Parent:** [Finite-depth local quantum circuit](#finite-depth-local-quantum-circuit)

The GHZ state has nonzero connected correlations between arbitrarily distant sites. A local circuit starting from a product state can create such a correlation only when the two backward light cones overlap, giving depth at least proportional to the system's linear size.

<h2 id="grover-s-algorithm">Grover's algorithm</h2>

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Grover's_algorithm)

Grover search rotates a uniform state toward a marked subspace and finds one of $M$ marked entries using order $\sqrt{N/M}$ oracle calls.

### First half-success time in Grover search

↑ **Parent:** [Grover's algorithm](#grover-s-algorithm)

For both oracle phases equal to $\pi$, the good/bad matrix is $\begin{pmatrix}\cos2\chi&\sin2\chi\\-\sin2\chi&\cos2\chi\end{pmatrix}$. Acting $r$ times on the initial vector $(\sin\chi,\cos\chi)$ yields success $\sin^2((2r+1)\chi)$. For $0<\chi\le\pi/4$, the first crossing of one half is the displayed integer, since the rounded angle stays between $\pi/4$ and $3\pi/4$. With $\sin^2\chi=m/N\ll1$ this is asymptotic to $(\pi/8)\sqrt{N/m}$. Iterating indefinitely is incorrect: the success oscillates after its first maximum.

### Continuous-time quantum search

↑ **Parent:** [Grover's algorithm](#grover-s-algorithm)

Take normalized states with real positive overlap $a\in(0,1)$. The eigenvectors proportional to $|s\rangle\pm|w\rangle$ have energies $\Delta(1\pm a)$. With $\hbar=1$, their relative phase changes by $\pi$ after the displayed time, giving $e^{-iHt_*}|s\rangle=-ie^{-i\Delta t_*}|w\rangle$. For a uniform search state and one marked basis vector in dimension $D$, $a=D^{-1/2}$, so the time is proportional to $\sqrt D$. Implementing the marked projector assumes access to a search oracle; the formula does not supply oracle information for free.

### Grover search with a nonzero reflection label

↑ **Parent:** [Grover's algorithm](#grover-s-algorithm)

Let $|s\rangle=H^{\otimes n}|0^n\rangle$, let $U_f$ be the [marked-state phase oracle](#marked-state-phase-oracle), and replace reflection about $|0^n\rangle$ by reflection about a known [computational basis](#computational-basis) vector $|y\rangle$. Define $T_y=\bigotimes_{j=0}^{n-1}Z_j^{y_j}$, so $T_y|x\rangle=(-1)^{x\cdot y}|x\rangle$ and $H^{\otimes n}|y\rangle=T_y|s\rangle$. The resulting Grover iterate obeys

$$
G_y=(2|s_y\rangle\langle s_y|-I)U_f=T_yGT_y,\qquad |s_y\rangle=T_y|s\rangle,
$$

because the two diagonal operators $T_y,U_f$ commute. Thus the good and bad uniform vectors are replaced by their signed vectors $T_y|g\rangle,T_y|b\rangle$, with exactly the same [Grover rotation angle](#grover-rotation-angle). Initializing in $H^{\otimes n}|y\rangle$ gives $G_y^r|s_y\rangle=T_yG^r|s\rangle$. Computational-basis measurement probabilities are unchanged because $T_y$ only multiplies amplitudes by signs.

### Verified Grover promise test

↑ **Parent:** [Grover's algorithm](#grover-s-algorithm)

Under the promise of either no marked entry or one marked entry in an $N$-element [Boolean quantum oracle](#boolean-quantum-oracle) search space, run the [Grover search algorithm](#grover-s-algorithm) for the displayed number of iterations, measure a candidate, and make one additional oracle query to check it. Since $|(2k+1)\theta-\pi/2|\leq\theta$, the marked-entry success probability is at least $\cos^2\theta=1-1/N$. For $N\geq4$ this is at least $3/4$. If no entry is marked the verification never accepts, so there is no false positive. The query count is $k+1=O(\sqrt N)$ because $\theta\geq1/\sqrt N$. Measuring a candidate without verification would not determine whether a marked entry exists.

### Marked density under a permutation

↑ **Parent:** [Grover's algorithm](#grover-s-algorithm)

For a [permutation](combinatorics.md#permutation) $f$ of an $N$-element set and a known marked output subset of size $K$, exactly $K$ inputs have marked outputs. The [uniform quantum superposition](#uniform-quantum-superposition) thus has good probability $K/N$, independent of which permutation the oracle represents. This allows a known-angle [amplitude amplification](#amplitude-amplification) schedule without counting unknown preimages.

#### Permutation-preimage quantum search

↑ **Parent:** [Marked density under a permutation](#marked-density-under-a-permutation)

To find an input of a [permutation](combinatorics.md#permutation) whose output lies in a known $K$-element subset, compute the output, apply its [marked-state phase oracle](#marked-state-phase-oracle), and use [uncomputation](#uncomputation). A [modular-addition quantum oracle](#modular-addition-quantum-oracle) costs two forward queries per marked reflection, because [modular-oracle inversion by negation](#modular-oracle-inversion-by-negation) supplies its inverse. [Amplitude amplification](#amplitude-amplification) then uses $O(\sqrt{N/K})$ queries for fixed success probability. Positive-square outputs have $K=\lfloor\sqrt{N-1}\rfloor$ and hence query cost $O(N^{1/4})$.

### Known-subset Grover search

↑ **Parent:** [Grover's algorithm](#grover-s-algorithm)

For a known finite set $B$, prepare the [uniform superposition state](quantum-circuit.md#uniform-superposition-state) $|s_B\rangle$ and implement its [reflection operator](#reflection-operator) $2|s_B\rangle\langle s_B|-I$. If exactly $k$ basis states in $B$ are marked, the same two-dimensional [Grover rotation angle](#grover-rotation-angle) argument uses $O(\sqrt{|B|/k})$ phase queries. Preparation and reflection are known operations with no calls to the unknown predicate. Their gate cost must be accounted for separately. The success guarantee requires $k>0$, and choosing the optimal iteration number uses a known $k$.

#### Clean subset superposition preparation

↑ **Parent:** [Known-subset Grover search](#known-subset-grover-search)

Suppose a known list of $2^m$ distinct $n$-bit strings $a_j$ is available and [computational basis](#computational-basis) transpositions on $n+m$ [qubits](quantum-mechanics.md#qubit) have polynomial-size implementations. Start with the [uniform superposition state](quantum-circuit.md#uniform-superposition-state) of index labels $j$, leaving the data zero. First swap $|0^n,j\rangle$ with $|a_j,j\rangle$ for each nonzero $a_j$. Next, for each $j\ne0$, swap $|a_j,j\rangle$ with $|a_j,0^m\rangle$. Distinct index labels separate the first-stage pairs, and distinct data strings separate the second-stage pairs. Thus no later transposition disturbs an earlier term. At most $2^{m+1}-1$ transpositions prepare the uniform data state and return the [quantum ancilla](quantum-information-theory.md#quantum-ancilla) to zero. For $m=O(\log n)$ the [quantum circuit](quantum-circuit.md) has polynomial size. This assumes the list is available; a membership predicate alone does not supply it.

### Grover diffusion operator

↑ **Parent:** [Grover's algorithm](#grover-s-algorithm)

For $|s\rangle=H^{\otimes n}|0^n\rangle$, the diffusion operator is $2|s\rangle\langle s|-I=-H^{\otimes n}I_0H^{\otimes n}$, where $I_0=I-2|0^n\rangle\langle0^n|$.

#### Inversion about the mean

↑ **Parent:** [Grover diffusion operator](#grover-diffusion-operator)

The diffusion operator sends every computational-basis amplitude $a_x$ to $2\overline a-a_x$, where $\overline a$ is their arithmetic mean.

### Grover rotation angle

↑ **Parent:** [Grover's algorithm](#grover-s-algorithm)

If $M$ of $N$ items are marked and $\sin\theta=\sqrt{M/N}$, each Grover iteration rotates the state by $2\theta$ in the marked--unmarked plane, so after $r$ iterations the marked amplitude is $\sin((2r+1)\theta)$.

#### First half-probability Grover iterate

↑ **Parent:** [Grover rotation angle](#grover-rotation-angle)

If the marked fraction is $p$ and $\theta=\arcsin\sqrt p$, the success probability after $n$ [Grover search algorithm](#grover-s-algorithm) iterations is $\sin^2((2n+1)\theta)$. For $0<p\leq1/2$, its first value at least $1/2$ occurs at

$$
n_{\min}=\left\lceil\frac{\pi}{8\theta}-\frac12\right\rceil.
$$

Before this integer the angle is below $\pi/4$, so success is below $1/2$. At this integer, the angle lies in $[\pi/4,\pi/4+2\theta)$, contained in $[\pi/4,3\pi/4)$, where squared sine is at least $1/2$. If $p\geq1/2$, no iteration is needed. For small $p$, $n_{\min}$ is asymptotic to $\pi/(8\sqrt p)$.

#### First successful Grover iterate

↑ **Parent:** [Grover rotation angle](#grover-rotation-angle)

For one marked element among $N\geq2$ candidates, set $\theta=\arcsin(N^{-1/2})$. The first nonnegative [Grover search algorithm](#grover-s-algorithm) iteration count attaining marked probability at least $\cos^2\theta$ is the displayed integer. Before the first success interval, the angle $(2k+1)\theta$ is below $\pi/2-\theta$; entering that interval requires $k\geq\pi/(4\theta)-1$. Rounding up gives an angle less than $\pi/2+\theta$, so it cannot skip the interval. Moreover $k_{\min}<\pi/(4\theta)<\pi\sqrt N/4$. For $N=1$, the known candidate is already the answer and no iteration is needed; the two-dimensional marked--unmarked plane degenerates.

#### Exact Grover search on four entries

↑ **Parent:** [Grover rotation angle](#grover-rotation-angle)

For $N=4$ and one marked item, $\theta=\pi/6$. One Grover iteration gives marked amplitude $\sin(3\theta)=1$, so measurement returns the target with certainty.

## Computational basis

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Computational_basis)

For $n$ qubits, the computational basis is the orthonormal basis $\{|x\rangle:x\in\{0,1\}^n\}$ labelled by bit strings.

### Quantum measurement in the computational basis

↑ **Parent:** [Computational basis](#computational-basis)

Measuring $\sum_xa_x|x\rangle$ in the computational basis returns $x$ with probability $|a_x|^2$ and leaves the measured register in $|x\rangle$.

#### Computational-basis state

↑ **Parent:** [Quantum measurement in the computational basis](#quantum-measurement-in-the-computational-basis)

A computational-basis state of $n$ qubits is $|x\rangle$ for a bit string $x\in\{0,1\}^n$.

## Deutsch-Jozsa algorithm

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Deutsch–Jozsa_algorithm)

The Deutsch-Jozsa algorithm uses phase kickback and interference to distinguish constant from perfectly balanced Boolean functions with one oracle call.

### Deutsch algorithm

↑ **Parent:** [Deutsch-Jozsa algorithm](#deutsch-jozsa-algorithm)

The one-input Deutsch algorithm determines whether a [Boolean function](combinatorics.md#boolean-function) is constant or balanced using one [Boolean quantum oracle](#boolean-quantum-oracle) call. Initialize the input [qubit](quantum-mechanics.md#qubit) in $|+\rangle$ and the answer [qubit](quantum-mechanics.md#qubit) in $|-\rangle$. [Quantum phase kickback](#phase-kickback) changes the input to $(-1)^{f(0)}(|0\rangle+(-1)^{f(0)\oplus f(1)}|1\rangle)/\sqrt2$. A [Hadamard gate](#hadamard-gate) and [computational-basis measurement](#quantum-measurement-in-the-computational-basis) therefore return the parity $f(0)\oplus f(1)$ with certainty.

#### Deutsch algorithm with pure dephasing

↑ **Parent:** [Deutsch algorithm](#deutsch-algorithm)

If the input [qubit](quantum-mechanics.md#qubit) of the [Deutsch algorithm](#deutsch-algorithm) acquires conditional environment states with overlap $\langle e_0|e_1\rangle=ve^{i\alpha}$ between its two [Hadamard gates](#hadamard-gate), its fixed zero-for-constant, one-for-balanced rule succeeds with probability $(1+v\cos\alpha)/2$. A known phase can be compensated before the last [Hadamard gate](#hadamard-gate), raising the success probability to $(1+v)/2$. An orthogonal pair of environment states gives $v=0$ and destroys all information in the input [qubit](quantum-mechanics.md#qubit) about the answer; unit overlap modulus preserves coherence up to a known phase.

### Opposite-pair elimination for exact quantum balance testing

↑ **Parent:** [Deutsch-Jozsa algorithm](#deutsch-jozsa-algorithm)

For an even-length Boolean string, one phase query followed by a known [unitary extension](hilbert-space.md#unitary-extension-of-a-finite-dimensional-isometry) can produce a zero-pair outcome with amplitude proportional to the zero-minus-one imbalance, or an index pair with amplitude proportional to the difference of their phase signs. A zero-pair observation certifies nonbalance. Every nonzero pair has opposite bits, so deleting it preserves the imbalance and allows recursion on two fewer indices. Ending with an empty list certifies balance. This [quantum circuit](quantum-circuit.md) is exact on all inputs and uses at most half the original length in queries, even without the constant-or-balanced promise.

### Deutsch-Jozsa test with an arbitrary uniform-state unitary

↑ **Parent:** [Deutsch-Jozsa algorithm](#deutsch-jozsa-algorithm)

If $F|0\rangle=N^{-1/2}\sum_i|i\rangle$, then applying a phase oracle followed by $F^{-1}$ gives amplitude

$$
\frac1N\sum_i(-1)^{f(i)}
$$

on $|0\rangle$. It has modulus one for a constant Boolean function and vanishes for a balanced one.

## Quantum Fourier transform

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_Fourier_transform)

The quantum Fourier transform maps $|k\rangle$ to $N^{-1/2}\sum_j e^{2\pi ijk/N}|j\rangle$.

### Dyadic quantum Fourier transform circuit

↑ **Parent:** [Quantum Fourier transform](#quantum-fourier-transform)

In most-significant-bit-first order, let $x=x_1\cdots x_n$ and $0.x_j\cdots x_n=\sum_{l=j}^n x_l2^{-(l-j+1)}$. On a [computational-basis state](#computational-basis-state), process wire $j$ with a [Hadamard gate](#hadamard-gate), then [controlled phase gates](#controlled-phase-gate) $R_{l-j+1}$ controlled by unprocessed wire $l$ for each $l>j$. Wire $j$ becomes $(|0\rangle+e^{2\pi i0.x_j\cdots x_n}|1\rangle)/\sqrt2$. Reversing the final wire order yields the positive-exponent [quantum Fourier transform](#quantum-fourier-transform). There are $n$ [Hadamard gates](#hadamard-gate) and $n(n-1)/2$ [controlled phase gates](#controlled-phase-gate). Physical reversal costs $\lfloor n/2\rfloor$ [swap operators](quantum-information-theory.md#swap-operator), each expressible as three [controlled-NOT gates](#controlled-not-gate), themselves implemented with [Hadamard gates](#hadamard-gate) and a [Controlled-Z gate](#controlled-z-gate). Thus the entire construction uses $O(n^2)$ gates from the specified family.

### Product decomposition of a Fourier phase state

↑ **Parent:** [Quantum Fourier transform](#quantum-fourier-transform)

Write the integer label in most-significant-bit-first order as $l=\sum_jb_j2^{n-j}$. The phase factors as $e^{i\phi l}=\prod_je^{i\phi b_j2^{n-j}}$, giving the displayed [product state](bell-state.md#product-state). For dyadic Fourier phases this explains why the Fourier basis states are unentangled even though a general [quantum Fourier transform](#quantum-fourier-transform) can create [entanglement](bell-state.md#entangled-state).

### Fourier sample

↑ **Parent:** [Quantum Fourier transform](#quantum-fourier-transform)

A Fourier sample is a [computational-basis measurement](#quantum-measurement-in-the-computational-basis) outcome after applying a [quantum Fourier transform](#quantum-fourier-transform) $F$ to a [quantum state](quantum-mechanics.md#quantum-state) $|\psi\rangle$. Its distribution is given by the squared Fourier amplitudes. For a uniform periodic coset of spacing $r\mid N$, samples are the multiples $sN/r$ with uniform $s\in\mathbb Z_r$. Samples need not individually reveal the whole period: a [greatest common divisor](number-theory.md#greatest-common-divisor) can remove factors from a single reduced denominator, motivating [two-sample exact period recovery](#two-sample-exact-period-recovery).

### Quantum Fourier transform over a finite abelian group

↑ **Parent:** [Quantum Fourier transform](#quantum-fourier-transform)

For a [finite abelian group](group.md#finite-abelian-group) $G$ with character group $\widehat G$, the quantum Fourier transform is

$$
|g\rangle\longmapsto\frac1{\sqrt{|G|}}\sum_{\chi\in\widehat G}\chi(g)|\chi\rangle,
$$

up to complex conjugation according to the transform convention.

### Square of the quantum Fourier transform

↑ **Parent:** [Quantum Fourier transform](#quantum-fourier-transform)

The [root-of-unity filter](algebra.md#root-of-unity-filter) gives

$$
\operatorname{QFT}_N^2|x\rangle=|-x\bmod N\rangle.
$$

Thus $\operatorname{QFT}_N^4=I$, while the square is an involution whose eigenvalues lie in $\{1,-1\}$.

### Quantum Fourier transform of a periodic coset state

↑ **Parent:** [Quantum Fourier transform](#quantum-fourier-transform)

Let $r$ divide $N$ and

$$
|\alpha\rangle=\frac1{\sqrt{N/r}}
\sum_{j=0}^{N/r-1}|x_0+jr\rangle.
$$

The geometric sum in the quantum Fourier transform vanishes unless $c$ is a multiple of $N/r$. Thus measurement after the transform returns the $r$ values

$$
c=0,\frac Nr,\ldots,(r-1)\frac Nr
$$

with equal probabilities $1/r$.

### Quantum period finding

↑ **Parent:** [Quantum Fourier transform](#quantum-fourier-transform)

For a function of period $r$ dividing $N$, prepare a uniform superposition of inputs, evaluate the function into a second register, and measure that register. The first register becomes a periodic coset state. Applying the [quantum Fourier transform](#quantum-fourier-transform) and measuring gives

$$
c=s\frac Nr,
\qquad 0\leq s<r.
$$

#### Exact period recovery from a Fourier sample

↑ **Parent:** [Quantum period finding](#quantum-period-finding)

For the exact sample $c=sN/r$, reducing

$$
\frac cN=\frac sr
$$

recovers denominator $r/\gcd(s,r)$. Thus one sample reveals the full period exactly when $s$ is coprime to $r$; otherwise it reveals only a proper divisor and the algorithm must obtain more information.

##### Two-sample exact period recovery

↑ **Parent:** [Exact period recovery from a Fourier sample](#exact-period-recovery-from-a-fourier-sample)

Suppose a function has least period $r\mid N$ and distinct values on distinct period cosets. Two independent [Fourier samples](#fourier-sample) have the form $c_j=s_jN/r$ with uniform $s_j\in\mathbb Z_r$. The displayed candidate is $r/\gcd(r,s_1,s_2)$, so exact recovery occurs when no prime divisor of $r$ divides both residues. The [Chinese remainder theorem](mathematics.md#chinese-remainder-theorem) gives probability $\prod_{\ell\mid r}(1-\ell^{-2})\ge1/\zeta(2)=6/\pi^2$, using the [Euler product](analytic-number-theory.md#euler-product). Unlike a single-sample coprimality probability, this bound is uniformly greater than one half. A candidate-period test makes successful recovery heralded when such a test is available.

##### Heralded exact quantum period finding when the period divides the register size

↑ **Parent:** [Exact period recovery from a Fourier sample](#exact-period-recovery-from-a-fourier-sample)

Suppose a function on $\mathbb Z_N$ has least period $r\mid N$ and is injective on each period. A Fourier sample $c=sN/r$ gives the candidate denominator $q=r/\gcd(s,r)$. If equality of function values can be tested efficiently, then $q$ is the full period exactly when $f(q)=f(0)$, so each successful run is certified. A sample succeeds with probability $\varphi(r)/r$, and an inverse-polylogarithmic lower bound for this ratio permits amplification to constant success probability with polynomially many repetitions.

###### Quantum Fourier sampling of powers of three modulo ten

↑ **Parent:** [Heralded exact quantum period finding when the period divides the register size](#heralded-exact-quantum-period-finding-when-the-period-divides-the-register-size)

The function $f(x)=3^x\bmod10$ on $\mathbb Z_{12}$ has period four. Measuring function value $3$ in its uniform input-output state leaves $(|1\rangle+|5\rangle+|9\rangle)/\sqrt3$. The quantum Fourier transform modulo twelve then returns each of $0,3,6,9$ with probability $1/4$.

### Hidden subgroup problem

↑ **Parent:** [Quantum Fourier transform](#quantum-fourier-transform)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hidden_subgroup_problem)

The hidden subgroup problem asks for a subgroup $H\leq G$ given an oracle $f:G\to X$ that is constant on each left coset of $H$ and takes different values on different cosets. Abelian instances are solved by preparing coset states and applying a group [quantum Fourier transform](#quantum-fourier-transform).

#### Discrete-logarithm Fourier sampling

↑ **Parent:** [Hidden subgroup problem](#hidden-subgroup-problem)

For a [generator of a group](group.md#generator-of-a-group) $g$ of order $M$ and $x=g^y$, the function $f(a,b)=g^ax^{-b}$ hides the [subgroup](group.md#subgroup) $\{(yb,b):b\in\mathbb Z_M\}$ of $\mathbb Z_M^2$. Each [fiber](function.md#fiber-of-a-function) is an affine [coset](group-theory.md#coset) $\{(yb+k,b):b\in\mathbb Z_M\}$. Measuring the function register gives its normalized [coset state](#coset-state). Applying the positive-exponent [quantum Fourier transform](#quantum-fourier-transform) to both input registers gives amplitude

$$
\frac{e^{2\pi ikc_1/M}}{M\sqrt M}\sum_{b=0}^{M-1}e^{2\pi ib(yc_1+c_2)/M}.
$$

The [finite geometric series](real-analysis.md#finite-geometric-series) vanishes off $c_2=-yc_1$ and equals $M$ on that line. Thus each allowed output pair has [probability](probability-theory.md#probability) $1/M$, independently of the coset offset. If $\gcd(c_1,M)=1$, a [modular inverse](number-theory.md#modular-multiplicative-inverse) recovers $y=-c_2c_1^{-1}$.

##### Linear congruence from a discrete-logarithm Fourier sample

↑ **Parent:** [Discrete-logarithm Fourier sampling](#discrete-logarithm-fourier-sampling)

Let $d=\gcd(c_1,M)$. A supported sample guarantees $d\mid c_2$. Dividing its [linear congruence](number-theory.md#linear-congruence) by $d$ gives an invertible coefficient modulo $M/d$ and a unique residue $y_0$ there. The $d$ compatible [discrete logarithms](coding-theory.md#discrete-logarithm-problem) modulo $M$ are $y_0+jM/d$ for $0\leq j<d$. Only $d=1$ determines the [discrete logarithm](coding-theory.md#discrete-logarithm-problem) from the sample alone; $(c_1,c_2)=(0,0)$ conveys no information for $M>1$.

#### Coset state

↑ **Parent:** [Hidden subgroup problem](#hidden-subgroup-problem)

For a finite group $G$, subgroup $H$, and $g\in G$, the coset state is the uniform superposition

$$
|gH\rangle=\frac1{\sqrt{|H|}}\sum_{h\in H}|gh\rangle.
$$

##### Periodic coset state

↑ **Parent:** [Coset state](#coset-state)

For $r\mid N$, a periodic coset state in the computational basis of $\mathbb Z_N$ is

$$
\frac1{\sqrt{N/r}}\sum_{j=0}^{N/r-1}|x_0+jr\rangle.
$$

It is the [coset state](#coset-state) of the subgroup $r\mathbb Z_N$ translated by $x_0$.

#### Group shift operator

↑ **Parent:** [Hidden subgroup problem](#hidden-subgroup-problem)

For a [finite abelian group](group.md#finite-abelian-group) $G$, $U(h)|g\rangle=|g+h\rangle$ defines the [regular representation](representation-theory.md#regular-representation) on the basis labelled by $G$. The [linear characters](representation-theory.md#linear-character) give the common [eigenbasis](linear-operator-theory.md#eigenbasis)

$$
|v_\chi\rangle=|G|^{-1/2}\sum_g\overline{\chi(g)}|g\rangle,
\qquad U(h)|v_\chi\rangle=\chi(h)|v_\chi\rangle.
$$

[Character orthogonality](representation-theory.md#character-orthogonality) proves orthonormality, and changing variables by the [translation in a group](group.md#translation-in-a-group) proves the eigenvalue formula.

#### Abelian hidden-subgroup Fourier sampling

↑ **Parent:** [Hidden subgroup problem](#hidden-subgroup-problem)

Measuring the [coset state](#coset-state) $|g_0+K\rangle$ in the [group shift operator](#group-shift-operator) [eigenbasis](linear-operator-theory.md#eigenbasis) samples uniformly from the [annihilator of a subgroup of a finite abelian group](group.md#annihilator-of-a-subgroup-of-a-finite-abelian-group) $K^\perp$. Indeed,

$$
\langle v_\chi|g_0+K\rangle
=\frac{\chi(g_0)}{\sqrt{|G||K|}}\sum_{k\in K}\chi(k),
$$

so the [character-sum cancellation lemma](group.md#character-sum-cancellation-lemma) gives probability $|K|/|G|$ on $K^\perp$ and zero elsewhere. The [modulus](complex-analysis.md#modulus) of $\chi(g_0)$ is one, so the offset has no effect on the distribution.

<h4 id="simon-s-problem">Simon's problem</h4>

↑ **Parent:** [Hidden subgroup problem](#hidden-subgroup-problem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simon's_problem)

Simon's problem asks for the hidden string $p\in\{0,1\}^n$ promised by $f(x)=f(y)$ exactly when $x\mathbin\oplus y\in\{0^n,p\}$. It is the [hidden subgroup problem](#hidden-subgroup-problem) on $(\mathbb Z_2)^n$ with hidden subgroup $\{0^n,p\}$.

<h5 id="classical-collision-query-bound-for-simon-s-problem">Classical collision query bound for Simon's problem</h5>

↑ **Parent:** [Simon's problem](#simon-s-problem)

For an unknown nonzero period, a collision $f(x)=f(y)$ reveals the period $x\mathbin\oplus y$. [Birthday problem](probability-and-statistics.md#birthday-problem) sampling finds one using $O(2^{n/2})$ queries with bounded error. A matching lower bound follows by choosing the period and output labels randomly: without a collision, $q$ queries rule out at most $\binom q2$ candidate periods. For $q=o(2^{n/2})$, almost all periods remain consistent with the transcript. The exponential separation is in query complexity, compared with [Simon's algorithm](#simon-s-algorithm)'s linear quantum query count.

<h5 id="simon-s-algorithm">Simon's algorithm</h5>

↑ **Parent:** [Simon's problem](#simon-s-problem)

Simon's algorithm prepares hidden-subgroup [coset states](#coset-state), applies the [quantum Fourier transform](#quantum-fourier-transform) over $(\mathbb Z_2)^n$, and samples vectors $y$ satisfying $y\cdot p=0$ over $\mathbb F_2$. Repeated samples and [Gaussian elimination](numerical-analysis.md#gaussian-elimination) recover $p$ with $O(n)$ oracle queries and polynomial computation.

###### Expected query count for Simon sampling

↑ **Parent:** [Simon's algorithm](#simon-s-algorithm)

With a nonzero hidden period, [Simon's algorithm](#simon-s-algorithm) samples uniformly from its $(n-1)$-dimensional [orthogonal complement over the binary field](#orthogonal-complement-over-the-binary-field). At rank $k$, a new sample raises the rank with probability $1-2^{k-(n-1)}$. Summing the geometric waiting times gives an expected $n-1+\sum_{j=1}^{n-1}(2^j-1)^{-1}<n+1$ queries. After $n-1+c$ samples, the probability of insufficient rank is less than $2^{-c}$, by a [union bound](probability-inequality.md#boole-s-inequality) over the nonzero linear functionals that could annihilate all samples.

<h6 id="single-sample-distribution-in-simon-s-algorithm">Single-sample distribution in Simon's algorithm</h6>

↑ **Parent:** [Simon's algorithm](#simon-s-algorithm)

If the hidden string is zero, one oracle-Hadamard run samples every $y\in\mathbb F_2^n$ with probability $2^{-n}$. If the hidden string is nonzero, it samples every $y$ satisfying $y\cdot p=0$ with probability $2^{-(n-1)}$ and every other string with probability zero. Pairing $x$ with $x\mathbin\oplus p$ makes the forbidden amplitudes cancel.

###### Orthogonal complement over the binary field

↑ **Parent:** [Simon's algorithm](#simon-s-algorithm)

For a subspace $W\leq\mathbb F_2^n$, its orthogonal complement is $W^\perp=\{y:x\cdot y=0\text{ for every }x\in W\}$, where the dot product is evaluated modulo two.

#### Stabilizer as a hidden subgroup

↑ **Parent:** [Hidden subgroup problem](#hidden-subgroup-problem)

For a [group action](group-theory.md#group-action) $F:G\times X\to X$ and fixed $x$, the orbit map $f_x(g)=F(g,x)$ hides the [stabilizer subgroup](group-theory.md#stabilizer-subgroup) $G_x$: $f_x(g)=f_x(h)$ exactly when $h^{-1}g\in G_x$, equivalently when $g$ and $h$ lie in the same left coset of $G_x$.

### Cyclic shift operator

↑ **Parent:** [Quantum Fourier transform](#quantum-fourier-transform)

On a basis indexed by $\mathbb Z_N$, a cyclic shift operator has the form $U(a)|b\rangle=|a+b\bmod N\rangle$. The [quantum Fourier transform](#quantum-fourier-transform) simultaneously diagonalizes all such shifts.

#### Cyclic shift diagonalization by the quantum Fourier transform

↑ **Parent:** [Cyclic shift operator](#cyclic-shift-operator)

For the cyclic shift $S|j\rangle=|j+1\bmod N\rangle$ and the convention

$$
\operatorname{QFT}_N|k\rangle=N^{-1/2}\sum_j e^{2\pi ijk/N}|j\rangle,
$$

the Fourier states obey

$$
S\operatorname{QFT}_N|k\rangle=e^{-2\pi ik/N}\operatorname{QFT}_N|k\rangle.
$$

Consequently $S=\operatorname{QFT}_N D\operatorname{QFT}_N^{-1}$, where $D|k\rangle=e^{-2\pi ik/N}|k\rangle$.

### Quantum phase estimation

↑ **Parent:** [Quantum Fourier transform](#quantum-fourier-transform)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_phase_estimation)

Given controlled powers of a unitary $U$ and an eigenstate $U|\psi\rangle=e^{2\pi i\phi}|\psi\rangle$, quantum phase estimation outputs an approximation to $\phi$. If the input is a superposition of eigenstates, measurement selects an eigenphase with probability equal to the squared magnitude of its coefficient.

#### Quantum phase estimation tail bound

↑ **Parent:** [Quantum phase estimation](#quantum-phase-estimation)

Let $L=2^t$, let $j_0$ be the nearest label to $L\phi$, and let $m\geq2$. The exact [quantum phase estimation](#quantum-phase-estimation) amplitude is $L^{-1}\sum_{a=0}^{L-1}e^{2\pi ia(\phi-j/L)}$. The sine bound on circular distances gives probability at most $1/(4d_j^2)$, where $d_j$ is the centered distance from $j$ to $L\phi$. At label distance $\ell$ from $j_0$, $|d_j|\geq\ell-1/2$, with at most two labels for each $\ell$. Since $(\ell-1/2)^{-2}\leq[(\ell-1)\ell]^{-1}$, the tail telescopes to the displayed bound. Adding $u$ control [qubits](quantum-mechanics.md#qubit) beyond $b$ desired phase bits gives circular accuracy below $2^{-b}$ with failure probability at most $[2(2^u-1)]^{-1}$.

#### Near-grid quantum phase estimation

↑ **Parent:** [Quantum phase estimation](#quantum-phase-estimation)

For register size $N=2^t$ and [eigenphase](vector-space.md#eigenphase) $\phi=2\pi n/N+\epsilon$, the amplitude of decoded label $m$ is $N^{-1}\sum_{k=0}^{N-1}e^{ik(\phi-2\pi m/N)}$. The [finite geometric series](real-analysis.md#finite-geometric-series) gives $P(n)=\sin^2(N\epsilon/2)/[N^2\sin^2(\epsilon/2)]$. If $N|\epsilon|\ll1$, this is $1-(N^2-1)\epsilon^2/12+O(N^4\epsilon^4)$. Thus the nearest exactly representable phase is returned with [probability](probability-theory.md#probability) near one, not with certainty unless the offset vanishes.

// Target: quantum-error-correction.bigb

#### Parallel phase multiplication by coherent fanout

↑ **Parent:** [Quantum phase estimation](#quantum-phase-estimation)

Use [CNOT gates](#controlled-not-gate) to encode one logical [qubit](quantum-mechanics.md#qubit) and $r-1$ zero ancillas into the repetition subspace spanned by $|0^r\rangle,|1^r\rangle$. Apply the [phase gate](#phase-gate) in parallel to all $r$ physical [qubits](quantum-mechanics.md#qubit), then undo the encoding. The logical phase is multiplied by $r$ in one oracle-time layer. This copies computational-basis labels coherently rather than cloning an arbitrary [quantum state](quantum-mechanics.md#quantum-state). Blocks of sizes $1,2,4,\ldots,2^{n-1}$ prepare a dyadic Fourier phase state using $2^n-1$ parallel oracle applications.

#### Quantum phase estimation with a maximally mixed target

↑ **Parent:** [Quantum phase estimation](#quantum-phase-estimation)

For a $d$-dimensional [unitary operator](vector-space.md#unitary-operator) $V=\sum_{j=1}^de^{i\phi_j}|v_j\rangle\langle v_j|$, a [maximally mixed state](#maximally-mixed-state) $I/d$ on its target is the equal mixture of these [orthonormal](linear-algebra.md#orthonormal-set) [eigenvectors](linear-operator-theory.md#eigenvector). Therefore [quantum phase estimation](#quantum-phase-estimation) with register size $L$ produces label $m$ with [probability](probability-theory.md#probability)

$$
p(m)=\frac1d\sum_{j=1}^d|a_m(\phi_j)|^2,\qquad a_m(\phi)=\frac1L\sum_{x=0}^{L-1}e^{ix(\phi-2\pi m/L)}.
$$

This follows by [linearity](vector-space.md#linearity) of [unitary time evolution](quantum-mechanics.md#unitary-time-evolution) and the [Born rule](quantum-mechanics.md#born-rule) on the spectral mixture. If every [eigenphase](vector-space.md#eigenphase) has an exact $L$-grid label, that label has [probability](probability-theory.md#probability) equal to its multiplicity divided by $d$. Otherwise the exact distribution has tails, and the nearest labels are guaranteed only the [nearest-integer success bound for quantum phase estimation](#nearest-integer-success-bound-for-quantum-phase-estimation) weighted by the corresponding spectral [probabilities](probability-theory.md#probability).

#### Nearest-integer success bound for quantum phase estimation

↑ **Parent:** [Quantum phase estimation](#quantum-phase-estimation)

For a [unitary operator](vector-space.md#unitary-operator) [eigenphase](vector-space.md#eigenphase) $\phi$, an $n$-qubit [quantum phase estimation](#quantum-phase-estimation) register of size $L=2^n$ has output [probability amplitude](quantum-mechanics.md#probability-amplitude)

$$
a_m(\phi)=\frac1L\sum_{x=0}^{L-1}e^{ix(\phi-2\pi m/L)}.
$$

Choose the nearest integer label $m$ to $L\phi/(2\pi)$, with labels understood modulo $L$, and put $d=L\phi/(2\pi)-m$, taking the representative $|d|\leq1/2$. The [finite geometric series](real-analysis.md#finite-geometric-series) gives $|a_m|=|\sin(\pi d)|/[L|\sin(\pi d/L)|]$. For $0<|d|\leq1/2$, [concavity](real-analysis.md#concave-function) of sine gives $|\sin(\pi d)|\geq2|d|$, while $|\sin(\pi d/L)|\leq\pi|d|/L$. Thus the [probability](probability-theory.md#probability) of the nearest label is at least $4/\pi^2$. At $d=0$ it is exactly one. If two labels tie for nearest, each satisfies the bound.

#### Dyadic phase-gate identification

↑ **Parent:** [Quantum phase estimation](#quantum-phase-estimation)

For the [phase gate](#phase-gate) $R_a=\operatorname{diag}(1,e^{2\pi ia/2^n})$, apply powers $R_a^{2^{n-1}},\ldots,R_a$ to a [uniform quantum superposition](#uniform-quantum-superposition) on $n$ qubits. Binary positional weights multiply the phases into $e^{2\pi iax/2^n}$ on basis vector $|x\rangle$. The inverse [quantum Fourier transform](#quantum-fourier-transform) returns $|a\rangle$ exactly, by [orthogonality of roots of unity](algebra.md#orthogonality-of-roots-of-unity). Preparing the powers by repeated applications uses $2^n-1$ copies of $R_a$; this does not claim a number of gate calls polynomial in $n$. If $a$ is odd, its powers generate the entire set of dyadic phase gates because $a$ has a [modular inverse](number-theory.md#modular-multiplicative-inverse) modulo $2^n$.

#### Tensor-product eigenphase amplification

↑ **Parent:** [Quantum phase estimation](#quantum-phase-estimation)

An [eigenstate](quantum-mechanics.md#eigenstate) with phase $\phi$ becomes an eigenstate with phase $n\phi$ under the tensor product of $n$ copies of the [unitary operator](vector-space.md#unitary-operator). A promise $0\le\phi<1/n$ prevents modulo-one aliasing. For $n=2^s$ and dyadic $\phi=x/2^m$, [exact quantum phase estimation](#exact-quantum-phase-estimation) then needs $m-s$ phase bits and $2^{m-s}-1$ queries to a supplied joint controlled oracle. This is a saving in joint-oracle calls, not in the total number of individual oracle invocations needed to build that joint operation.

#### Positive-phase fractional power of a unitary operator

↑ **Parent:** [Quantum phase estimation](#quantum-phase-estimation)

Choose eigenphase representatives $0\leq\phi_j<1$ for a [unitary operator](vector-space.md#unitary-operator) $U$ and a positive integer $M$. Its positive-phase fractional power acts on each [eigenstate](quantum-mechanics.md#eigenstate) by $e^{2\pi i\phi_j/M}$. This branch uses arguments in $[0,2\pi)$ and can differ from the usual complex principal branch using $(-\pi,\pi]$. For exactly dyadic phases, [exact quantum phase estimation](#exact-quantum-phase-estimation) stores each label in a coherent phase register; bitwise [phase gates](#phase-gate) multiply it by the required phase, and inverse phase estimation removes the labels. Keeping the phase register unmeasured preserves arbitrary [eigenstate](quantum-mechanics.md#eigenstate) superpositions and resets the [ancilla qubits](quantum-information-theory.md#ancilla-qubit). With only controlled-$U$ and controlled-$U^{-1}$ primitives, the direct method uses $2(2^n-1)$ oracle calls for $n$ exact phase bits.

#### Quantum spectral filtering

↑ **Parent:** [Quantum phase estimation](#quantum-phase-estimation)

Let a [Hermitian operator](hilbert-space.md#hermitian-operator) $A$ have dyadic [eigenvalues](linear-operator-theory.md#eigenvalue) $\lambda_j=c_j/2^t$ in $[0,1)$ for known $t$, with controlled access to the [unitary operator](vector-space.md#unitary-operator) $U=e^{2\pi iA}$. This interval ensures that different [eigenvalues](linear-operator-theory.md#eigenvalue) have different [eigenphases](vector-space.md#eigenphase); exact representability alone would not exclude phase aliasing, as $0$ and $1$ both give phase zero. Let a real [function](function.md) $h$ obey $|h(\lambda_j)|\leq1$, and assume the required [quantum variable rotations](#quantum-variable-rotation) are available. Coherent [exact quantum phase estimation](#exact-quantum-phase-estimation), a [quantum variable rotation](#quantum-variable-rotation) and [uncomputation](#uncomputation) implement

$$
|u_j\rangle|0\rangle\longmapsto|u_j\rangle\left(\sqrt{1-h(\lambda_j)^2}|0\rangle+h(\lambda_j)|1\rangle\right).
$$

[Postselection](quantum-measurement.md#postselection) on flag one gives $h(A)|b\rangle$ normalized, with [probability](probability-theory.md#probability) $\|h(A)|b\rangle\|^2$, provided this vector is nonzero. Erasing the [eigenvalue](linear-operator-theory.md#eigenvalue) label by [uncomputation](#uncomputation) is essential to preserve coherence between different [eigenvectors](linear-operator-theory.md#eigenvector). On this dyadic spectrum, $U^{2^t}=I$ gives $U^{-1}=U^{2^t-1}$, so reversing the phase-estimation gates is possible using forward controlled-$U$ calls. The choice $h(\lambda)=\lambda$ multiplies by $A$; a scaled reciprocal gives the different filter used in the [HHL algorithm](#hhl-algorithm).

##### Singular obstruction to normalized quantum matrix multiplication

↑ **Parent:** [Quantum spectral filtering](#quantum-spectral-filtering)

If $|b\rangle$ lies in the [kernel](linear-algebra.md#kernel-of-a-linear-map) of $A$, then $A|b\rangle=0$ has no normalized [quantum state](quantum-mechanics.md#quantum-state). A request to produce that normalized vector with positive [probability](probability-theory.md#probability) is consequently undefined. For example, $A=\operatorname{diag}(0,1/2)$ on one [qubit](quantum-mechanics.md#qubit) has distinct dyadic [eigenvalues](linear-operator-theory.md#eigenvalue), but annihilates $|0\rangle$. The corrected filtering assertion requires $A|b\rangle\neq0$; it cannot be repaired by assigning a positive success probability to this input.

##### Success probability of positive quantum spectral filtering

↑ **Parent:** [Quantum spectral filtering](#quantum-spectral-filtering)

For $0\leq A<I$ and normalized $|b\rangle=\sum_j\beta_j|u_j\rangle$, filtering by $h(\lambda)=\lambda$ succeeds with

$$
P=\sum_j|\beta_j|^2\lambda_j^2\geq\lambda_{\min}^2.
$$

The inequality follows by replacing each nonnegative $\lambda_j^2$ by its minimum and using $\sum_j|\beta_j|^2=1$. Equality holds exactly when all occupied [eigenvectors](linear-operator-theory.md#eigenvector) belong to the minimum-[eigenvalue](linear-operator-theory.md#eigenvalue) [eigenspace](linear-operator-theory.md#eigenspace). If $\lambda_{\min}=0$, success is positive exactly for inputs outside the [kernel](linear-algebra.md#kernel-of-a-linear-map) of $A$.

#### Exact quantum phase estimation

↑ **Parent:** [Quantum phase estimation](#quantum-phase-estimation)

If $U|\psi\rangle=e^{2\pi ij/N}|\psi\rangle$, controlled powers of $U$ applied to a uniform $N$-state control register produce

$$
|\phi_j\rangle=\frac1{\sqrt N}\sum_{k=0}^{N-1}e^{2\pi ijk/N}|k\rangle.
$$

These states are the Fourier basis. Applying the inverse quantum Fourier transform and measuring returns $j$ with probability one.

## BB84

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/BB84)

The BB84 protocol encodes random classical bits in independently chosen computational and Hadamard bases. Sender and receiver publicly compare bases and retain only positions where their bases agree; disturbance of a test sample detects eavesdropping.

### Bit error rate

↑ **Parent:** [BB84](#bb84)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bit_error_rate)

The bit error rate is the fraction, or probability, of transmitted or retained bits that differ between sender and receiver. In quantum key distribution, an unexpectedly high bit error rate reveals channel noise or possible eavesdropping.

## Breidbart basis

↑ **Parent:** [Quantum theory](quantum-theory.md)

The Breidbart basis bisects the computational and diagonal qubit bases. For equiprobable $|0\rangle$ and $|-\rangle$, whose overlap magnitude is $1/\sqrt2$, it realizes the Helstrom measurement and succeeds with probability

$$
\frac12\left(1+\frac1{\sqrt2}\right)=\cos^2\frac\pi8.
$$

This intermediate basis occurs in attacks and discrimination calculations involving [BB84](#bb84).

## Bell state

↑ **Parent:** [Quantum theory](quantum-theory.md)

[This section is present in another page, follow this link to view it.](bell-state.md)

## Variational method

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Variational_method)

The Rayleigh quotient of any normalized trial state is at least the ground-state energy.

### Nodeless theorem for a one-dimensional ground state

↑ **Parent:** [Variational method](#variational-method)

For a regular one-dimensional confining potential, the bound-state eigenfunctions can be ordered by their number of nodes. The unique nodeless normalizable eigenfunction is the ground state.

### Exact ground state of a solvable sextic potential

↑ **Parent:** [Variational method](#variational-method)

For

$$
V(x)=\frac{\hbar^2}{2m}(x^6-3x^2+2),
$$

the nodeless wavefunction $e^{-x^4/4}$ is an exact eigenstate with energy $\hbar^2/m$, and hence is the ground state.

### Gaussian variational estimate for a solvable sextic potential

↑ **Parent:** [Variational method](#variational-method)

For the trial state $e^{-\alpha x^2/2}$, the dimensionless Rayleigh quotient is

$$
\varepsilon(\alpha)=2+\frac\alpha2-\frac3{2\alpha}+\frac{15}{8\alpha^3}.
$$

Its unique minimizer is

$$
\alpha_*^2=\frac{-3+\sqrt{54}}2,
$$

and at the minimum $\varepsilon(\alpha_*)=2+2\alpha_*/3-1/\alpha_*$.

### Ground-state energy monotonicity under potential ordering

↑ **Parent:** [Variational method](#variational-method)

If $V_1\geq V_2$ pointwise for Hamiltonians with the same kinetic term, using the ground state of $H_1$ as a trial state for $H_2$ gives $E_1\geq E_2$.

### Quantum virial identity from scaling

↑ **Parent:** [Variational method](#variational-method)

For a normalized dilation $\psi_\lambda(x)=\lambda^{d/2}\psi(\lambda x)$ and a homogeneous potential of degree $-n$, the energy is $\lambda^2T+\lambda^nV$. Stationarity at an eigenstate gives $2T+nV=0$.

#### Fall to the centre for a supercritical inverse-power potential

↑ **Parent:** [Quantum virial identity from scaling](#quantum-virial-identity-from-scaling)

For an attractive potential $-\alpha/|x|^n$ with $n>2$, dilations make the negative potential energy grow faster than kinetic energy, sending the Rayleigh quotient to minus infinity.

### Exact variational solution in a two-level system

↑ **Parent:** [Variational method](#variational-method)

If a normalized trial family covers the entire two-dimensional Hilbert space, minimizing its Rayleigh quotient gives the exact lower eigenvalue rather than merely an upper bound.

#### Level repulsion in a two-level Hamiltonian

↑ **Parent:** [Exact variational solution in a two-level system](#exact-variational-solution-in-a-two-level-system)

The eigenvalues of $\left(\begin{smallmatrix}E_1&h\\h&E_2\end{smallmatrix}\right)$ are their mean plus or minus $\sqrt{(E_2-E_1)^2/4+h^2}$, so nonzero coupling increases their separation.

## Landau level

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Landau_level)

A charged particle in a uniform magnetic field has equally spaced orbital energy levels with guiding-centre degeneracy.

### Ground-state filling of two spin-degenerate Landau levels

↑ **Parent:** [Landau level](#landau-level)

For $2N$ noninteracting electrons in a planar sample of area $A$, neglecting Zeeman splitting leaves two spin states for each orbital. Each Landau level therefore holds $D=eBA/(\pi\hbar)$ electrons. When $N\le D\le2N$, fill the lowest level with $D$ electrons and the next with $2N-D$; summing their energies gives the displayed concave quadratic in $B$. The energies at the two integer-filling endpoints are equal.

### Lowest Landau level

↑ **Parent:** [Landau level](#landau-level)

The $n=0$ level of the transverse [harmonic oscillator](classical-mechanics.md#simple-harmonic-motion) in a uniform [magnetic field](electromagnetism.md#magnetic-field), with [energy](classical-mechanics.md#energy) $\hbar|qB|/(2m)$ before longitudinal [kinetic energy](classical-mechanics.md#kinetic-energy) or spin contributions.

### Cyclotron frequency

↑ **Parent:** [Landau level](#landau-level)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cyclotron_frequency)

A particle of charge $q$ and mass $m$ in a uniform magnetic field of magnitude $B$ has cyclotron angular frequency $\omega_c=|qB|/m$.

### Landau gauge for a uniform magnetic field

↑ **Parent:** [Landau level](#landau-level)

For $\mathbf B=B\mathbf e_z$, the vector potential $\mathbf A=(0,Bx,0)$ is a Landau gauge. Translation invariance in $y$ turns the transverse Hamiltonian into a family of harmonic oscillators in $x$ whose centres are labelled by the conserved $y$-momentum.

### Degeneracy of a Landau level

↑ **Parent:** [Landau level](#landau-level)

In a planar region of area $A$, each spinless Landau level has guiding-centre degeneracy

$$
D=\frac{|qB|A}{2\pi\hbar}=\frac{|\Phi|}{h/|q|}.
$$

Magnetic periodic boundary conditions require this flux count to be an integer.

### Spin splitting of Landau levels

↑ **Parent:** [Landau level](#landau-level)

For a spin-one-half particle with the Pauli magnetic term and gyromagnetic factor two, the orbital energies $\hbar\omega_c(n+1/2)$ split into $\hbar\omega_c n$ and $\hbar\omega_c(n+1)$. The lowest level has one spin branch; every positive level has two.

### Landau levels in crossed electric and magnetic fields

↑ **Parent:** [Landau level](#landau-level)

A uniform electric field perpendicular to a uniform magnetic field shifts each cyclotron oscillator's guiding centre and makes its energy depend linearly on the conserved momentum. The formerly degenerate Landau levels therefore become tilted bands.

#### Electric-cross-magnetic-field drift

↑ **Parent:** [Landau levels in crossed electric and magnetic fields](#landau-levels-in-crossed-electric-and-magnetic-fields)

In uniform perpendicular electric and magnetic fields, a charged particle's guiding centre drifts with velocity $\mathbf v_D=\mathbf E\times\mathbf B/B^2$, independently of its charge and mass. For $\mathbf E=E\mathbf e_x$ and $\mathbf B=B\mathbf e_z$, this gives $v_y=-E/B$.

#### Electric-field splitting of a Landau level in a rectangle

↑ **Parent:** [Landau levels in crossed electric and magnetic fields](#landau-levels-in-crossed-electric-and-magnetic-fields)

In [Landau gauge](#landau-gauge-for-a-uniform-magnetic-field) with periodic boundary conditions of length $L_y$, adjacent guiding centres differ by $\Delta k_y=2\pi/L_y$. A perpendicular electric field tilts the energy by $-(E/B)\hbar k_y$, so adjacent states formerly in one degenerate [Landau level](#landau-level) are separated by $2\pi\hbar|E/B|/L_y$.

### Symmetric gauge

↑ **Parent:** [Landau level](#landau-level)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Symmetric_gauge)

For a constant magnetic field,

$$
A(x)=\frac12B\times x
$$

is the symmetric gauge.

#### Kinetic momentum and magnetic pseudomomentum

↑ **Parent:** [Symmetric gauge](#symmetric-gauge)

For charge $e$, define

$$
\pi=p-eA,\qquad K=p+eA.
$$

In the symmetric gauge,

$$
[K_i,\pi_j]=0,
\qquad
[K_i,K_j]=-ie\hbar\varepsilon_{ijk}B_k.
$$

##### Kinetic momentum

↑ **Parent:** [Kinetic momentum and magnetic pseudomomentum](#kinetic-momentum-and-magnetic-pseudomomentum)

The kinetic momentum $\boldsymbol\Pi=\mathbf p-q\mathbf A$ equals $m\mathbf v$ for a nonrelativistic charged particle and is invariant under an electromagnetic [gauge transformation](electromagnetism.md#gauge-transformation).

##### Magnetic translation

↑ **Parent:** [Kinetic momentum and magnetic pseudomomentum](#kinetic-momentum-and-magnetic-pseudomomentum)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Magnetic_translation)

For a lattice vector $r$,

$$
\mathcal T_r=\exp\left(\frac i\hbar r\cdot K\right)
$$

acts in the symmetric gauge as

$$
(\mathcal T_r\psi)(x)
=\exp\left(\frac{ie}{2\hbar}r\cdot(B\times x)\right)\psi(x+r).
$$

It commutes with $(p-eA)^2/(2m)+V(x)$ when $V(x+r)=V(x)$.

###### Magnetic translation algebra

↑ **Parent:** [Magnetic translation](#magnetic-translation)

For constant $B$,

$$
\mathcal T_r\mathcal T_{r'}
=\exp\left(\frac{ie}{\hbar}(r\times r')\cdot B\right)
\mathcal T_{r'}\mathcal T_r.
$$

###### Magnetic flux quantum

↑ **Parent:** [Magnetic translation algebra](#magnetic-translation-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Magnetic_flux_quantum)

Magnetic translations along two lattice vectors commute when their cell flux obeys

$$
\frac{e\Phi}{\hbar}\in2\pi\mathbb Z,
\qquad\text{equivalently}\qquad
\Phi\in\frac he\mathbb Z.
$$

###### Fluxoid and flux quantization in a superconductor

↑ **Parent:** [Magnetic flux quantum](#magnetic-flux-quantum)

For a nonvanishing superconducting [order parameter](critical-phenomenon.md#order-parameter) $\psi=\sqrt{n_s}e^{i\theta}$, $j=(qn_s/m)(\hbar\nabla\theta-qA)$. Single-valuedness gives phase winding $2\pi N$ around a closed curve, hence the [fluxoid and flux quantization in a superconductor](#fluxoid-and-flux-quantization-in-a-superconductor) identity above. Magnetic flux alone is $Nh/q$ when the current integral vanishes. If the entire spanning surface is in a region where $D\psi=0$, the field vanishes there and the winding is zero; nonzero quantized flux requires a hole or a vortex core where that condition does not hold.

<h2 id="bloch-s-theorem">Bloch's theorem</h2>

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bloch's_theorem)

In a periodic potential, energy eigenstates have the form $e^{ik\cdot x}u_k(x)$ with lattice-periodic $u_k$.

### Particle in a one-dimensional lattice

↑ **Parent:** [Bloch's theorem](#bloch-s-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Particle_in_a_one-dimensional_lattice)

A quantum particle in a one-dimensional lattice experiences a periodic potential. Bloch states organize its spectrum into bands and gaps; the [Kronig-Penney model](#kronig-penney-model) realizes this behavior with an idealized array of barriers or narrow delta barriers.

#### Kronig-Penney model

↑ **Parent:** [Particle in a one-dimensional lattice](#particle-in-a-one-dimensional-lattice)

The delta-comb Kronig-Penney potential is

$$
V(x)=V_0\sum_{n\in\mathbb Z}\delta(x-na).
$$

##### Floquet discriminant of the delta-comb Kronig-Penney model

↑ **Parent:** [Kronig-Penney model](#kronig-penney-model)

For $E=\hbar^2k^2/(2m)$ and $\gamma=mV_0/(\hbar^2k)$,

$$
\frac12\operatorname{tr}M(E)
=\cos(ka)+\gamma\sin(ka).
$$

Thus the allowed bands satisfy $|\cos(ka)+\gamma\sin(ka)|\leq1$.

##### Attractive delta-comb Kronig-Penney model

↑ **Parent:** [Kronig-Penney model](#kronig-penney-model)

For

$$
V(x)=-\frac{\hbar^2\lambda}{m}\sum_{n\in\mathbb Z}\delta(x-na),
$$

the [wavefunction](quantum-mechanics.md#wave-function) is continuous across every lattice point and obeys

$$
\psi'(na^+)-\psi'(na^-)=-2\lambda\psi(na).
$$

At negative energy $E=-\hbar^2\mu^2/(2m)$, an [allowed energy band](#allowed-energy-band) satisfies

$$
\boxed{\lambda\tanh\frac{\mu a}{2}<\mu<\lambda\coth\frac{\mu a}{2}.}
$$

At positive energy $E=\hbar^2k^2/(2m)$, it satisfies

$$
\boxed{\left|\cos(ka)-\frac\lambda k\sin(ka)\right|<1.}
$$

###### Negative-energy band of an attractive delta comb

↑ **Parent:** [Attractive delta-comb Kronig-Penney model](#attractive-delta-comb-kronig-penney-model)

With well strength $\lambda$ and spacing $a$, negative-energy Bloch states obey $\tanh y\leq2y/(\lambda a)\leq\coth y$, where $y=\kappa a/2$. There is one negative band: it reaches zero when $\lambda a\leq2$ and is separated from zero when $\lambda a>2$.

##### Scattering-amplitude equations for one-dimensional band edges

↑ **Parent:** [Kronig-Penney model](#kronig-penney-model)

If one symmetric cell has reflection and transmission amplitudes $r,t$, then

$$
\operatorname{tr}M
=\frac{(t^2-r^2)e^{ika}+e^{-ika}}t.
$$

At a periodic or antiperiodic band edge, with $\operatorname{tr}M=2\sigma$ and $\sigma=\pm1$, setting $z=e^{-ika}$ gives

$$
z^2-2\sigma tz+t^2-r^2=0,
\qquad
z=\sigma t\pm r.
$$

### Electronic band structure

↑ **Parent:** [Bloch's theorem](#bloch-s-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Electronic_band_structure)

Electronic band structure is the collection of allowed electron energy bands and gaps in a periodic medium, usually represented as energy versus crystal momentum. An [energy band](#energy-band) is one branch of that structure.

#### Energy band

↑ **Parent:** [Electronic band structure](#electronic-band-structure)

An energy band is a continuous branch $E_j(k)$ of the [dispersion relation](wave-equation.md#dispersion-relation) of a periodic quantum system.

##### Impurity level in a crystal

↑ **Parent:** [Energy band](#energy-band)

A spatially localized electronic level produced by a defect or foreign atom in a crystalline potential. Such levels can lie in a host band gap, where no extended host state has the same energy, while impurity resonances can also occur inside an [energy band](#energy-band). Dilute localized levels are nearly independent; increasing overlap can broaden them into an impurity band. The location and existence of a bound level depend on the impurity potential.

##### Band effective mass

↑ **Parent:** [Energy band](#energy-band)

In one dimension the [band effective mass](#band-effective-mass) is defined by $1/m^*(k)=E''(k)/\hbar^2$. Together with $v=E'(k)/\hbar$ and $\hbar\dot k=F$, this gives $\dot v=F/m^*$. Negative band curvature produces negative [effective mass](#band-effective-mass) for the electron [wave packet](wave-equation.md#wave-packet); near a filled-band maximum the equivalent missing-electron description uses positively responding holes. In several dimensions the inverse mass is the Hessian $\partial_i\partial_jE/\hbar^2$.

##### Allowed energy band

↑ **Parent:** [Energy band](#energy-band)

An allowed energy band is an interval of energies supporting extended [Bloch states](#bloch-state). Adjacent bands may be separated by a [band gap](#band-gap).

##### Band gap

↑ **Parent:** [Energy band](#energy-band)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Band_gap)

A band gap is an energy interval between adjacent [energy bands](#energy-band) containing no allowed bulk state.

###### Avoided crossing

↑ **Parent:** [Band gap](#band-gap)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Avoided_crossing)

An avoided crossing occurs when two parameter-dependent [eigenvalues](linear-operator-theory.md#eigenvalue) approach one another but an interaction prevents equality. Near a two-level crossing, a nonzero off-diagonal [matrix element](vector-space.md#matrix-element) opens a positive minimum gap.

##### Band filling

↑ **Parent:** [Energy band](#energy-band)

For spin-one-half electrons, one nondegenerate orbital band contains two one-particle states per primitive cell, one for each spin. A partially filled band has nearby empty states into which an electric field can move electrons and is ordinarily conducting. A completely filled band carries no net current under a small field because all crystal momenta are occupied symmetrically.

###### Band insulator

↑ **Parent:** [Band filling](#band-filling)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Band_insulator)

A band insulator has an integer number of completely filled [energy bands](#energy-band), with the [Fermi energy](statistical-physics.md#fermi-energy) inside a positive [band gap](#band-gap). At zero temperature, no arbitrarily low-energy charged excitation is then available.

###### Overlapping energy bands prevent a band insulator

↑ **Parent:** [Band insulator](#band-insulator)

If the minimum of the next [energy band](#energy-band) lies at or below the maximum of the nominally filled band, electrons can lower their energy by occupying the next band and leaving holes in the first. The resulting partially filled bands prevent a band-insulating state.

### Bloch oscillation

↑ **Parent:** [Bloch's theorem](#bloch-s-theorem)

In a single isolated [energy band](#energy-band), a [wave packet](wave-equation.md#wave-packet) subject to a constant force satisfies $\hbar\dot k=F$. Its [group velocity](wave-equation.md#group-velocity) is periodic in $k$ with reciprocal-lattice period $2\pi/a$, so its position oscillates with period $2\pi\hbar/(|F|a)$ when its mean velocity over a band is zero. For $E(k)=E_0-2J\cos ka$, integrating the sinusoidal velocity gives the oscillation explicitly. This ideal description neglects scattering and interband tunnelling.

### Translation-character proof of Bloch theorem

↑ **Parent:** [Bloch's theorem](#bloch-s-theorem)

The lattice translations commute with one another and with a lattice-periodic Hamiltonian. They can therefore be diagonalized simultaneously within each energy eigenspace. Every unitary character of a [Bravais lattice](quantum-mechanics.md#bravais-lattice) has the form $r\mapsto e^{-ik\cdot r}$, with $k$ defined modulo the [reciprocal lattice](quantum-mechanics.md#reciprocal-lattice). Hence $T_r\psi_k=e^{-ik\cdot r}\psi_k$, so $u_k(x)=e^{-ik\cdot x}\psi_k(x)$ is lattice-periodic.

### Bloch state

↑ **Parent:** [Bloch's theorem](#bloch-s-theorem)

A Bloch state is an energy eigenstate of a lattice-periodic Hamiltonian that is simultaneously an eigenstate of every lattice translation. It can be written as $\psi_k(x)=e^{ik\cdot x}u_k(x)$ with lattice-periodic $u_k$.

#### Crystal momentum

↑ **Parent:** [Bloch state](#bloch-state)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Crystal_momentum)

Crystal momentum is the translation quantum number $\hbar k$ of a [Bloch state](#bloch-state). Since $k$ and $k+G$ give the same translation character whenever $G$ belongs to the [reciprocal lattice](quantum-mechanics.md#reciprocal-lattice), crystal momentum is defined modulo reciprocal-lattice vectors.

### Periodic potential

↑ **Parent:** [Bloch's theorem](#bloch-s-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Periodic_potential)

A periodic potential satisfies $V(x+a)=V(x)$ for some lattice period $a$. Its Fourier coefficients couple plane waves whose wavevectors differ by reciprocal-lattice vectors.

### Nearly-free electron model

↑ **Parent:** [Bloch's theorem](#bloch-s-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nearly-free_electron_model)

The nearly-free electron model treats a weak [periodic potential](#periodic-potential) by [degenerate perturbation theory](quantum-mechanics.md#degenerate-perturbation-theory). At a Bragg crossing, a Fourier coefficient $V_n$ couples the two degenerate plane waves and opens an energy gap of width $2|V_n|$.

#### Nearly-free electron dispersion near a one-dimensional band gap

↑ **Parent:** [Nearly-free electron model](#nearly-free-electron-model)

For

$$
V(x)=\sum_{n\in\mathbb Z}V_ne^{2\pi inx/a},
$$

write $k=n\pi/a+\kappa$. Near the $n$th Bragg crossing,

$$
E_\pm(k)=V_0+\frac{\hbar^2}{2m}
\left[\left(\frac{n\pi}{a}\right)^2+\kappa^2\right]
\pm\sqrt{
\left(\frac{\hbar^2n\pi\kappa}{ma}\right)^2+|V_n|^2}.
$$

At $\kappa=0$, the two branches differ by $2|V_n|$.

### Floquet matrix for a one-dimensional periodic potential

↑ **Parent:** [Bloch's theorem](#bloch-s-theorem)

For a potential of period $a$, the Floquet matrix $M(E)$ maps Cauchy data through one cell:

$$
\begin{pmatrix}\psi(x+a)\\\psi'(x+a)\end{pmatrix}
=M(E)\begin{pmatrix}\psi(x)\\\psi'(x)\end{pmatrix}.
$$

For a real Schrodinger equation, $\det M=1$.

#### Floquet discriminant and energy bands

↑ **Parent:** [Floquet matrix for a one-dimensional periodic potential](#floquet-matrix-for-a-one-dimensional-periodic-potential)

The Floquet multipliers solve

$$
\mu^2-\operatorname{tr}(M)\mu+1=0.
$$

Bounded Bloch waves occur when $|\operatorname{tr}M|\leq2$, with $\mu=e^{\pm iKa}$. Band edges satisfy $\operatorname{tr}M=\pm2$; outside the bands the multipliers are real reciprocal numbers and one solution grows exponentially.

### Tight binding

↑ **Parent:** [Bloch's theorem](#bloch-s-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tight_binding)

A tight-binding model expands a particle's state in localized orbitals and represents tunnelling between sites by off-diagonal Hamiltonian matrix elements.

#### Dilute-hopping lattice propagator

↑ **Parent:** [Tight binding](#tight-binding)

For equivalent minima with nearest-neighbour hopping magnitude $\Delta$, paths with $r$ right steps and $s$ left steps have $r-s=n-m$. Summing $(\Delta\tau/\hbar)^{r+s}/(r!s!)$ and applying the [Fourier representation of a Kronecker delta](numerical-analysis.md#fourier-representation-of-a-kronecker-delta) gives the displayed [modified Bessel function](analysis.md#modified-bessel-function) kernel in a normalized localized-site basis. Its Fourier exponent gives the [tight-binding model](#tight-binding) energy $E(\theta)=E_{\rm well}-2\Delta\cos\theta$. Position-endpoint kernels can have an additional common local-wavefunction prefactor.

#### Harmonic approximation near a potential minimum

↑ **Parent:** [Tight binding](#tight-binding)

Near a nondegenerate minimum $x_0$, a smooth potential satisfies

$$
V(x)=V(x_0)+\frac12V''(x_0)(x-x_0)^2+\cdots.
$$

The localized levels are therefore approximately those of a harmonic oscillator of frequency $\sqrt{V''(x_0)/m}$; tunnelling broadens each level into a narrow band.

#### Finite periodic tight-binding ring

↑ **Parent:** [Tight binding](#tight-binding)

For $N$ identical sites of spacing $a$ with periodic boundary conditions, translation eigenstates have coefficients

$$
c_n=\frac{1}{\sqrt N}e^{ikna},
\qquad
e^{ikNa}=1.
$$

Thus $k=2\pi j/(Na)$ modulo the reciprocal-lattice period $2\pi/a$.

#### Two-direction nearest-neighbour tight-binding dispersion

↑ **Parent:** [Tight binding](#tight-binding)

For hopping amplitude $-\lambda$ from each lattice site to its neighbours at $\pm a_1$ and $\pm a_2$, a Bloch state has energy

$$
E(k)=E_0-2\lambda\bigl(\cos(k\cdot a_1)+\cos(k\cdot a_2)\bigr).
$$

The band ranges from $E_0-4|\lambda|$ to $E_0+4|\lambda|$ and therefore has width $8|\lambda|$.

### Brillouin zone

↑ **Parent:** [Bloch's theorem](#bloch-s-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Brillouin_zone)

The first Brillouin zone is a fundamental cell in reciprocal space. For a one-dimensional lattice of spacing $a$, one conventional choice is

$$
-\frac{\pi}{a}\leq k<\frac{\pi}{a}.
$$

#### Bragg point

↑ **Parent:** [Brillouin zone](#brillouin-zone)

A Bragg point is a [crystal momentum](#crystal-momentum) at which two plane waves differing by a [reciprocal lattice](quantum-mechanics.md#reciprocal-lattice) vector are degenerate. A periodic potential mixes the waves there, producing an [avoided crossing](#avoided-crossing) and opening a [band gap](#band-gap).

#### Brillouin zone of a two-dimensional triangular lattice

↑ **Parent:** [Brillouin zone](#brillouin-zone)

The reciprocal lattice of a two-dimensional triangular [Bravais lattice](quantum-mechanics.md#bravais-lattice) is triangular, so its [Wigner-Seitz cell](quantum-mechanics.md#wigner-seitz-cell) is a regular hexagon. Opposite boundary points are identified modulo reciprocal-lattice translations, and the six corners fall into two inequivalent classes of three corners each, conventionally denoted $K$ and $K'$.

## Pauli Z gate

↑ **Parent:** [Quantum theory](quantum-theory.md)

The Pauli $Z$ gate fixes $|0\rangle$ and maps $|1\rangle$ to $-|1\rangle$.

This gate acts by the corresponding [Pauli matrix](algebra.md#pauli-matrices), viewed as a unitary operator on one qubit.

## Pauli Y gate

↑ **Parent:** [Quantum theory](quantum-theory.md)

The Pauli $Y$ gate is $Y=iXZ$ and maps $|0\rangle$ to $i|1\rangle$ and $|1\rangle$ to $-i|0\rangle$.

This gate acts by the corresponding [Pauli matrix](algebra.md#pauli-matrices), viewed as a unitary operator on one qubit.

## Pauli X gate

↑ **Parent:** [Quantum theory](quantum-theory.md)

The Pauli $X$ gate interchanges $|0\rangle$ and $|1\rangle$.

This gate acts by the corresponding [Pauli matrix](algebra.md#pauli-matrices), viewed as a unitary operator on one qubit.

## Phase gate

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Phase_gate)

The single-qubit phase gate is $P(\phi)=\operatorname{diag}(1,e^{i\phi})$. On a computational-basis bit $b$, it contributes the phase $e^{i\phi b}$.

### Phase-gate discretization error

↑ **Parent:** [Phase gate](#phase-gate)

For $R(\theta)=\operatorname{diag}(1,e^{i\theta})$, the difference vanishes on $|0\rangle$ and multiplies $|1\rangle$ by $e^{i\theta}(e^{i\delta}-1)$. Its [operator norm](continuous-dual-space.md#operator-norm) is therefore $|e^{i\delta}-1|=2|\sin(\delta/2)|$. Choosing the nearest angle on the grid $2\pi m/2^n$, with circular distance, gives $|\delta|\leq\pi/2^n$ and a uniform bound of this size on the output-state norm error. This bound concerns state vectors, not an asserted equality with measurement-probability error.

### Controlled phase gate

↑ **Parent:** [Phase gate](#phase-gate)

The controlled phase gate contributes $e^{i\phi}$ exactly when both of its computational-basis input bits are one. It is diagonal and symmetric between its two qubits.

#### Controlled-Z gate

↑ **Parent:** [Controlled phase gate](#controlled-phase-gate)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Controlled-Z_gate)

The controlled-Z gate is $CP(\pi)=\operatorname{diag}(1,1,1,-1)$. Conjugating the target of a [controlled-NOT gate](#controlled-not-gate) by [Hadamard gates](#hadamard-gate) turns controlled-NOT into controlled-Z.

### Probabilistic phase-gate injection

↑ **Parent:** [Phase gate](#phase-gate)

The magic state $|A_\theta\rangle=(|0\rangle+e^{i\theta}|1\rangle)/\sqrt2$ and a short [controlled-NOT gate](#controlled-not-gate) circuit can apply either $P(\theta)$ or $P(-\theta)$ to an input, with a measured bit identifying the branch.

## Inverse quantum circuit

↑ **Parent:** [Quantum theory](quantum-theory.md)

The inverse of a quantum circuit applies the adjoints of its gates in reverse temporal order. The [Hadamard gate](#hadamard-gate), [Pauli Z gate](#pauli-z-gate), and [controlled-NOT gate](#controlled-not-gate) are each self-inverse.

## Controlled unitary gate

↑ **Parent:** [Quantum theory](quantum-theory.md)

A controlled-$U$ gate applies $U$ to its target exactly when its control qubit is one.

### Quantum variable rotation

↑ **Parent:** [Controlled unitary gate](#controlled-unitary-gate)

A quantum variable rotation uses an angle stored in a quantum register to rotate a target qubit coherently. For a binary angle, controlled fixed-angle rotations from each bit multiply to the desired total rotation.

#### Binary-angle implementation of a quantum variable rotation

↑ **Parent:** [Quantum variable rotation](#quantum-variable-rotation)

Suppose a [reversible circuit](computer-science.md#reversible-circuit) computes the angle bits $b_l(x)$ in $\theta_x=\sum_l b_l(x)\alpha_l$, where $\alpha_l$ are known binary place values. Apply a [controlled unitary gate](#controlled-unitary-gate) $R_y(2\alpha_l)$ to the target for each set angle bit. The [rotations about the y-axis](quantum-circuit.md#rotation-about-the-y-axis) commute and their angles add, giving $R_y(2\theta_x)$. Finally perform [uncomputation](#uncomputation) of the angle and arithmetic workspace. An $L$-bit angle needs $L$ controlled rotations and twice the reversible angle-computation cost. This preserves coherent superpositions of inputs and underlies the [HHL controlled reciprocal rotation](#hhl-controlled-reciprocal-rotation).

### Fredkin gate

↑ **Parent:** [Controlled unitary gate](#controlled-unitary-gate)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fredkin_gate)

The Fredkin gate, or controlled-SWAP gate, exchanges two target qubits exactly when its control qubit is one.

### Controlled-NOT gate

↑ **Parent:** [Controlled unitary gate](#controlled-unitary-gate)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Controlled-NOT_gate)

The controlled-NOT gate maps $|a,b\rangle$ to $|a,b\mathbin\oplus a\rangle$.

#### CNOT control reversal in the Hadamard basis

↑ **Parent:** [Controlled-NOT gate](#controlled-not-gate)

Writing a [CNOT gate](#controlled-not-gate) as $P_0\otimes I+P_1\otimes X$ gives $I\otimes Q_++Z\otimes Q_-$, where $Q_\pm=(I\pm X)/2$. In the [Hadamard basis](#hadamard-basis), $Z$ flips the sign label and $X$ is diagonal. Thus the same gate matrix reverses its control and target roles under the two local basis changes.

##### Measurement direction of a CNOT interaction

↑ **Parent:** [CNOT control reversal in the Hadamard basis](#cnot-control-reversal-in-the-hadamard-basis)

A [CNOT gate](#controlled-not-gate) can correlate either the original control's computational label with a computational pointer, or the original target's sign-basis label with a sign-basis pointer. For the second interpretation prepare the original control in $|+\rangle$ and read it in the [Hadamard basis](#hadamard-basis). Its two pointer states become $|+\rangle$ and $|-\rangle$, measuring $X$ on the original target. An apparatus role therefore depends on the ready state and readout as well as the [measurement interaction](quantum-measurement.md#measurement-interaction).

#### SWAP gate

↑ **Parent:** [Controlled-NOT gate](#controlled-not-gate)

The SWAP gate maps $|x\rangle|y\rangle$ to $|y\rangle|x\rangle$.

##### Three-CNOT decomposition of the SWAP gate

↑ **Parent:** [SWAP gate](#swap-gate)

Applying controlled-NOT gates with directions $1\to2$, $2\to1$, and $1\to2$ maps

$$
(x,y)\mapsto(x,x\oplus y)\mapsto(y,x\oplus y)\mapsto(y,x),
$$

and therefore implements the [SWAP gate](#swap-gate).

<h4 id="greenberger-horne-zeilinger-state">Greenberger–Horne–Zeilinger state</h4>

↑ **Parent:** [Controlled-NOT gate](#controlled-not-gate)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Greenberger–Horne–Zeilinger_state)

The three-qubit GHZ state is

$$
|\operatorname{GHZ}\rangle
=\frac{|000\rangle+|111\rangle}{\sqrt2}.
$$

##### Localizing a Bell pair from a GHZ state

↑ **Parent:** [Greenberger–Horne–Zeilinger state](#greenberger-horne-zeilinger-state)

Charlie measures his qubit of a [GHZ state](#greenberger-horne-zeilinger-state) in the $X$ basis. The two equally likely outcomes leave Alice and Bob in the [Bell states](bell-state.md) $\Phi^+$ or $\Phi^-$, respectively. Charlie sends the outcome bit $c$ to Bob, who applies the [Pauli operator](quantum-circuit.md#pauli-operator) $XZ^c$, giving $\Psi^+$ in either case. This is deterministic [LOCC](bell-state.md#local-operations-and-classical-communication) entanglement localization. If Charlie's record is ignored, Alice and Bob instead have the separable mixture $(|00\rangle\langle00|+|11\rangle\langle11|)/2$. The classical outcome is necessary to turn the conditional entanglement into a known usable Bell pair.

##### GHZ preparation with Hadamard and controlled-Z gates

↑ **Parent:** [Greenberger–Horne–Zeilinger state](#greenberger-horne-zeilinger-state)

For $n\geq2$, apply a [Hadamard gate](#hadamard-gate) to one [qubit](quantum-mechanics.md#qubit), then controlled-NOTs from it to all others. Replacing each [controlled-NOT gate](#controlled-not-gate) by a target Hadamard, a [Controlled-Z gate](#controlled-z-gate), and another target Hadamard uses $1+3(n-1)$ allowed gates. Each one-qubit reduced state is $I/2$, proving entanglement across each qubit-versus-rest bipartition.

##### Bell measurement on one qubit and one leg of a GHZ state

↑ **Parent:** [Greenberger–Horne–Zeilinger state](#greenberger-horne-zeilinger-state)

For $|\alpha\rangle=a|0\rangle+b|1\rangle$, a Bell measurement on $|\alpha\rangle$ and the first leg of a GHZ state leaves the other two legs in $a|00\rangle\pm b|11\rangle$, after applying $X$ to both legs for the two $\Psi$ outcomes.

##### Quantum circuit preparation of a three-qubit GHZ state

↑ **Parent:** [Greenberger–Horne–Zeilinger state](#greenberger-horne-zeilinger-state)

Starting from $|000\rangle$, apply a Hadamard gate to the first qubit and then controlled-NOT gates from the first qubit to each of the other two qubits.

##### Three-party dense coding with a GHZ state

↑ **Parent:** [Greenberger–Horne–Zeilinger state](#greenberger-horne-zeilinger-state)

If two senders share a GHZ state with a receiver, one sender can encode two bits with $X^xZ^z$ and the other one bit with $X^b$. Sending both qubits to the receiver produces one of eight orthogonal GHZ-basis states, so a joint measurement recovers all three bits.

##### GHZ theorem

↑ **Parent:** [Greenberger–Horne–Zeilinger state](#greenberger-horne-zeilinger-state)

The GHZ theorem uses perfect multipartite quantum correlations to contradict local predetermined values without a statistical inequality. For the three-qubit GHZ state, three certain Pauli-product relations force a fourth product to have the opposite sign from its quantum-mechanical value.

###### GHZ contradiction for N congruent to 3 modulo 4

↑ **Parent:** [GHZ theorem](#ghz-theorem)

For $|G_N^-\rangle=(|0\rangle^{\otimes N}-|1\rangle^{\otimes N})/\sqrt2$, let $O_j$ have one [Pauli X gate](#pauli-x-gate) at site $j$ and [Pauli Y gates](#pauli-y-gate) elsewhere, and let $X_N=X^{\otimes N}$. The relations $Y|0\rangle=i|1\rangle$, $Y|1\rangle=-i|0\rangle$ show that $O_j|G_N^-\rangle$ is proportional to $|G_N^-\rangle$ exactly when $N$ is odd. In that case its [eigenvalue](linear-operator-theory.md#eigenvalue) is $\lambda_N=(-1)^{(N+1)/2}$, while $X_N$ always has [eigenvalue](linear-operator-theory.md#eigenvalue) $-1$.

Under the [EPR criterion of reality](#epr-criterion-of-reality) and locality, each site's $X$ and $Y$ outcomes have predetermined values $x_j,y_j\in\{\pm1\}$. Multiplying the $N$ certain equations $x_j\prod_{k\ne j}y_k=\lambda_N$ gives $\prod_jx_j=\lambda_N$ when $N$ is odd, since every $y_k$ appears an even number of times. This contradicts the certain quantum value $-1$ precisely when $N\equiv3\pmod4$. Thus the displayed [GHZ state](#greenberger-horne-zeilinger-state) gives an infinite family of perfect-correlation contradictions with [local hidden-variable theory](#local-hidden-variable-theory), without an inequality.

### Hadamard test

↑ **Parent:** [Controlled unitary gate](#controlled-unitary-gate)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hadamard_test)

The Hadamard test estimates the real part of $\langle\psi|U|\psi\rangle$ from one ancilla measurement.

#### Mixed-state Hadamard-test quadratures

↑ **Parent:** [Hadamard test](#hadamard-test)

For the [Hadamard test](#hadamard-test) with a [density operator](#density-matrix) $\rho$ in the auxiliary register, the output control [qubit](quantum-mechanics.md#qubit) has [Pauli Z gate](#pauli-z-gate) expectation $\operatorname{Re}m$ and [Pauli Y gate](#pauli-y-gate) expectation $-\operatorname{Im}m$, where $m=\operatorname{Tr}(\rho U)$. The minus sign comes from the final [Hadamard gate](#hadamard-gate), since $HYH=-Y$. Measuring in $(|0\rangle\pm i|1\rangle)/\sqrt2$ therefore estimates the imaginary part using the minus-outcome frequency minus the plus-outcome frequency.

##### Trace estimation by a maximally mixed Hadamard test

↑ **Parent:** [Mixed-state Hadamard-test quadratures](#mixed-state-hadamard-test-quadratures)

Prepare the auxiliary register in the [maximally mixed state](#maximally-mixed-state) $I/N$ and estimate both [mixed-state Hadamard-test quadratures](#mixed-state-hadamard-test-quadratures). Multiplying the normalized expectation by $N$ estimates the [trace](linear-algebra.md#matrix-trace) of $U$. A uniformly randomized preparation of any orthonormal basis produces $I/N$; the eigenvectors of $U$ need not be known.

#### Eigenphase Hadamard-test probability

↑ **Parent:** [Hadamard test](#hadamard-test)

If $U|\psi\rangle=e^{2\pi i\theta}|\psi\rangle$, the ordinary Hadamard test returns ancilla zero with probability

$$
p_0=\frac{1+\cos(2\pi\theta)}2=\cos^2(\pi\theta).
$$

#### Imaginary-part Hadamard test

↑ **Parent:** [Hadamard test](#hadamard-test)

Adding a phase gate to the Hadamard test rotates the interference signal and measures the imaginary part of $\langle\psi|U|\psi\rangle$.

### Swap test

↑ **Parent:** [Controlled unitary gate](#controlled-unitary-gate)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Swap_test)

The swap test on pure states $|a\rangle,|b\rangle$ returns ancilla zero with probability

$$
p_0=\frac12\left(1+|\langle a|b\rangle|^2\right).
$$

## Parallel quantum gates

↑ **Parent:** [Quantum theory](quantum-theory.md)

Independent gates $A$ and $B$ on separate registers act jointly as $A\otimes B$.

## Measurement of a Pauli observable

↑ **Parent:** [Quantum theory](quantum-theory.md)

The expectation of a Hermitian Pauli string can be obtained by basis rotation and measurement, or by a Hadamard test with the Pauli string as its controlled unitary.

### Ancilla-assisted Pauli measurement

↑ **Parent:** [Measurement of a Pauli observable](#measurement-of-a-pauli-observable)

Prepare an ancilla in $|+\rangle$, use it to control a Hermitian Pauli operator $P$, apply a Hadamard gate, and measure the ancilla. Outcome $s$ applies the projector $[I+(-1)^sP]/2$ to the data register.

### Pauli-based computation

↑ **Parent:** [Measurement of a Pauli observable](#measurement-of-a-pauli-observable)

Pauli-based computation performs an adaptive sequence of commuting Pauli measurements on nonstabilizer resource states. Classical outcomes determine later measurements and the final output.

## Born rule for a product-basis measurement

↑ **Parent:** [Quantum theory](quantum-theory.md)

For a bipartite state $|\psi\rangle$, measurement outcome $(x_j,y_k)$ has probability $|\langle x_jy_k|\psi\rangle|^2$.

### Matching-outcome projector

↑ **Parent:** [Born rule for a product-basis measurement](#born-rule-for-a-product-basis-measurement)

For two labelled orthonormal bases, the event of equal labels is represented by $\sum_j|x_jy_j\rangle\langle x_jy_j|$.

### Product-state factorization of measurement probabilities

↑ **Parent:** [Born rule for a product-basis measurement](#born-rule-for-a-product-basis-measurement)

For a product state, probabilities of local measurement outcomes multiply.

## Maximally entangled state

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Maximally_entangled_state)

A bipartite pure state is maximally entangled when either reduced density matrix is maximally mixed.

### Generalized Bell basis

↑ **Parent:** [Maximally entangled state](#maximally-entangled-state)

For a [primitive root of unity](algebra.md#primitive-root-of-unity) $\omega=e^{2\pi i/n}$ and labels $r,s$ modulo $n$, the displayed $n^2$ [maximally entangled states](#maximally-entangled-state) form an orthonormal basis. Inner products equal $\delta_{ss'}n^{-1}\sum_j\omega^{j(r'-r)}=\delta_{ss'}\delta_{rr'}$, by the [geometric series](real-analysis.md#geometric-series). A nonprimitive root repeats phase labels and does not give a complete orthonormal basis.

#### Bell basis

↑ **Parent:** [Generalized Bell basis](#generalized-bell-basis)

The Bell basis is the two-qubit case of the [generalized Bell basis](#generalized-bell-basis). Its four vectors are the [Bell states](bell-state.md), and a [Bell-basis measurement](bell-state.md#bell-basis-measurement) projects onto them.

##### Bell-basis conversion circuit

↑ **Parent:** [Bell basis](#bell-basis)

Apply a [Hadamard gate](#hadamard-gate) to the first qubit, then a [controlled-NOT gate](#controlled-not-gate) from the first to the second. This maps a [computational-basis state](#computational-basis-state) $|ij\rangle$ to the [Bell state](bell-state.md) with phase bit $i$ and parity bit $j$. Its inverse uses the same gates in reverse order because each gate is self-inverse but they do not commute. Applying the forward sequence twice is not generally a decoding operation.

##### Bell parity and phase observables

↑ **Parent:** [Bell basis](#bell-basis)

The [Bell basis](#bell-basis) diagonalizes the commuting [Pauli operators](quantum-circuit.md#pauli-operator) $Z\otimes Z$ and $X\otimes X$. Two local anticommutations make the joint operators commute. Their signs encode parity and relative phase. The displayed projectors turn the signed eigenvalues into literal zero-or-one bit eigenvalues: even parity and plus phase have bit zero.

###### LOCC discrimination of four Bell states using two copies

↑ **Parent:** [Bell parity and phase observables](#bell-parity-and-phase-observables)

Two identical copies of an unknown [Bell state](bell-state.md) suffice for perfect identification by [LOCC](bell-state.md#local-operations-and-classical-communication). Alice and Bob each measure $Z$ on the first copy and $X$ on the second. Comparing their local signs supplies the eigenvalues of $Z\otimes Z$ and $X\otimes X$. These are respectively $(+,+)$ for $\Phi^+$, $(+,-)$ for $\Phi^-$, $(-,+)$ for $\Psi^+$, and $(-,-)$ for $\Psi^-$. Each parity is certain even though individual local outcomes are random. Different copies provide the two complementary measurements, so measuring the first copy does not erase the phase information needed on the second.

#### Generalized Bell state

↑ **Parent:** [Generalized Bell basis](#generalized-bell-basis)

A generalized Bell state is one member of a [generalized Bell basis](#generalized-bell-basis). Its [reduced density matrices](bell-state.md#reduced-density-matrix) are both $I/n$, so it is a [maximally entangled state](#maximally-entangled-state). For $n=2$ these are the four [Bell states](bell-state.md).

### Orthogonal-basis invariance of a real Bell state

↑ **Parent:** [Maximally entangled state](#maximally-entangled-state)

For real orthogonal $U$, the Bell state $2^{-1/2}\sum_j|jj\rangle$ is invariant under $U\otimes U$ because $UU^T=I$.

### Bell-state correlation in two real bases

↑ **Parent:** [Maximally entangled state](#maximally-entangled-state)

For the real Bell state, the joint amplitude in real basis vectors $x,y$ equals $\langle x|y\rangle/\sqrt2$.

<h2 id="shor-s-algorithm">Shor's algorithm</h2>

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Shor's_algorithm)

Shor's factoring algorithm uses quantum period finding to determine a modular order and then extracts factors classically with greatest common divisors.

### Candidate-denominator gcd post-processing

↑ **Parent:** [Shor's algorithm](#shor-s-algorithm)

After [continued-fraction recovery in quantum order finding](#continued-fraction-recovery-in-quantum-order-finding), an even candidate denominator $q$ can be used to try the displayed [greatest common divisors](number-theory.md#greatest-common-divisor). Return only a divisor strictly between one and $N$. If $q$ is the true even [multiplicative order](number-theory.md#multiplicative-order) with a nontrivial halfway power, success follows from [factor extraction from an even modular order](#factor-extraction-from-an-even-modular-order). A candidate that is not a period can occasionally still yield a factor; testing $a^q\equiv1$ before the gcds therefore changes single-run success probabilities. The output-factor check guarantees correctness in either convention.

### Factor extraction from an even modular order

↑ **Parent:** [Shor's algorithm](#shor-s-algorithm)

If $r$ is even, $a^r\equiv1\pmod N$, and $a^{r/2}\not\equiv-1\pmod N$, then $\gcd(a^{r/2}-1,N)$ is a nontrivial factor unless the order was not minimal.

#### Probability of a useful unit in Shor factorization

↑ **Parent:** [Factor extraction from an even modular order](#factor-extraction-from-an-even-modular-order)

For an odd integer $N$ having at least two distinct prime divisors, choose a uniform unit $a\bmod N$. The [Chinese remainder theorem for unit groups](mathematics.md#chinese-remainder-theorem-for-unit-groups) makes its odd-prime-power components independent cyclic groups. Failure of [factor extraction from an even modular order](#factor-extraction-from-an-even-modular-order) requires all components to have equal 2-primary order exponents. For any component each possible exponent has probability at most $1/2$, so conditioning on another component bounds failure by $1/2$. Excluding the identity unit only improves the success proportion.

### Quantum order finding

↑ **Parent:** [Shor's algorithm](#shor-s-algorithm)

Quantum order finding Fourier-transforms a superposition of arguments having the same modular-exponentiation value, producing peaks near multiples of the reciprocal period.

#### Modular multiplication eigenstates

↑ **Parent:** [Quantum order finding](#quantum-order-finding)

For $\gcd(x,n)=1$ and order $r$, multiplication by $x$ modulo $n$ is a [unitary operator](vector-space.md#unitary-operator). On the orbit of one it cyclically permutes $r$ basis states. The displayed orthonormal [eigenstates](quantum-mechanics.md#eigenstate) have [eigenvalues](linear-operator-theory.md#eigenvalue) $e^{2\pi is/r}$, and $|1\rangle=r^{-1/2}\sum_s|u_s\rangle$. Thus [quantum phase estimation](#quantum-phase-estimation) on this efficiently prepared state samples a uniform $s$ without knowing $r$. Controlled powers are implemented by [quantum modular exponentiation](#quantum-modular-exponentiation). Sufficient phase resolution allows [continued-fraction recovery in quantum order finding](#continued-fraction-recovery-in-quantum-order-finding); the reduced denominator equals $r$ only when $s$ is coprime to $r$.

#### Quantum Fourier sampling bound for order finding

↑ **Parent:** [Quantum order finding](#quantum-order-finding)

In [quantum order finding](#quantum-order-finding), a phase $s/r$ produces amplitude $Q^{-1}\sum_{x=0}^{Q-1}e^{2\pi ix(s/r-j/Q)}$ after an inverse [quantum Fourier transform](#quantum-fourier-transform). Its nearest grid point has probability at least $4/\pi^2$, by bounding the sine ratio of this [finite geometric Fourier amplitude](#finite-geometric-fourier-amplitude). The initial modular orbit state is an equal-weight superposition of the $r$ phase eigenstates, so the phase label is uniform.

#### Quantum modular exponentiation

↑ **Parent:** [Quantum order finding](#quantum-order-finding)

Quantum modular exponentiation is the [reversible computation](computer-science.md#reversible-computation) that maps

$$
|x\rangle|0\rangle\longmapsto|x\rangle|a^x\bmod N\rangle.
$$

It can be implemented in [polynomial time](computer-science.md#polynomial-time) in the bit lengths of $x$ and $N$ by [repeated squaring](number-theory.md#exponentiation-by-squaring) and controlled modular multiplication.

#### Fourier transform of a finite periodic comb

↑ **Parent:** [Quantum order finding](#quantum-order-finding)

The Fourier amplitude of equally spaced basis states is a finite geometric sum with peaks where the Fourier phase increment is nearly one.

##### Finite geometric Fourier amplitude

↑ **Parent:** [Fourier transform of a finite periodic comb](#fourier-transform-of-a-finite-periodic-comb)

For $A$ terms with phase ratio $q$, the amplitude factor is $(1-q^A)/(1-q)$, with limiting value $A$ when $q=1$.

#### Continued-fraction recovery in quantum order finding

↑ **Parent:** [Quantum order finding](#quantum-order-finding)

If a measured ratio approximates a reduced $k/r$ within $1/(2r^2)$, continued-fraction convergents recover the candidate denominator $r$.

##### Uniqueness of a rational approximation with bounded denominator

↑ **Parent:** [Continued-fraction recovery in quantum order finding](#continued-fraction-recovery-in-quantum-order-finding)

Two distinct reduced fractions with denominators below $N$ differ by more than $1/N^2$, so an interval of radius $1/(2N^2)$ contains at most one.

## Quantum information theory

↑ **Parent:** [Quantum theory](quantum-theory.md)

[This section is present in another page, follow this link to view it.](quantum-information-theory.md)

## Quantum decoherence

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_decoherence)

Quantum decoherence is the suppression of observable phase coherence when a system becomes entangled with unobserved environmental degrees of freedom. In a preferred basis, tracing out the environment damps off-diagonal entries of the system's [reduced density matrix](bell-state.md#reduced-density-matrix) while leaving the corresponding populations unchanged.

### Zurek spin-bath model

↑ **Parent:** [Quantum decoherence](#quantum-decoherence)

A device qubit couples diagonally to a finite bath of spins. Conditional bath states acquire opposite phase rotations, and their [conditional environment overlap](#conditional-environment-overlap) multiplies the device coherence. An initially aligned bath leaves the overlap's modulus at one. Initially equatorial spins yield $z_N(t)=\prod_k\cos(2g_kt)$. Global [unitary time evolution](quantum-mechanics.md#unitary-time-evolution) remains reversible, and a [finite spin-bath coherence recurrence](#finite-spin-bath-coherence-recurrence) prevents a strict zero long-time limit at finite bath size.

#### Random-coupling spin-bath decoherence

↑ **Parent:** [Zurek spin-bath model](#zurek-spin-bath-model)

Independent random couplings suppress typical coherence as the bath size increases. This conclusion concerns an ensemble or a specified large-bath limit, and must be distinguished from a pointwise long-time limit for one finite realization. [Ensemble spin-bath coherence](#ensemble-spin-bath-coherence) supplies exact mean and mean-square formulas for a uniform coupling distribution, while [short-time Gaussian spin-bath decoherence](#short-time-gaussian-spin-bath-decoherence) gives the initial decay scale.

##### Short-time Gaussian spin-bath decoherence

↑ **Parent:** [Random-coupling spin-bath decoherence](#random-coupling-spin-bath-decoherence)

For initially equatorial spins and uniform couplings on $[0,g_*]$, expand $\log\cos(2g_kt)=-2g_k^2t^2+O(g_k^4t^4)$. The [strong law of large numbers](convergence-of-random-variables.md#strong-law-of-large-numbers) then gives $\sum g_k^2\simeq Ng_*^2/3$. On the scale $t=O((g_*\sqrt N)^{-1})$, the total fourth-order remainder tends to zero, giving the Gaussian coherence envelope. This approximation concerns early times and does not remove [finite spin-bath coherence recurrence](#finite-spin-bath-coherence-recurrence).

##### Ensemble spin-bath coherence

↑ **Parent:** [Random-coupling spin-bath decoherence](#random-coupling-spin-bath-decoherence)

For independent uniform couplings on $[0,g_*]$ and equatorial initial bath spins,

$$
\mathbb E z_N(t)=\left[\frac{\sin(2g_*t)}{2g_*t}\right]^N,\qquad
\mathbb E|z_N(t)|^2=\left[\frac12+\frac{\sin(4g_*t)}{8g_*t}\right]^N.
$$

At fixed finite $N$, the mean tends to zero and the mean square tends to $2^{-N}$ as time grows. At any fixed nonzero time, the mean-square bracket is strictly below one; the [Markov inequality](probability-inequality.md#markov-inequality) proves coherence tends to zero in probability as $N$ grows. Individual finite realizations still exhibit [finite spin-bath coherence recurrence](#finite-spin-bath-coherence-recurrence).

#### Finite spin-bath coherence recurrence

↑ **Parent:** [Zurek spin-bath model](#zurek-spin-bath-model)

For any finite set of couplings in $z_N(t)=\prod_k\cos(2g_kt)$, the simultaneous [Dirichlet approximation theorem](number-theory.md#dirichlet-s-approximation-theorem) supplies arbitrarily late near-alignment of all phases, or an exact common period. Thus finite bath coherence does not tend to zero as time tends to infinity. This remains true for almost every realization of continuous random couplings; an ensemble mean can decay while each realization has recurrences.

### Decoherence factor

↑ **Parent:** [Quantum decoherence](#quantum-decoherence)

If a joint pure state is $\alpha|0\rangle|E_0\rangle+\beta|1\rangle|E_1\rangle$, the off-diagonal entry of the system's [reduced density matrix](bell-state.md#reduced-density-matrix) is multiplied by the environmental overlap $\langle E_1|E_0\rangle$. Independent repeated interactions multiply these overlaps.

#### Conditional environment overlap

↑ **Parent:** [Decoherence factor](#decoherence-factor)

For a pure state $a|0\rangle|E_0\rangle+b|1\rangle|E_1\rangle$ with normalized environment states, the upper-right device [reduced density matrix](bell-state.md#reduced-density-matrix) entry is $ab^*\langle E_1|E_0\rangle$. Distinguishability of the conditional environment states suppresses device coherence. States differing only by a global phase have unit-modulus overlap and do not cause [quantum decoherence](#quantum-decoherence).

##### Single-qubit interference with conditional environment states

↑ **Parent:** [Conditional environment overlap](#conditional-environment-overlap)

Prepare a [qubit](quantum-mechanics.md#qubit) in $|+\rangle$, apply a [phase gate](#phase-gate) $P(\phi)=\operatorname{diag}(1,e^{i\phi})$, and correlate its [computational basis](#computational-basis) states with normalized environment states $|e_0\rangle,|e_1\rangle$. Write $\langle e_0|e_1\rangle=ve^{i\alpha}$. After a final [Hadamard gate](#hadamard-gate), the environment amplitude accompanying output zero is $(|e_0\rangle+e^{i\phi}|e_1\rangle)/2$. Its squared [norm](functional-analysis.md#norm) is $P_0=[1+v\cos(\phi+\alpha)]/2$. Thus $v$ is the [interference visibility](optics.md#interferometric-visibility), while $\alpha$ shifts the fringe. This [quantum decoherence](#quantum-decoherence) map commutes with the [phase gate](#phase-gate), so placing it immediately before that gate gives the same probabilities.

### Quantum recoherence

↑ **Parent:** [Quantum decoherence](#quantum-decoherence)

Quantum recoherence is a later restoration of phase coherence. It can occur when a finite environment revisits a state having substantial overlap with its initial conditional state.

### Measurement problem

↑ **Parent:** [Quantum decoherence](#quantum-decoherence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Measurement_problem)

The quantum measurement problem asks how a unitary superposition of system and apparatus outcomes gives rise to one definite observed outcome. [Quantum decoherence](#quantum-decoherence) explains the suppression of interference between outcome branches, but by itself does not select one branch.

## Foundations of quantum mechanics

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Foundations_of_quantum_mechanics)

The foundations of quantum mechanics study the physical and conceptual status of quantum states, measurement, nonlocal correlations, and possible extensions of quantum theory.

<h3 id="einstein-podolsky-rosen-paradox">Einstein–Podolsky–Rosen paradox</h3>

↑ **Parent:** [Foundations of quantum mechanics](#foundations-of-quantum-mechanics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Einstein–Podolsky–Rosen_paradox)

The EPR argument uses correlations of an entangled state and a locality assumption to challenge the completeness of the quantum description. Its [Einstein–Podolsky–Rosen criterion of reality](#einstein-podolsky-rosen-criterion-of-reality) identifies quantities predictable with certainty without disturbing a distant system as elements of physical reality.

<h4 id="einstein-podolsky-rosen-criterion-of-reality">Einstein–Podolsky–Rosen criterion of reality</h4>

↑ **Parent:** [Einstein–Podolsky–Rosen paradox](#einstein-podolsky-rosen-paradox)

The Einstein–Podolsky–Rosen criterion says that if one can predict a physical quantity with certainty without disturbing the system, then there is an element of physical reality corresponding to that quantity.

### Superselection rule

↑ **Parent:** [Foundations of quantum mechanics](#foundations-of-quantum-mechanics)

A [superselection rule](#superselection-rule) partitions a representation into sectors between which the specified observable algebra has no matrix elements. Relative phases between vectors in different sectors cannot be detected by those observables, so a coherent vector spanning sectors and its sector-diagonal mixture define the same observable state. The restriction is relative to the observable algebra; it is not by itself a physical wave-function collapse. Infinite-system phases can yield disjoint representations and emergent superselection sectors even though each finite system permits global connecting operators.

### EPR criterion of reality

↑ **Parent:** [Foundations of quantum mechanics](#foundations-of-quantum-mechanics)

The certainty of a prediction made without disturbing the system is proposed as sufficient evidence that the predicted quantity corresponds to an element of physical reality. It motivates the discussion of completeness and locality in [foundations of quantum mechanics](#foundations-of-quantum-mechanics), but is distinct from the conditional factorization assumed by [local hidden-variable theory](#local-hidden-variable-theory).

### de Broglie-Bohm theory

↑ **Parent:** [Foundations of quantum mechanics](#foundations-of-quantum-mechanics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/De_Broglie–Bohm_theory)

A deterministic interpretation with a definite particle configuration guided by the [wavefunction](quantum-mechanics.md#wave-function). The latter obeys the [Time-dependent Schrödinger equation](physics.md#time-dependent-schrodinger-equation), while the particle follows the [guidance equation](#guidance-equation). A [Born rule](quantum-mechanics.md#born-rule) distribution of initial positions is preserved by [quantum equilibrium equivariance](#quantum-equilibrium-equivariance). The guidance law restricts admissible initial velocities, even when trajectories are rewritten as a second-order force equation.

#### Bohmian circulation of an angular-momentum eigenstate

↑ **Parent:** [de Broglie-Bohm theory](#de-broglie-bohm-theory)

For the [separation of a two-dimensional central-potential eigenstate](quantum-mechanics.md#separation-of-a-two-dimensional-central-potential-eigenstate), the [guidance equation](#guidance-equation) gives zero radial velocity and constant-radius circular motion, with circulation $2\pi\hbar k/m$. A real superposition of the degenerate $k$ and $-k$ [eigenstates](quantum-mechanics.md#eigenstate) has zero current away from nodes instead. The speed depends on the actual [wavefunction](quantum-mechanics.md#wave-function), not just its energy.

#### Quantum potential

↑ **Parent:** [de Broglie-Bohm theory](#de-broglie-bohm-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_potential)

The amplitude-dependent extra potential in the [Madelung equations](physics.md#madelung-equations). Taking the [gradient](calculus.md#gradient) of their phase equation and using the [guidance equation](#guidance-equation) yields $mD\mathbf v/Dt=-\nabla(V+Q)$, where $D/Dt$ is the [material derivative](continuum-mechanics.md#material-derivative). At [wavefunction](quantum-mechanics.md#wave-function) nodes this local expression may be singular.

#### Guidance equation

↑ **Parent:** [de Broglie-Bohm theory](#de-broglie-bohm-theory)

For a spinless particle without a magnetic vector potential, [Bohmian mechanics](#de-broglie-bohm-theory) sets $\dot{\mathbf X}=\hbar\nabla S/m$, where $S$ is the dimensionless [quantum phase](quantum-mechanics.md#quantum-phase). Equivalently the velocity is the [probability current](quantum-mechanics.md#probability-current) divided by the [probability density](quantum-mechanics.md#probability-density). This formula is local to nonzero [wavefunction](quantum-mechanics.md#wave-function) regions.

##### Quantum equilibrium equivariance

↑ **Parent:** [Guidance equation](#guidance-equation)

Both the ensemble position density transported by the [guidance equation](#guidance-equation) and the squared wave amplitude satisfy the same [probability continuity equation](quantum-mechanics.md#probability-continuity-equation). Subject to existence and uniqueness of that transport, an initial [Born rule](quantum-mechanics.md#born-rule) distribution stays a [Born rule](quantum-mechanics.md#born-rule) distribution. This is a preservation statement, not a derivation that every initial ensemble is already in equilibrium.

### Ontological model of a quantum system

↑ **Parent:** [Foundations of quantum mechanics](#foundations-of-quantum-mechanics)

An ontological model associates each [quantum state preparation](quantum-circuit.md#quantum-state-preparation) with a [probability distribution](probability-theory.md#probability-distribution) over underlying physical states $\lambda$. A [measurement in quantum mechanics](quantum-measurement.md)'s response probabilities depend on its specification and $\lambda$, sum to one, and reproduce the [Born rule](quantum-mechanics.md#born-rule) when averaged over the preparation distribution. The model need not assign deterministic outcomes. Overlap or disjointness of preparation measures defines the [psi-epistemic model](#psi-epistemic-model) versus [psi-ontic model](#psi-ontic-model) distinction.

#### Pusey-Barrett-Rudolph theorem

↑ **Parent:** [Ontological model of a quantum system](#ontological-model-of-a-quantum-system)

Under [preparation independence](#preparation-independence), an [ontological model of a quantum system](#ontological-model-of-a-quantum-system) reproducing exact quantum [measurement in quantum mechanics](quantum-measurement.md) probabilities cannot assign overlapping preparation measures to distinct [pure states](#pure-state). An exclusion [measurement in quantum mechanics](quantum-measurement.md) on independent copies makes every outcome impossible for one possible preparation; a common ontic region would require every response to vanish there. Thus the conclusion is a [psi-ontic model](#psi-ontic-model), not a blanket exclusion of hidden variables or all informational interpretations.

##### Tensor-power reduction of PBR overlap

↑ **Parent:** [Pusey-Barrett-Rudolph theorem](#pusey-barrett-rudolph-theorem)

If two pure [quantum states](quantum-mechanics.md#quantum-state) overlap by $(1/\sqrt2)^{1/n}$, their $n$-copy states have overlap $1/\sqrt2$. Each block spans an effective [qubit](quantum-mechanics.md#qubit), with [orthonormal basis](linear-algebra.md#orthonormal-basis) $e_0=\Psi_1$ and $e_1=\sqrt2\Psi_2-\Psi_1$. Applying the two-block [PBR exclusion measurement for zero and plus](#pbr-exclusion-measurement-for-zero-and-plus) uses $2n$ independently prepared copies. A common single-copy ontic overlap of positive mass remains positive under this finite tensor power.

##### PBR exclusion measurement for zero and plus

↑ **Parent:** [Pusey-Barrett-Rudolph theorem](#pusey-barrett-rudolph-theorem)

The product preparations $00,0+,+0,++$ are excluded respectively by the orthonormal vectors $(01+10)/\sqrt2$, $(00-01+10+11)/2$, $(00+01-10+11)/2$ and $(00-11)/\sqrt2$, written in the computational basis. Each vector has zero inner product with its labelled preparation. This [projective measurement](quantum-measurement.md#projective-measurement) gives [antidistinguishable quantum states](quantum-measurement.md#antidistinguishable-quantum-states) and drives the two-copy [PBR theorem](#pusey-barrett-rudolph-theorem) contradiction.

#### Preparation independence

↑ **Parent:** [Ontological model of a quantum system](#ontological-model-of-a-quantum-system)

Independently operated [quantum state preparations](quantum-circuit.md#quantum-state-preparation) are assumed to produce independent underlying physical states. Their joint preparation measure factors into the single-system measures. This ontic factorization is an additional assumption, not a consequence of operational independence alone. It turns a common single-system overlap of mass $\varepsilon$ into a common $n$-system overlap of mass $\varepsilon^n$ in the [PBR theorem](#pusey-barrett-rudolph-theorem).

#### Psi-epistemic model

↑ **Parent:** [Ontological model of a quantum system](#ontological-model-of-a-quantum-system)

An [ontological model of a quantum system](#ontological-model-of-a-quantum-system) is psi-epistemic if some pair of distinct [pure states](#pure-state) has preparation measures with nonzero overlap. The same physical state can then be compatible with either preparation. This precise measure-overlap definition is stronger than merely interpreting a [wave function](quantum-mechanics.md#wave-function) as information or a computational tool.

#### Psi-ontic model

↑ **Parent:** [Ontological model of a quantum system](#ontological-model-of-a-quantum-system)

An [ontological model of a quantum system](#ontological-model-of-a-quantum-system) is psi-ontic if distinct [pure states](#pure-state) have mutually singular preparation distributions. The physical state then determines which pure [quantum state](quantum-mechanics.md#quantum-state) was prepared, almost surely in the pairwise sense. Extra underlying variables may still exist. The [PBR theorem](#pusey-barrett-rudolph-theorem) establishes this conclusion under [preparation independence](#preparation-independence) and exact quantum predictions.

### Bell theorem

↑ **Parent:** [Foundations of quantum mechanics](#foundations-of-quantum-mechanics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bell_theorem)

Bell's theorem shows that no theory assigning outcomes through local hidden variables can reproduce every quantum correlation.

#### Bell inequality

↑ **Parent:** [Bell theorem](#bell-theorem)

A [Bell inequality](#bell-inequality) is a constraint on observable correlations satisfied by the specified class of local hidden-variable models. In finite-setting scenarios such constraints bound linear combinations of probabilities or expectation values. The [CHSH inequality](#chsh-inequality) is one example, following from Bell factorization, measurement independence and bounded outcomes. A violation rules out the conjunction of the assumptions defining that model class; it does not alone identify a unique false premise.

#### Chained modular Bell inequality

↑ **Parent:** [Bell theorem](#bell-theorem)

For outcomes in $\{0,\ldots,d-1\}$, let $[x]_d$ be their nonnegative modular representative. A [deterministic local hidden-variable model](#deterministic-local-hidden-variable-model) satisfies

$$
I_{N,d}=\sum_{j=1}^N\mathbb E\big([A_j-B_j]_d\big)+\sum_{j=1}^{N-1}\mathbb E\big([B_j-A_{j+1}]_d\big)+\mathbb E\big([B_N-A_1-1]_d\big)\geq d-1.
$$

The unreduced chain telescopes to $-1$, so its reduced nonnegative sum is at least $d-1$ for each assignment. For binary outcomes and two settings, it is a form of the [CHSH inequality](#chsh-inequality): $I_{2,2}=2-(E_{11}+E_{21}+E_{22}-E_{12})/2$.

##### Coplanar qubit realization of the chained Bell inequality

↑ **Parent:** [Chained modular Bell inequality](#chained-modular-bell-inequality)

On $|\Phi^+\rangle$, measure $\sigma_z\cos\theta+\sigma_x\sin\theta$, assigning [bit](information-theory.md#bit) $a$ to eigenvalue $(-1)^a$. Choose Alice's angles $2(i-1)\delta$ and Bob's angles $(2i-1)\delta$, with $\delta=\pi/(2N)$. The [Bell state](bell-state.md) correlation is $\cos(\theta-\phi)$. Each adjacent disagreement term and the last agreement term therefore has [probability](probability-theory.md#probability) $\sin^2(\pi/(4N))$. For $N\geq2$, their total violates the [chained modular Bell inequality](#chained-modular-bell-inequality) bound one, and it tends to zero as $N\to\infty$. At $N=1$ the value is exactly one.

// Target: probability-and-statistics.bigb

#### Local hidden-variable theory

↑ **Parent:** [Bell theorem](#bell-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Local_hidden-variable_theory)

A local hidden-variable theory assigns each party's outcome from a shared hidden state and that party's own setting, independently of the spacelike-separated setting chosen by the other party.

##### Setting-independent heralding preserves Bell locality

↑ **Parent:** [Local hidden-variable theory](#local-hidden-variable-theory)

If a successful preparation flag is fixed before freely selected [Bell inequality](#bell-inequality) settings, conditioning a [local hidden-variable theory](#local-hidden-variable-theory) on that flag only replaces its hidden-variable distribution by the conditional distribution. The later response functions remain local and the distribution is independent of the later settings, so the [CHSH inequality](#chsh-inequality) still holds. Setting-dependent rejection during the Bell measurements does not satisfy this argument.

##### Outcome independence

↑ **Parent:** [Local hidden-variable theory](#local-hidden-variable-theory)

[Outcome independence](#outcome-independence) requires $P(A,B\mid a,b,\lambda)=P(A\mid a,b,\lambda)P(B\mid a,b,\lambda)$. It says that, once settings and the proposed complete state are fixed, learning the distant outcome does not change the local outcome probability. Combining it with [parameter independence](#parameter-independence) gives Bell factorization. Entangled quantum states generally fail outcome independence even though their observable marginal distributions obey [quantum no-signalling](#quantum-no-signalling).

##### Bell local causality

↑ **Parent:** [Local hidden-variable theory](#local-hidden-variable-theory)

For spacelike-separated measurement regions, a sufficient specification $\lambda$ of their relevant past should screen each outcome from additional information in the other wing. In a two-setting experiment a Bell-local model has $P(A,B\mid a,b,\lambda)=P(A\mid a,\lambda)P(B\mid b,\lambda)$. Together with [measurement independence](#measurement-independence) and bounded outcomes, this implies the [CHSH inequality](#chsh-inequality). [Bell local causality](#bell-local-causality) is stronger than [quantum no-signalling](#quantum-no-signalling) and is not an assumption that every outcome was predetermined.

##### Deterministic local hidden-variable model

↑ **Parent:** [Local hidden-variable theory](#local-hidden-variable-theory)

A setting-independent hidden variable fixes responses for every measurement choice, and each response depends only on the local setting. Stochastic [local hidden-variable theories](#local-hidden-variable-theory) can be represented as mixtures of these assignments by including local random seeds in the hidden variable. Deterministic counterfactual assignments are the starting point of the [chained modular Bell inequality](#chained-modular-bell-inequality).

##### Outcome determinism

↑ **Parent:** [Local hidden-variable theory](#local-hidden-variable-theory)

Outcome determinism says that a complete hidden state and the measurement settings fix each measurement outcome with probability one.

##### Parameter independence

↑ **Parent:** [Local hidden-variable theory](#local-hidden-variable-theory)

Parameter independence says that, conditional on the complete hidden state, the probability distribution of one party's outcome is independent of the other party's measurement setting.

##### Measurement independence

↑ **Parent:** [Local hidden-variable theory](#local-hidden-variable-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Measurement_independence)

Measurement independence says that the distribution of the hidden state is independent of the measurement settings: $\rho(\lambda|a,b)=\rho(\lambda)$. Its failure is the measurement-dependence loophole in a [Bell test](#bell-theorem).

#### CHSH inequality

↑ **Parent:** [Bell theorem](#bell-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/CHSH_inequality)

For local outcomes $A_0,A_1,B_0,B_1\in\{-1,1\}$, the Clauser–Horne–Shimony–Holt inequality is

$$
|E(A_0B_0)+E(A_0B_1)+E(A_1B_0)-E(A_1B_1)|\leq2.
$$

An arbitrary no-signalling correlation can reach the algebraic maximum $4$, while quantum correlations are bounded by $2\sqrt2$.

##### CHSH optimum from the correlation tensor

↑ **Parent:** [CHSH inequality](#chsh-inequality)

For spin-projective measurements on a two-qubit state, let $\lambda_1\geq\lambda_2\geq\lambda_3$ be the [eigenvalues](linear-operator-theory.md#eigenvalue) of $T^TT$, where $T$ is its [Pauli correlation tensor](#pauli-correlation-tensor). Bob's sum and difference of unit axes are orthogonal and have lengths $2\cos\phi$ and $2\sin\phi$. Maximizing Alice's two axes aligns them with the corresponding images under $T$. Maximizing $\phi$ then gives $2\sqrt{\|T\mathbf u\|^2+\|T\mathbf v\|^2}$ for orthonormal $\mathbf u,\mathbf v$. The maximum of this quadratic-form sum is $\lambda_1+\lambda_2$, by diagonalizing $T^TT$ and selecting its top two [eigenvectors](linear-operator-theory.md#eigenvector). Thus the displayed expression is both an upper bound and attainable. The same maximum applies to the form with the sum of two absolute values, since local outcome signs can select their positive branches.

<h5 id="gisin-s-theorem">Gisin's theorem</h5>

↑ **Parent:** [CHSH inequality](#chsh-inequality)

Every entangled pure state of two qubits violates a [CHSH inequality](#chsh-inequality) for a suitable choice of local measurement axes. If its two [Schmidt coefficients](von-neumann-entropy.md#schmidt-coefficient) are $c_0,c_1>0$, the optimal construction already gives a value $2\sqrt{1+(2c_0c_1)^2}>2$.

###### CHSH axes for an entangled pure two-qubit state

↑ **Parent:** [Gisin's theorem](#gisin-s-theorem)

For the [Schmidt-basis Pauli correlation tensor](von-neumann-entropy.md#schmidt-basis-pauli-correlation-tensor), choose Alice's axes $\mathbf e_z,\mathbf e_x$ and Bob's $(\mathbf e_z\pm s\mathbf e_x)/\sqrt{1+s^2}$. The [CHSH inequality](#chsh-inequality) expression is $2\sqrt{1+s^2}$. It exceeds two exactly when both [Schmidt coefficients](von-neumann-entropy.md#schmidt-coefficient) are nonzero, reaching $2\sqrt2$ for maximal [quantum entanglement](bell-state.md#entangled-state). A [product state](bell-state.md#product-state) gives $s=0$ and saturates rather than violates the inequality.

##### No-signalling box

↑ **Parent:** [CHSH inequality](#chsh-inequality)

A no-signalling box is a conditional probability distribution $P(x,y|a,b)$ whose marginal distribution for either party is independent of the other party's input. It can therefore exhibit correlations stronger than quantum correlations without transmitting information superluminally.

<h6 id="popescu-rohrlich-box">Popescu–Rohrlich box</h6>

↑ **Parent:** [No-signalling box](#no-signalling-box)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Popescu–Rohrlich_box)

A Popescu–Rohrlich box is a bipartite no-signalling box attaining the algebraic maximum of the [CHSH inequality](#chsh-inequality).

<h6 id="one-bit-computation-using-popescu-rohrlich-boxes">One-bit computation using Popescu–Rohrlich boxes</h6>

↑ **Parent:** [Popescu–Rohrlich box](#popescu-rohrlich-box)

Take a [separated Boolean decomposition](combinatorics.md#separated-boolean-decomposition) $f(x,y)=\bigoplus_{\ell}u_\ell(x)v_\ell(y)$. Feed $(u_\ell,v_\ell)$ to one independent [PR box](#popescu-rohrlich-box), obtaining outputs with $a_\ell\oplus b_\ell=u_\ell v_\ell$. Alice forms $A=\bigoplus_\ell a_\ell$, Bob forms $B=\bigoplus_\ell b_\ell$, and their parities satisfy $A\oplus B=f$. Sending the single bit $A$ lets Bob compute the answer with certainty. The truth-table decomposition needs at most $2^{\min(m,n)}$ boxes for input lengths $m,n$. Each box's local output is uniform, so Bob's uncommunicated output string carries no information about Alice's input; the final parity bit is essential for a general function depending on that input.

### Objective-collapse theory

↑ **Parent:** [Foundations of quantum mechanics](#foundations-of-quantum-mechanics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Objective-collapse_theory)

An objective-collapse theory treats wave-function collapse as a physical process localized in spacetime, rather than only as an observer's update of information.

#### Ghirardi-Rimini-Weber theory

↑ **Parent:** [Objective-collapse theory](#objective-collapse-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ghirardi–Rimini–Weber_theory)

The Ghirardi--Rimini--Weber theory modifies [unitary time evolution](quantum-mechanics.md#unitary-time-evolution) by random Gaussian position localizations. Each constituent collapses at a small fixed rate, while the rate for an entangled macroscopic body grows with its number of constituents.

##### GRW localization operator

↑ **Parent:** [Ghirardi-Rimini-Weber theory](#ghirardi-rimini-weber-theory)

For localization length $r_C$, the GRW localization operator acting on particle $i$ is

$$
L_i(\mathbf X)=(\pi r_C^2)^{-3/4}
\exp\left[-\frac{(\mathbf q_i-\mathbf X)^2}{2r_C^2}\right].
$$

A collapse centred at $\mathbf X$ sends $|\psi\rangle$ to the normalized state $L_i(\mathbf X)|\psi\rangle$ with probability density $\|L_i(\mathbf X)|\psi\rangle\|^2$.

###### GRW collapse-centre event probabilities

↑ **Parent:** [GRW localization operator](#grw-localization-operator)

For equal particle rates in the [GRW model](#ghirardi-rimini-weber-theory), the next centre falls in $B$ with probability $N^{-1}\sum_i\int_B\|L_i(c)\Psi\|^2dc$. With zero [Hamiltonian operator](quantum-mechanics.md#hamiltonian-quantum-mechanics), two successive centres in $B$ have joint probability $N^{-2}\sum_{ij}\int_Bdc\int_Bdd\|L_j(d)L_i(c)\Psi\|^2$. Dividing by the first-event probability gives the conditional second event, including repeated particle labels. Spatial probabilities depend on actual packet mass, not solely the nominal packet centres.

##### GRW amplification mechanism

↑ **Parent:** [Ghirardi-Rimini-Weber theory](#ghirardi-rimini-weber-theory)

For $N$ entangled constituents, independent localization rates add to approximately $N\lambda$. One constituent's collapse localizes the correlated macroscopic configuration, rapidly suppressing macroscopically separated branches.

###### GRW branch persistence versus geometric containment

↑ **Parent:** [GRW amplification mechanism](#grw-amplification-mechanism)

A first localization near one macroscopically separated branch suppresses the other branch through the Gaussian [GRW localization operator](#grw-localization-operator). This selects a correlated pointer alternative. However, if a region contains only packet centres and excludes substantial packet mass, the next centre need not lie in that region's small enlargement. Probabilities $|\alpha|^2$ for the first event and approximately one for the next require regions containing essentially all corresponding branch mass. The general [GRW collapse-centre event probabilities](#grw-collapse-centre-event-probabilities) retain the geometry exactly.

##### GRW spontaneous heating

↑ **Parent:** [Ghirardi-Rimini-Weber theory](#ghirardi-rimini-weber-theory)

GRW position localization increases the ensemble mean momentum variance. In three dimensions one collapse adds $3\hbar^2/(2r_C^2)$ to $\langle\mathbf p^2\rangle$, producing mean kinetic-energy increase $3\hbar^2/(4mr_C^2)$.

#### Local quantum state under objective collapse

↑ **Parent:** [Objective-collapse theory](#objective-collapse-theory)

At a spacetime point $x$, the local quantum state is the reduced density operator obtained on spacelike hypersurfaces approaching the past light cone of $x$. It includes the effects of objective collapses in that past light cone and excludes spacelike-separated collapses.

##### Quantum state readout device

↑ **Parent:** [Local quantum state under objective collapse](#local-quantum-state-under-objective-collapse)

A quantum state readout device at $x$ hypothetically outputs a classical description of the [local quantum state under objective collapse](#local-quantum-state-under-objective-collapse) without changing that state. Its output can respond to a remote collapse only after the collapse enters the past light cone of $x$, so the device preserves [relativistic causality](special-relativity.md#relativistic-causality).

##### Proper mixed state

↑ **Parent:** [Local quantum state under objective collapse](#local-quantum-state-under-objective-collapse)

A proper mixed state represents classical uncertainty over states selected by an actual preparation or collapse. Once that selecting event lies in the readout point's past light cone, a [quantum state readout device](#quantum-state-readout-device) returns the selected component rather than merely the ensemble average.

##### Improper mixed state

↑ **Parent:** [Local quantum state under objective collapse](#local-quantum-state-under-objective-collapse)

An improper mixed state is the [reduced density matrix](bell-state.md#reduced-density-matrix) of a subsystem entangled with unobserved degrees of freedom. A [quantum state readout device](#quantum-state-readout-device) returns that reduced state until a relevant collapse lies in its past light cone.

## Quantum gravity

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_gravity)

Quantum gravity seeks a theory in which gravity and quantum phenomena are described consistently.

### Two-dimensional quantum gravity

↑ **Parent:** [Quantum gravity](#quantum-gravity)

Quantum gravity with a two-dimensional spacetime or worldsheet. In the string formulation, one sums over surface metrics and topologies with matter fields on each surface. This worldsheet theory is distinct from the target-space gravity described by the [graviton](#graviton) in the closed-string spectrum.

### Graviton

↑ **Parent:** [Quantum gravity](#quantum-gravity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Graviton)

A graviton is the massless spin-two quantum of the gravitational field. It occurs in the symmetric trace-free transverse sector of the first massless [closed string](string-theory.md#closed-string) level.

### Semiclassical gravity

↑ **Parent:** [Quantum gravity](#quantum-gravity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Semiclassical_gravity)

Semiclassical gravity couples a classical spacetime metric to quantum matter. In its simplest expectation-value form, the classical gravitational field is sourced by the quantum expectation of the matter [stress-energy tensor](general-relativity.md#stress-energy-tensor).

#### Semiclassical Einstein equation

↑ **Parent:** [Semiclassical gravity](#semiclassical-gravity)

The semiclassical Einstein equation is

$$
G_{\mu\nu}=8\pi G\,\langle T_{\mu\nu}\rangle
$$

in units with $c=1$. A single classical metric responds to the expectation value over all matter branches.

<h5 id="page-geilker-experiment">Page–Geilker experiment</h5>

↑ **Parent:** [Semiclassical Einstein equation](#semiclassical-einstein-equation)

The Page–Geilker experiment used a quantum random decision to choose a macroscopic source-mass configuration and measured its field with a torsion balance. The observed field followed the configuration in the observed branch rather than the nearly cancelling expectation-value average predicted by the simplest no-collapse [semiclassical Einstein equation](#semiclassical-einstein-equation).

[https://doi.org/10.1103/PhysRevLett.47.979](https://doi.org/10.1103/PhysRevLett.47.979)

### Gravitationally induced entanglement

↑ **Parent:** [Quantum gravity](#quantum-gravity)

When two masses occupy spatial superpositions, their branch-dependent [Newtonian gravitational potential energy](classical-mechanics.md#newtonian-gravitational-potential-energy) produces relative phases. If those phases cannot be separated into one phase for each mass, the interaction turns an initial [product state](bell-state.md#product-state) into an [entangled state](bell-state.md#entangled-state).

<h4 id="bose-marletto-vedral-experiment">Bose--Marletto--Vedral experiment</h4>

↑ **Parent:** [Gravitationally induced entanglement](#gravitationally-induced-entanglement)

The Bose--Marletto--Vedral experiment proposes placing two nearby masses in spatial superpositions and detecting the [entanglement](bell-state.md#entangled-state) generated by their branch-dependent gravitational phases. Under locality assumptions and in the absence of other interactions, an entangling mediator must possess incompatible observables rather than behave as a single classical local variable.

[https://arxiv.org/abs/1707.06050](https://arxiv.org/abs/1707.06050)

[https://arxiv.org/abs/1707.06036](https://arxiv.org/abs/1707.06036)

## Pure state

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pure_state)

A pure quantum state is represented by a unit vector $|\psi\rangle$ up to global phase, or equivalently by the rank-one [density operator](#density-matrix) $|\psi\rangle\langle\psi|$.

### Relative state of a bipartite vector

↑ **Parent:** [Pure state](#pure-state)

For a bipartite vector $|v\rangle\in\mathcal H_R\otimes\mathcal H_A$ and a chosen orthonormal basis of $R$, the generally unnormalized relative state on $A$ is obtained by the partial inner product with one basis vector. It gives the expansion $|v\rangle=\sum_j|j\rangle\otimes|\eta_j\rangle$. The squared norm of a relative state is the probability of its corresponding basis outcome when $|v\rangle$ is normalized. Relative states of eigenvectors of a [Choi matrix](quantum-information-theory.md#choi-matrix) construct the columns of its [Kraus operators](quantum-information-theory.md#kraus-operator).

#### Index state

↑ **Parent:** [Relative state of a bipartite vector](#relative-state-of-a-bipartite-vector)

An index state is a chosen orthonormal basis vector in the indexing subsystem of a [relative state](#relative-state-of-a-bipartite-vector) decomposition. It labels the corresponding partial inner product; it need not be an eigenvector of the subsystem's [reduced density matrix](bell-state.md#reduced-density-matrix).

##### Conjugate index vector

↑ **Parent:** [Index state](#index-state)

Fix paired orthonormal bases and let $|\phi\rangle_A=\sum_jc_j|j\rangle_A$. Its conjugate index vector in the other [Hilbert space](hilbert-space.md) uses the conjugated coefficients. For the unnormalized [maximally entangled state](#maximally-entangled-state) $|\widetilde\Psi\rangle=\sum_j|j\rangle_A|j\rangle_B$, the partial inner product is $(I\otimes\langle\phi_B^*|)|\widetilde\Psi\rangle=|\phi\rangle_A$. Both the conjugation and the lack of normalization of $\widetilde\Psi$ matter. Applying a [linear operator](vector-space.md#linear-operator) on the first subsystem gives the corresponding [relative state](#relative-state-of-a-bipartite-vector) of the operated vector.

## Partial trace

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Partial_trace)

The partial trace over $B$ is the linear operation characterized by

$$
\operatorname{Tr}[M_A\operatorname{Tr}_B(X_{AB})]
=\operatorname{Tr}[(M_A\otimes I_B)X_{AB}].
$$

Applied to a [density operator](#density-matrix), it produces a [reduced density matrix](bell-state.md#reduced-density-matrix).

### Partial trace positivity from product vectors

↑ **Parent:** [Partial trace](#partial-trace)

The [partial trace](#partial-trace) of a [positive operator](hilbert-space.md#positive-operator) is positive by this sum of nonnegative expectations in an orthonormal basis of the traced factor. Its trace equals the original trace, using the product orthonormal basis. Basis independence follows from $\operatorname{Tr}[(\operatorname{Tr}_B\rho)A]=\operatorname{Tr}[\rho(A\otimes I)]$, which uniquely determines the reduced operator. Thus reductions of [density matrices](#density-matrix) remain density matrices. For a positive trace-class operator the same argument uses convergent nonnegative basis sums.

### Haar twirling conditional expectation

↑ **Parent:** [Partial trace](#partial-trace)

For an operator on a tensor-product [Hilbert space](hilbert-space.md), averaging unitary conjugations on subsystem $B$ with normalized [Haar measure](measure-theory.md#haar-measure) gives $\mathcal E_A(O)=(\operatorname{Tr}_B O/d_B)\otimes I_B$. It fixes precisely the operators acting trivially on $B$ and is contractive in [operator norm](continuous-dual-space.md#operator-norm). Writing $O-UOU^\dagger=[O,U]U^\dagger$ converts localization error into a [commutator](lie-algebra.md#commutator) bound.

## Adiabatic theorem

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Adiabatic_theorem)

If a Hamiltonian changes sufficiently slowly while an eigenstate remains separated from the rest of the spectrum by a nonzero gap, evolution keeps the state in the corresponding instantaneous eigenspace up to a dynamical and geometric phase. A degenerate isolated eigenspace can undergo a unitary holonomy within itself.

### Adiabatic preparation of a computational history state

↑ **Parent:** [Adiabatic theorem](#adiabatic-theorem)

A Hamiltonian path preserving the history subspace can be analysed using its restricted [spectral gap](linear-operator-theory.md#spectral-gap). If this gap is $\Omega(T^{-2})$ and the derivative has [operator norm](continuous-dual-space.md#operator-norm) $O(1)$, a runtime criterion proportional to $\|\dot H\|^2/(\epsilon\Delta^3)$ permits [computational history state](quantum-circuit.md#computational-history-state) preparation in time $O(T^6/\epsilon)$. Other invariant sectors do not cause leakage from a state initialized in the history subspace.

## Topological quantum matter

↑ **Parent:** [Quantum theory](quantum-theory.md)

[This section is present in another page, follow this link to view it.](topological-quantum-matter.md)

## Quantum error correction

↑ **Parent:** [Quantum theory](quantum-theory.md)

[This section is present in another page, follow this link to view it.](quantum-error-correction.md)

## Tensor network state

↑ **Parent:** [Quantum theory](quantum-theory.md)

A tensor network state contracts auxiliary indices of local tensors to encode a many-body wavefunction.

### Matrix product state

↑ **Parent:** [Tensor network state](#tensor-network-state)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matrix_product_state)

A matrix product state represents one-dimensional amplitudes as products of finite matrices. Its bond dimension bounds the Schmidt rank across a cut.

#### Matrix product state as an unravelling of a completely positive map

↑ **Parent:** [Matrix product state](#matrix-product-state)

Matrices $A^i$ define both the completely positive map $\mathcal E(X)=\sum_iA^iX(A^i)^\dagger$ and an MPS. Repeatedly retaining the Kraus label $i$ purifies the channel output into the physical MPS chain; tracing those labels recovers repeated application of $\mathcal E$.

#### Matrix product state transfer map

↑ **Parent:** [Matrix product state](#matrix-product-state)

For an MPS tensor $A^i$, the transfer map is the [completely positive map](quantum-information-theory.md#completely-positive-map) $\mathcal E(X)=\sum_iA^iX(A^i)^\dagger$. Its fixed points control normalization and local expectation values, while its subleading eigenvalues control correlation lengths.

#### Injective matrix product state

↑ **Parent:** [Matrix product state](#matrix-product-state)

An MPS tensor is injective after blocking when products of its physical matrices span the full virtual matrix algebra.

##### Blocking a matrix product state

↑ **Parent:** [Injective matrix product state](#injective-matrix-product-state)

Blocking $L$ neighboring sites replaces their physical labels by one composite label and their tensor by the products $A^{i_1}\cdots A^{i_L}$. An MPS is injective when such products span the full virtual matrix algebra for some finite $L$.

##### Uniform matrix product state

↑ **Parent:** [Injective matrix product state](#injective-matrix-product-state)

A uniform matrix product state uses the same local tensor $A^i$ at every site. For a periodic chain its amplitudes are $\operatorname{Tr}(A^{i_1}\cdots A^{i_N})$.

##### Fundamental theorem of matrix product states

↑ **Parent:** [Injective matrix product state](#injective-matrix-product-state)

Two injective uniform MPS tensors generate the same states on every sufficiently long periodic chain exactly when they differ by a virtual similarity transform and an overall phase: $A^i=e^{i\theta}XB^iX^{-1}$.

###### Gauge equivalence of injective matrix product state tensors

↑ **Parent:** [Fundamental theorem of matrix product states](#fundamental-theorem-of-matrix-product-states)

The virtual [similarity transformation](linear-algebra.md#similarity-transformation) $A^i\mapsto XA^iX^{-1}$ leaves every periodic MPS amplitude invariant by cyclicity of the [matrix trace](linear-algebra.md#matrix-trace). The [fundamental theorem of matrix product states](#fundamental-theorem-of-matrix-product-states) says that, up to an overall phase, this is the only ambiguity for injective uniform tensors.

<h5 id="affleck-kennedy-lieb-tasaki-state">Affleck--Kennedy--Lieb--Tasaki state</h5>

↑ **Parent:** [Injective matrix product state](#injective-matrix-product-state)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Affleck--Kennedy--Lieb--Tasaki_state)

The Affleck--Kennedy--Lieb--Tasaki state is an injective spin-one MPS whose virtual degrees of freedom are spin one-half. Its $\mathbb Z_2\times\mathbb Z_2$ symmetry acts linearly on physical spins and projectively on the virtual spins.

<h6 id="pauli-matrix-representation-of-the-affleck-kennedy-lieb-tasaki-state">Pauli-matrix representation of the Affleck--Kennedy--Lieb--Tasaki state</h6>

↑ **Parent:** [Affleck--Kennedy--Lieb--Tasaki state](#affleck-kennedy-lieb-tasaki-state)

In a Cartesian basis of the physical spin-one space, the AKLT MPS matrices are proportional to $\sigma_x,\sigma_y,\sigma_z$. Products of two such matrices span the full virtual matrix algebra, and the two-site parent term projects onto total spin two.

<h6 id="two-site-support-of-the-pauli-matrix-affleck-kennedy-lieb-tasaki-tensor">Two-site support of the Pauli-matrix Affleck--Kennedy--Lieb--Tasaki tensor</h6>

↑ **Parent:** [Pauli-matrix representation of the Affleck--Kennedy--Lieb--Tasaki state](#pauli-matrix-representation-of-the-affleck-kennedy-lieb-tasaki-state)

Because $\sigma_i\sigma_j=\delta_{ij}I+i\varepsilon_{ijk}\sigma_k$, the two-site image of the Pauli-matrix AKLT tensor is the direct sum of the scalar and antisymmetric subspaces, which have total spin zero and one. Its orthogonal complement is the symmetric traceless total-spin-two subspace.

<h6 id="affleck-kennedy-lieb-tasaki-parent-hamiltonian">Affleck--Kennedy--Lieb--Tasaki parent Hamiltonian</h6>

↑ **Parent:** [Affleck--Kennedy--Lieb--Tasaki state](#affleck-kennedy-lieb-tasaki-state)

The AKLT parent Hamiltonian is $H=\sum_jP^{(2)}_{j,j+1}$, where $P^{(2)}$ projects two neighboring spin-one particles onto total spin two. It is [frustration free](#frustration-free-quantum-hamiltonian), and the periodic AKLT MPS is its unique ground state on a sufficiently long chain.

<h6 id="symmetry-protected-equivalence-of-the-affleck-kennedy-lieb-tasaki-state-and-cluster-state">Symmetry-protected equivalence of the Affleck--Kennedy--Lieb--Tasaki state and cluster state</h6>

↑ **Parent:** [Affleck--Kennedy--Lieb--Tasaki state](#affleck-kennedy-lieb-tasaki-state)

After suitable blocking, the AKLT and one-dimensional cluster states realize the same nontrivial $\mathbb Z_2\times\mathbb Z_2$ symmetry-protected topological phase. Their virtual symmetries carry the same nontrivial projective class and produce protected edge degrees of freedom.

#### Entanglement spectrum of a matrix product state

↑ **Parent:** [Matrix product state](#matrix-product-state)

The entanglement spectrum is the spectrum of $-\log\rho_A$, equivalently the negative logarithms of squared Schmidt coefficients. A nontrivial projective virtual symmetry can enforce degeneracies throughout this spectrum.

#### Parent Hamiltonian of a matrix product state

↑ **Parent:** [Matrix product state](#matrix-product-state)

An MPS parent Hamiltonian is a sum of local projectors onto the orthogonal complement of the tensor's local support. The MPS is a frustration-free ground state.

### Matrix product operator

↑ **Parent:** [Tensor network state](#tensor-network-state)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matrix_product_operator)

A matrix product operator contracts a one-dimensional chain of tensors with physical input and output indices.

### Projected entangled pair state

↑ **Parent:** [Tensor network state](#tensor-network-state)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Projected_entangled_pair_state)

A projected entangled pair state generalizes an MPS to higher-dimensional lattices. Cutting a region intersects one virtual bond per boundary edge.

### Projected entangled pair operator

↑ **Parent:** [Tensor network state](#tensor-network-state)

A projected entangled pair operator is a higher-dimensional tensor-network operator with physical input and output legs.

## Hamiltonian simulation

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hamiltonian_simulation)

Hamiltonian simulation constructs a [quantum circuit](quantum-circuit.md) approximating the time-evolution operator $e^{-itH}$ generated by a [Hamiltonian operator](quantum-mechanics.md#hamiltonian-quantum-mechanics) $H$, with cost controlled by the evolution time, requested precision, and structure of $H$.

### Commuting local Hamiltonian simulation

↑ **Parent:** [Hamiltonian simulation](#hamiltonian-simulation)

If $H=\sum_jh_j$ and all local terms commute, then

$$
e^{-itH}=\prod_je^{-ith_j}
$$

exactly. Approximating each fixed-size factor to error at most $\varepsilon/m$ and applying the [telescoping bound for products of operators](continuous-dual-space.md#telescoping-bound-for-products-of-operators) gives total [operator norm](continuous-dual-space.md#operator-norm) error at most $\varepsilon$.

### Local Hamiltonian

↑ **Parent:** [Hamiltonian simulation](#hamiltonian-simulation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Local_Hamiltonian)

A local Hamiltonian is a sum of terms, each acting nontrivially on only a bounded number of subsystems.

#### Operator support

↑ **Parent:** [Local Hamiltonian](#local-hamiltonian)

The [operator support](#operator-support) is the set of subsystems on which an operator may act nontrivially; it acts as the identity outside that set. [Unitary time evolution](quantum-mechanics.md#unitary-time-evolution) can enlarge the support, while a [Lieb-Robinson bound](#lieb-robinson-bound) controls the error of replacing the evolved operator by one with smaller support. The support diameter and the number of sites in the support are different quantities.

#### Stoquastic Hamiltonian

↑ **Parent:** [Local Hamiltonian](#local-hamiltonian)

A [stoquastic Hamiltonian](#stoquastic-hamiltonian) is a real Hermitian [Hamiltonian operator](quantum-mechanics.md#hamiltonian-quantum-mechanics) with nonpositive off-diagonal entries in a specified basis, usually the [computational basis](#computational-basis). The property depends on that basis. [Permutation matrices](vector-space.md#permutation-matrix) in a [quantum circuit](quantum-circuit.md)'s propagation terms and $|-\rangle\langle-|$ input penalties give a useful family of such operators.

#### Spectral filtering of Hamiltonian terms

↑ **Parent:** [Local Hamiltonian](#local-hamiltonian)

A real nonnegative normalized filter $w$ defines $g_Z=\int w(t)e^{itH}h_Ze^{-itH}\,dt$. In an energy [eigenbasis](linear-operator-theory.md#eigenbasis), it multiplies each matrix element by $\widehat w(E_i-E_j)$. A Fourier cutoff at the [spectral gap](linear-operator-theory.md#spectral-gap) removes couplings between a unique [ground state](quantum-mechanics.md#ground-state) and excitations. The filtered terms still sum to $H$, because the total Hamiltonian is unchanged by its own [unitary time evolution](quantum-mechanics.md#unitary-time-evolution). Each term commutes with the ground projector, but need not be minimized there.

##### Almost-exponential locality of filtered Hamiltonian terms

↑ **Parent:** [Spectral filtering of Hamiltonian terms](#spectral-filtering-of-hamiltonian-terms)

In a [telescoping local-shell decomposition](#telescoping-local-shell-decomposition), split the [spectral filter](inverse-problem.md#spectral-filter) integral at a time proportional to the shell distance. A [Lieb-Robinson bound](#lieb-robinson-bound) controls short times, while the two-sided almost-exponential [spectral filter](inverse-problem.md#spectral-filter) tail controls long times. Polynomial shell-weight growth then gives the displayed decay. The estimate is asymptotic at large distance; small shells retain the elementary operator-norm bound. The [evenization of a nonnegative bandlimited filter](inverse-problem.md#evenization-of-a-nonnegative-bandlimited-filter) can supply the two-sided tail from a one-sided existence statement.

##### Filtering preserves existing frustration freeness

↑ **Parent:** [Spectral filtering of Hamiltonian terms](#spectral-filtering-of-hamiltonian-terms)

If each local term is already minimized by the global [ground state](quantum-mechanics.md#ground-state), subtract its minimum $a_Z$ to obtain a [positive operator](hilbert-space.md#positive-operator). Nonnegative normalized [spectral filtering of Hamiltonian terms](#spectral-filtering-of-hamiltonian-terms) preserves positivity and leaves the ground eigenvalue $a_Z$ unchanged. Thus the same state minimizes every filtered term. This preserves [frustration freeness](#frustration-freeness) but does not create it for an initially frustrated decomposition.

##### Commuting with a ground projector does not imply frustration freeness

↑ **Parent:** [Spectral filtering of Hamiltonian terms](#spectral-filtering-of-hamiltonian-terms)

The condition $[g_Z,P_0]=0$ makes a unique global [ground state](quantum-mechanics.md#ground-state) an [eigenvector](linear-operator-theory.md#eigenvector) of every filtered term, but its termwise eigenvalues can exceed the corresponding minima. For example $h_{12}=|1\rangle\langle1|_1+|0\rangle\langle0|_2$ and $h_{23}=|1\rangle\langle1|_3+2|1\rangle\langle1|_2$ commute with their sum. Their sum is uniquely minimized by $|000\rangle$, yet $h_{12}$ is lower on $|010\rangle$. Filtering leaves these commuting terms unchanged, so it cannot force [frustration freeness](#frustration-freeness).

##### Telescoping local-shell decomposition

↑ **Parent:** [Spectral filtering of Hamiltonian terms](#spectral-filtering-of-hamiltonian-terms)

Filter a fixed local term using a nested sequence of neighbourhood Hamiltonians $H_s$, and call the results $G_s$. The differences $G_s-G_{s-1}$ give a shell decomposition. When $H_0=h_Z$ and $H_D=H$, normalization gives $G_0=h_Z$ and telescoping gives $g_Z=h_Z+\sum_{s=1}^D(G_s-G_{s-1})$. Individual shell terms need not commute with the full ground projector.

#### Local Hamiltonian problem

↑ **Parent:** [Local Hamiltonian](#local-hamiltonian)

Given a polynomial list of fixed-locality Hermitian terms and thresholds $a<b$ separated by at least an inverse polynomial, distinguish whether the minimum [eigenvalue](linear-operator-theory.md#eigenvalue) of their sum is at most $a$ or at least $b$. Terms may be normalized to $0\leq h_j\leq I$ with polynomial rescaling. This [promise problem](computer-science.md#promise-problem) is in [QMA](computer-science.md#qma) by [local-energy measurement verification](#local-energy-measurement-verification).

##### Local-energy measurement verification

↑ **Parent:** [Local Hamiltonian problem](#local-hamiltonian-problem)

Uniformly sample one positive local term and measure the effect $h_j$. The averaged energy-flag effect on a witness is $H/M$, where $M$ is the number of terms. Repetition with a threshold halfway between the promised flag probabilities uses $O(M^2/(b-a)^2)$ witness registers for constant error. A spectral tensor-product analysis, as in [QMA parallel repetition with entangled witnesses](computer-science.md#qma-parallel-repetition-with-entangled-witnesses), proves soundness against entangled witnesses. Constant-locality [positive operator-valued measures](quantum-measurement.md#positive-operator-valued-measure) are efficiently implementable using one [ancilla qubit](quantum-information-theory.md#ancilla-qubit).

#### Diagonal Hamiltonian

↑ **Parent:** [Local Hamiltonian](#local-hamiltonian)

A diagonal Hamiltonian is diagonal in a specified product basis, usually the computational basis. Every basis state is therefore an [energy eigenstate](quantum-mechanics.md#energy-eigenstate), and optimization of its diagonal entries becomes minimization of the corresponding classical cost function.

#### Frustration-free quantum Hamiltonian

↑ **Parent:** [Local Hamiltonian](#local-hamiltonian)

A quantum Hamiltonian $H=\sum_jh_j$ with positive-semidefinite local terms is frustration free when one state minimizes every $h_j$ simultaneously. After shifting each local minimum to zero, that state lies in every kernel $\ker h_j$ and has zero total energy.

##### Detectability lemma

↑ **Parent:** [Frustration-free quantum Hamiltonian](#frustration-free-quantum-hamiltonian)

In a nearest-neighbour [frustration-free Hamiltonian](#frustration-free-quantum-hamiltonian) chain, multiply the bond [orthogonal projections](hilbert-space.md#orthogonal-projection) in two disjoint alternating layers. The resulting product $K$ fixes the common [ground state](quantum-mechanics.md#ground-state) space but contracts its orthogonal complement by a factor bounded away from one in terms of the [spectral gap](linear-operator-theory.md#spectral-gap). A bound $\|K|_{\operatorname{supp}H}\|\leq(1+\Delta/2)^{-1/3}$ implies exponentially convergent powers. The product is generally neither Hermitian nor normal.

###### Local projector cone in a frustration-free chain

↑ **Parent:** [Detectability lemma](#detectability-lemma)

To evaluate a layered product on $A_x|\psi_0\rangle$, scan the bond [orthogonal projections](hilbert-space.md#orthogonal-projection) from right to left. A projection disjoint from the current support commutes through the accumulated operator and disappears against the common [ground state](quantum-mechanics.md#ground-state). Retained projections expand the support by at most one site per layer. Their product $L$ gives a local operator $LA_x$ with both $K^rA_x|\psi_0\rangle=LA_x|\psi_0\rangle$ and $\langle\psi_0|LA_x=\langle\psi_0|A_x$.

###### Exponential clustering from layered projectors

↑ **Parent:** [Local projector cone in a frustration-free chain](#local-projector-cone-in-a-frustration-free-chain)

Combine a [local projector cone in a frustration-free chain](#local-projector-cone-in-a-frustration-free-chain) with the contraction bound from the [detectability lemma](#detectability-lemma). If the localized operator misses a second observable's support, their commutation and the exact ground-state bra identity convert the [connected correlation function](critical-phenomenon.md#connected-correlation-function) into an approximation error. The two-projection power estimate yields spatial decay rate $\alpha=\frac13\ln(1+\Delta/2)$ for the stated detectability contraction.

##### Frustration freeness

↑ **Parent:** [Frustration-free quantum Hamiltonian](#frustration-free-quantum-hamiltonian)

A decomposition $H=\sum_Zh_Z$ has [frustration freeness](#frustration-freeness) when a global [ground state](quantum-mechanics.md#ground-state) minimizes every term simultaneously. For finite-dimensional Hermitian terms this implies $E_0(H)=\sum_ZE_0(h_Z)$. Shifting each term by its minimum produces [positive operators](hilbert-space.md#positive-operator) with a common null vector. The property depends on the decomposition, not only the total operator.

#### k-local Hamiltonian

↑ **Parent:** [Local Hamiltonian](#local-hamiltonian)

A $k$-local Hamiltonian is a sum of terms that each act nontrivially on at most $k$ subsystems. The integer $k$ remains fixed as the system size grows.

### Product-formula Hamiltonian simulation

↑ **Parent:** [Hamiltonian simulation](#hamiltonian-simulation)

Product-formula Hamiltonian simulation approximates $e^{-it(A+B)}$ by alternating exponentials of $A$ and $B$, which are assumed easier to implement separately.

#### First-order two-local Hamiltonian simulation

↑ **Parent:** [Product-formula Hamiltonian simulation](#product-formula-hamiltonian-simulation)

For a sum of $M$ Hermitian two-local terms of norm below one, repeat a first-order [Lie-Trotter product formula](numerical-analysis.md#lie-product-formula) step $r$ times. The [first-order unitary product-formula error bound](numerical-analysis.md#first-order-unitary-product-formula-error-bound) gives total error at most $t^2\sum_{j<k}\|[H_j,H_k]\|/(2r)<M(M-1)t^2/(2r)$ for $M>1$. Taking $r=\max(1,\lceil M(M-1)t^2/(2\epsilon)\rceil)$ uses $Mr$ arbitrary two-qubit gates. At unit time and $M=O(n^2)$ this is a sufficient $O(n^6/\epsilon)$ bound; additional commutation structure can improve it.

#### Second-order product formula

↑ **Parent:** [Product-formula Hamiltonian simulation](#product-formula-hamiltonian-simulation)

The symmetric second-order formula, also called Strang splitting, is

$$
e^{-i\delta A/2}e^{-i\delta B}e^{-i\delta A/2}
=e^{-i\delta(A+B)}+O(\delta^3)
$$

for bounded operators, with the constant controlled by nested [commutators](lie-algebra.md#commutator).

### Simulation of a computable diagonal Hamiltonian

↑ **Parent:** [Hamiltonian simulation](#hamiltonian-simulation)

Let $A|x\rangle=a(x)|x\rangle$, where a [reversible circuit](computer-science.md#reversible-circuit) $C$ computes $a(x)$ into a clean register. Then applying $e^{-ita(x)}$ as a phase on that register and performing [uncomputation](#uncomputation) implements $e^{-itA}$ on the data register. For $a(x)=(-1)^{f(x)}$, a Boolean output qubit suffices: $C^\dagger(I\otimes e^{-itZ})C$ acts as $e^{-itA}$ when that qubit starts in $|0\rangle$. This exact construction avoids a [Lie-Trotter product formula](numerical-analysis.md#lie-product-formula) because the eigenvalue is computed directly.

#### Pauli-string phase by parity computation

↑ **Parent:** [Simulation of a computable diagonal Hamiltonian](#simulation-of-a-computable-diagonal-hamiltonian)

The [Pauli Z gates](#pauli-z-gate) give [eigenvalue](linear-operator-theory.md#eigenvalue) $(-1)^{\sum_jx_j}$ on $|x\rangle$. Use [parity computation by CNOT gates](coding-theory.md#parity-computation-by-cnot-gates) to put the [parity bit](coding-theory.md#parity-bit) in a zero ancilla, apply $e^{itZ}$ to it, and uncompute. The data acquire exactly $e^{it(-1)^{\sum_jx_j}}$, and the ancillary line returns to zero. This [compute-phase-uncompute construction](#compute-phase-uncompute-construction) needs $2n+1$ one- and [two-qubit gates](quantum-circuit.md#two-qubit-gate). Accumulating parity into the last data line instead uses $2n-1$ gates without an extra ancilla. Neither implementation drops the global phase.

## Block encoding

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Block_encoding)

A block encoding of a matrix $A$ is a [unitary operator](vector-space.md#unitary-operator) whose designated block equals $A/\alpha$ for a known normalization factor $\alpha$. It gives a quantum circuit coherent access to matrices that need not themselves be unitary.

## ↑ Ancestors (3)

1. [Branches of physics](physics.md#branches-of-physics)
2. [Physics](physics.md)
3. [Codex Wiki](README.md)

## ← Incoming links (5)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-54.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-58.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-59.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-59.md#5/solution)
- [Quantum field theory](quantum-field-theory.md)
