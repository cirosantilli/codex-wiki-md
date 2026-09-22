<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Agglomerative hierarchical clustering](../../../../../../agglomerative-hierarchical-clustering.md) starts with each observation as a singleton [cluster in cluster analysis](../../../../../../cluster-in-cluster-analysis.md), repeatedly joins the closest pair of current clusters, and continues until one remains. The input is a [dissimilarity matrix](../../../../../../dissimilarity-matrix.md), so choosing variable scales and a scientifically sensible dissimilarity is part of the analysis.

Different linkages define closeness differently:

$$
\begin{aligned}
d_{\mathrm{single}}(A,B)&=\min_{i\in A,j\in B}d_{ij},\\
d_{\mathrm{complete}}(A,B)&=\max_{i\in A,j\in B}d_{ij},\\
d_{\mathrm{average}}(A,B)&=\frac1{|A||B|}\sum_{i\in A,j\in B}d_{ij}.
\end{aligned}
$$

[Single-linkage clustering](../../../../../../single-linkage-clustering.md) can connect elongated chains through nearest neighbors; [complete-linkage clustering](../../../../../../complete-linkage-clustering.md) emphasizes compact clusters; [average-linkage clustering](../../../../../../average-linkage-clustering.md) averages all cross-pair distances. For Euclidean observations, [Ward minimum-variance clustering](../../../../../../ward-minimum-variance-clustering.md) instead chooses the smallest increase in within-cluster squared error,

$$
\Delta(A,B)=\frac{|A||B|}{|A|+|B|}\|\bar x_A-\bar x_B\|^2.
$$

This follows by expanding squared deviations around the merged mean and using the zero sums of within-cluster residuals.

A [dendrogram](../../../../../../dendrogram.md) plots merge heights. In the lower-left sketch, two close pairs first merge at small heights, then join across a much larger separation; a horizontal cut between these heights yields two groups. **The hierarchy gives nested partitions, not a uniquely established number of populations.** Examine sensitivity to scaling, linkage and ties; once an agglomerative merge is made, the method does not undo it. The absence of a probability model also means that a visually attractive [dendrogram](../../../../../../dendrogram.md) is not itself a significance test.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
