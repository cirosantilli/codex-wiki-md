<h1 id="d6/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the **[Erdős-Rényi model](../../../../../../erdos-renyi-model.md) $G(n,p)$**, choose the number $n$ of [vertices](../../../../../../vertex-graph-theory.md) and an edge [probability](../../../../../../probability.md) $0\leq p\leq1$. Visit every unordered pair of distinct [vertices](../../../../../../vertex-graph-theory.md) once and include its [edge](../../../../../../edge-of-a-graph.md) independently with [probability](../../../../../../probability.md) $p$. This construction gives a [simple graph](../../../../../../simple-graph.md) with expected edge count $p\binom n2$ and mean [vertex degree](../../../../../../degree-graph-theory.md) $p(n-1)$.

Increasing $p$ at fixed $n$ makes the [graph](../../../../../../graph-split.md) denser, increases typical [vertex degree](../../../../../../degree-graph-theory.md) and local [clustering coefficient](../../../../../../clustering-coefficient.md), and tends to shorten [graph distances](../../../../../../distance-graph-theory.md) and improve connectivity. Increasing $n$ at fixed $p$ also increases the mean [vertex degree](../../../../../../degree-graph-theory.md); to retain a sparse comparison one instead decreases $p$ approximately as $1/n$.

Its [degree distribution](../../../../../../degree-distribution.md) is [binomial distribution](../../../../../../binomial-distribution.md), approximately [Poisson distribution](../../../../../../poisson-distribution.md) in the sparse large-$n$ regime, so it is **not a [scale-free network](../../../../../../scale-free-network.md)**. Connected realizations can have short [average shortest path length](../../../../../../average-shortest-path-length.md), but their [clustering coefficients](../../../../../../clustering-coefficient.md) are not elevated above the random baseline they themselves define. Thus they are **not [small-world networks](../../../../../../small-world-network.md) under the high-clustering convention**, although “small world” is sometimes used more loosely to mean only short distances.

## ↑ Ancestors (14)

1. [I](../i.md)
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
