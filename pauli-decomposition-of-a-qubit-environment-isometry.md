# Pauli decomposition of a qubit-environment isometry

↑ **Parent:** [Pauli operator](pauli-operator.md)

Every linear map from a [qubit](qubit.md) into the [tensor product](tensor-product.md) of that [qubit](qubit.md) and an environment can be expanded in the [Pauli matrix](pauli-matrices.md) [orthonormal basis](orthonormal-basis.md) of operators. If $V|0\rangle=|0\rangle|e_{00}\rangle+|1\rangle|e_{01}\rangle$ and $V|1\rangle=|0\rangle|e_{10}\rangle+|1\rangle|e_{11}\rangle$, then the four coefficient vectors are

$$
|e_0\rangle=\frac{|e_{00}\rangle+|e_{11}\rangle}{2},\quad
|e_1\rangle=\frac{|e_{01}\rangle+|e_{10}\rangle}{2},\quad
|e_2\rangle=\frac{i(|e_{10}\rangle-|e_{01}\rangle)}{2},\quad
|e_3\rangle=\frac{|e_{00}\rangle-|e_{11}\rangle}{2}.
$$

These environment vectors need not be orthogonal, so this is an operator expansion rather than a claim that the [quantum channel](quantum-channel.md) is a classical [Pauli channel](pauli-channel.md). Physical [isometries](isometry.md) additionally preserve the [inner products](inner-product.md) of the two input basis states.

## ↑ Ancestors (7)

1. [Pauli operator](pauli-operator.md)
2. [Pauli group](pauli-group.md)
3. [Quantum circuit](quantum-circuit-split.md)
4. [Quantum theory](quantum-theory-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-47/3/solution.md)
