# Nonadaptive Clifford measurement pattern

↑ **Parent:** [Logical depth of a measurement pattern](logical-depth-of-a-measurement-pattern.md)

A path [graph state](graph-state.md) simulates a sequence of [Clifford gates](clifford-gate.md) $J(\alpha_j)$, $\alpha_j\in\{0,\pi/2\}$, using fixed [equatorial qubit measurement](equatorial-qubit-measurement.md) bases on successive path [vertices](vertex-graph-theory.md). Let $s_j$ be raw outcomes, $t_j=2\alpha_j/\pi\in\{0,1\}$, and start the [Pauli frame](pauli-frame.md) at $a_0=b_0=0$. Matrix commutation and $J(-\pi/2)=XJ(\pi/2)$ give

$$
a_j=s_j\oplus b_{j-1}\oplus t_ja_{j-1},\qquad b_j=a_{j-1}.
$$

Induction shows the final unmeasured state differs from the ideal circuit output by $X^{a_m}Z^{b_m}$, up to [global phase](global-phase.md). A final [computational basis](computational-basis.md) result $d$ is corrected to $d\oplus a_m$. All bases are fixed, and projectors on distinct [vertices](vertex-graph-theory.md) commute, so all measurements, including the final one, can occur in a single layer. The frame recurrence is classical outcome processing, not quantum feed-forward.

**Table of contents**

- [Nonadaptive Hadamard–CNOT measurement pattern](nonadaptive-hadamard-cnot-measurement-pattern.md)

## ↑ Ancestors (8)

1. [Logical depth of a measurement pattern](logical-depth-of-a-measurement-pattern.md)
2. [Measurement pattern](measurement-pattern.md)
3. [Measurement-based quantum computation](measurement-based-quantum-computation.md)
4. [Quantum circuit](quantum-circuit-split.md)
5. [Quantum theory](quantum-theory-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)
