<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $P(t)=e^{Qt}$ be the [transition probability matrix](../../../../../../transition-semigroup-of-a-continuous-time-markov-chain.md) of the four-state [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md), and put $N=\{S,R\}$ for a negative test and $P=\{E,I\}$ for a positive test. Starting susceptible at time zero, the likelihood contribution is

$$
\sum_{a\in N}\sum_{b\in P}\sum_{c\in N}
P_{Sa}(1)P_{ab}(1)P_{bc}(1).
$$

Equivalently, with indicator diagonal matrices $D_N,D_P$ and the susceptible basis vector $e_S$ it is

$$
e_S^TP(1)D_NP(1)D_PP(1)D_N\mathbf1.
$$

This sums over every hidden state sequence compatible with the three test results.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
