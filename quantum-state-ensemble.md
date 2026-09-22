# Quantum state ensemble

↑ **Parent:** [Density matrix](density-matrix.md)

A quantum state ensemble specifies a random preparation: normalized [pure states](pure-state.md) $|\psi_i\rangle$ are selected with [probabilities](probability.md) $p_i\geq0$, $\sum_i p_i=1$. Without an accessible preparation label, its measurement statistics are those of the [density operator](density-matrix.md) $\rho=\sum_i p_i|\psi_i\rangle\langle\psi_i|$. Indeed every [POVM](positive-operator-valued-measure.md) effect $E$ has probability $\sum_i p_i\langle\psi_i|E|\psi_i\rangle=\operatorname{Tr}(E\rho)$. Different ensembles can therefore have identical operational statistics: equal mixtures of computational-basis qubits or Hadamard-basis qubits both have density operator $I/2$. The ensemble decomposition contains information about the preparation, not additional information accessible from the system alone.

**Table of contents**

- [Convex roof extension](convex-roof-extension.md)
  - [Monotonicity of a convex roof under a quantum instrument](monotonicity-of-a-convex-roof-under-a-quantum-instrument.md)

## ↑ Ancestors (5)

1. [Density matrix](density-matrix.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Average pure-source fidelity after typical projection](average-pure-source-fidelity-after-typical-projection.md)
- [Ensemble-steering attack on quantum bit commitment](ensemble-steering-attack-on-quantum-bit-commitment.md)
- [Isometry parametrization of a density-matrix ensemble](isometry-parametrization-of-a-density-matrix-ensemble.md)
- [Memoryless quantum information source](memoryless-quantum-information-source.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-54/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-59/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-34/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-58/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-60/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-53/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-51/2/b/solution.md)
- [POVM–ensemble duality for the maximally mixed state](povm-ensemble-duality-for-the-maximally-mixed-state.md)
