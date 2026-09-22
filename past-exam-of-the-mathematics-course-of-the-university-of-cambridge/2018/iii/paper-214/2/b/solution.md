<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $m\geq1$, let $S_m$ be the set of vertices of $B(m)$ connected to $\partial B(m)$ by an open [path in a graph](../../../../../../path-in-a-graph.md) using only edges of $B(m)$. Every infinite-cluster vertex of $B(m)$ belongs to $S_m$, by stopping an infinite open [path in a graph](../../../../../../path-in-a-graph.md) at its first boundary visit. Hence the [increasing event](../../../../../../increasing-event.md)

$$
E_m=\{|S_m|\geq\theta(p)(2m+1)^2/2\}
$$

has probability at least $\theta(p)/2$ by part (a). Importantly, $E_m$ depends only on the edges with both endpoints in $B(m)$.

Open all $8m$ perimeter edges joining successive vertices of $\partial B(m)$. They form a [cycle in a graph](../../../../../../cycle-in-a-graph.md), and opening them joins every vertex of $S_m$ into one [percolation cluster](../../../../../../percolation-cluster.md), containing the specified perimeter vertex $v_m=(m,0)$. The [Harris-FKG inequality](../../../../../../harris-fkg-inequality.md) bounds the probability of this event together with $E_m$ below by $p^{8m}\theta(p)/2$.

Close all $8m+4$ edges in the [edge boundary](../../../../../../edge-boundary-in-a-graph.md) of $B(m)$. These edges are distinct from the internal edges already considered, so their states are independent of those events. The resulting [percolation cluster](../../../../../../percolation-cluster.md) of $v_m$ is finite, contained in $B(m)$, and has at least $|S_m|$ vertices. Therefore, by translating $v_m$ to the origin,

$$
\mathbb P_p\bigl(\theta(p)(2m+1)^2/2\leq|C|<\infty\bigr)\geq\frac{\theta(p)}2p^{8m}(1-p)^{8m+4}.
$$

For $n\geq1$, choose $m=\lceil\sqrt{n/(2\theta(p))}\rceil$. Then the threshold is at least $n$, and $m\leq(1+(2\theta(p))^{-1/2})\sqrt n$. Put $A=-\log p$ and $B=-\log(1-p)$; both are positive. The preceding lower bound is at least $e^{-c_1\sqrt n}$ with, for example,

$$
\boxed{c_1=8(A+B)\left(1+\frac1{\sqrt{2\theta(p)}}\right)+4B+\log\frac2{\theta(p)},\qquad
\mathbb P_p(n\leq|C|<\infty)\geq e^{-c_1\sqrt n}.}
$$

The construction modifies only order-$m$ boundary edges while trapping order-$m^2$ vertices, which explains the [stretched exponential](../../../../../../stretched-exponential-function.md) scale. Here $\mathbb N$ is interpreted as the positive integers; the proposed lower bound at $n=0$ would be false because $\theta(p)>0$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 214](../../../paper-214-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
