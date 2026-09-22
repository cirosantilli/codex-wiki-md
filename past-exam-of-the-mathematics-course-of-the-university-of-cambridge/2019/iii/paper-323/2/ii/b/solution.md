<h1 id="2/ii/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A compression-decompression scheme consists of [quantum channels](../../../../../../../quantum-channel.md) $\mathcal E_n:\mathcal D(\mathcal H^{\otimes n})\to\mathcal D(\mathcal K_n)$ and $\mathcal D_n:\mathcal D(\mathcal K_n)\to\mathcal D(\mathcal H^{\otimes n})$, where $\limsup_n n^{-1}\log_2\dim\mathcal K_n\leq R$. For the emitted pure-state ensemble, reliability means that the mean squared [quantum fidelity](../../../../../../../fidelity-of-quantum-states.md) tends to one:

$$
\boxed{\sum_kp_k\langle\Psi_k^{(n)}|
(\mathcal D_n\circ\mathcal E_n)(|\Psi_k^{(n)}\rangle\langle\Psi_k^{(n)}|)
|\Psi_k^{(n)}\rangle\longrightarrow1}.
$$

The average is taken over the actual source distribution, rather than the worst possible input vector.

A standard stronger formulation of [reliable quantum source compression](../../../../../../../reliable-quantum-source-compression.md) requires

$$
F_e(\pi^{\otimes n},\mathcal D_n\circ\mathcal E_n)\longrightarrow1,
$$

where [entanglement fidelity](../../../../../../../entanglement-fidelity.md) tests preservation of a purification and its reference-system correlations. It implies the mean-fidelity condition for every pure-state ensemble of $\pi^{\otimes n}$. [Schumacher compression](../../../../../../../schumacher-compression.md) achieves this at any rate $R>S(\pi)$: choose $0<\varepsilon<R-S(\pi)$, encode the [quantum typical subspace](../../../../../../../quantum-typical-subspace.md), and map atypical outcomes to a fallback state. The composed channel has a Kraus term $P_\varepsilon^{(n)}$, so its [entanglement fidelity](../../../../../../../entanglement-fidelity.md) is at least $[\operatorname{Tr}(\pi^{\otimes n}P_\varepsilon^{(n)})]^2\to1$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [Ii](../../ii.md)
3. [2](../../../2.md)
4. [Paper 323](../../../../paper-323-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
