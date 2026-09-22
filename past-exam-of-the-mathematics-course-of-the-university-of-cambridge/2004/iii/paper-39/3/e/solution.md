<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

A valid [triangulation of an undirected graph](../../../../../../triangulation-of-an-undirected-graph.md) adds exactly the two fill edges

$$
\boxed{AC\quad\text{and}\quad AM.}
$$

To verify it, eliminate the vertices in the order $P,Q,R,S,X,Y,B,D,F,M,A,C,U,V$. The first eight eliminations have neighboring vertices already joined. When $F$ is eliminated, its remaining neighbors are $A,M$, so add $AM$. When $M$ is eliminated, its remaining neighbors are $A,C$, so add $AC$. The remaining $A,C,U,V$ form a [clique](../../../../../../clique-graph-theory.md).

Thus this order is a [perfect elimination ordering](../../../../../../perfect-elimination-ordering.md) of the completed graph, which is a [chordal graph](../../../../../../chordal-graph.md). The fill edges are computational devices for genotype elimination; they do not add parent-child relationships to the [pedigree](../../../../../../pedigree.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
