<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**Yes: a deterministic LOCC protocol exists for every allowed value of the parameter.** Here is an explicit implementation, so existence does not depend on merely quoting a pure-state conversion theorem.

First convert the input [Bell state](../../../../../../bell-state-split.md) to $|\Phi^+\rangle=(|00\rangle+|11\rangle)/\sqrt2$ by [local unitary operations](../../../../../../local-unitary-operation.md):

$$
(Z_A\otimes X_B)|\Psi^-\rangle=|\Phi^+\rangle.
$$

Write $c=\cos\phi$ and $s=\sin\phi$. Alice performs the two-outcome [measurement in quantum mechanics](../../../../../../quantum-measurement-split.md) with [Kraus operators](../../../../../../kraus-operator.md)

$$
M_0=\begin{pmatrix}c&0\\0&s\end{pmatrix},\qquad
M_1=\begin{pmatrix}s&0\\0&c\end{pmatrix}.
$$

They define a physical [measurement in quantum mechanics](../../../../../../quantum-measurement-split.md) because

$$
M_0^\dagger M_0+M_1^\dagger M_1=(c^2+s^2)I=I.
$$

Acting on $|\Phi^+\rangle$, the unnormalized branch vectors are

$$
(M_0\otimes I)|\Phi^+\rangle=\frac{c|00\rangle+s|11\rangle}{\sqrt2},\qquad
(M_1\otimes I)|\Phi^+\rangle=\frac{s|00\rangle+c|11\rangle}{\sqrt2}.
$$

Both branches have [probability](../../../../../../probability.md) $1/2$. Alice communicates the outcome to Bob. If it is one, both apply the [Pauli X gate](../../../../../../pauli-x-gate.md); this turns the normalized second branch into $c|00\rangle+s|11\rangle$. If it is zero, neither applies this correction. Finally Bob applies a [Pauli X gate](../../../../../../pauli-x-gate.md) in either branch, obtaining

$$
\boxed{c|01\rangle+s|10\rangle.}
$$

Every outcome produces the same target [pure state](../../../../../../pure-state.md), so this is deterministic [local operations and classical communication](../../../../../../local-operations-and-classical-communication.md), not a successful branch selected by [postselection](../../../../../../postselection.md). This [two-outcome LOCC dilution of a Bell pair](../../../../../../two-outcome-locc-dilution-of-a-bell-pair.md) remains valid at $\phi=0$, where the output is a [product state](../../../../../../product-state.md), and at $\phi=\pi/4$, where it is another [Bell state](../../../../../../bell-state-split.md).

The target [Schmidt coefficients](../../../../../../schmidt-coefficient.md) are $c,s$, while those of the input are both $1/\sqrt2$. For an interior value $0<\phi<\pi/4$, [local unitary operations](../../../../../../local-unitary-operation.md) alone could not change these [Schmidt coefficients](../../../../../../schmidt-coefficient.md); the local [measurement in quantum mechanics](../../../../../../quantum-measurement-split.md) is the step that reduces the [entanglement](../../../../../../entangled-state.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
