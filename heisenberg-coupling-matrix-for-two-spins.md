# Heisenberg coupling matrix for two spins

↑ **Parent:** [Heisenberg model](heisenberg-model.md)

For two [spin one-half](spin-one-half.md) systems, the dimensionless isotropic [Heisenberg model](heisenberg-model.md) coupling is $C=X\otimes X+Y\otimes Y+Z\otimes Z$, where $X,Y,Z$ are [Pauli matrices](pauli-matrices.md). In the ordered [computational basis](computational-basis.md) $(|00\rangle,|01\rangle,|10\rangle,|11\rangle)$,

$$
C=\begin{pmatrix}1&0&0&0\\0&-1&2&0\\0&2&-1&0\\0&0&0&1\end{pmatrix}=2S-I,
$$

where $S$ is the [SWAP gate](swap-gate.md). This follows by acting on each basis state: the $XX+YY$ terms exchange the two opposite-spin states with coefficient two and annihilate the parallel-spin states. The symmetric three-dimensional sector has [eigenvalue](eigenvalue.md) $1$ and the antisymmetric sector has [eigenvalue](eigenvalue.md) $-3$. Hence

$$
e^{-iaC/2}=e^{ia/2}\bigl(\cos a\,I-i\sin a\,S\bigr).
$$

This identity explains how isotropic [exchange interaction](exchange-interaction.md) generates a [SWAP gate](swap-gate.md) at $a=\pi/2$ up to a [global phase](global-phase.md).

## ↑ Ancestors (7)

1. [Heisenberg model](heisenberg-model.md)
2. [Spin](spin.md)
3. [Angular momentum operator](angular-momentum-operator-split.md)
4. [Quantum mechanics](quantum-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2008/6/1/solution.md)
