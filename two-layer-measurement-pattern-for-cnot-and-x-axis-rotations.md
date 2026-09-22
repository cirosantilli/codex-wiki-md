# Two-layer measurement pattern for CNOT and x-axis rotations

↑ **Parent:** [Logical depth of a measurement pattern](logical-depth-of-a-measurement-pattern.md)

An $R(\alpha)=J(\alpha)J(0)$ gadget with input [Pauli frame](pauli-frame.md) $X^pZ^q$, angle-zero outcome $s$, and arbitrary-angle outcome $t$ uses angle $(-1)^{s\oplus q}\alpha$ and produces frame $X^{p\oplus t}Z^{q\oplus s}$. The [CNOT gate](controlled-not-gate.md) gadget also updates its $Z$ frames without any dependence on incoming $X$ frames. Therefore all adaptive angle signs depend solely on angle-zero outcomes. Measure all those vertices first, compute every sign, and measure all remaining vertices in a second layer. The result is the desired logical circuit in a known [Pauli frame](pauli-frame.md). Computational output measurements can share the second layer.

## ↑ Ancestors (8)

1. [Logical depth of a measurement pattern](logical-depth-of-a-measurement-pattern.md)
2. [Measurement pattern](measurement-pattern.md)
3. [Measurement-based quantum computation](measurement-based-quantum-computation.md)
4. [Quantum circuit](quantum-circuit-split.md)
5. [Quantum theory](quantum-theory-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-67/3/c/solution.md)
