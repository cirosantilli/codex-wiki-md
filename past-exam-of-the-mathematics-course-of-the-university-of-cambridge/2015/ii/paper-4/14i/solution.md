<h1 id="14i/solution">Solution</h1>

↑ **Parent:** [14I](../14i.md)

A [matching in a graph](../../../../../matching-graph-theory.md) from $X$ to $Y$ is a collection of edges with disjoint endpoints covering every vertex of $X$; equivalently it chooses a distinct neighbour in $Y$ for each $x\in X$. For a finite [bipartite graph](../../../../../bipartite-graph.md), the [Hall marriage theorem](../../../../../hall-s-marriage-theorem.md) says this exists exactly when $|N(A)|\geq|A|$ for every $A\subseteq X$. Necessity follows by counting the distinct matched neighbours.

For sufficiency, induct on $|X|$. If a nonempty proper subset $A$ is tight, $|N(A)|=|A|$, Hall's condition holds on $(A,N(A))$. It also holds on $(X\setminus A,Y\setminus N(A))$: for $B\subseteq X\setminus A$, the original condition applied to $A\cup B$ gives $|N(B)\setminus N(A)|\geq|B|$. Induction provides two disjoint [matching in a graph](../../../../../matching-graph-theory.md) whose union covers $X$. If no nonempty proper subset is tight, choose an edge $xy$, possible by Hall's condition. Delete its endpoints. Each nonempty subset of $X\setminus\{x\}$ had at least one extra neighbour, so deleting $y$ leaves Hall's condition intact. Induction and then the edge $xy$ finish the proof. The single-vertex case is immediate.

For the degree condition, fix $A\subseteq X$ and double-count with weights:

$$
|N(A)|\geq\sum_{y\in N(A)}\frac{d_A(y)}{d(y)}
=\sum_{x\in A}\sum_{y\sim x}\frac1{d(y)}
\geq\sum_{x\in A}\frac{d(x)}{d(x)}=|A|.
$$

Every denominator is nonzero; the last inequality uses $d(y)\leq d(x)$ along each edge. The [Hall marriage theorem](../../../../../hall-s-marriage-theorem.md) therefore proves **the required matching exists**. Finiteness, as in the usual course version of the theorem, is understood; the same proof covers a finite $X$ with arbitrary $Y$ and finite degrees.

## ↑ Ancestors (10)

1. [14I](../14i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
