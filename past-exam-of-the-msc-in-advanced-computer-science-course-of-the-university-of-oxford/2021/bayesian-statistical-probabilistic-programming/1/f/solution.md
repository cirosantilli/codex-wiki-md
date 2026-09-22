<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

For each adjacent pair, the [detailed balance equations](../../../../../detailed-balance.md) follows directly:

$$
\pi_nP(n,n+1)=\tfrac12\pi_n\min(1,\pi_{n+1}/\pi_n)=\tfrac12\min(\pi_n,\pi_{n+1})=\pi_{n+1}P(n+1,n).
$$

For nonadjacent distinct states both fluxes vanish, and diagonal fluxes agree trivially. Since $\sum_n\pi_n=e^{-\lambda}\sum_n\lambda^n/n!=1$, this is a genuine [stationary distribution](../../../../../stationary-distribution.md), rather than merely an invariant measure of infinite mass.

Every upward and downward [transition probability](../../../../../transition-probability.md) between neighbouring states is positive for $\lambda>0$. Any two states can therefore be joined by a finite path of positive [probability](../../../../../probability.md): the [Markov chain](../../../../../markov-chain-split.md) is [irreducible](../../../../../irreducible-representation.md). Moreover,

$$
P(0,0)=1-\tfrac12\min(1,\lambda)\geq\tfrac12>0.
$$

State zero has period one; [Markov chain irreducibility](../../../../../irreducible-markov-chain.md) makes every state [aperiodic](../../../../../aperiodic-markov-chain.md). Finally, the standard countable-state recurrence theorem states that an [irreducible Markov chain](../../../../../irreducible-markov-chain.md) admitting a [stationary distribution](../../../../../stationary-distribution.md) of total mass one is [positive recurrent](../../../../../positive-recurrent-markov-chain.md), with that [stationary distribution](../../../../../stationary-distribution.md) unique. The [countable-state Markov chain convergence theorem](../../../../../countable-state-markov-chain-convergence-theorem.md) then states that [Markov chain irreducibility](../../../../../irreducible-markov-chain.md), [positive recurrence](../../../../../positive-recurrent-markov-chain.md) and [aperiodicity](../../../../../aperiodic-markov-chain.md) imply $P^k(i,j)\to\pi_j$ for all states $i,j$. The hypotheses just verified hold on the infinite [state space](../../../../../state-space.md) $\mathbb N_0$, not merely on a numerical truncation.[Sections 1.7–1.8, invariant distributions and convergence to equilibrium](../../../../../markov-chains-by-james-r-norris.md)

Consequently, **the unique [stationary distribution](../../../../../stationary-distribution.md) and the [limiting distribution](../../../../../limiting-distribution.md) are both $\operatorname{Poisson}(\lambda)$**, from every initial state. The [countable-state Markov chain ergodic theorem](../../../../../countable-state-markov-chain-ergodic-theorem.md) also gives $N^{-1}\sum_{k=1}^Nf(X_k)\to\sum_n\pi_nf(n)$ [almost surely](../../../../../almost-sure-convergence.md) whenever $\sum_n\pi_n|f(n)|<\infty$.[Section 1.10, ergodic theorem](../../../../../markov-chains-by-james-r-norris.md)

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Bayesian statistical probabilistic programming](../../../bayesian-statistical-probabilistic-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../split.md)
6. [MSc in advanced computer science course of the University of Oxford](../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
