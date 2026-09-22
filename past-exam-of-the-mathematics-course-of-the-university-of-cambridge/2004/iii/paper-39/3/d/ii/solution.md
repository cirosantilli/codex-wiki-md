<h1 id="3/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the undirected representation of the [pedigree graphical model](../../../../../../../pedigree-graphical-model.md), take the [moral graph](../../../../../../../moral-graph.md): remove arrowheads from all parent-child edges and join coparents. The added coparent edges are

$$
UV,\quad PQ,\quad RS,\quad AB,\quad CD,\quad FM.
$$

Every [Mendelian segregation](../../../../../../../mendelian-segregation.md) factor involves a child and its two parents, so its variables form a [clique](../../../../../../../clique-graph-theory.md) in this graph. The product in the previous part is thus an undirected factorization. A separation of variables by a conditioning set in this graph implies the corresponding [conditional independence](../../../../../../../conditional-independence.md).

This is a valid [conditional independence graph](../../../../../../../conditional-independence-graph.md) representation of the joint genotype law. It need not be its minimal representation without a [faithfulness of a directed acyclic graph](../../../../../../../faithfulness-of-a-directed-acyclic-graph.md) assumption: some inheritance probabilities are zero, and special parameter choices can yield additional independences. It also differs from a graph of unconditioned correlations, since [full siblings](../../../../../../../full-sibling.md) remain correlated through their parents when the parental genotypes are not conditioned on.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [Paper 39](../../../../paper-39-split.md)
5. [Iii](../../../../split.md)
6. [2004](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
