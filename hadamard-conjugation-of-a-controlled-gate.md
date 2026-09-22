# Hadamard conjugation of a controlled gate

↑ **Parent:** [Controlled unitary gate](controlled-unitary-gate.md)

For a [controlled unitary gate](controlled-unitary-gate.md) $C(V)=|0\rangle\langle0|\otimes I+|1\rangle\langle1|\otimes V$, [Hadamard gates](hadamard-gate.md) on the target before and after the gate produce $C(HVH)$. Proof: the control-zero branch applies $HIH=I$, while the control-one branch applies $HVH$. [Linearity](linearity.md) extends the identity to arbitrary [quantum states](quantum-state.md). Since $C(H)C(V)C(H)=C(HVH)$ too, a pair of controlled [Hadamard gates](hadamard-gate.md) surrounding the same target operation can be replaced by ordinary target [Hadamard gates](hadamard-gate.md). No single controlled [Hadamard gate](hadamard-gate.md) is thereby identified with an ordinary one.

## ↑ Ancestors (5)

1. [Controlled unitary gate](controlled-unitary-gate.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/quantum-information/2/d/solution.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2006/5/1/solution.md)
