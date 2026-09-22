# Three-vertex graph-state wire

↑ **Parent:** [Measurement-based quantum computation](measurement-based-quantum-computation.md)

A path [graph state](graph-state.md) on three [qubits](qubit.md) simulates two successive gates $U(\theta)=H\operatorname{diag}(1,e^{-i\theta})=J(-\theta)$. Measure vertex one in the [equatorial qubit measurement](equatorial-qubit-measurement.md) basis $|v_r(\alpha)\rangle=(|0\rangle+(-1)^re^{i\alpha}|1\rangle)/\sqrt2$, then vertex two at angle $(-1)^r\beta$, obtaining bits $r,s$. Two [one-bit teleportations](one-bit-teleportation.md) and $U(\theta)X=e^{-i\theta}ZU(-\theta)$ leave vertex three in $X^sZ^rU(\beta)U(\alpha)|+\rangle$, up to [global phase](global-phase.md). A computational output bit $z$ is corrected to $z\oplus s$; the $Z$ factor affects only phase. Adaptive sign choice is required for general angles, although the final bit correction is purely classical.

## ↑ Ancestors (6)

1. [Measurement-based quantum computation](measurement-based-quantum-computation.md)
2. [Quantum circuit](quantum-circuit-split.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-49/2/b/solution.md)
- [Two-bit remote state preparation on a graph-state path](two-bit-remote-state-preparation-on-a-graph-state-path.md)
