<h1 id="1/f/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Now $T^2=S=\operatorname{diag}(1,i)$. The gates $H,S$ and CNOT are [Clifford gates](../../../../../../clifford-gate.md): conjugating a [Pauli matrix](../../../../../../pauli-matrices.md) or a [tensor product](../../../../../../tensor-product.md) of them gives another signed Pauli tensor. On one wire,

$$
HXH=Z,\quad HZH=X,\quad SXS^\dagger=Y,\quad SZS^\dagger=Z.
$$

For CNOT the generator images are $X\otimes I\mapsto X\otimes X$, $I\otimes X\mapsto I\otimes X$, $Z\otimes I\mapsto Z\otimes I$, and $I\otimes Z\mapsto Z\otimes Z$. These identities can be checked on the four computational [vectors](../../../../../../vector.md) and generate the preservation property for all Pauli tensors.[Section 3 and Table 1, Clifford generators and their Pauli conjugation rules](../../../../../../the-heisenberg-representation-of-quantum-computers-by-daniel-gottesman.md)

For a fixed number $n$ of wires there are only finitely many possible images of the $2n$ generators $X_j,Z_j$ in the [Pauli group](../../../../../../pauli-group.md). Their images determine a unitary up to [global phase](../../../../../../global-phase.md). To see this, if two [unitary operators](../../../../../../unitary-operator.md) induce identical images, their quotient commutes with every $Z_j$, so is diagonal in the [computational basis](../../../../../../computational-basis.md); commuting with every $X_j$ then forces all diagonal entries to be equal. The quotient is a scalar phase. Thus the generated gates form a finite set modulo [global phase](../../../../../../global-phase.md), which cannot be dense in the continuous space of all [unitary operators](../../../../../../unitary-operator.md). This is [finiteness of the projective Clifford group](../../../../../../finiteness-of-the-projective-clifford-group.md).

A small visible consequence is that from $|0\rangle$, one-qubit [Clifford circuits](../../../../../../clifford-circuit.md) reach only the six states $|0\rangle,|1\rangle,|+\rangle,|-\rangle,|+i\rangle,|-i\rangle$ up to [global phase](../../../../../../global-phase.md). For instance, $T|+\rangle$ is outside this finite set. The fixed-$n$ Pauli argument also covers circuits using CNOT on several wires. Therefore **$\{\mathrm{CNOT},H,T^2\}$ is not universal**.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [F](../../f.md)
3. [1](../../../1.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2020](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
