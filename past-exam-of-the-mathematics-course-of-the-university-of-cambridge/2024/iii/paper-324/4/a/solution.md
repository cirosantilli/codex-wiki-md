<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First construct a [controlled unitary gate](../../../../../../controlled-unitary-gate.md) from the uncontrolled oracle. Keep the supplied $|v_0\rangle$ in a reference register. Controlled on an extra qubit, swap the data and reference registers, query $U$ on the register that contains $|v_0\rangle$ in one branch, and swap back. Because $U|v_0\rangle=|v_0\rangle$, that branch is unchanged, while the other branch acquires $U$ on the data. Reversing the control convention with [Pauli X gates](../../../../../../pauli-x-gate.md) gives controlled-$U$. The reference state is returned unchanged, and each use costs one query to $U$ and $O(n)$ [controlled-SWAP gates](../../../../../../fredkin-gate.md).

Expand $|b\rangle=\sum_jb_j|v_j\rangle$ in an [eigenbasis](../../../../../../eigenbasis.md) of $U$. [Exact quantum phase estimation](../../../../../../exact-quantum-phase-estimation.md) with an $m$-qubit phase register produces

$$
\sum_jb_j|c_j\rangle|v_j\rangle,
\qquad
U|v_j\rangle=e^{2\pi ic_j/2^m}|v_j\rangle.
$$

Apply the available [phase gates](../../../../../../phase-gate.md), controlled by the corresponding bits of $c_j$, to multiply branch $j$ by

$$
e^{-2\pi ic_j/2^m}=\lambda_j^{-1}.
$$

Then reverse phase estimation. Although no $U^\dagger$ oracle was supplied, every eigenvalue obeys $\lambda_j^{2^m}=1$, so $U^{-q}=U^{2^m-q}$. The inverse controlled powers can therefore be implemented with forward calls to $U$. Since $2^m=\operatorname{poly}(n)$, phase estimation and its inverse use only $\operatorname{poly}(n)$ queries. The phase register returns to $|0^m\rangle$, while the data register is

$$
\sum_jb_j\lambda_j^{-1}|v_j\rangle
=\boxed{U^\dagger|b\rangle}.
$$

As a direct check, the same spectral promise implies $U^\dagger=U^{2^m-1}$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
