<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Writing $s_i=2x_i-1$, the edge term rewards neighboring computers having the same infection state, as in a ferromagnetic [Ising model](../../../../../../ising-model.md), while $-\frac1{10}\sum_i x_i$ expresses a mild prior preference for the rarer uninfected state. Thus the prior encodes local transmission over the network without assuming independent infections.

The observation likelihood is

$$
L(x)=\prod_{i\in V_2}\frac14\mathbf1_{\{x_i=1\}}
\prod_{i\in V_1\setminus V_2}\left(\frac34\right)^{x_i}.
$$

Consequently the [posterior distribution](../../../../../../bayesian-posterior.md) is

$$
p(x_V\mid V_2)
\propto
\exp\left[
\sum_{\{i,j\}\in E}(2x_i-1)(2x_j-1)
-\frac1{10}\sum_i x_i
\right]L(x).
$$

This remains a binary pairwise [Markov random field](../../../../../../markov-random-field.md) on a tree. To find its [maximum a posteriori estimate](../../../../../../maximum-a-posteriori-estimate.md), run [max-product belief propagation](../../../../../../max-product-belief-propagation.md): send a two-entry message in each direction along every edge, then backtrack from the maximizing root state. Each message examines four state pairs, and the maximum degree is bounded, so the total cost is

$$
\boxed{O(|V|).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
