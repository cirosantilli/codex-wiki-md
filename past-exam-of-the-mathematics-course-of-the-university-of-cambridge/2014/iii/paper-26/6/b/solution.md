<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $Z=X+Y$, where the two [Lévy processes](../../../../../../levy-process.md) are independent as processes. For any disjoint ordered time intervals, the increment vectors of $X$ and $Y$ are independent of one another, and each vector has independent coordinates. Thus the pairs of corresponding increments are independent across intervals, and so are their sums. The law of each summed increment is the convolution of the two increment laws, depending only on the interval length. This proves [independent increments](../../../../../../independent-increments.md) and [stationary increments](../../../../../../stationary-increments.md) for $Z$.

Also $Z_0=0$, and for every $\varepsilon>0$,

$$
\mathbb P(|Z_s-Z_t|>\varepsilon)
\leq\mathbb P(|X_s-X_t|>\varepsilon/2)+\mathbb P(|Y_s-Y_t|>\varepsilon/2)\longrightarrow0.
$$

Thus $Z$ is [stochastically continuous](../../../../../../stochastic-continuity.md). The sum of two [càdlàg](../../../../../../cadlag.md) functions is [càdlàg](../../../../../../cadlag.md). **All defining properties hold, so $X+Y$ is a [Lévy process](../../../../../../levy-process.md).** Independence of the entire two processes, not merely equality of some one-time laws, is what supplies independent summed increments.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
