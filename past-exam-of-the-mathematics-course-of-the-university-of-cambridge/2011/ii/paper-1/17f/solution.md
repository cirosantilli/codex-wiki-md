<h1 id="17f/solution">Solution</h1>

↑ **Parent:** [17F](../17f.md)

A [matching in a graph](../../../../../matching-graph-theory.md) is a set of edges with no shared endpoints. A matching from $X$ to $Y$ here covers every vertex of $X$. Necessity of the [Hall marriage theorem](../../../../../hall-s-marriage-theorem.md) condition is immediate: the partners of vertices of $A\subseteq X$ are distinct members of its neighbour set $\Gamma(A)$.

For sufficiency, take a matching of maximum size. If it leaves $x\in X$ unmatched, follow alternating unmatched and matched edges from $x$. Let $A\subseteq X$ and $B\subseteq Y$ be the reachable vertices. No vertex of $B$ can be unmatched, because the resulting [augmenting path in a matching](../../../../../augmenting-path-in-a-matching.md) would increase the matching. Every neighbour of $A$ is in $B$, and the matching pairs $B$ bijectively with $A\setminus\{x\}$. Thus $|\Gamma(A)|=|B|=|A|-1$, contradicting Hall's condition. The maximum matching therefore covers $X$.

For the deficiency bound, adjoin $d$ new vertices to $Y$, each adjacent to all of $X$. Every nonempty $A$ then has $|\Gamma(A)|+d\geq|A|$ neighbours. Apply the [Hall marriage theorem](../../../../../hall-s-marriage-theorem.md) and remove the at most $d$ edges using new vertices. This leaves **at least $|X|-d$ independent edges**. The lower bound is vacuous if $d>|X|$.

Write the [adjacency matrix of a graph](../../../../../adjacency-matrix.md) in bipartite block form $\left(\begin{smallmatrix}0&C\\C^T&0\end{smallmatrix}\right)$. If Hall's condition failed for $A\subseteq X$, the linear map from vectors supported on $A$ to their neighbour coordinates in $Y$ would have fewer output than input coordinates. It therefore has a nonzero [kernel](../../../../../kernel-of-a-linear-map.md), giving a nonzero vector $v$ supported on $A$ with $C^Tv=0$. The vector $(v,0)$ would be a zero [eigenvector](../../../../../eigenvector.md) of the adjacency matrix. Consequently **absence of the zero eigenvalue implies a matching covering $X$**.

The converse is **false**, even with equal part sizes. The four-cycle $K_{2,2}$ has a [perfect matching](../../../../../perfect-matching.md), but its matrix $C=\left(\begin{smallmatrix}1&1\\1&1\end{smallmatrix}\right)$ is singular. Its adjacency matrix has eigenvalues $2,-2,0,0$.

## ↑ Ancestors (11)

1. [17F](../17f.md)
2. [Section II](../section-ii.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ii](../../split.md)
5. [2011](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
