<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Because $\chi(H)=3$, every bipartite graph is $H$-free. The balanced complete bipartite graph therefore gives

$$
\liminf_{n\to\infty}\frac{\operatorname{ex}(n,H)}{\binom n2}\ge\frac12.
$$

For the reverse bound, fix $\delta>0$ and suppose that $G$ has more than $(1/2+\delta)\binom n2$ edges. Apply the [Szemerédi regularity lemma](../../../../../../szemeredi-regularity-lemma.md) with parameters much smaller than $\delta$. Form the reduced graph whose vertices are the regularity classes and whose edges are the regular pairs of density above a small fixed threshold. Edges inside classes, irregular pairs, and regular pairs below the threshold account for $o_\delta(n^2)$ edges. The remaining edges force the reduced graph to have more than $m^2/4$ edges.

By the [Turan theorem](../../../../../../turan-s-theorem.md), the reduced graph contains a triangle. The three corresponding regular pairs all have positive density, and the [graph embedding lemma for regular pairs](../../../../../../graph-embedding-lemma-for-regular-pairs.md) embeds every fixed three-colourable graph, in particular $H$, across suitable repeated subclusters of these three classes. Thus every sufficiently large graph of density above $1/2+\delta$ contains $H$. Letting $\delta\downarrow0$ gives

$$
\boxed{\lim_{n\to\infty}\frac{\operatorname{ex}(n,H)}{\binom n2}=\frac12.}
$$

This is the chromatic-number-three case of the [Erdős-Stone theorem](../../../../../../erdos-stone-theorem.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 132](../../../paper-132-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
