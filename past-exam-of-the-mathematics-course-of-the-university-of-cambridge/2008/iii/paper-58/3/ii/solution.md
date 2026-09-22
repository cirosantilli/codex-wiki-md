<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $Q$ be Alice's unknown [qubit](../../../../../../qubit.md), with [pure state](../../../../../../pure-state.md) $|\phi\rangle_Q=\alpha|0\rangle+\beta|1\rangle$. Alice and Bob initially share the [Bell state](../../../../../../bell-state-split.md) $|\Phi^+\rangle_{AB}=(|00\rangle+|11\rangle)/\sqrt2$. Alice holds $Q,A$ and Bob holds $B$. Define the [Bell basis](../../../../../../bell-basis.md)

$$
|\Phi^\pm\rangle=\frac{|00\rangle\pm|11\rangle}{\sqrt2},\qquad
|\Psi^\pm\rangle=\frac{|01\rangle\pm|10\rangle}{\sqrt2}.
$$

Expanding in this [orthonormal basis](../../../../../../orthonormal-basis.md) gives the [Bell-basis teleportation identity](../../../../../../bell-basis-teleportation-identity.md)

$$
\begin{aligned}
|\phi\rangle_Q|\Phi^+\rangle_{AB}=\frac12\bigl(&|\Phi^+\rangle_{QA}|\phi\rangle_B
+|\Phi^-\rangle_{QA}Z|\phi\rangle_B\\
&+|\Psi^+\rangle_{QA}X|\phi\rangle_B
+|\Psi^-\rangle_{QA}XZ|\phi\rangle_B\bigr).
\end{aligned}
$$

For example, the last branch on $B$ is $\alpha|1\rangle-\beta|0\rangle$, which is $XZ|\phi\rangle$; the ordering of the [Pauli operators](../../../../../../pauli-operator.md) therefore matters.

Alice performs a [projective measurement](../../../../../../projective-measurement.md) in the [Bell basis](../../../../../../bell-basis.md) on her two local [qubits](../../../../../../qubit.md). Each outcome has [probability](../../../../../../probability.md) $1/4$, independent of the unknown amplitudes. She encodes the four possible outcomes as two classical bits and sends them to Bob. For outcomes $\Phi^+,\Phi^-,\Psi^+,\Psi^-$, respectively, Bob applies the [local unitary operations](../../../../../../local-unitary-operation.md)

$$
I,\qquad Z,\qquad X,\qquad ZX.
$$

These are inverses of the corresponding branch [Pauli operators](../../../../../../pauli-operator.md), so **Bob obtains exactly the unknown input qubit in every branch**. Using $XZ$ instead of $ZX$ as the last correction also succeeds up to an irrelevant overall phase. Alice need not know $\alpha$ or $\beta$. Every quantum operation is local to one of the parties, and the only transmitted information is the two-bit classical outcome. The shared [Bell pair](../../../../../../bell-pair.md) is consumed.

Before the message arrives, Bob's [density operator](../../../../../../density-matrix.md) is

$$
\frac14\left(\rho+Z\rho Z+X\rho X+XZ\rho ZX\right)=\frac I2,
$$

so no unknown-state information is available without the [classical communication](../../../../../../classical-communication.md). Alice's original [qubit](../../../../../../qubit.md) has been included in the destructive [Bell-basis measurement](../../../../../../bell-basis-measurement.md); the protocol creates no extra copy. Since the corrected transformation is the identity on every input vector and is linear, it also preserves [entanglement](../../../../../../entangled-state.md) with an external reference and transfers mixed inputs. Thus this is deterministic [quantum teleportation](../../../../../../quantum-teleportation.md), using precisely one shared maximally entangled [Bell pair](../../../../../../bell-pair.md), two classical bits, and local operations.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
