<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the closed set

$$
E_\epsilon=\left\{P:
\left|\sum_{a\in\mathcal A}P(a)f(a)-\mu\right|\geq\epsilon
\right\}.
$$

It does not contain $Q$. Since the probability simplex is compact, $Q$ has full support, and [Kullback-Leibler divergence](../../../../../../kullback-leibler-divergence.md) is continuous and vanishes only at $Q$,

$$
c_\epsilon=\inf_{P\in E_\epsilon}D(P\|Q)>0.
$$

The event in the question is exactly $\{\widehat P_n\in E_\epsilon\}$. The upper-bound half of [Sanov theorem](../../../../../../sanov-theorem.md) gives probability at most a polynomial factor times $2^{-nc_\epsilon}$, which tends to zero. This proves the [weak law of large numbers](../../../../../../weak-law-of-large-numbers.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
