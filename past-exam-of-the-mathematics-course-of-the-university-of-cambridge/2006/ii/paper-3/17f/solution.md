<h1 id="17f/solution">Solution</h1>

↑ **Parent:** [17F](../17f.md)

Define the asymmetric [Ramsey number](../../../../../ramsey-number.md) $R(s,t)$ for a red $K_s$ or a blue $K_t$. The base cases $R(1,t)=R(s,1)=1$ are finite. If $n=R(s-1,t)+R(s,t-1)$, choose a vertex of $K_n$. Its red neighbors number at least $R(s-1,t)$, or its blue neighbors number at least $R(s,t-1)$. Apply the appropriate smaller [Ramsey number](../../../../../ramsey-number.md) inside that neighborhood: either the opposite-color clique already exists, or a same-color clique extends by the chosen vertex. Thus $R(s,t)\le R(s-1,t)+R(s,t-1)$, proving finiteness by induction, in particular for $R(s)=R(s,s)$.

In a graph of [maximum degree](../../../../../maximum-degree.md) $d\ge2$, a ball of radius $k-1$ about a vertex has at most $\sum_{j=0}^{k-1}d^j=(d^k-1)/(d-1)<d^k$ vertices. Hence a connected graph of order $d^k$ has a vertex outside this ball, at distance at least $k$. The argument also applies whenever the graph has at least $d^k$ vertices.

Now take a connected graph of order $R(s)^s$. If some vertex has at least $R(s)$ neighbors, apply the two-color [Ramsey theorem](../../../../../ramsey-theorem.md) to their pairs, coloring an edge red and a nonedge blue. A red $K_s$ is an induced complete graph, while a blue $K_s$ is an independent set of $s$ neighbors, which with the centre induces $K_{1,s}$. Otherwise the [maximum degree](../../../../../maximum-degree.md) satisfies $d<R(s)$. For $s\ge2$, connectedness and the vertex count rule out $d\le1$. The ball bound then provides vertices at distance at least $s$. A shortest path between them has no chord, since a chord would shorten it; its first $s$ edges induce $P_s$. The case $s=1$ is immediate. Therefore

$$
\boxed{C(s)\le R(s)^s.}
$$

## ↑ Ancestors (10)

1. [17F](../17f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
