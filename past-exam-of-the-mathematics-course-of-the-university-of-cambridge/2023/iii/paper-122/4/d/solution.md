<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Fix the requested $\varepsilon>0$ and choose much smaller constants $\eta,\delta,\rho>0$ in that order. Apply the [Szemerédi regularity lemma](../../../../../../szemeredi-regularity-lemma.md) with regularity parameter $\rho$ and a sufficiently large lower bound $m_0$ to a largest [triangle-free](../../../../../../triangle-free-graph.md) subgraph $F\subseteq G$. Let

$$
V(G)=V_0\sqcup V_1\sqcup\cdots\sqcup V_m
$$

be the resulting equitable partition, and form the [reduced graph of a regularity partition](../../../../../../reduced-graph-of-a-regularity-partition.md) $R$ on $[m]$ by joining $i$ and $j$ when $(V_i,V_j)$ is $\rho$-uniform in $F$ and has $F$-density at least $\delta$.

Choose $\rho<\delta/2$. If $R$ contained a triangle, the [triangle embedding lemma for regular pairs](../../../../../../triangle-embedding-lemma-for-regular-pairs.md) would give a triangle in $F$. Thus $R$ is triangle-free, and [Turan theorem](../../../../../../turan-s-theorem.md) gives

$$
e(R)\leq\frac{m^2}{4}.
$$

Part (c), with error $\eta$, holds simultaneously for every pair of sets of size at least $n/\log n$. Since $m$ is bounded independently of $n$, all regularity classes and their halves satisfy this size condition for large $n$. It follows that every cross-pair contains at most $(p+\eta)|V_i||V_j|$ edges of $G$. It also gives

$$
e_G(V_i)\leq\frac{p+\eta}{2}|V_i|^2:
$$

take a bipartition of $V_i$ carrying at least half its internal edges and apply the cross-pair estimate.

Now count the edges of $F$. Pairs represented in $R$ contribute at most

$$
(p+\eta)e(R)\left(\frac nm\right)^2
\leq\frac{p+\eta}{4}n^2.
$$

The exceptional set, the at most $\rho m^2$ irregular pairs, pairs of $F$-density below $\delta$, and edges inside classes together contribute at most

$$
O(\rho n^2)+O(\delta n^2)+O(n^2/m_0).
$$

Choose $\eta$, then $\delta,
ho$, and finally $m_0^{-1}$ small enough in terms of $p\varepsilon$. The total is at most

$$
\frac{(1+\varepsilon)pn^2}{4}
$$

[with high probability](../../../../../../with-high-probability.md), as required.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
