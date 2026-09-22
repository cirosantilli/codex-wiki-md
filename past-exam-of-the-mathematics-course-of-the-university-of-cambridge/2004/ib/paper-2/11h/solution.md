<h1 id="11h/solution">Solution</h1>

↑ **Parent:** [11H](../11h.md)

For a [Markov chain](../../../../../markov-chain.md) started in its [stationary distribution](../../../../../stationary-distribution.md), reversibility means that for every $n$, the joint distribution of $(X_0,\ldots,X_n)$ equals that of $(X_n,\ldots,X_0)$. More generally, stationarity then makes every finite segment invariant under reversal of its time order.

If the [Markov chain](../../../../../markov-chain.md) is reversible, take $n=1$. Comparing the events $(X_0,X_1)=(i,j)$ and $(j,i)$ gives the [detailed balance](../../../../../detailed-balance.md) equations

$$
\boxed{\pi_iP_{ij}=\pi_jP_{ji}\quad(i,j\in S).}
$$

Conversely, an [irreducible Markov chain](../../../../../irreducible-markov-chain.md) with an invariant probability distribution has $\pi_i>0$ for every state. Under [detailed balance](../../../../../detailed-balance.md), a transition is positive exactly when its reverse is positive. For a path with positive probability, substitute $P_{ij}=\pi_jP_{ji}/\pi_i$ in each factor to obtain

$$
\pi_{i_0}\prod_{r=0}^{n-1}P_{i_ri_{r+1}}
=\pi_{i_n}\prod_{r=0}^{n-1}P_{i_{r+1}i_r}.
$$

The factors of $\pi$ telescope. If a path has a zero transition, its reverse does too, so the equality still holds. These are the respective forward and reversed path probabilities. Summing over any collection of paths proves equality of the joint distributions, hence a [reversible Markov chain](../../../../../reversible-markov-chain.md). The first factor in the PDF's balance equation is $\pi_i$; the converted TeX incorrectly changes it to $\pi_j$.

## ↑ Ancestors (10)

1. [11H](../11h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
