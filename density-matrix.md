# Density matrix

↑ **Parent:** [Quantum theory](quantum-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Density_matrix)

A finite-dimensional [density operator](density-matrix.md) $\rho$ represents a [quantum state](quantum-state.md) on a [Hilbert space](hilbert-space-split.md). It is [Hermitian](hermitian-operator.md), [positive semidefinite](positive-semidefinite-matrix.md), and has [trace](matrix-trace.md) one:

$$
\rho=\rho^\dagger,\qquad \langle v|\rho|v\rangle\geq0\text{ for every }|v\rangle,\qquad \operatorname{Tr}\rho=1.
$$

The [density matrix](density-matrix.md) is its [matrix](matrix.md) in a chosen [orthonormal basis](orthonormal-basis.md). In [dimension](dimension-vector-space.md) $N$ it has $N^2-1$ real parameters: a [Hermitian matrix](hermitian-operator.md) has $N^2$, and fixing its [trace](matrix-trace.md) removes one; positivity restricts the allowed values.

A [quantum state ensemble](quantum-state-ensemble.md) of normalized [pure states](pure-state.md) $|\psi_i\rangle$ with positive [probabilities](probability.md) $p_i$ gives

$$
\rho=\sum_i p_i|\psi_i\rangle\langle\psi_i|,\qquad p_i>0,\qquad \sum_i p_i=1.
$$

