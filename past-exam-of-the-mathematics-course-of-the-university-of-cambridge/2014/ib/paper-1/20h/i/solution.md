<h1 id="20h/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a state $i$, its period is $d_i=\gcd\{n\geq1:p_{ii}^{(n)}>0\}$; the condition $d_i=1$ defines [aperiodicity](../../../../../../aperiodic-markov-chain.md). It is a [positive recurrent state](../../../../../../positive-recurrent-state.md) if return occurs almost surely and its first strictly positive return time has finite expectation. An [ergodic state of a Markov chain](../../../../../../ergodic-state-of-a-markov-chain.md) is positive recurrent and aperiodic.

The PDF specifies $p_{i,i-1}=1$ for $i\geq1$; the TeX aid drops the essential value one. Consequently every positive state reaches zero deterministically. From zero, every positive state $j$ is reached in one step with probability $pq^{j-1}>0$. Paths through zero connect any pair of states, proving **irreducibility**.

Let $J$ be the jump out of zero. It has $\mathbb P(J=j)=pq^{j-1}$ for $j\geq1$, after which exactly $j$ downward steps return to zero. Therefore $T_0=J+1$, giving

$$
\boxed{\mathbb P_0(T_0=n)=\begin{cases}0,&n=1,\\pq^{n-2},&n\geq2.\end{cases}}
$$

These probabilities sum to one and

$$
\boxed{\mathbb E_0T_0=1+1/p=(1+p)/p.}
$$

Returns of lengths two and three both have positive probability, so the period is one. Hence **state zero is ergodic**, and by irreducibility all states are positive recurrent and have the same period.

For this [geometric-jump countdown Markov chain](../../../../../../geometric-jump-countdown-markov-chain.md), the invariant equations give $\pi_0=\pi_1$ and $\pi_j=\pi_{j+1}+\pi_0pq^{j-1}$ for $j\geq1$. Summing the tail, or counting visits in a regeneration cycle, yields $\pi_j=\pi_0q^{j-1}$. Normalization gives

$$
\boxed{\pi_0=\frac p{1+p},\qquad \pi_j=\frac p{1+p}q^{j-1}\quad(j\geq1).}
$$

This is the [stationary distribution of a regenerative countdown chain](../../../../../../stationary-distribution-of-a-regenerative-countdown-chain.md). The standard recurrence identity for an irreducible positive recurrent [Markov chain](../../../../../../markov-chain.md) is $\mathbb E_iT_i^+=1/\pi_i$, so

$$
\boxed{\mathbb E_iT_i^+=\frac{1+p}{p q^{i-1}}\quad(i\geq1).}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [20H](../../20h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
