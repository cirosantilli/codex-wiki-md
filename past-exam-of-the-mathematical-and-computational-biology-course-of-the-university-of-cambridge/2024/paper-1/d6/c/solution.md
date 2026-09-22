<h1 id="d6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The supplied [adjacency matrix](../../../../../adjacency-matrix.md) describes a four-[vertex](../../../../../vertex-graph-theory.md) [cycle graph](../../../../../cycle-graph.md), with every [vertex degree](../../../../../degree-graph-theory.md) equal to two. [Degree-preserving edge rewiring](../../../../../degree-preserving-edge-rewiring.md) is random, so it does not determine one unique labelled output [adjacency matrix](../../../../../adjacency-matrix.md). For example, replace [edges](../../../../../edge-of-a-graph.md) $AB$ and $CD$ by $AC$ and $BD$, retaining $AD$ and $BC$. This valid switch gives, in order $A,B,C,D$,

$$
\boxed{A'=\begin{pmatrix}
0&0&1&1\\
0&0&1&1\\
1&1&0&0\\
1&1&0&0
\end{pmatrix}}.
$$

Each row still sums to two. Under the [simple graph](../../../../../simple-graph.md) convention, all allowed outputs have the same unlabelled four-cycle topology: there are three possible labelled four-cycles. A rejected switch or later return can also leave the original [adjacency matrix](../../../../../adjacency-matrix.md).

**It is not a [scale-free network](../../../../../scale-free-network.md).** Its [degree distribution](../../../../../degree-distribution.md) is concentrated entirely at degree two, with no power-law tail; [degree-preserving edge rewiring](../../../../../degree-preserving-edge-rewiring.md) cannot change that.

## ↑ Ancestors (13)

1. [C](../c.md)
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
