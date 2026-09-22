<h1 id="9h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [reversible Markov chain](../../../../../../reversible-markov-chain.md) has a stationary law $\pi$ for which every finite path has the same distribution as its time-reversed path:

$$
\boxed{(X_0,\ldots,X_k)\overset d=(X_k,\ldots,X_0)\quad\text{for every }k\ge0.}
$$

For a transition matrix $P$, the equivalent [detailed balance](../../../../../../detailed-balance.md) condition is $\pi_iP_{ij}=\pi_jP_{ji}$ for all $i,j$. It implies $\pi P=\pi$ by summing over $i$. Multiplying the balance identities along a path shows equality of its forward and reverse probabilities when $X_0\sim\pi$; conversely, taking paths of length one gives those identities.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9H](../../9h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
