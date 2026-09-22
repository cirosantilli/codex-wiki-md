<h1 id="d6/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For the **[Barabási-Albert model](../../../../../../barabasi-albert-model.md)**, choose a connected seed [graph](../../../../../../graph-split.md) on $m_0$ [vertices](../../../../../../vertex-graph-theory.md), the number $m\leq m_0$ of new [edges](../../../../../../edge-of-a-graph.md) per added [vertex](../../../../../../vertex-graph-theory.md), and a final size $n$. A complete seed with $m_0\geq2$ suffices. Add one [vertex](../../../../../../vertex-graph-theory.md) at a time, attaching it to $m$ distinct existing [vertices](../../../../../../vertex-graph-theory.md) selected with weights proportional to their current [vertex degrees](../../../../../../degree-graph-theory.md). Exclude duplicate [edges](../../../../../../edge-of-a-graph.md) and [self-loops](../../../../../../loop-graph-theory.md).

Increasing $n$ creates a larger network and permits older hubs to grow. Increasing $m$ makes the [graph](../../../../../../graph-split.md) denser, with asymptotic average [vertex degree](../../../../../../degree-graph-theory.md) $2m$, and tends to shorten [graph distances](../../../../../../distance-graph-theory.md). The seed affects early structure and the oldest hubs; standard linear [preferential attachment](../../../../../../preferential-attachment.md) gives a robust large-size tail exponent.

Its asymptotic [degree distribution](../../../../../../degree-distribution.md) is $P(k)\propto k^{-3}$, so **it is a [scale-free network](../../../../../../scale-free-network.md)**. Hubs produce short [average shortest path length](../../../../../../average-shortest-path-length.md), but elevated [clustering coefficients](../../../../../../clustering-coefficient.md) are not automatic: $m=1$ with a tree seed gives a triangle-free [tree](../../../../../../tree-graph-theory-split.md), and clustering decreases with size in the standard model. **The strict clustered [small-world network](../../../../../../small-world-network.md) property is therefore not guaranteed.**[pp. 510–511, growth, attachment and degree exponent](../../../../../../emergence-of-scaling-in-random-networks-by-albert-laszlo-barabasi-and-reka-albert.md)

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [D6](../../../d6.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../../split.md)
7. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
