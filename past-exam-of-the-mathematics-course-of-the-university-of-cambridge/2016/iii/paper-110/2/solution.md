<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For disjoint nonempty vertex sets $A,B$, write $d(A,B)=e(A,B)/(|A||B|)$. The [regular pair of vertex sets](../../../../../regular-pair-of-vertex-sets.md) $(A,B)$ is $\epsilon$-uniform when every $X\subseteq A$, $Y\subseteq B$ with $|X|\ge\epsilon|A|$ and $|Y|\ge\epsilon|B|$ satisfies

$$
\boxed{|d(X,Y)-d(A,B)|\le\epsilon.}
$$

This is also called an $\epsilon$-regular pair.

**Count transversal [cliques](../../../../../clique-graph-theory.md) by maintaining common neighbourhoods.** For $r=1$ there are exactly $n$ copies, so the claim is immediate. For $r\ge2$ the hypotheses are vacuous if $\lambda>1$; assume $0<\lambda\le1$. Set

$$
a=(\lambda/2)^{r-1},\qquad 0<\eta\le\min\{\lambda/2,a/(2r)\},\qquad \delta_0=(a/2)^r.
$$

After choosing vertices in the first $i-1$ classes, let $C_j\subseteq V_j$ be their common neighbours in each later class. We maintain $|C_j|\ge(\lambda-\eta)^{i-1}n\ge an$. In a regular pair, whenever $|C_j|\ge\eta n$, fewer than $\eta n$ vertices of $V_i$ have fewer than $(d(V_i,V_j)-\eta)|C_j|$ neighbours in $C_j$: otherwise those bad vertices, together with $C_j$, contradict regularity. There are at most $r-1$ future classes, so their union excludes at most $(r-1)\eta n$ candidates from $C_i$. At least $an/2$ choices remain, and each maintains the stated bound for all new common neighbourhoods.

Making these choices through all $r$ classes gives at least $(an/2)^r$ transversal [cliques](../../../../../clique-graph-theory.md). Different selections give different vertex sets, since the classes are disjoint. Consequently

$$
\boxed{\#K_r\ge\delta_0 n^r.}
$$

All constants depend only on $r,\lambda$, not on $n$.

The [Szemerédi regularity lemma](../../../../../szemeredi-regularity-lemma.md) states that for every $\eta>0$ and integer $m_0$ there exist $M,n_0$ such that every [graph](../../../../../graph-split.md) of order $N\ge n_0$ has a partition $V_0,V_1,\ldots,V_k$ with $m_0\le k\le M$, $|V_0|\le\eta N$, equal-sized nonexceptional classes, and at most $\eta k^2$ irregular unordered pairs of classes.

**Apply the partition to prove [clique](../../../../../clique-graph-theory.md) removal.** For $r\ge2$, choose $\lambda=\min\{\epsilon/4,1/2\}$, $m_0\ge\max\{r,4/\epsilon\}$, and a regularity parameter $\eta\le\min\{\epsilon/8,1/2\}$ small enough for the preceding counting argument at density $\lambda$. The [Szemerédi regularity lemma](../../../../../szemeredi-regularity-lemma.md) supplies $M$. Delete all edges incident with $V_0$, inside individual classes, between irregular pairs, and between regular pairs with density below $\lambda$. If the common class size is $L$, the number deleted is at most

$$
\eta N^2+\frac{N^2}{2m_0}+\eta k^2L^2+\frac{\lambda N^2}{2}
\le\left(2\eta+\frac1{2m_0}+\frac\lambda2\right)N^2<\epsilon N^2.
$$

A surviving $K_r$ would have its vertices in distinct classes; every pair of these classes is regular and has density at least $\lambda$. The counting result would then give at least $\delta_0 L^r$ copies in the original [graph](../../../../../graph-split.md). Since $L=(N-|V_0|)/k\ge N/(2M)$, choose, for example,

$$
\delta=\frac{\delta_0}{2(2M)^r}.
$$

This would exceed $\delta N^r$, contradicting the assumed copy count. Thus **fewer than $\delta N^r$ [cliques](../../../../../clique-graph-theory.md) can be destroyed by removing at most $\epsilon N^2$ edges**, leaving no $K_r$. This is the [clique removal lemma](../../../../../clique-removal-lemma.md).

For $r=1$, take $\delta<1$: a [graph](../../../../../graph-split.md) of order $N$ always has $N$ copies of $K_1$, so the hypothesis is impossible. The assertion in that degenerate case is vacuous, rather than an edge-removal procedure capable of deleting vertices.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 110](../../paper-110-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
