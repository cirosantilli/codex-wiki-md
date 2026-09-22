<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

If $X=0$, every pair of [vertices](../../../../../../../vertex-graph-theory.md) has a [common neighbour](../../../../../../../common-neighbour.md), so every pair has [graph distance](../../../../../../../distance-graph-theory.md) at most two. In particular the [graph](../../../../../../../graph-split.md) is [connected](../../../../../../../connected-space.md) and its [graph diameter](../../../../../../../graph-diameter.md) is at most two. By the [Markov inequality](../../../../../../../markov-inequality.md) and part (ii),

$$
\mathbb P(\operatorname{diam}G(n,p)>2)
\leq\mathbb P(X>0)
\leq\binom n2(1-p^2)^{n-2}\longrightarrow0.
$$

We include disconnected graphs among those with diameter greater than two. Therefore

$$
\boxed{\mathbb P(\operatorname{diam}G(n,p)\leq2)\longrightarrow1},
$$

by [diameter bound for a fixed-density binomial random graph](../../../../../../../diameter-bound-for-a-fixed-density-binomial-random-graph.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 36](../../../../paper-36-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
