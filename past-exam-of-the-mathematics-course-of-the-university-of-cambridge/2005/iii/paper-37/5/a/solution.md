<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Under the intended assumption that one use of the [quantum channel](../../../../../../quantum-channel.md) transmits one [qubit](../../../../../../qubit.md) without noise, Alice can communicate two [classical bits](../../../../../../bit.md) with certainty if she and Bob already share a [Bell pair](../../../../../../bell-pair.md). She uses **superdense coding**. The prior distribution of the [Bell pair](../../../../../../bell-pair.md) must be a resource available before the permitted channel use; distributing it through that same channel would consume another use.

Take the shared [Bell state](../../../../../../bell-state-split.md) to be $|\Phi^+\rangle=(|00\rangle+|11\rangle)/\sqrt2$, with Alice holding the first [qubit](../../../../../../qubit.md). For a two-[bit](../../../../../../bit.md) message $(a,b)\in\{0,1\}^2$, Alice applies the [local unitary operation](../../../../../../local-unitary-operation.md) $U_{ab}=X^aZ^b$ to her [qubit](../../../../../../qubit.md). The four encoded [pure states](../../../../../../pure-state.md) are, up to irrelevant [global phases](../../../../../../global-phase.md),

$$
\begin{array}{c|c|c}
(a,b)&U_{ab}&(U_{ab}\otimes I)|\Phi^+\rangle\\\hline
(0,0)&I&|\Phi^+\rangle\\
(0,1)&Z&|\Phi^-\rangle\\
(1,0)&X&|\Psi^+\rangle\\
(1,1)&XZ&-|\Psi^-\rangle
\end{array}
$$

They are [orthogonal](../../../../../../orthogonal-vectors.md): for any [matrix](../../../../../../matrix.md) $V$ on the first [qubit](../../../../../../qubit.md), $\langle\Phi^+|(V\otimes I)|\Phi^+\rangle=\operatorname{Tr}V/2$, and the four [Pauli operators](../../../../../../pauli-operator.md) are [orthogonal](../../../../../../orthogonal-vectors.md) in the [trace inner product](../../../../../../frobenius-inner-product.md). Explicitly,

$$
\langle\Phi^+|(U_{ab}^\dagger U_{a'b'}\otimes I)|\Phi^+\rangle
=\delta_{aa'}\delta_{bb'}.
$$

Alice sends her [qubit](../../../../../../qubit.md) through the [quantum channel](../../../../../../quantum-channel.md) once. Bob now holds both [qubits](../../../../../../qubit.md) and performs a [Bell-basis measurement](../../../../../../bell-basis-measurement.md). Its four [orthogonal projectors](../../../../../../orthogonal-projection.md) identify $(a,b)$ with certainty, giving

$$
\boxed{\text{one shared Bell pair + one noiseless qubit transmission}
\ \Longrightarrow\ \text{two classical bits}.}
$$

Before the transmission, Bob's [reduced density matrix](../../../../../../reduced-density-matrix.md) is $I/2$ for every message, so shared [entanglement](../../../../../../entangled-state.md) alone does not convey the message.

Without shared [entanglement](../../../../../../entangled-state.md), a noiseless single-[qubit](../../../../../../qubit.md) transmission cannot perfectly distinguish four messages: perfect discrimination requires [orthogonal](../../../../../../orthogonal-vectors.md) state supports, and its two-dimensional [Hilbert space](../../../../../../hilbert-space-split.md) has room for at most two nonzero mutually [orthogonal](../../../../../../orthogonal-vectors.md) supports. The [Holevo bound](../../../../../../holevo-s-theorem.md) also limits its accessible classical information to one [bit](../../../../../../bit.md). For the usual protocol starting with a shared two-[qubit](../../../../../../qubit.md) [pure state](../../../../../../pure-state.md) and using local unitary encodings, exact two-[bit](../../../../../../bit.md) transmission requires a maximally mixed Bob marginal. Indeed all encoded joint states are pure and have the same $\rho_B$, while [Subadditivity of Von Neumann entropy](../../../../../../subadditivity-of-von-neumann-entropy.md) gives their average entropy at most $1+S(\rho_B)$. Four equally likely perfectly distinguishable messages have average [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md) two, forcing $S(\rho_B)=1$ and hence a [maximally entangled state](../../../../../../maximally-entangled-state.md).

The specification “quantum channel” alone does not determine its dimension or noise, so the one-[qubit](../../../../../../qubit.md), noiseless interpretation is needed for this particular conclusion. A noiseless four-dimensional channel could send four [orthogonal](../../../../../../orthogonal-vectors.md) states without any shared [entanglement](../../../../../../entangled-state.md); a completely depolarizing [qubit](../../../../../../qubit.md) channel cannot transmit the message even with a shared [Bell pair](../../../../../../bell-pair.md), since its output is independent of Alice's encoding. Shared [entanglement](../../../../../../entangled-state.md) is therefore the extra resource for the intended single-[qubit](../../../../../../qubit.md) channel, not a guarantee for every unspecified [quantum channel](../../../../../../quantum-channel.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
