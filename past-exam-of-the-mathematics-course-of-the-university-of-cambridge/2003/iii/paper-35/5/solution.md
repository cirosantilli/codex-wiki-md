<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For a [memoryless quantum channel](../../../../../memoryless-quantum-channel.md) $\mathcal N$, successive uses are described by $\mathcal N^{\otimes n}$. Its [entanglement-assisted classical capacity](../../../../../entanglement-assisted-classical-capacity.md) is the supremum of classical bits per use achievable with error tending to zero when sender and receiver may use unlimited preshared [quantum entanglement](../../../../../entangled-state.md), independent of the message. Only the channel is used to transmit the message.

For input state $\rho_A$, choose a [purification](../../../../../purification-of-a-density-operator.md) $|\psi_\rho\rangle_{RA}$ and set $\omega_{RB}=(\operatorname{id}_R\otimes\mathcal N)(|\psi_\rho\rangle\langle\psi_\rho|)$. The capacity formula is

$$
\boxed{C_E(\mathcal N)=\max_{\rho_A}I(R;B)_\omega
=\max_{\rho_A}\bigl[S(\rho_A)+S(\mathcal N(\rho_A))-S(\omega_{RB})\bigr].}
$$

[Purifications](../../../../../purification-of-a-density-operator.md) differ only by an isometry on the reference, so this expression depends only on the input [density matrix](../../../../../density-matrix.md). The quantity optimized is [quantum mutual information](../../../../../quantum-mutual-information.md).

The binary [quantum erasure channel](../../../../../quantum-erasure-channel.md) sends a [qubit](../../../../../qubit.md) to a [qubit](../../../../../qubit.md) subspace plus an orthogonal erasure flag:

$$
\mathcal E_p(\rho)=(1-p)\rho\oplus p|e\rangle\langle e|,\qquad0\le p\le1.
$$

On the nonerased branch it transmits the entire state, including its coherences. Put $s=S(\rho)$. The [entropy of an orthogonal quantum mixture](../../../../../entropy-of-an-orthogonal-quantum-mixture.md) gives

$$
S(\mathcal E_p(\rho))=h_2(p)+(1-p)s.
$$

The reference-output state has two orthogonal branches:

$$
\omega_{RB}=(1-p)|\psi_\rho\rangle\langle\psi_\rho|\ \oplus\ p\rho_R\otimes|e\rangle\langle e|.
$$

The first branch is pure; the second has entropy $S(\rho_R)=s$. Thus $S(\omega_{RB})=h_2(p)+ps$ and

$$
I(R;B)_\omega=s+h_2(p)+(1-p)s-h_2(p)-ps=2(1-p)s.
$$

A [qubit](../../../../../qubit.md) has entropy at most one bit, with equality at $\rho=I_2/2$. We conclude

$$
\boxed{C_E(\mathcal E_p)=2(1-p)\text{ bits per channel use}.}
$$

The endpoint capacities are two and zero. As an operational check, [superdense coding](../../../../../superdense-coding.md) encodes four classical messages in one member of a shared Bell pair. A successful channel use lets the receiver identify the message; an erased [qubit](../../../../../qubit.md) yields the flag. This induces a four-symbol classical erasure channel of capacity $(1-p)\log_24=2(1-p)$, agreeing with the entropy calculation.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
