<h1 id="17h/solution">Solution</h1>

↑ **Parent:** [17H](../17h.md)

Let $R(s,t)$ be the two-colour [clique](../../../../../clique-graph-theory.md) Ramsey number. At a vertex of $K_{R(s-1,t)+R(s,t-1)}$, either its red neighbourhood has at least $R(s-1,t)$ vertices or its blue neighbourhood has at least $R(s,t-1)$. In the first case a red $(s-1)$-[clique](../../../../../clique-graph-theory.md) extends through the vertex, or there is a blue $t$-[clique](../../../../../clique-graph-theory.md); the second case is symmetric. Hence

$$
R(s,t)\le R(s-1,t)+R(s,t-1).
$$

With $R(1,t)=R(s,1)=1$, induction and Pascal's identity give $R(s,t)\le\binom{s+t-2}{s-1}$. Taking $s=t$ proves

$$
\boxed{R(K_t)\le\binom{2t-2}{t-1}.}
$$

The four-vertex graph is the [paw graph](../../../../../paw-graph.md), a triangle with a pendant edge; the copy need not be induced. For the lower bound, colour two disjoint triangles in $K_6$ red and all edges between them blue. Red components have only three vertices and blue is bipartite, so neither colour contains a paw. Thus $R(H)\ge7$.

For the upper bound, $R(3,3)\le6$ guarantees a monochromatic triangle in $K_7$, say red on a vertex set $T$. A red edge from $T$ to any outside vertex immediately supplies a red paw. Otherwise all edges from $T$ to the remaining four vertices are blue. If those four vertices contain a blue edge $ab$, then $a,b$ and any vertex of $T$ form a blue triangle, and another vertex of $T$ joined to $a$ supplies its pendant edge. If they contain no blue edge, they are a red $K_4$, which contains a red paw. Therefore

$$
\boxed{R(H)=7.}
$$

## ↑ Ancestors (10)

1. [17H](../17h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
