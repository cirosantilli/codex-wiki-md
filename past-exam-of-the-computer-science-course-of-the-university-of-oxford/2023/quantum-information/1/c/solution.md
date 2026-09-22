<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use [deterministic two-qubit entanglement dilution](../../../../../deterministic-two-qubit-entanglement-dilution.md), retaining the specified complex [probability amplitudes](../../../../../probability-amplitude.md). Alice implements a [quantum instrument](../../../../../quantum-instrument.md) on $A$ with [Kraus operators](../../../../../kraus-operator.md)

$$
M_0=\begin{pmatrix}\alpha&0\\0&\beta\end{pmatrix},
\qquad
M_1=\begin{pmatrix}\beta&0\\0&\alpha\end{pmatrix}.
$$

The [Kraus representation](../../../../../kraus-representation.md) completeness condition holds even for complex $\alpha,\beta$:

$$
M_0^\dagger M_0+M_1^\dagger M_1=(|\alpha|^2+|\beta|^2)I=I.
$$

To realize this using the permitted [quantum gates](../../../../../quantum-logic-gate.md) and a [basic measurement](../../../../../basic-measurement.md), Alice initializes an [ancilla qubit](../../../../../ancilla-qubit.md) $C$ to $|0\rangle$. Conditional on her [computational-basis state](../../../../../computational-basis-state.md) being $j$, she applies to $C$ the [unitary matrix](../../../../../unitary-matrix.md)

$$
V_0=\begin{pmatrix}\alpha&-\overline\beta\\\beta&\overline\alpha\end{pmatrix},
\qquad
V_1=\begin{pmatrix}\beta&-\overline\alpha\\\alpha&\overline\beta\end{pmatrix}.
$$

Each has [orthonormal](../../../../../orthonormal-set.md) columns. Therefore $W=|0\rangle\langle0|_A\otimes V_0+|1\rangle\langle1|_A\otimes V_1$ is a [unitary gate](../../../../../quantum-logic-gate.md), with

$$
W\bigl(|u\rangle_A|0\rangle_C\bigr)
=M_0|u\rangle_A|0\rangle_C+M_1|u\rangle_A|1\rangle_C.
$$

A [computational-basis measurement](../../../../../quantum-measurement-in-the-computational-basis.md) of $C$ implements the desired [quantum instrument](../../../../../quantum-instrument.md). Its two unnormalized branches on $AB$ are

$$
(M_0\otimes I)|\phi_+\rangle
=\frac{\alpha|00\rangle+\beta|11\rangle}{\sqrt2},
\qquad
(M_1\otimes I)|\phi_+\rangle
=\frac{\beta|00\rangle+\alpha|11\rangle}{\sqrt2}.
$$

Each has [probability](../../../../../probability.md) $1/2$. Alice sends her outcome $m$ as one classical [bit](../../../../../bit.md). For $m=0$, both parties keep their [qubits](../../../../../qubit.md) unchanged. For $m=1$, both apply a [Pauli X gate](../../../../../pauli-x-gate.md), giving

$$
(X\otimes X)(\beta|00\rangle+\alpha|11\rangle)
=\alpha|00\rangle+\beta|11\rangle.
$$

Thus **both outcomes produce the exact target using one classical bit and local operations**. The construction includes $\alpha=0$ or $\beta=0$ and arbitrary [relative quantum phases](../../../../../relative-quantum-phase.md); it requires no [quantum channel](../../../../../quantum-channel.md) between the parties.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Quantum information](../../../quantum-information-split.md)
4. [2023](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
