<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Fix an [orthonormal basis](../../../../../../orthonormal-basis.md) $\{|i\rangle\}_{i=1}^d$ of the input [Hilbert space](../../../../../../hilbert-space-split.md), where $d=\dim\mathcal H$, and a reference copy $R\simeq\mathcal H$. Use the normalized maximally entangled vector $|\Omega_d\rangle=d^{-1/2}\sum_i|i\rangle_R|i\rangle_{\mathcal H}$. The normalized [Choi–Jamiołkowski state](../../../../../../choi-state.md) is

$$
\boxed{J_{R\mathcal K}(\Lambda)=(\operatorname{id}_R\otimes\Lambda)(|\Omega_d\rangle\langle\Omega_d|)
=\frac1d\sum_{i,j}|i\rangle\langle j|_R\otimes\Lambda(|i\rangle\langle j|).}
$$

Complete positivity makes $J\geq0$, and trace preservation gives $\operatorname{Tr}_{\mathcal K}J=I_R/d$, hence $\operatorname{Tr}J=1$. It is therefore a genuine [density operator](../../../../../../density-matrix.md). In the unnormalized [Choi matrix](../../../../../../choi-matrix.md) convention the factor $1/d$ is omitted and the trace is $d$; specifying normalization distinguishes a [Choi state](../../../../../../choi-state.md) from that matrix convention. The reference basis also fixes the transpose in the [Choi reconstruction formula](../../../../../../choi-reconstruction-formula.md), $\Lambda(X)=d\operatorname{Tr}_R[(X^T\otimes I)J]$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
