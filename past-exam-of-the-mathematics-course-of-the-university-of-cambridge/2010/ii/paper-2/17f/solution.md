<h1 id="17f/solution">Solution</h1>

↑ **Parent:** [17F](../17f.md)

A [matching in a graph](../../../../../matching-graph-theory.md) from $X$ to $Y$ chooses one distinct neighbour in $Y$ for each vertex of $X$. For a finite [bipartite graph](../../../../../bipartite-graph.md), the [Hall marriage theorem](../../../../../hall-s-marriage-theorem.md) states that such a matching exists if and only if $|\Gamma(A)|\geq|A|$ for every $A\subseteq X$. Necessity follows because the matched neighbours of $A$ are distinct members of $\Gamma(A)$.

For sufficiency use induction on $|X|$, with the empty and one-vertex cases immediate. If some nonempty proper $A$ satisfies $|\Gamma(A)|=|A|$, the induced graph on $A,\Gamma(A)$ satisfies Hall's condition. The remaining graph on $X\setminus A,Y\setminus\Gamma(A)$ does too: for $B\subseteq X\setminus A$,

$$
|\Gamma(B)\setminus\Gamma(A)|=|\Gamma(A\cup B)|-|\Gamma(A)|\geq|B|.
$$

Inductively match both pieces and combine them. If no nonempty proper subset is tight, choose an edge $xy$ and remove its endpoints. Every nonempty subset $B$ of the remaining $X$ is proper in the original $X$, so $|\Gamma(B)|\geq|B|+1$; removing $y$ preserves Hall's condition. Match the remainder inductively and add $xy$. This proves the theorem without a flow or disjoint-path theorem.

## ↑ Ancestors (10)

1. [17F](../17f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
