<h1 id="17g/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

If the edge $uv$ lies in no triangle, no vertex can be adjacent to both endpoints; hence the [neighbourhoods](../../../../../../vertex-neighbourhood.md) satisfy $\Gamma(u)\cap\Gamma(v)=\varnothing$.

Suppose $|\Gamma(u)|+|\Gamma(v)|=2n$. The two disjoint neighbourhoods then partition $V(G)$. If both were [independent](../../../../../../independent-set-graph-theory.md), every edge would run between these two parts, so $G$ would be [bipartite](../../../../../../bipartite-graph.md) and

$$
e(G)\leq|\Gamma(u)|\,|\Gamma(v)|
\leq\left(\frac{|\Gamma(u)|+|\Gamma(v)|}{2}\right)^2=n^2,
$$

contrary to $e(G)=n^2+1$. Thus at least one neighbourhood contains an edge, and that edge forms a triangle with $u$ or $v$.

We now prove by induction on $n\geq2$ the [Triangle lower bound one edge above the Mantel threshold](../../../../../../triangle-lower-bound-one-edge-above-the-mantel-threshold.md): every graph on $2n$ vertices with at least $n^2+1$ edges has at least $n$ triangles. Part (ii) is the base case. For $n\geq3$, if every edge lies in a triangle, part (iii) gives

$$
t(G)\geq\frac{n^2+1}{3}\geq n.
$$

Otherwise choose an edge $uv$ lying in no triangle and put $s=d(u)+d(v)\leq2n$. Deleting $u,v$ removes $s-1$ edges, so the graph $G'=G-u-v$ has

$$
e(G')=n^2+2-s\geq(n-1)^2+1.
$$

If $s=2n$, induction gives at least $n-1$ triangles in $G'$, while the nonindependence proved above supplies a further triangle through $u$ or $v$.

If $s\leq2n-1$, then $e(G')\geq(n-1)^2+2$. Induction first supplies a triangle $\Delta$ in $G'$. Delete one edge of $\Delta$; the remaining graph still has at least $(n-1)^2+1$ edges, so induction supplies $n-1$ triangles avoiding that edge. Together with $\Delta$, these give at least $n$ distinct triangles in $G$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [17G](../../17g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
