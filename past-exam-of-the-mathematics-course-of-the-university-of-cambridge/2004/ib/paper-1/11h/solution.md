<h1 id="11h/solution">Solution</h1>

↑ **Parent:** [11H](../11h.md)

Irreducibility and the presence of another state imply $P_{ii}<1$: otherwise $i$ would be absorbing and could not reach that other state. Hence the proposed matrix has nonnegative entries and row sums $\sum_{j\ne i}P_{ij}/(1-P_{ii})=1$.

Observe the original [Markov chain](../../../../../markov-chain.md) only at times when it changes state. Starting from $i$, the next different state is $j\ne i$ with [probability](../../../../../probability.md)

$$
\sum_{r=0}^\infty P_{ii}^rP_{ij}=\frac{P_{ij}}{1-P_{ii}}.
$$

Each holding run has a finite geometric length almost surely. The [Strong Markov property](../../../../../strong-markov-property.md) at the successive change times therefore identifies the observed process as the [discrete-time jump chain](../../../../../jump-chain-of-a-discrete-time-markov-chain.md) with [transition matrix](../../../../../stochastic-matrix.md) $\widetilde P$.

Any positive-[probability](../../../../../probability.md) path of the original chain gives a path of this new chain after repeated consecutive states are deleted. Every remaining edge has positive $\widetilde P$ [probability](../../../../../probability.md), so **$\widetilde P$ is irreducible**. For recurrence, starting at any state $i$, repeated application of the Markov property at return times shows that the original recurrent chain visits $i$ infinitely often almost surely. A single sojourn cannot account for infinitely many visits, because every sojourn is finite almost surely. There must therefore be infinitely many separate visits to $i$ in the observed chain too. Thus **$\widetilde P$ is recurrent**, proving that [recurrence survives deletion of self-transitions](../../../../../recurrence-survives-deletion-of-self-transitions.md).

## ↑ Ancestors (10)

1. [11H](../11h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
