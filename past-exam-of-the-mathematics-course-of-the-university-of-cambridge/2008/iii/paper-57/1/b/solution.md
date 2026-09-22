<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $N=2k+1$ and abbreviate the [Dicke states](../../../../../../dicke-state.md) by $|D_j^n\rangle=|\Psi_j^n\rangle$. Alice's shared resource has decomposition

$$
\frac1{\sqrt2}\left(|0\rangle|D_{k+1}^N\rangle+|1\rangle|D_k^N\rangle\right).
$$

Follow the actual circuit order: a [controlled-NOT gate](../../../../../../controlled-not-gate.md) from the input to $q_0$, a [Hadamard gate](../../../../../../hadamard-gate.md) on the input and a [Pauli X gate](../../../../../../pauli-x-gate.md) on $q_0$, followed by [computational basis](../../../../../../computational-basis.md) measurements. Just before measurement, the joint [vector](../../../../../../vector.md) is

$$
\begin{aligned}
\frac12\big[&|00\rangle(\alpha|D_k^N\rangle+\beta|D_{k+1}^N\rangle)\\
+&|01\rangle(\alpha|D_{k+1}^N\rangle+\beta|D_k^N\rangle)\\
+&|10\rangle(\alpha|D_k^N\rangle-\beta|D_{k+1}^N\rangle)\\
+&|11\rangle(\alpha|D_{k+1}^N\rangle-\beta|D_k^N\rangle)\big].
\end{aligned}
$$

The [Dicke states](../../../../../../dicke-state.md) in each branch are [orthogonal](../../../../../../orthogonal-vectors.md), so each branch has squared [norm](../../../../../../norm.md) $1/4$. Conditioning on outcome $00$ and normalizing therefore gives the state of the other $N$ parties:

$$
\boxed{|\Omega\rangle=\alpha|D_{(N-1)/2}^N\rangle+\beta|D_{(N+1)/2}^N\rangle.}
$$

This is the encoding used in [Dicke-resource telecloning](../../../../../../dicke-resource-telecloning.md). The extra [Pauli X gate](../../../../../../pauli-x-gate.md) on Alice's resource [qubit](../../../../../../qubit.md) is essential to the displayed ordering of the amplitudes.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
