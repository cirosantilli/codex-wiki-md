<h1 id="9f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Again assume independent die scores. Their sum has the discrete [convolution](../../../../../../convolution.md) of the two score distributions, so

$$
\boxed{P(X=2)=p_1q_1,\qquad
P(X=7)=\sum_{i=1}^6p_iq_{7-i},\qquad
P(X=12)=p_6q_6.}
$$

All terms are nonnegative. The [arithmetic-geometric mean inequality](../../../../../../arithmetic-geometric-mean-inequality.md) applied to the two extreme-score contributions gives

$$
P(X=7)\geq p_1q_6+p_6q_1
\geq2\sqrt{p_1q_6p_6q_1}
=2\sqrt{P(X=2)P(X=12)}.
$$

If all eleven probabilities were equal, normalization would make each $1/11$, but the inequality would require $1/11\geq2/11$. This contradiction proves **the sum cannot be uniform on $\{2,\ldots,12\}$**, whatever the individual die probabilities.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [9F](../../9f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
