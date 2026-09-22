<h1 id="29k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a bounded [stopping time](../../../../../../stopping-time.md) $T\leq N$, write

$$
\widehat M_T=\widehat M_0+\sum_{n=1}^N1_{\{T\geq n\}}(\widehat M_n-\widehat M_{n-1}).
$$

The indicator is measurable at time $n-1$. Taking conditional expectations term by term and using the [supermartingale](../../../../../../supermartingale.md) inequality gives $\mathbb E\widehat M_T\leq\mathbb E\widehat M_0$. The same calculation gives equality for the [martingale](../../../../../../martingale-split.md) $M$. Since their initial values agree, $\mathbb E M_T\geq\mathbb E\widehat M_T$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [29K](../../29k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
