<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a finite generating set $A$, use the symmetric alphabet $\Sigma=A\cup A^{-1}$. The [Cayley graph](../../../../../../cayley-graph.md) has a vertex for each $g\in G$ and an oriented edge labelled $a$ from $g$ to $ga$. Give every edge length one. Its vertex [word metric](../../../../../../word-metric.md) is

$$
\boxed{d_A(g,h)=\min\{|w|:w\text{ over }\Sigma\text{ represents }g^{-1}h\}}.
$$

Two [finitely presented groups](../../../../../../finitely-presented-group.md) are quasi-isometric when their [Cayley graphs](../../../../../../cayley-graph.md), with these [path](../../../../../../continuous-path.md) metrics, are quasi-isometric. The choice of finite generating set is immaterial, as the following proof shows; the [relators](../../../../../../relator.md) identify vertices but do not otherwise enter the metric definition.

Given finite generating sets $A,B$ of the same group, put $L=\max(1,\max_{a\in A^{\pm1}}|a|_B)$ and $M=\max(1,\max_{b\in B^{\pm1}}|b|_A)$. Replace each letter in a shortest $A$-word by a fixed $B$-word to obtain $|g|_B\le L|g|_A$. Reversing the roles gives $|g|_A\le M|g|_B$. Therefore the vertex identity map satisfies

$$
\boxed{M^{-1}d_A(g,h)\le d_B(g,h)\le Ld_A(g,h)}.
$$

It is onto, and hence a [quasi-isometry](../../../../../../quasi-isometry.md). Map each edge to the fixed word [path](../../../../../../continuous-path.md) for its label, or pass through the uniformly dense vertex sets, to obtain the corresponding graph [quasi-isometry](../../../../../../quasi-isometry.md) with a bounded additive error. This proves [equivalence of finite word metrics](../../../../../../equivalence-of-finite-word-metrics.md) and independence of the two [finite group presentations](../../../../../../finite-group-presentation.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
