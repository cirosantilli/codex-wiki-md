# Two-qubit parity phase gate

↑ **Parent:** [Phase gate](phase-gate.md)

A [two-qubit parity phase gate](two-qubit-parity-phase-gate.md) multiplies odd-parity computational [vectors](vector.md) by $e^{i\theta}$ and fixes even-parity ones. With $R_\theta=\operatorname{diag}(1,e^{i\theta})$,

$$
G_\theta=\mathrm{CNOT}(I\otimes R_\theta)\mathrm{CNOT}.
$$

The first [controlled-NOT gate](controlled-not-gate.md) computes $x\oplus y$ in the second wire, the [phase gate](phase-gate.md) multiplies by $e^{i\theta(x\oplus y)}$, and the last [controlled-NOT gate](controlled-not-gate.md) restores the original bits. This [compute-phase-uncompute construction](compute-phase-uncompute-construction.md) leaves the data unchanged except for the desired phases. The more general [Pauli-string phase by parity computation](pauli-string-phase-by-parity-computation.md) uses the same mechanism. In terms of the [Pauli Z gate](pauli-z-gate.md), $G_\theta=e^{i\theta/2}\exp[-i\theta(Z\otimes Z)/2]$; the scalar factor ensures equality as a [matrix](matrix.md), rather than only up to [global phase](global-phase.md).

## ↑ Ancestors (5)

1. [Phase gate](phase-gate.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/quantum-information/1/e/ii/solution.md)
- [Two-qubit parity phase gate](two-qubit-parity-phase-gate.md)
