<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the [ratio definition of cutoff](../../../../../../ratio-definition-of-cutoff.md) from part (a), and write $T_n=t_{\mathrm{mix}}^{(n)}(1/4)$. In the [reversible Markov chain](../../../../../../reversible-markov-chain.md) setting of the preceding parts let $\gamma_n=1-\lambda_{2,n}$ and $\gamma_{*,n}=1-\max_{j\geq2}|\lambda_{j,n}|$. In particular $\gamma_{*,n}\leq\gamma_n$.

If $\gamma_nT_n$ did not tend to infinity, there would be a subsequence and $B>0$ for which $\gamma_nT_n\leq B$. Along it part (c) implies, for every fixed $0<\varepsilon<1/2$,

$$
\frac{t_{\mathrm{mix}}^{(n)}(\varepsilon)}{T_n}
\geq\left(\frac1{\gamma_{*,n}T_n}-\frac1{T_n}\right)\log\frac1{2\varepsilon}
\geq\left(\frac1B-\frac1{T_n}\right)\log\frac1{2\varepsilon}.
$$

Since $T_n\to\infty$, choose fixed $\varepsilon$ so small that $\log(1/(2\varepsilon))>B$. The lower limit of this ratio is then greater than one, contradicting [cutoff for Markov chains](../../../../../../cutoff-for-markov-chains.md). Thus the [Peres product condition](../../../../../../peres-product-condition.md) holds:

$$
\boxed{\gamma_nT_n\longrightarrow\infty.}
$$

In fact the argument with $\gamma_{*,n}$ proves the stronger absolute-gap product condition. Part (d) does not repeat the [reversible Markov chain](../../../../../../reversible-markov-chain.md) hypothesis; the ordinary real ordering of [eigenvalues](../../../../../../eigenvalue.md) above uses that hypothesis. If arbitrary chains are intended, define the [spectral gap](../../../../../../spectral-gap.md) explicitly: the [eigenvalue lower bound for total variation mixing](../../../../../../eigenvalue-lower-bound-for-total-variation-mixing.md) works for complex [eigenfunctions](../../../../../../eigenfunction.md) too, and proves the same assertion for $\gamma_*$ or for $1-\max_{j\geq2}\operatorname{Re}\lambda_j$, which is at least $\gamma_*$. No real ordering of complex [eigenvalues](../../../../../../eigenvalue.md) is implicit.

For the requested counterexample take nonlazy [simple random walk](../../../../../../simple-random-walk.md) on the [complete graph](../../../../../../complete-graph.md) $K_n$, $n\geq3$. Let $\Pi$ have every row equal to the [uniform distribution on a finite set](../../../../../../discrete-uniform-distribution.md), and let $a=-1/(n-1)$. Then

$$
P=\Pi+a(I-\Pi),\quad P^t=\Pi+a^t(I-\Pi),\quad
\boxed{d_n(t)=\left(1-\frac1n\right)(n-1)^{-t}.}
$$

Thus $d_n(0)\to1$ and $d_n(1)=1/n\to0$: every fixed-level [mixing time](../../../../../../mixing-time-of-a-markov-chain.md) is eventually one. This is a bounded-time jump satisfying the [ratio definition of cutoff](../../../../../../ratio-definition-of-cutoff.md). The ordinary [spectral gap](../../../../../../spectral-gap.md) is $n/(n-1)$ and the absolute one is $(n-2)/(n-1)$, so both products with $T_n=1$ tend to one, not infinity. The divergence assumption on $T_n$ is therefore essential under this convention.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
