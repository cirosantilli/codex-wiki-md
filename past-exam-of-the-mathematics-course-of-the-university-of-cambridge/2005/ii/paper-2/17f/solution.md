<h1 id="17f/solution">Solution</h1>

↑ **Parent:** [17F](../17f.md)

First suppose $G$ is 3-connected and noncomplete, and write $\Delta=\Delta(G)$. There is an induced path $a,v,b$ with $a,b$ nonadjacent: otherwise the first three vertices of any shortest path between nonadjacent vertices would contradict that assertion. Since $G$ is 3-connected, $G-\{a,b\}$ is a [connected graph](../../../../../connected-graph.md). Choose a [spanning tree](../../../../../spanning-tree.md) of that graph rooted at $v$. Color $a,b$ first with the same color, then color the other vertices in reverse tree order, leaving $v$ last. Every vertex except $v$ has its tree parent uncolored and thus at most $\Delta-1$ previously colored neighbors. At $v$, the two neighbors $a,b$ share a color, so again at most $\Delta-1$ colors are forbidden. This constructs a proper $\Delta$-coloring and proves **Brooks' bound for 3-connected noncomplete graphs**. A [complete graph](../../../../../complete-graph.md) is exactly the excluded case; a [3-connected graph](../../../../../3-connected-graph.md) cannot be an [odd cycle](../../../../../odd-cycle.md).

For the partition claim, assume $d_1,d_2$ are nonnegative integers with $d_1+d_2=\Delta-1$. Minimize

$$
\Phi=d_2e(G[V_1])+d_1e(G[V_2]).
$$

If a vertex in $V_1$ has internal degree $a\geq d_1+1$, its degree $b$ into $V_2$ is at most $d_2$. Moving it to $V_2$ changes $\Phi$ by $d_1b-d_2a\leq-d_2$, contradicting minimality when $d_2>0$. The analogous move handles a violation in $V_2$ when $d_1>0$. For a zero coefficient, break ties among minimizers by minimizing the total number of internal edges. If $d_2=0<d_1$, minimality of $\Phi=d_1e(G[V_2])$ ensures $V_2$ is [independent](../../../../../independent-random-variables.md); a violating vertex in $V_1$ has all its $\Delta=d_1+1$ neighbors in $V_1$ and no neighbor in $V_2$, so moving it reduces the tie-break quantity without increasing $\Phi$. The reversed argument handles $d_1=0$. If both are zero then $\Delta=1$, and the graph is a union of isolated vertices and edges, admitting two [independent](../../../../../independent-random-variables.md) parts. Thus

$$
\boxed{\Delta(G[V_i])\leq d_i\quad(i=1,2).}
$$

For $\Delta\geq5$, put $d_1=3,d_2=\Delta-4$. A maximum-degree-three graph containing no $K_4$ is 3-colorable. Here is why the previously proved 3-connected case suffices: [connected](../../../../../connected-space.md) graphs of degree at most two are paths or cycles and use at most three colors. Split a larger graph at cut vertices and permute colors when gluing. In a 2-connected cubic graph with a two-vertex cut $\{u,v\}$, a cut edge $uv$ gives colorings of the sides glued with their distinct endpoint colors. If $u,v$ are nonadjacent, the cut components have positive numbers of edges to both endpoints and the total endpoint degrees are at most three. There are at most three components. With three components, adding $uv$ to each side preserves [maximum degree](../../../../../maximum-degree.md) three and gives the endpoints degree two. No new $K_4$ is created, so induction supplies side colorings with distinct endpoint colors, which can be permuted to agree. With two components, the components incident twice to $u$ and twice to $v$ either agree or differ. If they differ, adding $uv$ to each side preserves [maximum degree](../../../../../maximum-degree.md) three; each augmented side is smaller and cannot be $K_4$, because one endpoint then has degree only two, so induction gives distinct-endpoint colorings. If they agree, call the side with only one edge from each endpoint the small side. Any coloring of the other side can be matched on it: for equal endpoint colors, contract $u,v$ in the small side (the merged vertex has degree at most two); for distinct colors add $uv$ (the endpoints again have degree two). Induction applies in both cases. A 2-connected graph with no two-vertex cut is 3-connected and was handled above. This proves the needed subcubic coloring fact without quoting the unproved full theorem.

Use three colors on $V_1$ and at most $d_2+1=\Delta-3$ fresh colors on $V_2$, by greedy coloring. This gives $\chi(G)\leq\Delta$. More usefully, repeatedly remove degree-at-most-three parts: the partition supplies a four-degree reduction for a cost of three colors. If $f(\Delta)=\frac34\Delta+\frac32$, then $3+f(\Delta-4)=f(\Delta)$. Induction in $\Delta$, with the remaining part still $K_4$-free, gives

$$
\boxed{\chi(G)\leq\frac34\Delta(G)+\frac32.}
$$

The base cases $\Delta=0,1,2,3$ use respectively $1,2,3,3$ colors, within this bound; at $\Delta=4$, Brooks' theorem would give four, but the same partition with $(3,0)$ gives a 3-colorable part and an [independent](../../../../../independent-random-variables.md) part, hence four. Thus the induction requires no unproved general Brooks theorem.

## ↑ Ancestors (10)

1. [17F](../17f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
