<h1 id="2/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

If $m=0$, use a single color. Otherwise choose

$$
r=\max\left\{0,\left\lceil\log_3\frac{4m}{n}\right\rceil\right\}.
$$

The previous bound gives $\mathbb E B\leq n/4$, including the case $r=0$. By [Markov inequality](../../../../../../../markov-inequality.md), $\mathbb P(B>n/2)\leq1/2$. Sample the hyperplanes, count the monochromatic [edges](../../../../../../../edge-of-a-graph.md), and repeat if $B>n/2$. The success probability is at least $1/2$, so at most two draws are needed on average.

For a successful draw, select one endpoint of each monochromatic [edge](../../../../../../../edge-of-a-graph.md) and let $D$ be the union of the selected [vertices](../../../../../../../vertex-graph-theory.md). Then $|D|\leq B\leq n/2$. Every monochromatic [edge](../../../../../../../edge-of-a-graph.md) meets $D$, so the original colors give a proper [graph colouring](../../../../../../../graph-coloring.md) on the [induced subgraph](../../../../../../../induced-subgraph.md) with vertex set $W=V\setminus D$. Since $|W|\geq n/2$, the coloring of all [vertices](../../../../../../../vertex-graph-theory.md) is a [semicoloring](../../../../../../../semicoloring.md). This is a [random alteration method](../../../../../../../random-alteration-method.md); no additional colors for $D$ are required.

The number of available colors satisfies $2^r\leq2\max\{1,(4m/n)^{\log_3 2}\}$. A simple [graph](../../../../../../../graph-split.md) has $m\leq n(n-1)/2$, hence [semicoloring by independent hyperplanes](../../../../../../../semicoloring-by-independent-hyperplanes.md) gives

$$
\boxed{k=O(n^\gamma),\qquad\gamma=\log_3 2=\frac{\log2}{\log3}\approx0.63093<1.}
$$

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 339](../../../../paper-339-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
