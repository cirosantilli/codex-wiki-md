<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For the [countable-state Markov chain ergodic theorem](../../../../../countable-state-markov-chain-ergodic-theorem.md), let the [Markov chain](../../../../../markov-chain-split.md) be irreducible and positive recurrent, with its unique [stationary distribution](../../../../../stationary-distribution.md) $\pi$. From any initial state, for every real $f$ satisfying $\sum_j\pi_j|f(j)|<\infty$,

$$
\boxed{\frac1n\sum_{m=0}^{n-1}f(X_m)\longrightarrow\sum_j\pi_jf(j)\quad\text{almost surely}.}
$$

In particular, $n^{-1}\sum_{m=0}^{n-1}\mathbf1_{\{X_m=j\}}\to\pi_j$ [almost surely](../../../../../almost-sure-convergence.md). This time-average conclusion requires no [aperiodicity](../../../../../aperiodic-markov-chain.md).

The [countable-state Markov chain convergence theorem](../../../../../countable-state-markov-chain-convergence-theorem.md) adds the hypothesis of an [aperiodic Markov chain](../../../../../aperiodic-markov-chain.md) and concludes

$$
\boxed{P^n(i,j)\longrightarrow\pi_j\quad\text{for every }i,j.}
$$

It also follows that $\mathbb P_\nu(X_n=j)\to\pi_j$ for every initial [probability distribution](../../../../../probability-distribution-split.md) $\nu$. For an irreducible recurrent chain, the occupation-frequency theorem can also be stated as a limit $1/\mathbb E_jT_j^+$, interpreted as zero for a [null recurrent state](../../../../../null-recurrent-state.md); in the positive recurrent case this equals $\pi_j$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
