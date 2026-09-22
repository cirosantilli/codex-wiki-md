<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A compression scheme consists of [quantum channels](../../../../../../quantum-channel.md)

$$
\mathcal C_n:\mathcal B(\mathcal H^{\otimes n})\to\mathcal B(\mathcal K_n),\qquad\mathcal D_n:\mathcal B(\mathcal K_n)\to\mathcal B(\mathcal H^{\otimes n}),
$$

where each is a [CPTP map](../../../../../../quantum-channel.md). The [Hilbert space](../../../../../../hilbert-space-split.md) $\mathcal K_n$ is the compressed register. Its block rate in qubits per source qubit is $R_n=n^{-1}\log_2\dim\mathcal K_n$, with asymptotic rate $R=\limsup_nR_n$ (or the limit when it exists).

Use the [squared quantum fidelity](../../../../../../squared-quantum-fidelity.md) convention for the ensemble overlap:

$$
\boxed{F_n=\sum_kp_k^{(n)}\langle\Psi_k^{(n)}|\mathcal D_n\mathcal C_n(|\Psi_k^{(n)}\rangle\langle\Psi_k^{(n)}|)|\Psi_k^{(n)}\rangle.}
$$

This definition tests preservation of the emitted vectors themselves, including nonorthogonal ones; preserving only their classical labels would be a different task. **The scheme is reliable when $F_n\to1$ as $n\to\infty$.** This is the ensemble-average criterion for [reliable quantum source compression](../../../../../../reliable-quantum-source-compression.md). A square root is not taken in this definition, even though an unsquared convention is also used for [quantum fidelity](../../../../../../fidelity-of-quantum-states.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
