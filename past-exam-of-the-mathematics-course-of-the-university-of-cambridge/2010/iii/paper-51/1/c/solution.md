<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**Yes: deterministic entanglement swapping gives the required singlet.** Denote Bob's two local qubits by $B_1,B_2$. Known [local unitary operations](../../../../../../local-unitary-operation.md) first convert the two given [spin singlet states](../../../../../../spin-singlet-state.md) into $|\Phi^+\rangle_{AB_1}$ and $|\Phi^+\rangle_{B_2C}$. For example applying $ZX$ to the second qubit of a singlet gives $|\Phi^+\rangle$, where $X,Z$ are [Pauli operators](../../../../../../pauli-operator.md).

Use the binary-labelled [Bell states](../../../../../../bell-state-split.md)

$$
|B_{pq}\rangle=(I\otimes X^qZ^p)|\Phi^+\rangle,\qquad p,q\in\{0,1\}.
$$

They are $\Phi^+,\Phi^-,\Psi^+,\Psi^-$ for labels $(0,0),(1,0),(0,1),(1,1)$. Reordering registers to group Bob's qubits, direct expansion gives

$$
|\Phi^+\rangle_{AB_1}|\Phi^+\rangle_{B_2C}
=\frac12\sum_{p,q=0}^1|B_{pq}\rangle_{B_1B_2}|B_{pq}\rangle_{AC}.
$$

All four basis vectors are real in this convention; otherwise the paired expansion must account for complex conjugation. Bob performs the [Bell-basis measurement](../../../../../../bell-basis-measurement.md) on $B_1B_2$. This joint operation is local to him, so it is allowed by [LOCC](../../../../../../local-operations-and-classical-communication.md). Each outcome occurs with probability $1/4$ and leaves $AC$ in the corresponding [Bell state](../../../../../../bell-state-split.md).

Bob sends $(p,q)$ to Charlie. Charlie applies $Z^pX^{-q}$ to obtain $|\Phi^+\rangle_{AC}$, and then $XZ$ to obtain

$$
\boxed{|\Psi^-\rangle_{AC}=\frac{|01\rangle-|10\rangle}{\sqrt2}.}
$$

The correction works for every outcome, so no postselection or successful-outcome assumption is needed. This is [entanglement swapping](../../../../../../entanglement-swapping.md), equivalently teleportation of $B_1$ to $C$ while preserving its entanglement with $A$. If Bob's measurement result is ignored, the average $AC$ state is $I_4/4$; the protocol therefore does not supply entanglement usable without the classical outcome or violate the [no-communication theorem](../../../../../../no-communication-theorem.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
