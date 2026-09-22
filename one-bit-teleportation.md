# One-bit teleportation

↑ **Parent:** [Quantum teleportation](quantum-teleportation.md)

Apply a [Controlled-Z gate](controlled-z-gate.md) to input $a|0\rangle+b|1\rangle$ and a fresh $|+\rangle$ [quantum ancilla](quantum-ancilla.md). Measuring the input in the [equatorial qubit measurement](equatorial-qubit-measurement.md) basis at angle $\alpha$, with outcome $s$, leaves the unnormalized output

$$
\frac1{\sqrt2}\left(a|+\rangle+(-1)^se^{i\alpha}b|-\rangle\right)=\frac1{\sqrt2}X^sJ(\alpha)|\psi\rangle.
$$

Each branch has [probability](probability.md) $1/2$, independently of the input. The logical output is $J(\alpha)|\psi\rangle$ with known [Pauli frame](pauli-frame.md) $X^s$; the input [qubit](qubit.md) has been measured, so this does not clone it.

**Table of contents**

- [Pauli-frame propagation along a measurement wire](pauli-frame-propagation-along-a-measurement-wire.md)
- [Graph-state preparation of a computational-basis input](graph-state-preparation-of-a-computational-basis-input.md)
- [Heralded Pauli X correction using controlled-Z and measurements](heralded-pauli-x-correction-using-controlled-z-and-measurements.md)
- [J gate in measurement-based quantum computation](j-gate-in-measurement-based-quantum-computation.md)
  - [J-gate phase-error operator norm](j-gate-phase-error-operator-norm.md)

## ↑ Ancestors (7)

1. [Quantum teleportation](quantum-teleportation.md)
2. [Local operations and classical communication](local-operations-and-classical-communication.md)
3. [Bell state](bell-state-split.md)
4. [Quantum theory](quantum-theory-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (18)

- [Equatorial measurement of a graph-state leaf](equatorial-measurement-of-a-graph-state-leaf.md)
- [Five-vertex graph-state circuit simulation](five-vertex-graph-state-circuit-simulation.md)
- [Four-cycle graph-state simulation of an entangle-and-measure circuit](four-cycle-graph-state-simulation-of-an-entangle-and-measure-circuit.md)
- [Heralded Pauli X correction using controlled-Z and measurements](heralded-pauli-x-correction-using-controlled-z-and-measurements.md)
- [Measurement-based quantum computation](measurement-based-quantum-computation.md)
- [Nonadaptive Hadamard–CNOT measurement pattern](nonadaptive-hadamard-cnot-measurement-pattern.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-51/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-51/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-49/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-67/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-67/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-67/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-61/4/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-61/4/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324/4/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324/4/a/iii/solution.md)
- [Pauli-frame propagation along a measurement wire](pauli-frame-propagation-along-a-measurement-wire.md)
- [Three-vertex graph-state wire](three-vertex-graph-state-wire.md)
