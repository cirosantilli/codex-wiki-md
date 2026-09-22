<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the clock states modulo $M$. The [detailed balance equations](../../../../../../detailed-balance.md) are $p_m\lambda_m=\nu p_{m-1}$. The product condition makes these equations consistent around the circle, so the [stationary distribution](../../../../../../stationary-distribution.md) is

$$
\boxed{p_m=\frac{w_m}{\sum_{k=0}^{M-1}w_k},\qquad w_0=1,\qquad w_m=\prod_{j=1}^{m}\frac{\nu}{\lambda_j}.}
$$

Indeed, the rate of the [time reversal of a continuous-time Markov chain](../../../../../../time-reversal-of-a-continuous-time-markov-chain.md) along a clockwise edge is $p_{m+1}\lambda_{m+1}/p_m=\nu$, while its anticlockwise rate is $p_{m-1}\nu/p_m=\lambda_m$. Thus the clock is a [reversible Markov chain](../../../../../../reversible-markov-chain.md).

The reversed clockwise transitions can be driven by a single independent rate-$\nu$ [Poisson process](../../../../../../poisson-process.md), since their rate does not depend on the clock state. They correspond to the original anticlockwise transitions. Consequently **the anticlockwise event times form a stationary Poisson process of rate $\nu$**. Its events before a given time are independent of the clock state at that time, which is the relevant [quasireversibility](../../../../../../quasireversibility.md) property. If clockwise and anticlockwise transitions have the same destination, their direction is retained as an event mark when reversing the process.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
