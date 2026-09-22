<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use [entanglement-assisted discrimination of a Pauli basis](../../../../../entanglement-assisted-discrimination-of-a-pauli-basis.md). Define the known single-[qubit](../../../../../qubit.md) [unitary operator](../../../../../unitary-operator.md) $V$ by $V|0\rangle=|\psi\rangle$ and $V|1\rangle=|\psi^\perp\rangle$. Prepare the device input $A$ and a reference [ancilla qubit](../../../../../ancilla-qubit.md) $R$ in

$$
|\Omega\rangle_{AR}=(V_A\otimes I_R)|\phi_+\rangle
=\frac{|\psi\rangle_A|0\rangle_R+|\psi^\perp\rangle_A|1\rangle_R}{\sqrt2}.
$$

Apply the unknown device once to $A$, then apply the known inverse $V^\dagger$ to $A$. Since

$$
V^\dagger U_0V=I,\quad V^\dagger U_1V=Z,\quad
V^\dagger U_2V=X,\quad V^\dagger U_3V=iY,
$$

the possible two-[qubit](../../../../../qubit.md) outputs are

$$
\begin{aligned}
U_0:&\quad (|00\rangle+|11\rangle)/\sqrt2,\\
U_1:&\quad (|00\rangle-|11\rangle)/\sqrt2,\\
U_2:&\quad (|01\rangle+|10\rangle)/\sqrt2,\\
U_3:&\quad (|01\rangle-|10\rangle)/\sqrt2.
\end{aligned}
$$

These are the four mutually [orthogonal](../../../../../orthogonal-vectors.md) [Bell states](../../../../../bell-state-split.md). A [Bell-basis measurement](../../../../../bell-basis-measurement.md) therefore identifies the device with certainty. Explicitly, apply a [controlled-NOT gate](../../../../../controlled-not-gate.md) $A\to R$, then a [Hadamard gate](../../../../../hadamard-gate.md) on $A$, followed by [computational-basis measurements](../../../../../quantum-measurement-in-the-computational-basis.md). The readouts $00,10,01,11$ identify $U_0,U_1,U_2,U_3$, respectively. Thus **one use of the device and one reference qubit suffice**.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Quantum information](../../../quantum-information-split.md)
4. [2022](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
