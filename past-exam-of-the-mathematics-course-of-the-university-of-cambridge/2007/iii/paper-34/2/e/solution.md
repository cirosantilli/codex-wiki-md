<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Choose $0<\varepsilon<R-S(\pi)$. The preceding construction and the [typical subspace theorem](../../../../../../typical-subspace-theorem.md) give, for all sufficiently large $n$,

$$
\dim\mathcal K_n\leq2^{n(S(\pi)+\varepsilon)}+1\leq2^{\lceil nR\rceil}.
$$

Embed this code into $m_n=\lceil nR\rceil$ qubits. The unused subspace can be decoded to a fixed source state, making the extended decoder trace preserving; encoded states never enter it. Hence its rate is $m_n/n\to R$.

For every $\delta>0$, sufficiently large $n$ has $\operatorname{Tr}(\pi^{\otimes n}P_\varepsilon^{(n)})\geq1-\delta$. The proved fidelity bound yields

$$
1\geq F_n\geq1-2\delta.
$$

Since $\delta$ is arbitrary, $F_n\to1$. Therefore

$$
\boxed{R>S(\pi)\ \Longrightarrow\ \text{a reliable quantum source code of rate }R\text{ exists}.}
$$

This establishes the achievability part of [Schumacher compression](../../../../../../schumacher-compression.md), including the failure flag and without presuming the source ensemble is orthogonal. If $R$ exceeds one, the same rate-budget construction simply uses spare code qubits; no claim of reducing the physical register size is then needed.

## ↑ Ancestors (11)

1. [E](../e.md)
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
