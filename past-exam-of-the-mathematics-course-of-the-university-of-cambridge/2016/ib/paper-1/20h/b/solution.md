<h1 id="20h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An irreducible [Markov chain](../../../../../../markov-chain.md) has [positive recurrent states](../../../../../../positive-recurrent-state.md) if the expected first return time to a state is finite; this then holds for every state. A recurrent chain with infinite mean return time has [null recurrent states](../../../../../../null-recurrent-state.md).

An irreducible positive recurrent chain admits a [stationary distribution](../../../../../../stationary-distribution.md). If such a distribution $\pi$ existed for this walk, its stationarity equations would give

$$
\pi_j=\tfrac12(\pi_{j-1}+\pi_{j+1})\quad(j\in\mathbb Z).
$$

Thus $\pi_{j+1}-\pi_j=\pi_j-\pi_{j-1}$, so $\pi_j=A+Bj$. Nonnegativity for all positive and negative integers forces $B=0$. A constant sequence cannot sum to one over $\mathbb Z$, so no stationary probability distribution exists. Hence **the walk is null recurrent, not positive recurrent**: all its states are [null recurrent states](../../../../../../null-recurrent-state.md). The first-return generating function in part (c) also verifies directly that its mean return time is infinite.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [20H](../../20h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
