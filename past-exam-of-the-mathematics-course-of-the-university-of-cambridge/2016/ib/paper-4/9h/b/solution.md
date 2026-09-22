<h1 id="9h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A finite [irreducible Markov chain](../../../../../../irreducible-markov-chain.md) is positive recurrent. Its [mean recurrence time](../../../../../../mean-recurrence-time.md) to state $i$, starting at $i$ and counting the first positive return, is $1/\pi_i$. This identity comes from the long-run fraction of time spent at that state: successive return cycles each contain one visit at their start, so the fraction is the reciprocal of the mean cycle length. It remains valid for a periodic chain.

Here $\pi_0=2^{-k}$, hence

$$
\boxed{\mathbb E_0[T]=2^k\text{ minutes}.}
$$

For $k=1$ the return is deterministically after two minutes, which checks the formula.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [9H](../../9h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
