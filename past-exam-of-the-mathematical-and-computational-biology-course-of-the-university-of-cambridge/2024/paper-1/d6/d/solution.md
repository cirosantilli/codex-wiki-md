<h1 id="d6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The diagram has all possible undirected [edges](../../../../../edge-of-a-graph.md) except $AB$: it is a [complete graph](../../../../../complete-graph.md) on five [vertices](../../../../../vertex-graph-theory.md) with one [edge](../../../../../edge-of-a-graph.md) removed. Therefore $A$ and $B$ each have three neighbours, while $C,D,E$ each have four.

The neighbours of $A$ and $B$ form a triangle, so their [clustering coefficients](../../../../../clustering-coefficient.md) equal one. Each of $C,D,E$ has five of the six possible neighbour–neighbour [edges](../../../../../edge-of-a-graph.md), giving $5/6$. The nodal [average shortest path length](../../../../../average-shortest-path-length.md) is $\ell_i=\frac14\sum_{j\ne i}d(i,j)$. All [graph distances](../../../../../distance-graph-theory.md) equal one except $d(A,B)=d(B,A)=2$, hence

$$
\boxed{\begin{array}{c|ccccc}
i&A&B&C&D&E\\\hline
k_i&3&3&4&4&4\\
C_i&1&1&5/6&5/6&5/6\\
\ell_i&5/4&5/4&1&1&1
\end{array}}.
$$

Averaging the nodal quantities gives

$$
\boxed{\bar C=\frac9{10}=0.9,\qquad L=\frac{11}{10}=1.1}.
$$

The ordered-pair distance sum is $22$, and the [graph diameter](../../../../../graph-diameter.md) is two.

If the intended unnormalized “small-worldness” is the ratio of clustering to path length, the computed quantities give

$$
\boxed{\frac{\bar C}{L}=\frac9{11}\approx0.818}.
$$

That ratio has no universal threshold for identifying a [small-world network](../../../../../small-world-network.md). The standard reference-normalized [small-worldness](../../../../../small-worldness.md), $\sigma=(\bar C/C_{\rm ref})/(L/L_{\rm ref})$, cannot receive a numerical value when no reference is specified and the question forbids using a [network null model](../../../../../network-null-model.md).[New measures of small-world-ness, Definitions 1–2](../../../../../network-%E2%80%98small-world-ness%E2%80%99-a-quantitative-method-for-determining-canonical-network-equivalence-by-mark-d-humphries-and-others.md)

**The graph has high clustering and short paths in the descriptive sense.** With nine of ten possible [edges](../../../../../edge-of-a-graph.md), however, those properties follow directly from its near completeness; they do not by themselves establish [small-world network](../../../../../small-world-network.md) structure relative to a reference. This distinguishes the metrics that can be computed directly from the stronger classification that requires a stated convention.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [D6](../../d6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
