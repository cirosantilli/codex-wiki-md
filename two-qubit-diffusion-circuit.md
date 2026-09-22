# Two-qubit diffusion circuit

↑ **Parent:** [Inversion about the mean](inversion-about-the-mean.md)

The [inversion about the mean](inversion-about-the-mean.md) for four [computational-basis states](computational-basis-state.md) can be implemented using [Hadamard gates](hadamard-gate.md), [Pauli X gates](pauli-x-gate.md) and one [controlled-NOT gate](controlled-not-gate.md), up to [global phase](global-phase.md). Let $Q=H\otimes H$ and $P=X\otimes X$. Since $CZ=(I\otimes H)\operatorname{CNOT}(I\otimes H)=I-2|11\rangle\langle11|$, one has $PCZP=I-2|00\rangle\langle00|$ and therefore $QPCZPQ=I-2|++\rangle\langle++|=-D$. This gives an exact [quantum circuit](quantum-circuit-split.md) representative of the four-entry [Grover search algorithm](grover-s-algorithm.md) diffusion step modulo its irrelevant overall minus sign.

## ↑ Ancestors (7)

1. [Inversion about the mean](inversion-about-the-mean.md)
2. [Grover diffusion operator](grover-diffusion-operator.md)
3. [Grover's algorithm](grover-s-algorithm.md)
4. [Quantum theory](quantum-theory-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/quantum-information/2/d/solution.md)
