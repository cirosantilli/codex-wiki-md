<h1 id="26i/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A [discrete-time Markov chain](../../../../../../discrete-time-markov-chain.md) with initial distribution $\widehat\pi$ is [reversible](../../../../../../reversible-markov-chain.md) if $(Y_0,\ldots,Y_n)$ and $(Y_n,\ldots,Y_0)$ have the same law for every $n$. Its [detailed balance](../../../../../../detailed-balance.md) equations are $\widehat\pi_i\widehat P_{ij}=\widehat\pi_j\widehat P_{ji}$. These equations are equivalent to reversibility. Indeed, reversing every factor in the [probability](../../../../../../probability.md) $\widehat\pi_{i_0}\prod_{r=1}^n\widehat P_{i_{r-1}i_r}$ gives the reverse path [probability](../../../../../../probability.md); the converse follows by taking $n=1$.

Summing [detailed balance](../../../../../../detailed-balance.md) over $i$ gives

$$
(\widehat\pi\widehat P)_j=\sum_i\widehat\pi_i\widehat P_{ij}=\widehat\pi_j\sum_i\widehat P_{ji}=\widehat\pi_j.
$$

Hence $\widehat\pi$ is an [stationary distribution](../../../../../../stationary-distribution.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
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
