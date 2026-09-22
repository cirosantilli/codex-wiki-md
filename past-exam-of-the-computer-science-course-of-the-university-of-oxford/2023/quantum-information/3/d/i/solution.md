<h1 id="3/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Alice holds the input [qubit](../../../../../../qubit.md) $Q$ in $|\psi\rangle_Q=a|0\rangle+b|1\rangle$ and her half $A$ of a shared [Bell pair](../../../../../../bell-pair.md) $|\phi_+\rangle_{AB}$; Bob holds $B$. Alice applies a [controlled-NOT gate](../../../../../../controlled-not-gate.md) $Q\to A$, then a [Hadamard gate](../../../../../../hadamard-gate.md) on $Q$. In the system order $Q,A,B$, the initial [quantum state](../../../../../../quantum-state.md) is

$$
\frac1{\sqrt2}\left(a|000\rangle+a|011\rangle+b|100\rangle+b|111\rangle\right).
$$

After these two [quantum gates](../../../../../../quantum-logic-gate.md), direct expansion yields the [quantum teleportation](../../../../../../quantum-teleportation.md) identity

$$
\frac12\Bigl[
|00\rangle_{QA}(a|0\rangle+b|1\rangle)_B
+|01\rangle_{QA}(b|0\rangle+a|1\rangle)_B
+|10\rangle_{QA}(a|0\rangle-b|1\rangle)_B
+|11\rangle_{QA}(-b|0\rangle+a|1\rangle)_B
\Bigr]
=\frac12\sum_{m,n=0}^1|mn\rangle_{QA}X_B^nZ_B^m|\psi\rangle_B.
$$

Alice performs [computational-basis measurements](../../../../../../quantum-measurement-in-the-computational-basis.md) on $Q,A$, and sends the two classical [bits](../../../../../../bit.md) $m,n$ to Bob. Each outcome has [probability](../../../../../../probability.md) $1/4$, independently of the input [pure state](../../../../../../pure-state.md). Bob applies the indicated [Pauli gates](../../../../../../pauli-gate.md): first $X^n$, then $Z^m$, so his total correction is $Z^mX^n$. In every branch,

$$
\boxed{Z^mX^nX^nZ^m|\psi\rangle=|\psi\rangle.}
$$

This proves exact [quantum teleportation](../../../../../../quantum-teleportation.md) using one [Bell pair](../../../../../../bell-pair.md) and two classical [bits](../../../../../../bit.md). Alice's original [qubit](../../../../../../qubit.md) has been measured; the protocol transfers the [quantum state](../../../../../../quantum-state.md) without leaving her another copy.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
