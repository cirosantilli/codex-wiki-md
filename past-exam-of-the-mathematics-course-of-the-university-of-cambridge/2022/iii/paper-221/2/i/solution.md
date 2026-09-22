<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take all components to be centered and let their marginal variances be $V_A,V_C,V_E$. A [linear structural equation model](../../../../../../linear-structural-equation-model.md) is

$$
C_{i1}=C_{i2}=C_i,
\qquad
Y_{ij}=A_{ij}+C_i+E_{ij},
$$

where $C_i,E_{i1},E_{i2}$ are mutually independent and the $E_{ij}$ are identically distributed. The [causal directed acyclic graph](../../../../../../causal-directed-acyclic-graph.md) has arrows

$$
A_{i1}\to Y_{i1}\leftarrow C_i\to Y_{i2}\leftarrow A_{i2},
\qquad
E_{i1}\to Y_{i1},
\qquad
E_{i2}\to Y_{i2}.
$$

For [monozygotic twins](../../../../../../monozygotic-twin.md), set $A_{i1}=A_{i2}=G_i$ with $\operatorname{Var}(G_i)=V_A$; the genetic cause is completely shared. For [dizygotic twins](../../../../../../dizygotic-twin.md), one explicit construction is

$$
A_{i1}=G_i+G_{i1},
\qquad
A_{i2}=G_i+G_{i2},
$$

where $G_i,G_{i1},G_{i2}$ are independent with variance $V_A/2$. Then both additive genetic terms have variance $V_A$, while their covariance is $V_A/2$ and their [correlation coefficient](../../../../../../pearson-correlation-coefficient.md) is $1/2$. In a fuller graph, the shared $G_i$ points to both genetic components and the unique $G_{ij}$ points only to its own component.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
