<h1 id="26i/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The [jump chain](../../../../../../jump-chain.md) records the successive states visited at actual jumps of the [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md). Put $q_i=-q_{ii}$. For an irreducible chain with at least two states, all $q_i>0$, and its transition [probabilities](../../../../../../probability.md) are $\widehat P_{ij}=q_{ij}/q_i$ for $j\ne i$, with $\widehat P_{ii}=0$. The holding time in state $i$ is exponential with mean $1/q_i$.

If $\pi Q=0$, set $C=\sum_i\pi_iq_i$ and $\widehat\pi_i=\pi_iq_i/C$. Then

$$
(\widehat\pi\widehat P)_j=\frac1C\sum_{i\ne j}\pi_iq_{ij}=\frac{\pi_jq_j}{C}=\widehat\pi_j.
$$

Conversely, $\widehat\pi\widehat P=\widehat\pi$ implies that $\pi_i=c\widehat\pi_i/q_i$, normalized to sum one, satisfies $\pi Q=0$. Therefore

$$
\boxed{\widehat\pi_i=\frac{\pi_iq_i}{\sum_j\pi_jq_j},\qquad \pi_i=\frac{\widehat\pi_i/q_i}{\sum_j\widehat\pi_j/q_j}.}
$$

Jump observations overrepresent states with short holding times. A one-state chain has no actual jumps; its trivial equilibrium can be handled separately, without using this division by $q_i=0$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [26I](../../26i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
