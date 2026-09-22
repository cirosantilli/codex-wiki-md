<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The forward contract initiated at $t$ has payoff $S_T-F_t^T$ and zero value. Pricing under the [T-forward measure](../../../../../../t-forward-measure.md) gives

$$
0=B_t^T\mathbb E_{Q^T}[S_T-F_t^T\mid\mathcal F_t].
$$

Because $F_t^T$ is $\mathcal F_t$-measurable and $B_t^T>0$,

$$
F_t^T=\mathbb E_{Q^T}[S_T\mid\mathcal F_t].
$$

The [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) therefore makes $(F_t^T)_{t<T}$ a $Q^T$-martingale.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
