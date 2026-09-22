<h1 id="d6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [network null model](../../../../../network-null-model.md) is an ensemble representing a specified baseline against which to assess an observed biological network. It should preserve the features that would otherwise confound the test: at least the number of [vertices](../../../../../vertex-graph-theory.md) and [edges](../../../../../edge-of-a-graph.md), and often the [degree sequence](../../../../../degree-sequence.md), direction, edge type, or relevant spatial constraints. It should randomize the feature whose biological organization is under investigation. An ensemble that preserves that very feature cannot test whether the feature is unusual.

For example, test whether a measured [protein-protein interaction network](../../../../../protein-protein-interaction-network.md) contains more closed three-protein interaction groups than can be explained by the interaction counts of individual [proteins](../../../../../protein-split.md). Define [vertices](../../../../../vertex-graph-theory.md) as the measured [proteins](../../../../../protein-split.md) and an undirected [edge](../../../../../edge-of-a-graph.md) as a reproducible detected interaction, using a fixed assay threshold and treatment of duplicates. Preselect the triangle count as the test statistic. Generate many simple [random graphs](../../../../../random-graph-split.md) by [degree-preserving edge rewiring](../../../../../degree-preserving-edge-rewiring.md), rejecting [self-loops](../../../../../loop-graph-theory.md) and duplicate [edges](../../../../../edge-of-a-graph.md), with enough accepted swaps and separation to obtain a well-mixed reference sample. This retains the observed [degree sequence](../../../../../degree-sequence.md) while disrupting higher-order association.

Compute the same triangle count for every reference [graph](../../../../../graph-split.md). Compare the observed count with this distribution; an empirical upper-tail [p-value](../../../../../p-value.md) can be reported as $(1+\#\{T_{\rm null}\geq T_{\rm obs}\})/(M+1)$ for $M$ suitably sampled reference [graphs](../../../../../graph-split.md). Report the size of the excess as well as its tail frequency, and check sensitivity to the assay threshold and any required connectivity constraint. A significant excess is evidence beyond the chosen degree baseline, while assay bias or spatial organization omitted from that baseline can still explain it.

A generative network model specifies a mechanism for producing networks, such as growth with [preferential attachment](../../../../../preferential-attachment.md), and asks what structures that mechanism creates. A [network null model](../../../../../network-null-model.md) is defined by its role as a comparison baseline. These roles can overlap: the same random mechanism can be a proposed biological explanation in one analysis and a deliberately simplified null in another.

## ↑ Ancestors (13)

1. [A](../a.md)
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
