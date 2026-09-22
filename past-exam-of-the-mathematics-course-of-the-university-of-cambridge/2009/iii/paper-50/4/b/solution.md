<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**Yes, the conversion can be deterministic using [local operations and classical communication](../../../../../../local-operations-and-classical-communication.md).** Put $s=\sin\theta$ and $c=\cos\theta$. The initial state's squared [Schmidt coefficients](../../../../../../schmidt-coefficient.md) are $(1/2,1/2)$, while the target's decreasingly ordered squared [Schmidt coefficients](../../../../../../schmidt-coefficient.md) are $(c^2,s^2)$. Since $0<\theta<\pi/4$, one has $1/2<c^2$ and both pairs sum to one. Thus

$$
(1/2,1/2)\prec(c^2,s^2).
$$

The direction of this [majorization](../../../../../../majorization.md) is the allowed one in [Nielsen's pure-state conversion theorem](../../../../../../nielsen-s-pure-state-conversion-theorem.md): maximal entanglement can be reduced by deterministic [LOCC](../../../../../../local-operations-and-classical-communication.md).

Here is an explicit protocol, so no conversion theorem need be assumed. The sender first applies a [Pauli Z gate](../../../../../../pauli-z-gate.md) to remove the initial Bell-state minus sign. Starting from $|\Phi^+\rangle$, she performs a two-outcome local measurement with [Kraus operators](../../../../../../kraus-operator.md)

$$
M_0=\begin{pmatrix}s&0\\0&c\end{pmatrix},
\qquad
M_1=\begin{pmatrix}c&0\\0&s\end{pmatrix}.
$$

They define a valid measurement because $M_0^\dagger M_0+M_1^\dagger M_1=I$. The two unnormalized states after measurement are

$$
(M_0\otimes I)|\Phi^+\rangle=\frac{s|00\rangle+c|11\rangle}{\sqrt2},
\qquad
(M_1\otimes I)|\Phi^+\rangle=\frac{c|00\rangle+s|11\rangle}{\sqrt2}.
$$

Each outcome has probability $1/2$. For outcome zero, the normalized state is already $s|00\rangle+c|11\rangle$. For outcome one, both parties apply [Pauli X gates](../../../../../../pauli-x-gate.md), obtaining the same state. The sender communicates only which outcome occurred. Finally the receiver applies a [Pauli X gate](../../../../../../pauli-x-gate.md), giving $s|01\rangle+c|10\rangle$ in either branch. This is [deterministic two-qubit entanglement dilution](../../../../../../deterministic-two-qubit-entanglement-dilution.md), with total success probability one; it does not rely on postselection.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