Zero-weight terms can be omitted. Conversely, the [spectral theorem](spectral-theorem.md) gives such an ensemble for every [density operator](density-matrix.md), using its [orthonormal](orthonormal-set.md) [eigenvectors](eigenvector.md) and nonnegative [eigenvalues](eigenvalue.md), with zero [eigenvalues](eigenvalue.md) omitted. A [pure state](pure-state.md) has $\rho=|\psi\rangle\langle\psi|$; a [mixed state](mixed-state.md) needs at least two nonzero [eigenvalues](eigenvalue.md). [Watrous, The Theory of Quantum Information, chapter 2, section 2.1.2, pp. 62–64](https://cs.uwaterloo.ca/~watrous/TQI/TQI.2.pdf)

For a [projective measurement](projective-measurement.md) with [orthogonal projections](orthogonal-projection.md) $\Pi_a$, the [Born rule](born-rule.md) is

$$
P(a)=\operatorname{Tr}(\rho\Pi_a)=\sum_i p_i\langle\psi_i|\Pi_a|\psi_i\rangle.
$$

This is the average of the component [pure state](pure-state.md) [probabilities](probability.md). Positivity makes each outcome [probability](probability.md) nonnegative, and $\sum_a\Pi_a=I$ makes them sum to one. The same [density operator](density-matrix.md) therefore predicts every measurement on the system without requiring a unique preparation history. [Preskill, Physics 229 notes, chapter 2, section 2.3.1, equations (2.51)–(2.59)](https://www.preskill.caltech.edu/ph229/notes/chap2.pdf)

For a closed system, [Schrödinger picture](schrodinger-picture.md) evolution under a [unitary operator](unitary-operator.md) is

$$
\rho_S(t)=U(t)\rho_HU(t)^\dagger
$$

when $\rho_H=\rho_S(0)$ denotes the time-independent [Heisenberg picture](heisenberg-picture.md) state and $U(0)=I$. In the [Schrödinger picture](schrodinger-picture.md) the [density operator](density-matrix.md) evolves; in the [Heisenberg picture](heisenberg-picture.md) the [observables](observable.md) evolve instead, with identical measurement predictions. This [unitary operator](unitary-operator.md) preserves the [eigenvalues](eigenvalue.md) and hence the [purity of a density operator](purity-of-a-density-operator.md). [Preskill, Physics 229 notes, chapter 2, section 2.3.4, equation (2.79)](https://www.preskill.caltech.edu/ph229/notes/chap2.pdf)

A historical source for the probabilistic formulation of [quantum mechanics](quantum-mechanics-split.md) is von Neumann's 1927 paper Wahrscheinlichkeitstheoretischer Aufbau der Quantenmechanik. [von Neumann, Nachrichten von der Gesellschaft der Wissenschaften zu Göttingen, Mathematisch-Physikalische Klasse, 1927, pp. 245–272](https://geodesic.mathdoc.fr/item/NGWGMP_1927__1927_59230/)

**Table of contents**

- [Quantum state population](quantum-state-population.md)
- [Quantum coherence in a specified basis](quantum-coherence-in-a-specified-basis.md)
- [Two-qubit Werner state](two-qubit-werner-state.md)
  - [Single-copy Werner filtering normalization bound](single-copy-werner-filtering-normalization-bound.md)
    - [Single-copy Werner filtering cannot increase concurrence](single-copy-werner-filtering-cannot-increase-concurrence.md)
  - [Concurrence of a two-qubit Werner state](concurrence-of-a-two-qubit-werner-state.md)
  - [Bell twirling followed by triplet symmetrization](bell-twirling-followed-by-triplet-symmetrization.md)
- [Extreme points of the density-operator state space](extreme-points-of-the-density-operator-state-space.md)
- [Unitary orbit of a density operator](unitary-orbit-of-a-density-operator.md)
- [Quantum state ensemble](quantum-state-ensemble.md)
  - [Convex roof extension](convex-roof-extension.md)
    - [Monotonicity of a convex roof under a quantum instrument](monotonicity-of-a-convex-roof-under-a-quantum-instrument.md)
- [Pauli correlation tensor](pauli-correlation-tensor.md)
- [Maximally mixed state](maximally-mixed-state.md)
  - [Obstruction to uniform probability lowering by a unitary](obstruction-to-uniform-probability-lowering-by-a-unitary.md)
- [Mixed state](mixed-state.md)
- [Von Neumann equation](von-neumann-equation.md)
- [Purification of a density operator](purification-of-a-density-operator.md)
  - [Purity decouples a subsystem from its purification](purity-decouples-a-subsystem-from-its-purification.md)
  - [Flagged purification of a quantum ensemble](flagged-purification-of-a-quantum-ensemble.md)
  - [Unitary freedom of purification](unitary-freedom-of-purification.md)
  - [Hughston–Jozsa–Wootters theorem](hughston-jozsa-wootters-theorem.md)
    - [Isometry parametrization of a density-matrix ensemble](isometry-parametrization-of-a-density-matrix-ensemble.md)
  - [Uhlmann's theorem](uhlmann-s-theorem.md)
- [Trace distance](trace-distance.md)
  - [Trace distance between qubit states](trace-distance-between-qubit-states.md)
  - [Trace-distance contraction under quantum channels](trace-distance-contraction-under-quantum-channels.md)
  - [Trace distance for qubit dephasing](trace-distance-for-qubit-dephasing.md)
  - [Pure-target upper bound on trace distance](pure-target-upper-bound-on-trace-distance.md)
  - [Spectral-parts formula for trace distance](spectral-parts-formula-for-trace-distance.md)
  - [Pure-target lower bound on trace distance](pure-target-lower-bound-on-trace-distance.md)
  - [Variational characterization of trace distance](variational-characterization-of-trace-distance.md)
    - [Trace-distance-preserving binary measurement](trace-distance-preserving-binary-measurement.md)
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
- [Purity of a density operator](purity-of-a-density-operator.md)
- [Reduced density operator of a weakly coupled oscillator pair](reduced-density-operator-of-a-weakly-coupled-oscillator-pair.md)
- [Bloch vector](bloch-vector.md)
  - [Bloch ball](bloch-ball.md)
    - [Antipodal eigenprojectors of a qubit density matrix](antipodal-eigenprojectors-of-a-qubit-density-matrix.md)
  - [Generalized Bloch representation](generalized-bloch-representation.md)
    - [Hamiltonian rotations of Bloch vectors](hamiltonian-rotations-of-bloch-vectors.md)
    - [Purity bound for generalized Bloch vectors](purity-bound-for-generalized-bloch-vectors.md)
    - [Affine Bloch equation](affine-bloch-equation.md)
      - [Transverse relaxation](transverse-relaxation.md)
      - [Population relaxation](population-relaxation.md)
      - [Steady states of an affine Bloch equation](steady-states-of-an-affine-bloch-equation.md)
  - [Bloch sphere](bloch-sphere.md)
    - [Pure-qubit overlap identity](pure-qubit-overlap-identity.md)
    - [Uniform pure-qubit average](uniform-pure-qubit-average.md)
  - [Informationally complete three-observable qubit tomography](informationally-complete-three-observable-qubit-tomography.md)

## ↑ Ancestors (4)

1. [Quantum theory](quantum-theory-split.md)
2. [Branches of physics](branches-of-physics.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (44)

- [Antipodal eigenprojectors of a qubit density matrix](antipodal-eigenprojectors-of-a-qubit-density-matrix.md)
- [Born rule](born-rule.md)
- [Canonical ensemble](canonical-ensemble.md)
- [Density matrix](density-matrix.md)
- [Dephasing channel](dephasing-channel.md)
- [Expectation value](expectation-value.md)
- [Hadamard gate](hadamard-gate.md)
- [Interferometric polarization tomography](interferometric-polarization-tomography.md)
- [Partial trace positivity from product vectors](partial-trace-positivity-from-product-vectors.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-25/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-25/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-35/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-35/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-32/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-32/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-32/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-32/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-32/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-58/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-58/1/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-58/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-58/4/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-59/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-33/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-58/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-58/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-58/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-59/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-60/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-59/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-58/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-60/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-60/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-53/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-53/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-53/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-53/4/a/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-53/4/b/protocol-2/solution.md)
- [Photon polarization](photon-polarization.md)
- [Pure-qubit overlap identity](pure-qubit-overlap-identity.md)
- [Quantum superposition](quantum-superposition.md)
- [Quantum theory](quantum-theory-split.md)
- [Qubit](qubit.md)
- [Qubit state](qubit-state.md)
