<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $r=|V_0|$, $s=|V_1|$, and $e=|E(G)|=\alpha|X||Y|$. We construct a random [graph homomorphism](../../../../../graph-homomorphism.md) $\Psi:T\to G$. Choose a root of the [tree](../../../../../tree-graph-theory.md). Map it according to the [degree-biased vertex distribution](../../../../../degree-biased-vertex-distribution.md) on the corresponding side of the [bipartite graph](../../../../../bipartite-graph.md); after mapping any vertex, map each child independently and uniformly to a neighbour of its parent's image.

Every oriented tree edge is then mapped uniformly onto the $e$ edges of $G$. Every tree vertex in $V_0$ has the degree-biased marginal on $X$, of entropy $H_X$, and every vertex in $V_1$ has the analogous marginal of entropy $H_Y$. Repeated use of the [chain rule for information entropy](../../../../../chain-rule-for-information-entropy.md) along the rooted tree gives

$$
H(\Psi)
=(k-1)\log e
-\sum_{v\in V_0}(\deg_Tv-1)H_X
-\sum_{v\in V_1}(\deg_Tv-1)H_Y.
$$

Since a $k$-vertex [tree](../../../../../tree-graph-theory.md) has $k-1$ edges,

$$
\sum_{v\in V_0}(\deg_Tv-1)=s-1,
\qquad
\sum_{v\in V_1}(\deg_Tv-1)=r-1.
$$

The [maximum entropy distribution on a finite set](../../../../../maximum-entropy-distribution-on-a-finite-set.md) gives $H_X\leq\log|X|$ and $H_Y\leq\log|Y|$. Hence

$$
\begin{aligned}
H(\Psi)
&\geq(k-1)\log(\alpha|X||Y|)
-(s-1)\log|X|-(r-1)\log|Y|\\
&=\log\!\left(\alpha^{k-1}|X|^r|Y|^s\right).
\end{aligned}
$$

If $N$ is the number of bipartition-respecting [graph homomorphisms](../../../../../graph-homomorphism.md) $T\to G$, the support of $\Psi$ has size $N$, so the [maximum entropy distribution on a finite set](../../../../../maximum-entropy-distribution-on-a-finite-set.md) also gives $H(\Psi)\leq\log N$. Thus

$$
N\geq\alpha^{k-1}|X|^r|Y|^s.
$$

There are $|X|^r|Y|^s$ bipartition-respecting maps in total, so a uniformly chosen one is a [graph homomorphism](../../../../../graph-homomorphism.md) with probability at least $\alpha^{k-1}$. This proves the [Sidorenko inequality for trees](../../../../../sidorenko-inequality-for-trees.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 164](../../paper-164-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
