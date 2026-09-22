<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A density factorizes according to a [Directed acyclic graph](../../../../../../directed-acyclic-graph.md) when

$$
f(v_1,\ldots,v_p)=\prod_{j=1}^p
f(v_j\mid v_{\operatorname{pa}(j)}),
$$

where $\operatorname{pa}(j)$ is the set of parents of vertex $j$.

The required undirected graph is the [moral graph](../../../../../../moral-graph.md): join every pair of parents having a common child, retain the parent-child adjacencies, and remove all arrowheads. Each DAG family $\{j\}\cup\operatorname{pa}(j)$ is then a clique, so each conditional factor is a clique potential and the DAG factorization is also an undirected factorization. These edges are minimal for a guarantee covering every DAG-factorizing density, because an arbitrary conditional factor can couple every pair of variables in its family.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
