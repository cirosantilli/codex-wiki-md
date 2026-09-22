<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $K(y\mid x)$ be a [Markov kernel](../../../../../../markov-kernel.md), and let $P_Y=PK$, $Q_Y=QK$ be the output [probability distributions](../../../../../../probability-distribution.md). Applying the [log-sum inequality](../../../../../../log-sum-inequality.md) for each $y$ to $a_x=P(x)K(y\mid x)$ and $b_x=Q(x)K(y\mid x)$ gives

$$
\sum_xP(x)K(y\mid x)\log\frac{P(x)}{Q(x)}
\geq P_Y(y)\log\frac{P_Y(y)}{Q_Y(y)}.
$$

Summing over $y$ and using $\sum_yK(y\mid x)=1$ yields the [data processing inequality for relative entropy](../../../../../../data-processing-inequality-for-relative-entropy.md)

$$
\boxed{D(PK\Vert QK)\leq D(P\Vert Q).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
