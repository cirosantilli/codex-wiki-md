<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For each $z$, integrate the probability of occupying the ill state:

$$
\mathbb E_H^{(z)}\!\left[\text{total future time in }I\right]
=\int_0^\infty P_{HI}^{(z)}(t)\,dt.
$$

Equivalently, this is the $(H,I)$ entry of the [fundamental matrix of an absorbing continuous-time Markov chain](../../../../../../fundamental-matrix-of-an-absorbing-continuous-time-markov-chain.md) $(-Q_{z,T})^{-1}$.

There is also a direct calculation. Each episode is fatal with probability $\delta/(\gamma+\delta)$, so the expected number of episodes before death is $(\gamma+\delta)/\delta$. Each lasts on average $1/(\gamma+\delta)$, giving

$$
\mathbb E_H^{(z)}[\text{total ill time}]=\frac1\delta=100\text{ days}.
$$

The acquisition rates change the waiting time between episodes but, under this model, not the total time eventually spent ill. Thus both risk groups have the same estimate.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
