<h1 id="5/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Choose $P_X$ uniform on $\mathcal A_M$ and zero outside it, so the marginal [density operator](../../../../../../density-matrix.md) of $Q$ is $\bar\rho_Q=k^{-1}\sum_m\rho(m)_Q$. Define the [binary test for quantum decoding success](../../../../../../binary-test-for-quantum-decoding-success.md) by

$$
\boxed{F(0)=\sum_{m\in\mathcal A_M}|m\rangle\langle m|_{\widetilde X}\otimes E(m)_Q,\qquad
F(1)=I_{\widetilde XQ}-F(0).}
$$

Each $E(m)$ is a [positive contraction](../../../../../../positive-contraction.md). The [computational basis](../../../../../../computational-basis.md) blocks of $F(0)$ are these effects on $\mathcal A_M$ and zero elsewhere. Thus $0\leq F(0)\leq I$, making $F$ a [POVM](../../../../../../positive-operator-valued-measure.md) on the whole space, including labels outside $\mathcal A_M$.

On the correlated [classical-quantum state](../../../../../../classical-quantum-state.md), its acceptance probability is

$$
\operatorname{Tr}[F(0)\rho_{\widetilde XQ}]
=\frac1k\sum_m\operatorname{Tr}[E(m)\rho(m)]=1-\epsilon.
$$

On the product of the marginal [density operators](../../../../../../density-matrix.md),

$$
\operatorname{Tr}[F(0)(\rho_{\widetilde X}\otimes\bar\rho_Q)]
=\frac1k\sum_m\operatorname{Tr}[E(m)\bar\rho_Q]
=\frac1k\operatorname{Tr}\bar\rho_Q=\frac1k,
$$

since $\sum_mE(m)=I_Q$. **The two requested probabilities are therefore $1-\epsilon$ and $1/k$.** In the notation for binary output [density operators](../../../../../../density-matrix.md), the [measurement channel](../../../../../../measurement-channel.md) sends the joint input to $\omega[\epsilon]$ and the product input to $\omega[1-1/k]$; their parameters describe outcome one, not outcome zero.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [5](../../5.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
