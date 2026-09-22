<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Represent the [simple random walk](../../../../../simple-random-walk.md) by $X_n=\xi_1+\cdots+\xi_n$, where the increments are [independent and identically distributed](../../../../../independent-and-identically-distributed-random-variables.md) and satisfy $\mathbb P(\xi_k=1)=p$, $\mathbb P(\xi_k=-1)=1-p$. They are integrable and have [expectation](../../../../../expected-value-split.md) $2p-1$, so the [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) gives

$$
\boxed{\frac{X_n}{n}\longrightarrow\mu=2p-1\quad\text{almost surely}.}
$$

If $p\ne1/2$, this nonzero drift implies that $X_n$ eventually leaves every fixed finite interval and tends to the appropriate infinity. Hence it visits zero only finitely many times [almost surely](../../../../../almost-sure-convergence.md), so zero is a [transient state](../../../../../transient-state.md). By translation of the starting state, every state is transient: **the chain is transient for $p\ne1/2$**. This also covers the deterministic endpoint cases $p=0,1$, without assuming [Markov chain irreducibility](../../../../../irreducible-markov-chain.md) at those endpoints.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
